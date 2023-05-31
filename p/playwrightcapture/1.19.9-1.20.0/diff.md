# Comparing `tmp/playwrightcapture-1.19.9.tar.gz` & `tmp/playwrightcapture-1.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.19.9.tar", max compression
+gzip compressed data, was "playwrightcapture-1.20.0.tar", max compression
```

## Comparing `playwrightcapture-1.19.9.tar` & `playwrightcapture-1.20.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.19.9/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.19.9/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.19.9/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    25992 2023-04-12 10:57:41.597394 playwrightcapture-1.19.9/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.19.9/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.19.9/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.19.9/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1739 2023-04-12 10:59:39.110047 playwrightcapture-1.19.9/pyproject.toml
--rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.19.9/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.0/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.0/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.0/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    29544 2023-05-31 08:32:38.199235 playwrightcapture-1.20.0/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.0/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.20.0/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.0/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1734 2023-05-31 08:34:19.983617 playwrightcapture-1.20.0/pyproject.toml
+-rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.20.0/PKG-INFO
```

### Comparing `playwrightcapture-1.19.9/LICENSE` & `playwrightcapture-1.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.9/README.md` & `playwrightcapture-1.20.0/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.9/playwrightcapture/capture.py` & `playwrightcapture-1.20.0/playwrightcapture/capture.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,22 +43,23 @@
 
 
 BROWSER = Literal['chromium', 'firefox', 'webkit']
 
 
 class Capture():
 
-    _user_agent: str = ''
     _browsers: List[BROWSER] = ['chromium', 'firefox', 'webkit']
     _default_viewport: ViewportSize = {'width': 1920, 'height': 1080}
-    _viewport: Optional[ViewportSize] = None
     _general_timeout: Union[int, float] = 60 * 1000   # in miliseconds, set to 60s by default
-    _cookies: List[SetCookieParam] = []
-    _http_credentials: Dict[str, str] = {}
-    _headers: Dict[str, str] = {}
+
+    _user_agent: str
+    _cookies: List[SetCookieParam]
+    _http_credentials: Dict[str, str]
+    _headers: Dict[str, str]
+    _viewport: Optional[ViewportSize]
 
     def __init__(self, browser: Optional[BROWSER]=None, device_name: Optional[str]=None,
                  proxy: Optional[Union[str, Dict[str, str]]]=None,
                  general_timeout_in_sec: Optional[int] = None, loglevel: str='INFO'):
         """Captures a page with Playwright.
 
         :param browser: The browser to use for the capture.
@@ -79,14 +80,19 @@
             else:
                 self.proxy = {'server': proxy['server'], 'bypass': proxy.get('bypass', ''),
                               'username': proxy.get('username', ''),
                               'password': proxy.get('password', '')}
 
         self.should_retry: bool = False
         self.__network_not_idle: int = 1
+        self._cookies = []
+        self._http_credentials = {}
+        self._headers = {}
+        self._viewport = None
+        self._user_agent = ''
 
     async def __aenter__(self) -> 'Capture':
         '''Launch the browser'''
         self._temp_harfile = NamedTemporaryFile(delete=False)
 
         self.playwright = await async_playwright().start()
 
@@ -173,16 +179,24 @@
             for header_line in headers.splitlines():
                 if header_line and ':' in header_line:
                     splitted = header_line.split(':', 1)
                     if splitted and len(splitted) == 2:
                         header, h_value = splitted
                         if header and h_value:
                             self._headers[header.strip()] = h_value.strip()
+        elif isinstance(headers, dict):
+            # Check if they are valid
+            safe_headers = {name: value for name, value in headers.items() if isinstance(name, str) and isinstance(value, str) and name.strip() and value.strip()}
+            if safe_headers != headers:
+                self.logger.critical(f'Headers contains invalid values:\n{json.dumps(headers, indent=2)}')
+            self._headers = safe_headers
         else:
-            self._headers = headers
+            # This shouldn't happen, but somehow it does
+            self.logger.critical(f'Headers contains invalid values:\n{json.dumps(headers, indent=2)}')  # type: ignore[unreachable]
+            return
 
     @property
     def viewport(self) -> Optional[ViewportSize]:
         return self._viewport
 
     @viewport.setter
     def viewport(self, viewport: Optional[Dict[str, int]]) -> None:
@@ -395,15 +409,15 @@
             return await page.screenshot(full_page=True)
         except Error as e:
             self.logger.info(f"Capturing a screenshot of the full page failed, trying to scale it down: {e}")
 
         try:
             return await page.screenshot(full_page=True, scale="css")
         except Error as e:
-            self.logger.warning(f"Capturing a screenshot of the full page failed, trying to get the current viewport only: {e}")
+            self.logger.info(f"Capturing a screenshot of the full page failed, trying to get the current viewport only: {e}")
 
         try:
             return await page.screenshot()
         except Error as e:
             self.logger.warning(f"Unable to get any screenshot: {e}")
             raise e
 
@@ -419,18 +433,21 @@
             else:
                 capturing_sub = False
                 page = await self.context.new_page()
             try:
                 # NOTE 2022-12-02: allow 15s less than the general timeout to get a DOM
                 await page.goto(url, wait_until='domcontentloaded', timeout=self.general_timeout - 15000, referer=referer if referer else '')
             except Error as initial_error:
-                # page.goto failed, but it (might have) triggered a download event.
-                # If it is the case, let's try to save it.
+                self._update_exceptions(initial_error)
+                if self._exception_is_network_error(initial_error):
+                    raise initial_error
                 try:
-                    async with page.expect_download(timeout=5000) as download_info:
+                    # page.goto failed, but it (might have) triggered a download event.
+                    # If it is the case, let's try to save it.
+                    async with page.expect_download(timeout=self.general_timeout - 15000) as download_info:
                         tmp_f = NamedTemporaryFile(delete=False)
                         download = await download_info.value
                         await download.save_as(tmp_f.name)
                         to_return["downloaded_filename"] = download.suggested_filename
                         with open(tmp_f.name, "rb") as f:
                             to_return["downloaded_file"] = f.read()
                         os.unlink(tmp_f.name)
@@ -522,45 +539,98 @@
                             except (TimeoutError, asyncio.exceptions.TimeoutError):
                                 self.logger.warning(f'Timeout error, took more than {max_capture_time}s. Unable to capture {url}.')
                             else:
                                 runtime = int(time.time() - start_time)
                                 self.logger.info(f'Successfully captured child URL: {url} in {runtime}s. {total_urls - index - 1} to go.')
                             try:
                                 await page.go_back()
-                            except PlaywrightTimeoutError as e:
-                                self.logger.warning(f'Go back timed out, it is probably not a big deal: {e}')
+                            except PlaywrightTimeoutError:
+                                self.logger.info('Go back timed out, it is probably not a big deal.')
 
         except PlaywrightTimeoutError as e:
             to_return['error'] = f"The capture took too long - {e.message}"
             self.should_retry = True
         except Error as e:
+            self._update_exceptions(e)
             to_return['error'] = e.message
-            # TODO: check e.name and figure out if it is worth retrying or not.
-            self.logger.critical(f'Something went poorly with {url}: {e.message}')
+            # TODO: check e.message and figure out if it is worth retrying or not.
+            # NOTE: e.name is generally (always?) "Error"
+            if self._exception_is_network_error(e):
+                # Expected errors
+                self.logger.info(f'Unable to process {url}: {e.message}')
+                if e.name == 'net::ERR_CONNECTION_RESET':
+                    self.should_retry = True
+            elif e.name in ['NS_BINDING_CANCELLED_OLD_LOAD',
+                            'NS_BINDING_ABORTED',
+                            'NS_ERROR_PARSED_DATA_CACHED']:
+                # this one sounds like something we can retry...
+                self.logger.info(f'Issue with {url} (retrying): {e.message}')
+                self.should_retry = True
+            elif e.name in ['Download is starting',
+                            'Connection closed',
+                            'Navigation interrupted by another one',
+                            'Navigation failed because page was closed!']:
+                # Other errors, let's give it another shot
+                self.logger.info(f'Issue with {url} (retrying): {e.message}')
+                self.should_retry = True
+            else:
+                # Unexpected ones
+                self.logger.exception(f'Something went poorly with {url}: {e.message}')
         finally:
             if not capturing_sub:
                 to_return['cookies'] = await self.context.cookies()
                 # frames_tree = self.make_frame_tree(page.main_frame)
                 try:
                     await self.context.close()  # context needs to be closed to generate the HAR
                     with open(self._temp_harfile.name) as _har:
                         to_return['har'] = json.load(_har)
                 except Exception as e:
                     to_return['error'] = f'Unable to generate HAR file: {e}'
         self.logger.debug('Capture done')
         return to_return
 
+    def _update_exceptions(self, exception: Error) -> None:
+        if '\n' in exception.message:
+            name, _ = exception.message.split('\n', maxsplit=1)
+            if ' at ' in name:
+                name, _ = name.split(' at ', maxsplit=1)
+            elif '; ' in name:
+                name, _ = name.split('; ', maxsplit=1)
+            exception.name = name.strip()
+
+    def _exception_is_network_error(self, exception: Error) -> bool:
+        if exception.name in ['NS_ERROR_UNKNOWN_HOST',
+                              'NS_ERROR_CONNECTION_REFUSED',
+                              'NS_ERROR_NET_RESET',
+                              'NS_ERROR_UNEXPECTED',
+                              'NS_ERROR_NET_TIMEOUT',
+                              'NS_ERROR_REDIRECT_LOOP',
+                              'NS_ERROR_NET_INTERRUPT',
+                              'NS_ERROR_UNKNOWN_PROTOCOL',
+                              'NS_ERROR_ABORT',
+                              'net::ERR_EMPTY_RESPONSE',
+                              'net::ERR_CONNECTION_REFUSED',
+                              'net::ERR_CONNECTION_RESET',
+                              'net::ERR_ADDRESS_UNREACHABLE',
+                              'net::ERR_NAME_NOT_RESOLVED',
+                              'net::ERR_SSL_PROTOCOL_ERROR',
+                              'net::ERR_TOO_MANY_REDIRECTS',
+                              'net::ERR_TIMED_OUT',
+                              'net::ERR_ABORTED',
+                              ]:
+            return True
+        return False
+
     async def __aexit__(self, exc_type: Any, exc: Any, tb: Any) -> None:
         if hasattr(self, '_temp_harfile'):
             os.unlink(self._temp_harfile.name)
 
         try:
             await self.browser.close()
         except Exception as e:
             # We may land in a situation where the capture was forcefully closed and the browser is already closed
             self.logger.info(f'Unable to close browser: {e}')
         try:
-            # This method *must* be awaited but for some reason, MyPy complains.
-            await self.playwright.stop()  # type: ignore
+            await self.playwright.stop()
         except Exception as e:
             # this should't happen, but just in case it does...
-            self.logger.info(f'Unable to stop playwright: {e}')
+            self.logger.warning(f'Unable to stop playwright: {e}')
```

### Comparing `playwrightcapture-1.19.9/playwrightcapture/helpers.py` & `playwrightcapture-1.20.0/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.9/pyproject.toml` & `playwrightcapture-1.20.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.19.9"
+version = "1.20.0"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -17,39 +17,39 @@
     'Topic :: Internet',
 ]
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
-playwright = "^1.32.1"
+playwright = "^1.34.0"
 dateparser = "^1.1.8"
 beautifulsoup4 = "^4.12.2"
 w3lib = "^2.1.1"
 lxml = "^4.9.2"
-requests = {version = "^2.28.2", optional = true}
+requests = {version = "^2.31.0", optional = true}
 pydub = {version = "^0.25.1", optional = true}
 SpeechRecognition = {version = "^3.10.0", optional = true}
 
 [tool.poetry.extras]
 recaptcha = ["requests", "pydub", "SpeechRecognition"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-types-beautifulsoup4 = "^4.11.6.6"
-pytest = "^7.2.1"
-mypy = "^1.0.1"
-types-dateparser = "^1.1.4.7"
-types-requests = "^2.28.11.13"
+types-beautifulsoup4 = "^4.12.0.3"
+pytest = "^7.3.1"
+mypy = "^1.2.0"
+types-dateparser = "^1.1.4.9"
+types-requests = "^2.28.11.17"
 
 
 [build-system]
-requires = ["poetry-core>=1.1"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 check_untyped_defs = true
```

### Comparing `playwrightcapture-1.19.9/PKG-INFO` & `playwrightcapture-1.20.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.19.9
+Version: 1.20.0
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -20,17 +20,17 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: recaptcha
 Requires-Dist: SpeechRecognition (>=3.10.0,<4.0.0) ; extra == "recaptcha"
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: playwright (>=1.32.1,<2.0.0)
+Requires-Dist: playwright (>=1.34.0,<2.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "recaptcha"
-Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "recaptcha"
+Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "recaptcha"
 Requires-Dist: w3lib (>=2.1.1,<3.0.0)
 Project-URL: Repository, https://github.com/Lookyloo/PlaywrightCapture
 Description-Content-Type: text/markdown
 
 # Playwright Capture
 
 Simple replacement for [splash](https://github.com/scrapinghub/splash) using [playwright](https://github.com/microsoft/playwright-python).
```

