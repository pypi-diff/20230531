# Comparing `tmp/pymatgen-analysis-defects-2023.5.8.tar.gz` & `tmp/pymatgen-analysis-defects-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen-analysis-defects-2023.5.8.tar", last modified: Mon May  8 23:46:05 2023, max compression
+gzip compressed data, was "pymatgen-analysis-defects-2023.6.1.tar", last modified: Wed May 31 07:26:34 2023, max compression
```

## Comparing `pymatgen-analysis-defects-2023.5.8.tar` & `pymatgen-analysis-defects-2023.6.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.506053 pymatgen-analysis-defects-2023.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-08 23:46:05.506053 pymatgen-analysis-defects-2023.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.498053 pymatgen-analysis-defects-2023.5.8/pymatgen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.498053 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.502053 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26443 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.506053 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/corrections/
--rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/corrections/freysoldt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/corrections/kumagai.py
--rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17001 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/supercells.py
--rw-r--r--   0 runner    (1001) docker     (123)    42384 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.506053 pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-08 23:46:05.000000 pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-08 23:46:05.000000 pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 23:46:05.000000 pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-08 23:46:05.000000 pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 23:46:05.000000 pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 23:46:05.506053 pymatgen-analysis-defects-2023.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:46:05.506053 pymatgen-analysis-defects-2023.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/tests/test_ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-08 23:45:48.000000 pymatgen-analysis-defects-2023.5.8/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-08 23:45:49.000000 pymatgen-analysis-defects-2023.5.8/tests/test_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-08 23:45:49.000000 pymatgen-analysis-defects-2023.5.8/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-08 23:45:49.000000 pymatgen-analysis-defects-2023.5.8/tests/test_recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-08 23:45:49.000000 pymatgen-analysis-defects-2023.5.8/tests/test_supercells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-08 23:45:49.000000 pymatgen-analysis-defects-2023.5.8/tests/test_thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-08 23:45:49.000000 pymatgen-analysis-defects-2023.5.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.322738 pymatgen-analysis-defects-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-31 07:26:34.322738 pymatgen-analysis-defects-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.318738 pymatgen-analysis-defects-2023.6.1/pymatgen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.318738 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.318738 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28813 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.318738 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/corrections/
+-rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/corrections/freysoldt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/corrections/kumagai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/supercells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.318738 pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-31 07:26:34.000000 pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-31 07:26:34.000000 pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:26:34.000000 pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-31 07:26:34.000000 pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 07:26:34.000000 pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 07:26:34.322738 pymatgen-analysis-defects-2023.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.322738 pymatgen-analysis-defects-2023.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/tests/test_ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-31 07:26:17.000000 pymatgen-analysis-defects-2023.6.1/tests/test_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-31 07:26:17.000000 pymatgen-analysis-defects-2023.6.1/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-31 07:26:17.000000 pymatgen-analysis-defects-2023.6.1/tests/test_recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-31 07:26:17.000000 pymatgen-analysis-defects-2023.6.1/tests/test_supercells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-31 07:26:17.000000 pymatgen-analysis-defects-2023.6.1/tests/test_thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-31 07:26:17.000000 pymatgen-analysis-defects-2023.6.1/tests/test_utils.py
```

### Comparing `pymatgen-analysis-defects-2023.5.8/LICENSE` & `pymatgen-analysis-defects-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/PKG-INFO` & `pymatgen-analysis-defects-2023.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2023.5.8
+Version: 2023.6.1
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
```

### Comparing `pymatgen-analysis-defects-2023.5.8/README.rst` & `pymatgen-analysis-defects-2023.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/ccd.py` & `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/ccd.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/constants.py` & `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/constants.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/core.py` & `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,25 +160,28 @@
         sc_mat: np.ndarray | None = None,
         dummy_species: str | None = None,
         min_atoms: int = 80,
         max_atoms: int = 240,
         min_length: float = 10.0,
         force_diagonal: bool = False,
         relax_radius: float | str | None = None,
+        perturb: float | None = None,
     ) -> Structure:
         """Generate the supercell for a defect.
 
         Args:
             sc_mat: supercell matrix if None, the supercell will be determined by `CubicSupercellAnalyzer`.
             dummy_species: Dummy species to highlight the defect position (for visualizing vacancies).
             max_atoms: Maximum number of atoms allowed in the supercell.
             min_atoms: Minimum number of atoms allowed in the supercell.
             min_length: Minimum length of the smallest supercell lattice vector.
             force_diagonal: If True, return a transformation with a diagonal transformation matrix.
             relax_radius: Relax the supercell atoms to a sphere of this radius around the defect site.
+            perturb: The amount to perturb the sites in the supercell. Only perturb the sites with
+                selective dynamics set to True. So this setting only works with `relax_radius`.
 
         Returns:
             Structure: The supercell structure.
         """
         if sc_mat is None:
             sc_mat = get_sc_fromstruct(
                 self.structure,
@@ -202,17 +205,20 @@
         if dummy_species is not None:
             dummy_pos = np.dot(self.site.frac_coords, sc_mat_inv)
             dummy_pos = np.mod(dummy_pos, 1)
             sc_defect_struct.insert(len(sc_structure), dummy_species, dummy_pos)
 
         _set_selective_dynamics(
             structure=sc_defect_struct,
-            site_pos=sc_pos,
+            site_pos=sc_site.coords,
             relax_radius=relax_radius,
         )
+        if perturb is not None:
+            _perturb_dynamic_sites(sc_defect_struct, distance=perturb)
+
         return sc_defect_struct
 
     @property
     def symmetrized_structure(self) -> SymmetrizedStructure:
         """Returns the multiplicity of a defect site within the structure.
 
         This is required for concentration analysis and confirms that defect_site is a
@@ -352,24 +358,19 @@
         """Name of the defect."""
         return f"{get_element(self.site.specie)}_{get_element(self.defect_site.specie)}"
 
     @property
     def defect_structure(self) -> Structure:
         """Returns the defect structure."""
         struct: Structure = self.structure.copy()
-        rm_oxi = struct.sites[self.defect_site_index].specie.oxi_state
         struct.remove_sites([self.defect_site_index])
-        sub_states = self.site.specie.icsd_oxidation_states
-        if len(sub_states) == 0:
-            sub_states = self.site.specie.oxidation_states
-        sub_oxi = min(sub_states, key=lambda x: abs(x - rm_oxi))
-        sub_specie = Species(self.site.specie.symbol, sub_oxi)
+        insert_el = get_element(self.site.specie)
         struct.insert(
             self.defect_site_index,
-            species=sub_specie,
+            species=insert_el,
             coords=np.mod(self.site.frac_coords, 1),
         )
         return struct
 
     @property
     def defect_site(self):
         """Returns the site in the structure that corresponds to the defect site."""
@@ -402,17 +403,23 @@
 
         For a substitution defect, the oxidation state of the defect is given
         by the difference between the oxidation state of the new and old atoms.
 
         Returns:
             float: The oxidation state of the defect.
         """
-        orig_site = self.defect_site
-        sub_site = self.defect_structure[self.defect_site_index]
-        return sub_site.specie.oxi_state - orig_site.specie.oxi_state
+        rm_oxi = self.structure[self.defect_site_index].specie.oxi_state
+        sub_states = self.site.specie.common_oxidation_states
+        if len(sub_states) == 0:
+            raise ValueError(
+                f"No common oxidation states found for {self.site.specie}."
+                "Please specify the oxidation state manually."
+            )
+        sub_oxi = sub_states[0]
+        return sub_oxi - rm_oxi
 
     def __repr__(self) -> str:
         """Representation of a substitutional defect."""
         rm_species = get_element(self.defect_site.specie)
         sub_species = get_element(self.site.specie)
         return (
             f"{sub_species} subsitituted on the {rm_species} site at "
@@ -575,25 +582,29 @@
         sc_mat: np.ndarray | None = None,
         dummy_species: Species | None = None,
         min_atoms: int = 80,
         max_atoms: int = 240,
         min_length: float = 10.0,
         force_diagonal: bool = False,
         relax_radius: float | str | None = None,
+        perturb: float | None = None,
     ) -> Structure:
         """Generate the supercell for a defect.
 
         Args:
             sc_mat: supercell matrix if None, the supercell will be determined by `CubicSupercellAnalyzer`.
             dummy_species: Dummy species used for visualization. Will be placed at the average
                 position of the defect sites.
             max_atoms: Maximum number of atoms allowed in the supercell.
             min_atoms: Minimum number of atoms allowed in the supercell.
             min_length: Minimum length of the smallest supercell lattice vector.
             force_diagonal: If True, return a transformation with a diagonal transformation matrix.
+            relax_radius: Relax the supercell atoms to a sphere of this radius around the defect site.
+            perturb: The amount to perturb the sites in the supercell. Only perturb the sites with
+                selective dynamics set to True. So this setting only works with `relax_radius`.
 
         Returns:
             Structure: The supercell structure.
         """
         if sc_mat is None:
             sc_mat = get_sc_fromstruct(
                 self.structure,
@@ -615,17 +626,21 @@
             for defect in self.defects:
                 dummy_pos = np.dot(defect.site.frac_coords, sc_mat_inv)
                 dummy_pos = np.mod(dummy_pos, 1)
                 sc_defect_struct.insert(len(sc_defect_struct), dummy_species, dummy_pos)
 
         _set_selective_dynamics(
             structure=sc_defect_struct,
-            site_pos=sc_pos,
+            site_pos=sc_site.coords,
             relax_radius=relax_radius,
         )
+
+        if perturb is not None:
+            _perturb_dynamic_sites(sc_defect_struct, distance=perturb)
+
         return sc_defect_struct
 
 
 def update_structure(structure, site, defect_type):
     """Update the structure with the defect site.
 
     Types of operations:
@@ -719,24 +734,73 @@
 def _set_selective_dynamics(structure, site_pos, relax_radius):
     if relax_radius is None:
         return
     if relax_radius == "auto":
         relax_radius = min(get_plane_spacing(structure.lattice.matrix)) / 2.0
     if not isinstance(relax_radius, float):
         raise ValueError("relax_radius must be a float or 'auto' or None")
-
     structure.get_sites_in_sphere(site_pos, relax_radius)
     relax_sites = structure.get_sites_in_sphere(
-        [0, 0, 0], relax_radius, include_index=True
+        site_pos, relax_radius, include_index=True
     )
     relax_indices = [site.index for site in relax_sites]
     relax_mask = [[False, False, False]] * len(structure)
     for i in relax_indices:
         relax_mask[i] = [True, True, True]
     structure.add_site_property("selective_dynamics", relax_mask)
 
 
+def perturb_sites(
+    structure,
+    distance: float,
+    min_distance: float | None = None,
+    site_indices: list | None = None,
+) -> None:
+    """
+    Performs a random perturbation of the sites in a structure to break
+    symmetries.
+
+    Args:
+        structure (Structure): Input structure.
+        distance (float): Distance in angstroms by which to perturb each
+            site.
+        min_distance (None, int, or float): if None, all displacements will
+            be equal amplitude. If int or float, perturb each site a
+            distance drawn from the uniform distribution between
+            'min_distance' and 'distance'.
+        site_indices (list): List of site indices on which to perform the
+            perturbation. If None, all sites will be perturbed.
+
+    """
+
+    def get_rand_vec():
+        # deals with zero vectors.
+        vector = np.random.randn(3)
+        vnorm = np.linalg.norm(vector)
+        dist = distance
+        if isinstance(min_distance, (float, int)):
+            dist = np.random.uniform(min_distance, dist)
+        return vector / vnorm * dist if vnorm != 0 else get_rand_vec()
+
+    if site_indices is None:
+        site_indices_ = list(range(len(structure._sites)))
+    else:
+        site_indices_ = site_indices
+
+    for i in site_indices_:
+        structure.translate_sites([i], get_rand_vec(), frac_coords=False)
+
+
+def _perturb_dynamic_sites(structure, distance):
+    free_indices = [
+        i
+        for i, site in enumerate(structure)
+        if site.properties["selective_dynamics"][0]
+    ]
+    perturb_sites(structure=structure, distance=distance, site_indices=free_indices)
+
+
 # TODO: matching defect complexes might be done with some kind of CoM site to fix the periodicity
 # Get this by taking the periodic average of all the provided sites.
 # class DefectComplex(DummySpecies):
 #     def __init__(self, oxidation_state: float = 0, properties: dict | None = None):
 #         super().__init__("Vac", oxidation_state, properties)
```

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/corrections/freysoldt.py` & `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/corrections/freysoldt.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/corrections/kumagai.py` & `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/corrections/kumagai.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/finder.py` & `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/finder.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,26 +44,34 @@
             raise ImportError(
                 "dscribe is required to use DefectSiteFinder. Install with ``pip install dscribe``."
             )
         self.symprec = symprec
         self.angle_tolerance = angle_tolerance
 
     def get_defect_fpos(
-        self, defect_structure: Structure, base_structure: Structure
+        self,
+        defect_structure: Structure,
+        base_structure: Structure,
+        remove_oxi: bool = True,
     ) -> ArrayLike:
         """Get the position of a defect in the pristine structure.
 
         Args:
             defect_structure: Relaxed structure containing the defect
             base_structure: Structure for the pristine cell
+            remove_oxi: Whether to remove oxidation states from the structures
 
         Returns:
             ArrayLike: Position of the defect in the pristine structure
             (in fractional coordinates)
         """
+        if remove_oxi:
+            defect_structure.remove_oxidation_states()
+            base_structure.remove_oxidation_states()
+
         if self._is_impurity(defect_structure, base_structure):
             return self.get_impurity_position(defect_structure, base_structure)
         else:
             return self.get_native_defect_position(defect_structure, base_structure)
 
     def _is_impurity(
         self, defect_structure: Structure, base_structure: Structure
```

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/generators.py` & `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,21 +349,23 @@
         clustering_tol: float = 0.6,
         ltol: float = 0.2,
         stol: float = 0.3,
         angle_tol: float = 5,
         min_dist: float = 1.0,
         avg_radius: float = 0.4,
         max_avg_charge: float = 0.9,
+        max_insertions: int | None = None,
     ) -> None:
         self.clustering_tol = clustering_tol
         self.ltol = ltol
         self.stol = stol
         self.angle_tol = angle_tol
         self.avg_radius = avg_radius
         self.max_avg_charge = max_avg_charge
+        self.max_insertions = max_insertions
         super().__init__(min_dist=min_dist)
 
     def generate(self, chgcar: Chgcar, insert_species: set[str] | list[str], **kwargs) -> Generator[Interstitial, None, None]:  # type: ignore[override]
         """Generate interstitials.
 
         Args:
             chgcar: The chgcar object to be used for the charge density.
@@ -371,14 +373,16 @@
             **kwargs: Additional keyword arguments for the ``Interstitial`` constructor.
         """
         if len(set(insert_species)) != len(insert_species):  # pragma: no cover
             raise ValueError("Insert species must be unique.")
         cand_sites_and_mul = [*self._get_candidate_sites(chgcar)]
         for species in insert_species:
             cand_sites = [cand_site for cand_site, mul in cand_sites_and_mul]
+            if self.max_insertions is not None:
+                cand_sites = cand_sites[: self.max_insertions]
             multiplicity = [mul for cand_site, mul in cand_sites_and_mul]
             yield from super().generate(
                 chgcar.structure,
                 insertions={species: cand_sites},
                 multiplicies={species: multiplicity},
                 **kwargs,
             )
@@ -400,16 +404,28 @@
 
 
 def generate_all_native_defects(
     host: Structure | Chgcar,
     sub_generator: SubstitutionGenerator | None = None,
     vac_generator: VacancyGenerator | None = None,
     int_generator: ChargeInterstitialGenerator | None = None,
+    max_insertions: int | None = None,
 ):
-    """Generate all native defects."""
+    """Generate all native defects.
+
+    Convenience function to generate all native defects for a host structure or chgcar object.
+
+    Args:
+        host: The host structure or chgcar object.
+        sub_generator: The substitution generator, if None, a default generator is used.
+        vac_generator: The vacancy generator, if None, a default generator is used.
+        int_generator: The interstitial generator, if None, a default
+            ChargeInterstitialGenerator is used.
+        max_insertions: The maximum number of interstitials to attempt to insert.
+    """
     if isinstance(host, Chgcar):
         struct = host.structure
         chgcar = host
     elif isinstance(host, Structure):
         struct = host
         chgcar = None
     else:
@@ -422,15 +438,17 @@
     yield from vac_generator.generate(struct)
     # generate substitutions for all pairs of species
     for sp1, sp2 in itertools.combinations(species, 2):
         yield from sub_generator.generate(struct, {sp1: sp2})
         yield from sub_generator.generate(struct, {sp2: sp1})
     # generate interstitials if a chgcar is provided
     if chgcar is not None:
-        int_generator = int_generator or ChargeInterstitialGenerator()
+        int_generator = int_generator or ChargeInterstitialGenerator(
+            max_insertions=max_insertions
+        )
         yield from int_generator.generate(chgcar, insert_species=species)
 
 
 def _element_str(sp_or_el: Species | Element) -> str:
     """Convert a species or element to a string."""
     if isinstance(sp_or_el, Species):
         return str(sp_or_el.element)
```

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/recombination.py` & `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/supercells.py` & `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/thermo.py` & `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/thermo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1003,27 +1003,28 @@
     elif isinstance(formation_energy_diagrams, FormationEnergyDiagram):
         formation_energy_diagrams = [formation_energy_diagrams]
 
     filterfunction = filterfunction if filterfunction else lambda x: True
     formation_energy_diagrams = list(filter(filterfunction, formation_energy_diagrams))
 
     band_gap = formation_energy_diagrams[0].band_gap
-    if not xlim and not band_gap:
+    if not xlim and band_gap is None:
         raise ValueError("Must specify xlim or set band_gap attribute")
 
     if axis is None:
         _, axis = plt.subplots()
-    axis.plot([0, 0], [0, 1], color=band_edge_color, linestyle="--", linewidth=1)
-    if not xlim and band_gap:
+    axis.axvline(band_gap, color=band_edge_color, linestyle="--", linewidth=1)
+    axis.axvline(0, color=band_edge_color, linestyle="--", linewidth=1)
+    if not xlim:
         xmin, xmax = np.subtract(-0.2, alignment), np.subtract(
             band_gap + 0.2, alignment
         )
     else:
         xmin, xmax = xlim
-    ymin, ymax = 0.0, 1.0
+    ymin, ymax = np.inf, -np.inf
     legends_txt = []
     artists = []
     fontwidth = 12
     ax_fontsize = 1.3
     lg_fontsize = 10
 
     colors = (
@@ -1047,17 +1048,20 @@
         lines = single_fed._get_lines(chempots=chempots_)
         lowerlines = get_lower_envelope(lines)
         trans = np.array(
             get_transitions(
                 lowerlines, np.add(xmin, alignment), np.add(xmax, alignment)
             )
         )
+        trans_y = trans[:, 1]
+        ymin = min(ymin, min(trans_y))
+        ymax = max(ymax, max(trans_y))
         axis.plot(
             np.subtract(trans[:, 0], alignment),
-            trans[:, 1],
+            trans_y,
             color=colors[fid],
             ls=linestyle,
             lw=linewidth,
             alpha=envelope_alpha,
             label=fed_name,
             marker=transition_marker,
             markersize=transition_markersize,
```

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen/analysis/defects/utils.py` & `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/utils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/PKG-INFO` & `pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2023.5.8
+Version: 2023.6.1
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
```

### Comparing `pymatgen-analysis-defects-2023.5.8/pymatgen_analysis_defects.egg-info/SOURCES.txt` & `pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/pyproject.toml` & `pymatgen-analysis-defects-2023.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/tests/test_ccd.py` & `pymatgen-analysis-defects-2023.6.1/tests/test_ccd.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/tests/test_core.py` & `pymatgen-analysis-defects-2023.6.1/tests/test_core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 from pymatgen.core.periodic_table import Element, Specie
-from pymatgen.io.vasp import Poscar
 
 from pymatgen.analysis.defects.core import (
     Adsorbate,
     DefectComplex,
     Interstitial,
     PeriodicSite,
     Substitution,
     Vacancy,
 )
+from pymatgen.analysis.defects.finder import DefectSiteFinder
 
 
 def test_vacancy(gan_struct):
     s = gan_struct.copy()
     vac = Vacancy(s, s.sites[0])
     vac2 = Vacancy(s, s.sites[1])
     assert vac == vac2  # symmetry equivalent sites
@@ -43,18 +43,35 @@
     sc = sub.get_supercell_structure()
     assert sc.formula == "Ga64 N63 O1"
     assert sub.name == "O_N"
     assert sub == sub
     assert sub.element_changes == {Element("N"): -1, Element("O"): 1}
 
     # test supercell with locking
-    sc_locked = sub.get_supercell_structure(relax_radius=1.0)
-    poscar_locked = Poscar(sc_locked)
-    poscar_string = poscar_locked.get_string()
-    assert len(poscar_string.split("\n")) == 138
+    sc_locked = sub.get_supercell_structure(relax_radius=5.0)
+    free_sites = [
+        i
+        for i, site in enumerate(sc_locked)
+        if site.properties["selective_dynamics"][0]
+    ]
+
+    finder = DefectSiteFinder()
+    fpos = finder.get_defect_fpos(sc_locked, sub.structure)
+    cpos = sc_locked.lattice.get_cartesian_coords(fpos)
+    free_sites_ref = sc_locked.get_sites_in_sphere(cpos, 5.0, include_index=True)
+    free_sites_ref = [site.index for site in free_sites_ref]
+    free_sites_union = set(free_sites_ref) | set(free_sites)
+    free_sites_intersection = set(free_sites_ref) & set(free_sites)
+    assert len(free_sites_intersection) / len(free_sites_union) == 1.0
+
+    # test perturbation
+    sc_locked = sub.get_supercell_structure(relax_radius=5.0, perturb=0.0)
+    free_sites_ref2 = sc_locked.get_sites_in_sphere(cpos, 5.0, include_index=True)
+    free_sites_ref2 = [site.index for site in free_sites_ref2]
+    assert set(free_sites_ref2) == set(free_sites_ref)
 
     # test for user defined charge
     dd = sub.as_dict()
     dd["user_charges"] = [-100, 102]
     sub_ = Substitution.from_dict(dd)
     assert sub_.get_charge_states() == [-100, 102]
```

### Comparing `pymatgen-analysis-defects-2023.5.8/tests/test_corrections.py` & `pymatgen-analysis-defects-2023.6.1/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/tests/test_finder.py` & `pymatgen-analysis-defects-2023.6.1/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/tests/test_generators.py` & `pymatgen-analysis-defects-2023.6.1/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/tests/test_recombination.py` & `pymatgen-analysis-defects-2023.6.1/tests/test_recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/tests/test_supercells.py` & `pymatgen-analysis-defects-2023.6.1/tests/test_supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/tests/test_thermo.py` & `pymatgen-analysis-defects-2023.6.1/tests/test_thermo.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.5.8/tests/test_utils.py` & `pymatgen-analysis-defects-2023.6.1/tests/test_utils.py`

 * *Files identical despite different names*

