# Comparing `tmp/xenoslib-0.1.28.5.tar.gz` & `tmp/xenoslib-0.1.28.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.28.5.tar", last modified: Tue May 30 06:47:28 2023, max compression
+gzip compressed data, was "xenoslib-0.1.28.6.tar", last modified: Wed May 31 01:50:04 2023, max compression
```

## Comparing `xenoslib-0.1.28.5.tar` & `xenoslib-0.1.28.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:47:28.008428 xenoslib-0.1.28.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-30 06:47:28.008428 xenoslib-0.1.28.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:47:28.008428 xenoslib-0.1.28.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:47:28.008428 xenoslib-0.1.28.5/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-30 06:47:16.000000 xenoslib-0.1.28.5/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:47:28.008428 xenoslib-0.1.28.5/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-30 06:47:27.000000 xenoslib-0.1.28.5/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-30 06:47:28.000000 xenoslib-0.1.28.5/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:47:27.000000 xenoslib-0.1.28.5/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-30 06:47:28.000000 xenoslib-0.1.28.5/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 06:47:28.000000 xenoslib-0.1.28.5/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:50:04.489658 xenoslib-0.1.28.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 01:50:04.489658 xenoslib-0.1.28.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 01:50:04.489658 xenoslib-0.1.28.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:50:04.489658 xenoslib-0.1.28.6/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-31 01:49:53.000000 xenoslib-0.1.28.6/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:50:04.489658 xenoslib-0.1.28.6/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 01:50:04.000000 xenoslib-0.1.28.6/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-31 01:50:04.000000 xenoslib-0.1.28.6/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:50:04.000000 xenoslib-0.1.28.6/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-31 01:50:04.000000 xenoslib-0.1.28.6/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 01:50:04.000000 xenoslib-0.1.28.6/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.28.5/LICENSE` & `xenoslib-0.1.28.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.5/README.md` & `xenoslib-0.1.28.6/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.5/setup.py` & `xenoslib-0.1.28.6/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.5/xenoslib/base.py` & `xenoslib-0.1.28.6/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.5/xenoslib/dev.py` & `xenoslib-0.1.28.6/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.5/xenoslib/extend.py` & `xenoslib-0.1.28.6/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.5/xenoslib/linux.py` & `xenoslib-0.1.28.6/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.5/xenoslib/mail.py` & `xenoslib-0.1.28.6/xenoslib/mail.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from xenoslib.mail import MailFetcher, SMTPMail
 
 # Fetch emails
 for email_data in MailFetcher(imap_server, mail_addr, mail_pwd, interval=30, days=30):
     print(email_data["subject"])
 
 # Send email
-sender = SMTPMail(smtp_server, sender, password, smtp_port=25)
+sender = SMTPMail(smtp_server, sender, password, port=25)
 sender.send(subject, message, receiver, cc, bcc, filename)
 
 """
 import os
 import datetime
 from time import sleep
 import logging
@@ -95,20 +95,20 @@
             client.select_folder("INBOX", readonly=True)
             messages = client.search(["SINCE", date_str])
             emails = client.fetch(messages, ["INTERNALDATE", "BODY.PEEK[]"])
             return emails
 
 
 class SMTPMail:
-    def __init__(self, smtp_server="", sender="", password="", smtp_port=25):
+    def __init__(self, smtp_server="", sender="", password="", port=25):
         self.smtp_server = smtp_server
-        self.smtp_port = int(smtp_port)
+        self.port = int(port)
         self.sender = sender
         self.password = password
-        if self.smtp_port == 465:
+        if self.port == 465:  # use SSL by port
             self.SMTP = smtplib.SMTP_SSL
         else:
             self.SMTP = smtplib.SMTP
 
     def send(self, subject, message, receiver=[], cc=[], bcc=[], filename=None):
         msg = MIMEMultipart()
         msg["Subject"] = Header(subject, "utf-8")
@@ -121,15 +121,15 @@
         msg.attach(MIMEText(message, "html", "utf-8"))
 
         if filename:
             attachment = MIMEApplication(open(filename, "rb").read())
             attachment.add_header("Content-Disposition", "attachment", filename=filename)
             msg.attach(attachment)
 
-        with self.SMTP(self.smtp_server, self.smtp_port) as smtp:
+        with self.SMTP(self.smtp_server, self.port) as smtp:
             print(smtp.has_extn("STARTTLS"))
             if smtp.has_extn("STARTTLS"):
                 smtp.starttls()
             try:
                 smtp.login(self.sender, self.password)
             except Exception as exc:
                 logger.warning(exc)
@@ -158,15 +158,15 @@
     except ModuleNotFoundError:
         pass
     mail_addr = os.environ["SMTP_ADDR"]
     mail_pwd = os.environ["SMTP_PASS"]
     smtp_server = os.environ["SMTP_SERVER"]
     subject = "Test Email2"
     message = '<span style="color:red">This is a test email.</span>'
-    email_sender = SMTPMail(smtp_server, sender=mail_addr, password=mail_pwd, smtp_port=465)
-    # email_sender = SMTPMail(smtp_server, sender=mail_addr, password=mail_pwd, smtp_port=587)
+    email_sender = SMTPMail(smtp_server, sender=mail_addr, password=mail_pwd, port=465)
+    # email_sender = SMTPMail(smtp_server, sender=mail_addr, password=mail_pwd, port=587)
     email_sender.send(subject=subject, message=message, receiver=[os.environ["RECEIVER"]])
 
 
 if __name__ == "__main__":
     test_imap()
     # test()
```

### Comparing `xenoslib-0.1.28.5/xenoslib/mock.py` & `xenoslib-0.1.28.6/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.5/xenoslib/onedrive.py` & `xenoslib-0.1.28.6/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.5/xenoslib/win_trayicon.py` & `xenoslib-0.1.28.6/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.5/xenoslib/windows.py` & `xenoslib-0.1.28.6/xenoslib/windows.py`

 * *Files identical despite different names*

