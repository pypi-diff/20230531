# Comparing `tmp/UnlimitedGPT-0.1.1.tar.gz` & `tmp/UnlimitedGPT-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.1.1.tar", last modified: Wed May 31 18:06:51 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.1.2.tar", last modified: Wed May 31 20:49:24 2023, max compression
```

## Comparing `UnlimitedGPT-0.1.1.tar` & `UnlimitedGPT-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-31 18:06:51.927599 UnlimitedGPT-0.1.1/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-05-31 18:06:51.927599 UnlimitedGPT-0.1.1/PKG-INFO
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-31 18:06:51.919600 UnlimitedGPT-0.1.1/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    27066 2023-05-31 17:55:34.000000 UnlimitedGPT-0.1.1/UnlimitedGPT/UnlimitedGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.1/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-31 18:06:51.927599 UnlimitedGPT-0.1.1/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2273 2023-05-31 16:18:56.000000 UnlimitedGPT-0.1.1/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-31 16:19:36.000000 UnlimitedGPT-0.1.1/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      115 2023-05-31 17:42:42.000000 UnlimitedGPT-0.1.1/UnlimitedGPT/internal/exceptions.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-28 11:29:18.000000 UnlimitedGPT-0.1.1/UnlimitedGPT/internal/objects.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-31 18:06:51.923599 UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-05-31 18:06:50.000000 UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-05-31 18:06:50.000000 UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-31 18:06:50.000000 UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-31 18:06:50.000000 UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-05-31 18:06:50.000000 UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-31 18:06:51.927599 UnlimitedGPT-0.1.1/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-05-31 18:05:50.000000 UnlimitedGPT-0.1.1/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-31 20:49:24.838829 UnlimitedGPT-0.1.2/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-05-31 20:49:24.838829 UnlimitedGPT-0.1.2/PKG-INFO
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-31 20:49:24.830829 UnlimitedGPT-0.1.2/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    26341 2023-05-31 20:42:42.000000 UnlimitedGPT-0.1.2/UnlimitedGPT/UnlimitedGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.2/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-31 20:49:24.838829 UnlimitedGPT-0.1.2/UnlimitedGPT/internal/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2383 2023-05-31 20:36:47.000000 UnlimitedGPT-0.1.2/UnlimitedGPT/internal/chatgpt_data.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-31 16:19:36.000000 UnlimitedGPT-0.1.2/UnlimitedGPT/internal/driver.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      115 2023-05-31 17:42:42.000000 UnlimitedGPT-0.1.2/UnlimitedGPT/internal/exceptions.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-31 20:14:14.000000 UnlimitedGPT-0.1.2/UnlimitedGPT/internal/objects.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-31 20:49:24.834829 UnlimitedGPT-0.1.2/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-05-31 20:49:23.000000 UnlimitedGPT-0.1.2/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-05-31 20:49:23.000000 UnlimitedGPT-0.1.2/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-31 20:49:23.000000 UnlimitedGPT-0.1.2/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-31 20:49:23.000000 UnlimitedGPT-0.1.2/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-05-31 20:49:23.000000 UnlimitedGPT-0.1.2/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-31 20:49:24.838829 UnlimitedGPT-0.1.2/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-05-31 20:48:50.000000 UnlimitedGPT-0.1.2/setup.py
```

### Comparing `UnlimitedGPT-0.1.1/PKG-INFO` & `UnlimitedGPT-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.1
+Version: 0.1.2
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
```

### Comparing `UnlimitedGPT-0.1.1/UnlimitedGPT/UnlimitedGPT.py` & `UnlimitedGPT-0.1.2/UnlimitedGPT/UnlimitedGPT.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,44 +31,39 @@
         session_token (str): The session token for authentication.
         conversation_id (str, optional): The conversation ID. Defaults to ''.
         proxy (Optional[str], optional): The proxy server URL. Defaults to None.
         disable_moderation (bool, optional): Whether to disable moderation. Defaults to True.
         verbose (bool, optional): Whether to enable verbose logging. Defaults to False.
         headless (bool, optional): Whether to run the browser in headless mode. Defaults to False.
         chrome_args (list, optional): Additional arguments for the Chrome browser. Defaults to [].
-        input_mode(list, options): The input mode. Defaults to 'INSTANT'.
-        input_delay(float, options): The input delay. Defaults to 0.2.
     
     Raises:
     ----------
+        InvalidConversationID: If the conversation ID is invalid.
         ValueError: If the session token is not provided.
         ValueError: If the proxy is invalid.
     """
 
     def __init__(
         self,
         session_token: str,
         conversation_id: str = '',
         proxy: Optional[str] = None,
         disable_moderation: bool = True,
         verbose: bool = False,
         headless: bool = False,
         chrome_args: list = [],
-        input_mode: Literal['INSTANT', 'SLOW'] = 'INSTANT',
-        input_delay: float = 0.2,
     ) -> None:
         self._session_token = session_token
         self._conversation_id = conversation_id
         self._proxy = proxy
         self._disable_moderation = disable_moderation
         self._headless = headless
         self._chrome_args = chrome_args
         self._clicked_buttons = False
-        self._input_mode = input_mode
-        self._input_delay = input_delay
         self._init_logger(verbose)
 
         if not self._session_token:
             raise ValueError("session_token is required")
         if self._proxy and not re.findall(
             r'(https?|socks(4|5)?):\/\/.+:\d{1,5}', self._proxy # type: ignore
         ):
@@ -276,52 +271,63 @@
             raise ValueError('Invalid session token')
         self.logger.debug('Authorization is valid')
 
         self.logger.debug('Closing tab...')
         self.driver.close()
         self.driver.switch_to.window(original_window)
 
-    def send_message(self, message: str, timeout: int = 240) -> ChatGPTResponse:
+    def send_message(
+        self,
+        message: str,
+        timeout: int = 240,
+        input_mode: Literal['INSTANT', 'SLOW'] = "INSANT",
+        input_delay: float = 0.1,
+    ) -> ChatGPTResponse:
         """
         Send a message to ChatGPT.
 
         Args:
         ----------
             message (str): Message to send.
             timeout (int, optional): Timeout in seconds. Defaults to 240.
+            input_mode(list, optional): The input mode. Defaults to 'INSTANT'.
+            input_delay(float, optional): The input delay. Defaults to 0.1.
 
         Returns:
         ----------
             ChatGPTResponse: Response from ChatGPT.
 
         Raises:
         ----------
             TimeoutException: If the message fails to send.
             ValueError: If the response is invalid.
             ValueError: If the response is not found.
         """
-        self.logger.debug(f'Sending message with mode {self._input_mode}{f" with {self._input_delay} delay" if self._input_mode == "SLOW" else ""}...')
+        self.logger.debug(f'Sending message with mode {input_mode}{f" with {input_delay} delay" if input_mode == "SLOW" else ""}...')
 
         textbox = WebDriverWait(self.driver, 60).until(
             EC.element_to_be_clickable(CGPTV.chatgpt_textbox)
         )
-        if self._input_mode == 'INSTANT':
+        if input_mode == 'INSTANT':
             self.driver.execute_script("arguments[0].value = arguments[1];", textbox, message)
         else:
             for char in message:
                 try:
                     textbox.send_keys(char)
                 except StaleElementReferenceException:
                     textbox = WebDriverWait(self.driver, 60).until(
                         EC.element_to_be_clickable(CGPTV.chatgpt_textbox)
                     )
                     textbox.send_keys(char)
-                sleep(self._input_delay)
 
-        textbox.send_keys(Keys.ENTER)
+        while True:
+            value = self.driver.execute_script("return arguments[0].value;", textbox)
+            if len(value.strip().replace('\n', '').replace(' ', '').replace('\r', '')) == 0:
+                break
+            textbox.send_keys(Keys.ENTER)
 
         self.logger.debug('Waiting for completion...')
         WebDriverWait(self.driver, timeout).until_not(
             EC.presence_of_element_located(CGPTV.chatgpt_streaming)
         )
 
         self.logger.debug('Getting response...')
@@ -338,29 +344,16 @@
             self.logger.debug('Response not found, resetting conversation...')
             self.reset_conversation()
             raise ValueError('Response not found')
 
         content = markdownify(response.get_attribute('innerHTML')).replace(
             'Copy code`', '`'
         )
-        
-        pattern = re.compile(
-            r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}'
-        )
-        matches = pattern.search(self.driver.current_url)
-        if not matches:
-            self.reset_conversation()
-            self.driver.safe_click(CGPTV.chatgpt_chats_list_first_node, 60)
-            sleep(0.5)
-            matches = pattern.search(self.driver.current_url)
-        try:
-            conversation_id = matches.group() # type: ignore
-        except:
-            conversation_id = None
-        return ChatGPTResponse(content, conversation_id)
+
+        return ChatGPTResponse(content, self._conversation_id)
 
     def reset_conversation(self) -> None:
         """
         Resets the conversation.
         """
         if not self.driver.current_url.startswith(CGPTV.chatgpt_chat_url):
             return self.logger.debug('Current URL is not chat page, skipping reset')
@@ -429,15 +422,15 @@
             
             current_theme_value = self.driver.find_element(*CGPTV.chatgpt_outer_html).get_attribute('class')
             current_theme = 'LIGHT' if 'light' in current_theme_value else 'DARK'
             if theme == current_theme:
                 self.logger.debug('Theme is already set to the desired theme')
                 return self._get_out_of_menu()
 
-            select_element = self.driver.find_element(CGPTV.chatgpt_theme_select)
+            select_element = self.driver.find_element(*CGPTV.chatgpt_theme_select)
             ActionChains(self.driver).move_to_element(select_element).perform()
             select_clicked = self.driver.safe_click(CGPTV.chatgpt_theme_select, 60)
             if not select_clicked:
                 self.logger.debug('Could not click theme select')
                 return self._get_out_of_menu()
 
             if theme == 'OPPOSITE':
@@ -510,25 +503,32 @@
         Get the session data.
 
         Returns:
         ----------
             SessionData: The ChatGPT session data.
         """
         self.logger.debug('Getting account data...')
+        original_window = self.driver.current_window_handle
+        self.logger.debug('Opening new tab...')
+        self.driver.execute_script("window.open();")
+        self.driver.switch_to.window(self.driver.window_handles[-1])
         self.driver.get('https://chat.openai.com/api/auth/session')
         response = self.driver.page_source
         if response[0] != '{':
             response = self.driver.find_element(By.TAG_NAME, 'pre').text
         response = loads(response)
         session_data = SessionData(
             User(**response['user']),
             response["expires"],
             response["accessToken"],
             response["authProvider"]
         )
+        self.logger.debug('Closing tab...')
+        self.driver.close()
+        self.driver.switch_to.window(original_window)
         return session_data
 
     def logout(self) -> None:
         """
         Logs out of the current account signed into https://chat.openai.com
         """
         self.logger.debug('Logging out...')
@@ -572,15 +572,15 @@
 
             self.logger.debug('Clicked settings button')
 
             wait = WebDriverWait(self.driver, 60)
 
             # Click "Data controls" button
             data_controls_button_clicked = self.driver.safe_click(
-                CGPTV.chatgpt_menu_data_controls_button, 60
+                CGPTV.chatgpt_data_controls_button, 60
             )
             if not data_controls_button_clicked:
                 self.logger.debug('Could not click data controls button')
                 return self._get_out_of_menu()
 
             # Click "Disable chat history" button
             # Not using safe_click because it there are some checks that need to be done before clicking
@@ -645,25 +645,9 @@
             self.reset_conversation()
             raise ValueError('Response not found')
 
         content = markdownify(response.get_attribute('innerHTML')).replace(
             'Copy code`', '`'
         )
         
-        pattern = re.compile(
-            r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}'
-        )
-        matches = pattern.search(self.driver.current_url)
-        if not matches:
-            self.reset_conversation()
-            list_first_node_clicked = self.driver.safe_click(CGPTV.chatgpt_chats_list_first_node, 60)
-            if not list_first_node_clicked:
-                self.logger.debug('Could not click chats list first node')
-                raise TimeoutException('Could not click chats list first node')
-            sleep(0.5)
-            matches = pattern.search(self.driver.current_url)
-        try:
-            conversation_id = matches.group() # type: ignore
-        except:
-            conversation_id = None
         self.logger.debug('Regenerated response')
-        return ChatGPTResponse(content, conversation_id)
+        return ChatGPTResponse(content, self._conversation_id)
```

### Comparing `UnlimitedGPT-0.1.1/UnlimitedGPT/internal/driver.py` & `UnlimitedGPT-0.1.2/UnlimitedGPT/internal/driver.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.1/UnlimitedGPT/internal/objects.py` & `UnlimitedGPT-0.1.2/UnlimitedGPT/internal/objects.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/PKG-INFO` & `UnlimitedGPT-0.1.2/UnlimitedGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.1
+Version: 0.1.2
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
```

### Comparing `UnlimitedGPT-0.1.1/setup.py` & `UnlimitedGPT-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     author='Sxvxge',
     url='https://github.com/Sxvxgee/UnlimitedGPT',
     project_urls={
         'Documentation': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md',
         'Issue tracker': 'https://github.com/Sxvxgee/UnlimitedGPT/issues',
         'Changelog': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md',
     },
-    version="0.1.1",
+    version="0.1.2",
     packages=['UnlimitedGPT', 'UnlimitedGPT/internal'],
     py_modules=['UnlimitedGPT'],
     license='GPL-3.0 license',
     description='An unofficial Python wrapper for OpenAI\'s ChatGPT API',
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
```

