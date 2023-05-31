# Comparing `tmp/pyndjs-0.0.4.tar.gz` & `tmp/pyndjs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyndjs-0.0.4.tar", last modified: Wed May 31 07:07:33 2023, max compression
+gzip compressed data, was "pyndjs-0.0.5.tar", last modified: Wed May 31 07:10:09 2023, max compression
```

## Comparing `pyndjs-0.0.4.tar` & `pyndjs-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 07:07:33.795314 pyndjs-0.0.4/
--rw-rw-rw-   0        0        0       72 2023-05-31 07:07:33.794314 pyndjs-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-31 07:07:33.788206 pyndjs-0.0.4/pyndjs/
--rw-rw-rw-   0        0        0       52 2023-02-08 08:23:02.000000 pyndjs-0.0.4/pyndjs/__init__.py
--rw-rw-rw-   0        0        0     6111 2023-02-09 01:10:26.000000 pyndjs-0.0.4/pyndjs/pyndjs.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:07:33.793314 pyndjs-0.0.4/pyndjs.egg-info/
--rw-rw-rw-   0        0        0       72 2023-05-31 07:07:33.000000 pyndjs-0.0.4/pyndjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-05-31 07:07:33.000000 pyndjs-0.0.4/pyndjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 07:07:33.000000 pyndjs-0.0.4/pyndjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-31 07:07:33.000000 pyndjs-0.0.4/pyndjs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 07:07:33.000000 pyndjs-0.0.4/pyndjs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 07:07:33.795314 pyndjs-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      275 2023-05-31 07:06:54.000000 pyndjs-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:10:09.752204 pyndjs-0.0.5/
+-rw-rw-rw-   0        0        0      160 2023-05-31 07:10:09.751198 pyndjs-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 07:10:09.743882 pyndjs-0.0.5/pyndjs/
+-rw-rw-rw-   0        0        0       52 2023-02-08 08:23:02.000000 pyndjs-0.0.5/pyndjs/__init__.py
+-rw-rw-rw-   0        0        0     6103 2023-05-31 07:09:59.000000 pyndjs-0.0.5/pyndjs/pyndjs.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:10:09.750084 pyndjs-0.0.5/pyndjs.egg-info/
+-rw-rw-rw-   0        0        0      160 2023-05-31 07:10:09.000000 pyndjs-0.0.5/pyndjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-05-31 07:10:09.000000 pyndjs-0.0.5/pyndjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:10:09.000000 pyndjs-0.0.5/pyndjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-31 07:10:09.000000 pyndjs-0.0.5/pyndjs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 07:10:09.000000 pyndjs-0.0.5/pyndjs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:10:09.752204 pyndjs-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      275 2023-05-31 07:09:59.000000 pyndjs-0.0.5/setup.py
```

### Comparing `pyndjs-0.0.4/pyndjs/pyndjs.py` & `pyndjs-0.0.5/pyndjs/pyndjs.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,8 +70,8 @@
     if stdoutdata == "":
         return stderrdata.strip()
     else:
         stdoutdata = json.loads(stdoutdata)
         if len(stdoutdata)<2:
             print('\033[3;31m函数可能没有使用return返回执行结果！\033[m')
             return ''
-    return json.loads(stdoutdata)[-1]
+        return stdoutdata[-1]
```

