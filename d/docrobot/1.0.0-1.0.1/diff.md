# Comparing `tmp/docrobot-1.0.0.tar.gz` & `tmp/docrobot-1.0.1.tar.gz`

## Comparing `docrobot-1.0.0.tar` & `docrobot-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 docrobot-1.0.0/convert.ps1
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 docrobot-1.0.0/requirements.txt
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 docrobot-1.0.0/src/docrobot/form.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 docrobot-1.0.0/src/docrobot/form.ui
--rw-r--r--   0        0        0    10765 2020-02-02 00:00:00.000000 docrobot-1.0.0/src/docrobot/guimain.pyw
--rw-r--r--   0        0        0    11188 2020-02-02 00:00:00.000000 docrobot-1.0.0/src/docrobot/main.py
--rw-r--r--   0        0        0    27599 2020-02-02 00:00:00.000000 docrobot-1.0.0/temple/logo.png
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 docrobot-1.0.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 docrobot-1.0.0/LICENSE
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 docrobot-1.0.0/README.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 docrobot-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 docrobot-1.0.1/convert.ps1
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 docrobot-1.0.1/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.1/src/docrobot/__init__.py
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 docrobot-1.0.1/src/docrobot/form.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 docrobot-1.0.1/src/docrobot/form.ui
+-rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 docrobot-1.0.1/src/docrobot/guimain.pyw
+-rw-r--r--   0        0        0    11203 2020-02-02 00:00:00.000000 docrobot-1.0.1/src/docrobot/util.py
+-rw-r--r--   0        0        0    27599 2020-02-02 00:00:00.000000 docrobot-1.0.1/temple/logo.png
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 docrobot-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 docrobot-1.0.1/LICENSE
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 docrobot-1.0.1/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 docrobot-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 docrobot-1.0.1/PKG-INFO
```

### Comparing `docrobot-1.0.0/src/docrobot/form.py` & `docrobot-1.0.1/src/docrobot/form.py`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.0/src/docrobot/form.ui` & `docrobot-1.0.1/src/docrobot/form.ui`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.0/src/docrobot/guimain.pyw` & `docrobot-1.0.1/src/docrobot/guimain.pyw`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import os
 import re
 import sys
-from configparser import ConfigParser, DuplicateSectionError
+from configparser import ConfigParser
 
 from PySide6 import QtCore
 from PySide6.QtCore import QEventLoop, QTimer
-from PySide6.QtGui import QTextCursor
 from PySide6.QtWidgets import QApplication, QMainWindow, QFileDialog
 from docx import Document
 from docx.opc.exceptions import PackageNotFoundError
 from openpyxl.reader.excel import load_workbook
 from win32com.client import Dispatch
 
-import main
-from form import Ui_MainWindow
+from docrobot import util
+from docrobot.form import Ui_MainWindow
 
 
 class EmittingStr(QtCore.QObject):
     textWritten = QtCore.Signal(str)
 
     def write(self, text):
         self.textWritten.emit(str(text))
@@ -48,18 +47,19 @@
         self.actionreplace.triggered.connect(lambda: self.replaceprj(True))
         self.actioncheckall.triggered.connect(self.checkall)
 
         self.config = ConfigParser()
         try:
             self.config.read('config.ini', encoding='UTF-8')
             self.workdir = self.config['config']['lasting']
-            self.onchangeworkdir()
+        except KeyError:
             self.config.add_section('config')
-        except DuplicateSectionError:
-            pass
+        try:
+            if self.workdir != '':
+                self.onchangeworkdir()
         except FileNotFoundError as e:
             self.textEdit.append('路径错误：' + e.filename)
             self.workdir = ''
         self.lineEdit.setText(self.workdir)
 
     def outputWritten(self, text):
         # cursor = self.textEdit.textCursor()
@@ -102,18 +102,18 @@
             doc_name = ''
             try:
                 doc_name = self.workdir + '/RD' + project.p_order + project.p_name + '.docx'
                 document = Document(doc_name)
                 # debug_doc(document)
                 # TODO to be fixed
                 # replace_header(document)
-                match = match + main.first_table(document, project)
-                match = match + main.start_time(document, project)
-                match = match + main.second_table(document, project)
-                match = match + main.third_table(document, project)
+                match = match + util.first_table(document, project)
+                match = match + util.start_time(document, project)
+                match = match + util.second_table(document, project)
+                match = match + util.third_table(document, project)
 
                 match = match + self.checkpat2(document, project)
 
                 if modify:
                     document.save(doc_name)
             except PackageNotFoundError:
                 self.textEdit.append('Error打开文件错误：' + doc_name)
@@ -224,15 +224,15 @@
         else:
             print("Error: 找不到 公司名")
         max_row_num = ws.max_row
         range_cell = ws[f'A3:P{max_row_num}']
         for r in range_cell:
             if r[0].value is None:
                 break
-            project = main.Project()
+            project = util.Project()
             project.p_comname = com_name
             project.p_order = str(r[0].value).strip().zfill(2)
             project.p_name = str(r[1].value).strip()  # 项目名称
             project.p_start = r[2].value.strftime('%Y-%m-%d')
             project.p_end = r[3].value.strftime('%Y-%m-%d')
             project.p_cost = str(r[5].value).strip()
             project.p_people = str(r[6].value).strip()  # 人数
```

### Comparing `docrobot-1.0.0/src/docrobot/main.py` & `docrobot-1.0.1/src/docrobot/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,16 @@
             for m, cell in enumerate(row.cells):
                 for i, para in enumerate(cell.paragraphs):
                     print(f'Table.{k} Row.{l} Cell{m} Para.{i} : ', para.text, sep='')
                     # for j, run in enumerate(para.runs):
                     #     print(f'Para.{i} Run{j}: ', run.text, sep='')
 
 
-def replace_header(doc):
-    check_replace(doc.sections[0].header.paragraphs, '.*公司', com_name)
+def replace_header(doc, prj):
+    check_replace(doc.sections[0].header.paragraphs, '.*公司', prj.com_name)
 
 
 def first_table(doc, prj):
     match = 0
     if doc.tables[0].rows[0].cells[0].paragraphs[0].text == '项目名称：':
         doc.tables[0].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
         clear_runs(doc.tables[0].rows[0].cells[1].paragraphs[0].runs)
@@ -246,11 +246,11 @@
             print(Fore.RED + '打开文件错误：' + doc_name)
 
     #         document = replace_header(document, company)
     #         document = check_and_change(document, replace_dict)
     #         document = replace_tables(document, replace_dict)
 
     if workdir_change:
-        with open('config.ini', 'w', encoding='utf-8') as file:
+        with open('../../config.ini', 'w', encoding='utf-8') as file:
             config = ConfigParser()
             config.write(file)  # 数据写入配置文件
     input("处理完成.")
```

### Comparing `docrobot-1.0.0/temple/logo.png` & `docrobot-1.0.1/temple/logo.png`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.0/LICENSE` & `docrobot-1.0.1/LICENSE`

 * *Files identical despite different names*

