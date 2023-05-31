# Comparing `tmp/docrobot-1.0.1.tar.gz` & `tmp/docrobot-1.0.2.tar.gz`

## Comparing `docrobot-1.0.1.tar` & `docrobot-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 docrobot-1.0.1/convert.ps1
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 docrobot-1.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.1/src/docrobot/__init__.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 docrobot-1.0.1/src/docrobot/form.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 docrobot-1.0.1/src/docrobot/form.ui
--rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 docrobot-1.0.1/src/docrobot/guimain.pyw
--rw-r--r--   0        0        0    11203 2020-02-02 00:00:00.000000 docrobot-1.0.1/src/docrobot/util.py
--rw-r--r--   0        0        0    27599 2020-02-02 00:00:00.000000 docrobot-1.0.1/temple/logo.png
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 docrobot-1.0.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 docrobot-1.0.1/LICENSE
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 docrobot-1.0.1/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 docrobot-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 docrobot-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 docrobot-1.0.2/convert.ps1
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 docrobot-1.0.2/requirements.txt
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 docrobot-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.2/src/docrobot/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 docrobot-1.0.2/src/docrobot/config.ini
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 docrobot-1.0.2/src/docrobot/form.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 docrobot-1.0.2/src/docrobot/form.ui
+-rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 docrobot-1.0.2/src/docrobot/guimain.pyw
+-rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 docrobot-1.0.2/src/docrobot/util.py
+-rw-r--r--   0        0        0    27599 2020-02-02 00:00:00.000000 docrobot-1.0.2/temple/logo.png
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 docrobot-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 docrobot-1.0.2/LICENSE
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 docrobot-1.0.2/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 docrobot-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 docrobot-1.0.2/PKG-INFO
```

### Comparing `docrobot-1.0.1/src/docrobot/form.py` & `docrobot-1.0.2/src/docrobot/form.py`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.1/src/docrobot/form.ui` & `docrobot-1.0.2/src/docrobot/form.ui`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.1/src/docrobot/guimain.pyw` & `docrobot-1.0.2/src/docrobot/guimain.pyw`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.1/src/docrobot/util.py` & `docrobot-1.0.2/src/docrobot/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,18 +116,18 @@
     match = match + check_replace(doc.tables[1].rows[1].cells[1].paragraphs
                                   , '项目团队由(.*)人组成，项目实施周期为(.*)个月。'
                                   , '项目团队由' + prj.p_people + '人组成，项目实施周期为' + prj.p_cost + '个月。')
     match = match + check_replace(doc.tables[1].rows[6].cells[1].paragraphs
                                   , '\d{4}[-/]\d{1,2}[-/]\d{1,2}至\d{4}[-/]\d{1,2}[-/]\d{1,2}',
                                   prj.p_start + '至' + prj.p_end)
     match = match + check_replace(doc.tables[1].rows[7].cells[1].paragraphs
-                                  , '项目总资金预算\d+万元', '项目总资金预算' + prj.p_money + '万元')
+                                  , '项目总资金预算.*万元', '项目总资金预算' + prj.p_money + '万元')
 
     match = match + check_replace(doc.tables[1].rows[8].cells[1].paragraphs
-                                  , '项目总人数：\d+人', '项目总人数：' + prj.p_people + '人')
+                                  , '项目总人数：.*人', '项目总人数：' + prj.p_people + '人')
     if prj.p_owner != 'None':
         match = match + check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '项目负责人：.*',
                                       '项目负责人：' + prj.p_owner)
     if prj.p_rnd != 'None':
         match = match + check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '研发成员：.*', '研发成员：' + prj.p_rnd)
     match = match + check_replace(doc.tables[1].rows[9].cells[1].paragraphs, '\d{4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_start)
```

### Comparing `docrobot-1.0.1/temple/logo.png` & `docrobot-1.0.2/temple/logo.png`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.1/LICENSE` & `docrobot-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.1/pyproject.toml` & `docrobot-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "docrobot"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Xu Hong", email="icehong@gmail.com" },
 ]
 description = "一个文档自动化处理工具"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `docrobot-1.0.1/PKG-INFO` & `docrobot-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrobot
-Version: 1.0.1
+Version: 1.0.2
 Summary: 一个文档自动化处理工具
 Project-URL: Homepage, https://github.com/icehong/docrobot
 Project-URL: Bug Tracker, https://github.com/icehong/docrobot/issues
 Author-email: Xu Hong <icehong@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -16,15 +16,15 @@
 Requires-Dist: pywin32
 Description-Content-Type: text/markdown
 
 # 一个文档自动处理工具
 
 暂时没有啥说明
 
-安装:  pip install docrobot
+安装:  pip install docrobot  
 升级： pip install --upgrade docrobot
 
 然后找到
 
 构建环境准备:
 python -m pip install -U pip setuptools
 pip install pywin32 colorama python-docx openpyxl pyside6 -i https://mirrors.aliyun.com/pypi/simple/ --trusted-host mirrors.aliyun.com
```

