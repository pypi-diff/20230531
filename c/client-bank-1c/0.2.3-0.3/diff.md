# Comparing `tmp/client_bank_1c-0.2.3.tar.gz` & `tmp/client_bank_1c-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_bank_1c-0.2.3.tar", max compression
+gzip compressed data, was "client_bank_1c-0.3.tar", max compression
```

## Comparing `client_bank_1c-0.2.3.tar` & `client_bank_1c-0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1057 2023-04-04 23:35:03.689527 client_bank_1c-0.2.3/LICENSE
--rw-r--r--   0        0        0     4487 2023-05-02 07:01:05.507966 client_bank_1c-0.2.3/client_bank_1c.py
--rw-r--r--   0        0        0      888 2023-05-02 07:02:58.819738 client_bank_1c-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 client_bank_1c-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-04-04 23:35:03.689527 client_bank_1c-0.3/LICENSE
+-rw-r--r--   0        0        0     6890 2023-05-31 16:48:52.958992 client_bank_1c-0.3/client_bank_1c.py
+-rw-r--r--   0        0        0      886 2023-05-31 16:49:51.706842 client_bank_1c-0.3/pyproject.toml
+-rw-r--r--   0        0        0     1006 1970-01-01 00:00:00.000000 client_bank_1c-0.3/PKG-INFO
```

### Comparing `client_bank_1c-0.2.3/LICENSE` & `client_bank_1c-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `client_bank_1c-0.2.3/client_bank_1c.py` & `client_bank_1c-0.3/client_bank_1c.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import datetime
 import decimal
 import io
 import re
 from typing import NamedTuple, List
 
+DATE_FORMAT = '%d.%m.%Y'
+TIME_FORMAT = '%H:%M:%S'
+MONEY_FIELDS = {
+    'НачальныйОстаток',
+    'КонечныйОстаток',
+    'ВсегоПоступило',
+    'ВсегоСписано',
+    'Сумма',
+}
+
 
 class ClientBank1CStatement(NamedTuple):
     info: dict
     accounts: List[dict]
     documents: List[dict]
 
 
 class ClientBank1CLoader:
     LINE_REGEXP = re.compile(r'(?P<key>\w+)(?:=(?P<value>.*))?')
-    MONEY_FIELDS = {
-        'НачальныйОстаток',
-        'КонечныйОстаток',
-        'ВсегоПоступило',
-        'ВсегоСписано',
-        'Сумма',
-    }
     NUMBER_FIELDS = {'СрокАкцепта'}
 
     def __init__(self, money_type=decimal.Decimal, result_class=ClientBank1CStatement,
                  fill_collected_fields=False):
         self.money_type = money_type
         self.result_class = result_class
         self.fill_collected_fields = fill_collected_fields
@@ -95,18 +98,18 @@
 
     def _parse_line(self, line):
         key, value = self.LINE_REGEXP.match(line).groups()
         if not value:
             return key, value
 
         if 'Дата' in key:
-            value = datetime.datetime.strptime(value, '%d.%m.%Y').date()
+            value = datetime.datetime.strptime(value, DATE_FORMAT).date()
         elif 'Время' in key:
-            value = datetime.datetime.strptime(value, '%H:%M:%S').time()
-        elif key in self.MONEY_FIELDS:
+            value = datetime.datetime.strptime(value, TIME_FORMAT).time()
+        elif key in MONEY_FIELDS:
             value = self.money_type(value)
         elif key in self.NUMBER_FIELDS:
             value = int(value)
 
         return key, value
 
     def _process_result(self, info, accounts, documents):
@@ -121,18 +124,91 @@
         return info, accounts, documents
 
     @staticmethod
     def _fill_collected_field(document, field_name):
         def get(field_suffix):
             return document.get(field_name + field_suffix)
 
-        field_value = f"ИНН {get('ИНН')}\n{get('1')}\n\nр/с{get('2')}"
+        field_value = f"ИНН {get('ИНН')}\n{get('1')}"
+        if get('2'):
+            field_value += '\n\nр/с ' + get('2')
+
         if get('3'):
             field_value += '\n\nв ' + get('3')
 
         if get('4'):
             field_value += '\n\n' + get('4')
 
         document[field_name] = field_value
 
 
+class ClientBank1CDump:
+    INFO_DEFAULTS = {
+        'ВерсияФормата': '1.03',
+        'Кодировка': 'Windows',
+        'Отправитель': 'Бухгалтерия предприятия, редакция 2.0',
+    }
+
+    EMPTY_VALUES = {False, None}
+
+    def __call__(self, documents, info=None):
+        result = '1CClientBankExchange\n'
+
+        info = self._process_info(info or {})
+
+        for key, value in info.items():
+            result += self._render_line(key, value)
+
+        for document in documents:
+            result += self._render_line('РасчСчет', document['ПлательщикСчет'])
+
+        for document in documents:
+            result += self._render_line('СекцияДокумент', document['ВидДокумента'])
+            for key, value in document.items():
+                if key == 'ВидДокумента':
+                    continue
+                result += self._render_line(key, value)
+            result += 'КонецДокумента\n'
+
+        result += 'КонецФайла\n'
+
+        coding = 'cp1251' if info['Кодировка'] == 'Windows' else 'cp866'
+        return result.encode(coding)
+
+    def _process_info(self, info):
+        info = self._set_defaults(info)
+
+        if 'ДатаСоздания' not in info:
+            now = datetime.datetime.now()
+            info['ДатаСоздания'] = now.today()
+            info['ВремяСоздания'] = now.time()
+
+        coding = info.get('Кодировка')
+        if coding not in {'DOS', 'Windows'}:
+            raise ValueError(f'Incorrect coding: {coding!r}')
+
+        return info
+
+    def _set_defaults(self, info):
+        for key, value in self.INFO_DEFAULTS.items():
+            info.setdefault(key, value)
+        return info
+
+    def _render_line(self, key, value):
+        if value in self.EMPTY_VALUES:
+            value = ''
+
+        if not isinstance(value, str):
+            if key in MONEY_FIELDS:
+                value = format(value, '.2f')
+            elif 'Дата' in key:
+                value = format(value, DATE_FORMAT)
+            elif 'Время' in key:
+                value = format(value, TIME_FORMAT)
+            else:
+                value = str(value)
+
+        return f'{key}={value}\n'
+
+
 load = ClientBank1CLoader()
+dump = ClientBank1CDump()
```

### Comparing `client_bank_1c-0.2.3/pyproject.toml` & `client_bank_1c-0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "client-bank-1c"
-version = "0.2.3"
+version = "0.3"
 description = "1C Client Bank Exchange Format"
 authors = ["Dmitry Voronin <dimka665@gmail.com>"]
 
 repository = "https://github.com/odoo-ru/client-bank-1c"
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `client_bank_1c-0.2.3/PKG-INFO` & `client_bank_1c-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: client-bank-1c
-Version: 0.2.3
+Version: 0.3
 Summary: 1C Client Bank Exchange Format
 Home-page: https://github.com/odoo-ru/client-bank-1c
 License: MIT
 Author: Dmitry Voronin
 Author-email: dimka665@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Intended Audience :: Developers
```

