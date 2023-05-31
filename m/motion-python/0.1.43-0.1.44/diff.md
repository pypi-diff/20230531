# Comparing `tmp/motion_python-0.1.43.tar.gz` & `tmp/motion_python-0.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.43.tar", max compression
+gzip compressed data, was "motion_python-0.1.44.tar", max compression
```

## Comparing `motion_python-0.1.43.tar` & `motion_python-0.1.44.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     2752 2023-05-23 16:50:57.023610 motion_python-0.1.43/README.md
--rw-r--r--   0        0        0      187 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/__init__.py
--rw-r--r--   0        0        0     1817 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/cli.py
--rw-r--r--   0        0        0    20577 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/component.py
--rw-r--r--   0        0        0     5733 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/execute.py
--rw-r--r--   0        0        0     6823 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/route.py
--rw-r--r--   0        0        0     3734 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/utils.py
--rw-r--r--   0        0        0     1657 2023-05-23 16:51:19.371545 motion_python-0.1.43/pyproject.toml
--rw-r--r--   0        0        0     3875 1970-01-01 00:00:00.000000 motion_python-0.1.43/PKG-INFO
+-rw-r--r--   0        0        0     3319 2023-05-31 21:42:14.375259 motion_python-0.1.44/README.md
+-rw-r--r--   0        0        0      202 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/cli.py
+-rw-r--r--   0        0        0    23617 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/component.py
+-rw-r--r--   0        0        0    12098 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/execute.py
+-rw-r--r--   0        0        0     4392 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/fit_task.py
+-rw-r--r--   0        0        0     7489 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      595 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/route.py
+-rw-r--r--   0        0        0     6283 2023-05-31 21:42:14.379260 motion_python-0.1.44/motion/utils.py
+-rw-r--r--   0        0        0     1775 2023-05-31 21:42:39.411378 motion_python-0.1.44/pyproject.toml
+-rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 motion_python-0.1.44/PKG-INFO
```

### Comparing `motion_python-0.1.43/README.md` & `motion_python-0.1.44/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -30,7 +30,19 @@
 Motion is developed and maintained by researchers at the [UC Berkeley EPIC Lab](https://epic.berkeley.edu) who specialize in data management for ML pipelines.
 
 ## Getting Started
 
 Check out the [docs](https://dm4ml.github.io/motion/) for more information.
 
 Motion is currently in alpha. We are actively working on improving the documentation and adding more features. If you are interested in using Motion and would like dedicated support from one of our team members, please reach out to us at [shreyashankar@berkeley.edu](mailto:shreyashankar@berkeley.edu).
+
+## Testing and Development
+
+You can run `make install` to install an editable source of Motion. We use `poetry` to manage dependencies.
+
+To run tests, we use `pytest` and a local Redis cache. You should run Redis on port 6381 before you run `make tests`. To run Redis with Docker, either run the `docker-compose.yml` file in this repo (i.e., `docker-compose up`) or run the following command in your terminal:
+
+```bash
+docker run -p 6381:6379 --name motion-backend-testing redis/redis-stack-server:latest
+```
+
+Then when you run `make tests`, your tests should pass.
```

### Comparing `motion_python-0.1.43/motion/cli.py` & `motion_python-0.1.44/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.43/motion/component.py` & `motion_python-0.1.44/motion/component.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import inspect
 from typing import Any, Callable, Dict, List, Optional, get_type_hints
 
 from pydantic import BaseModel
 
 from motion.instance import ComponentInstance
 from motion.route import Route
-from motion.utils import CustomDict, validate_args
+from motion.utils import CustomDict, random_passphrase, validate_args
 
 
 class Component:
     """Component class for creating Motion components.
     Here are some examples:
 
     === "Basic"
@@ -29,15 +29,15 @@
 
         @AdderComponent.fit("add")
         def add(state, values, infer_results):
             return {"value": state["value"] + sum(values)}
 
         if __name__ == "__main__":
             c = AdderComponent() # Create instance of AdderComponent
-            c.run(add=1, wait_for_fit=True) # Will return 1, blocking until fit
+            c.run(add=1, force_fit=True) # Will return 1, blocking until fit
             # is done. Resulting state is {"value": 1}
             c.run(add=2) # Will return 3, not waiting for fit operation.
             # Resulting state will eventually be {"value": 3}
         ```
 
     === "Multiple Dataflows"
         ```python
@@ -63,17 +63,17 @@
 
         @Calculator.fit("subtract")
         def decrement(state, values, infer_results):
             return {"value": state["value"] - sum(values)}
 
         if __name__ == "__main__":
             c = Calculator()
-            c.run(add=1, wait_for_fit=True) # Will return 1, blocking until fit
+            c.run(add=1, force_fit=True) # Will return 1, blocking until fit
             # is done. Resulting state is {"value": 1}
-            c.run(subtract=1, wait_for_fit=True) # Will return 0, blocking
+            c.run(subtract=1, force_fit=True) # Will return 0, blocking
             # until fit is done. Resulting state is {"value": 0}
         ```
 
     === "Batch Size > 1"
 
         ```python
         from motion import Component
@@ -146,14 +146,16 @@
         self._name = name
         self._params = CustomDict(name, "params", params)
 
         # Set up routes
         self._infer_routes: Dict[str, Route] = {}
         self._fit_routes: Dict[str, List[Route]] = {}
         self._init_state_func: Optional[Callable] = None
+        self._save_state_func: Optional[Callable] = None
+        self._load_state_func: Optional[Callable] = None
 
     @property
     def name(self) -> str:
         """Name of the component.
 
         Example Usage:
         ```python
@@ -228,25 +230,77 @@
 
         @MyComponent.init_state
         def setUp():
             return {"value": 0}
         ```
 
         Args:
-            func (Callable): Function without any arguments.
+            func (Callable): Function that initializes a state. Must return
+                a dictionary.
 
         Returns:
             Callable: Decorated init_state function.
         """
-        # Assert that init function has no arguments
-        if inspect.signature(func).parameters:
-            raise ValueError("init_state function should have no arguments")
         self._init_state_func = func
         return func
 
+    def save_state(self, func: Callable) -> Callable:
+        """Decorator for the save_state function. This function
+        saves the state of the component to be accessible in
+        future component instances of the same name.
+
+        Usage:
+        ```python
+        from motion import Component
+
+        MyComponent = Component("MyComponent")
+
+        @c.save_state
+        def save(state):
+            # state might have other unpicklable keys, like a DB connection
+            return {"fit_count": state["fit_count"]}
+        ```
+
+        Args:
+            func (Callable): Function that returns a cloudpickleable object.
+
+        Returns:
+            Callable: Decorated save_state function.
+        """
+        self._save_state_func = func
+        return func
+
+    def load_state(self, func: Callable) -> Callable:
+        """Decorator for the load_state function. This function
+        loads the state of the component from the unpickled state.
+
+        Usage:
+        ```python
+        from motion import Component
+
+        MyComponent = Component("MyComponent")
+
+        @c.load_state
+        def load(state):
+            conn = sqlite3.connect(":memory:")
+            cursor = conn.cursor()
+            return {"cursor": cursor, "fit_count": state["fit_count"]}
+        ```
+
+        Args:
+            func (Callable): Function that consumes a cloudpickleable object.
+                Should return a dictionary representing the state of the
+                component instance.
+
+        Returns:
+            Callable: Decorated load_state function.
+        """
+        self._load_state_func = func
+        return func
+
     def infer(self, key: str) -> Callable:
         """Decorator for any infer dataflow through the component. Takes
         in a string that represents the input keyword for the infer dataflow.
 
         2 arguments required for an infer operation:
             * `state`: The current state of the component, which is a
                 dictionary with string keys and any type values.
@@ -277,24 +331,26 @@
             return state["value"] + value
 
         @MyComponent.infer("multiply")
         def multiply(state, value):
             return state["value"] * value
 
         c = MyComponent()
-        c.run(add=1, wait_for_fit=True) # Returns 1
+        c.run(add=1, force_fit=True) # Returns 1
         c.run(multiply=2) # Returns 2
         ```
 
         Args:
             key (str): Keyword for the infer dataflow.
 
         Returns:
             Callable: Decorated infer function.
         """
+        if "::" in key:
+            raise ValueError(f"Dataflow key {key} should not have a double colon (::)")
 
         def decorator(func: Callable) -> Any:
             type_hint = get_type_hints(func).get("value", None)
             if not validate_args(inspect.signature(func).parameters, "infer"):
                 raise ValueError(
                     f"Infer function {func.__name__} should have 2 arguments "
                     + "`state` and `value`"
@@ -366,15 +422,15 @@
         def multiply(state, values, infer_results):
             product = 1
             for value in values:
                 product *= value
             return state["value"] * product
 
         c = MyComponent()
-        c.run(add=1, wait_for_fit=True) # Returns 1
+        c.run(add=1, force_fit=True) # Returns 1
         c.run(multiply=2) # Returns 2, fit not executed yet
         c.run(multiply=3) # Returns 3, fit will execute; state["value"] = 6
         # Some time later...
         c.run(multiply=4) # Returns 24
         ```
 
         Args:
@@ -383,14 +439,21 @@
             batch_size (int, optional):
                 Number of values to wait for before
                 calling the fit function. Defaults to 1.
 
         Returns:
             Callable: Decorated fit function.
         """
+        frame = inspect.currentframe().f_back  # type: ignore
+        fname = frame.f_code.co_name  # type: ignore
+        if fname != "<module>":
+            raise ValueError(
+                f"Component {self.name} fit method must be defined in a module "
+                + f"context. It's currently initialized from function {fname}."
+            )
 
         def decorator(func: Callable) -> Any:
             if not validate_args(inspect.signature(func).parameters, "fit"):
                 raise ValueError(
                     f"Fit method {func.__name__} should have 3 arguments: "
                     + "`state`, `values`, and `infer_results`."
                 )
@@ -403,60 +466,84 @@
             )  # type: ignore
             return func
 
         return decorator
 
     def __call__(
         self,
-        cleanup: bool = False,
+        name: str = "",
+        init_state_params: Dict[str, Any] = {},
         logging_level: str = "WARNING",
     ) -> ComponentInstance:
         """Creates and returns a new instance of a Motion component.
         See `ComponentInstance` docs for more info.
 
         Usage:
         ```python
         from motion import Component
 
         MyComponent = Component("MyComponent")
 
         @MyComponent.init_state
-        def setUp():
-            return {"value": 0}
+        def setUp(starting_val):
+            return {"value": starting_val}
 
         # Define infer and fit operations
         @MyComponent.infer("key1")
         def ...
 
         @MyComponent.fit("key1)
         def ...
 
-        c_instance = MyComponent() # Creates instance of MyComponent
+        c_instance = MyComponent(init_state_params={"starting_val": 3})
+        # Creates instance of MyComponent
         c_instance.run(..)
         ```
 
         Args:
-            cleanup (bool, optional):
-                Whether to process the remainder of fit events after the user
-                shuts down the program. Defaults to False.
+            name (str, optional):
+                Name of the component instance. Defaults to "".
+            init_state_params (Dict[str, Any], optional):
+                Parameters to pass into the init_state function. Defaults to {}.
             logging_level (str, optional):
                 Logging level for the Motion logger. Uses the logging library.
                 Defaults to "WARNING".
         Returns:
             ComponentInstance: Component instance to run dataflows with.
         """
+        if not name:
+            name = random_passphrase()
 
-        return ComponentInstance(
-            component_name=self.name,
-            init_state_func=self._init_state_func,
-            infer_routes=self._infer_routes,
-            fit_routes=self._fit_routes,
-            cleanup=cleanup,
-            logging_level=logging_level,
-        )
+        if "__" in name:
+            raise ValueError(
+                f"Instance name {name} cannot contain '__'. Strip the component"
+                + "name from your instance name."
+            )
+
+        instance_name = f"{self.name}__{name}"
+
+        try:
+            ci = ComponentInstance(
+                component_name=self.name,
+                instance_name=instance_name,
+                init_state_func=self._init_state_func,
+                init_state_params=init_state_params,
+                save_state_func=self._save_state_func,
+                load_state_func=self._load_state_func,
+                infer_routes=self._infer_routes,
+                fit_routes=self._fit_routes,
+                logging_level=logging_level,
+            )
+        except RuntimeError:
+            raise RuntimeError(
+                "Error creating component instance. Make sure the entry point "
+                + "of your program is protected, using `if __name__ == '__main__':`"
+            )
+
+        return ci
 
     def get_graph(self, x_offset_step: int = 600) -> Dict[str, Any]:
         """
         Gets the graph of infer and fit ops for this component.
         """
 
         graph: Dict[str, Dict[str, Any]] = {}
```

### Comparing `motion_python-0.1.43/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.44/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.43/motion/route.py` & `motion_python-0.1.44/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.43/pyproject.toml` & `motion_python-0.1.44/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.43"
+version = "0.1.44"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -20,14 +20,17 @@
 uvicorn = "^0.21.1"
 httpx = "^0.23.3"
 python-multipart = "^0.0.6"
 pydantic = "^1.10.7"
 urllib3 = "^1.26.15"
 flask = "^2.2.3"
 rich = "^13.3.4"
+cloudpickle = "^2.2.1"
+redis = "^4.5.5"
+psutil = "^5.9.5"
 
 [tool.poetry.group.dev.dependencies]
 poetry-types = "^0.3.5"
 pytest = "^7.2.2"
 mypy = "^1.1.1"
 coverage = {extras = ["toml"], version = "^7.2.3"}
 pre-commit = "^3.2.1"
@@ -39,20 +42,22 @@
 mkdocstrings = {version="^0.20.0", extras = ["python"] }
 pytkdocs = "^0.16.1"
 linkchecker = "^10.2.1"
 ruff = "^0.0.261"
 maturin = "^0.14.17"
 mike = "^1.1.2"
 scikit-learn = "^1.2.2"
+types-redis = "^4.5.5.2"
 
 [tool.poetry.scripts]
 motion = "motion.cli:motioncli"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
+addopts = "--basetemp=/tmp/pytest"
 
 [tool.mypy]
 files = "motion"
 mypy_path = "motion"
 warn_return_any = true
 warn_unused_configs = true
 disallow_untyped_defs = true
```

### Comparing `motion_python-0.1.43/PKG-INFO` & `motion_python-0.1.44/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.43
+Version: 0.1.44
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: croniter (>=1.3.8,<2.0.0)
 Requires-Dist: duckdb (>=0.7.1,<0.8.0)
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: flask (>=2.2.3,<3.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
+Requires-Dist: redis (>=4.5.5,<5.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Description-Content-Type: text/markdown
 
 # Motion
@@ -60,7 +63,19 @@
 
 ## Getting Started
 
 Check out the [docs](https://dm4ml.github.io/motion/) for more information.
 
 Motion is currently in alpha. We are actively working on improving the documentation and adding more features. If you are interested in using Motion and would like dedicated support from one of our team members, please reach out to us at [shreyashankar@berkeley.edu](mailto:shreyashankar@berkeley.edu).
 
+## Testing and Development
+
+You can run `make install` to install an editable source of Motion. We use `poetry` to manage dependencies.
+
+To run tests, we use `pytest` and a local Redis cache. You should run Redis on port 6381 before you run `make tests`. To run Redis with Docker, either run the `docker-compose.yml` file in this repo (i.e., `docker-compose up`) or run the following command in your terminal:
+
+```bash
+docker run -p 6381:6379 --name motion-backend-testing redis/redis-stack-server:latest
+```
+
+Then when you run `make tests`, your tests should pass.
+
```

