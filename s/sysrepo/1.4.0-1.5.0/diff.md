# Comparing `tmp/sysrepo-1.4.0.tar.gz` & `tmp/sysrepo-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysrepo-1.4.0.tar", last modified: Mon Dec  5 16:19:12 2022, max compression
+gzip compressed data, was "sysrepo-1.5.0.tar", last modified: Wed May 31 14:27:54 2023, max compression
```

## Comparing `sysrepo-1.4.0.tar` & `sysrepo-1.5.0.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 16:19:12.497022 sysrepo-1.4.0/
--rw-r--r--   0 root         (0) root         (0)     1565 2022-12-05 16:19:00.000000 sysrepo-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      188 2022-12-05 16:19:00.000000 sysrepo-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6268 2022-12-05 16:19:12.497022 sysrepo-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5684 2022-12-05 16:19:00.000000 sysrepo-1.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 16:19:12.493022 sysrepo-1.4.0/cffi/
--rw-r--r--   0 root         (0) root         (0)     1156 2022-12-05 16:19:00.000000 sysrepo-1.4.0/cffi/build.py
--rw-r--r--   0 root         (0) root         (0)     9108 2022-12-05 16:19:00.000000 sysrepo-1.4.0/cffi/cdefs.h
--rw-r--r--   0 root         (0) root         (0)      320 2022-12-05 16:19:00.000000 sysrepo-1.4.0/cffi/source.c
--rw-r--r--   0 root         (0) root         (0)      360 2022-12-05 16:19:00.000000 sysrepo-1.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      730 2022-12-05 16:19:12.497022 sysrepo-1.4.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     5502 2022-12-05 16:19:00.000000 sysrepo-1.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 16:19:12.497022 sysrepo-1.4.0/sysrepo/
--rw-r--r--   0 root         (0) root         (0)        6 2022-12-05 16:19:12.497022 sysrepo-1.4.0/sysrepo/VERSION
--rw-r--r--   0 root         (0) root         (0)     2114 2022-12-05 16:19:00.000000 sysrepo-1.4.0/sysrepo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8369 2022-12-05 16:19:00.000000 sysrepo-1.4.0/sysrepo/change.py
--rw-r--r--   0 root         (0) root         (0)     9186 2022-12-05 16:19:00.000000 sysrepo-1.4.0/sysrepo/connection.py
--rw-r--r--   0 root         (0) root         (0)     4671 2022-12-05 16:19:00.000000 sysrepo-1.4.0/sysrepo/errors.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-05 16:19:00.000000 sysrepo-1.4.0/sysrepo/py.typed
--rw-r--r--   0 root         (0) root         (0)    52779 2022-12-05 16:19:00.000000 sysrepo-1.4.0/sysrepo/session.py
--rw-r--r--   0 root         (0) root         (0)    24143 2022-12-05 16:19:00.000000 sysrepo-1.4.0/sysrepo/subscription.py
--rw-r--r--   0 root         (0) root         (0)     3421 2022-12-05 16:19:00.000000 sysrepo-1.4.0/sysrepo/util.py
--rw-r--r--   0 root         (0) root         (0)     5319 2022-12-05 16:19:00.000000 sysrepo-1.4.0/sysrepo/value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 16:19:12.497022 sysrepo-1.4.0/sysrepo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6268 2022-12-05 16:19:12.000000 sysrepo-1.4.0/sysrepo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2022-12-05 16:19:12.000000 sysrepo-1.4.0/sysrepo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-05 16:19:12.000000 sysrepo-1.4.0/sysrepo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-05 16:19:12.000000 sysrepo-1.4.0/sysrepo.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       63 2022-12-05 16:19:12.000000 sysrepo-1.4.0/sysrepo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-12-05 16:19:12.000000 sysrepo-1.4.0/sysrepo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:27:54.710266 sysrepo-1.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-05-31 14:27:43.000000 sysrepo-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-31 14:27:43.000000 sysrepo-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6268 2023-05-31 14:27:54.710266 sysrepo-1.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5684 2023-05-31 14:27:43.000000 sysrepo-1.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:27:54.706266 sysrepo-1.5.0/cffi/
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-05-31 14:27:43.000000 sysrepo-1.5.0/cffi/build.py
+-rw-r--r--   0 root         (0) root         (0)     9108 2023-05-31 14:27:43.000000 sysrepo-1.5.0/cffi/cdefs.h
+-rw-r--r--   0 root         (0) root         (0)      320 2023-05-31 14:27:43.000000 sysrepo-1.5.0/cffi/source.c
+-rw-r--r--   0 root         (0) root         (0)      360 2023-05-31 14:27:43.000000 sysrepo-1.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      730 2023-05-31 14:27:54.710266 sysrepo-1.5.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     5502 2023-05-31 14:27:43.000000 sysrepo-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:27:54.710266 sysrepo-1.5.0/sysrepo/
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-31 14:27:54.710266 sysrepo-1.5.0/sysrepo/VERSION
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-05-31 14:27:43.000000 sysrepo-1.5.0/sysrepo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8364 2023-05-31 14:27:43.000000 sysrepo-1.5.0/sysrepo/change.py
+-rw-r--r--   0 root         (0) root         (0)     9186 2023-05-31 14:27:43.000000 sysrepo-1.5.0/sysrepo/connection.py
+-rw-r--r--   0 root         (0) root         (0)     4670 2023-05-31 14:27:43.000000 sysrepo-1.5.0/sysrepo/errors.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 14:27:43.000000 sysrepo-1.5.0/sysrepo/py.typed
+-rw-r--r--   0 root         (0) root         (0)    57499 2023-05-31 14:27:43.000000 sysrepo-1.5.0/sysrepo/session.py
+-rw-r--r--   0 root         (0) root         (0)    24606 2023-05-31 14:27:43.000000 sysrepo-1.5.0/sysrepo/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     3421 2023-05-31 14:27:43.000000 sysrepo-1.5.0/sysrepo/util.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2023-05-31 14:27:43.000000 sysrepo-1.5.0/sysrepo/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:27:54.710266 sysrepo-1.5.0/sysrepo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6268 2023-05-31 14:27:54.000000 sysrepo-1.5.0/sysrepo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      619 2023-05-31 14:27:54.000000 sysrepo-1.5.0/sysrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 14:27:54.000000 sysrepo-1.5.0/sysrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 14:27:54.000000 sysrepo-1.5.0/sysrepo.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-31 14:27:54.000000 sysrepo-1.5.0/sysrepo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-31 14:27:54.000000 sysrepo-1.5.0/sysrepo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:27:54.710266 sysrepo-1.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-05-31 14:27:43.000000 sysrepo-1.5.0/tests/test_connection.py
+-rw-r--r--   0 root         (0) root         (0)     5568 2023-05-31 14:27:43.000000 sysrepo-1.5.0/tests/test_session.py
+-rw-r--r--   0 root         (0) root         (0)    18765 2023-05-31 14:27:43.000000 sysrepo-1.5.0/tests/test_subs_module_change.py
+-rw-r--r--   0 root         (0) root         (0)     3356 2023-05-31 14:27:43.000000 sysrepo-1.5.0/tests/test_subs_notification.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2023-05-31 14:27:43.000000 sysrepo-1.5.0/tests/test_subs_oper.py
+-rw-r--r--   0 root         (0) root         (0)     6482 2023-05-31 14:27:43.000000 sysrepo-1.5.0/tests/test_subs_rpc.py
```

### Comparing `sysrepo-1.4.0/LICENSE` & `sysrepo-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sysrepo-1.4.0/PKG-INFO` & `sysrepo-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrepo
-Version: 1.4.0
+Version: 1.5.0
 Summary: Sysrepo CFFI bindings
 Home-page: https://www.6wind.com/
 Author: Robin Jarry
 Author-email: robin.jarry@6wind.com
 License: BSD 3 clause
 Keywords: sysrepo,libyang,cffi
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sysrepo-1.4.0/README.rst` & `sysrepo-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `sysrepo-1.4.0/cffi/build.py` & `sysrepo-1.5.0/cffi/build.py`

 * *Files identical despite different names*

### Comparing `sysrepo-1.4.0/cffi/cdefs.h` & `sysrepo-1.5.0/cffi/cdefs.h`

 * *Files identical despite different names*

### Comparing `sysrepo-1.4.0/setup.cfg` & `sysrepo-1.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sysrepo-1.4.0/setup.py` & `sysrepo-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `sysrepo-1.4.0/sysrepo/__init__.py` & `sysrepo-1.5.0/sysrepo/__init__.py`

 * *Files identical despite different names*

### Comparing `sysrepo-1.4.0/sysrepo/change.py` & `sysrepo-1.5.0/sysrepo/change.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import libyang
 
 from _sysrepo import lib
 
 
 # ------------------------------------------------------------------------------
 class Change:
-
     __slots__ = ("xpath",)
 
     def __init__(self, xpath: str):
         self.xpath = xpath
 
     class Skip(Exception):
         """
@@ -109,15 +108,14 @@
 
     def __str__(self) -> str:
         return self.xpath
 
 
 # ------------------------------------------------------------------------------
 class ChangeCreated(Change):
-
     __slots__ = ("value", "after")
 
     def __init__(self, xpath: str, value: Any, after: Optional[str] = None):
         super().__init__(xpath)
         self.value = value
         self.after = after
 
@@ -134,15 +132,14 @@
         if self.after is not None:
             return "%s: %r: AFTER %r" % (self.xpath, self.value, self.after)
         return "%s: %r" % (self.xpath, self.value)
 
 
 # ------------------------------------------------------------------------------
 class ChangeModified(Change):
-
     __slots__ = ("value", "prev_val", "prev_dflt")
 
     def __init__(self, xpath: str, value: Any, prev_val: str, prev_dflt: bool = False):
         super().__init__(xpath)
         self.value = value
         self.prev_val = prev_val
         self.prev_dflt = prev_dflt
@@ -157,15 +154,14 @@
 
     def __str__(self) -> str:
         return "%s: %r -> %r" % (self.xpath, self.prev_val, self.value)
 
 
 # ------------------------------------------------------------------------------
 class ChangeDeleted(Change):
-
     __slots__ = ("value",)
 
     def __init__(self, xpath: str, value: Any):
         super().__init__(xpath)
         self.value = value
 
     def __eq__(self, other: Any) -> bool:
@@ -173,15 +169,14 @@
 
     def __str__(self) -> str:
         return "%s: %r" % (self.xpath, self.value)
 
 
 # ------------------------------------------------------------------------------
 class ChangeMoved(Change):
-
     __slots__ = ("after",)
 
     def __init__(self, xpath: str, after: str):
         super().__init__(xpath)
         self.after = after
 
     def __eq__(self, other: Any) -> bool:
```

### Comparing `sysrepo-1.4.0/sysrepo/connection.py` & `sysrepo-1.5.0/sysrepo/connection.py`

 * *Files identical despite different names*

### Comparing `sysrepo-1.4.0/sysrepo/errors.py` & `sysrepo-1.5.0/sysrepo/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from _sysrepo import ffi, lib
 from .util import c2str
 
 
 # ------------------------------------------------------------------------------
 class SysrepoError(Exception):
-
     rc = None
     __slots__ = ("msg",)
 
     def __init__(self, msg: str):
         super().__init__()
         self.msg = msg
```

### Comparing `sysrepo-1.4.0/sysrepo/session.py` & `sysrepo-1.5.0/sysrepo/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .errors import (
     SysrepoInternalError,
     SysrepoNotFoundError,
     SysrepoUnsupportedError,
     check_call,
 )
 from .subscription import Subscription
-from .util import c2str, str2c
+from .util import c2str, is_async_func, str2c
 from .value import Value
 
 
 LOG = logging.getLogger(__name__)
 
 
 # ------------------------------------------------------------------------------
@@ -360,14 +360,126 @@
         check_call(
             lib.sr_module_change_subscribe,
             self.cdata,
             str2c(module),
             str2c(xpath),
             lib.srpy_module_change_cb,
             sub.handle,
+            priority,
+            flags,
+            sub_p,
+        )
+        sub.init(sub_p[0])
+
+        self.subscriptions.append(sub)
+
+    UnsafeModuleChangeCallbackType = Callable[["SysrepoSession", str, int, Any], None]
+    """
+    Callback to be called when the change in the datastore occurs. Provides implicit 
+    session object instead of list of changes. THE CALLBACK SHOULD NEVER KEEP A
+    REFERENCE ON THE IMPLICIT SESSION OBJECT TO AVOID USER-AFTER-FREE BUGS.
+
+    :arg session:
+        Implicit session (do not stop) with information about the changed data.
+    :arg event:
+        Type of the callback event that has occurred. Can be one of: "update", "change",
+        "done", "abort", "enabled".
+    :arg req_id:
+        Request ID unique for the specific module name. Connected events for one request
+        ("change" and "done" for example) have the same request ID.
+    :arg private_data:
+        Private context opaque to sysrepo used when subscribing.
+
+    When event is one of ("update", "change"), if the callback raises an exception, the
+    changes will be rejected and the error will be forwarded to the client that made the
+    change. If the exception is a subclass of `SysrepoError`, the traceback will not be
+    sent to the logging system. For consistency and to avoid confusion with unexpected
+    errors, the callback should raise explicit `SysrepoValidationFailedError` exceptions
+    to reject changes.
+    """
+
+    def subscribe_module_change_unsafe(
+        self,
+        module: str,
+        xpath: Optional[str],
+        callback: UnsafeModuleChangeCallbackType,
+        *,
+        priority: int = 0,
+        no_thread: bool = False,
+        passive: bool = False,
+        done_only: bool = False,
+        enabled: bool = False,
+        private_data: Any = None,
+        asyncio_register: bool = False,
+    ) -> None:
+        """
+        Subscribe for changes made in the specified module. Implicit session object
+        is returned to callback instead of list of changes. When callback returns to
+        Sysrepo, the session is freed, so we cannot keep a reference on it and
+        schedule async code to run later. For this reason, async callbacks are NOT
+        allowed here.
+
+        :arg module:
+            Name of the module of interest for change notifications.
+        :arg xpath:
+            Optional xpath further filtering the changes that will be handled
+            by this subscription.
+        :arg callback:
+            Callback to be called when the change in the datastore occurs.
+        :arg priority:
+            Specifies the order in which the callbacks (**within module**) will
+            be called.
+        :arg no_thread:
+            There will be no thread created for handling this subscription
+            meaning no event will be processed! Default to `True` if
+            asyncio_register is `True`.
+        :arg passive:
+            The subscriber is not the "owner" of the subscribed data tree, just
+            a passive watcher for changes.
+        :arg done_only:
+            The subscriber does not support verification of the changes and
+            wants to be notified only after the changes has been applied in the
+            datastore, without the possibility to deny them.
+        :arg enabled:
+            The subscriber wants to be notified about the current configuration
+            at the moment of subscribing.
+        :arg private_data:
+            Private context passed to the callback function, opaque to sysrepo.
+        :arg asyncio_register:
+            Add the created subscription event pipe into asyncio event loop
+            monitored read file descriptors. Implies `no_thread=True`.
+        """
+        if self.is_implicit:
+            raise SysrepoUnsupportedError("cannot subscribe with implicit sessions")
+        if is_async_func(callback):
+            raise SysrepoUnsupportedError(
+                "cannot use unsafe subscription with async callback"
+            )
+        _check_subscription_callback(callback, self.UnsafeModuleChangeCallbackType)
+
+        sub = Subscription(
+            callback,
+            private_data,
+            asyncio_register=asyncio_register,
+            unsafe=True,
+        )
+        sub_p = ffi.new("sr_subscription_ctx_t **")
+
+        if asyncio_register:
+            no_thread = True  # we manage our own event loop
+        flags = _subscribe_flags(
+            no_thread=no_thread, passive=passive, done_only=done_only, enabled=enabled
+        )
+        check_call(
+            lib.sr_module_change_subscribe,
+            self.cdata,
+            str2c(module),
+            str2c(xpath),
+            lib.srpy_module_change_cb,
+            sub.handle,
             priority,
             flags,
             sub_p,
         )
         sub.init(sub_p[0])
 
         self.subscriptions.append(sub)
```

### Comparing `sysrepo-1.4.0/sysrepo/subscription.py` & `sysrepo-1.5.0/sysrepo/subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         callback: Callable,
         private_data: Any = None,
         asyncio_register: bool = False,
         strict: bool = False,
         include_implicit_defaults: bool = True,
         include_deleted_values: bool = False,
         extra_info: bool = False,
+        unsafe: bool = False,
     ):
         """
         :arg callback:
             The python callback function or coroutine function used when subscribing.
         :arg private_data:
             Opaque data used when subscribing, will be passed to callback.
         :arg asyncio_register:
@@ -54,14 +55,16 @@
         :arg include_deleted_values:
             If True, include the complete deleted node values into Change objects passed
             to module change callbacks.
         :arg extra_info:
             When True, the given callback is called with extra keyword arguments
             containing extra information of the sysrepo session that gave origin to the
             event
+        :arg unsafe:
+            When True, the given callback returns implicit session.
         """
         if is_async_func(callback) and not asyncio_register:
             raise ValueError(
                 "%s is an async function, asyncio_register is mandatory" % callback
             )
         self.callback = callback
         self.private_data = private_data
@@ -74,14 +77,15 @@
             self.loop = asyncio.get_event_loop()
         else:
             self.loop = None
         self.tasks = {}
         self.cdata = None
         self.fd = -1
         self.handle = ffi.new_handle(self)
+        self.unsafe = unsafe
 
     def init(self, cdata) -> None:
         """
         Initialization of this object is not complete after calling __init__. The
         sr_subscription_ctx_t object is allocated by sysrepo when calling one of
         sr_*_subscribe functions and we need to pass self.handle to these functions so
         that this subscription can be forwarded to C callbacks.
@@ -176,14 +180,15 @@
     lib.SR_EV_NOTIF_REPLAY: "replay",
     lib.SR_EV_NOTIF_REPLAY_COMPLETE: "replay_complete",
     lib.SR_EV_NOTIF_TERMINATED: "terminated",
     lib.SR_EV_NOTIF_SUSPENDED: "suspended",
     lib.SR_EV_NOTIF_RESUMED: "resumed",
 }
 
+
 # ------------------------------------------------------------------------------
 @ffi.def_extern(name="srpy_module_change_cb")
 def module_change_callback(session, sub_id, module, xpath, event, req_id, priv):
     """
     Callback to be called on the event of changing datastore content of the specified
     module.
 
@@ -223,19 +228,28 @@
         module = c2str(module)
         xpath = c2str(xpath)
         root_xpath = ("/%s:*" % module) if xpath is None else xpath
         subscription = ffi.from_handle(priv)
         callback = subscription.callback
         private_data = subscription.private_data
         event_name = EVENT_NAMES[event]
+        if subscription.unsafe:
+            callback(session, event_name, req_id, private_data)
+            return lib.SR_ERR_OK
         if subscription.extra_info:
-            extra_info = {
-                "netconf_id": session.get_netconf_id(),
-                "user": session.get_user(),
-            }
+            try:
+                extra_info = {
+                    "netconf_id": session.get_netconf_id(),
+                    "user": session.get_user(),
+                }
+            except SysrepoError:
+                extra_info = {
+                    "netconf_id": -1,
+                    "user": "",
+                }
         else:
             extra_info = {}
 
         if is_async_func(callback):
             task_id = (event, req_id)
 
             if task_id not in subscription.tasks:
```

### Comparing `sysrepo-1.4.0/sysrepo/util.py` & `sysrepo-1.5.0/sysrepo/util.py`

 * *Files identical despite different names*

### Comparing `sysrepo-1.4.0/sysrepo/value.py` & `sysrepo-1.5.0/sysrepo/value.py`

 * *Files identical despite different names*

### Comparing `sysrepo-1.4.0/sysrepo.egg-info/PKG-INFO` & `sysrepo-1.5.0/sysrepo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrepo
-Version: 1.4.0
+Version: 1.5.0
 Summary: Sysrepo CFFI bindings
 Home-page: https://www.6wind.com/
 Author: Robin Jarry
 Author-email: robin.jarry@6wind.com
 License: BSD 3 clause
 Keywords: sysrepo,libyang,cffi
 Classifier: Development Status :: 4 - Beta
```

