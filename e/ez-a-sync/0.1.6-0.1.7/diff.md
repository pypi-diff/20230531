# Comparing `tmp/ez-a-sync-0.1.6.tar.gz` & `tmp/ez-a-sync-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.1.6.tar", last modified: Fri Mar 24 19:26:46 2023, max compression
+gzip compressed data, was "ez-a-sync-0.1.7.tar", last modified: Wed May 31 17:50:23 2023, max compression
```

## Comparing `ez-a-sync-0.1.6.tar` & `ez-a-sync-0.1.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 19:26:46.109623 ez-a-sync-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 19:26:46.093623 ez-a-sync-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 19:26:46.097623 ez-a-sync-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-03-24 19:26:46.109623 ez-a-sync-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 19:26:46.101623 ez-a-sync-0.1.6/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4462 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     1584 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     2855 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6316 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 19:26:46.105623 ez-a-sync-0.1.6/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 19:26:46.105623 ez-a-sync-0.1.6/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/modifiers/semaphores.py
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 19:26:46.105623 ez-a-sync-0.1.6/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-03-24 19:26:45.000000 ez-a-sync-0.1.6/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-03-24 19:26:45.000000 ez-a-sync-0.1.6/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-24 19:26:45.000000 ez-a-sync-0.1.6/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-03-24 19:26:45.000000 ez-a-sync-0.1.6/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-03-24 19:26:45.000000 ez-a-sync-0.1.6/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-24 19:26:46.109623 ez-a-sync-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 19:26:46.109623 ez-a-sync-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-03-24 19:26:27.000000 ez-a-sync-0.1.6/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 17:50:23.873684 ez-a-sync-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 17:50:23.869684 ez-a-sync-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 17:50:23.869684 ez-a-sync-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-05-31 17:50:23.873684 ez-a-sync-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 17:50:23.873684 ez-a-sync-0.1.7/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4462 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2855 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6316 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 17:50:23.873684 ez-a-sync-0.1.7/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 17:50:23.873684 ez-a-sync-0.1.7/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/modifiers/semaphores.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 17:50:23.873684 ez-a-sync-0.1.7/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-05-31 17:50:23.000000 ez-a-sync-0.1.7/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-05-31 17:50:23.000000 ez-a-sync-0.1.7/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 17:50:23.000000 ez-a-sync-0.1.7/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-31 17:50:23.000000 ez-a-sync-0.1.7/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-31 17:50:23.000000 ez-a-sync-0.1.7/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-31 17:50:23.873684 ez-a-sync-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 17:50:23.873684 ez-a-sync-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-05-31 17:50:12.000000 ez-a-sync-0.1.7/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.1.6/.github/workflows/codeql.yaml` & `ez-a-sync-0.1.7/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/.github/workflows/mypy.yaml` & `ez-a-sync-0.1.7/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/.github/workflows/pytest.yaml` & `ez-a-sync-0.1.7/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/.github/workflows/release.yaml` & `ez-a-sync-0.1.7/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/LICENSE.txt` & `ez-a-sync-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/__init__.py` & `ez-a-sync-0.1.7/a_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/_bound.py` & `ez-a-sync-0.1.7/a_sync/_bound.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/_flags.py` & `ez-a-sync-0.1.7/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/_helpers.py` & `ez-a-sync-0.1.7/a_sync/_helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 from async_property.cached import \
     AsyncCachedPropertyDescriptor  # type: ignore [import]
 
 from a_sync import _flags
 from a_sync._typing import *
 
 
+def get_event_loop() -> asyncio.BaseEventLoop:
+    try:
+        return asyncio.get_event_loop()
+    except RuntimeError:
+        asyncio.set_event_loop(asyncio.new_event_loop())
+        return asyncio.get_event_loop()
+    
 def _validate_wrapped_fn(fn: Callable) -> None:
     """Ensures 'fn' is an appropriate function for wrapping with a_sync."""
     if isinstance(fn, (AsyncPropertyDescriptor, AsyncCachedPropertyDescriptor)):
         return # These are always valid
     if not callable(fn):
         raise TypeError(f'Input is not callable. Unable to decorate {fn}')
     fn_args = getfullargspec(fn)[0]
@@ -23,18 +30,18 @@
         if flag in fn_args:
             raise RuntimeError(f"{fn} must not have any arguments with the following names: {_flags.VIABLE_FLAGS}")
 
 running_event_loop_msg = f"You may want to make this an async function by setting one of the following kwargs: {_flags.VIABLE_FLAGS}"
 
 def _await(awaitable: Awaitable[T]) -> T:
     try:
-        return asyncio.get_event_loop().run_until_complete(awaitable)
+        return get_event_loop().run_until_complete(awaitable)
     except RuntimeError as e:
         if str(e) == "This event loop is already running":
             raise RuntimeError(str(e), running_event_loop_msg)
         raise
 
 def _asyncify(func: SyncFn[P, T], executor: Executor) -> CoroFn[P, T]:
     @functools.wraps(func)
     async def _asyncify_wrap(*args: P.args, **kwargs: P.kwargs) -> T:
-        return await asyncio.get_event_loop().run_in_executor(executor, func, *args, **kwargs)
+        return await get_event_loop().run_in_executor(executor, func, *args, **kwargs)
     return _asyncify_wrap
```

### Comparing `ez-a-sync-0.1.6/a_sync/_kwargs.py` & `ez-a-sync-0.1.7/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/_meta.py` & `ez-a-sync-0.1.7/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/_typing.py` & `ez-a-sync-0.1.7/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/abstract.py` & `ez-a-sync-0.1.7/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/base.py` & `ez-a-sync-0.1.7/a_sync/base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/config.py` & `ez-a-sync-0.1.7/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/decorator.py` & `ez-a-sync-0.1.7/a_sync/decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/exceptions.py` & `ez-a-sync-0.1.7/a_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/modified.py` & `ez-a-sync-0.1.7/a_sync/modified.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/modifiers/__init__.py` & `ez-a-sync-0.1.7/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.1.7/a_sync/modifiers/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.1.7/a_sync/modifiers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/modifiers/limiter.py` & `ez-a-sync-0.1.7/a_sync/modifiers/limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/modifiers/manager.py` & `ez-a-sync-0.1.7/a_sync/modifiers/manager.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.1.7/a_sync/modifiers/semaphores.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/a_sync/property.py` & `ez-a-sync-0.1.7/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.1.7/ez_a_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/setup.py` & `ez-a-sync-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/tests/fixtures.py` & `ez-a-sync-0.1.7/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/tests/test_base.py` & `ez-a-sync-0.1.7/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/tests/test_cache.py` & `ez-a-sync-0.1.7/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/tests/test_decorator.py` & `ez-a-sync-0.1.7/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/tests/test_meta.py` & `ez-a-sync-0.1.7/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.6/tests/test_semaphore.py` & `ez-a-sync-0.1.7/tests/test_semaphore.py`

 * *Files identical despite different names*

