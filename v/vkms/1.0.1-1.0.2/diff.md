# Comparing `tmp/vkms-1.0.1.tar.gz` & `tmp/vkms-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vkms-1.0.1.tar", last modified: Mon Mar 13 15:55:06 2023, max compression
+gzip compressed data, was "vkms-1.0.2.tar", last modified: Wed May 31 08:51:01 2023, max compression
```

## Comparing `vkms-1.0.1.tar` & `vkms-1.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:55:06.730459 vkms-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-13 15:54:58.000000 vkms-1.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:55:06.726459 vkms-1.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-13 15:54:58.000000 vkms-1.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:55:06.726459 vkms-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-13 15:54:58.000000 vkms-1.0.1/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-13 15:54:58.000000 vkms-1.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-13 15:54:58.000000 vkms-1.0.1/.github/workflows/stats.yml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-13 15:54:58.000000 vkms-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-13 15:54:58.000000 vkms-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-03-13 15:54:58.000000 vkms-1.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-13 15:54:58.000000 vkms-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-03-13 15:55:06.730459 vkms-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-13 15:54:58.000000 vkms-1.0.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       84 2023-03-13 15:54:58.000000 vkms-1.0.1/VK-MS.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:55:06.726459 vkms-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-03-13 15:54:58.000000 vkms-1.0.1/docs/DOCS.md
--rw-r--r--   0 runner    (1001) docker     (123)    68137 2023-03-13 15:54:58.000000 vkms-1.0.1/docs/html_saver_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-03-13 15:54:58.000000 vkms-1.0.1/docs/txt_saver_example.png
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-13 15:54:58.000000 vkms-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 15:55:06.730459 vkms-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:55:06.730459 vkms-1.0.1/vkms/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-13 15:54:58.000000 vkms-1.0.1/vkms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-03-13 15:54:58.000000 vkms-1.0.1/vkms/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-03-13 15:54:58.000000 vkms-1.0.1/vkms/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-03-13 15:54:58.000000 vkms-1.0.1/vkms/attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-13 15:54:58.000000 vkms-1.0.1/vkms/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-13 15:54:58.000000 vkms-1.0.1/vkms/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-03-13 15:54:58.000000 vkms-1.0.1/vkms/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-03-13 15:54:58.000000 vkms-1.0.1/vkms/peers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-03-13 15:54:58.000000 vkms-1.0.1/vkms/saver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:55:06.730459 vkms-1.0.1/vkms/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    49364 2023-03-13 15:54:58.000000 vkms-1.0.1/vkms/templates/peer.html
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-03-13 15:54:58.000000 vkms-1.0.1/vkms/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-13 15:54:58.000000 vkms-1.0.1/vkms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-13 15:55:06.000000 vkms-1.0.1/vkms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 15:55:06.730459 vkms-1.0.1/vkms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-03-13 15:55:06.000000 vkms-1.0.1/vkms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-13 15:55:06.000000 vkms-1.0.1/vkms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 15:55:06.000000 vkms-1.0.1/vkms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-13 15:55:06.000000 vkms-1.0.1/vkms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-13 15:55:06.000000 vkms-1.0.1/vkms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-13 15:55:06.000000 vkms-1.0.1/vkms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:51:01.551185 vkms-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 08:50:53.000000 vkms-1.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:51:01.547185 vkms-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-31 08:50:53.000000 vkms-1.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:51:01.547185 vkms-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-31 08:50:53.000000 vkms-1.0.2/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-31 08:50:53.000000 vkms-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-31 08:50:53.000000 vkms-1.0.2/.github/workflows/stats.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-31 08:50:53.000000 vkms-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-31 08:50:53.000000 vkms-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-31 08:50:53.000000 vkms-1.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 08:50:53.000000 vkms-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-31 08:51:01.551185 vkms-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-31 08:50:53.000000 vkms-1.0.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       84 2023-05-31 08:50:53.000000 vkms-1.0.2/VK-MS.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:51:01.547185 vkms-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-05-31 08:50:53.000000 vkms-1.0.2/docs/DOCS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    68137 2023-05-31 08:50:53.000000 vkms-1.0.2/docs/html_saver_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-05-31 08:50:53.000000 vkms-1.0.2/docs/txt_saver_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-31 08:50:53.000000 vkms-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 08:51:01.551185 vkms-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:51:01.551185 vkms-1.0.2/vkms/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 08:50:53.000000 vkms-1.0.2/vkms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-05-31 08:50:53.000000 vkms-1.0.2/vkms/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-31 08:50:53.000000 vkms-1.0.2/vkms/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-05-31 08:50:53.000000 vkms-1.0.2/vkms/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-31 08:50:53.000000 vkms-1.0.2/vkms/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 08:50:53.000000 vkms-1.0.2/vkms/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-31 08:50:53.000000 vkms-1.0.2/vkms/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-31 08:50:53.000000 vkms-1.0.2/vkms/peers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-31 08:50:53.000000 vkms-1.0.2/vkms/saver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:51:01.551185 vkms-1.0.2/vkms/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    49364 2023-05-31 08:50:53.000000 vkms-1.0.2/vkms/templates/peer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-31 08:50:53.000000 vkms-1.0.2/vkms/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-31 08:50:53.000000 vkms-1.0.2/vkms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 08:51:01.000000 vkms-1.0.2/vkms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:51:01.551185 vkms-1.0.2/vkms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-31 08:51:01.000000 vkms-1.0.2/vkms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-31 08:51:01.000000 vkms-1.0.2/vkms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:51:01.000000 vkms-1.0.2/vkms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 08:51:01.000000 vkms-1.0.2/vkms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-31 08:51:01.000000 vkms-1.0.2/vkms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 08:51:01.000000 vkms-1.0.2/vkms.egg-info/top_level.txt
```

### Comparing `vkms-1.0.1/.github/workflows/check.yml` & `vkms-1.0.2/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/.github/workflows/release.yml` & `vkms-1.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/.github/workflows/stats.yml` & `vkms-1.0.2/.github/workflows/stats.yml`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/.pre-commit-config.yaml` & `vkms-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/CHANGELOG.md` & `vkms-1.0.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # vk-messages-saver | Changelog
 
 ## [Unreleased]
+#### Fixed
+- Исправлен баг с бесконечным циклом в `peers.py` при количестве переписок > 200
+- Исправлен баг с обработкой сообщений с идентификатором отправителя 0
 
 ## [1.0.1] - 2023-03-13
 #### Fixed
 - Исправлен баг с кодировками записываемых файлов (на Windows появляется ошибка *UnicodeEncodeError*)
 - Исправлен баг с локалями месяцов при генерации дат `msg.full_date()`
 - Исправлен баг с загрузкой диалога, состоящего из сообщений только одного участника
```

### Comparing `vkms-1.0.1/LICENSE` & `vkms-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/PKG-INFO` & `vkms-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkms
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utility for saving messages from the VK social network
 Author-email: Yaroslav Kikel <yaroslav.kikel.06@inbox.ru>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/YariKartoshe4ka/vk-messages-saver
 Keywords: api,parser,vk,messages,saver
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vkms Version: 1.0.1 Summary: Utility for saving
+Metadata-Version: 2.1 Name: vkms Version: 1.0.2 Summary: Utility for saving
 messages from the VK social network Author-email: Yaroslav Kikel
 kikel.06@inbox.ru> License: GPL-3.0-only Project-URL: Homepage, https://
 github.com/YariKartoshe4ka/vk-messages-saver Keywords:
 api,parser,vk,messages,saver Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `vkms-1.0.1/README.md` & `vkms-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/docs/DOCS.md` & `vkms-1.0.2/docs/DOCS.md`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/docs/html_saver_example.png` & `vkms-1.0.2/docs/html_saver_example.png`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/docs/txt_saver_example.png` & `vkms-1.0.2/docs/txt_saver_example.png`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/pyproject.toml` & `vkms-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "vkms"
 description = "Utility for saving messages from the VK social network"
 license = { text = "GPL-3.0-only" }
 authors = [
     { name = "Yaroslav Kikel", email = "yaroslav.kikel.06@inbox.ru"}
 ]
 dependencies = [
-    "pathvalidate<3,>=2.5",
+    "pathvalidate>=2.5,<4",
     "requests<3,>=2.24",
     "Jinja2<4,>=3.1",
     "minify-html<1,>=0.8",
     "vk<4,>=3.0",
     "SQLAlchemy>=1.4,<3"
 ]
 urls.Homepage = "https://github.com/YariKartoshe4ka/vk-messages-saver"
```

### Comparing `vkms-1.0.1/vkms/actions.py` & `vkms-1.0.2/vkms/actions.py`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/vkms/argparser.py` & `vkms-1.0.2/vkms/argparser.py`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/vkms/attachments.py` & `vkms-1.0.2/vkms/attachments.py`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/vkms/database.py` & `vkms-1.0.2/vkms/database.py`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/vkms/main.py` & `vkms-1.0.2/vkms/main.py`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/vkms/messages.py` & `vkms-1.0.2/vkms/messages.py`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/vkms/peers.py` & `vkms-1.0.2/vkms/peers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     processed = len(peers)
 
     # Повторяем действия выше, пока все переписки не будут загружены
     while processed < res['count']:
         res = api.messages.getConversations(offset=processed, count=200)
         peers += [item['conversation'] for item in res['items']]
+        processed += 200
 
     return peers
 
 
 def export_json(out_dir, session):
     """
     Экспортирует данные из SQLite в немного модифицированный JSON
@@ -67,14 +68,15 @@
     """
 
     def __init__(self, session):
         # Загружаем и сохраняем информацию о переписке из JSON
         self.account, self.info = session.query(db.Peer.account, db.Peer.info).one()
 
         usernames = users.parse(session)
+        usernames[0] = self.account
 
         # Парсим все сообщения переписки
         self.msgs = messages.MessagesFactory(session, usernames).parse()
 
         # Сохраняем название переписки
         if self.info['peer']['type'] == 'chat':
             self.title = self.info['chat_settings']['title']
```

### Comparing `vkms-1.0.1/vkms/saver.py` & `vkms-1.0.2/vkms/saver.py`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/vkms/templates/peer.html` & `vkms-1.0.2/vkms/templates/peer.html`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/vkms/users.py` & `vkms-1.0.2/vkms/users.py`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/vkms/utils.py` & `vkms-1.0.2/vkms/utils.py`

 * *Files identical despite different names*

### Comparing `vkms-1.0.1/vkms.egg-info/PKG-INFO` & `vkms-1.0.2/vkms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkms
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utility for saving messages from the VK social network
 Author-email: Yaroslav Kikel <yaroslav.kikel.06@inbox.ru>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/YariKartoshe4ka/vk-messages-saver
 Keywords: api,parser,vk,messages,saver
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vkms Version: 1.0.1 Summary: Utility for saving
+Metadata-Version: 2.1 Name: vkms Version: 1.0.2 Summary: Utility for saving
 messages from the VK social network Author-email: Yaroslav Kikel
 kikel.06@inbox.ru> License: GPL-3.0-only Project-URL: Homepage, https://
 github.com/YariKartoshe4ka/vk-messages-saver Keywords:
 api,parser,vk,messages,saver Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `vkms-1.0.1/vkms.egg-info/SOURCES.txt` & `vkms-1.0.2/vkms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

