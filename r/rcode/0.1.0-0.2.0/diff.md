# Comparing `tmp/rcode-0.1.0.tar.gz` & `tmp/rcode-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcode-0.1.0.tar", last modified: Wed Jun 22 12:21:38 2022, max compression
+gzip compressed data, was "rcode-0.2.0.tar", last modified: Wed May 31 14:28:36 2023, max compression
```

## Comparing `rcode-0.1.0.tar` & `rcode-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2022-06-22 12:21:38.785254 rcode-0.1.0/
--rw-r--r--   0 hyi        (502) staff       (20)     1075 2022-05-04 07:51:13.000000 rcode-0.1.0/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)      714 2022-06-22 12:21:38.784988 rcode-0.1.0/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     1000 2022-06-22 12:19:51.000000 rcode-0.1.0/README.md
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2022-06-22 12:21:38.781322 rcode-0.1.0/rcode/
--rw-r--r--   0 hyi        (502) staff       (20)       20 2022-05-04 07:51:13.000000 rcode-0.1.0/rcode/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       63 2022-05-04 07:51:13.000000 rcode-0.1.0/rcode/__main__.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     5306 2022-06-22 12:20:04.000000 rcode-0.1.0/rcode/rcode.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2022-06-22 12:21:38.784397 rcode-0.1.0/rcode.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)      714 2022-06-22 12:21:38.000000 rcode-0.1.0/rcode.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      277 2022-06-22 12:21:38.000000 rcode-0.1.0/rcode.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2022-06-22 12:21:38.000000 rcode-0.1.0/rcode.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       43 2022-06-22 12:21:38.000000 rcode-0.1.0/rcode.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)        8 2022-06-22 12:21:38.000000 rcode-0.1.0/rcode.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)        6 2022-06-22 12:21:38.000000 rcode-0.1.0/rcode.egg-info/top_level.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2022-05-04 07:53:39.000000 rcode-0.1.0/rcode.egg-info/zip-safe
--rw-r--r--   0 hyi        (502) staff       (20)       38 2022-06-22 12:21:38.785349 rcode-0.1.0/setup.cfg
--rw-r--r--   0 hyi        (502) staff       (20)      965 2022-06-22 12:21:26.000000 rcode-0.1.0/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-31 14:28:36.239100 rcode-0.2.0/
+-rw-r--r--   0 hyi        (502) staff       (20)     1075 2023-05-31 14:01:02.000000 rcode-0.2.0/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)      569 2023-05-31 14:28:36.238899 rcode-0.2.0/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     1075 2023-05-31 14:28:11.000000 rcode-0.2.0/README.md
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-31 14:28:36.236137 rcode-0.2.0/rcode/
+-rw-r--r--   0 hyi        (502) staff       (20)       20 2023-05-31 14:01:02.000000 rcode-0.2.0/rcode/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       63 2023-05-31 14:01:02.000000 rcode-0.2.0/rcode/__main__.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)     5975 2023-05-31 14:26:19.000000 rcode-0.2.0/rcode/rcode.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-31 14:28:36.238491 rcode-0.2.0/rcode.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)      569 2023-05-31 14:28:36.000000 rcode-0.2.0/rcode.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      277 2023-05-31 14:28:36.000000 rcode-0.2.0/rcode.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2023-05-31 14:28:36.000000 rcode-0.2.0/rcode.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       43 2023-05-31 14:28:36.000000 rcode-0.2.0/rcode.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        8 2023-05-31 14:28:36.000000 rcode-0.2.0/rcode.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        6 2023-05-31 14:28:36.000000 rcode-0.2.0/rcode.egg-info/top_level.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2023-05-31 14:03:42.000000 rcode-0.2.0/rcode.egg-info/zip-safe
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2023-05-31 14:28:36.239163 rcode-0.2.0/setup.cfg
+-rw-r--r--   0 hyi        (502) staff       (20)      867 2023-05-31 14:28:23.000000 rcode-0.2.0/setup.py
```

### Comparing `rcode-0.1.0/LICENSE` & `rcode-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcode-0.1.0/PKG-INFO` & `rcode-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 Metadata-Version: 2.1
 Name: rcode
-Version: 0.1.0
+Version: 0.2.0
 Summary: vscode remode code .
 Home-page: https://github.com/yihong0618/code-connect
 Author: chvolkmann, yihong0618
 Author-email: zouzou0208@gmail.com
-License: UNKNOWN
 Keywords: python vscode
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `rcode-0.1.0/README.md` & `rcode-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 ## INFO
 
 1. pip3 install rcode (or clone it pip3 install .)
 2. install socat like: (sudo yum install socat)
 3. just `rcode file` like your VSCode `code .`
 4. local open remote use rcode if you use `.ssh/config` --> `rcode remote_ssh ~/test`
+5. local open latest remote `.ssh/config` --> `rcode -l or rcode --latest`
 
 > Note:
 > - Be sure to [connect to the remote host](https://code.visualstudio.com/docs/remote/ssh#_connect-to-a-remote-host) first before typing any `rcode` in the terminal
 > - We may want to add `~/.local/bin` in to your `$PATH` in your `~/.zshrc` or `~/.bashrc` to enable `rcode` being resolved properly
 > ```diff
 > - export PATH=$PATH:/usr/local/go/bin
 > + export PATH=$PATH:/usr/local/go/bin:~/.local/bin
```

### Comparing `rcode-0.1.0/rcode/rcode.py` & `rcode-0.2.0/rcode/rcode.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             "Please make sure to connect to this machine with a standard "
             + "VS Code remote SSH session before using this tool.",
         )
 
 
 def is_remote_vscode() -> bool:
     code_repos = Path.home().glob(".vscode-server/bin/*")
-    return len(list(code_repos)) > 0
+    return len(list(code_repos)) > 0 and os.getenv('SSH_CLIENT')
 
 
 def get_code_binary() -> Path:
     """Returns the path to the most recently accessed code executable."""
 
     # Every entry in ~/.vscode-server/bin corresponds to a commit id
     # Pick the most recent one
@@ -126,27 +126,41 @@
         # run the "code" executable with the proper environment variable set
         # stdout/stderr remain connected to the current process
         proc = sp.run(args)
         # return the same exit code as the wrapped process
         exit(proc.returncode)
     else:
         # run local to open remote
+        rcode_home = Path.home() / ".rcode" 
         ssh_remote = "vscode-remote://ssh-remote+{remote_name}{remote_dir}"
-        assert len(args) == 3
+        if args[1] == "-l" or args[1] == "--latest":
+            if os.path.exists(rcode_home):
+                with open(rcode_home) as f:
+                    if l := list(f.read().splitlines()):
+                        ssh_remote_latest = l[-1]
+                        proc = sp.run(["code", "--folder-uri", ssh_remote_latest])
+                        exit(proc.returncode)
+                    else:
+                        print("Not use rcode before")
+                        return
+        else:
+            assert len(args) == 3
         sshs = read_ssh_config(expanduser("~/.ssh/config"))
         hosts = sshs.hosts()
         remote_name = args[1]
         if remote_name not in hosts:
             raise Exception("Please config your .ssh config to use this")
         dir_name = args[2]
         local_home_dir = expanduser("~")
         if args[2].startswith(local_home_dir):
             user_name = sshs.host(remote_name).get("user", "root")
             # replace with the remote ~
             dir_name = str(args[2]).replace(local_home_dir, f"/home/{user_name}")
         ssh_remote = ssh_remote.format(remote_name=remote_name, remote_dir=dir_name) 
+        with open(rcode_home, "a") as f:
+            f.write(ssh_remote + str(os.linesep))
         proc = sp.run(["code", "--folder-uri", ssh_remote])
         exit(proc.returncode)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `rcode-0.1.0/rcode.egg-info/PKG-INFO` & `rcode-0.2.0/rcode.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 Metadata-Version: 2.1
 Name: rcode
-Version: 0.1.0
+Version: 0.2.0
 Summary: vscode remode code .
 Home-page: https://github.com/yihong0618/code-connect
 Author: chvolkmann, yihong0618
 Author-email: zouzou0208@gmail.com
-License: UNKNOWN
 Keywords: python vscode
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `rcode-0.1.0/setup.py` & `rcode-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.0"
+VERSION = "0.2.0"
 
 setup(
     name="rcode",
     version=VERSION,
     description="vscode remode code .",
     keywords="python vscode",
     author="chvolkmann, yihong0618",
@@ -17,16 +17,14 @@
         'sshconf'
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Libraries",
     ],
     entry_points={
         "console_scripts": ["rcode = rcode.rcode:main"],
     },
```

