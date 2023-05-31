# Comparing `tmp/starmerxauth_erp-0.2.3.tar.gz` & `tmp/starmerxauth_erp-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/yf/pippackage/starmerxauth_erp/dist/tmpcxc1i1h5/starmerxauth_erp-0.2.3.tar", last modified: Wed May 31 08:06:53 2023, max compression
+gzip compressed data, was "/home/yf/pippackage/starmerxauth_erp/dist/tmpnhxvybwx/starmerxauth_erp-0.2.4.tar", last modified: Wed May 31 09:09:56 2023, max compression
```

## Comparing `starmerxauth_erp-0.2.3.tar` & `starmerxauth_erp-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/
--rw-rw-r--   0 yf        (1000) yf        (1000)     1053 2022-04-08 06:58:25.000000 starmerxauth_erp-0.2.3/LICENSE
--rw-rw-r--   0 yf        (1000) yf        (1000)      436 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/PKG-INFO
--rw-rw-rw-   0 yf        (1000) yf        (1000)       28 2022-04-28 03:03:21.000000 starmerxauth_erp-0.2.3/README.md
--rw-rw-r--   0 yf        (1000) yf        (1000)       85 2022-04-08 06:37:48.000000 starmerxauth_erp-0.2.3/pyproject.toml
--rw-rw-r--   0 yf        (1000) yf        (1000)      554 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/setup.cfg
-drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/src/
-drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp/
--rw-rw-r--   0 yf        (1000) yf        (1000)       26 2021-02-03 07:45:13.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp/__init__.py
--rw-rw-r--   0 yf        (1000) yf        (1000)     3139 2023-05-31 08:05:35.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp/middleware.py
-drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp.egg-info/
--rw-rw-r--   0 yf        (1000) yf        (1000)      436 2023-05-31 08:06:52.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp.egg-info/PKG-INFO
--rw-rw-r--   0 yf        (1000) yf        (1000)      329 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp.egg-info/SOURCES.txt
--rw-rw-r--   0 yf        (1000) yf        (1000)        1 2023-05-31 08:06:52.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp.egg-info/dependency_links.txt
--rw-rw-r--   0 yf        (1000) yf        (1000)       31 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp.egg-info/requires.txt
--rw-rw-r--   0 yf        (1000) yf        (1000)       17 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp.egg-info/top_level.txt
+drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 09:09:56.000000 starmerxauth_erp-0.2.4/
+-rw-rw-r--   0 yf        (1000) yf        (1000)     1053 2022-04-08 06:58:25.000000 starmerxauth_erp-0.2.4/LICENSE
+-rw-rw-r--   0 yf        (1000) yf        (1000)      436 2023-05-31 09:09:56.000000 starmerxauth_erp-0.2.4/PKG-INFO
+-rw-rw-rw-   0 yf        (1000) yf        (1000)       28 2022-04-28 03:03:21.000000 starmerxauth_erp-0.2.4/README.md
+-rw-rw-r--   0 yf        (1000) yf        (1000)       85 2022-04-08 06:37:48.000000 starmerxauth_erp-0.2.4/pyproject.toml
+-rw-rw-r--   0 yf        (1000) yf        (1000)      554 2023-05-31 09:09:56.000000 starmerxauth_erp-0.2.4/setup.cfg
+drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 09:09:56.000000 starmerxauth_erp-0.2.4/src/
+drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 09:09:56.000000 starmerxauth_erp-0.2.4/src/starmerxauth_erp/
+-rw-rw-r--   0 yf        (1000) yf        (1000)       26 2021-02-03 07:45:13.000000 starmerxauth_erp-0.2.4/src/starmerxauth_erp/__init__.py
+-rw-rw-r--   0 yf        (1000) yf        (1000)     3147 2023-05-31 09:09:16.000000 starmerxauth_erp-0.2.4/src/starmerxauth_erp/middleware.py
+drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 09:09:56.000000 starmerxauth_erp-0.2.4/src/starmerxauth_erp.egg-info/
+-rw-rw-r--   0 yf        (1000) yf        (1000)      436 2023-05-31 09:09:55.000000 starmerxauth_erp-0.2.4/src/starmerxauth_erp.egg-info/PKG-INFO
+-rw-rw-r--   0 yf        (1000) yf        (1000)      329 2023-05-31 09:09:55.000000 starmerxauth_erp-0.2.4/src/starmerxauth_erp.egg-info/SOURCES.txt
+-rw-rw-r--   0 yf        (1000) yf        (1000)        1 2023-05-31 09:09:55.000000 starmerxauth_erp-0.2.4/src/starmerxauth_erp.egg-info/dependency_links.txt
+-rw-rw-r--   0 yf        (1000) yf        (1000)       31 2023-05-31 09:09:55.000000 starmerxauth_erp-0.2.4/src/starmerxauth_erp.egg-info/requires.txt
+-rw-rw-r--   0 yf        (1000) yf        (1000)       17 2023-05-31 09:09:55.000000 starmerxauth_erp-0.2.4/src/starmerxauth_erp.egg-info/top_level.txt
```

### Comparing `starmerxauth_erp-0.2.3/LICENSE` & `starmerxauth_erp-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starmerxauth_erp-0.2.3/setup.cfg` & `starmerxauth_erp-0.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = starmerxauth_erp
-version = 0.2.3
+version = 0.2.4
 author = yang
 author_email = yangjuan@starmerx.com
 description = starmerx verify jwt in erp
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python
```

### Comparing `starmerxauth_erp-0.2.3/src/starmerxauth_erp/middleware.py` & `starmerxauth_erp-0.2.4/src/starmerxauth_erp/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         except:
             logger.info('verify jwt error:token:' + token)
             return AnonymousUser()
         username = payload.get('username')
         try:
             user = User.objects.get(partner__name=username)
             if user:
-                logger.info('verify jwt:' + str(user.username))
+                logger.info('verify jwt:' + str(user.partner.username))
                 return user
         except:
             logger.info('verify jwt fail:username:' + str(username))
         return AnonymousUser()
 
     def verify_token(self, token):
         """
```

