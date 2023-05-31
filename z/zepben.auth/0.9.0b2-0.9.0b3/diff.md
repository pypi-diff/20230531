# Comparing `tmp/zepben.auth-0.9.0b2-py3-none-any.whl.zip` & `tmp/zepben.auth-0.9.0b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11500 bytes, number of entries: 9
--rw-r--r--  2.0 unx      246 b- defN 22-Apr-14 05:48 zepben/auth/__init__.py
--rw-r--r--  2.0 unx      416 b- defN 22-Apr-14 05:48 zepben/auth/client/__init__.py
--rw-r--r--  2.0 unx     8712 b- defN 22-Apr-14 05:48 zepben/auth/client/token_fetcher.py
--rw-r--r--  2.0 unx      449 b- defN 22-Apr-14 05:48 zepben/auth/client/util.py
--rw-r--r--  2.0 unx    16725 b- defN 22-Apr-14 05:49 zepben.auth-0.9.0b2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1551 b- defN 22-Apr-14 05:49 zepben.auth-0.9.0b2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Apr-14 05:49 zepben.auth-0.9.0b2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 22-Apr-14 05:49 zepben.auth-0.9.0b2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      755 b- defN 22-Apr-14 05:49 zepben.auth-0.9.0b2.dist-info/RECORD
-9 files, 28953 bytes uncompressed, 10188 bytes compressed:  64.8%
+Zip file size: 11508 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      246 b- defN 22-Apr-20 05:13 zepben/auth/__init__.py
+-rw-r--r--  2.0 unx      416 b- defN 22-Apr-20 05:13 zepben/auth/client/__init__.py
+-rw-r--r--  2.0 unx     8717 b- defN 22-Apr-20 05:13 zepben/auth/client/token_fetcher.py
+-rw-r--r--  2.0 unx      449 b- defN 22-Apr-20 05:13 zepben/auth/client/util.py
+-rw-r--r--  2.0 unx    16725 b- defN 22-Apr-20 05:14 zepben.auth-0.9.0b3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1551 b- defN 22-Apr-20 05:14 zepben.auth-0.9.0b3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Apr-20 05:14 zepben.auth-0.9.0b3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 22-Apr-20 05:14 zepben.auth-0.9.0b3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      755 b- defN 22-Apr-20 05:14 zepben.auth-0.9.0b3.dist-info/RECORD
+9 files, 28958 bytes uncompressed, 10196 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: zepben/auth/client/token_fetcher.py
 Comment: 
 
 Filename: zepben/auth/client/util.py
 Comment: 
 
-Filename: zepben.auth-0.9.0b2.dist-info/LICENSE
+Filename: zepben.auth-0.9.0b3.dist-info/LICENSE
 Comment: 
 
-Filename: zepben.auth-0.9.0b2.dist-info/METADATA
+Filename: zepben.auth-0.9.0b3.dist-info/METADATA
 Comment: 
 
-Filename: zepben.auth-0.9.0b2.dist-info/WHEEL
+Filename: zepben.auth-0.9.0b3.dist-info/WHEEL
 Comment: 
 
-Filename: zepben.auth-0.9.0b2.dist-info/top_level.txt
+Filename: zepben.auth-0.9.0b3.dist-info/top_level.txt
 Comment: 
 
-Filename: zepben.auth-0.9.0b2.dist-info/RECORD
+Filename: zepben.auth-0.9.0b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zepben/auth/client/token_fetcher.py

```diff
@@ -164,15 +164,15 @@
                     url = f"https://{host}{p}"
                 else:
                     url = f"https://{host}:{port}{p}"
                 response = requests.get(url, verify=verify_certificates and (conf_ca_filename or True))
                 if response.ok:
                     break
                 else:
-                    url_err.append(url)
+                    url_err.append(f"{url} responded with: {response.status_code} - {response.reason} {response.text}")
 
         except Exception as e:
             warnings.warn(str(e))
             warnings.warn("If RemoteDisconnected, this process may hang indefinetly.")
             raise ConnectionError("Are you trying to connect to a HTTPS server with HTTP?")
 
         if response.ok:
@@ -186,9 +186,9 @@
                         auth_method=auth_method,
                         verify_certificate=verify_certificates,
                         ca_filename=auth_ca_filename
                     )
             except ValueError as e:
                 raise ValueError(f"Expected JSON response from {url}, but got: {response.text}.", e)
         else:
-            raise ValueError(f"{url_err} responded with error: {response.status_code} - {response.reason} {response.text}")
+            raise ValueError("\n".join(url_err))
     return None
```

## Comparing `zepben.auth-0.9.0b2.dist-info/LICENSE` & `zepben.auth-0.9.0b3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zepben.auth-0.9.0b2.dist-info/METADATA` & `zepben.auth-0.9.0b3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zepben.auth
-Version: 0.9.0b2
+Version: 0.9.0b3
 Summary: Utilities for authenticating to the Evolve App Server and Energy Workbench Server
 Home-page: https://bitbucket.org/zepben/zepben-auth-python
 Author: Ramon Bouckaert
 Author-email: ramon.bouckaert@zepben.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

## Comparing `zepben.auth-0.9.0b2.dist-info/RECORD` & `zepben.auth-0.9.0b3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 zepben/auth/__init__.py,sha256=eWLMVpL5EUe1GnAFVZKrZ72Dkw7fRTcsEwCMakoC5yM,246
 zepben/auth/client/__init__.py,sha256=KV-nbtQmxemthsDMqDBltrBuARm6eoz_ta56Q5hL6D8,416
-zepben/auth/client/token_fetcher.py,sha256=Ozbo5fhEntzQh-M7j3x6v0Av0dFMYYV0V3h8gSmkj9A,8712
+zepben/auth/client/token_fetcher.py,sha256=sCiX9FGlWccnPHX-BTBQrFjsRSCkAaqjEVtICRQ2Ht8,8717
 zepben/auth/client/util.py,sha256=O6Qtbd20Juku0megvHQBaOgNxmIYfz_FkYQPUgnFYb0,449
-zepben.auth-0.9.0b2.dist-info/LICENSE,sha256=aAHD66h6PQIETpkJDvg5yEObyFvXUED8u7S8dlh6K0Y,16725
-zepben.auth-0.9.0b2.dist-info/METADATA,sha256=ckUHbu44I3B0GjHRSxbutgyZ-rf5uIW6YIcfCAqAkOo,1551
-zepben.auth-0.9.0b2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-zepben.auth-0.9.0b2.dist-info/top_level.txt,sha256=eVLDJiO6FGjL_Z7KdmFE-R8uf1Q07aaVLGe9Ee4kmBw,7
-zepben.auth-0.9.0b2.dist-info/RECORD,,
+zepben.auth-0.9.0b3.dist-info/LICENSE,sha256=aAHD66h6PQIETpkJDvg5yEObyFvXUED8u7S8dlh6K0Y,16725
+zepben.auth-0.9.0b3.dist-info/METADATA,sha256=8bSm36gmVsKKislSxdmg1E_eeE8Nmu-xzSpDFOnbzeE,1551
+zepben.auth-0.9.0b3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+zepben.auth-0.9.0b3.dist-info/top_level.txt,sha256=eVLDJiO6FGjL_Z7KdmFE-R8uf1Q07aaVLGe9Ee4kmBw,7
+zepben.auth-0.9.0b3.dist-info/RECORD,,
```

