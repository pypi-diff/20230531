# Comparing `tmp/starmerxauth_erp-0.2.2.tar.gz` & `tmp/starmerxauth_erp-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/yf/pippackage/starmerxauth_erp/dist/tmp7nwgiutn/starmerxauth_erp-0.2.2.tar", last modified: Wed May 31 07:37:33 2023, max compression
+gzip compressed data, was "/home/yf/pippackage/starmerxauth_erp/dist/tmpcxc1i1h5/starmerxauth_erp-0.2.3.tar", last modified: Wed May 31 08:06:53 2023, max compression
```

## Comparing `starmerxauth_erp-0.2.2.tar` & `starmerxauth_erp-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/
--rw-rw-r--   0 yf        (1000) yf        (1000)     1053 2022-04-08 06:58:25.000000 starmerxauth_erp-0.2.2/LICENSE
--rw-rw-r--   0 yf        (1000) yf        (1000)      436 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/PKG-INFO
--rw-rw-rw-   0 yf        (1000) yf        (1000)       28 2022-04-28 03:03:21.000000 starmerxauth_erp-0.2.2/README.md
--rw-rw-r--   0 yf        (1000) yf        (1000)       85 2022-04-08 06:37:48.000000 starmerxauth_erp-0.2.2/pyproject.toml
--rw-rw-r--   0 yf        (1000) yf        (1000)      554 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/setup.cfg
-drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/src/
-drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp/
--rw-rw-r--   0 yf        (1000) yf        (1000)       26 2021-02-03 07:45:13.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp/__init__.py
--rw-rw-r--   0 yf        (1000) yf        (1000)     3055 2022-06-15 05:59:46.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp/middleware.py
-drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp.egg-info/
--rw-rw-r--   0 yf        (1000) yf        (1000)      436 2023-05-31 07:37:32.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp.egg-info/PKG-INFO
--rw-rw-r--   0 yf        (1000) yf        (1000)      329 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp.egg-info/SOURCES.txt
--rw-rw-r--   0 yf        (1000) yf        (1000)        1 2023-05-31 07:37:32.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp.egg-info/dependency_links.txt
--rw-rw-r--   0 yf        (1000) yf        (1000)       31 2023-05-31 07:37:32.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp.egg-info/requires.txt
--rw-rw-r--   0 yf        (1000) yf        (1000)       17 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp.egg-info/top_level.txt
+drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/
+-rw-rw-r--   0 yf        (1000) yf        (1000)     1053 2022-04-08 06:58:25.000000 starmerxauth_erp-0.2.3/LICENSE
+-rw-rw-r--   0 yf        (1000) yf        (1000)      436 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/PKG-INFO
+-rw-rw-rw-   0 yf        (1000) yf        (1000)       28 2022-04-28 03:03:21.000000 starmerxauth_erp-0.2.3/README.md
+-rw-rw-r--   0 yf        (1000) yf        (1000)       85 2022-04-08 06:37:48.000000 starmerxauth_erp-0.2.3/pyproject.toml
+-rw-rw-r--   0 yf        (1000) yf        (1000)      554 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/setup.cfg
+drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/src/
+drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp/
+-rw-rw-r--   0 yf        (1000) yf        (1000)       26 2021-02-03 07:45:13.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp/__init__.py
+-rw-rw-r--   0 yf        (1000) yf        (1000)     3139 2023-05-31 08:05:35.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp/middleware.py
+drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp.egg-info/
+-rw-rw-r--   0 yf        (1000) yf        (1000)      436 2023-05-31 08:06:52.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp.egg-info/PKG-INFO
+-rw-rw-r--   0 yf        (1000) yf        (1000)      329 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp.egg-info/SOURCES.txt
+-rw-rw-r--   0 yf        (1000) yf        (1000)        1 2023-05-31 08:06:52.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp.egg-info/dependency_links.txt
+-rw-rw-r--   0 yf        (1000) yf        (1000)       31 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp.egg-info/requires.txt
+-rw-rw-r--   0 yf        (1000) yf        (1000)       17 2023-05-31 08:06:53.000000 starmerxauth_erp-0.2.3/src/starmerxauth_erp.egg-info/top_level.txt
```

### Comparing `starmerxauth_erp-0.2.2/LICENSE` & `starmerxauth_erp-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `starmerxauth_erp-0.2.2/setup.cfg` & `starmerxauth_erp-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = starmerxauth_erp
-version = 0.2.2
+version = 0.2.3
 author = yang
 author_email = yangjuan@starmerx.com
 description = starmerx verify jwt in erp
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python
```

### Comparing `starmerxauth_erp-0.2.2/src/starmerxauth_erp/middleware.py` & `starmerxauth_erp-0.2.3/src/starmerxauth_erp/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,19 @@
             raise Exception("please config LOGIN_URL and LOGOUT_URL")
         if request.path != settings.LOGIN_URL and request.path != settings.LOGOUT_URL:
             jwt_user = SimpleLazyObject(lambda: self.get_jwt_user(request))
             jwt_test = str(request.COOKIES.get('test'))
             if jwt_test == '1':
                 logger.info('test=1,use jwt user:' + str(jwt_user.username))
                 request._user = jwt_user
+                request.user = jwt_user
             else:
                 if not isinstance(jwt_user, AnonymousUser):
                     request._user = jwt_user
+                    request.user = jwt_user
 
     def get_jwt_user(self, request):
         token = request.META.get("HTTP_JWTAUTHORIZATION")
         if not token:
             return AnonymousUser()
         try:
             payload = self.verify_token(token[7:])
```

