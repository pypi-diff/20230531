# Comparing `tmp/slurm-parallel-0.1.5.tar.gz` & `tmp/slurm-parallel-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurm-parallel-0.1.5.tar", last modified: Wed May 10 06:17:54 2023, max compression
+gzip compressed data, was "slurm-parallel-0.1.7.tar", last modified: Wed May 31 21:48:26 2023, max compression
```

## Comparing `slurm-parallel-0.1.5.tar` & `slurm-parallel-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-10 06:17:54.606019 slurm-parallel-0.1.5/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1065 2023-05-01 18:25:25.000000 slurm-parallel-0.1.5/LICENSE
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      112 2023-05-09 20:43:09.000000 slurm-parallel-0.1.5/MANIFEST.in
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-10 06:17:54.593040 slurm-parallel-0.1.5/PKG-INFO
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       83 2023-05-01 18:25:25.000000 slurm-parallel-0.1.5/README.md
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      714 2023-05-10 06:06:43.000000 slurm-parallel-0.1.5/pyproject.toml
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       38 2023-05-10 06:17:54.612728 slurm-parallel-0.1.5/setup.cfg
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-10 06:17:51.694422 slurm-parallel-0.1.5/src/
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-10 06:17:54.082582 slurm-parallel-0.1.5/src/slurm_parallel/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 20:47:47.000000 slurm-parallel-0.1.5/src/slurm_parallel/__init__.py
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       61 2023-05-02 01:39:05.000000 slurm-parallel-0.1.5/src/slurm_parallel/config.toml
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      918 2023-05-09 07:36:00.000000 slurm-parallel-0.1.5/src/slurm_parallel/run.py
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       28 2023-05-09 04:55:29.000000 slurm-parallel-0.1.5/src/slurm_parallel/run.sh
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     9659 2023-05-10 06:13:55.000000 slurm-parallel-0.1.5/src/slurm_parallel/slurm.py
--rwxr-xr-x   0 hc3190   (413786699) domain users (413600513)       46 2023-05-09 20:13:12.000000 slurm-parallel-0.1.5/src/slurm_parallel/summarize.sh
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     2099 2023-05-08 17:39:51.000000 slurm-parallel-0.1.5/src/slurm_parallel/utils.py
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-10 06:17:54.439805 slurm-parallel-0.1.5/src/slurm_parallel.egg-info/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-10 06:17:51.000000 slurm-parallel-0.1.5/src/slurm_parallel.egg-info/PKG-INFO
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      468 2023-05-10 06:17:51.000000 slurm-parallel-0.1.5/src/slurm_parallel.egg-info/SOURCES.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)        1 2023-05-10 06:17:51.000000 slurm-parallel-0.1.5/src/slurm_parallel.egg-info/dependency_links.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       20 2023-05-10 06:17:51.000000 slurm-parallel-0.1.5/src/slurm_parallel.egg-info/requires.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-10 06:17:51.000000 slurm-parallel-0.1.5/src/slurm_parallel.egg-info/top_level.txt
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-10 06:17:54.520734 slurm-parallel-0.1.5/test/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1414 2023-05-10 06:09:23.000000 slurm-parallel-0.1.5/test/test.py
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-31 21:48:26.858444 slurm-parallel-0.1.7/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1065 2023-05-01 18:25:25.000000 slurm-parallel-0.1.7/LICENSE
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      112 2023-05-09 20:43:09.000000 slurm-parallel-0.1.7/MANIFEST.in
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-31 21:48:26.821153 slurm-parallel-0.1.7/PKG-INFO
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       83 2023-05-01 18:25:25.000000 slurm-parallel-0.1.7/README.md
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      714 2023-05-31 21:45:47.000000 slurm-parallel-0.1.7/pyproject.toml
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       38 2023-05-31 21:48:26.877651 slurm-parallel-0.1.7/setup.cfg
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-31 21:48:23.757691 slurm-parallel-0.1.7/src/
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-31 21:48:25.688122 slurm-parallel-0.1.7/src/slurm_parallel/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 20:47:47.000000 slurm-parallel-0.1.7/src/slurm_parallel/__init__.py
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       61 2023-05-02 01:39:05.000000 slurm-parallel-0.1.7/src/slurm_parallel/config.toml
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      918 2023-05-09 07:36:00.000000 slurm-parallel-0.1.7/src/slurm_parallel/run.py
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       28 2023-05-09 04:55:29.000000 slurm-parallel-0.1.7/src/slurm_parallel/run.sh
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     9883 2023-05-31 21:15:25.000000 slurm-parallel-0.1.7/src/slurm_parallel/slurm.py
+-rwxr-xr-x   0 hc3190   (413786699) domain users (413600513)       46 2023-05-09 20:13:12.000000 slurm-parallel-0.1.7/src/slurm_parallel/summarize.sh
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     2099 2023-05-08 17:39:51.000000 slurm-parallel-0.1.7/src/slurm_parallel/utils.py
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-31 21:48:26.513601 slurm-parallel-0.1.7/src/slurm_parallel.egg-info/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-31 21:48:22.000000 slurm-parallel-0.1.7/src/slurm_parallel.egg-info/PKG-INFO
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      468 2023-05-31 21:48:23.000000 slurm-parallel-0.1.7/src/slurm_parallel.egg-info/SOURCES.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)        1 2023-05-31 21:48:23.000000 slurm-parallel-0.1.7/src/slurm_parallel.egg-info/dependency_links.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       20 2023-05-31 21:48:23.000000 slurm-parallel-0.1.7/src/slurm_parallel.egg-info/requires.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-31 21:48:23.000000 slurm-parallel-0.1.7/src/slurm_parallel.egg-info/top_level.txt
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-31 21:48:26.691647 slurm-parallel-0.1.7/test/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1581 2023-05-31 21:43:07.000000 slurm-parallel-0.1.7/test/test.py
```

### Comparing `slurm-parallel-0.1.5/LICENSE` & `slurm-parallel-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `slurm-parallel-0.1.5/PKG-INFO` & `slurm-parallel-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-parallel
-Version: 0.1.5
+Version: 0.1.7
 Summary: Easy parallelization of python functions on SLURM using job arrays.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slurm-parallel-0.1.5/pyproject.toml` & `slurm-parallel-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"] # editable install using setuptool available since v64.0.0
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slurm-parallel"
-version = "0.1.5"
+version = "0.1.7"
 description = "Easy parallelization of python functions on SLURM using job arrays."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "Ho Yin Chau"},
 ]
```

### Comparing `slurm-parallel-0.1.5/src/slurm_parallel/run.py` & `slurm-parallel-0.1.7/src/slurm_parallel/run.py`

 * *Files identical despite different names*

### Comparing `slurm-parallel-0.1.5/src/slurm_parallel/slurm.py` & `slurm-parallel-0.1.7/src/slurm_parallel/slurm.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 __all__ = ['parallelize']
 
 class StringTemplate(Template):
     delimiter = '%'
     idpattern = "(?a-i:[sF])" # ASCII-only, don't ignore case
 
 @lib.functools.parametrized
-def parallelize(func, database=None, table=None, columns=None, max_n_tasks=None, tmp_dir=None, out_dir=None, out_file=None, time_per_config=30, wait=True, progress_dt=5, **default_kwargs):
+def parallelize(func, database=None, table=None, columns=None, max_n_tasks=None, max_n_simul_tasks=None, tmp_dir=None, out_dir=None, out_file=None, time_per_config=30, wait=True, progress_dt=5, **default_kwargs):
     for k in default_kwargs:
         if k not in allowed_args:
             raise KeyError(f"parallelize got an unexpected argument '{k}'")
             
     funcname = func.__name__
     filename = inspect.getsourcefile(func)
     
@@ -94,15 +94,15 @@
                     else:
                         result = {column: v for v in result}
 
                 database[table].append(config | result)
 
                 logger.info(f"Saved output of config {i}.")
     
-    def remote(configs, logging_kwargs=None, max_n_tasks=max_n_tasks, tmp_dir=tmp_dir, out_dir=out_dir, out_file=out_file, time_per_config=time_per_config, wait=wait, progress_dt=progress_dt, **kwargs):
+    def remote(configs, logging_kwargs=None, max_n_tasks=max_n_tasks, max_n_simul_tasks=max_n_simul_tasks, tmp_dir=tmp_dir, out_dir=out_dir, out_file=out_file, time_per_config=time_per_config, wait=wait, progress_dt=progress_dt, **kwargs):
         for k in kwargs:
             if k not in allowed_args:
                 raise KeyError(f"remote got an unexpected argument '{k}'")
                 
         if not isinstance(configs, list):
             raise TypeError(f"configs must be a list, but {type(configs)=}.")
             
@@ -146,19 +146,23 @@
         out_dir = pathlib.Path(datetime.datetime.now().strftime(out_dir))
         out_dir.mkdir(parents=True, exist_ok=True)
         out_file = StringTemplate(out_file).safe_substitute(s=pathlib.Path(filename).stem, F=funcname)
         
         n_tasks = min(n_configs, max_n_tasks)
         time_per_task = int(math.ceil(n_configs / n_tasks)) * time_per_config
         
+        array = f'0-{n_tasks-1}'
+        if max_n_simul_tasks is not None:
+            array = f'{array}%{max_n_simul_tasks}'
+        
         run_kwargs = {
             'c': 2,
             'mem_per_cpu': '2gb',
             'time': lib.datetime.strftime(time_per_task, '%d-%H:%M:%S'),
-            'array': f'0-{n_tasks-1}',
+            'array': array,
             'output': out_dir / out_file,
             'parsable': not wait,
             'wait': wait,
             'job_name': f'{pathlib.Path(filename).stem}_{funcname}',
         } | default_kwargs | kwargs
         run_options = utils.to_cmd_options(**run_kwargs)
         
@@ -174,15 +178,15 @@
                 json.dump(configs, f)
                 
             logger.debug(f"Saved configs to tmp file {tmp_filename}.")
             
             args = ["sbatch", *run_options, run_script, run_py_script, filename, funcname, tmp_filename, *logging_options]
             logger.debug(f"Invoking subprocess with arguments {args}")
             
-            success = False
+            run_PID, success = None, False
             try:
                 with subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, bufsize=1, text=True) as p:
                     for line in p.stdout:
                         match = re.search('Submitted batch job ([0-9]{6})', line)
                         if match is not None:
                             run_PID = match.group(1)
                             break
@@ -211,15 +215,15 @@
             except Exception as err:
                 raise err
                 
             else:
                 success = True
                 
             finally:
-                if not success:
+                if not success and run_PID is not None:
                     subprocess.run(['scancel', run_PID], check=True)
                     logger.info(f"Ensured batch job {run_PID} for {pathlib.Path(filename).stem}.{funcname} is cancelled.")
     
     func.run_task = run_task
     func.remote = remote
     
     return func
```

### Comparing `slurm-parallel-0.1.5/src/slurm_parallel/utils.py` & `slurm-parallel-0.1.7/src/slurm_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `slurm-parallel-0.1.5/src/slurm_parallel.egg-info/PKG-INFO` & `slurm-parallel-0.1.7/src/slurm_parallel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-parallel
-Version: 0.1.5
+Version: 0.1.7
 Summary: Easy parallelization of python functions on SLURM using job arrays.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slurm-parallel-0.1.5/test/test.py` & `slurm-parallel-0.1.7/test/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 import sqlalchemy as sa
 import dfdb
 import hyclib as lib
 
 import slurm_parallel as sp
 
-db = dfdb.Database(database='test/data/test.db')
+db = dfdb.Database(database='/home/hc3190/slurm-parallel/test/data/test.db', connect_args={"timeout": 30})
 logger = logging.getLogger()
 
-@sp.parallelize(mem_per_cpu='1gb', c=1, partition='ctn')
+@sp.parallelize(mem_per_cpu='1mb', c=1, partition='ctn')
 def print_results():
     df = db['results'].fetch()
     print(df)
 
 @sp.parallelize(database=db, table='results', columns='result', mem_per_cpu='1gb', c=1, partition='ctn')
 def func(a, b):
-    # time.sleep(20)
+    time.sleep(20)
     # if a == 5:
     #     raise RuntimeError()
     return a + b
 
 def main():
     lib.logging.basic_config()
     logger.setLevel('DEBUG')
@@ -34,20 +34,21 @@
         sa.Column('a', sa.Integer()),
         sa.Column('b', sa.Integer()),
         sa.Column('result', sa.Integer()),
         sa.Column('created', sa.DateTime(), server_default=sa.func.now()),
     )
     
     configs = [
-        # {'a': 1, 'b': 2},
-        # {'a': 3, 'b': 4},
-        # {'a': 5, 'b': 6},
-        # {'a': 7, 'b': 8},
+        {'a': 1, 'b': 2},
+        {'a': 3, 'b': 4},
+        {'a': 5, 'b': 6},
+        {'a': 7, 'b': 8},
     ]
     # job = func.remote(configs, wait=False, max_n_tasks=3, logging_kwargs=dict(level='DEBUG'))
     # print_results.remote([{}], wait=False, dependency=f'afterany:{job}')
     
-    func.remote(configs, max_n_tasks=3, logging_kwargs=dict(level='DEBUG'))
+    # func.remote(configs, max_n_tasks=3, logging_kwargs=dict(level='DEBUG'))
+    func.remote(configs, max_n_tasks=3, max_n_simul_tasks=2, p='issa', A='issa', logging_kwargs=dict(level='DEBUG'))
     print_results.remote([{}])
 
 if __name__ == '__main__':
     main()
```

