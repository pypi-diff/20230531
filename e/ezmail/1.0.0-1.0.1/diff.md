# Comparing `tmp/ezmail-1.0.0.tar.gz` & `tmp/ezmail-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezmail-1.0.0.tar", last modified: Tue May 30 20:20:03 2023, max compression
+gzip compressed data, was "ezmail-1.0.1.tar", last modified: Wed May 31 16:36:31 2023, max compression
```

## Comparing `ezmail-1.0.0.tar` & `ezmail-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 20:20:03.104018 ezmail-1.0.0/
--rw-r--r--   0 alex       (501) staff       (20)    35149 2023-05-30 04:28:26.000000 ezmail-1.0.0/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)     3831 2023-05-30 20:20:03.103546 ezmail-1.0.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     3381 2023-05-30 20:18:56.000000 ezmail-1.0.0/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 20:20:03.098398 ezmail-1.0.0/ezmail/
--rw-r--r--   0 alex       (501) staff       (20)       30 2023-05-30 04:46:48.000000 ezmail-1.0.0/ezmail/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1107 2023-05-30 04:54:44.000000 ezmail-1.0.0/ezmail/__main__.py
--rw-r--r--   0 alex       (501) staff       (20)     4231 2023-05-30 04:43:32.000000 ezmail-1.0.0/ezmail/ezmail.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 20:20:03.102588 ezmail-1.0.0/ezmail.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     3831 2023-05-30 20:20:02.000000 ezmail-1.0.0/ezmail.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      230 2023-05-30 20:20:03.000000 ezmail-1.0.0/ezmail.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-05-30 20:20:02.000000 ezmail-1.0.0/ezmail.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       14 2023-05-30 20:20:02.000000 ezmail-1.0.0/ezmail.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)        7 2023-05-30 20:20:02.000000 ezmail-1.0.0/ezmail.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-05-30 20:20:03.104201 ezmail-1.0.0/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      735 2023-05-30 20:19:33.000000 ezmail-1.0.0/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-31 16:36:31.798727 ezmail-1.0.1/
+-rw-r--r--   0 alex       (501) staff       (20)    35149 2023-05-30 04:28:26.000000 ezmail-1.0.1/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     4151 2023-05-31 16:36:31.798369 ezmail-1.0.1/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     3678 2023-05-31 16:16:22.000000 ezmail-1.0.1/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-31 16:36:31.795030 ezmail-1.0.1/ezmail/
+-rw-r--r--   0 alex       (501) staff       (20)       30 2023-05-30 04:46:48.000000 ezmail-1.0.1/ezmail/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1194 2023-05-31 16:21:05.000000 ezmail-1.0.1/ezmail/__main__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4333 2023-05-31 16:11:51.000000 ezmail-1.0.1/ezmail/ezmail.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-31 16:36:31.797821 ezmail-1.0.1/ezmail.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     4151 2023-05-31 16:36:31.000000 ezmail-1.0.1/ezmail.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      230 2023-05-31 16:36:31.000000 ezmail-1.0.1/ezmail.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-05-31 16:36:31.000000 ezmail-1.0.1/ezmail.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       14 2023-05-31 16:36:31.000000 ezmail-1.0.1/ezmail.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)        7 2023-05-31 16:36:31.000000 ezmail-1.0.1/ezmail.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-05-31 16:36:31.798874 ezmail-1.0.1/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      764 2023-05-31 16:34:59.000000 ezmail-1.0.1/setup.py
```

### Comparing `ezmail-1.0.0/LICENSE` & `ezmail-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezmail-1.0.0/PKG-INFO` & `ezmail-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,90 @@
 Metadata-Version: 2.1
 Name: ezmail
-Version: 1.0.0
+Version: 1.0.1
 Summary: easily send out emails via SMTP
 Home-page: https://github.com/Alex23rodriguez/ezmail
 Author: Alex Rodriguez
 Author-email: alex.rodriguez.oro@gmail.com
 Keywords: python,mail,smtp,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ezmail
+
 easily send out emails via python or the cli using python's SMTP module.
 
 ---
 
 # Getting started
+
 download the package using pip: `pip install ezmail`
 
 ## `.env` file
+
 This module uses environment files to handle sensitive info.
 Make sure the following values are defined in it:
+
 ```.env
 USERNAME=sender@exmaple.com
 PASSWORD=<password>
 SMTP=<provider's SMTP server>
 PORT=<provider's port>
 ```
+
 See examples [below](https://github.com/Alex23rodriguez/ezmail/edit/main/README.md#smtp-servers) for popular providers.
 
 ## send from python
+
 ```python
 from ezmail import send_mail
 
 # by default, an env file named `.env` is searched.
 send_mail(
   subject="Email sent with Python",
   recipients=["r1@example.com", "John Doe <john@example.com>"],
   message="Here go the contents of the message.",
 )
 ```
 
 ## send from the cli
+
 `python -m ezmail -s "Email sent from bash" -r "r1@example.com" "r2@example.com" -m "This is my message."`
 
 ---
 
 # More advanced uses
+
 This module allows adding attachments to the email, as well as reading in the message and / or recipients from a file instead of defining them directly.
 
 ## python
+
 Python automatically detects the type of data that is passed into the different fields.
 
 For example, to read the recipients from a file, simply pass in a Path or file object instead of a list of strings.
 
 A file that defines the recipients must have one recipient per line:
+
 ```recipients.txt
 r1@example.com
 John Doe <john@example.com>
 ```
+
 The message can also be taken from a Path or file object.
 
 To add attachments, pass in a list of Paths or (read-binary) file objects. The type is automatically detected.
 
 If an env file with a name different from `.env` is used, pass it into `envfile` as a Path object or a string
+
 ### For example:
+
 ```python
 from pathlib import Path
 from ezmail import send_mail
 
 recipients_file = Path("path/to/recipients.txt")
 messages_file = open("path/to/message.txt", "r")
 
@@ -87,43 +101,54 @@
   message=messages_file,
   attachments=attachments,
   envfile=envfile
 )
 ```
 
 ## cli
+
 `python -m ezmail --help` to see how to call from the command line
 
 Possible flags:
+
 - `-s` or `--subject`: the subject of the email (single argument)
 - message:
   - `-m` or `--message`: the contents of the email OR
   - `-f` or `--file`: the file containing the contents of the email
 - recipients:
   - `-r` or `--recipients`: the recipients of the email (one or more arguments) OR
   - `-rf` or `--recipientsfile`: the file containing the addresses of the recipients
 - `-a` or `--attachments`: a list of files to attach to the email (one or more arguments)
 - `-e` or `--env`: the env file where the credentials are defined (default `.env`)
+- `-v` or `--verbose`: set SMTP server debug level to 1, to debug possible connection issues
 
 ---
 
 # Popular SMTP servers
+
+Here is a brief description of popular SMTP servers.
+
+If having trouble setting up the SMTP server, pass in `verbose=True` into the python method, or the flag `-v` on the cli version.
+
+## gmail
+
 Gmail constantly changes the requirements to be able to send out emails through SMTP. It is recommended that you follow a [guide](https://www.gmass.co/blog/gmail-smtp/).
 
 Then, fill in the missing values from the following `.env` file
-## gmail
+
 ```.env
 USERNAME=
 PASSWORD=
 SMTP="smtp.gmail.com"
 PORT=465
 ```
 
 # Zoho
+
 Zoho makes it very simple to send emails through SMTP. Fill in the missing values from the following `.env` file and that's it!
+
 ```.env
 USERNAME=
 PASSWORD=
 SMTP="smtp.zoho.com"
 PORT=465
 ```
-
```

### Comparing `ezmail-1.0.0/README.md` & `ezmail-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,75 @@
 # ezmail
+
 easily send out emails via python or the cli using python's SMTP module.
 
 ---
 
 # Getting started
+
 download the package using pip: `pip install ezmail`
 
 ## `.env` file
+
 This module uses environment files to handle sensitive info.
 Make sure the following values are defined in it:
+
 ```.env
 USERNAME=sender@exmaple.com
 PASSWORD=<password>
 SMTP=<provider's SMTP server>
 PORT=<provider's port>
 ```
+
 See examples [below](https://github.com/Alex23rodriguez/ezmail/edit/main/README.md#smtp-servers) for popular providers.
 
 ## send from python
+
 ```python
 from ezmail import send_mail
 
 # by default, an env file named `.env` is searched.
 send_mail(
   subject="Email sent with Python",
   recipients=["r1@example.com", "John Doe <john@example.com>"],
   message="Here go the contents of the message.",
 )
 ```
 
 ## send from the cli
+
 `python -m ezmail -s "Email sent from bash" -r "r1@example.com" "r2@example.com" -m "This is my message."`
 
 ---
 
 # More advanced uses
+
 This module allows adding attachments to the email, as well as reading in the message and / or recipients from a file instead of defining them directly.
 
 ## python
+
 Python automatically detects the type of data that is passed into the different fields.
 
 For example, to read the recipients from a file, simply pass in a Path or file object instead of a list of strings.
 
 A file that defines the recipients must have one recipient per line:
+
 ```recipients.txt
 r1@example.com
 John Doe <john@example.com>
 ```
+
 The message can also be taken from a Path or file object.
 
 To add attachments, pass in a list of Paths or (read-binary) file objects. The type is automatically detected.
 
 If an env file with a name different from `.env` is used, pass it into `envfile` as a Path object or a string
+
 ### For example:
+
 ```python
 from pathlib import Path
 from ezmail import send_mail
 
 recipients_file = Path("path/to/recipients.txt")
 messages_file = open("path/to/message.txt", "r")
 
@@ -73,43 +86,54 @@
   message=messages_file,
   attachments=attachments,
   envfile=envfile
 )
 ```
 
 ## cli
+
 `python -m ezmail --help` to see how to call from the command line
 
 Possible flags:
+
 - `-s` or `--subject`: the subject of the email (single argument)
 - message:
   - `-m` or `--message`: the contents of the email OR
   - `-f` or `--file`: the file containing the contents of the email
 - recipients:
   - `-r` or `--recipients`: the recipients of the email (one or more arguments) OR
   - `-rf` or `--recipientsfile`: the file containing the addresses of the recipients
 - `-a` or `--attachments`: a list of files to attach to the email (one or more arguments)
 - `-e` or `--env`: the env file where the credentials are defined (default `.env`)
+- `-v` or `--verbose`: set SMTP server debug level to 1, to debug possible connection issues
 
 ---
 
 # Popular SMTP servers
+
+Here is a brief description of popular SMTP servers.
+
+If having trouble setting up the SMTP server, pass in `verbose=True` into the python method, or the flag `-v` on the cli version.
+
+## gmail
+
 Gmail constantly changes the requirements to be able to send out emails through SMTP. It is recommended that you follow a [guide](https://www.gmass.co/blog/gmail-smtp/).
 
 Then, fill in the missing values from the following `.env` file
-## gmail
+
 ```.env
 USERNAME=
 PASSWORD=
 SMTP="smtp.gmail.com"
 PORT=465
 ```
 
 # Zoho
+
 Zoho makes it very simple to send emails through SMTP. Fill in the missing values from the following `.env` file and that's it!
+
 ```.env
 USERNAME=
 PASSWORD=
 SMTP="smtp.zoho.com"
 PORT=465
 ```
-
```

### Comparing `ezmail-1.0.0/ezmail/__main__.py` & `ezmail-1.0.1/ezmail/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 group2.add_argument("-r", "--recipients", nargs="+")
 group2.add_argument("-rf", "--recipientsfile", type=FileType("r"))
 
 parser.add_argument("-a", "--attachments", nargs="+", type=FileType("rb"), default=[])
 
 parser.add_argument("-e", "--env", required=False, default=".env")
 
+parser.add_argument("-v", "--verbose", action="store_true")
+
 args = parser.parse_args()
 
 if args.recipients:
     recipients = args.recipients
 else:
     recipients = args.recipientsfile.read().splitlines()
 
@@ -35,8 +37,9 @@
 
 send_mail(
     envfile=args.env,
     recipients=recipients,
     subject=args.subject,
     message=message,
     attachments=args.attachments,
+    verbose=args.verbose,
 )
```

### Comparing `ezmail-1.0.0/ezmail/ezmail.py` & `ezmail-1.0.1/ezmail/ezmail.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from email.message import EmailMessage
 from io import BufferedReader, TextIOWrapper
 from pathlib import Path
 import ssl
 import smtplib
 from mimetypes import guess_type
+from typing import Union
 
 from dotenv import dotenv_values
 
 
 def send_mail(
     *,
-    envfile: str | Path = ".env",
-    recipients: list[str] | Path | TextIOWrapper,
+    envfile: Union[str, Path] = ".env",
+    recipients: Union[list[str], Path, TextIOWrapper],
     subject: str,
-    message: str | Path | TextIOWrapper,
-    attachments: list[Path] | list[BufferedReader] = [],
+    message: Union[str, Path, TextIOWrapper],
+    attachments: Union[list[Path], list[BufferedReader]] = [],
+    verbose: bool = False,
 ):
     envfile = Path(envfile)
     assert (
         envfile.exists() and envfile.is_file()
     ), "Could not load specified environment file!"
 
     environ = dotenv_values(envfile)
@@ -27,15 +29,15 @@
         key in environ for key in ("PORT", "USERNAME", "PASSWORD", "SMTP")
     ), "environment found, but incomplete!"
     port = int(environ["PORT"])
     sender = environ["USERNAME"]
     password = environ["PASSWORD"]
     smtp_server = environ["SMTP"]
 
-    def tofile(a: Path | BufferedReader) -> BufferedReader:
+    def tofile(a: Union[Path, BufferedReader]) -> BufferedReader:
         if isinstance(a, Path):
             return open(a, "rb")
 
         assert type(a) is BufferedReader, type(a)
         return a
 
     assert any(
@@ -93,15 +95,16 @@
         )
 
     ### setup to connect to ssl (secure) server
     context = ssl.create_default_context()
 
     # establish connection and send email
     with smtplib.SMTP_SSL(smtp_server, port, context=context) as smtp:
-        # smtp.set_debuglevel(1)
+        if verbose:
+            smtp.set_debuglevel(1)
         smtp.login(sender, password)
         smtp.send_message(em)
 
     print("mail sent successfully")
 
 
 ### parse arguments
```

### Comparing `ezmail-1.0.0/ezmail.egg-info/PKG-INFO` & `ezmail-1.0.1/ezmail.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,90 @@
 Metadata-Version: 2.1
 Name: ezmail
-Version: 1.0.0
+Version: 1.0.1
 Summary: easily send out emails via SMTP
 Home-page: https://github.com/Alex23rodriguez/ezmail
 Author: Alex Rodriguez
 Author-email: alex.rodriguez.oro@gmail.com
 Keywords: python,mail,smtp,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ezmail
+
 easily send out emails via python or the cli using python's SMTP module.
 
 ---
 
 # Getting started
+
 download the package using pip: `pip install ezmail`
 
 ## `.env` file
+
 This module uses environment files to handle sensitive info.
 Make sure the following values are defined in it:
+
 ```.env
 USERNAME=sender@exmaple.com
 PASSWORD=<password>
 SMTP=<provider's SMTP server>
 PORT=<provider's port>
 ```
+
 See examples [below](https://github.com/Alex23rodriguez/ezmail/edit/main/README.md#smtp-servers) for popular providers.
 
 ## send from python
+
 ```python
 from ezmail import send_mail
 
 # by default, an env file named `.env` is searched.
 send_mail(
   subject="Email sent with Python",
   recipients=["r1@example.com", "John Doe <john@example.com>"],
   message="Here go the contents of the message.",
 )
 ```
 
 ## send from the cli
+
 `python -m ezmail -s "Email sent from bash" -r "r1@example.com" "r2@example.com" -m "This is my message."`
 
 ---
 
 # More advanced uses
+
 This module allows adding attachments to the email, as well as reading in the message and / or recipients from a file instead of defining them directly.
 
 ## python
+
 Python automatically detects the type of data that is passed into the different fields.
 
 For example, to read the recipients from a file, simply pass in a Path or file object instead of a list of strings.
 
 A file that defines the recipients must have one recipient per line:
+
 ```recipients.txt
 r1@example.com
 John Doe <john@example.com>
 ```
+
 The message can also be taken from a Path or file object.
 
 To add attachments, pass in a list of Paths or (read-binary) file objects. The type is automatically detected.
 
 If an env file with a name different from `.env` is used, pass it into `envfile` as a Path object or a string
+
 ### For example:
+
 ```python
 from pathlib import Path
 from ezmail import send_mail
 
 recipients_file = Path("path/to/recipients.txt")
 messages_file = open("path/to/message.txt", "r")
 
@@ -87,43 +101,54 @@
   message=messages_file,
   attachments=attachments,
   envfile=envfile
 )
 ```
 
 ## cli
+
 `python -m ezmail --help` to see how to call from the command line
 
 Possible flags:
+
 - `-s` or `--subject`: the subject of the email (single argument)
 - message:
   - `-m` or `--message`: the contents of the email OR
   - `-f` or `--file`: the file containing the contents of the email
 - recipients:
   - `-r` or `--recipients`: the recipients of the email (one or more arguments) OR
   - `-rf` or `--recipientsfile`: the file containing the addresses of the recipients
 - `-a` or `--attachments`: a list of files to attach to the email (one or more arguments)
 - `-e` or `--env`: the env file where the credentials are defined (default `.env`)
+- `-v` or `--verbose`: set SMTP server debug level to 1, to debug possible connection issues
 
 ---
 
 # Popular SMTP servers
+
+Here is a brief description of popular SMTP servers.
+
+If having trouble setting up the SMTP server, pass in `verbose=True` into the python method, or the flag `-v` on the cli version.
+
+## gmail
+
 Gmail constantly changes the requirements to be able to send out emails through SMTP. It is recommended that you follow a [guide](https://www.gmass.co/blog/gmail-smtp/).
 
 Then, fill in the missing values from the following `.env` file
-## gmail
+
 ```.env
 USERNAME=
 PASSWORD=
 SMTP="smtp.gmail.com"
 PORT=465
 ```
 
 # Zoho
+
 Zoho makes it very simple to send emails through SMTP. Fill in the missing values from the following `.env` file and that's it!
+
 ```.env
 USERNAME=
 PASSWORD=
 SMTP="smtp.zoho.com"
 PORT=465
 ```
-
```

### Comparing `ezmail-1.0.0/setup.py` & `ezmail-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ezmail",
-    version="1.0.0",
+    version="1.0.1",
     author="Alex Rodriguez",
     author_email="alex.rodriguez.oro@gmail.com",
     description="easily send out emails via SMTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Alex23rodriguez/ezmail",
     packages=setuptools.find_packages(),
     keywords=["python", "mail", "smtp", "cli"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=["python-dotenv"],
+    python_requires=">=3.9",
 )
```

