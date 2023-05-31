# Comparing `tmp/orbit_component_base-0.99.2.tar.gz` & `tmp/orbit_component_base-0.99.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_base-0.99.2.tar", max compression
+gzip compressed data, was "orbit_component_base-0.99.5.tar", max compression
```

## Comparing `orbit_component_base-0.99.2.tar` & `orbit_component_base-0.99.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1099 2023-05-30 10:22:19.434839 orbit_component_base-0.99.2/LICENSE.md
--rw-r--r--   0        0        0      307 2023-05-30 10:24:05.900452 orbit_component_base-0.99.2/README.md
--rw-r--r--   0        0        0      248 2023-05-26 21:23:29.392298 orbit_component_base-0.99.2/orbit_component_base/__init__.py
--rw-r--r--   0        0        0      698 2023-05-26 14:58:49.369068 orbit_component_base-0.99.2/orbit_component_base/plugin.py
--rw-r--r--   0        0        0     1020 2023-05-26 15:16:14.168223 orbit_component_base-0.99.2/orbit_component_base/schema/OrbitSessions.py
--rw-r--r--   0        0        0      343 2023-05-26 15:16:31.111878 orbit_component_base-0.99.2/orbit_component_base/schema/OrbitUsers.py
--rwxr-xr-x   0        0        0     3489 2023-05-26 15:35:41.416368 orbit_component_base-0.99.2/orbit_component_base/src/orbit_app.py
--rw-r--r--   0        0        0     6315 2023-05-26 15:07:46.174514 orbit_component_base-0.99.2/orbit_component_base/src/orbit_auth.py
--rw-r--r--   0        0        0     6348 2023-05-26 15:11:22.310156 orbit_component_base-0.99.2/orbit_component_base/src/orbit_config.py
--rw-r--r--   0        0        0     1232 2023-05-26 15:11:34.365912 orbit_component_base-0.99.2/orbit_component_base/src/orbit_database.py
--rw-r--r--   0        0        0     3749 2023-05-09 09:42:38.245588 orbit_component_base-0.99.2/orbit_component_base/src/orbit_decorators.py
--rw-r--r--   0        0        0      290 2023-03-24 17:01:29.910135 orbit_component_base-0.99.2/orbit_component_base/src/orbit_logger.py
--rw-r--r--   0        0        0      834 2023-05-26 15:11:48.925617 orbit_component_base-0.99.2/orbit_component_base/src/orbit_make_ssl.py
--rw-r--r--   0        0        0     8612 2023-05-26 15:12:25.840869 orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql.py
--rw-r--r--   0        0        0     3534 2023-03-28 12:50:44.012670 orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql_buffer.py
--rw-r--r--   0        0        0      895 2023-04-03 10:19:17.442215 orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql_emitter.py
--rw-r--r--   0        0        0     4442 2023-05-23 12:28:15.559177 orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql_session.py
--rw-r--r--   0        0        0     6409 2023-05-25 11:09:33.029380 orbit_component_base-0.99.2/orbit_component_base/src/orbit_orm.py
--rw-r--r--   0        0        0     2293 2023-05-26 21:23:57.215737 orbit_component_base-0.99.2/orbit_component_base/src/orbit_plugin.py
--rw-r--r--   0        0        0     1243 2023-05-26 16:04:04.125398 orbit_component_base-0.99.2/orbit_component_base/src/orbit_plugins.py
--rw-r--r--   0        0        0     2329 2023-05-26 15:13:02.796118 orbit_component_base-0.99.2/orbit_component_base/src/orbit_router.py
--rw-r--r--   0        0        0      629 2023-05-23 16:46:20.522320 orbit_component_base-0.99.2/orbit_component_base/src/orbit_shared.py
--rw-r--r--   0        0        0       21 2023-05-24 17:39:08.131348 orbit_component_base-0.99.2/orbit_component_base/src/orbit_version.py
--rw-r--r--   0        0        0       76 2023-05-26 15:02:23.180928 orbit_component_base-0.99.2/orbit_component_base/tests/test_main.py
--rw-r--r--   0        0        0     1395 2023-05-30 11:29:01.775331 orbit_component_base-0.99.2/pyproject.toml
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 orbit_component_base-0.99.2/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/LICENSE.md
+-rw-r--r--   0        0        0      307 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/README.md
+-rw-r--r--   0        0        0      248 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/__init__.py
+-rw-r--r--   0        0        0      698 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/plugin.py
+-rw-r--r--   0        0        0     1020 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/schema/OrbitSessions.py
+-rw-r--r--   0        0        0      343 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/schema/OrbitUsers.py
+-rwxr-xr-x   0        0        0     3506 2023-05-30 20:47:27.827498 orbit_component_base-0.99.5/orbit_component_base/src/orbit_app.py
+-rw-r--r--   0        0        0     6315 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_auth.py
+-rw-r--r--   0        0        0     6281 2023-05-30 16:47:54.685910 orbit_component_base-0.99.5/orbit_component_base/src/orbit_config.py
+-rw-r--r--   0        0        0     1232 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_database.py
+-rw-r--r--   0        0        0     3749 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_decorators.py
+-rw-r--r--   0        0        0      290 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_logger.py
+-rw-r--r--   0        0        0      834 2023-05-30 16:30:11.592032 orbit_component_base-0.99.5/orbit_component_base/src/orbit_make_ssl.py
+-rw-r--r--   0        0        0     8612 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_nql.py
+-rw-r--r--   0        0        0     3534 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_nql_buffer.py
+-rw-r--r--   0        0        0      895 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_nql_emitter.py
+-rw-r--r--   0        0        0     4442 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_nql_session.py
+-rw-r--r--   0        0        0     6409 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_orm.py
+-rw-r--r--   0        0        0     2293 2023-05-30 15:19:20.188832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_plugin.py
+-rw-r--r--   0        0        0     1243 2023-05-30 15:19:20.192832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_plugins.py
+-rw-r--r--   0        0        0     2329 2023-05-30 21:39:29.016203 orbit_component_base-0.99.5/orbit_component_base/src/orbit_router.py
+-rw-r--r--   0        0        0      629 2023-05-30 15:19:20.192832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_shared.py
+-rw-r--r--   0        0        0       21 2023-05-30 15:19:20.192832 orbit_component_base-0.99.5/orbit_component_base/src/orbit_version.py
+-rw-r--r--   0        0        0       76 2023-05-30 15:19:20.192832 orbit_component_base-0.99.5/orbit_component_base/tests/test_main.py
+-rw-r--r--   0        0        0     1395 2023-05-31 13:07:50.239547 orbit_component_base-0.99.5/pyproject.toml
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 orbit_component_base-0.99.5/PKG-INFO
```

### Comparing `orbit_component_base-0.99.2/LICENSE.md` & `orbit_component_base-0.99.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/plugin.py` & `orbit_component_base-0.99.5/orbit_component_base/plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/schema/OrbitSessions.py` & `orbit_component_base-0.99.5/orbit_component_base/schema/OrbitSessions.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_app.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                     handle_signals=False,
                     host=world.conf.host,
                     port=world.conf.port,
                     ssl_context=ssl_context)            
             else:
                 web.run_app(
                     app,
-                    host="localhost",
-                    port=world.conf.local_port)
+                    host=world.conf.host,
+                    port=world.conf.port)                   
         except Exception as e:
             log.exception(e)
         finally:
             print()
             log.info('Shutdown')
             raise GracefulExit()
```

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_auth.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_auth.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_config.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,23 @@
 from warnings import filterwarnings
 from orbit_component_base.src.orbit_shared import world
 from platform import system
 
 
 class OrbitConfig:
 
-    BASE_authentication = 'secure'
+    BASE_authentication = 'autoenroll'
 
     @property
     def path (self):            return Path(self._conf.get('BASE', 'path')).expanduser()
 
     @property
     def code (self):            return Path(self._conf.get('BASE', 'code')).expanduser()
 
     @property
-    def namespace (self):       return self._conf.get('BASE', 'namespace')
-
-    @property
     def authentication (self):  return self._conf.get('BASE', 'authentication')
 
     @property
     def name (self):            return self._conf.get('SSL', 'name')
 
     @property
     def ssl (self):             return self.mkpath('SSL', 'ssl')
@@ -49,15 +46,15 @@
     @property
     def engineio_debug (self):  return self._conf.getboolean('NETWORK', 'engineio_debug')
 
     @property
     def vite_port (self):       return self._conf.getint('DEV', 'vite_port')
 
     @property
-    def make_keys (self):       return self.mkcode('TOOLS', 'make_keys')
+    def make_keys (self):       return self._conf.get('TOOLS', 'make_keys')
 
     @property
     def database (self):        return self.mkpath('DATA', 'database')
 
     @property
     def tmp (self):             return self.mkpath('DATA', 'tmp')
 
@@ -108,46 +105,48 @@
         value = self._conf.get(section, option)
         if not value:
             return None
         if value[0] in './~':
             p = Path(self._conf.get(section, option)).expanduser()
         else:
             p = path / self._conf.get(section, option)
-        p.mkdir(parents=True, exist_ok=True)
+        try:
+            p.mkdir(parents=True, exist_ok=True)
+        except FileExistsError:
+            pass
         return p
 
     def open (self):
         self._path.mkdir(parents=True, exist_ok=True)
         self._conf = ConfigParser()
         self._conf.read(self._file.as_posix())
         for section in ['BASE', 'NETWORK', 'TOOLS', 'DATA', 'SSL', 'DEV']:
             if section not in self._conf.sections():
                 self._conf.add_section(section)
                 self._changed = True
         code_path = f'/Applications/{self._appl}.app/Contents/Resources/' if system() == 'Darwin' else f'/opt/{self._appl}'
         self._option('BASE', 'path', f'~/.local/{self._appl}')
         self._option('BASE', 'code', code_path)
-        self._option('BASE', 'namespace', '/orb')
         self._option('BASE', 'authentication', self.BASE_authentication)
         self._option('SSL', 'name', 'localhost')
         self._option('SSL', 'ssl', 'ssl')
         self._option('SSL', 'secure', 'true')
         self._option('NETWORK', 'host', '127.0.0.1')
         self._option('NETWORK', 'port', '8445')
         self._option('NETWORK', 'local_port', '8445')
-        self._option('DEV', 'vite_port', '3000')
+        self._option('DEV', 'vite_port', '5173')
         self._option('NETWORK', 'sio_debug', 'false')
         self._option('NETWORK', 'engineio_debug', 'false')
-        self._option('TOOLS', 'make_keys', 'scripts/make_keys.sh')
         self._option('DATA', 'database', 'orbit_database')
         self._option('DATA', 'tmp', 'tmp')
         self._option('DATA', 'templates', 'templates')
         self._option('DATA', 'web', 'web')
         self._option('DATA', 'logs', 'logs')
         self._option('DATA', 'writemap', 'true')        
+        self._option('TOOLS', 'make_keys', 'scripts/make_keys.sh')
         if self._changed:
             with open(self._file.as_posix(), 'w') as configfile:
                 self._conf.set('DEFAULT', 'updated', datetime.now().isoformat())
                 self._conf.write(configfile)
         self.setup_logging()                
         return self
```

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_database.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_database.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_decorators.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_decorators.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_make_ssl.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_make_ssl.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_nql.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql_buffer.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_nql_buffer.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql_emitter.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_nql_emitter.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql_session.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_nql_session.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_orm.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_orm.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_plugin.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_plugins.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_plugins.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_router.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_router.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/orbit_component_base/src/orbit_shared.py` & `orbit_component_base-0.99.5/orbit_component_base/src/orbit_shared.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.2/pyproject.toml` & `orbit_component_base-0.99.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-base"
-version = "0.99.2"
+version = "0.99.5"
 description = "Orbit Framework - base component"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "orbit_component_base"}]
 include = ['README.md', 'LICENSE.md']
 keywords = ['orbit-framework', 'orbit-component', 'orbit-database']
```

### Comparing `orbit_component_base-0.99.2/PKG-INFO` & `orbit_component_base-0.99.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-base
-Version: 0.99.2
+Version: 0.99.5
 Summary: Orbit Framework - base component
 Home-page: https://gitlab.com/madpenguin/orbit-component-base
 License: MIT
 Keywords: orbit-framework,orbit-component,orbit-database
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
```

