# Comparing `tmp/twAuto-0.3.4.tar.gz` & `tmp/twAuto-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\twAuto-0.3.4.tar", last modified: Tue Feb 21 03:06:24 2023, max compression
+gzip compressed data, was "twAuto-0.3.5.tar", last modified: Wed May 31 11:12:55 2023, max compression
```

## Comparing `twAuto-0.3.4.tar` & `twAuto-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 03:06:24.723361 twAuto-0.3.4/
--rw-rw-rw-   0        0        0     1107 2023-02-18 22:19:42.000000 twAuto-0.3.4/LICENCE.MD
--rw-rw-rw-   0        0        0       67 2023-02-18 22:19:42.000000 twAuto-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4782 2023-02-21 03:06:24.722364 twAuto-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     4449 2023-02-21 03:05:55.000000 twAuto-0.3.4/README.md
--rw-rw-rw-   0        0        0       42 2023-02-21 03:06:24.723361 twAuto-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-02-21 03:05:59.000000 twAuto-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-21 03:06:24.539843 twAuto-0.3.4/twAuto/
--rw-rw-rw-   0        0        0       28 2023-02-18 22:19:42.000000 twAuto-0.3.4/twAuto/__init__.py
--rw-rw-rw-   0        0        0    31088 2023-02-21 03:05:18.000000 twAuto-0.3.4/twAuto/twauto.py
-drwxrwxrwx   0        0        0        0 2023-02-21 03:06:24.715389 twAuto-0.3.4/twAuto.egg-info/
--rw-rw-rw-   0        0        0     4782 2023-02-21 03:06:24.000000 twAuto-0.3.4/twAuto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-02-21 03:06:24.000000 twAuto-0.3.4/twAuto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 03:06:24.000000 twAuto-0.3.4/twAuto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-02-21 03:06:24.000000 twAuto-0.3.4/twAuto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-21 03:06:24.000000 twAuto-0.3.4/twAuto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:55.517353 twAuto-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-31 11:12:40.000000 twAuto-0.3.5/LICENCE.MD
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-31 11:12:40.000000 twAuto-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-31 11:12:55.517353 twAuto-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-31 11:12:40.000000 twAuto-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 11:12:55.517353 twAuto-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-31 11:12:40.000000 twAuto-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:55.517353 twAuto-0.3.5/twAuto/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 11:12:40.000000 twAuto-0.3.5/twAuto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31693 2023-05-31 11:12:40.000000 twAuto-0.3.5/twAuto/twauto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:55.517353 twAuto-0.3.5/twAuto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-31 11:12:55.000000 twAuto-0.3.5/twAuto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-31 11:12:55.000000 twAuto-0.3.5/twAuto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:12:55.000000 twAuto-0.3.5/twAuto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 11:12:55.000000 twAuto-0.3.5/twAuto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 11:12:55.000000 twAuto-0.3.5/twAuto.egg-info/top_level.txt
```

### Comparing `twAuto-0.3.4/LICENCE.MD` & `twAuto-0.3.5/LICENCE.MD`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) <year> <copyright holders>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+The MIT License (MIT)
+
+Copyright (c) <year> <copyright holders>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
```

### Comparing `twAuto-0.3.4/PKG-INFO` & `twAuto-0.3.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,221 +1,211 @@
-Metadata-Version: 2.1
-Name: twAuto
-Version: 0.3.4
-Summary: TwAuto is a library for testing your code on pre-Twitter API application stage.
-Home-page: https://github.com/EKOzkan/twAuto
-Author: Ekin Kagan Ozkan
-Author-email: ekinkagan@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENCE.MD
-
-# twAuto - Twitter Automation Tool v0.3.4 🦆
-
-twAuto is a library for "Tweeting", "Retweeting", "Replying", "Tweet Quoting", "Tweet Liking" without any API requirements using Selenium.
-
-<br/>
-
-Note: While using this library I didnt encounter any problems/bad response from Twitter like banning account etc. but please use at your own risk.
-
-## Requirements
-
-- Python 3.7+
-
-- [beautifulsoup4](https://pypi.org/project/beautifulsoup4/)
-
-- [selenium](https://pypi.org/project/selenium/)
-
-- [webdriver-manager](https://pypi.org/project/webdriver-manager/)
-
-## Installation
-
-**Pip:**
-
-```bash
-pip3 install twAuto
-```
-
-## Functions
-
-**- Import:**
-
-```python
-import twAuto
-```
-
-<br/>
-
-**- Configure:**
-
-```python
-tw = twAuto.twAuto(
-  username="Your Twitter Username",
-  email="Your Twitter E-Mail",
-  password="Your Twitter Password",
-  chromeDriverMode="manual" or "auto", #if you use auto twAuto will automatically download the chrome driver for you,
-                                       #if you use the manual option, you need to provide the driver path in driverPath parameter.
-  pathType="testId" or "xPath", #It is testId by default. If you had any problems with library you can try the xPath mode too.
-  headless=True/False, #Headless is true by default.
-  debugMode= True/False #Really poorly implemented debug mode, this is for reading occured errors.
-                        #It is not realiable right now but you can give it a try if you want to.
-)
-
-```
-
-<br/>
-
-**- Start:** Start functions runs the selenium driver.
-
-```python
-tw.start()
-```
-
-<br/>
-
-**- Login:** Logs in to the Twitter account
-
-```python
-tw.login()
-```
-
-<br/>
-
-**- Login Errors:** If you encounter any error in the login process, you can use manualCookieCreation() to get your cookie file manually.
-Run the function after tw.start() line. Then after the browser window opened, login to account you want to automate, then enter any character in the terminal. This will create a cookie file after this, you can use the library.
-
-Note: Headless must be False to use this function.
-
-```python
-tw.manualCookieCreation()
-```
-
-Example:
-
-First run this code to get your cookie file.
-
-```python
-tw = twAuto.twAuto(
-  username="Your Twitter Username",
-  email="Your Twitter E-Mail",
-  password="Your Twitter Password",
-  chromeDriverMode="auto",
-  pathType="xPath",
-  headless=False #Headless must be False to use this function.
-)
-
-tw.start()
-tw.manualCookieCreation()
-```
-
-After doing the steps that is described above, you can run your main code.
-
-```python
-tw = twAuto.twAuto(
-  username="Your Twitter Username",
-  email="Your Twitter E-Mail",
-  password="Your Twitter Password",
-  chromeDriverMode="auto",
-  pathType="xPath"
-)
-
-tw.start()
-tw.login()
-#other functions...
-```
-
-<br/>
-
-**- Like:** Likes tweet in the given url \
-->Returns: True/False as Success/Failed
-
-```python
-tw.like(url="")
-```
-
-<br/>
-
-**- Reply:** Replies to the tweet in the given url with given text.\
-->Returns: Reply URL/False
-
-```python
-tw.reply(url="", imgpath="", text="")
-```
-
-<br/>
-
-**- Tweet:** Tweets the text and image if given.\
-->Returns: Tweet URL/False
-
-```python
-tw.tweet(text="",imgpath="")
-```
-
-<br/>
-
-**- Quote Tweet:** Quotes the tweet in the given url with the given text.\
-->Returns: Quoted Tweet URL/False
-
-```python
-tw.quoteTweet(url="", imgpath="" ,text="")
-```
-
-<br/>
-
-**- Retweet:** Retweets the tweet in the given url.\
-->Returns: True/False as Success/Failed
-
-```python
-tw.retweet(url="")
-```
-
-<br/>
-
-**- Unretweet:** Unretweets the tweet in the given url.\
-->Returns: True/False as Success/Failed
-
-```python
-tw.unretweet(url="")
-```
-
-<br/>
-
-**- Logout:** Logs out from current Twitter account and deletes the cookies file.
-
-```python
-tw.logout()
-```
-
-<br/>
-
-**- Quit/Close:** Ends the session, closes the selenium driver application
-
-```python
-tw.close()
-```
-
-## Example Code
-
-```python
-tw = twAuto.twAuto(
-  username="",
-  email="",
-  password="",
-  headless=True,
-  chromeDriverMode="auto",
-  pathType="testId")
-
-tw.start()
-tw.login()
-
-tw.reply(url="",imgpath="", text="")
-
-tw.close()
-
-```
-
-## To Do's 📝 :
-
-- [x] Send image with Quote, Reply.
-- [ ] Send gif with Quote, Reply.
-- [x] Retweet without adding url at the end.
-- [ ] Linux integration(not tested yet).
+# twAuto - Twitter Automation Tool v0.3.4 🦆
+
+twAuto is a library for "Tweeting", "Retweeting", "Replying", "Tweet Quoting", "Tweet Liking" without any API requirements using Selenium.
+
+<br/>
+
+Note: While using this library I didnt encounter any problems/bad response from Twitter like banning account etc. but please use at your own risk.
+
+## Requirements
+
+- Python 3.7+
+
+- [beautifulsoup4](https://pypi.org/project/beautifulsoup4/)
+
+- [selenium](https://pypi.org/project/selenium/)
+
+- [webdriver-manager](https://pypi.org/project/webdriver-manager/)
+
+## Installation
+
+**Pip:**
+
+```bash
+pip3 install twAuto
+```
+
+## Functions
+
+**- Import:**
+
+```python
+import twAuto
+```
+
+<br/>
+
+**- Configure:**
+
+```python
+tw = twAuto.twAuto(
+  username="Your Twitter Username",
+  email="Your Twitter E-Mail",
+  password="Your Twitter Password",
+  chromeDriverMode="manual" or "auto", #if you use auto twAuto will automatically download the chrome driver for you,
+                                       #if you use the manual option, you need to provide the driver path in driverPath parameter.
+  driverPath="your drivers path", #use only if you are using the chromeDriverMode in manual mode 
+  pathType="testId" or "xPath", #It is xPath by default. I highly recommend you to use testId instead of xPath. If you had any problems with library you can try the xPath mode too.
+  headless=True/False, #Headless is true by default.
+  debugMode= True/False #Really poorly implemented debug mode, this is for reading occured errors.
+                        #It is not reliable right now but you can give it a try if you want to.
+)
+
+```
+
+<br/>
+
+**- Start:** Start functions runs the selenium driver.
+
+```python
+tw.start()
+```
+
+<br/>
+
+**- Login:** Logs in to the Twitter account
+
+```python
+tw.login()
+```
+
+<br/>
+
+**- Login Errors:** If you encounter any errors in the login process, you can use manualCookieCreation() to get your cookie file manually.
+Run the function after tw.start() line. Then after the browser window opened, login to account you want to automate, then enter any character in the terminal. This will create a cookie file after this, you can use the library.
+
+Note: Headless must be False to use this function.
+
+```python
+tw.manualCookieCreation()
+```
+
+Example:
+
+First run this code to get your cookie file.
+
+```python
+tw = twAuto.twAuto(
+  username="Your Twitter Username",
+  email="Your Twitter E-Mail",
+  password="Your Twitter Password",
+  chromeDriverMode="auto",
+  pathType="xPath",
+  headless=False #Headless must be False to use this function.
+)
+
+tw.start()
+tw.manualCookieCreation()
+```
+
+After doing the steps that is described above, you can run your main code.
+
+```python
+tw = twAuto.twAuto(
+  username="Your Twitter Username",
+  email="Your Twitter E-Mail",
+  password="Your Twitter Password",
+  chromeDriverMode="auto",
+  pathType="xPath"
+)
+
+tw.start()
+tw.login()
+#other functions...
+```
+
+<br/>
+
+**- Like:** Likes tweet in the given url \
+->Returns: True/False as Success/Failed
+
+```python
+tw.like(url="")
+```
+
+<br/>
+
+**- Reply:** Replies to the tweet in the given url with given text.\
+->Returns: Reply URL/False
+
+```python
+tw.reply(url="", imgpath="", text="")
+```
+
+<br/>
+
+**- Tweet:** Tweets the text and image if given.\
+->Returns: Tweet URL/False
+
+```python
+tw.tweet(text="",imgpath="")
+```
+
+<br/>
+
+**- Quote Tweet:** Quotes the tweet in the given url with the given text.\
+->Returns: Quoted Tweet URL/False
+
+```python
+tw.quoteTweet(url="", imgpath="" ,text="")
+```
+
+<br/>
+
+**- Retweet:** Retweets the tweet in the given url.\
+->Returns: True/False as Success/Failed
+
+```python
+tw.retweet(url="")
+```
+
+<br/>
+
+**- Unretweet:** Unretweets the tweet in the given url.\
+->Returns: True/False as Success/Failed
+
+```python
+tw.unretweet(url="")
+```
+
+<br/>
+
+**- Logout:** Logs out from current Twitter account and deletes the cookies file.
+
+```python
+tw.logout()
+```
+
+<br/>
+
+**- Quit/Close:** Ends the session, closes the selenium driver application
+
+```python
+tw.close()
+```
+
+## Example Code
+
+```python
+tw = twAuto.twAuto(
+  username="",
+  email="",
+  password="",
+  headless=True,
+  chromeDriverMode="auto",
+  pathType="testId")
+
+tw.start()
+tw.login()
+
+tw.reply(url="",imgpath="", text="")
+
+tw.close()
+
+```
+
+## To Do's 📝 :
+
+- [x] Send image with Quote, Reply.
+- [ ] Send gif with Quote, Reply.
+- [x] Retweet without adding url at the end.
+- [ ] Linux integration(not tested yet).
```

### Comparing `twAuto-0.3.4/README.md` & `twAuto-0.3.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,210 +1,222 @@
-# twAuto - Twitter Automation Tool v0.3.4 🦆
-
-twAuto is a library for "Tweeting", "Retweeting", "Replying", "Tweet Quoting", "Tweet Liking" without any API requirements using Selenium.
-
-<br/>
-
-Note: While using this library I didnt encounter any problems/bad response from Twitter like banning account etc. but please use at your own risk.
-
-## Requirements
-
-- Python 3.7+
-
-- [beautifulsoup4](https://pypi.org/project/beautifulsoup4/)
-
-- [selenium](https://pypi.org/project/selenium/)
-
-- [webdriver-manager](https://pypi.org/project/webdriver-manager/)
-
-## Installation
-
-**Pip:**
-
-```bash
-pip3 install twAuto
-```
-
-## Functions
-
-**- Import:**
-
-```python
-import twAuto
-```
-
-<br/>
-
-**- Configure:**
-
-```python
-tw = twAuto.twAuto(
-  username="Your Twitter Username",
-  email="Your Twitter E-Mail",
-  password="Your Twitter Password",
-  chromeDriverMode="manual" or "auto", #if you use auto twAuto will automatically download the chrome driver for you,
-                                       #if you use the manual option, you need to provide the driver path in driverPath parameter.
-  pathType="testId" or "xPath", #It is testId by default. If you had any problems with library you can try the xPath mode too.
-  headless=True/False, #Headless is true by default.
-  debugMode= True/False #Really poorly implemented debug mode, this is for reading occured errors.
-                        #It is not realiable right now but you can give it a try if you want to.
-)
-
-```
-
-<br/>
-
-**- Start:** Start functions runs the selenium driver.
-
-```python
-tw.start()
-```
-
-<br/>
-
-**- Login:** Logs in to the Twitter account
-
-```python
-tw.login()
-```
-
-<br/>
-
-**- Login Errors:** If you encounter any error in the login process, you can use manualCookieCreation() to get your cookie file manually.
-Run the function after tw.start() line. Then after the browser window opened, login to account you want to automate, then enter any character in the terminal. This will create a cookie file after this, you can use the library.
-
-Note: Headless must be False to use this function.
-
-```python
-tw.manualCookieCreation()
-```
-
-Example:
-
-First run this code to get your cookie file.
-
-```python
-tw = twAuto.twAuto(
-  username="Your Twitter Username",
-  email="Your Twitter E-Mail",
-  password="Your Twitter Password",
-  chromeDriverMode="auto",
-  pathType="xPath",
-  headless=False #Headless must be False to use this function.
-)
-
-tw.start()
-tw.manualCookieCreation()
-```
-
-After doing the steps that is described above, you can run your main code.
-
-```python
-tw = twAuto.twAuto(
-  username="Your Twitter Username",
-  email="Your Twitter E-Mail",
-  password="Your Twitter Password",
-  chromeDriverMode="auto",
-  pathType="xPath"
-)
-
-tw.start()
-tw.login()
-#other functions...
-```
-
-<br/>
-
-**- Like:** Likes tweet in the given url \
-->Returns: True/False as Success/Failed
-
-```python
-tw.like(url="")
-```
-
-<br/>
-
-**- Reply:** Replies to the tweet in the given url with given text.\
-->Returns: Reply URL/False
-
-```python
-tw.reply(url="", imgpath="", text="")
-```
-
-<br/>
-
-**- Tweet:** Tweets the text and image if given.\
-->Returns: Tweet URL/False
-
-```python
-tw.tweet(text="",imgpath="")
-```
-
-<br/>
-
-**- Quote Tweet:** Quotes the tweet in the given url with the given text.\
-->Returns: Quoted Tweet URL/False
-
-```python
-tw.quoteTweet(url="", imgpath="" ,text="")
-```
-
-<br/>
-
-**- Retweet:** Retweets the tweet in the given url.\
-->Returns: True/False as Success/Failed
-
-```python
-tw.retweet(url="")
-```
-
-<br/>
-
-**- Unretweet:** Unretweets the tweet in the given url.\
-->Returns: True/False as Success/Failed
-
-```python
-tw.unretweet(url="")
-```
-
-<br/>
-
-**- Logout:** Logs out from current Twitter account and deletes the cookies file.
-
-```python
-tw.logout()
-```
-
-<br/>
-
-**- Quit/Close:** Ends the session, closes the selenium driver application
-
-```python
-tw.close()
-```
-
-## Example Code
-
-```python
-tw = twAuto.twAuto(
-  username="",
-  email="",
-  password="",
-  headless=True,
-  chromeDriverMode="auto",
-  pathType="testId")
-
-tw.start()
-tw.login()
-
-tw.reply(url="",imgpath="", text="")
-
-tw.close()
-
-```
-
-## To Do's 📝 :
-
-- [x] Send image with Quote, Reply.
-- [ ] Send gif with Quote, Reply.
-- [x] Retweet without adding url at the end.
-- [ ] Linux integration(not tested yet).
+Metadata-Version: 2.1
+Name: twAuto
+Version: 0.3.5
+Summary: TwAuto is a library for testing your code on pre-Twitter API application stage.
+Home-page: https://github.com/EKOzkan/twAuto
+Author: Ekin Kagan Ozkan
+Author-email: ekinkagan@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENCE.MD
+
+# twAuto - Twitter Automation Tool v0.3.4 🦆
+
+twAuto is a library for "Tweeting", "Retweeting", "Replying", "Tweet Quoting", "Tweet Liking" without any API requirements using Selenium.
+
+<br/>
+
+Note: While using this library I didnt encounter any problems/bad response from Twitter like banning account etc. but please use at your own risk.
+
+## Requirements
+
+- Python 3.7+
+
+- [beautifulsoup4](https://pypi.org/project/beautifulsoup4/)
+
+- [selenium](https://pypi.org/project/selenium/)
+
+- [webdriver-manager](https://pypi.org/project/webdriver-manager/)
+
+## Installation
+
+**Pip:**
+
+```bash
+pip3 install twAuto
+```
+
+## Functions
+
+**- Import:**
+
+```python
+import twAuto
+```
+
+<br/>
+
+**- Configure:**
+
+```python
+tw = twAuto.twAuto(
+  username="Your Twitter Username",
+  email="Your Twitter E-Mail",
+  password="Your Twitter Password",
+  chromeDriverMode="manual" or "auto", #if you use auto twAuto will automatically download the chrome driver for you,
+                                       #if you use the manual option, you need to provide the driver path in driverPath parameter.
+  driverPath="your drivers path", #use only if you are using the chromeDriverMode in manual mode 
+  pathType="testId" or "xPath", #It is xPath by default. I highly recommend you to use testId instead of xPath. If you had any problems with library you can try the xPath mode too.
+  headless=True/False, #Headless is true by default.
+  debugMode= True/False #Really poorly implemented debug mode, this is for reading occured errors.
+                        #It is not reliable right now but you can give it a try if you want to.
+)
+
+```
+
+<br/>
+
+**- Start:** Start functions runs the selenium driver.
+
+```python
+tw.start()
+```
+
+<br/>
+
+**- Login:** Logs in to the Twitter account
+
+```python
+tw.login()
+```
+
+<br/>
+
+**- Login Errors:** If you encounter any errors in the login process, you can use manualCookieCreation() to get your cookie file manually.
+Run the function after tw.start() line. Then after the browser window opened, login to account you want to automate, then enter any character in the terminal. This will create a cookie file after this, you can use the library.
+
+Note: Headless must be False to use this function.
+
+```python
+tw.manualCookieCreation()
+```
+
+Example:
+
+First run this code to get your cookie file.
+
+```python
+tw = twAuto.twAuto(
+  username="Your Twitter Username",
+  email="Your Twitter E-Mail",
+  password="Your Twitter Password",
+  chromeDriverMode="auto",
+  pathType="xPath",
+  headless=False #Headless must be False to use this function.
+)
+
+tw.start()
+tw.manualCookieCreation()
+```
+
+After doing the steps that is described above, you can run your main code.
+
+```python
+tw = twAuto.twAuto(
+  username="Your Twitter Username",
+  email="Your Twitter E-Mail",
+  password="Your Twitter Password",
+  chromeDriverMode="auto",
+  pathType="xPath"
+)
+
+tw.start()
+tw.login()
+#other functions...
+```
+
+<br/>
+
+**- Like:** Likes tweet in the given url \
+->Returns: True/False as Success/Failed
+
+```python
+tw.like(url="")
+```
+
+<br/>
+
+**- Reply:** Replies to the tweet in the given url with given text.\
+->Returns: Reply URL/False
+
+```python
+tw.reply(url="", imgpath="", text="")
+```
+
+<br/>
+
+**- Tweet:** Tweets the text and image if given.\
+->Returns: Tweet URL/False
+
+```python
+tw.tweet(text="",imgpath="")
+```
+
+<br/>
+
+**- Quote Tweet:** Quotes the tweet in the given url with the given text.\
+->Returns: Quoted Tweet URL/False
+
+```python
+tw.quoteTweet(url="", imgpath="" ,text="")
+```
+
+<br/>
+
+**- Retweet:** Retweets the tweet in the given url.\
+->Returns: True/False as Success/Failed
+
+```python
+tw.retweet(url="")
+```
+
+<br/>
+
+**- Unretweet:** Unretweets the tweet in the given url.\
+->Returns: True/False as Success/Failed
+
+```python
+tw.unretweet(url="")
+```
+
+<br/>
+
+**- Logout:** Logs out from current Twitter account and deletes the cookies file.
+
+```python
+tw.logout()
+```
+
+<br/>
+
+**- Quit/Close:** Ends the session, closes the selenium driver application
+
+```python
+tw.close()
+```
+
+## Example Code
+
+```python
+tw = twAuto.twAuto(
+  username="",
+  email="",
+  password="",
+  headless=True,
+  chromeDriverMode="auto",
+  pathType="testId")
+
+tw.start()
+tw.login()
+
+tw.reply(url="",imgpath="", text="")
+
+tw.close()
+
+```
+
+## To Do's 📝 :
+
+- [x] Send image with Quote, Reply.
+- [ ] Send gif with Quote, Reply.
+- [x] Retweet without adding url at the end.
+- [ ] Linux integration(not tested yet).
```

### Comparing `twAuto-0.3.4/setup.py` & `twAuto-0.3.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='twAuto',
-    version='0.3.4',
-    packages=find_packages(exclude=['tests*']),
-    license='MIT',
-    description='TwAuto is a library for testing your code on pre-Twitter API application stage.',
-    long_description=open('README.md',  encoding="utf8").read(),
-    long_description_content_type='text/markdown',
-    install_requires=['selenium', 'bs4', 'webdriver-manager'],
-    url='https://github.com/EKOzkan/twAuto',
-    author='Ekin Kagan Ozkan',
-    author_email='ekinkagan@gmail.com'
-)
+from setuptools import setup, find_packages
+
+setup(
+    name='twAuto',
+    version='0.3.5',
+    packages=find_packages(exclude=['tests*']),
+    license='MIT',
+    description='TwAuto is a library for testing your code on pre-Twitter API application stage.',
+    long_description=open('README.md',  encoding="utf8").read(),
+    long_description_content_type='text/markdown',
+    install_requires=['selenium', 'bs4', 'webdriver-manager'],
+    url='https://github.com/EKOzkan/twAuto',
+    author='Ekin Kagan Ozkan',
+    author_email='ekinkagan@gmail.com'
+)
```

### Comparing `twAuto-0.3.4/twAuto/twauto.py` & `twAuto-0.3.5/twAuto/twauto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,621 +1,637 @@
-import pickle
-from selenium import webdriver
-from selenium.webdriver.common.keys import Keys
-from selenium.common.exceptions import TimeoutException
-from selenium.webdriver.support.ui import WebDriverWait
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.common.by import By
-import time
-from socket import timeout
-from os.path import exists
-import os
-import requests
-import bs4
-from bs4 import BeautifulSoup
-from urllib import request
-
-from selenium.webdriver.chrome.service import Service as ChromiumService
-from webdriver_manager.chrome import ChromeDriverManager
-from webdriver_manager.core.utils import ChromeType
-
-class twAuto:
-    driver = None
-    cookies_exists = exists('cookies.pkl')
-    chrome_options = webdriver.ChromeOptions()
-    chrome_options.add_argument("--disable-extensions")
-    chrome_options.add_argument('--disable-gpu')
-    chrome_options.add_argument('--ignore-certificate-errors')
-    chrome_options.add_experimental_option(
-        "excludeSwitches", ["enable-logging"])
-
-    def __init__(
-        self,
-        password="",
-        username="",
-        email="",
-        headless=True,
-        debugMode=False,
-        chromeDriverMode="auto", #manual or auto
-        driverPath = "./chrome.exe", #if you use manual, pass the driverPath
-        pathType = "xPath" #xPath or testId
-    ):
-        self.email = email
-        self.username = username
-        self.password = password
-        self.chromeDriverMode = chromeDriverMode
-        self.driverPath = driverPath
-        self.pathType = pathType
-        self.headless = headless
-        self.debugMode = debugMode
-        if headless:
-            twAuto.chrome_options.add_argument('--headless')
-        if debugMode:
-            print("twAuto started.")
-
-    # start selenium driver
-    def start(self):
-        try:
-            if self.chromeDriverMode == "auto":
-                twAuto.driver = webdriver.Chrome(ChromeDriverManager().install(), options=twAuto.chrome_options)
-            else:
-                twAuto.driver = webdriver.Chrome(self.driverPath, options=twAuto.chrome_options)
-        except Exception as e:
-            if self.debugMode:
-                print("twAuto Error: ", e)
-    # test function to open twitter on chrome
-    def openTw(self):
-        twAuto.driver.get("https://twitter.com/home")
-
-    # login to twitter
-    def login(self):
-        try:
-            twAuto.driver.get("https://twitter.com/")
-            # this cookie importing prevents 'New login notification" in every action
-            if twAuto.cookies_exists:
-                cookies = pickle.load(open("cookies.pkl", "rb"))
-                for cookie in cookies:
-                    twAuto.driver.add_cookie(cookie)
-            if twAuto.cookies_exists:
-                twAuto.driver.get("https://twitter.com/")
-            else:
-                twAuto.driver.get("https://twitter.com/login")
-                try:
-                    wait = WebDriverWait(twAuto.driver, 120)
-                    wait.until(EC.presence_of_element_located(
-                        (By.XPATH, "//*[@id='layers']/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div/div/div/div[5]/label/div/div[2]/div/input")))
-                except TimeoutException:
-                    pass
-                mailInput = twAuto.driver.find_element(
-                    'xpath', "//*[@id='layers']/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div/div/div/div[5]/label/div/div[2]/div/input")
-                mailInput.send_keys(self.email)
-                twAuto.driver.find_element(
-                    'xpath', "//div[@class='css-18t94o4 css-1dbjc4n r-sdzlij r-1phboty r-rs99b7 r-ywje51 r-usiww2 r-2yi16 r-1qi8awa r-1ny4l3l r-ymttw5 r-o7ynqc r-6416eg r-lrvibr r-13qz1uu']").click()
-                time.sleep(3)
-
-                try:
-                    userNameInput = twAuto.driver.find_element(
-                        'xpath', "/html/body/div/div/div/div[1]/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div[1]/div/div/div[3]/div/label/div/div[2]/div[1]/input")
-                except:
-                    userNameInput = twAuto.driver.find_element(
-                        'xpath', "/html/body/div/div/div/div[1]/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div[1]/div/div[2]/label/div/div[2]/div/input")
-
-                userNameInput.send_keys(self.username)
-
-                twAuto.driver.find_element(
-                    'xpath', "//*[@id='layers']/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div[2]/div/div/div/div").click()
-
-                try:
-                    wait = WebDriverWait(twAuto.driver, 120)
-                    wait.until(EC.presence_of_element_located(
-                        (By.XPATH, "//*[@id='layers']/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div[1]/div/div/div[3]/div/label/div/div[2]/div[1]/input")))
-                except TimeoutException:
-                    pass
-                passwordInput = twAuto.driver.find_element(
-                    'xpath', "//*[@id='layers']/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div[1]/div/div/div[3]/div/label/div/div[2]/div[1]/input")
-                passwordInput.send_keys(self.password)
-                twAuto.driver.find_element(
-                    'xpath', "//*[@id='layers']/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div[2]/div/div[1]/div/div/div").click()
-
-            try:
-                wait = WebDriverWait(twAuto.driver, 120)
-                wait.until(EC.presence_of_element_located(
-                    (By.XPATH, "//*[@id='react-root']/div/div/div[2]/header/div/div/div/div[1]/div[2]/nav/a[1]")))
-                print("Succesfully Logged In")
-            except Exception as e:
-                if self.debugMode:
-                    print("twAuto Error: ", e)
-
-            twAuto.driver.get("https://twitter.com/Twitter/")
-
-            if not twAuto.cookies_exists:
-                pickle.dump(twAuto.driver.get_cookies(), open("cookies.pkl", "wb"))
-                
-        except Exception as e:
-            if self.debugMode:
-                    print("twAuto Error: ", e)
-            return False   
-
-    #this functions is for the ones that having trouble in the login process, 
-    #you must pass the headless parameter as true to use this function
-    #after you login manually, open the console window and enter any key to continue
-    #this function will save the cookies to the cookies.pkl file
-    #and after that you can use the login function and module without any problem
-    def manualCookieCreation(self):
-        if not self.headless:
-            twAuto.driver.get("https://twitter.com/login")
-            input("Please login to your account. After you login, press any key to save your cookies to current folder.")
-            pickle.dump(twAuto.driver.get_cookies(), open("cookies.pkl", "wb"))
-        else:
-            print("Please pass the headless parameter as False to use this function")
-            sleep(3)
-            self.close()
-
-    # tweet text
-    def tweet(self, imgpath=None, text=""):
-        # load tweeting page
-        twAuto.driver.get("https://twitter.com/home")
-        twAuto.driver.get('https://twitter.com/compose/tweet')
-
-
-        if self.pathType=="xPath":
-            try:
-                # try finding tweet inbox
-                try:
-                    wait = WebDriverWait(twAuto.driver, 120)
-                    wait.until(EC.presence_of_element_located(
-                        (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[1]/div/div/div/div/div/div[2]/div/div/div/div/label/div[1]/div/div/div/div/div/div[2]/div")))
-                except TimeoutException:
-                    print('Couldnt tweet.')
-
-                # modify tweet text
-                full_text = text
-
-                input_field = twAuto.driver.find_element(
-                    'xpath', "//*[@id='layers']/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[1]/div/div/div/div/div/div[2]/div/div/div/div/label/div[1]/div/div/div/div/div/div[2]/div")
-                input_field.send_keys(full_text)
-
-                try:
-                    wait = WebDriverWait(twAuto.driver, 120)
-                    wait.until(EC.presence_of_element_located(
-                        (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[3]/div/div/div[2]/div[4]")))
-                except TimeoutException:
-                    print('Couldnt tweet.')
-                    
-                if imgpath != None:
-                    element = twAuto.driver.find_element(
-                        By.XPATH, "//input[@type='file']")
-                    '''//*[@id="layers"]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[3]/div/div/div[1]/div[1]'''
-                    twAuto.driver.execute_script(
-                        "arguments[0].style.display = 'block';", element)
-
-                    element.send_keys(imgpath)
-
-                twAuto.driver.find_element(By.XPATH,
-                                        '//*[@id="layers"]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[3]/div/div/div[2]/div[4]').click()
-                try:
-                    wait = WebDriverWait(twAuto.driver, 5)
-                    wait.until(EC.presence_of_element_located(
-                        (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span")))
-                    twAuto.driver.find_element(
-                        'xpath', "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span").click()
-                    tweetUrl = twAuto.driver.current_url
-                    print("Tweeted Successfully")
-                    print("Tweet URL:"+tweetUrl)
-                    return tweetUrl
-                except TimeoutException:
-                    try:
-                        twAuto.driver.find_element(
-                            'xpath', "//*[@id='layers']/div[3]/div/div/div/div/div[1]")
-                        print('Couldnt Tweet.')
-                        return None
-                    except:
-                        try:
-                            wait = WebDriverWait(twAuto.driver, 5)
-                            wait.until(EC.presence_of_element_located(
-                                (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span")))
-                            twAuto.driver.find_element(
-                                By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span").click()
-                            tweetUrl = twAuto.driver.current_url
-                            print("Tweeted Successfully")
-                            print("Tweet URL:"+tweetUrl)
-                        except:
-                            print('Couldnt Tweet.')
-                            return None
-            except Exception as e:
-                if self.debugMode:
-                    print("twAuto Error: ", e)
-                return False
-
-        if self.pathType == "testId":
-            try:
-                # try finding tweet inbox
-                try:
-                    wait = WebDriverWait(twAuto.driver, 120)
-                    wait.until(EC.presence_of_element_located(
-                        (By.XPATH, '//div[@data-testid="tweetTextarea_0"]')))
-                except TimeoutException:
-                    print('Couldnt tweet.')
-                
-                # modify tweet text
-                full_text = text
-                
-                input_field = twAuto.driver.find_element(
-                    'xpath', '//div[@data-testid="tweetTextarea_0"]')
-                input_field.send_keys(full_text)
-                
-                try:
-                    wait = WebDriverWait(twAuto.driver, 120)
-                    wait.until(EC.presence_of_element_located((By.XPATH, '//div[@data-testid="tweetButton"]')))
-                    
-                except TimeoutException:
-                    print('Couldnt tweet.' )
-                
-                if imgpath != None:
-                    element = twAuto.driver.find_element(
-                        By.XPATH, "//input[@type='file']")
-
-                    twAuto.driver.execute_script(
-                        "arguments[0].style.display = 'block';", element)
-
-                    element.send_keys(imgpath)
-                
-                #find tweet button
-                tweetButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetButton"]')
-                
-                #click tweet button
-                twAuto.driver.execute_script("arguments[0].click()", tweetButton)
-
-                try:
-                    wait = WebDriverWait(twAuto.driver, 5)
-                    wait.until(EC.presence_of_element_located(
-                        (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span")))
-                    twAuto.driver.find_element(
-                        'xpath', "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span").click()
-                    tweetUrl = twAuto.driver.current_url
-                    print("Tweeted Successfully")
-                    print("Tweet URL:"+tweetUrl)
-                    return tweetUrl
-                except TimeoutException:
-                    try:
-                        twAuto.driver.find_element(
-                            'xpath', "//*[@id='layers']/div[3]/div/div/div/div/div[1]")
-                        print('Couldnt Tweet.')
-                        return None
-                    except:
-                        try:
-                            wait = WebDriverWait(twAuto.driver, 5)
-                            wait.until(EC.presence_of_element_located(
-                                (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span")))
-                            twAuto.driver.find_element(
-                                By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span").click()
-                            tweetUrl = twAuto.driver.current_url
-                            print("Tweeted Successfully")
-                            print("Tweet URL:"+tweetUrl)
-                        except:
-                            print('Couldnt Tweet.')
-                            return None
-            except Exception as e:
-                if self.debugMode:
-                    print("twAuto Error: ", e)
-                return False
-
-        
-    # quote tweet. this function uses the "adding the quoted tweets url to end of the text method" but maybe i will add the another version of this function that uses the quote tweet function later
-    def quoteTweet(self, url="", imgpath="", text=""):
-        try:
-            twAuto.driver.get("https://twitter.com/home")
-            fixUrl=url+"?s=20"
-            twAuto.driver.get(fixUrl)
-            container_element = self.findTweet(url=url)
-            
-            if self.pathType == "testId":
-                try:
-
-                    body_element = container_element.find_element(By.XPATH, './/div[@data-testid="retweet"]')
-                    twAuto.driver.execute_script("arguments[0].click()", body_element)
-                    
-                except Exception as e:
-                    body_element = container_element.find_element(By.XPATH, './/div[@data-testid="unretweet"]')
-                    twAuto.driver.execute_script("arguments[0].click()", body_element)
-                    try:
-                        quoteButton = twAuto.driver.find_element(
-                            By.XPATH, '//*[@id="layers"]/div[2]/div/div/div/div[2]/div/div[3]/div/div/div/a')
-                        twAuto.driver.execute_script("arguments[0].click()", quoteButton)
-                        input_field = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetTextarea_0"]')
-                        input_field.send_keys(text+" ")
-                        if imgpath != None:
-                            element = twAuto.driver.find_element(
-                                By.XPATH, "//input[@type='file']")
-
-                            twAuto.driver.execute_script(
-                                "arguments[0].style.display = 'block';", element)
-
-                            element.send_keys(imgpath)
-                        tweetButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetButton"]')
-                        twAuto.driver.execute_script("arguments[0].click()", tweetButton)
-                        return True
-                    except:
-                        return False
-                try:
-                    quoteButton = twAuto.driver.find_element(
-                        By.XPATH, '//*[@id="layers"]/div[2]/div/div/div/div[2]/div/div[3]/div/div/div/a')
-                    twAuto.driver.execute_script("arguments[0].click()", quoteButton)
-                    input_field = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetTextarea_0"]')
-                    input_field.send_keys(text+" ")
-                    if imgpath != None:
-                            element = twAuto.driver.find_element(
-                                By.XPATH, "//input[@type='file']")
-
-                            twAuto.driver.execute_script(
-                                "arguments[0].style.display = 'block';", element)
-
-                            element.send_keys(imgpath)
-                    tweetButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetButton"]')
-                    twAuto.driver.execute_script("arguments[0].click()", tweetButton)
-                    return True
-                except:
-                    return False
-            
-            if self.pathType == "xPath":
-                modified_text = text + "\n" + url
-                result = self.tweet(text=modified_text, imgpath=imgpath)
-                if result == None:
-                    print('Quote Tweet Failed')
-                    return None
-                else:
-                    print('Quoted Tweet Successfully')
-                    print('Quote Tweet URL:'+result)
-                    return result
-            #old method for qutoing, this method adds url of the tweet at the end of the text for quoting, then tweets the text.
-            '''modified_text = text + "\n" + url
-            result = self.tweet(text=modified_text)
-            if result == None:
-                print('Quote Tweet Failed')
-                return None
-            else:
-                print('Quoted Tweet Successfully')
-                print('Quote Tweet URL:'+result)
-                return result
-            '''
-        except Exception as e:
-            if self.debugMode:
-                print("twAuto Error: ", e)
-            return False
-            
-    # retweet and like functions are not working with tweets or replies with no text. I will fix it in the future.
-    def retweet(self, url=""):
-        try:
-            twAuto.driver.get("https://twitter.com/home")
-            fixUrl=url+"?s=20"
-            twAuto.driver.get(fixUrl)
-            container_element = self.findTweet(url=url)
-            if self.pathType=="xPath":
-                try:
-                    try:
-                        body_element = container_element.find_element(
-                            By.XPATH, './/div[3]/div[8]/div/div[2]/div')
-                    except:
-                        body_element = container_element.find_element(
-                            By.XPATH, './/div[3]/div[7]/div/div[2]/div')
-                    body_element.click()
-                    try:
-                        retweetButton = twAuto.driver.find_element(
-                            By.XPATH, '/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div[2]/div/div[3]/div/div/div/div')
-                        retweetButton.click()
-                        return True
-                    except:
-                        return False
-                except:
-                    return False
-            if self.pathType == "testId":
-                try:
-
-                    body_element = container_element.find_element(By.XPATH, './/div[@data-testid="retweet"]')
-                    twAuto.driver.execute_script("arguments[0].click()", body_element)
-                except Exception as e:
-                    print("This account already retweeted this tweet.")
-                try:
-                    retweetButton = twAuto.driver.find_element(
-                        By.XPATH, './/div[@data-testid="retweetConfirm"]')
-                    twAuto.driver.execute_script("arguments[0].click()", retweetButton)
-                    return True
-                except:
-                    return False
-        except Exception as e:
-            if self.debugMode:
-                print("twAuto Error: ", e)
-            return False
-
-
-    # likes tweet
-    def like(self, url=""):
-        try:
-            twAuto.driver.get("https://twitter.com/home")
-            fixUrl=url+"?s=20"
-            twAuto.driver.get(fixUrl)
-            container_element = self.findTweet(url=url)
-            if self.pathType == "xPath":
-                try:
-                    try:
-                        body_element = container_element.find_element(
-                            By.XPATH, './/div[3]/div[8]/div/div[3]/div')
-                    except:
-                        body_element = container_element.find_element(
-                            By.XPATH, './/div[3]/div[7]/div/div[3]/div')
-                    body_element.click()
-                    return True
-                except:
-                    return False
-            if self.pathType == "testId":
-                try:
-                    body_element = container_element.find_element(By.XPATH, './/div[@data-testid="like"]')
-                    twAuto.driver.execute_script("arguments[0].click()", body_element)
-                except:
-                    return False
-        except Exception as e:
-            if self.debugMode:
-                print("twAuto Error: ", e)
-            return False
-    # reply to a tweet
-    def reply(self, url="", imgpath="", text=""):
-        try:
-            twAuto.driver.get("https://twitter.com/home")
-            fixUrl=url+"?s=20"
-            twAuto.driver.get(fixUrl)
-            container_element = self.findTweet(url=url)
-            if self.pathType == "xPath":
-                try:
-                    try:
-                        body_element = container_element.find_element(
-                            By.XPATH, './/div[3]/div[8]/div/div[1]/div')
-                    except:
-                        body_element = container_element.find_element(
-                            By.XPATH, './/div[3]/div[7]/div/div[1]/div')
-                    body_element.click()
-                    try:
-                        wait = WebDriverWait(twAuto.driver, 5)
-                        wait.until(EC.presence_of_element_located(
-                            (By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[2]/div/div/div/div/div[2]/div[1]/div/div/div/div/div/div/div/div/div/div/label/div[1]/div/div/div/div/div/div[2]/div")))
-                        twAuto.driver.find_element(
-                            By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[2]/div/div/div/div/div[2]/div[1]/div/div/div/div/div/div/div/div/div/div/label/div[1]/div/div/div/div/div/div[2]/div").send_keys(text+" ")
-                        if imgpath != "":
-                            element = twAuto.driver.find_element(
-                                By.XPATH, "//input[@type='file']")
-
-                            twAuto.driver.execute_script(
-                                "arguments[0].style.display = 'block';", element)
-
-                            element.send_keys(imgpath)
-                        tweetReplyButton = twAuto.driver.find_element(
-                            By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[2]/div/div/div/div/div[2]/div[3]/div/div/div[2]/div[2]")
-                        tweetReplyButton.click()
-                        wait.until(EC.presence_of_element_located(
-                            (By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div[2]/a")))
-                        replyURL = twAuto.driver.find_element(
-                            By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div[2]/a").get_attribute("href")
-                        return replyURL
-                    except:
-                        return False
-                except:
-                    return False
-            if self.pathType == "testId":
-                #data-testid="tweetTextarea_0_label"]tweetButton
-                try:
-                    try:
-                        body_element = container_element.find_element(
-                            By.XPATH, './/div[3]/div[8]/div/div[1]/div')
-                    except:
-                        body_element = container_element.find_element(
-                            By.XPATH, './/div[3]/div[7]/div/div[1]/div')
-                    body_element.click()
-                    try:
-                        #tweetTextarea_0
-                        wait = WebDriverWait(twAuto.driver, 5)
-                        wait.until(EC.presence_of_element_located(
-                            (By.XPATH, '//div[@data-testid="tweetTextarea_0"]')))
-                        
-                        input_field = twAuto.driver.find_element(
-                            'xpath', '//div[@data-testid="tweetTextarea_0"]')
-                        if text=="":
-                            input_field.send_keys(text)
-                        else:
-                            input_field.send_keys(text)
-                            
-                        #imgbutton = container_element.find_element(
-                        #    By.XPATH, './/div/div/div[2]/div/div[2]/div[2]/div/div/div/div[2]/div[3]/div/div/div[1]/div[1]')
-                        
-                        if imgpath != "":
-                            element = twAuto.driver.find_element(
-                                By.XPATH, "//input[@type='file']")
-
-                            twAuto.driver.execute_script(
-                                "arguments[0].style.display = 'block';", element)
-
-                            element.send_keys(imgpath)
-
-                        #find tweet button
-                        tweetButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetButton"]')
-                        
-                        #click tweet button
-                        twAuto.driver.execute_script("arguments[0].click()", tweetButton)
-                    
-                        wait.until(EC.presence_of_element_located(
-                            (By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div[2]/a")))
-                        replyURL = twAuto.driver.find_element(
-                            By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div[2]/a").get_attribute("href")
-                        return replyURL
-                    except:
-                        return False
-                except:
-                    return False
-        except Exception as e:
-            if self.debugMode:
-                print("twAuto Error: ", e)
-            return False
-                
-    # locates tweet in the page based on the tweets content
-    def findTweet(self, url=""):
-        try:
-            #twAuto.driver.get(url)
-            try:
-                wait = WebDriverWait(twAuto.driver, 120)
-                wait.until(EC.presence_of_element_located(
-                    (By.CSS_SELECTOR, ".css-1dbjc4n.r-18u37iz.r-15zivkp")))
-                time.sleep(1)
-                tmp_element = twAuto.driver.find_element(
-                    By.CSS_SELECTOR, ".css-1dbjc4n.r-18u37iz.r-15zivkp")
-                container_element = tmp_element.find_element(By.XPATH, '..')
-                return container_element
-            except TimeoutException:
-                return None
-        except Exception as e:
-            if self.debugMode:
-                print("twAuto Error: ", e)
-            return False
-
-    # undo retweet action - !!!Unstable!!!
-    def unretweet(self, url=""):
-        twAuto.driver.get("https://twitter.com/home")
-        fixUrl=url+"?s=20"
-        twAuto.driver.get(fixUrl)
-        container_element = self.findTweet(url=url)
-        #unretweetConfirm
-        try:
-            wait = WebDriverWait(twAuto.driver, 120)
-            wait.until(EC.presence_of_element_located(
-                (By.XPATH, '//div[@data-testid="unretweet"]')))
-            
-            #find unretweet button
-            unretweetButton = container_element.find_element(By.XPATH, './/div[@data-testid="unretweet"]')
-                    
-            #click unretweet button
-            twAuto.driver.execute_script("arguments[0].click()", unretweetButton)
-            
-             #find unretweet button
-            unretweetConfirmButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="unretweetConfirm"]')
-                    
-            #click unretweet button
-            twAuto.driver.execute_script("arguments[0].click()", unretweetConfirmButton)
-            return True
-        except Exception as e:
-            if self.debugMode:
-                print("twAuto Error: ", e)
-            return False
-    
-    # logs out from twitter and deletes the cookies
-    def logout(self):
-        twAuto.driver.get("https://twitter.com/logout")
-        try:
-            wait = WebDriverWait(twAuto.driver, 120)
-            wait.until(EC.presence_of_element_located(
-                (By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div[2]/div[1]")))
-        except TimeoutException:
-            print('Couldnt log out.')
-        twAuto.driver.find_element(
-            'xpath', "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div[2]/div[1]").click()
-        os.remove("cookies.pkl")
-        print("Succesfully logged out")
-        
-    # closes selenium driver
-    def close(self):
-        twAuto.driver.quit()
+import pickle
+from selenium import webdriver
+from selenium.webdriver.common.keys import Keys
+from selenium.common.exceptions import TimeoutException
+from selenium.webdriver.support.ui import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.common.by import By
+import time
+from socket import timeout
+from os.path import exists
+import os
+import requests
+import bs4
+from bs4 import BeautifulSoup
+from urllib import request
+
+from selenium.webdriver.chrome.service import Service as ChromiumService
+from webdriver_manager.chrome import ChromeDriverManager
+from webdriver_manager.core.utils import ChromeType
+
+class twAuto:
+    driver = None
+    cookies_exists = exists('cookies.pkl')
+    chrome_options = webdriver.ChromeOptions()
+    chrome_options.add_argument("--disable-extensions")
+    chrome_options.add_argument('--disable-gpu')
+    chrome_options.add_argument('--ignore-certificate-errors')
+    chrome_options.add_experimental_option(
+        "excludeSwitches", ["enable-logging"])
+
+    def __init__(
+        self,
+        password="",
+        username="",
+        email="",
+        headless=True,
+        debugMode=False,
+        chromeDriverMode="auto", #manual or auto
+        driverPath = "./chrome.exe", #if you use manual, pass the driverPath
+        pathType = "testId" #xPath or testId
+    ):
+        self.email = email
+        self.username = username
+        self.password = password
+        self.chromeDriverMode = chromeDriverMode
+        self.driverPath = driverPath
+        self.pathType = pathType
+        self.headless = headless
+        self.debugMode = debugMode
+        if headless:
+            twAuto.chrome_options.add_argument('--headless')
+        if debugMode:
+            print("twAuto started.")
+
+    # start selenium driver
+    def start(self):
+        try:
+            if self.chromeDriverMode == "auto":
+                twAuto.driver = webdriver.Chrome(ChromeDriverManager().install(), options=twAuto.chrome_options)
+            else:
+                twAuto.driver = webdriver.Chrome(self.driverPath, options=twAuto.chrome_options)
+        except Exception as e:
+            if self.debugMode:
+                print("twAuto Error: ", e)
+    # test function to open twitter on chrome
+    def openTw(self):
+        twAuto.driver.get("https://twitter.com/home")
+
+    # login to twitter
+    def login(self):
+        try:
+            twAuto.driver.get("https://twitter.com/")
+            # this cookie importing prevents 'New login notification" in every action
+            if twAuto.cookies_exists:
+                cookies = pickle.load(open("cookies.pkl", "rb"))
+                for cookie in cookies:
+                    twAuto.driver.add_cookie(cookie)
+            if twAuto.cookies_exists:
+                twAuto.driver.get("https://twitter.com/")
+            else:
+                twAuto.driver.get("https://twitter.com/login")
+                try:
+                    wait = WebDriverWait(twAuto.driver, 120)
+                    wait.until(EC.presence_of_element_located(
+                        (By.XPATH, "//*[@id='layers']/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div/div/div/div[5]/label/div/div[2]/div/input")))
+                except TimeoutException:
+                    pass
+                mailInput = twAuto.driver.find_element(
+                    'xpath', "//*[@id='layers']/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div/div/div/div[5]/label/div/div[2]/div/input")
+                mailInput.send_keys(self.email)
+                twAuto.driver.find_element(
+                    'xpath', "//div[@class='css-18t94o4 css-1dbjc4n r-sdzlij r-1phboty r-rs99b7 r-ywje51 r-usiww2 r-2yi16 r-1qi8awa r-1ny4l3l r-ymttw5 r-o7ynqc r-6416eg r-lrvibr r-13qz1uu']").click()
+                time.sleep(3)
+
+                try:
+                    userNameInput = twAuto.driver.find_element(
+                        'xpath', "/html/body/div/div/div/div[1]/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div[1]/div/div/div[3]/div/label/div/div[2]/div[1]/input")
+                except:
+                    userNameInput = twAuto.driver.find_element(
+                        'xpath', "/html/body/div/div/div/div[1]/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div[1]/div/div[2]/label/div/div[2]/div/input")
+
+                userNameInput.send_keys(self.username)
+
+                twAuto.driver.find_element(
+                    'xpath', "//*[@id='layers']/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div[2]/div/div/div/div").click()
+
+                try:
+                    wait = WebDriverWait(twAuto.driver, 120)
+                    wait.until(EC.presence_of_element_located(
+                        (By.XPATH, "//*[@id='layers']/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div[1]/div/div/div[3]/div/label/div/div[2]/div[1]/input")))
+                except TimeoutException:
+                    pass
+                passwordInput = twAuto.driver.find_element(
+                    'xpath', "//*[@id='layers']/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div[1]/div/div/div[3]/div/label/div/div[2]/div[1]/input")
+                passwordInput.send_keys(self.password)
+                twAuto.driver.find_element(
+                    'xpath', "//*[@id='layers']/div/div/div/div/div/div/div[2]/div[2]/div/div/div[2]/div[2]/div[2]/div/div[1]/div/div/div").click()
+
+            try:
+                wait = WebDriverWait(twAuto.driver, 120)
+                wait.until(EC.presence_of_element_located(
+                    (By.XPATH, "//*[@id='react-root']/div/div/div[2]/header/div/div/div/div[1]/div[2]/nav/a[1]")))
+                print("Succesfully Logged In")
+            except Exception as e:
+                if self.debugMode:
+                    print("twAuto Error: ", e)
+
+            twAuto.driver.get("https://twitter.com/Twitter/")
+
+            if not twAuto.cookies_exists:
+                pickle.dump(twAuto.driver.get_cookies(), open("cookies.pkl", "wb"))
+                
+        except Exception as e:
+            if self.debugMode:
+                    print("twAuto Error: ", e)
+            return False   
+
+    #this functions is for the ones that having trouble in the login process, 
+    #you must pass the headless parameter as true to use this function
+    #after you login manually, open the console window and enter any key to continue
+    #this function will save the cookies to the cookies.pkl file
+    #and after that you can use the login function and module without any problem
+    def manualCookieCreation(self):
+        if not self.headless:
+            twAuto.driver.get("https://twitter.com/login")
+            input("Please login to your account. After you login, press any key to save your cookies to current folder.")
+            pickle.dump(twAuto.driver.get_cookies(), open("cookies.pkl", "wb"))
+        else:
+            print("Please pass the headless parameter as False to use this function")
+            sleep(3)
+            self.close()
+
+    # tweet text
+    def tweet(self, imgpath=None, text=""):
+        # load tweeting page
+        twAuto.driver.get("https://twitter.com/home")
+        twAuto.driver.get('https://twitter.com/compose/tweet')
+
+
+        if self.pathType=="xPath":
+            try:
+                # try finding tweet inbox
+                try:
+                    wait = WebDriverWait(twAuto.driver, 120)
+                    wait.until(EC.presence_of_element_located(
+                        (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[1]/div/div/div/div/div/div[2]/div/div/div/div/label/div[1]/div/div/div/div/div/div[2]/div")))
+                except TimeoutException:
+                    print('Couldnt tweet.')
+
+                # modify tweet text
+                full_text = text
+
+                input_field = twAuto.driver.find_element(
+                    'xpath', "//*[@id='layers']/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[1]/div/div/div/div/div/div[2]/div/div/div/div/label/div[1]/div/div/div/div/div/div[2]/div")
+                input_field.send_keys(full_text)
+
+                try:
+                    wait = WebDriverWait(twAuto.driver, 120)
+                    wait.until(EC.presence_of_element_located(
+                        (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[3]/div/div/div[2]/div[4]")))
+                except TimeoutException:
+                    print('Couldnt tweet.')
+                    
+                if imgpath != None:
+                    element = twAuto.driver.find_element(
+                        By.XPATH, "//input[@type='file']")
+                    '''//*[@id="layers"]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[3]/div/div/div[1]/div[1]'''
+                    twAuto.driver.execute_script(
+                        "arguments[0].style.display = 'block';", element)
+
+                    element.send_keys(imgpath)
+
+                twAuto.driver.find_element(By.XPATH,
+                                        '//*[@id="layers"]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[1]/div/div/div/div/div[2]/div[3]/div/div/div[2]/div[4]').click()
+                try:
+                    wait = WebDriverWait(twAuto.driver, 5)
+                    wait.until(EC.presence_of_element_located(
+                        (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span")))
+                    twAuto.driver.find_element(
+                        'xpath', "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span").click()
+                    tweetUrl = twAuto.driver.current_url
+                    print("Tweeted Successfully")
+                    print("Tweet URL:"+tweetUrl)
+                    return tweetUrl
+                except TimeoutException:
+                    try:
+                        twAuto.driver.find_element(
+                            'xpath', "//*[@id='layers']/div[3]/div/div/div/div/div[1]")
+                        print('Couldnt Tweet.')
+                        return None
+                    except:
+                        try:
+                            wait = WebDriverWait(twAuto.driver, 5)
+                            wait.until(EC.presence_of_element_located(
+                                (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span")))
+                            twAuto.driver.find_element(
+                                By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span").click()
+                            tweetUrl = twAuto.driver.current_url
+                            print("Tweeted Successfully")
+                            print("Tweet URL:"+tweetUrl)
+                        except:
+                            print('Couldnt Tweet.')
+                            return None
+            except Exception as e:
+                if self.debugMode:
+                    print("twAuto Error: ", e)
+                return False
+
+        if self.pathType == "testId":
+            try:
+                # try finding tweet inbox
+                try:
+                    wait = WebDriverWait(twAuto.driver, 120)
+                    wait.until(EC.presence_of_element_located(
+                        (By.XPATH, '//div[@data-testid="tweetTextarea_0"]')))
+                except TimeoutException:
+                    print('Couldnt tweet.')
+                
+                # modify tweet text
+                full_text = text
+                
+                input_field = twAuto.driver.find_element(
+                    'xpath', '//div[@data-testid="tweetTextarea_0"]')
+                input_field.send_keys(full_text)
+                
+                try:
+                    wait = WebDriverWait(twAuto.driver, 120)
+                    wait.until(EC.presence_of_element_located((By.XPATH, '//div[@data-testid="tweetButton"]')))
+                    
+                except TimeoutException:
+                    print('Couldnt tweet.' )
+                
+                if imgpath != None:
+                    element = twAuto.driver.find_element(
+                        By.XPATH, "//input[@type='file']")
+
+                    twAuto.driver.execute_script(
+                        "arguments[0].style.display = 'block';", element)
+
+                    element.send_keys(imgpath)
+                
+                #find tweet button
+                tweetButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetButton"]')
+                
+                #click tweet button
+                twAuto.driver.execute_script("arguments[0].click()", tweetButton)
+
+                try:
+                    wait = WebDriverWait(twAuto.driver, 5)
+                    wait.until(EC.presence_of_element_located(
+                        (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span")))
+                    twAuto.driver.find_element(
+                        'xpath', "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span").click()
+                    tweetUrl = twAuto.driver.current_url
+                    print("Tweeted Successfully")
+                    print("Tweet URL:"+tweetUrl)
+                    return tweetUrl
+                except TimeoutException:
+                    try:
+                        twAuto.driver.find_element(
+                            'xpath', "//*[@id='layers']/div[3]/div/div/div/div/div[1]")
+                        print('Couldnt Tweet.')
+                        return None
+                    except:
+                        try:
+                            wait = WebDriverWait(twAuto.driver, 5)
+                            wait.until(EC.presence_of_element_located(
+                                (By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span")))
+                            twAuto.driver.find_element(
+                                By.XPATH, "//*[@id='layers']/div[2]/div/div/div/div/div[2]/a/span").click()
+                            tweetUrl = twAuto.driver.current_url
+                            print("Tweeted Successfully")
+                            print("Tweet URL:"+tweetUrl)
+                        except:
+                            print('Couldnt Tweet.')
+                            return None
+            except Exception as e:
+                if self.debugMode:
+                    print("twAuto Error: ", e)
+                return False
+
+        
+    # quote tweet. this function uses the "adding the quoted tweets url to end of the text method" but maybe i will add the another version of this function that uses the quote tweet function later
+    def quoteTweet(self, url="", imgpath="", text=""):
+        try:
+            twAuto.driver.get("https://twitter.com/home")
+            fixUrl=url+"?s=20"
+            twAuto.driver.get(fixUrl)
+            container_element = self.findTweet(url=url)
+            
+            if self.pathType == "testId":
+                try:
+
+                    body_element = container_element.find_element(By.XPATH, './/div[@data-testid="retweet"]')
+                    twAuto.driver.execute_script("arguments[0].click()", body_element)
+                    
+                except Exception as e:
+                    body_element = container_element.find_element(By.XPATH, './/div[@data-testid="unretweet"]')
+                    twAuto.driver.execute_script("arguments[0].click()", body_element)
+                    try:
+                        quoteButton = twAuto.driver.find_element(
+                            By.XPATH, '//*[@id="layers"]/div[2]/div/div/div/div[2]/div/div[3]/div/div/div/a')
+                        twAuto.driver.execute_script("arguments[0].click()", quoteButton)
+                        input_field = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetTextarea_0"]')
+                        input_field.send_keys(text+" ")
+                        if imgpath != None:
+                            element = twAuto.driver.find_element(
+                                By.XPATH, "//input[@type='file']")
+
+                            twAuto.driver.execute_script(
+                                "arguments[0].style.display = 'block';", element)
+
+                            element.send_keys(imgpath)
+                        tweetButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetButton"]')
+                        twAuto.driver.execute_script("arguments[0].click()", tweetButton)
+                        return True
+                    except:
+                        return False
+                try:
+                    quoteButton = twAuto.driver.find_element(
+                        By.XPATH, '//*[@id="layers"]/div[2]/div/div/div/div[2]/div/div[3]/div/div/div/a')
+                    twAuto.driver.execute_script("arguments[0].click()", quoteButton)
+                    input_field = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetTextarea_0"]')
+                    input_field.send_keys(text+" ")
+                    if imgpath != None:
+                            element = twAuto.driver.find_element(
+                                By.XPATH, "//input[@type='file']")
+
+                            twAuto.driver.execute_script(
+                                "arguments[0].style.display = 'block';", element)
+
+                            element.send_keys(imgpath)
+                    tweetButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetButton"]')
+                    twAuto.driver.execute_script("arguments[0].click()", tweetButton)
+                    return True
+                except:
+                    return False
+            
+            if self.pathType == "xPath":
+                modified_text = text + "\n" + url
+                result = self.tweet(text=modified_text, imgpath=imgpath)
+                if result == None:
+                    print('Quote Tweet Failed')
+                    return None
+                else:
+                    print('Quoted Tweet Successfully')
+                    print('Quote Tweet URL:'+result)
+                    return result
+            #old method for qutoing, this method adds url of the tweet at the end of the text for quoting, then tweets the text.
+            '''modified_text = text + "\n" + url
+            result = self.tweet(text=modified_text)
+            if result == None:
+                print('Quote Tweet Failed')
+                return None
+            else:
+                print('Quoted Tweet Successfully')
+                print('Quote Tweet URL:'+result)
+                return result
+            '''
+        except Exception as e:
+            if self.debugMode:
+                print("twAuto Error: ", e)
+            return False
+            
+    # retweet and like functions are not working with tweets or replies with no text. I will fix it in the future.
+    def retweet(self, url=""):
+        try:
+            twAuto.driver.get("https://twitter.com/home")
+            fixUrl=url+"?s=20"
+            twAuto.driver.get(fixUrl)
+            container_element = self.findTweet(url=url)
+            if self.pathType=="xPath":
+                try:
+                    try:
+                        body_element = container_element.find_element(
+                            By.XPATH, './/div[3]/div[8]/div/div[2]/div')
+                    except:
+                        body_element = container_element.find_element(
+                            By.XPATH, './/div[3]/div[7]/div/div[2]/div')
+                    body_element.click()
+                    try:
+                        retweetButton = twAuto.driver.find_element(
+                            By.XPATH, '/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div[2]/div/div[3]/div/div/div/div')
+                        retweetButton.click()
+                        return True
+                    except:
+                        return False
+                except:
+                    return False
+            if self.pathType == "testId":
+                try:
+
+                    body_element = container_element.find_element(By.XPATH, './/div[@data-testid="retweet"]')
+                    twAuto.driver.execute_script("arguments[0].click()", body_element)
+                except Exception as e:
+                    print("This account already retweeted this tweet.")
+                try:
+                    retweetButton = twAuto.driver.find_element(
+                        By.XPATH, './/div[@data-testid="retweetConfirm"]')
+                    twAuto.driver.execute_script("arguments[0].click()", retweetButton)
+                    return True
+                except:
+                    return False
+        except Exception as e:
+            if self.debugMode:
+                print("twAuto Error: ", e)
+            return False
+
+
+    # likes tweet
+    def like(self, url=""):
+        try:
+            twAuto.driver.get("https://twitter.com/home")
+            fixUrl=url+"?s=20"
+            twAuto.driver.get(fixUrl)
+            container_element = self.findTweet(url=url)
+            if self.pathType == "xPath":
+                try:
+                    try:
+                        body_element = container_element.find_element(
+                            By.XPATH, './/div[3]/div[8]/div/div[3]/div')
+                    except:
+                        body_element = container_element.find_element(
+                            By.XPATH, './/div[3]/div[7]/div/div[3]/div')
+                    body_element.click()
+                    return True
+                except:
+                    return False
+            if self.pathType == "testId":
+                try:
+                    body_element = container_element.find_element(By.XPATH, './/div[@data-testid="like"]')
+                    twAuto.driver.execute_script("arguments[0].click()", body_element)
+                except:
+                    return False
+        except Exception as e:
+            if self.debugMode:
+                print("twAuto Error: ", e)
+            return False
+    # reply to a tweet
+    def reply(self, url="", imgpath="", text=""):
+        try:
+            twAuto.driver.get("https://twitter.com/home")
+            fixUrl=url+"?s=20"
+            twAuto.driver.get(fixUrl)
+            container_element = self.findTweet(url=url)
+            """ if self.pathType == "xPath":
+                try:
+                    try:
+                        body_element = container_element.find_element(
+                            By.XPATH, './/div[3]/div[8]/div/div[1]/div')
+                    except Exception as e:
+                        body_element = container_element.find_element(
+                            By.XPATH, './/div[3]/div[7]/div/div[1]/div')
+                        if self.debugMode : print("twAuto Error: ", e)
+                    body_element.click()
+                    try:
+                        wait = WebDriverWait(twAuto.driver, 5)
+                        wait.until(EC.presence_of_element_located(
+                            (By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[2]/div/div/div/div/div[2]/div[1]/div/div/div/div/div/div/div/div/div/div/label/div[1]/div/div/div/div/div/div[2]/div")))
+                        twAuto.driver.find_element(
+                            By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[2]/div/div/div/div/div[2]/div[1]/div/div/div/div/div/div/div/div/div/div/label/div[1]/div/div/div/div/div/div[2]/div").send_keys(text+" ")
+                        if imgpath != "":
+                            element = twAuto.driver.find_element(
+                                By.XPATH, "//input[@type='file']")
+
+                            twAuto.driver.execute_script(
+                                "arguments[0].style.display = 'block';", element)
+
+                            element.send_keys(imgpath)
+                        tweetReplyButton = twAuto.driver.find_element(
+                            By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div/div/div/div[3]/div/div[2]/div/div/div/div/div[2]/div[3]/div/div/div[2]/div[2]")
+                        tweetReplyButton.click()
+                        wait.until(EC.presence_of_element_located(
+                            (By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div[2]/a")))
+                        replyURL = twAuto.driver.find_element(
+                            By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div[2]/a").get_attribute("href")
+                        return replyURL
+                    except Exception as e:
+                        if self.debugMode : print("twAuto Error: ", e)
+                        return False
+                except Exception as e:
+                    if self.debugMode : print("twAuto Error: ", e)
+                    return False """
+            if self.pathType == "testId" or self.pathType == "xPath":
+                #data-testid="tweetTextarea_0_label"]tweetButton
+                try:
+                    try:
+                        body_element = container_element.find_element(
+                            By.XPATH, './/div[3]/div[8]/div/div[1]/div')
+                    except Exception as e:
+                        body_element = container_element.find_element(
+                            By.XPATH, '//div[@data-testid="tweetTextarea_0RichTextInputContainer"]')
+                    body_element.click()
+                    try:
+                        #tweetTextarea_0
+                        wait = WebDriverWait(twAuto.driver, 5)
+                        wait.until(EC.presence_of_element_located(
+                            (By.XPATH, '//div[@data-testid="tweetTextarea_0"]')))
+                        
+                        input_field = twAuto.driver.find_element(
+                            'xpath', '//div[@data-testid="tweetTextarea_0"]')
+                        if text=="":
+                            input_field.send_keys(text)
+                        else:
+                            input_field.send_keys(text)
+                            
+                        #imgbutton = container_element.find_element(
+                        #    By.XPATH, './/div/div/div[2]/div/div[2]/div[2]/div/div/div/div[2]/div[3]/div/div/div[1]/div[1]')
+                        
+                        if imgpath != "":
+                            element = twAuto.driver.find_element(
+                                By.XPATH, "//input[@type='file']")
+
+                            twAuto.driver.execute_script(
+                                "arguments[0].style.display = 'block';", element)
+
+                            element.send_keys(imgpath)
+                        time.sleep(1)
+                        #check if there is a mask
+                        try:
+                            maskClose = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="app-bar-close"]')
+                            twAuto.driver.execute_script("arguments[0].click()", maskClose)
+                        except:
+                            pass
+                        #find tweet button
+                        try:
+                            tweetButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetButton"]')
+                            #click tweet button
+                            twAuto.driver.execute_script("arguments[0].click()", tweetButton)
+                        except:
+                            tweetButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="tweetButtonInline"]')
+                            #click tweet button
+                            twAuto.driver.execute_script("arguments[0].click()", tweetButton)
+
+                    
+                        wait.until(EC.presence_of_element_located(
+                            (By.XPATH, '//div[@data-testid="toast"]')))
+                        replyURLButton = twAuto.driver.find_element(
+                            By.XPATH, '//div[@data-testid="toast"]')
+                        replyURLElement = replyURLButton.find_element(By.XPATH, './/div[2]/a[1]').get_attribute("href")
+                        return replyURLElement
+                    except Exception as e:
+                        if self.debugMode : print("twAuto Error: ", e)
+                        return False
+                except Exception as e:
+                    if self.debugMode : print("twAuto Error: ", e)
+                    return False
+        except Exception as e:
+            if self.debugMode : print("twAuto Error: ", e)
+            return False
+                
+    # locates tweet in the page based on the tweets content
+    def findTweet(self, url=""):
+        try:
+            #twAuto.driver.get(url)
+            try:
+                wait = WebDriverWait(twAuto.driver, 120)
+                wait.until(EC.presence_of_element_located(
+                    (By.CSS_SELECTOR, ".css-1dbjc4n.r-18u37iz.r-15zivkp")))
+                time.sleep(1)
+                tmp_element = twAuto.driver.find_element(
+                    By.CSS_SELECTOR, ".css-1dbjc4n.r-18u37iz.r-15zivkp")
+                container_element = tmp_element.find_element(By.XPATH, '..')
+                return container_element
+            except TimeoutException:
+                return None
+        except Exception as e:
+            if self.debugMode:
+                print("twAuto Error: ", e)
+            return False
+
+    # undo retweet action - !!!Unstable!!!
+    def unretweet(self, url=""):
+        twAuto.driver.get("https://twitter.com/home")
+        fixUrl=url+"?s=20"
+        twAuto.driver.get(fixUrl)
+        container_element = self.findTweet(url=url)
+        #unretweetConfirm
+        try:
+            wait = WebDriverWait(twAuto.driver, 120)
+            wait.until(EC.presence_of_element_located(
+                (By.XPATH, '//div[@data-testid="unretweet"]')))
+            
+            #find unretweet button
+            unretweetButton = container_element.find_element(By.XPATH, './/div[@data-testid="unretweet"]')
+                    
+            #click unretweet button
+            twAuto.driver.execute_script("arguments[0].click()", unretweetButton)
+            
+             #find unretweet button
+            unretweetConfirmButton = twAuto.driver.find_element(By.XPATH, '//div[@data-testid="unretweetConfirm"]')
+                    
+            #click unretweet button
+            twAuto.driver.execute_script("arguments[0].click()", unretweetConfirmButton)
+            return True
+        except Exception as e:
+            if self.debugMode:
+                print("twAuto Error: ", e)
+            return False
+    
+    # logs out from twitter and deletes the cookies
+    def logout(self):
+        twAuto.driver.get("https://twitter.com/logout")
+        try:
+            wait = WebDriverWait(twAuto.driver, 120)
+            wait.until(EC.presence_of_element_located(
+                (By.XPATH, "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div[2]/div[1]")))
+        except TimeoutException:
+            print('Couldnt log out.')
+        twAuto.driver.find_element(
+            'xpath', "/html/body/div[1]/div/div/div[1]/div[2]/div/div/div/div/div/div[2]/div[2]/div[2]/div[1]").click()
+        os.remove("cookies.pkl")
+        print("Succesfully logged out")
+        
+    # closes selenium driver
+    def close(self):
+        twAuto.driver.quit()
```

### Comparing `twAuto-0.3.4/twAuto.egg-info/PKG-INFO` & `twAuto-0.3.5/twAuto.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,221 +1,222 @@
-Metadata-Version: 2.1
-Name: twAuto
-Version: 0.3.4
-Summary: TwAuto is a library for testing your code on pre-Twitter API application stage.
-Home-page: https://github.com/EKOzkan/twAuto
-Author: Ekin Kagan Ozkan
-Author-email: ekinkagan@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENCE.MD
-
-# twAuto - Twitter Automation Tool v0.3.4 🦆
-
-twAuto is a library for "Tweeting", "Retweeting", "Replying", "Tweet Quoting", "Tweet Liking" without any API requirements using Selenium.
-
-<br/>
-
-Note: While using this library I didnt encounter any problems/bad response from Twitter like banning account etc. but please use at your own risk.
-
-## Requirements
-
-- Python 3.7+
-
-- [beautifulsoup4](https://pypi.org/project/beautifulsoup4/)
-
-- [selenium](https://pypi.org/project/selenium/)
-
-- [webdriver-manager](https://pypi.org/project/webdriver-manager/)
-
-## Installation
-
-**Pip:**
-
-```bash
-pip3 install twAuto
-```
-
-## Functions
-
-**- Import:**
-
-```python
-import twAuto
-```
-
-<br/>
-
-**- Configure:**
-
-```python
-tw = twAuto.twAuto(
-  username="Your Twitter Username",
-  email="Your Twitter E-Mail",
-  password="Your Twitter Password",
-  chromeDriverMode="manual" or "auto", #if you use auto twAuto will automatically download the chrome driver for you,
-                                       #if you use the manual option, you need to provide the driver path in driverPath parameter.
-  pathType="testId" or "xPath", #It is testId by default. If you had any problems with library you can try the xPath mode too.
-  headless=True/False, #Headless is true by default.
-  debugMode= True/False #Really poorly implemented debug mode, this is for reading occured errors.
-                        #It is not realiable right now but you can give it a try if you want to.
-)
-
-```
-
-<br/>
-
-**- Start:** Start functions runs the selenium driver.
-
-```python
-tw.start()
-```
-
-<br/>
-
-**- Login:** Logs in to the Twitter account
-
-```python
-tw.login()
-```
-
-<br/>
-
-**- Login Errors:** If you encounter any error in the login process, you can use manualCookieCreation() to get your cookie file manually.
-Run the function after tw.start() line. Then after the browser window opened, login to account you want to automate, then enter any character in the terminal. This will create a cookie file after this, you can use the library.
-
-Note: Headless must be False to use this function.
-
-```python
-tw.manualCookieCreation()
-```
-
-Example:
-
-First run this code to get your cookie file.
-
-```python
-tw = twAuto.twAuto(
-  username="Your Twitter Username",
-  email="Your Twitter E-Mail",
-  password="Your Twitter Password",
-  chromeDriverMode="auto",
-  pathType="xPath",
-  headless=False #Headless must be False to use this function.
-)
-
-tw.start()
-tw.manualCookieCreation()
-```
-
-After doing the steps that is described above, you can run your main code.
-
-```python
-tw = twAuto.twAuto(
-  username="Your Twitter Username",
-  email="Your Twitter E-Mail",
-  password="Your Twitter Password",
-  chromeDriverMode="auto",
-  pathType="xPath"
-)
-
-tw.start()
-tw.login()
-#other functions...
-```
-
-<br/>
-
-**- Like:** Likes tweet in the given url \
-->Returns: True/False as Success/Failed
-
-```python
-tw.like(url="")
-```
-
-<br/>
-
-**- Reply:** Replies to the tweet in the given url with given text.\
-->Returns: Reply URL/False
-
-```python
-tw.reply(url="", imgpath="", text="")
-```
-
-<br/>
-
-**- Tweet:** Tweets the text and image if given.\
-->Returns: Tweet URL/False
-
-```python
-tw.tweet(text="",imgpath="")
-```
-
-<br/>
-
-**- Quote Tweet:** Quotes the tweet in the given url with the given text.\
-->Returns: Quoted Tweet URL/False
-
-```python
-tw.quoteTweet(url="", imgpath="" ,text="")
-```
-
-<br/>
-
-**- Retweet:** Retweets the tweet in the given url.\
-->Returns: True/False as Success/Failed
-
-```python
-tw.retweet(url="")
-```
-
-<br/>
-
-**- Unretweet:** Unretweets the tweet in the given url.\
-->Returns: True/False as Success/Failed
-
-```python
-tw.unretweet(url="")
-```
-
-<br/>
-
-**- Logout:** Logs out from current Twitter account and deletes the cookies file.
-
-```python
-tw.logout()
-```
-
-<br/>
-
-**- Quit/Close:** Ends the session, closes the selenium driver application
-
-```python
-tw.close()
-```
-
-## Example Code
-
-```python
-tw = twAuto.twAuto(
-  username="",
-  email="",
-  password="",
-  headless=True,
-  chromeDriverMode="auto",
-  pathType="testId")
-
-tw.start()
-tw.login()
-
-tw.reply(url="",imgpath="", text="")
-
-tw.close()
-
-```
-
-## To Do's 📝 :
-
-- [x] Send image with Quote, Reply.
-- [ ] Send gif with Quote, Reply.
-- [x] Retweet without adding url at the end.
-- [ ] Linux integration(not tested yet).
+Metadata-Version: 2.1
+Name: twAuto
+Version: 0.3.5
+Summary: TwAuto is a library for testing your code on pre-Twitter API application stage.
+Home-page: https://github.com/EKOzkan/twAuto
+Author: Ekin Kagan Ozkan
+Author-email: ekinkagan@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENCE.MD
+
+# twAuto - Twitter Automation Tool v0.3.4 🦆
+
+twAuto is a library for "Tweeting", "Retweeting", "Replying", "Tweet Quoting", "Tweet Liking" without any API requirements using Selenium.
+
+<br/>
+
+Note: While using this library I didnt encounter any problems/bad response from Twitter like banning account etc. but please use at your own risk.
+
+## Requirements
+
+- Python 3.7+
+
+- [beautifulsoup4](https://pypi.org/project/beautifulsoup4/)
+
+- [selenium](https://pypi.org/project/selenium/)
+
+- [webdriver-manager](https://pypi.org/project/webdriver-manager/)
+
+## Installation
+
+**Pip:**
+
+```bash
+pip3 install twAuto
+```
+
+## Functions
+
+**- Import:**
+
+```python
+import twAuto
+```
+
+<br/>
+
+**- Configure:**
+
+```python
+tw = twAuto.twAuto(
+  username="Your Twitter Username",
+  email="Your Twitter E-Mail",
+  password="Your Twitter Password",
+  chromeDriverMode="manual" or "auto", #if you use auto twAuto will automatically download the chrome driver for you,
+                                       #if you use the manual option, you need to provide the driver path in driverPath parameter.
+  driverPath="your drivers path", #use only if you are using the chromeDriverMode in manual mode 
+  pathType="testId" or "xPath", #It is xPath by default. I highly recommend you to use testId instead of xPath. If you had any problems with library you can try the xPath mode too.
+  headless=True/False, #Headless is true by default.
+  debugMode= True/False #Really poorly implemented debug mode, this is for reading occured errors.
+                        #It is not reliable right now but you can give it a try if you want to.
+)
+
+```
+
+<br/>
+
+**- Start:** Start functions runs the selenium driver.
+
+```python
+tw.start()
+```
+
+<br/>
+
+**- Login:** Logs in to the Twitter account
+
+```python
+tw.login()
+```
+
+<br/>
+
+**- Login Errors:** If you encounter any errors in the login process, you can use manualCookieCreation() to get your cookie file manually.
+Run the function after tw.start() line. Then after the browser window opened, login to account you want to automate, then enter any character in the terminal. This will create a cookie file after this, you can use the library.
+
+Note: Headless must be False to use this function.
+
+```python
+tw.manualCookieCreation()
+```
+
+Example:
+
+First run this code to get your cookie file.
+
+```python
+tw = twAuto.twAuto(
+  username="Your Twitter Username",
+  email="Your Twitter E-Mail",
+  password="Your Twitter Password",
+  chromeDriverMode="auto",
+  pathType="xPath",
+  headless=False #Headless must be False to use this function.
+)
+
+tw.start()
+tw.manualCookieCreation()
+```
+
+After doing the steps that is described above, you can run your main code.
+
+```python
+tw = twAuto.twAuto(
+  username="Your Twitter Username",
+  email="Your Twitter E-Mail",
+  password="Your Twitter Password",
+  chromeDriverMode="auto",
+  pathType="xPath"
+)
+
+tw.start()
+tw.login()
+#other functions...
+```
+
+<br/>
+
+**- Like:** Likes tweet in the given url \
+->Returns: True/False as Success/Failed
+
+```python
+tw.like(url="")
+```
+
+<br/>
+
+**- Reply:** Replies to the tweet in the given url with given text.\
+->Returns: Reply URL/False
+
+```python
+tw.reply(url="", imgpath="", text="")
+```
+
+<br/>
+
+**- Tweet:** Tweets the text and image if given.\
+->Returns: Tweet URL/False
+
+```python
+tw.tweet(text="",imgpath="")
+```
+
+<br/>
+
+**- Quote Tweet:** Quotes the tweet in the given url with the given text.\
+->Returns: Quoted Tweet URL/False
+
+```python
+tw.quoteTweet(url="", imgpath="" ,text="")
+```
+
+<br/>
+
+**- Retweet:** Retweets the tweet in the given url.\
+->Returns: True/False as Success/Failed
+
+```python
+tw.retweet(url="")
+```
+
+<br/>
+
+**- Unretweet:** Unretweets the tweet in the given url.\
+->Returns: True/False as Success/Failed
+
+```python
+tw.unretweet(url="")
+```
+
+<br/>
+
+**- Logout:** Logs out from current Twitter account and deletes the cookies file.
+
+```python
+tw.logout()
+```
+
+<br/>
+
+**- Quit/Close:** Ends the session, closes the selenium driver application
+
+```python
+tw.close()
+```
+
+## Example Code
+
+```python
+tw = twAuto.twAuto(
+  username="",
+  email="",
+  password="",
+  headless=True,
+  chromeDriverMode="auto",
+  pathType="testId")
+
+tw.start()
+tw.login()
+
+tw.reply(url="",imgpath="", text="")
+
+tw.close()
+
+```
+
+## To Do's 📝 :
+
+- [x] Send image with Quote, Reply.
+- [ ] Send gif with Quote, Reply.
+- [x] Retweet without adding url at the end.
+- [ ] Linux integration(not tested yet).
```

