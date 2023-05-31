# Comparing `tmp/UnlimitedGPT-0.1.0.tar.gz` & `tmp/UnlimitedGPT-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.1.0.tar", last modified: Mon May 29 16:25:03 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.1.1.tar", last modified: Wed May 31 18:06:51 2023, max compression
```

## Comparing `UnlimitedGPT-0.1.0.tar` & `UnlimitedGPT-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-29 16:25:02.984886 UnlimitedGPT-0.1.0/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4181 2023-05-29 16:25:02.984886 UnlimitedGPT-0.1.0/PKG-INFO
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-29 16:25:02.976886 UnlimitedGPT-0.1.0/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    25484 2023-05-29 16:14:45.000000 UnlimitedGPT-0.1.0/UnlimitedGPT/UnlimitedGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.0/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-29 16:25:02.980886 UnlimitedGPT-0.1.0/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2188 2023-05-29 14:53:34.000000 UnlimitedGPT-0.1.0/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-28 11:02:47.000000 UnlimitedGPT-0.1.0/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-28 11:29:18.000000 UnlimitedGPT-0.1.0/UnlimitedGPT/internal/objects.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-29 16:25:02.980886 UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4181 2023-05-29 16:25:02.000000 UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      344 2023-05-29 16:25:02.000000 UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-29 16:25:02.000000 UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-29 16:25:02.000000 UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-05-29 16:25:02.000000 UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-29 16:25:02.988886 UnlimitedGPT-0.1.0/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1686 2023-05-29 16:20:08.000000 UnlimitedGPT-0.1.0/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-31 18:06:51.927599 UnlimitedGPT-0.1.1/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-05-31 18:06:51.927599 UnlimitedGPT-0.1.1/PKG-INFO
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-31 18:06:51.919600 UnlimitedGPT-0.1.1/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    27066 2023-05-31 17:55:34.000000 UnlimitedGPT-0.1.1/UnlimitedGPT/UnlimitedGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.1/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-31 18:06:51.927599 UnlimitedGPT-0.1.1/UnlimitedGPT/internal/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2273 2023-05-31 16:18:56.000000 UnlimitedGPT-0.1.1/UnlimitedGPT/internal/chatgpt_data.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-31 16:19:36.000000 UnlimitedGPT-0.1.1/UnlimitedGPT/internal/driver.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      115 2023-05-31 17:42:42.000000 UnlimitedGPT-0.1.1/UnlimitedGPT/internal/exceptions.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-28 11:29:18.000000 UnlimitedGPT-0.1.1/UnlimitedGPT/internal/objects.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-31 18:06:51.923599 UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-05-31 18:06:50.000000 UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-05-31 18:06:50.000000 UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-31 18:06:50.000000 UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-31 18:06:50.000000 UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-05-31 18:06:50.000000 UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-31 18:06:51.927599 UnlimitedGPT-0.1.1/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-05-31 18:05:50.000000 UnlimitedGPT-0.1.1/setup.py
```

### Comparing `UnlimitedGPT-0.1.0/PKG-INFO` & `UnlimitedGPT-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.0
+Version: 0.1.1
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
+Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `UnlimitedGPT-0.1.0/UnlimitedGPT/UnlimitedGPT.py` & `UnlimitedGPT-0.1.1/UnlimitedGPT/UnlimitedGPT.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from json import loads
 from logging import getLogger, DEBUG, Formatter, StreamHandler
 from weakref import finalize
 
 from markdownify import markdownify
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.wait import WebDriverWait
-from selenium.common.exceptions import TimeoutException, NoSuchElementException
+from selenium.common.exceptions import TimeoutException, NoSuchElementException, StaleElementReferenceException
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.action_chains import ActionChains
 from undetected_chromedriver import ChromeOptions
 
 from .internal.driver import ChatGPTDriver
 from .internal.chatgpt_data import ChatGPTVariables as CGPTV
 from .internal.objects import ChatGPTResponse, User, SessionData
+from .internal.exceptions import InvalidConversationID
 
 class ChatGPT:
     """
     A class for interacting with ChatGPT.
 
     Args:
     ----------
@@ -32,15 +32,15 @@
         conversation_id (str, optional): The conversation ID. Defaults to ''.
         proxy (Optional[str], optional): The proxy server URL. Defaults to None.
         disable_moderation (bool, optional): Whether to disable moderation. Defaults to True.
         verbose (bool, optional): Whether to enable verbose logging. Defaults to False.
         headless (bool, optional): Whether to run the browser in headless mode. Defaults to False.
         chrome_args (list, optional): Additional arguments for the Chrome browser. Defaults to [].
         input_mode(list, options): The input mode. Defaults to 'INSTANT'.
-        input_delay(int, options): The input delay. Defaults to 0.2.
+        input_delay(float, options): The input delay. Defaults to 0.2.
     
     Raises:
     ----------
         ValueError: If the session token is not provided.
         ValueError: If the proxy is invalid.
     """
 
@@ -50,15 +50,15 @@
         conversation_id: str = '',
         proxy: Optional[str] = None,
         disable_moderation: bool = True,
         verbose: bool = False,
         headless: bool = False,
         chrome_args: list = [],
         input_mode: Literal['INSTANT', 'SLOW'] = 'INSTANT',
-        input_delay: int = 0.2,
+        input_delay: float = 0.2,
     ) -> None:
         self._session_token = session_token
         self._conversation_id = conversation_id
         self._proxy = proxy
         self._disable_moderation = disable_moderation
         self._headless = headless
         self._chrome_args = chrome_args
@@ -209,33 +209,32 @@
 
     def _check_blocking_elements(self) -> None:
         """
         Check for blocking elements and dismiss them.
         """
         self.logger.debug('Looking for blocking elements...')
         try:
-            intro = WebDriverWait(self.driver, 3).until(
+            intro = WebDriverWait(self.driver, 5).until(
                 EC.presence_of_element_located(CGPTV.chatgpt_intro)
             )
             self.logger.debug('Dismissing intro...')
             self.driver.execute_script('arguments[0].remove()', intro)
         except TimeoutException:
             pass
 
         alerts = self.driver.find_elements(*CGPTV.chatgpt_alert)
         if alerts:
+            if 'unable to load conversation' in alerts[0].text.lower():
+                raise InvalidConversationID(alerts[0].text)
             self.logger.debug('Dismissing alert...')
             self.driver.execute_script('arguments[0].remove()', alerts[0])
 
         if not self._clicked_buttons:
             for button in CGPTV.chatgpt_info_buttons:
-                btn = WebDriverWait(self.driver, 60).until(
-                    EC.element_to_be_clickable(button)
-                )
-                btn.click()
+                self.driver.safe_click(button, 60)
             self._clicked_buttons = True
 
     def _ensure_cf(self, retry: int = 3) -> None:
         """
         Ensure Cloudflare cookies are set.
 
         Args:
@@ -254,15 +253,14 @@
         self.driver.get('https://chat.openai.com/api/auth/session')
         try:
             WebDriverWait(self.driver, 10).until_not(
                 EC.presence_of_element_located(CGPTV.cf_challenge_form)
             )
         except TimeoutException:
             self.logger.debug(f'Cloudflare challenge failed, retrying {retry}...')
-            self.driver.save_screenshot(f'cf_failed_{retry}.png')
             if retry > 0:
                 self.logger.debug('Closing tab...')
                 self.driver.close()
                 self.driver.switch_to.window(original_window)
                 return self._ensure_cf(retry - 1)
             raise ValueError('Cloudflare challenge failed')
         self.logger.debug('Cloudflare challenge passed')
@@ -306,15 +304,21 @@
         textbox = WebDriverWait(self.driver, 60).until(
             EC.element_to_be_clickable(CGPTV.chatgpt_textbox)
         )
         if self._input_mode == 'INSTANT':
             self.driver.execute_script("arguments[0].value = arguments[1];", textbox, message)
         else:
             for char in message:
-                textbox.send_keys(char)
+                try:
+                    textbox.send_keys(char)
+                except StaleElementReferenceException:
+                    textbox = WebDriverWait(self.driver, 60).until(
+                        EC.element_to_be_clickable(CGPTV.chatgpt_textbox)
+                    )
+                    textbox.send_keys(char)
                 sleep(self._input_delay)
 
         textbox.send_keys(Keys.ENTER)
 
         self.logger.debug('Waiting for completion...')
         WebDriverWait(self.driver, timeout).until_not(
             EC.presence_of_element_located(CGPTV.chatgpt_streaming)
@@ -341,17 +345,15 @@
         
         pattern = re.compile(
             r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}'
         )
         matches = pattern.search(self.driver.current_url)
         if not matches:
             self.reset_conversation()
-            WebDriverWait(self.driver, 60).until(
-                EC.element_to_be_clickable(CGPTV.chatgpt_chats_list_first_node)
-            ).click()
+            self.driver.safe_click(CGPTV.chatgpt_chats_list_first_node, 60)
             sleep(0.5)
             matches = pattern.search(self.driver.current_url)
         try:
             conversation_id = matches.group() # type: ignore
         except:
             conversation_id = None
         return ChatGPTResponse(content, conversation_id)
@@ -361,33 +363,42 @@
         Resets the conversation.
         """
         if not self.driver.current_url.startswith(CGPTV.chatgpt_chat_url):
             return self.logger.debug('Current URL is not chat page, skipping reset')
 
         self.logger.debug('Resetting conversation...')
         try:
-            self.driver.find_element(*CGPTV.chatgpt_new_chat).click()
+            self.driver.safe_click(CGPTV.chatgpt_new_chat, 60)
         except NoSuchElementException:
             self.logger.debug('New chat button not found')
-            self.driver.save_screenshot('reset_conversation_failed.png')
+            return self._get_out_of_menu()
 
     def clear_conversations(self) -> None:
         """
         Clears all conversations.
         """
         self.logger.debug('Clearing all conversations...')
         try:
-            menu_button = self.driver.find_element(*CGPTV.chatgpt_menu_button)
-            menu_button.click()
-            clear_conversations = self.driver.find_element(*CGPTV.chatgpt_menu_clear_conversations)
-            clear_conversations.click()
-            clear_conversations.click() # Confirm button is the same path
+            menu_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_button, 60)
+            if not menu_button_clicked:
+                self.logger.debug('Could not click menu button')
+                return self._get_out_of_menu()
+            
+            clear_conversations_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_clear_conversations, 60)
+            if not clear_conversations_button_clicked:
+                self.logger.debug('Could not click clear conversations button')
+                return self._get_out_of_menu()
+            
+            confirm_clear_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_clear_conversations, 60)
+            if not confirm_clear_button_clicked:
+                self.logger.debug('Could not click confirm clear conversations button')
+                return self._get_out_of_menu()
         except NoSuchElementException:
             self.logger.debug('Could not find menu buttons')
-            self.driver.save_screenshot('clear_conversations_failed.png')
+            return self._get_out_of_menu()
 
     def switch_theme(self, theme: Literal['LIGHT', 'DARK', 'OPPOSITE', 'SYSTEM']) -> None:
         """
         Switch the theme.
 
         Args:
         ----------
@@ -418,35 +429,43 @@
             
             current_theme_value = self.driver.find_element(*CGPTV.chatgpt_outer_html).get_attribute('class')
             current_theme = 'LIGHT' if 'light' in current_theme_value else 'DARK'
             if theme == current_theme:
                 self.logger.debug('Theme is already set to the desired theme')
                 return self._get_out_of_menu()
 
-            select_element = self.driver.find_element(By.CSS_SELECTOR, 'select.rounded')
-            ActionChains(self.driver).move_to_element(select_element).click().perform()
+            select_element = self.driver.find_element(CGPTV.chatgpt_theme_select)
+            ActionChains(self.driver).move_to_element(select_element).perform()
+            select_clicked = self.driver.safe_click(CGPTV.chatgpt_theme_select, 60)
+            if not select_clicked:
+                self.logger.debug('Could not click theme select')
+                return self._get_out_of_menu()
 
             if theme == 'OPPOSITE':
                 if current_theme == 'SYSTEM':
                     self.logger.debug('Theme cannot be set to opposite of system theme')
                     return self._get_out_of_menu()
                     
                 opposite_theme = 'dark' if current_theme == 'LIGHT' else 'light'
-                option = self.driver.find_element(By.CSS_SELECTOR, f'select.rounded option[value={opposite_theme}]')
-                option.click()
+                option_clicked = self.driver.safe_click((By.CSS_SELECTOR, f'select.rounded option[value={opposite_theme}]'), 60)
+                if not option_clicked:
+                    self.logger.debug('Could not click opposite theme option')
+                    return self._get_out_of_menu()
                 self.logger.debug(f'Selected opposite theme of {current_theme}')
             else:
-                option = self.driver.find_element(By.CSS_SELECTOR, f'select.rounded option[value={theme.lower()}]')
-                option.click()
+                option_clicked = self.driver.safe_click((By.CSS_SELECTOR, f'select.rounded option[value={theme.lower()}]'), 60)
+                if not option_clicked:
+                    self.logger.debug('Could not click theme option')
+                    return self._get_out_of_menu()
                 self.logger.debug(f'Selected theme {theme}')
             
             self._get_out_of_menu()
         except NoSuchElementException:
             self.logger.debug('Could not find theme buttons')
-            self.driver.save_screenshot('theme_switch_failed.png')
+            return self._get_out_of_menu()
 
     def switch_account(self, session_token: str):
         """
         Switch the account.
 
         Args:
         ----------
@@ -549,33 +568,38 @@
             settings_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_settings_button)
             if not settings_button_clicked:
                 self.logger.debug('Could not click settings button')
                 return self._get_out_of_menu()
 
             self.logger.debug('Clicked settings button')
 
-            wait = WebDriverWait(self.driver, 20)
+            wait = WebDriverWait(self.driver, 60)
 
             # Click "Data controls" button
-            data_controls_button: WebElement = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button[data-state="inactive"][id^="radix-"][id$="-trigger-DataControls"]')))
-            data_controls_button.click()
+            data_controls_button_clicked = self.driver.safe_click(
+                CGPTV.chatgpt_menu_data_controls_button, 60
+            )
+            if not data_controls_button_clicked:
+                self.logger.debug('Could not click data controls button')
+                return self._get_out_of_menu()
 
             # Click "Disable chat history" button
+            # Not using safe_click because it there are some checks that need to be done before clicking
             chat_history_toggle = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, f'button[aria-label="Chat History & Training"]')))
             current_state = True if chat_history_toggle.get_attribute('aria-checked') == 'true' else False
             if current_state == state:
                 self.logger.debug('Chat history is already set to the desired state')
                 return self._get_out_of_menu()
-            
+
             chat_history_toggle.click()
             self.logger.debug(f'Chat history is now {"enabled" if state else "disabled"}')
             self._get_out_of_menu()
         except:
             self.logger.debug(f'Could not {"enable" if state else "disable"} chat history')
-            self.driver.save_screenshot('disable_chat_history_failed.png')
+            return self._get_out_of_menu()
     
     def regenerate_response(self, message_timeout: int = 240, click_timeout: int = 20) -> ChatGPTResponse:
         """
         Regenerate the response.
 
         Returns:
         ----------
@@ -589,18 +613,20 @@
             TimeoutException: If the click fails to succeed.
             ValueError: If the response is invalid.
             ValueError: If the response is not found.
         """
         self.logger.debug('Regenerating response...')
 
         # Click "Regenerate response" button
-        regenerate_response_button = WebDriverWait(self.driver, click_timeout).until(
-            EC.element_to_be_clickable(CGPTV.chatgpt_regenerate_response_button)
+        regenerate_response_button_clicked = self.driver.safe_click(
+            CGPTV.chatgpt_regenerate_response_button, click_timeout
         )
-        regenerate_response_button.click()
+        if not regenerate_response_button_clicked:
+            self.logger.debug('Could not click regenerate response button')
+            raise TimeoutException('Could not click regenerate response button')
 
         # Get the response, same way as send_message without the part of sending the message
         self.logger.debug('Waiting for completion...')
         WebDriverWait(self.driver, message_timeout).until_not(
             EC.presence_of_element_located(CGPTV.chatgpt_streaming)
         )
 
@@ -625,17 +651,18 @@
         
         pattern = re.compile(
             r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}'
         )
         matches = pattern.search(self.driver.current_url)
         if not matches:
             self.reset_conversation()
-            WebDriverWait(self.driver, 60).until(
-                EC.element_to_be_clickable(CGPTV.chatgpt_chats_list_first_node)
-            ).click()
+            list_first_node_clicked = self.driver.safe_click(CGPTV.chatgpt_chats_list_first_node, 60)
+            if not list_first_node_clicked:
+                self.logger.debug('Could not click chats list first node')
+                raise TimeoutException('Could not click chats list first node')
             sleep(0.5)
             matches = pattern.search(self.driver.current_url)
         try:
             conversation_id = matches.group() # type: ignore
         except:
             conversation_id = None
         self.logger.debug('Regenerated response')
```

### Comparing `UnlimitedGPT-0.1.0/UnlimitedGPT/internal/chatgpt_data.py` & `UnlimitedGPT-0.1.1/UnlimitedGPT/internal/chatgpt_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,9 +63,13 @@
         By.XPATH,
         "/html/body/div[5]/div/div/div/div[2]/div/div[2]/div/div[1]/div/select"
     )
     chatgpt_regenerate_response_button = (
         By.XPATH,
         "/html/body/div[1]/div[2]/div[2]/div/main/div[3]/form/div/div[1]/div/button"
     )
+    chatgpt_theme_select = (
+        By.CSS_SELECTOR,
+        'select.rounded'
+    )
 
     chatgpt_chat_url = 'https://chat.openai.com/chat'
```

### Comparing `UnlimitedGPT-0.1.0/UnlimitedGPT/internal/driver.py` & `UnlimitedGPT-0.1.1/UnlimitedGPT/internal/driver.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.0/UnlimitedGPT/internal/objects.py` & `UnlimitedGPT-0.1.1/UnlimitedGPT/internal/objects.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.0/UnlimitedGPT.egg-info/PKG-INFO` & `UnlimitedGPT-0.1.1/UnlimitedGPT.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.0
+Version: 0.1.1
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
+Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `UnlimitedGPT-0.1.0/setup.py` & `UnlimitedGPT-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 setup(
     name='UnlimitedGPT',
     author='Sxvxge',
     url='https://github.com/Sxvxgee/UnlimitedGPT',
     project_urls={
         'Documentation': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md',
         'Issue tracker': 'https://github.com/Sxvxgee/UnlimitedGPT/issues',
+        'Changelog': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md',
     },
-    version="0.1.0",
+    version="0.1.1",
     packages=['UnlimitedGPT', 'UnlimitedGPT/internal'],
     py_modules=['UnlimitedGPT'],
     license='GPL-3.0 license',
     description='An unofficial Python wrapper for OpenAI\'s ChatGPT API',
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
```

