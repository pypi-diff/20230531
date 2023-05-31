# Comparing `tmp/cmrseq-0.21.tar.gz` & `tmp/cmrseq-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmrseq-0.21.tar", last modified: Wed May 24 08:16:49 2023, max compression
+gzip compressed data, was "cmrseq-0.22.tar", last modified: Wed May 31 14:47:29 2023, max compression
```

## Comparing `cmrseq-0.21.tar` & `cmrseq-0.22.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:16:49.940080 cmrseq-0.21/
--rw-rw-rw-   0 root         (0) root         (0)    35076 2023-04-12 07:04:17.000000 cmrseq-0.21/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3033 2023-05-24 08:16:49.940080 cmrseq-0.21/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2541 2023-04-12 07:04:17.000000 cmrseq-0.21/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:16:49.928075 cmrseq-0.21/cmrseq/
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-24 08:16:49.000000 cmrseq-0.21/cmrseq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:16:49.928075 cmrseq-0.21/cmrseq/contrib/
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-04-12 07:04:17.000000 cmrseq-0.21/cmrseq/contrib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10174 2023-04-12 07:04:17.000000 cmrseq-0.21/cmrseq/contrib/sequences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:16:49.932077 cmrseq-0.21/cmrseq/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 08:16:36.000000 cmrseq-0.21/cmrseq/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    34883 2023-05-24 07:28:55.000000 cmrseq-0.21/cmrseq/core/_sequence.py
--rw-rw-rw-   0 root         (0) root         (0)     7495 2023-05-24 07:59:28.000000 cmrseq-0.21/cmrseq/core/_system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:16:49.932077 cmrseq-0.21/cmrseq/core/bausteine/
--rw-rw-rw-   0 root         (0) root         (0)      678 2023-04-12 11:43:48.000000 cmrseq-0.21/cmrseq/core/bausteine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7561 2023-05-23 15:09:08.000000 cmrseq-0.21/cmrseq/core/bausteine/_adc.py
--rw-rw-rw-   0 root         (0) root         (0)     2558 2023-05-23 15:09:08.000000 cmrseq-0.21/cmrseq/core/bausteine/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1050 2023-05-23 15:09:08.000000 cmrseq-0.21/cmrseq/core/bausteine/_delay.py
--rw-rw-rw-   0 root         (0) root         (0)    24837 2023-05-23 15:09:08.000000 cmrseq-0.21/cmrseq/core/bausteine/_gradients.py
--rw-rw-rw-   0 root         (0) root         (0)    18259 2023-05-24 07:28:55.000000 cmrseq-0.21/cmrseq/core/bausteine/_rf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:16:49.936078 cmrseq-0.21/cmrseq/io/
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-12 07:04:17.000000 cmrseq-0.21/cmrseq/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6074 2023-04-12 07:04:17.000000 cmrseq-0.21/cmrseq/io/_json.py
--rw-rw-rw-   0 root         (0) root         (0)    25748 2023-05-23 15:09:08.000000 cmrseq-0.21/cmrseq/io/_phillips_load.py
--rw-rw-rw-   0 root         (0) root         (0)    53656 2023-05-20 14:39:52.000000 cmrseq-0.21/cmrseq/io/_pulseq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:16:49.936078 cmrseq-0.21/cmrseq/parametric_definitions/
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-12 07:04:17.000000 cmrseq-0.21/cmrseq/parametric_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13840 2023-05-23 15:09:08.000000 cmrseq-0.21/cmrseq/parametric_definitions/diffusion.py
--rw-rw-rw-   0 root         (0) root         (0)    14602 2023-05-23 15:09:08.000000 cmrseq-0.21/cmrseq/parametric_definitions/excitation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:16:49.936078 cmrseq-0.21/cmrseq/parametric_definitions/readout/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-12 07:04:17.000000 cmrseq-0.21/cmrseq/parametric_definitions/readout/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16647 2023-05-23 15:09:08.000000 cmrseq-0.21/cmrseq/parametric_definitions/readout/_cartesian_single_lines.py
--rw-rw-rw-   0 root         (0) root         (0)    24190 2023-05-24 07:28:55.000000 cmrseq-0.21/cmrseq/parametric_definitions/readout/_epi.py
--rw-rw-rw-   0 root         (0) root         (0)     8143 2023-04-12 07:11:24.000000 cmrseq-0.21/cmrseq/parametric_definitions/readout/_radial.py
--rw-rw-rw-   0 root         (0) root         (0)    10626 2023-04-12 07:04:17.000000 cmrseq-0.21/cmrseq/parametric_definitions/readout/_spiral.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:16:49.940080 cmrseq-0.21/cmrseq/parametric_definitions/sequences/
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-12 07:04:17.000000 cmrseq-0.21/cmrseq/parametric_definitions/sequences/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13141 2023-04-12 07:04:17.000000 cmrseq-0.21/cmrseq/parametric_definitions/sequences/_gradient_echo.py
--rw-rw-rw-   0 root         (0) root         (0)     8295 2023-05-24 07:28:55.000000 cmrseq-0.21/cmrseq/parametric_definitions/sequences/_spin_echo.py
--rw-rw-rw-   0 root         (0) root         (0)    18600 2023-05-23 15:09:08.000000 cmrseq-0.21/cmrseq/parametric_definitions/sequences/_ssfp.py
--rw-rw-rw-   0 root         (0) root         (0)    27016 2023-04-12 07:04:17.000000 cmrseq-0.21/cmrseq/parametric_definitions/velocity.py
--rw-rw-rw-   0 root         (0) root         (0)    16097 2023-05-23 15:09:08.000000 cmrseq-0.21/cmrseq/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)    11966 2023-04-12 07:04:17.000000 cmrseq-0.21/cmrseq/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:16:49.928075 cmrseq-0.21/cmrseq.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3033 2023-05-24 08:16:49.000000 cmrseq-0.21/cmrseq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1282 2023-05-24 08:16:49.000000 cmrseq-0.21/cmrseq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 08:16:49.000000 cmrseq-0.21/cmrseq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-05-24 08:16:49.000000 cmrseq-0.21/cmrseq.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-24 08:16:49.000000 cmrseq-0.21/cmrseq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 08:16:49.940080 cmrseq-0.21/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1635 2023-04-12 07:04:18.000000 cmrseq-0.21/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:47:29.839788 cmrseq-0.22/
+-rw-rw-rw-   0 root         (0) root         (0)    35076 2023-04-12 07:04:17.000000 cmrseq-0.22/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-05-31 14:47:29.839788 cmrseq-0.22/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-04-12 07:04:17.000000 cmrseq-0.22/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:47:29.831784 cmrseq-0.22/cmrseq/
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-31 14:47:29.000000 cmrseq-0.22/cmrseq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:47:29.835786 cmrseq-0.22/cmrseq/contrib/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-04-12 07:04:17.000000 cmrseq-0.22/cmrseq/contrib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10174 2023-04-12 07:04:17.000000 cmrseq-0.22/cmrseq/contrib/sequences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:47:29.835786 cmrseq-0.22/cmrseq/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 14:47:17.000000 cmrseq-0.22/cmrseq/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36794 2023-05-31 13:18:21.000000 cmrseq-0.22/cmrseq/core/_sequence.py
+-rw-rw-rw-   0 root         (0) root         (0)     7495 2023-05-24 07:59:28.000000 cmrseq-0.22/cmrseq/core/_system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:47:29.835786 cmrseq-0.22/cmrseq/core/bausteine/
+-rw-rw-rw-   0 root         (0) root         (0)      678 2023-04-12 11:43:48.000000 cmrseq-0.22/cmrseq/core/bausteine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8204 2023-05-30 13:22:20.000000 cmrseq-0.22/cmrseq/core/bausteine/_adc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2023-05-30 13:22:20.000000 cmrseq-0.22/cmrseq/core/bausteine/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-05-23 15:09:08.000000 cmrseq-0.22/cmrseq/core/bausteine/_delay.py
+-rw-rw-rw-   0 root         (0) root         (0)    27710 2023-05-31 14:40:20.000000 cmrseq-0.22/cmrseq/core/bausteine/_gradients.py
+-rw-rw-rw-   0 root         (0) root         (0)    25494 2023-05-31 13:18:21.000000 cmrseq-0.22/cmrseq/core/bausteine/_rf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:47:29.835786 cmrseq-0.22/cmrseq/io/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-12 07:04:17.000000 cmrseq-0.22/cmrseq/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6074 2023-04-12 07:04:17.000000 cmrseq-0.22/cmrseq/io/_json.py
+-rw-rw-rw-   0 root         (0) root         (0)    25748 2023-05-23 15:09:08.000000 cmrseq-0.22/cmrseq/io/_phillips_load.py
+-rw-rw-rw-   0 root         (0) root         (0)    53656 2023-05-20 14:39:52.000000 cmrseq-0.22/cmrseq/io/_pulseq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:47:29.839788 cmrseq-0.22/cmrseq/parametric_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-12 07:04:17.000000 cmrseq-0.22/cmrseq/parametric_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13840 2023-05-30 11:44:20.000000 cmrseq-0.22/cmrseq/parametric_definitions/diffusion.py
+-rw-rw-rw-   0 root         (0) root         (0)    14602 2023-05-23 15:09:08.000000 cmrseq-0.22/cmrseq/parametric_definitions/excitation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:47:29.839788 cmrseq-0.22/cmrseq/parametric_definitions/readout/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-12 07:04:17.000000 cmrseq-0.22/cmrseq/parametric_definitions/readout/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16647 2023-05-23 15:09:08.000000 cmrseq-0.22/cmrseq/parametric_definitions/readout/_cartesian_single_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)    24190 2023-05-24 07:28:55.000000 cmrseq-0.22/cmrseq/parametric_definitions/readout/_epi.py
+-rw-rw-rw-   0 root         (0) root         (0)     8143 2023-04-12 07:11:24.000000 cmrseq-0.22/cmrseq/parametric_definitions/readout/_radial.py
+-rw-rw-rw-   0 root         (0) root         (0)    10626 2023-04-12 07:04:17.000000 cmrseq-0.22/cmrseq/parametric_definitions/readout/_spiral.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:47:29.839788 cmrseq-0.22/cmrseq/parametric_definitions/sequences/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-12 07:04:17.000000 cmrseq-0.22/cmrseq/parametric_definitions/sequences/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13141 2023-04-12 07:04:17.000000 cmrseq-0.22/cmrseq/parametric_definitions/sequences/_gradient_echo.py
+-rw-rw-rw-   0 root         (0) root         (0)     8295 2023-05-24 07:28:55.000000 cmrseq-0.22/cmrseq/parametric_definitions/sequences/_spin_echo.py
+-rw-rw-rw-   0 root         (0) root         (0)    18600 2023-05-23 15:09:08.000000 cmrseq-0.22/cmrseq/parametric_definitions/sequences/_ssfp.py
+-rw-rw-rw-   0 root         (0) root         (0)    27016 2023-04-12 07:04:17.000000 cmrseq-0.22/cmrseq/parametric_definitions/velocity.py
+-rw-rw-rw-   0 root         (0) root         (0)    16098 2023-05-31 13:18:21.000000 cmrseq-0.22/cmrseq/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)    11966 2023-04-12 07:04:17.000000 cmrseq-0.22/cmrseq/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:47:29.835786 cmrseq-0.22/cmrseq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-05-31 14:47:29.000000 cmrseq-0.22/cmrseq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-31 14:47:29.000000 cmrseq-0.22/cmrseq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 14:47:29.000000 cmrseq-0.22/cmrseq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-05-31 14:47:29.000000 cmrseq-0.22/cmrseq.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-31 14:47:29.000000 cmrseq-0.22/cmrseq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 14:47:29.839788 cmrseq-0.22/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1635 2023-04-12 07:04:18.000000 cmrseq-0.22/setup.py
```

### Comparing `cmrseq-0.21/LICENSE` & `cmrseq-0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/PKG-INFO` & `cmrseq-0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmrseq
-Version: 0.21
+Version: 0.22
 Summary: UNKNOWN
 Home-page: https://gitlab.ethz.ch/jweine/cmrseq
 Author: Jonathan Weine, Charles McGrath
 Author-email: weine@biomed.ee.ethz.ch, mcgrath@biomed.ee.ethz.ch
 License: UNKNOWN
 Project-URL: Documentation, https://people.ee.ethz.ch/~jweine/cmrseq/latest/index.html
 Project-URL: Source, https://gitlab.ethz.ch/jweine/cmrseq
```

### Comparing `cmrseq-0.21/README.rst` & `cmrseq-0.22/README.rst`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/contrib/sequences.py` & `cmrseq-0.22/cmrseq/contrib/sequences.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/core/_sequence.py` & `cmrseq-0.22/cmrseq/core/_sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     There are multiple ways to query single or even multiple blocks at once from the sequence
     object. To get a complete list of unique block-names use the property :code:`seq.blocks`.
 
     *Access by name*:
     1. Indexing by unique name: :code:`seq["trapezoidal_0"]`
     2. Get all blocks by partial string match: :code:`seq.get_block(partial_string_match=...)`
     3. Get all blocks by matching regular expression on unique names: :code:`seq.get_block(regular_expression=...)`
+    4. Get a sequence object containing copies of all blocks matched as in (2. & 3.) :code:`seq.partial_copy(...)`
 
     *Assuming temporal order of start*
     1. Indexing by integer: :code:`seq[0]`
     2. Indexing by slice: :code:`seq[0:5]`
     3. Indexing by tuple of integers: :code:`seq[(0, 2, 5)]`
     4. Iterating over sequence: :code:`[block for block in seq]`
     5. Iterating over sequence with block-names :code:`{name: block for (name, block) in seq.items()}`
@@ -79,28 +80,38 @@
     Gradient moments of specified order can be integrated using the function :code:`seq.calculate_moment`.
 
     To get a representation of the kspace-trajectory as well as timing and position of sampling
     events defined by contained ADC blocks can be obtained by the :code:`seq.calculate_kspace` function.
 
     :param building_blocks: List of building Blocks
     :param system_specs: Instance of SystemSpec
+    :param snap_to_raster:
+    :param copy: 
     """
 
     #: System specification object
     _system_specs: SystemSpec
     #:
     _blocks: List[SequenceBaseBlock]
     #:
     _block_lookup: Dict[str, SequenceBaseBlock]
 
-    def __init__(self, building_blocks: List[SequenceBaseBlock], system_specs: SystemSpec):
+    def __init__(self, building_blocks: List[SequenceBaseBlock], system_specs: SystemSpec,
+                 snap_to_raster: bool = False, copy: bool = False):
+                     
         self._system_specs = system_specs
-        self._blocks = building_blocks
-        self.validate()
+        if copy:
+            self._blocks = [b.copy() for b in building_blocks]
+        else:
+            self._blocks = building_blocks
 
+        if snap_to_raster:
+            [b.snap_to_raster(self._system_specs) for b in self._blocks]
+            
+        self.validate()
         self._block_lookup = {}
         for block in self._blocks:
             self._add_unique_block_name(block)
 
 
     def __add__(self, other: 'Sequence') -> 'Sequence':
         """ If both system specifications match, returns a new sequence containing deep copies
@@ -417,16 +428,34 @@
         """Returns a tuple containing the names of all blocks contained in the sequence object,
         where temporal ordering is assumed"""
         names_and_times = self._create_sorted_block_list(reversed=False)
         names = [n for n, t in names_and_times]
         return names
 
     def copy(self):
+        """ Returns deepcopy of the sequence object"""
         return deepcopy(self)
 
+    def partial_copy(self, partial_string_match: Union[str, Iterable[str]] = None,
+                     regular_expression: Union[str, Iterable[str]] = None, **kwargs) -> 'Sequence':
+        """Returns a cmrseq.Sequence object containing deepcopies of all blocks matched
+        either with partial-string-match or regular expressions specified as keyword argument.
+        
+        :param partial_string_match: str or iterable of strings that specify partial string matches.
+                    All blocks partially matching at least one are returned.
+        :param regular_expression: str or iterable of strings containing regular expressions that
+                            are matched against the block-names. All blocks, matching at least one
+                            of the given expressions are returned.
+        :return: Sequence object
+        """
+        matched_blocks = self.get_block(block_name=None, partial_string_match=partial_string_match,
+                                        regular_expression=regular_expression)
+        block_copies = [b.copy() for b in matched_blocks]
+        return Sequence(building_blocks=block_copies, system_specs=self._system_specs, **kwargs)
+                         
     # pylint: disable=R0914, C0103
     def gradients_to_grid(self) -> Tuple[np.ndarray, np.ndarray]:
         """ Grids gradient definitions of all blocks contained in the sequence, on a joint time grid
         from the minimal to maximal value in single time-points definitions with a step-length
         defined in system_specs.grad_raster_time.
         If gradients occur at the same time on the same channel, they are added.
 
@@ -438,21 +467,21 @@
         if not gradients:
             return None, None
 
         time_points = [g[0].m_as("ms") for g in gradients]
         wave_forms = [g[1].m_as("mT/m") for g in gradients]
 
         dt = self._system_specs.grad_raster_time.m_as("ms")
-        t_grid = np.arange(0, self.end_time.m_as("ms") + dt, dt)
+        t_grid = np.arange(self.start_time.m_as("ms"), self.end_time.m_as("ms") + dt, dt)
         wf_grid = np.zeros((3, t_grid.shape[0]))
 
         for t, wf, bidx in zip(time_points, wave_forms, range(len(self._blocks))):
             t = np.array(t)
-            tidx = np.around(t / dt)
-            if not np.allclose(t / dt, tidx, rtol=1e-6):
+            tidx = np.around((t - self.start_time.m_as("ms")) / dt)
+            if not np.allclose((t - self.start_time.m_as("ms")) / dt, tidx, rtol=1e-6):
                 warn(f"Gradient definition of block {bidx} is not on gradient raster")
             start, end = int(tidx[0]), int(tidx[-1])
             interpolated_wfx = np.interp(t_grid[start:end], t, wf[0])
             interpolated_wfy = np.interp(t_grid[start:end], t, wf[1])
             interpolated_wfz = np.interp(t_grid[start:end], t, wf[2])
             wf_grid[:, start:end] += np.stack([interpolated_wfx,
                                                interpolated_wfy,
@@ -474,21 +503,21 @@
         if not rf:
             return None, None
 
         time_points = [r[0].m_as("ms") for r in rf]
         wave_forms = [r[1].m_as("mT") for r in rf]
 
         dt = self._system_specs.rf_raster_time.m_as("ms")
-        t_grid = np.arange(0, self.end_time.m_as("ms") + dt, dt)
+        t_grid = np.arange(self.start_time.m_as("ms"), self.end_time.m_as("ms") + dt, dt)
         rf_grid = np.zeros((t_grid.shape[0]), dtype=np.complex64)
 
         for t, complex_alpha, bidx in zip(time_points, wave_forms, range(len(rf))):
             t = np.array(t)
-            tidx = np.around(t / dt)
-            if not np.allclose(t / dt, tidx, rtol=1e-6):
+            tidx = np.around((t - self.start_time.m_as("ms")) / dt)
+            if not np.allclose((t - self.start_time.m_as("ms")) / dt, tidx, atol=1e-6):
                 warn(f"RF definition of block {bidx} is not on RF raster")
             start, end = int(tidx[0]), int(tidx[-1])
             rf_grid[start:end] += np.interp(t_grid[start:end], t, complex_alpha)
         return t_grid, rf_grid
 
     # pylint: disable=R0914, C0103
     def adc_to_grid(self, force_raster: bool = False) \
```

### Comparing `cmrseq-0.21/cmrseq/core/_system.py` & `cmrseq-0.22/cmrseq/core/_system.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/core/bausteine/__init__.py` & `cmrseq-0.22/cmrseq/core/bausteine/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/core/bausteine/_adc.py` & `cmrseq-0.22/cmrseq/core/bausteine/_adc.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,46 +11,46 @@
 from cmrseq.core._system import SystemSpec
 
 
 class ADC(SequenceBaseBlock):
     """ ADC-specific extension to the SequenceBaseBlock, serves as base class for all
     ADC implementations"""
     #: Quantity[ms] defining sampling event times
-    adc_timing: Quantity = None
-
+    adc_timing: Quantity
     #: Quantity[ms] Time defining the center of the adc-events
-    adc_center: Quantity = None
-
+    adc_center: Quantity
     #: Quantity[rad]
     phase_offset: Quantity
-
     #: Quantity[Hz]
     frequency_offset: Quantity
 
     def __init__(self, system_specs: SystemSpec, name: str,
+                 adc_timing: Quantity, adc_center: Quantity,
                  frequency_offset: Quantity, phase_offset: Quantity):
         super().__init__(system_specs, name)
-        self.frequency_offset = frequency_offset.to("Hz")
-        self.phase_offset = phase_offset.to("rad")
+        self.adc_timing : Quantity = adc_timing.to("ms")
+        self.adc_center : Quantity = adc_center.to("ms")
+        self.frequency_offset : Quantity = frequency_offset.to("Hz")
+        self.phase_offset : Quantity = phase_offset.to("rad")
 
     @property
-    def adc_phase(self):
+    def adc_phase(self) -> Quantity:
         """ Returns the phase at each adc-event in radians"""
         t = self.adc_timing
         t_zero_ref = t - t[0]
         phase_per_time = (self.phase_offset.m_as("rad") +
                           2 * np.pi * self.frequency_offset.m_as("kHz") * t_zero_ref.m_as("ms"))
         return phase_per_time
 
     @property
-    def tmin(self):
+    def tmin(self) -> Quantity:
         return self.adc_timing[0]
 
     @property
-    def tmax(self):
+    def tmax(self) -> Quantity:
         return self.adc_timing[-1]
 
     def validate(self, system_specs: SystemSpec):
         return
 
     def shift(self, time_shift: Quantity) -> None:
         """Adds the time-shift to all adc definition points and the adc-center"""
@@ -60,20 +60,24 @@
 
     def flip(self, time_flip: Quantity = None):
         if time_flip is None:
             time_flip = self.tmax
         self.adc_timing = np.flip(time_flip.to("ms") - self.adc_timing, axis=0)
         self.adc_center = np.flip(time_flip.to("ms") - self.adc_center, axis=0)
 
-    def snap_to_raster(self, system_specs: SystemSpec):
+    def snap_to_raster(self, system_specs: SystemSpec) -> None:
         pass
 
 class SymmetricADC(ADC):
     """ ADC object with instantaneous encoding events at k-space positions """
-
+    #: 
+    _n_samples: int
+    #: 
+    _dwell: Quantity
+    
     def __init__(self, system_specs: SystemSpec,
                  num_samples: int,
                  dwell: Quantity = None,
                  duration: Quantity = None,
                  delay: Quantity = None,
                  frequency_offset: Quantity = Quantity(0., "Hz"),
                  phase_offset: Quantity = Quantity(0., "rad"),
@@ -91,35 +95,41 @@
         :param duration: Quantity[time] Total sampling duration corresponding to (1 / \Delta kx).
                           Usually is the same as flat_duration of accompanying trapezoidal gradient.
         :param delay: Quantity[time] Leading time without sampling events
         :param frequency_offset:
         :param phase_offset:
         :return:
         """
-        super().__init__(system_specs=system_specs, name=name,
-                         frequency_offset=frequency_offset.to("Hz"),
-                         phase_offset=phase_offset.to("rad"))
 
         if (dwell is None and duration is None) or not (dwell is None or duration is None):
             raise ValueError("Either dwell or duration must be defined")
 
         if duration:
             dwell = duration / num_samples
 
         delay = Quantity(0, "ms") if delay is None else delay
         if num_samples % 2 == 1:
-            self.adc_timing = (np.arange(0, num_samples) + 0.5) * dwell + delay
+            adc_timing = (np.arange(0, num_samples) + 0.5) * dwell + delay
         else:
-            self.adc_timing = (np.arange(0, num_samples)) * dwell + delay
+            adc_timing = (np.arange(0, num_samples)) * dwell + delay
+
+        frequency_offset=frequency_offset.to("Hz")
+        phase_offset=phase_offset.to("rad")
+     
         self._n_samples = int(num_samples)
         self._dwell = dwell
-        self.adc_center = self.adc_timing[int(np.floor(num_samples / 2))]
+        adc_center = adc_timing[int(np.floor(num_samples / 2))]
+        
+        super().__init__(system_specs=system_specs, name=name, 
+                         adc_timing=adc_timing, adc_center=adc_center,
+                         phase_offset=phase_offset, 
+                         frequency_offset=frequency_offset)              
 
     @property
-    def tmin(self):
+    def tmin(self) -> Quantity:
         """ Returns the time of the first sampling event. Behavior varies for odd/even number of
         samples:
 
             - **odd**: Returns the time of the first sampling event minus half a dwell time on
                        gradient raster time.
             - **even**: Returns the time of the first sampling event
 
@@ -129,15 +139,15 @@
         if self._n_samples % 2 != 0:  # odd number of samples
             start_ = first_sample_time - self._dwell / 2
         else:
             start_ = first_sample_time
         return start_
 
     @property
-    def tmax(self):
+    def tmax(self) -> Quantity:
         """Returns the time of the last sampling event. Behavior varies for odd/even number of
         samples:
 
             - **odd**: Returns the time of the last sampling event plus half a dwell time.
             - **even**: Returns the time of the last sampling event plus a a full dwell time.
 
         In both cases this corresponds to the end of the plateau of a readout gradient
@@ -163,32 +173,35 @@
         :param system_specs:
         :param duration:
         :param delay:
         :param freq_offset:
         :param phase_offset:
         :param name:
         """
-        super().__init__(system_specs, name, frequency_offset, phase_offset)
-
+        
         rounded_raster_time = decimal.Decimal(str(float(np.round(system_specs.adc_raster_time.m_as("ms"), decimals=6))))
         delay_dec = decimal.Decimal(str(float(np.round(delay.m_as("ms"), decimals=6))))
         duration_dec = decimal.Decimal(str(float(np.round(duration.m_as("ms"), decimals=6))))
         if not (delay_dec % rounded_raster_time == decimal.Decimal("0.0")):
             raise ValueError(f"Specified delay {delay:1.6} is not on adc_raster_time")
         if not (duration_dec % rounded_raster_time == decimal.Decimal("0.0")):
             raise ValueError(f"Specified duration {duration:1.6} is not on adc_raster_time")
         n_steps = math.ceil(duration / system_specs.adc_raster_time)
         time_grid = np.arange(0, n_steps+1, 1) * system_specs.adc_raster_time.m_as("ms")
-        self.adc_timing = Quantity(time_grid, "ms") + delay
-        self.adc_center = system_specs.time_to_raster(duration / 2, "adc") + delay
+        
+        super().__init__(system_specs=system_specs, name=name,
+                         adc_timing=Quantity(time_grid, "ms") + delay, 
+                         adc_center=system_specs.time_to_raster(duration / 2, "adc") + delay,
+                         frequency_offset=frequency_offset,
+                         phase_offset=phase_offset)             
 
     @property
-    def tmin(self):
+    def tmin(self) -> Quantity:
         return self.adc_timing[0]
 
     @property
-    def tmax(self):
+    def tmax(self) -> Quantity:
         return self.adc_timing[-1]
```

### Comparing `cmrseq-0.21/cmrseq/core/bausteine/_base.py` & `cmrseq-0.22/cmrseq/core/bausteine/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,27 @@
 from pint import Quantity
 
 from cmrseq.core._system import SystemSpec
 
 
 # pylint: disable=C0103
 class SequenceBaseBlock(SimpleNamespace):
-    """ Base class for all building blocks. All general operations performed on all sequence
-    blocks must be compatible with this class. When implementing new building blocks, inherit
-    from this class """
+    """ Base class for all building blocks, defining the abstract interface for generic
+    interaction with blocks.
+
+    All subclases must implent the abstract methods, and all general methods on 
+    blocks must only access the implemented methods when no sub-class type check 
+    is performed.
+
+    Furthermore, all subclasses must call the base-class constructor.
+    
+    :param system_specs:
+    :param name: 
+    :param snap_to_raster: 
+    """
     # Field that should be used to describe the semantic meaning of the block object
     name: str
 
     def __init__(self, system_specs: SystemSpec, name: str, snap_to_raster: bool = False):
         """ Must be called as last line of subclass.__init__"""
         super().__init__(name=name)
         if snap_to_raster:
@@ -32,27 +42,27 @@
 
     def __deepcopy__(self, memodict={}) -> "SequenceBaseBlock":
         ret = SequenceBaseBlock(system_specs=None, name=self.name)
         ret.__class__ = self.__class__  # pylint: disable=W0201
         ret.__dict__.update(deepcopy(self.__dict__))
         return ret
 
-    def copy(self):
+    def copy(self) -> 'SequenceBaseBlock':
         """Returns a deep copied building block object"""
         return self.__deepcopy__()
 
     @abstractmethod
-    def snap_to_raster(self, system_specs: SystemSpec):
+    def snap_to_raster(self, system_specs: SystemSpec) -> None:
         pass
 
     def _clean(self):
         pass
 
     @abstractmethod
-    def validate(self, system_specs: SystemSpec):
+    def validate(self, system_specs: SystemSpec) -> None:
         """Should raise a ValueError if subclass logic is not met by definition
         :param system_specs:
         :return:
         """
         return
 
     @property
```

### Comparing `cmrseq-0.21/cmrseq/core/bausteine/_delay.py` & `cmrseq-0.22/cmrseq/core/bausteine/_delay.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/core/bausteine/_gradients.py` & `cmrseq-0.22/cmrseq/core/bausteine/_gradients.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,66 @@
 from pint import Quantity
 
 from cmrseq.core.bausteine._base import SequenceBaseBlock
 from cmrseq.core._system import SystemSpec
 
 
 class Gradient(SequenceBaseBlock):
-    """
+    """Generic implementation of a MRI-sequence building block containing gradient waveforms on
+    3 channels.
+
+    This class implements all functionality that should be provided by all types of gradients. 
+    Special cases of gradients are meant to be inherited from this class.
+
+    Some of the implemented functionalities and their underlying assumptions are described below.
 
+    **Addition**:
+    Gradient instances can be added using the :code:`+` operator, where breakpoints are combined and 
+    linear interpolation of the waveform per channel inbetween the breakpoints is assumed.
+    The result of adding two :code:`Gradient` objects, is a tuple containing the time and waveform 
+    definition as shown in the example code below.
+
+    .. Dropdown:: Example addition
+        :animate: fade-in-slide-down
+        :icon: graph
+        :color: secondary
+        
+        .. code::
+
+            trap1 = cmrseq.bausteine.TrapezoidalGradient.from_dur_amp(system_specs, orientation=np.array([1., 0., 0.]),
+                                                          duration=Quantity(1, "ms"), amplitude=Quantity(10, "mT/m"), name="trap_1")
+
+            trap2 = cmrseq.bausteine.TrapezoidalGradient.from_dur_amp(system_specs, orientation=np.array([1., 0., 0.]),
+                                                                      duration=Quantity(1, "ms"), amplitude=Quantity(10, "mT/m"), 
+                                                                      delay=Quantity(0.2, "ms"), name="trap_2")
+            combined_t, combined_wf = trap1 + trap2
+            combined_gradient = cmrseq.bausteine.ArbitraryGradient(system_specs, combined_t, combined_wf, name="combined_trap")
+            seq = cmrseq.Sequence([combined_gradient], system_specs)
+
+    **Split**:
+    This functionality mainly is required to adhere to the pulseq file format, which requires
+    the gradient definition to be sub-divided into blocks, such that the each gradient channel
+    has at max one gradient block. The :code:`split` function allows to separate the gradient 
+    definition at an arbitrary time.
+
+
+    **Validation**:
+    Gradient objects are validated against the system-specifications with regard to:
+    1. Maximal gradient strength
+    2. Maximal gradient slew-rate
+    3. Adherence to the gradient-raster time
+    
+    If the raster time does not match, one option is to apply the snap to raster method, 
+    which rounds all temporal definitions to the closest raster point. In most cases this
+    includes unwanted side-effects e.g changing moments. If all time-points are offset 
+    from the grid by the same amount this methods should not have unwanted side effects.    
     """
     #: Tuple containing defining points of gradient waveforms as np.array (wrapped as Quantity)
     #: with shape (time: (t, ), waveform: (3, t)). Between points, linear interpolation is assumed
-    gradients: Tuple[Quantity, Quantity] = None
+    gradients: Tuple[Quantity, Quantity]
 
     def __add__(self, other) -> (Quantity, Quantity):
         """ Add to gradient definition and always returns a Tuple (time_points[n], waveforms[3, n])
 
         :param other:
         :return:
         """
@@ -147,28 +193,28 @@
                      np.diff(self.gradients[0].m_as("ms"), axis=0)[np.newaxis])
         grad_slew_in_specs = np.all(np.around(grad_slew, decimals=6)
                                     <= system_specs.max_slew.m_as("mT/m/ms"))
         tgridded = self.gradients[0].m_as("ms") / system_specs.grad_raster_time.m_as("ms")
         grad_on_grid = np.allclose(tgridded, np.around(tgridded), rtol=1e-6)
         if not all([max_grad_in_specs, grad_slew_in_specs, grad_on_grid]):
             raise ValueError(f"Gradient definition of {self.name} invalid:\n"
-                             f"\t- max grad: {max_grad_in_specs}\n"
-                             f"\t- max slew: {grad_slew_in_specs}\n"
+                             f"\t- max grad: {max_grad_in_specs} [{np.max(self.gradients[1].m_as('mT/m'))} {'<' if max_grad_in_specs else '<'} {system_specs.max_grad.m_as('mT/m')}]\n"
+                             f"\t- max slew: {grad_slew_in_specs} [{np.max(grad_slew)} {'<' if grad_slew_in_specs else '<'} {system_specs.max_slew.m_as('mT/m/ms')}] \n"
                              f"\t- definition on grid: {grad_on_grid}")
 
     def snap_to_raster(self, system_specs: SystemSpec):
         warn("When calling snap_to_raster the waveform points are simply rounded to their nearest"
              f"neighbour if the difference is below the relative tolerance. Therefore this in"
              f" not guaranteed to be precise anymore")
         time_ndt = np.around(self.gradients[0].m_as("ms") /
                              system_specs.grad_raster_time.m_as("ms"), decimals=0)
         time_ndt = time_ndt * system_specs.grad_raster_time.to("ms")
         self.gradients = (time_ndt.to("ms"), self.gradients[1].to("mT/m"))
 
-    def shift(self, time_shift: Quantity) -> None:
+    def shift(self, time_shift: Quantity):
         """Adds the time-shift to all gradient definition points"""
         self.gradients = (self.gradients[0] + time_shift.to("ms"), self.gradients[1])
 
     def flip(self, time_flip: Quantity = None):
         """Time reverses block by flipping about a given time point. If no
         time is specified, the center of this gradient block is choosen."""
         if time_flip is None:
```

### Comparing `cmrseq-0.21/cmrseq/core/bausteine/_rf.py` & `cmrseq-0.22/cmrseq/core/bausteine/_rf.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,41 +8,69 @@
 import numpy as np
 
 from cmrseq.core.bausteine._base import SequenceBaseBlock
 from cmrseq.core._system import SystemSpec
 
 
 class RFPulse(SequenceBaseBlock):
-    """ RF-specific extension to the SequenceBaseBlock, serves as base class for all
-    RF implementations"""
+    """Generic MRI-sequence radio-frequency building block 
+    
+    This class implements all functionality that should be provided by all subtypes of 
+    RF-pulses. 
+
+    The waveform (assuming linear interpolation between the points) and the time-points have to
+    be specified on construction of the RF object, where the waveform is assumed to be real-valued.
+    It also is assumed, that all RF-pulse subclasses correctly calculate and provide the following
+    quantities:
+
+    1. Pulse bandwidth
+    2. Frequency offset 
+    3. Phase offset
+
+    The phase offset and frequency offset attributes are used to compute the complex rf-waveform
+    representation using the `RFPulse.rf` - property.
+
+    :param system_specs: 
+    :param name:
+    :param time: (# points) time-points defining the waveform duration
+    :param rf_waveform: (#points) rf-amplitude
+    :param phase_offset: 
+    :param frequency_offset:
+    :param rf_events:
+    :param snap_to_raster:
+    """
     #: Tuple containing defining points of RF-waveforms as np.array (wrapped as Quantity)
     #: with shape (time: (t, ), waveform: (3, t)). Between points, linear interpolation is assumed
-    _rf: Tuple[Quantity, Quantity] = None
-
+    _rf: Tuple[Quantity, Quantity]
     #: Tuple containing rf events (time, flip_angle)
-    rf_events: Tuple[Quantity, Quantity] = None
-
+    rf_events: Tuple[Quantity, Quantity]
     #: RF pulse bandwidth in kilo Hertz. Used to calculate gradient strength
     bandwidth: Quantity
-
     #: RF phase offset in radians. This is used phase shift the complex rf amplitude in self.rf
     phase_offset: Quantity
-
     #: RF frequency offset in Hertz. This is used to modulate the complex rf amplitude in self.rf
     frequency_offset: Quantity
 
-    def __init__(self, system_specs: SystemSpec, name: str, frequency_offset: Quantity,
-                 phase_offset: Quantity, bandwidth: Quantity, snap_to_raster: bool):
+    def __init__(self, system_specs: SystemSpec, name: str,
+                 time: Quantity, rf_waveform: Quantity,
+                 frequency_offset: Quantity, phase_offset: Quantity, 
+                 bandwidth: Quantity,
+                 rf_events: Tuple[Quantity, Quantity],
+                 snap_to_raster: bool = False):
+
+        self._rf = (time.to("ms"), rf_waveform.to("uT"))
+        self.rf_events = (rf_events[0].to("ms"), rf_events[1].to("degree"))
+
         self.phase_offset = phase_offset.to("rad")
         self.frequency_offset = frequency_offset.to("Hz")
         self.bandwidth = bandwidth.to("kHz")
         super().__init__(system_specs, name, snap_to_raster)
 
     @property
-    def tmin(self):
+    def tmin(self) -> Quantity:
         return self._rf[0][0]
 
     @property
     def tmax(self) -> Quantity:
         return self._rf[0][-1]
 
     def validate(self, system_specs: SystemSpec):
@@ -56,35 +84,40 @@
             raise ValueError(f"RF definition invalid:\n"
                              f"\t - definition on grid: {ongrid}\n")
 
         if np.max(np.abs(wf)) > system_specs.rf_peak_power:
             raise ValueError(f"RF definition invalid:\n"
                              f"\t - peak power exceeds system limits: {np.max(np.abs(wf))}\n")
 
+        if not np.allclose([wf[0].m_as("uT"), wf[-1].m_as("uT")],
+                           Quantity(0, "uT").m, atol=1e-3):
+            start, end = [np.round(wf[i].m_as('uT'), decimals=3) for i in (0, -1)]
+            raise ValueError(f"RF definition invalid:\n",
+                             f"\t - start/end of waveform != 0: {start}/{end}\n")
+
+
     @property
-    def rf(self):
+    def rf(self) -> (Quantity, Quantity):
         """ Returns the complex RF-amplitude shifted/modulated by the phase/frequency offsets """
         t, amplitude = self._rf
         t_zero_ref = t - t[0]
-        if amplitude.m_as("uT").dtype in [np.complex64, np.complex128]:
-            complex_amplitude = np.array(amplitude.m_as("uT"))
-        else:
-            complex_amplitude = np.array((amplitude.m_as("uT") + 1j * np.zeros_like(amplitude.m_as("uT"))))
+        complex_amplitude = np.array((amplitude.m_as("uT") + 1j * np.zeros_like(amplitude.m_as("uT"))))
         phase_per_time = (self.phase_offset.m_as("rad") +
                           2 * np.pi * self.frequency_offset.m_as("kHz") * t_zero_ref.m_as("ms"))
         complex_amplitude = complex_amplitude * np.exp(1j * phase_per_time)
         return t, Quantity(complex_amplitude, "uT")
 
     @rf.setter
     def rf(self, value: Tuple[Quantity, Quantity]):
         self._rf = value
 
     @property
     def normalized_waveform(self) -> (np.ndarray, Quantity, np.ndarray, Quantity):
-        """
+        """Computes the normalized waveform (scaling between -1, 1).
+
         :return: - Normalized amplitude between [-1, 1] [dimensionless] (flipped such that the
                     maximum normalized value is positive. Scaling with peak amplitude inverts the
                     shape again)
                  - Peak amplitude in uT
                  - Phase per timestep in rad
                  - Time raster definition points
         """
@@ -202,19 +235,19 @@
         bandwidth = Quantity(time_bandwidth_product / duration.to("ms"), "1/ms")
 
         unit_flip_angle = np.sum((unit_wf[1:] + unit_wf[:-1]) / 2) * system_specs.rf_raster_time.to("ms")\
                           * system_specs.gamma_rad.to("rad/mT/ms")
 
         amplitude = unit_wf * flip_angle.to("rad") / unit_flip_angle
 
-        self._rf = (time_points + delay, amplitude)
-        self.rf_events = (center * duration + delay, flip_angle)
-
-        super().__init__(system_specs=system_specs, name=name, frequency_offset=frequency_offset,
-                         phase_offset=phase_offset, bandwidth=bandwidth, snap_to_raster=False)
+        super().__init__(system_specs=system_specs, name=name,
+                         time=time_points + delay, rf_waveform=amplitude,
+                         frequency_offset=frequency_offset, phase_offset=phase_offset,
+                         rf_events=(center * duration + delay, flip_angle),
+                         bandwidth=bandwidth, snap_to_raster=False)
     
     @staticmethod
     def _get_unit_waveform(raster_time: Quantity, time_bandwidth_product: float,
                            duration: Quantity,
                            apodization: float, center: float) -> Quantity:
         """ Constructs the sinc-pulse waveform according to:
 
@@ -233,16 +266,17 @@
 
         """   
         bandwidth = Quantity(time_bandwidth_product / duration.m_as("ms"), "1/ms")
         n_steps = np.around(duration.m_as("ms") / raster_time.m_as("ms"))
         time_points = Quantity(np.arange(0., n_steps+1, 1) * raster_time.m_as("ms"), "ms")
         time_rel_center = time_points.to("ms") - (center * duration.to("ms"))
         window = (1 - apodization) + apodization * np.cos(2 * np.pi * np.arange(-n_steps//2, n_steps//2+1, 1) / n_steps)
-        unit_wf = np.sinc((bandwidth.to("1/ms") * time_rel_center).m_as("dimensionless")) #* window
-        return time_points, unit_wf * window
+        unit_wf = np.sinc((bandwidth.to("1/ms") * time_rel_center).m_as("dimensionless")) * window
+        unit_wf -= unit_wf[0]
+        return time_points, unit_wf
 
     @classmethod
     def from_shortest(cls, system_specs: SystemSpec, flip_angle: Quantity,  
                       time_bandwidth_product: float = 3., center: float = 0.5,
                       delay: Quantity = Quantity(0., "ms"), 
                       apodization: float = 0.46, 
                       frequency_offset: Quantity = Quantity(0., "Hz"), 
@@ -254,15 +288,15 @@
         durations = Quantity(np.linspace(0.1, 1.5, 2), "ms")
         fas = []
         for dur in durations:
             _, unit_wf = cls._get_unit_waveform(raster_time=system_specs.rf_raster_time,
                                                 time_bandwidth_product=time_bandwidth_product,
                                                 duration=dur, apodization=apodization,
                                                 center=center)
-            max_wf =  unit_wf.m_as("dimensionless") * system_specs.rf_peak_power.to("uT")
+            max_wf =  unit_wf * system_specs.rf_peak_power.to("uT")
             fa = np.sum((max_wf[1:] + max_wf[:-1]) / 2 * system_specs.rf_raster_time.to("ms"))
             fa *= system_specs.gamma_rad.to("rad/mT/ms") 
             fas.append(fa.m_as("degree"))
         slope = Quantity(np.diff(durations.m_as("ms")) / np.diff(fas), "ms/degree")
         target_duration = system_specs.time_to_raster(np.abs(flip_angle) * slope, "rf")
         
         return cls(system_specs, duration=target_duration,
@@ -318,33 +352,46 @@
             flip_angle = -flip_angle
 
         raster_time = system_specs.rf_raster_time.to("ms")
         n_steps = np.around(duration.m_as("ms") / raster_time.m_as("ms"))
         time_points = Quantity(np.arange(0., n_steps+1, 1) * raster_time.m_as("ms"), "ms")
 
         amplitude = (flip_angle/system_specs.gamma_rad/raster_time/(n_steps+1)).to('mT')
-        self._rf = (time_points + delay, amplitude*np.ones_like(time_points))
-        self.rf_events = (duration/2 + delay, flip_angle)
 
-        super().__init__(system_specs=system_specs, name=name, frequency_offset=frequency_offset,
-                         phase_offset=phase_offset, bandwidth=0.5/duration, snap_to_raster=False)
+        super().__init__(system_specs=system_specs, name=name,
+                         time=time_points + delay, rf_waveform=amplitude*np.ones_like(time_points),
+                         frequency_offset=frequency_offset, phase_offset=phase_offset,
+                         rf_events=(duration/2 + delay, flip_angle),
+                         bandwidth=0.5/duration, snap_to_raster=False)
 
 class ArbitraryRFPulse(RFPulse):
     """ Wrapper for arbitrary rf shapes, to adhere to building block concept. 
     The gridding is assumed to be on raster time and **not** shifted by half
     a raster time. This shift (useful for simulations) can be incorporated when
     calling the gridding function of the sequence.
 
-    waveform is assumed to start and end with values of 0 uT
+    The waveform is assumed to start and end with values of 0 uT. If the given waveform does not
+    adhere to that definition, the arrays are padded.
+
+    The rf-center (time-point of effective excitation) is estimated from pulse maximum.
+
+    If not specified, the bandwidth of the given waveform is estimated by using the full width
+    at half maximum of the power-spectrum.
+
+      .. warning::
+
+        For very long pulses, the estimation of bandwidth might not be reasonable anymore, due to
+        relaxation.
+
 
     :param system_specs:
     :param name:
     :param time_points: Shape (#steps)
-    :param waveform: Shape (#steps) in uT as complex array
-    :param bandwidth:
+    :param waveform: Shape (#steps) in uT as real-valued array
+    :param bandwidth: in Hz, if not specified, the pulse bandwidth is estimated
     :param frequency_offset:
     :param phase_offset:
     :param snap_to_raster:
     """
     def __init__(self, system_specs: SystemSpec, name: str,
                  time_points: Quantity,
                  waveform: Quantity,
@@ -354,27 +401,124 @@
                  phase_offset: Quantity = Quantity(0., "rad"),
                  snap_to_raster: bool = False):
         """ 
         :param system_specs:
         :param name:
         :param time_points: Shape (#steps)
         :param waveform: Shape (#steps) in uT as complex array
-        :param bandwidth:
+        :param bandwidth: If not specified, the bandwidth is estimated from the spectrum as
+                            full-width-half-maximum.
         :param frequency_offset:
         :param phase_offset:
         :param snap_to_raster:
         """
-        self._rf = (time_points.to("ms") + delay, waveform.to("mT"))
+
+        if not np.isclose(waveform[0].m_as("uT"), 0., atol=1e-3):
+            time_points = np.concatenate([[time_points[0] - system_specs.rf_raster_time],
+                                           time_points], axis=0)
+            waveform = np.concatenate([[Quantity(0., "uT")], waveform], axis=0)
+
+        if not np.isclose(waveform[-1].m_as("uT"), 0., atol=1e-3):
+            time_points = np.concatenate([time_points,
+                                          [time_points[-1] + system_specs.rf_raster_time]], axis=0)
+            waveform = np.concatenate([waveform, [Quantity(0., "uT")]], axis=0)
+
+        center, center_index = self._calculate_rf_center(time=time_points.to("ms"),
+                                                         rf_waveform=waveform)
+        flip_angle = self._calculate_flipangle(time=time_points, rf_waveform=waveform,
+                                               gamma_rad=system_specs.gamma_rad)
+
+        ## This is a weird case that can occur on loading other format definitions
+        if np.allclose(waveform.m_as("uT"), 0., atol=1e-3):
+            bandwidth = Quantity(0, "Hz")
+
         if bandwidth is None:
-            # TODO: estimate bandwidth of arbitrary rf pulses
-            bandwidth = Quantity(0, "kHz")
-        #TODO estimate phase offset and freqoffset from complex wf
-
-        center = (time_points.to("ms")[-1] - time_points.to("ms")[0]) / 2 + time_points.to("ms")[0]
-        flip_angle = system_specs.gamma_rad * Quantity(np.trapz(waveform.real.m_as("mT"), time_points.m_as("ms")), "mT ms")
-        self.rf_events = (center, flip_angle.to("rad"))
+            _, _, bandwidth = self._calculate_bandwidth(time=time_points, rf_waveform=waveform,
+                                                        cut_off_percent=0.5,
+                                                        min_frequency_resolution=Quantity(10, "Hz"))
 
         super().__init__(system_specs, name, frequency_offset=frequency_offset,
+                         time=time_points.to("ms") + delay, rf_waveform=waveform.to("mT"),
                          phase_offset=phase_offset, bandwidth=bandwidth,
+                         rf_events=(time_points[center_index] + delay, flip_angle.to("rad")),
                          snap_to_raster=snap_to_raster)
 
+    @staticmethod
+    def _calculate_flipangle(time: Quantity, rf_waveform: Quantity, gamma_rad: Quantity) \
+            -> Quantity:
+        """Numerical integration of the rf-waveform to obtain the flip-angle
+
+        :param time: (#points, )
+        :param rf_waveform: (#points, )
+        :param gamma_rad: gyromagnetic ratio in units of radian
+        :return: Quantity
+        """
+        flip_angle = gamma_rad * Quantity(np.trapz(rf_waveform.real.m_as("mT"), time.m_as("ms")),
+                                          "mT ms")
+        return flip_angle
 
+    @staticmethod
+    def _calculate_bandwidth(time: Quantity, rf_waveform: Quantity, cut_off_percent: float,
+                             min_frequency_resolution : Quantity) -> \
+            Tuple[Quantity, Quantity, Quantity]:
+        """ Calculates the RF-bandwidth for the given waveform as the spectral width at
+        cut-off-percent.
+
+        :param time: Quantity[Time] (#points,  ) Time centered around the RF-center
+        :param rf_waveform: Quantity[Tesla]  (#points, )
+        :param cut_off_percent:
+        :param min_frequency_resolution: Minimal frequency target frequency resolution for spectrum
+        :return: (frequency_grid, power_spectrum, bandwidth)
+        """
+
+        if np.abs(time[-1] - time[0]) > Quantity(20, "ms"):
+            warn(f"Long pulses > 20ms might not be accurately covered using the bandwidth "
+                 f"estimation method for arbitrary RF pulses.")
+
+        resample_dt = Quantity(1, "us")
+        duration = (time[-1] - time[0]).to("us")
+        n_grid_points = np.round((duration / resample_dt).m_as("dimensionless")).astype(int)
+
+        # Padding the resampled temporal grid is done to achieve acceptable frequency resolution
+        # for bandwidth calculation
+        padding_factor = (1 / min_frequency_resolution / duration / 2).m_as("dimensionless")
+
+        resampled_t_grid = Quantity(np.arange(
+                                        -np.floor(n_grid_points * padding_factor).astype(int),
+                                        np.ceil(n_grid_points * (padding_factor + 1)).astype(int)),
+                                   "dimensionless") * resample_dt
+        interpolated_wf = np.interp(xp=(time - time[0]).m_as("ms"), fp=rf_waveform.m_as("uT"),
+                                    x=resampled_t_grid.m_as("ms"), left=0, right=0)
+
+        power_spectrum = np.abs(np.fft.fft(interpolated_wf))
+        freq_grid = Quantity(np.fft.fftfreq(resampled_t_grid.shape[0], resample_dt.m_as("s")), "Hz")
+
+        ## For ascending order of the frequency grid
+        sort_indices = np.argsort(freq_grid)
+        freq_grid  = freq_grid[sort_indices]
+        power_spectrum = power_spectrum[sort_indices]
+
+        peak = np.max(power_spectrum)
+
+        above_threshold_indices = np.where(power_spectrum > peak * cut_off_percent)
+        freq_band = freq_grid[above_threshold_indices].m_as("Hz")
+
+        bandwidth = Quantity(freq_band[-1] - freq_band[0], "Hz")
+        return freq_grid, power_spectrum, bandwidth
+
+    @staticmethod
+    def _calculate_rf_center(time: Quantity, rf_waveform: Quantity) -> Tuple[Quantity, int]:
+        """Calculates the time point of effective rotation for a given rf-waveform.
+
+        Assumptions: - Mean of Peaks of absolute defines center
+                     - Index on grid by rounding to nearest neighbor
+
+        :param time: Quantity[Time] (#points,  )
+        :param rf_waveform: Quantity[Tesla]  (#points, )
+        :return: (Quantity, int) time-center (not on necessarily on grid) and integer to
+                    index the handed waveforms for a representation on grid
+        """
+        rf_max = np.max(np.abs(rf_waveform.m_as("uT")))
+        peak_indices = np.where(np.abs(rf_waveform.m_as("uT")) >= rf_max * (1 - 1e-5))[0]
+        time_center = np.mean([time.m_as("ms")[i] for i in peak_indices])
+        center_index = np.round(np.mean(peak_indices)).astype(int)
+        return Quantity(time_center, "ms"), center_index
```

### Comparing `cmrseq-0.21/cmrseq/io/_json.py` & `cmrseq-0.22/cmrseq/io/_json.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/io/_phillips_load.py` & `cmrseq-0.22/cmrseq/io/_phillips_load.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/io/_pulseq.py` & `cmrseq-0.22/cmrseq/io/_pulseq.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/parametric_definitions/diffusion.py` & `cmrseq-0.22/cmrseq/parametric_definitions/diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,16 +263,16 @@
              - lambda: flat duration of fist trapezoidal
              - gmax: actually used max-gradient
              - slew: actually used slew-rate
              - b_actual: actual resulting b-value
     """
     # Strip units consistently for scipy optimize call
     gamma = system_specs.gamma_rad.m_as("1/ms/mT")
-    max_slew = system_specs.max_slew.m_as("mT/m/ms") * 0.98
-    gmax = system_specs.max_grad.m_as("mT/m") * 0.98
+    max_slew = system_specs.max_slew.m_as("mT/m/ms") * 0.97
+    gmax = system_specs.max_grad.m_as("mT/m") * 0.97
     zeta = system_specs.time_to_raster(Quantity(gmax / max_slew, "ms"))
     zeta = zeta.m
 
     def _optim(x): # Minimize total duration
         return 12 * zeta + 7 * x[0]
 
     def _constraint(x): # Match the target b-value
```

### Comparing `cmrseq-0.21/cmrseq/parametric_definitions/excitation.py` & `cmrseq-0.22/cmrseq/parametric_definitions/excitation.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/parametric_definitions/readout/__init__.py` & `cmrseq-0.22/cmrseq/parametric_definitions/readout/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/parametric_definitions/readout/_cartesian_single_lines.py` & `cmrseq-0.22/cmrseq/parametric_definitions/readout/_cartesian_single_lines.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/parametric_definitions/readout/_epi.py` & `cmrseq-0.22/cmrseq/parametric_definitions/readout/_epi.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/parametric_definitions/readout/_radial.py` & `cmrseq-0.22/cmrseq/parametric_definitions/readout/_radial.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/parametric_definitions/readout/_spiral.py` & `cmrseq-0.22/cmrseq/parametric_definitions/readout/_spiral.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/parametric_definitions/sequences/_gradient_echo.py` & `cmrseq-0.22/cmrseq/parametric_definitions/sequences/_gradient_echo.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/parametric_definitions/sequences/_spin_echo.py` & `cmrseq-0.22/cmrseq/parametric_definitions/sequences/_spin_echo.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/parametric_definitions/sequences/_ssfp.py` & `cmrseq-0.22/cmrseq/parametric_definitions/sequences/_ssfp.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/parametric_definitions/velocity.py` & `cmrseq-0.22/cmrseq/parametric_definitions/velocity.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq/plotting.py` & `cmrseq-0.22/cmrseq/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
                           ]
         legend_names = ["RF", r"$Re$", r"$Im$", "Gx", "Gy", "Gz", "ADC", "events",
                         "phase", "RF-centers", "ADC-centers", ""]
         legend = axes[0].legend(handles=legend_handles, labels=legend_names, ncol=4,
                                 columnspacing=2, fontsize=10, handlelength=3, loc=legend_position)
         small_texts = [legend.get_texts()[i] for i in [1, 2, 7, 8]]
         [t.set_size(7) for t in small_texts]
-        small_handles = [legend.legendHandles[i] for i in [1, 2, 7, 8]]
+        small_handles = [legend.legend_handles[i] for i in [1, 2, 7, 8]]
         [plt.setp(h, xdata=np.array([h.get_xdata()[-1] * 0.4, *h.get_xdata()[1:]]))
          for h in small_handles]
 
     if format_axes:
         [ax.set_ylabel(l) for ax, l in zip(axes, [r"RF [$\mu$T]", "G [mT/m]",
                                                   "G [mT/m]", "G [mT/m]"])]
         axes[-1].set_xlabel("Time [ms]")
```

### Comparing `cmrseq-0.21/cmrseq/utils.py` & `cmrseq-0.22/cmrseq/utils.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/cmrseq.egg-info/PKG-INFO` & `cmrseq-0.22/cmrseq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmrseq
-Version: 0.21
+Version: 0.22
 Summary: UNKNOWN
 Home-page: https://gitlab.ethz.ch/jweine/cmrseq
 Author: Jonathan Weine, Charles McGrath
 Author-email: weine@biomed.ee.ethz.ch, mcgrath@biomed.ee.ethz.ch
 License: UNKNOWN
 Project-URL: Documentation, https://people.ee.ethz.ch/~jweine/cmrseq/latest/index.html
 Project-URL: Source, https://gitlab.ethz.ch/jweine/cmrseq
```

### Comparing `cmrseq-0.21/cmrseq.egg-info/SOURCES.txt` & `cmrseq-0.22/cmrseq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmrseq-0.21/setup.py` & `cmrseq-0.22/setup.py`

 * *Files identical despite different names*

