# Comparing `tmp/matchmaps-0.2.0.tar.gz` & `tmp/matchmaps-0.3.0.tar.gz`

## Comparing `matchmaps-0.2.0.tar` & `matchmaps-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github_changelog_generator
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.2.0/setup.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.2.0/tox.ini
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github/workflows/cron.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/Makefile
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/about.md
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/cli.md
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/conf.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/index.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/make.bat
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/_static/custom.css
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.2.0/src/matchmaps/__init__.py
--rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 matchmaps-0.2.0/src/matchmaps/_compute_ncs_diff.py
--rwxr-xr-x   0        0        0    11908 2020-02-02 00:00:00.000000 matchmaps-0.2.0/src/matchmaps/_compute_realspace_diff.py
--rw-r--r--   0        0        0    20103 2020-02-02 00:00:00.000000 matchmaps-0.2.0/src/matchmaps/_utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.2.0/tests/test_matchmaps.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.2.0/LICENSE
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.2.0/README.md
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 matchmaps-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 matchmaps-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github_changelog_generator
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.3.0/setup.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.3.0/tox.ini
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/about.md
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/cli.md
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/index.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/_static/custom.css
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.3.0/src/matchmaps/__init__.py
+-rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 matchmaps-0.3.0/src/matchmaps/_compute_mr_diff.py
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 matchmaps-0.3.0/src/matchmaps/_compute_ncs_diff.py
+-rwxr-xr-x   0        0        0    12085 2020-02-02 00:00:00.000000 matchmaps-0.3.0/src/matchmaps/_compute_realspace_diff.py
+-rw-r--r--   0        0        0    26050 2020-02-02 00:00:00.000000 matchmaps-0.3.0/src/matchmaps/_utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.3.0/tests/test_matchmaps.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.3.0/LICENSE
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.3.0/README.md
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 matchmaps-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 matchmaps-0.3.0/PKG-INFO
```

### Comparing `matchmaps-0.2.0/.pre-commit-config.yaml` & `matchmaps-0.3.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   autofix_commit_msg: "style(pre-commit.ci): auto fixes [...]"
   autoupdate_commit_msg: "ci(pre-commit.ci): autoupdate"
 
 default_install_hook_types: [pre-commit, commit-msg]
 
 repos:
   - repo: https://github.com/compilerla/conventional-pre-commit
-    rev: v2.1.1
+    rev: v2.2.0
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
```

### Comparing `matchmaps-0.2.0/setup.py` & `matchmaps-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.2.0/tox.ini` & `matchmaps-0.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `matchmaps-0.2.0/.github/workflows/build_docs.yml` & `matchmaps-0.3.0/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.2.0/.github/workflows/ci.yml` & `matchmaps-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.2.0/.github/workflows/cron.yml` & `matchmaps-0.3.0/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.2.0/docs/Makefile` & `matchmaps-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `matchmaps-0.2.0/docs/conf.py` & `matchmaps-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.2.0/docs/index.md` & `matchmaps-0.3.0/docs/index.md`

 * *Files 18% similar despite different names*

```diff
@@ -27,17 +27,21 @@
 ```bash
 source /path/to/phenix/phenix_env.sh
 /path/to/ccp4/start
 ```
 
 At this point, you should be good to go! Please [file an issue on github](https://github.com/dennisbrookner/matchmaps/issues) is this is not working.
 
-## Using matchmaps
+## Using `matchmaps`
 
-Read about [using `matchmaps` in the command-line](cli.md)
+`matchmaps` consists of three command-line utilities. Usage for all three is documented [here](cli.md). All three produce a real-space difference map and require a single starting model for phasing, but differ in the types of reflection data they require. Briefly:
+
+ - **`matchmaps`** takes in two mtzs containing similar data and which are nearly isomorphous and computes an unbiased real-space difference map between them
+ - **`matchmaps.mr`** takes in two mtzs containing similar data but which are in different spacegroups (or the same spacegroup but different crystal packing) and computes an unbiased real-space difference map between them.
+ - **`matchmaps.mr`** takes in a single mtz and computes an internal difference map across a defined non-crystallographic symmetry present in the data.
 
 ```{eval-rst}
 .. toctree::
    :maxdepth: 1
    :hidden:
 
    Command-line usage <cli>
```

### Comparing `matchmaps-0.2.0/docs/make.bat` & `matchmaps-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `matchmaps-0.2.0/src/matchmaps/_compute_ncs_diff.py` & `matchmaps-0.3.0/src/matchmaps/_compute_ncs_diff.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.2.0/src/matchmaps/_compute_realspace_diff.py` & `matchmaps-0.3.0/src/matchmaps/_compute_realspace_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     _handle_special_positions,
     # align_grids_from_model_transform,
     make_floatgrid_from_mtz,
     rigid_body_refinement_wrapper,
     _realspace_align_and_subtract,
     _rbr_selection_parser,
     _renumber_waters,
+    # _clean_up_files,
 )
 
 
 def compute_realspace_difference_map(
     pdboff,
     mtzoff,
     mtzon,
@@ -36,15 +37,15 @@
     input_dir="./",
     output_dir="./",
     verbose=False,
     rbr_selections=None,
     eff=None,
 ):
     """
-    _summary_.
+    Compute a real-space difference map from mtzs.
 
     Parameters
     ----------
     pdboff : string
         Name of input .pdb file to use for phasing
     mtzoff : string
         Name of input .mtz file containing 'off' data
@@ -63,15 +64,15 @@
         by default None, meaning only the .pdb is required for refinement
     dmin : float, optional
         Minimum resolution (in Angstroms) reflections to be used in computing real-space maps from mtzs.
         If omitted, resolution cutoff is the maximum resolution from the lower-resolution input file.
     spacing : float, optional
         Approximate size of real-space voxels in Angstroms, by default 0.5 A
     on_as_stationary : bool, optional
-        _description_, by default False
+        If True, align "off" data onto "on" data, by default False
     input_dir : str, optional
         Path to directory containing input files, by default "./" (current directory)
     output_dir : str, optional
         Path to directory to which output files should be written, by default "./" (current directory)
     verbose : bool, optional
         If True, print outputs of scaleit and phenix.refine, by default False
     rbr_selections : list of strings, optional
@@ -191,14 +192,17 @@
                 pdbon=pdbon,
                 output_dir=output_dir,
                 on_name=on_name_rbr,
                 off_name=off_name_rbr,
                 on_as_stationary=on_as_stationary,
                 selection=selection,
             )
+    # print(f"{time.strftime('%H:%M:%S')}: Cleaning up files...")
+
+    # _clean_up_files()
 
     print(f"{time.strftime('%H:%M:%S')}: Done!")
 
     return
 
 
 def parse_arguments():
```

### Comparing `matchmaps-0.2.0/src/matchmaps/_utils.py` & `matchmaps-0.3.0/src/matchmaps/_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Utilities and helperfunctions used by matchmaps.
 
 Functions make_floatgrid_from_mtz, rigid_body_refinement_wrapper, and align_grids_from_model_transform
 are exported to python for use in prototyping and testing
 """
 
+import os
 import glob
 import shutil
 import subprocess
 import time
 import re
 from functools import partial
 
@@ -224,20 +225,31 @@
 
     if off_labels is None:
         nickname = f"{mtzon.removesuffix('.mtz')}_rbr_to_{pdboff.removesuffix('.pdb')}"
     else:
         nickname = f"{mtzon.removesuffix('.mtz')}_rbr_to_self"
 
     # check existing files because phenix doesn't like to overwrite things
+
+    # number = _find_available_suffix(prefix=f"{output_dir}/{nickname}_", suffix='_1.*')
+    # nickname += f'_{number}'
+
     similar_files = glob.glob(f"{output_dir}/{nickname}_[0-9]_1.*")
     if len(similar_files) == 0:
         nickname += "_0"
     else:
-        n = max([int(s.split("_")[-2]) for s in similar_files])
-        nickname += f"_{n+1}"
+        # n = max([int(s.split("_")[-2]) for s in similar_files])
+        # nickname += f"_{n+1}"
+        nums = []
+        for s in similar_files:
+            try:
+                nums.append(int(s.split("_")[-2]))
+            except ValueError:
+                pass
+        nickname += f"_{max(nums)+1}"
 
     # read in mtz to access cell parameters and spacegroup
     mtz = rs.read_mtz((output_dir if (off_labels is None) else input_dir) + mtzon)
     cell_string = f"{mtz.cell.a} {mtz.cell.b} {mtz.cell.c} {mtz.cell.alpha} {mtz.cell.beta} {mtz.cell.gamma}"
     sg = mtz.spacegroup.short_name()
 
     # edit refinement template
@@ -365,14 +377,180 @@
     )
 
     print(f"{time.strftime('%H:%M:%S')}: Moved waters to nearest protein chains...")
 
     return pdb_renumbered
 
 
+def _remove_waters(
+    input_pdb,
+    dir,
+):
+    output_pdb = input_pdb.removesuffix(".pdb") + "_dry"
+
+    subprocess.run(
+        f"phenix.pdbtools {dir}/{input_pdb} remove='water' \
+            output.prefix='{dir}/' \
+            output.suffix='{output_pdb}'",
+        shell=True,
+        capture_output=True,
+    )
+
+    return output_pdb + ".pdb"
+
+
+def phaser_wrapper(
+    mtzfile,
+    pdb,
+    input_dir,
+    output_dir,
+    off_labels,
+    eff=None,
+    verbose=False,
+):
+    """
+    Handle simple phaser run from the command line
+    """
+
+    if shutil.which("phenix.phaser") is None:
+        raise OSError(
+            "Cannot find executable, phenix.phaser. Please set up your phenix environment."
+        )
+
+    if eff is None:
+        eff_contents = """
+phaser {
+  mode = ANO CCA EP_AUTO *MR_AUTO MR_FRF MR_FTF MR_PAK MR_RNP NMAXYZ SCEDS
+  hklin = mtz_input
+  labin = labels
+  model = pdb_input
+  model_identity = 100
+  component_copies = 1
+  search_copies = 1
+  chain_type = *protein dna rna
+  crystal_symmetry {
+    unit_cell = cell_parameters
+    space_group = sg
+  }
+  keywords {
+    general {
+      root = '''nickname'''
+      title = '''matchmaps_MR'''
+      mute = None
+      xyzout = True
+      xyzout_ensemble = True
+      hklout = True
+      jobs = 6
+    }
+  }
+}
+        """
+    else:
+        raise NotImplementedError("Custom phaser specifications are not yet supported")
+
+    nickname = f"{mtzfile.removesuffix('.mtz')}_phased_with_{pdb.removesuffix('.pdb')}"
+
+    similar_files = glob.glob(f"{output_dir}/{nickname}_*")
+    if len(similar_files) == 0:
+        nickname += "_0"
+    else:
+        nums = []
+        for s in similar_files:
+            try:
+                nums.append(int(s.split("_")[-1].split(".")[0]))
+            except ValueError:
+                pass
+        # n = max([int(s.split("_")[-1].split(".")[0]) for s in similar_files])
+        nickname += f"_{max(nums)+1}"
+
+    mtz = rs.read_mtz(input_dir + mtzfile)
+    cell_string = f"{mtz.cell.a} {mtz.cell.b} {mtz.cell.c} {mtz.cell.alpha} {mtz.cell.beta} {mtz.cell.gamma}"
+    sg = mtz.spacegroup.short_name()
+
+    eff = f"{output_dir}/params_{nickname}.eff"
+
+    params = {
+        "sg": sg,
+        "cell_parameters": cell_string,
+        "pdb_input": output_dir + pdb,
+        "mtz_input": input_dir + mtzfile,
+        "nickname": output_dir + nickname,
+        "labels": off_labels,  # should be prepackaged as a string
+    }
+
+    for key, value in params.items():
+        eff_contents = eff_contents.replace(key, value)
+
+    with open(eff, "w") as file:
+        file.write(eff_contents)
+
+    subprocess.run(
+        f"phenix.phaser {eff}",
+        shell=True,
+        capture_output=(not verbose),
+    )
+
+    return nickname
+
+
+def _restore_ligand_occupancy(
+    pdb_to_be_restored,
+    original_pdb,
+    output_dir,
+):
+    # do stuff
+    # replace with actual logical about ligands being present
+    # if len(ligands) == 0:
+    #     edited_pdb = pdb_to_be_restored
+
+    # else:
+    #     edited_pdb = pdb_to_be_restored.removesuffix(".pdb") + "_restoreligs"
+
+    #     ligand_names = [f"resname {l.removesuffix('.cif')}" for l in ligands]
+    #     selection = " or ".join(ligand_names)
+
+    #     print(ligand_names)
+    #     print(selection)
+
+    #     subprocess.run(
+    #         f"phenix.pdbtools {output_dir}/{pdb_to_be_restored} \
+    #             output.prefix='{output_dir}'  output.suffix='{edited_pdb}'\
+    #             modify.selection='{selection}' modify.occupancies.set=1",
+    #         shell=True,
+    #         capture_output=True,
+    #     )
+
+    # grab occupancies of all HETATMs in original_pdb
+    with open(output_dir + original_pdb, "r") as o:
+        original = o.readlines()
+    original_hetatm = []
+    for l in original:
+        if ("HETATM" in l) and (not "REMARK" in l):
+            original_hetatm.append(l)
+    original_occs = [h[56:60] for h in original_hetatm]
+    print(len(original_occs))
+
+    with open(output_dir + pdb_to_be_restored, "r") as p:
+        pdb = p.readlines()
+    pdb_hetatm = []
+    n = 0
+    for i in range(len(pdb)):
+        if ("HETATM" in pdb[i]) and (not "REMARK" in pdb[i]):
+            print(i, n)
+            pdb[i] = pdb[i][:56] + original_occs[n] + pdb[i][60:]
+            n += 1
+
+    edited_pdb = original_pdb.removesuffix(".pdb") + "_restorehetatms.pdb"
+
+    with open(output_dir + edited_pdb, "w") as output:
+        output.write("".join(pdb))
+
+    return edited_pdb
+
+
 def _realspace_align_and_subtract(
     output_dir,
     fg_off,
     fg_on,
     pdboff,
     pdbon,
     on_name,
@@ -651,21 +829,78 @@
     print(f"{time.strftime('%H:%M:%S')}: Writing files...")
 
     write_maps = partial(
         rs.io.write_ccp4_map, cell=fg.unit_cell, spacegroup=fg.spacegroup
     )
 
     write_maps(fg.array, f"{output_dir}/{name}_{ncs_chains[0]}.map")
-    write_maps(fg2.array, f"{output_dir}/{name}_{ncs_chains[1]}.map")
+    write_maps(
+        fg2.array, f"{output_dir}/{name}_{ncs_chains[1]}_onto_{ncs_chains[0]}.map"
+    )
 
     write_maps(
         fg2.array - fg.array,
         f"{output_dir}/{name}_{ncs_chains[1]}_minus_{ncs_chains[0]}.map",
     )
 
     print(f"{time.strftime('%H:%M:%S')}: Done!")
 
     return
 
 
 def _quicknorm(array):
     return (array - array.mean()) / array.std()
+
+
+def _phaser_wrapper(
+    mtz,
+    pdb,
+    input_dir,
+    output_dir,
+    eff=None,
+    verbose=False,
+    ncopies=1,
+):
+    # confirm that phenix is active in the command-line environment
+    if shutil.which("phenix.phaser") is None:
+        raise OSError(
+            "Cannot find executable, phenix.phaser. Please set up your phenix environment."
+        )
+
+    # if eff is None:
+    #     eff_contents = """
+
+    # """
+    return
+
+
+def _find_available_dirname(prefix):
+    existing = glob.glob(f"{prefix}_[0-9]/")
+
+    if len(existing) == 0:
+        new_suffix = "0"
+    else:
+        n = max([int(s.split("_")[-1].removesuffix("/")) for s in existing])
+        new_suffix = f"{n+1}"
+
+    return new_suffix
+
+    # def _clean_up_files(output_dir, prefix, mode='vanilla'):
+    """
+    I know exactly what files are produced by the vanilla version:
+
+
+    """
+
+
+#     n = _find_available_dirname(prefix='matchmapsfiles')
+#     cleanup_dir = f"{output_dir}/matchmaps_{n}"
+
+#     os.makedirs(cleanup_dir)
+
+#     files_to_move = []
+
+
+#     # for suffix in ()
+#     files_to_move.append(glob.glob(output_dir + ))
+
+#     return
```

### Comparing `matchmaps-0.2.0/.gitignore` & `matchmaps-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `matchmaps-0.2.0/LICENSE` & `matchmaps-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmaps-0.2.0/README.md` & `matchmaps-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `matchmaps-0.2.0/pyproject.toml` & `matchmaps-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 homepage = "https://dennisbrookner.github.io/matchmaps/"
 repository = "https://github.com/dennisbrookner/matchmaps"
 
 # same as console_scripts entry point
 [project.scripts]
 matchmaps = "matchmaps._compute_realspace_diff:main"
 "matchmaps.ncs" = "matchmaps._compute_ncs_diff:main"
+"matchmaps.mr" = "matchmaps._compute_mr_diff:main"
 
 # Entry points
 # https://peps.python.org/pep-0621/#entry-points
 # [project.entry-points."spam.magical"]
 # tomatoes = "spam:main_tomatoes"
 
 # https://hatch.pypa.io/latest/config/metadata/
```

### Comparing `matchmaps-0.2.0/PKG-INFO` & `matchmaps-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmaps
-Version: 0.2.0
+Version: 0.3.0
 Summary: Make unbiased difference maps even for non-isomorphous inputs
 Project-URL: homepage, https://dennisbrookner.github.io/matchmaps/
 Project-URL: repository, https://github.com/dennisbrookner/matchmaps
 Author-email: Dennis Brookner <debrookner@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

