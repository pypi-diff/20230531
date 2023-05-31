# Comparing `tmp/edwh_sshfs_plugin-0.1.1.tar.gz` & `tmp/edwh_sshfs_plugin-0.1.2.tar.gz`

## Comparing `edwh_sshfs_plugin-0.1.1.tar` & `edwh_sshfs_plugin-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,11 @@
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/test.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/src/edwh_sshfs_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/src/edwh_sshfs_plugin/__init__.py
--rw-r--r--   0        0        0     7718 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/src/edwh_sshfs_plugin/fabfile.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/tests/test_sshfs.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/tests/sshfs_test_dir/hi.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/README.md
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/src/edwh_sshfs_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/src/edwh_sshfs_plugin/__init__.py
+-rw-r--r--   0        0        0     7927 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/src/edwh_sshfs_plugin/fabfile.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/tests/test_sshfs.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/README.md
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 edwh_sshfs_plugin-0.1.2/PKG-INFO
```

### Comparing `edwh_sshfs_plugin-0.1.1/CHANGELOG.md` & `edwh_sshfs_plugin-0.1.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.2 (2023-05-31)
+### Fix
+* **import:** Don't crash the entire edwh tool if sshfs is not installed! ([`03b8365`](https://github.com/educationwarehouse/edwh-sshfs-plugin/commit/03b836576b36d3c814a9678ad0b98fd12a7e246f))
+
 ## v0.1.1 (2023-05-25)
 ### Fix
 * Set umask to highest permission level ([`c8c7362`](https://github.com/educationwarehouse/edwh-sshfs-plugin/commit/c8c7362b8ea77c0ec62672bdaaa798b388806c89))
 * Pytest use anyio instead of anyio now. also events are used now instead of queue's for simplicity and added allow root instead of allow other ([`6c002b6`](https://github.com/educationwarehouse/edwh-sshfs-plugin/commit/6c002b681e77a6f31ee135468bf541601b0e5a55))
 * Pytest use anyio instead of anyio now. also events are used now instead of queue's for simplicity ([`913f135`](https://github.com/educationwarehouse/edwh-sshfs-plugin/commit/913f135e167bf83f5bec3ce6340c81c2e85f75f3))
 * Added umask and removed ro because ro is (read-only) ([`3f63ff0`](https://github.com/educationwarehouse/edwh-sshfs-plugin/commit/3f63ff0c7fde0b21b1e369cbf3693c60252ad6dd))
 * Added ro ([`0d9e27d`](https://github.com/educationwarehouse/edwh-sshfs-plugin/commit/0d9e27daa3eb31f7c28c4129869675cd530562ab))
```

### Comparing `edwh_sshfs_plugin-0.1.1/src/edwh_sshfs_plugin/fabfile.py` & `edwh_sshfs_plugin-0.1.2/src/edwh_sshfs_plugin/fabfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,28 @@
-import asyncio
 import os
 import socket
 import getpass
+import warnings
+
 import invoke
 from plumbum import BG
-from plumbum.cmd import ssh, sshfs
+from plumbum.commands.processes import CommandNotFound
 from fabric import task
 import anyio
 
+try:
+    from plumbum.cmd import ssh, sshfs
+except CommandNotFound:
+    warnings.warn("edwh sshfs plugin is installed but sshfs is missing. "
+                  "Please check README.md#installation on how to fix this! "
+                  "The commands in this plugin will NOT work unless this is fixed.")
+
 STOP_RUNNING = False
 
+
 def get_available_port(c):
     """
     Retrieves an available port that is both locally and remotely accessible.
 
     Args:
         c: The connection object used to communicate with the remote server.
 
@@ -98,17 +107,17 @@
         c.run(f"lsof -n {dir} 2>/dev/null")
         pids = c.run("lsof -t -n /home/ubuntu/testing 2>/dev/null", hide=True).stdout.strip().split('\n')
         print(f'Terminate with: kill {" ".join(pids)}; sleep 2; umount {dir}')
     else:
         print("successfully exited :)")
 
 
-@task(help={'workstation-dir' : "The directory path on the local machine to mount the server directory.",
-            'server-dir' : "The directory path on the remote server to be mounted.",
-            'queue' : "An optional queue object used for synchronization. Defaults to None, optional"})
+@task(help={'workstation-dir': "The directory path on the local machine to mount the server directory.",
+            'server-dir': "The directory path on the remote server to be mounted.",
+            'queue': "An optional queue object used for synchronization. Defaults to None, optional"})
 def remote_mount(c, workstation_dir, server_dir, queue=None):
     """
     The remote_mount function is an asynchronous Python task that allows you to mount a remote directory
     on your local machine using SSHFS (SSH Filesystem). It establishes a secure connection to a remote server,
     forwards a port, and mounts the remote directory on the local machine.
 
     Returns:
@@ -118,17 +127,17 @@
         print("please give up a host using -H")
         exit(255)
 
     # get an available port that is usable on local and remote so we can setup a connection with the ports
     port = get_available_port(c)
     ssh_cmd = ssh["-A", f"-R {port}:127.0.0.1:22", f"{c.user}@{c.host}"]
     sshfs_cmd = ssh_cmd["sshfs", "-f", f"-p {port}", "-o allow_root,default_permissions",
-                        "-o StrictHostKeyChecking=no,reconnect,ServerAliveInterval=3,ServerAliveCountMax=3," \
-                        f"uid={getuid()},gid={getgid()}",
-                        f"{getpass.getuser()}@127.0.0.1:{workstation_dir}", f"{server_dir}"]
+    "-o StrictHostKeyChecking=no,reconnect,ServerAliveInterval=3,ServerAliveCountMax=3," \
+    f"uid={getuid()},gid={getgid()}",
+    f"{getpass.getuser()}@127.0.0.1:{workstation_dir}", f"{server_dir}"]
 
     if not queue:
         print(f"starting sshfs with(started when nothing happens): {str(sshfs_cmd)}")
     try:
         sshfs_cmd()
     except KeyboardInterrupt:
         unmount_dir(c, server_dir)
@@ -147,40 +156,41 @@
             None
         """
     # os.popen(f"lsof -n {workstation_dir} 2>/dev/null")
     if not hasattr(c, "host"):
         print("please give up a host using -H")
         exit(255)
     # TODO: remove mount on exit
-    sshfs_cmd = sshfs[  "-f", "-o", "allow_root,default_permissions,umask=000,StrictHostKeyChecking=no,reconnect," \
-                        f"uid={getuid()},gid={getgid()}",
-                        f"{c.user}@{c.host}:{server_dir}", workstation_dir]
+    sshfs_cmd = sshfs["-f", "-o", "allow_root,default_permissions,umask=000,StrictHostKeyChecking=no,reconnect," \
+                                  f"uid={getuid()},gid={getgid()}",
+    f"{c.user}@{c.host}:{server_dir}", workstation_dir]
 
     if not queue:
         print("running sshfs...")
 
     sshfs_cmd()
 
     local_connection = invoke.context.Context()
     local_connection.run(f"umount {workstation_dir}", hide=True)
 
-#----------------------------------#
-#|             async              |#
-#----------------------------------#
+
+# ----------------------------------#
+# |             async              |#
+# ----------------------------------#
 
 async def async_local_mount(c, workstation_dir, server_dir, event=None):
     """
     async version of local_mount
     """
     if not hasattr(c, "host"):
         print("please give up a host using -H")
         exit(255)
 
     sshfs_cmd = sshfs["-f", "-o", "allow_root,default_permissions,umask=000,StrictHostKeyChecking=no,reconnect," \
-                        f"uid={getuid()},gid={getgid()}",
+                                  f"uid={getuid()},gid={getgid()}",
     f"{c.user}@{c.host}:{server_dir}", workstation_dir]
 
     if not event:
         print("running sshfs...")
 
     process = sshfs_cmd & BG
     await event.wait()
@@ -188,33 +198,34 @@
     process.proc.terminate()
 
     local_connection = invoke.context.Context()
     local_connection.run(f"umount {workstation_dir}", warn=True, hide=True)
 
     await anyio.sleep(1)
 
+
 async def async_remote_mount(c, workstation_dir, server_dir, event=None):
     """
     async version of remote_mount
     """
     if not hasattr(c, "host"):
         print("please give up a host using -H")
         exit(255)
 
     # get an available port that is usable on local and remote so we can setup a connection with the ports
     port = get_available_port(c)
     ssh_cmd = ssh["-A", f"-R {port}:127.0.0.1:22", f"{c.user}@{c.host}"]
     sshfs_cmd = ssh_cmd["sshfs", "-f", f"-p {port}", "-o allow_root,default_permissions",
-                        "-o StrictHostKeyChecking=no,reconnect,ServerAliveInterval=3,ServerAliveCountMax=3," \
-                        f"uid={getuid()},gid={getgid()}",
-                        f"{getpass.getuser()}@127.0.0.1:{workstation_dir}", f"{server_dir}"]
+    "-o StrictHostKeyChecking=no,reconnect,ServerAliveInterval=3,ServerAliveCountMax=3," \
+    f"uid={getuid()},gid={getgid()}",
+    f"{getpass.getuser()}@127.0.0.1:{workstation_dir}", f"{server_dir}"]
 
     if not event:
         print(f"starting sshfs with(started when nothing happens): {str(sshfs_cmd)}")
     try:
         process = sshfs_cmd & BG
         await event.wait()
         process.proc.terminate()
         await anyio.sleep(1)
         c.run(f"umount {server_dir}", warn=True, hide=True)
     except KeyboardInterrupt:
-        unmount_dir(c, server_dir)
+        unmount_dir(c, server_dir)
```

### Comparing `edwh_sshfs_plugin-0.1.1/tests/test_sshfs.py` & `edwh_sshfs_plugin-0.1.2/tests/test_sshfs.py`

 * *Files identical despite different names*

### Comparing `edwh_sshfs_plugin-0.1.1/LICENSE.txt` & `edwh_sshfs_plugin-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_sshfs_plugin-0.1.1/README.md` & `edwh_sshfs_plugin-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `edwh_sshfs_plugin-0.1.1/pyproject.toml` & `edwh_sshfs_plugin-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_sshfs_plugin-0.1.1/PKG-INFO` & `edwh_sshfs_plugin-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-sshfs-plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: sshfs project with a plugin to be discovered from the edwh package
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-sshfs-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-sshfs-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-sshfs-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

