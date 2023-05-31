# Comparing `tmp/neuromllite-0.5.4.tar.gz` & `tmp/neuromllite-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuromllite-0.5.4.tar", last modified: Mon May 15 10:59:11 2023, max compression
+gzip compressed data, was "neuromllite-0.5.6.tar", last modified: Wed May 31 16:23:02 2023, max compression
```

## Comparing `neuromllite-0.5.4.tar` & `neuromllite-0.5.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:11.855770 neuromllite-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-15 10:59:01.000000 neuromllite-0.5.4/LICENSE.lesser
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-15 10:59:11.855770 neuromllite-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-05-15 10:59:01.000000 neuromllite-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:11.851770 neuromllite-0.5.4/neuromllite/
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/ArborHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/BBPConnectomeReader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/BindsNETHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/ConnectivityHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/DefaultNetworkHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    33672 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/GraphVizHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22883 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/MDFHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/MatrixHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    89346 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/NetworkGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/NeuronHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/PsyNeuLinkHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/PsyNeuLinkReader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/PyNNHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/SonataHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    51976 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/SonataReader.py
--rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:11.851770 neuromllite-0.5.4/neuromllite/gui/
--rw-r--r--   0 runner    (1001) docker     (123)    45481 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/gui/NMLliteUI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:11.855770 neuromllite-0.5.4/neuromllite/sweep/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/sweep/GenerateTests.py
--rw-r--r--   0 runner    (1001) docker     (123)    27090 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/sweep/ParameterSweep.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:11.851770 neuromllite-0.5.4/neuromllite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-15 10:59:11.000000 neuromllite-0.5.4/neuromllite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-15 10:59:11.000000 neuromllite-0.5.4/neuromllite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:59:11.000000 neuromllite-0.5.4/neuromllite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 10:59:11.000000 neuromllite-0.5.4/neuromllite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-15 10:59:11.000000 neuromllite-0.5.4/neuromllite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 10:59:11.000000 neuromllite-0.5.4/neuromllite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 10:59:11.855770 neuromllite-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-15 10:59:01.000000 neuromllite-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:23:02.567059 neuromllite-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-31 16:22:52.000000 neuromllite-0.5.6/LICENSE.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-31 16:23:02.567059 neuromllite-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-05-31 16:22:52.000000 neuromllite-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:23:02.567059 neuromllite-0.5.6/neuromllite/
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/ArborHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/BBPConnectomeReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/BindsNETHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/ConnectivityHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/DefaultNetworkHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33647 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/GraphVizHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/MDFHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/MatrixHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90154 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/NetworkGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/NeuronHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/PsyNeuLinkHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/PsyNeuLinkReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/PyNNHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/SonataHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51950 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/SonataReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:23:02.567059 neuromllite-0.5.6/neuromllite/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)    45579 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/gui/NMLliteUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:23:02.567059 neuromllite-0.5.6/neuromllite/sweep/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/sweep/GenerateTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27076 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/sweep/ParameterSweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-05-31 16:22:52.000000 neuromllite-0.5.6/neuromllite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:23:02.567059 neuromllite-0.5.6/neuromllite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-31 16:23:02.000000 neuromllite-0.5.6/neuromllite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-31 16:23:02.000000 neuromllite-0.5.6/neuromllite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:23:02.000000 neuromllite-0.5.6/neuromllite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 16:23:02.000000 neuromllite-0.5.6/neuromllite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 16:23:02.000000 neuromllite-0.5.6/neuromllite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 16:23:02.000000 neuromllite-0.5.6/neuromllite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 16:23:02.567059 neuromllite-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-31 16:22:52.000000 neuromllite-0.5.6/setup.py
```

### Comparing `neuromllite-0.5.4/LICENSE.lesser` & `neuromllite-0.5.6/LICENSE.lesser`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.4/PKG-INFO` & `neuromllite-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuromllite
-Version: 0.5.4
+Version: 0.5.6
 Summary: A common JSON/YAML based format for compact network specification, closely tied to NeuroML v2
 Home-page: https://github.com/NeuroML/NeuroMLlite
 Author: Padraig Gleeson
 Author-email: p.gleeson@gmail.com
 License: LICENSE.lesser
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `neuromllite-0.5.4/README.md` & `neuromllite-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.4/neuromllite/ArborHandler.py` & `neuromllite-0.5.6/neuromllite/ArborHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 import numpy as np
 
 import arbor
 
 
 class ArborHandler(DefaultNetworkHandler):
-
     pops_vs_components = {}
     proj_weights = {}
     proj_delays = {}
     input_info = {}
     input_lists = {}
 
     """
@@ -38,25 +37,23 @@
         self.nl_network = nl_network
         self.curr_gid = 0
 
     def handle_document_start(self, id, notes):
         print_v("Document: %s" % id)
 
     def handle_network(self, network_id, notes, temperature=None):
-
         print_v("Network: %s" % network_id)
         if temperature:
             print_v("  Temperature: " + temperature)
         if notes:
             print_v("  Notes: " + notes)
 
     def handle_population(
         self, population_id, component, size=-1, component_obj=None, properties={}
     ):
-
         sizeInfo = " as yet unspecified size"
         if size >= 0:
             sizeInfo = ", size: " + str(size) + " cells"
         if component_obj:
             compInfo = " (%s)" % component_obj.__class__.__name__
         else:
             compInfo = ""
@@ -103,15 +100,14 @@
         synapse,
         hasWeights=False,
         hasDelays=False,
         type="projection",
         synapse_obj=None,
         pre_synapse_obj=None,
     ):
-
         synInfo = ""
         if synapse_obj:
             synInfo += " (syn: %s)" % synapse_obj.__class__.__name__
 
         if pre_synapse_obj:
             synInfo += " (pre comp: %s)" % pre_synapse_obj.__class__.__name__
 
@@ -160,15 +156,14 @@
         preSegId=0,
         preFract=0.5,
         postSegId=0,
         postFract=0.5,
         delay=0,
         weight=1,
     ):
-
         self.print_connection_information(
             projName, id, prePop, postPop, synapseType, preCellId, postCellId, weight
         )
         print_v(
             "Src cell: %d, seg: %f, fract: %f -> Tgt cell %d, seg: %f, fract: %f; weight %s, delay: %s ms"
             % (
                 preCellId,
@@ -187,15 +182,14 @@
 
     #
     #  Should be overridden to handle end of network connection
     #
     def finalise_projection(
         self, projName, prePop, postPop, synapse=None, type="projection"
     ):
-
         print_v(
             "Projection finalising: "
             + projName
             + " from "
             + prePop
             + " to "
             + postPop
@@ -204,15 +198,14 @@
 
     #
     #  Should be overridden to create input source array
     #
     def handle_input_list(
         self, inputListId, population_id, component, size, input_comp_obj=None
     ):
-
         self.print_input_information(inputListId, population_id, component, size)
         if input_comp_obj:
             print("Input comp: %s" % input_comp_obj)
 
         if size < 0:
             self.log.error(
                 "Error! Need a size attribute in sites element to create spike source!"
@@ -224,15 +217,14 @@
 
     #
     #  Should be overridden to to connect each input to the target cell
     #
     def handle_single_input(
         self, inputListId, id, cellId, segId=0, fract=0.5, weight=1
     ):
-
         population_id, component, input_comp_obj = self.input_info[inputListId]
 
         print_v(
             "Input: %s[%s] (%s), pop: %s, cellId: %i, seg: %i, fract: %f, weight: %f"
             % (inputListId, id, component, population_id, cellId, segId, fract, weight)
         )
         self.input_lists[inputListId].append((cellId, segId, fract, weight))
@@ -257,16 +249,14 @@
             self.proj_weights,
             self.proj_delays,
             self.input_info,
             self.input_lists,
         )
 
 
-
-
 # Create a NeuroML recipe
 class NeuroML_Arbor_Recipe(arbor.recipe):
     def __init__(
         self,
         nl_network,
         pop_indices_vs_gids,
         pops_vs_components,
@@ -285,19 +275,16 @@
         self.pops_vs_components = pops_vs_components
         self.nl_network = nl_network
         self.proj_weights = proj_weights
         self.proj_delays = proj_delays
         self.input_info = input_info
         self.input_lists = input_lists
 
-
     def create_arbor_cell(self, cell, gid, pop_id, index):
-
         if cell.arbor_cell == "cable_cell":
-
             default_tree = arbor.segment_tree()
             radius = (
                 evaluate(cell.parameters["radius"], self.nl_network.parameters)
                 if "radius" in cell.parameters
                 else 3
             )
 
@@ -319,37 +306,42 @@
                 if "v_init" in cell.parameters
                 else -70
             )
             decor.set_property(Vm=v_init)
 
             decor.paint('"soma"', arbor.density(cell.parameters["mechanism"]))
 
-            decor.place('"center"', arbor.spike_detector(0), "detector")
+            decor.place('"center"', arbor.threshold_detector(0), "detector")
 
             for ip in self.input_info:
                 if self.input_info[ip][0] == pop_id:
-                    print_v("Stim: %s (%s) being placed on %s" % (ip,self.input_info[ip],pop_id))
+                    print_v(
+                        "Stim: %s (%s) being placed on %s"
+                        % (ip, self.input_info[ip], pop_id)
+                    )
                     for il in self.input_lists[ip]:
                         cellId, segId, fract, weight = il
                         if cellId == index:
-                            if self.input_info[ip][1] == 'i_clamp': # TODO: remove hardcoding of this...
+                            if (
+                                self.input_info[ip][1] == "i_clamp"
+                            ):  # TODO: remove hardcoding of this...
                                 ic = arbor.iclamp(
                                     self.nl_network.parameters["input_del"],
                                     self.nl_network.parameters["input_dur"],
                                     self.nl_network.parameters["input_amp"],
                                 )
-                                print_v("Stim: %s on %s" % (ic,gid))
+                                print_v("Stim: %s on %s" % (ic, gid))
                                 decor.place('"center"', ic, "iclamp")
 
             # (2) Mark location for synapse at the midpoint of branch 1 (the first dendrite).
             labels["synapse_site"] = "(location 0 0.5)"
             # (4) Attach a single synapse.
             decor.place('"synapse_site"', arbor.synapse("expsyn"), "syn")
 
-            default_cell = arbor.cable_cell(default_tree, labels, decor)
+            default_cell = arbor.cable_cell(default_tree, labels=labels, decor=decor)
 
             print_v("Created a new cell for gid %i: %s" % (gid, cell))
             print_v("%s" % (default_cell))
 
             return default_cell
 
     def get_pop_index(self, gid):
@@ -380,15 +372,14 @@
         comp = self.pops_vs_components[pop_id]
 
         a_cell = self.create_arbor_cell(
             self.nl_network.get_child(comp, "cells"), gid, pop_id, index
         )
         return a_cell
 
-
     # The kind method returns the type of cell with gid.
     # Note: this must agree with the type returned by cell_description.
     def cell_kind(self, gid):
         cell_kind = arbor.cell_kind.cable
         print_v("Getting cell_kind: %s" % (cell_kind))
         return cell_kind
 
@@ -448,18 +439,18 @@
 
         print_v("num_sources for %i: %s" % (gid, tot_out))
         return 1
 
     # (9) Attach a generator to the first cell in the ring.
     def event_generators(self, gid):
         egs = []
-        '''
+        """
         if gid == 0:
             sched = arbor.explicit_schedule([1])
-            egs = [arbor.event_generator("syn", 0.1, sched)]'''
+            egs = [arbor.event_generator("syn", 0.1, sched)]"""
 
         print_v("Getting event_generators for %s: %s" % (gid, egs))
         return egs
 
     # (10) Place a probe at the root of each cell.
     def probes(self, gid):
         return [arbor.cable_probe_membrane_voltage('"root"')]
```

### Comparing `neuromllite-0.5.4/neuromllite/BBPConnectomeReader.py` & `neuromllite-0.5.6/neuromllite/BBPConnectomeReader.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,24 @@
 from neuroml.hdf5.NetworkContainer import *
 from neuromllite import NetworkReaderX
 
 from neuromllite.utils import print_v
 
 
 class BBPConnectomeReader(NetworkReaderX):
-
     component_objects = {}  # Store cell ids vs objects, e.g. NeuroML2 based object
 
     def __init__(self, **parameters):
-
         print_v("Creating BBPConnectomeReader with %s..." % parameters)
         self.parameters = parameters
         self.current_population = None
         self.pre_pop = None
         self.post_pop = None
 
     def parse(self, handler):
-
         filename = os.path.abspath(self.parameters["filename"])
         id = filename.split("/")[-1].split(".")[0]
 
         if "id" in self.parameters:
             id = self.parameters["id"]
 
         self.handler = handler
@@ -83,15 +80,14 @@
             return True
 
     def parse_dataset(self, d):
         # print_v("Parsing dataset/array: "+ str(d))
 
         # Population
         if self.current_population and d.name == "locations":
-
             perc_cells = (
                 self.parameters["percentage_cells_per_pop"]
                 if "percentage_cells_per_pop" in self.parameters
                 else 100
             )
             if perc_cells > 100:
                 perc_cells = 100
@@ -176,15 +172,14 @@
                     properties=properties,
                 )
 
                 print_v(
                     "   There are %i cells in: %s" % (size, self.current_population)
                 )
                 for i in range(0, d.shape[0]):
-
                     if i < size:
                         row = d[i, :]
                         x = row[0]
                         y = row[1]
                         z = row[2]
                         self.pop_locations[self.current_population][i] = (x, y, z)
                         self.handler.handle_location(
@@ -194,15 +189,14 @@
                             x,
                             y,
                             z,
                         )
 
         # Projection
         elif self.pre_pop != None and self.post_pop != None:
-
             proj_id = "Proj__%s__%s" % (self.pre_pop, self.post_pop)
             synapse = "gaba"
             if (
                 "PC" in self.pre_pop or "SS" in self.pre_pop
             ):  # TODO: better choice between E/I cells
                 synapse = "ampa"
 
@@ -259,15 +253,14 @@
                         proj_id, self.pre_pop, self.post_pop, synapse
                     )
 
             self.post_pop = None
 
 
 if __name__ == "__main__":
-
     filename = "test_files/cons_locs_pathways_mc0_Column.h5"
 
     percentage_cells_per_pop = 1
 
     bbp = BBPConnectomeReader(
         filename=filename,
         percentage_cells_per_pop=percentage_cells_per_pop,
```

### Comparing `neuromllite-0.5.4/neuromllite/BindsNETHandler.py` & `neuromllite-0.5.6/neuromllite/BindsNETHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 import numpy as np
 
 import bindsnet
 
 
 class BindsNETHandler(DefaultNetworkHandler):
-
     pops_vs_components = {}
     pops_vs_bn_layers = {}
 
     proj_weights = {}
     proj_delays = {}
 
     input_info = {}
@@ -42,25 +41,23 @@
 
         self.bn_network = bindsnet.network.Network(dt=1.0)
 
     def handle_document_start(self, id, notes):
         print_v("Document: %s" % id)
 
     def handle_network(self, network_id, notes, temperature=None):
-
         print_v("Network: %s" % network_id)
         if temperature:
             print_v("  Temperature: " + temperature)
         if notes:
             print_v("  Notes: " + notes)
 
     def handle_population(
         self, population_id, component, size=-1, component_obj=None, properties={}
     ):
-
         sizeInfo = " as yet unspecified size"
         if size >= 0:
             sizeInfo = ", size: " + str(size) + " cells"
         if component_obj:
             compInfo = " (%s)" % component_obj.__class__.__name__
         else:
             compInfo = ""
@@ -99,15 +96,14 @@
         synapse,
         hasWeights=False,
         hasDelays=False,
         type="projection",
         synapse_obj=None,
         pre_synapse_obj=None,
     ):
-
         synInfo = ""
         if synapse_obj:
             synInfo += " (syn: %s)" % synapse_obj.__class__.__name__
 
         if pre_synapse_obj:
             synInfo += " (pre comp: %s)" % pre_synapse_obj.__class__.__name__
 
@@ -156,15 +152,14 @@
         preSegId=0,
         preFract=0.5,
         postSegId=0,
         postFract=0.5,
         delay=0,
         weight=1,
     ):
-
         self.print_connection_information(
             projName, id, prePop, postPop, synapseType, preCellId, postCellId, weight
         )
         print_v(
             "Src cell: %d, seg: %f, fract: %f -> Tgt cell %d, seg: %f, fract: %f; weight %s, delay: %s ms"
             % (
                 preCellId,
@@ -183,15 +178,14 @@
 
     #
     #  Should be overridden to handle end of network connection
     #
     def finalise_projection(
         self, projName, prePop, postPop, synapse=None, type="projection"
     ):
-
         print_v(
             "Projection finalising: "
             + projName
             + " from "
             + prePop
             + " to "
             + postPop
@@ -200,15 +194,14 @@
 
     #
     #  Should be overridden to create input source array
     #
     def handle_input_list(
         self, inputListId, population_id, component, size, input_comp_obj=None
     ):
-
         self.print_input_information(inputListId, population_id, component, size)
         if input_comp_obj:
             print("Input comp: %s" % input_comp_obj)
 
         if size < 0:
             self.log.error(
                 "Error! Need a size attribute in sites element to create spike source!"
@@ -219,15 +212,14 @@
 
     #
     #  Should be overridden to to connect each input to the target cell
     #
     def handle_single_input(
         self, inputListId, id, cellId, segId=0, fract=0.5, weight=1
     ):
-
         population_id, component = self.input_info[inputListId]
 
         print_v(
             "Input: %s[%s] (%s), pop: %s, cellId: %i, seg: %i, fract: %f, weight: %f"
             % (inputListId, id, component, population_id, cellId, segId, fract, weight)
         )
```

### Comparing `neuromllite-0.5.4/neuromllite/ConnectivityHandler.py` & `neuromllite-0.5.6/neuromllite/ConnectivityHandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from neuromllite.utils import print_v
 from neuromllite.DefaultNetworkHandler import DefaultNetworkHandler
 from pyneuroml.pynml import convert_to_units
 
 
 class ConnectivityHandler(DefaultNetworkHandler):
-
     CUTOFF_INH_SYN_MV = -50  # erev below -50mV => inhibitory, above => excitatory
 
     include_ext_inputs = False
 
     positions = {}
 
     pop_sizes = {}
@@ -40,19 +39,17 @@
 
     sizes_ils = {}
     pops_ils = {}
     weights_ils = {}
     input_comp_obj_ils = {}
 
     def handle_document_start(self, id, notes):
-
         print_v("Document: %s" % id)
 
     def handle_network(self, network_id, notes, temperature=None):
-
         print_v("Network: %s" % network_id)
         self.network_id = network_id
 
     # Nice clean number for use in graphs, labels etc.
     def format_float(self, f, d=3, approx=False):
         if int(f) == f:
             return int(f)
@@ -84,26 +81,24 @@
     def get_size_pre_pop(self, projName):
         return self.pop_sizes[self.proj_pre_pops[projName]]
 
     def get_size_post_pop(self, projName):
         return self.pop_sizes[self.proj_post_pops[projName]]
 
     def get_reversal_potential_mV(self, synapse_obj):
-
         if hasattr(synapse_obj, "erev"):
             return convert_to_units(synapse_obj.erev, "mV")
 
         elif hasattr(synapse_obj, "e_rev"):  # PyNN, no units, in mV
             return float(synapse_obj.e_rev)
 
         else:
             return None
 
     def _get_gbase_nS(self, projName, return_orig_string_also=False):
-
         gbase_nS = None
         gbase = "???"
         # print('Getting gbase for %s'%projName)
         if projName in self.proj_syn_objs:
             syn = self.proj_syn_objs[projName]
             if hasattr(syn, "gbase"):
                 gbase = syn.gbase
@@ -119,30 +114,28 @@
 
         if return_orig_string_also:
             return gbase_nS, gbase
 
         return gbase_nS
 
     def _scale_individual_weight(self, weight, projName):
-
         orig_weight = weight
 
         if self.scale_by_post_pop_cond:
             gbase_nS = self._get_gbase_nS(projName)
             if gbase_nS != None:
                 weight *= gbase_nS
 
         if not orig_weight == weight:
             # print(' - Weight for %s modified %s->%s'%(projName, orig_weight, weight))
             pass
 
         return weight
 
     def _scale_population_weight(self, weight, projName):
-
         orig_weight = weight
         if self.scale_by_post_pop_size:
             weight /= self.get_size_post_pop(projName)
 
         if self.scale_by_post_pop_cond:
             gbase_nS = self._get_gbase_nS(projName)
             if gbase_nS != None:
@@ -151,15 +144,14 @@
         if not orig_weight == weight:
             # print(' - Weight for %s modified %s->%s'%(projName, orig_weight, weight))
             pass
 
         return weight
 
     def handle_location(self, id, population_id, component, x, y, z):
-
         pass
 
     def handle_connection(
         self,
         projName,
         id,
         prePop,
@@ -170,15 +162,14 @@
         preSegId=0,
         preFract=0.5,
         postSegId=0,
         postFract=0.5,
         delay=0,
         weight=1.0,
     ):
-
         # print_v(" - Connection for %s, cell %i -> %i, w: %s"%(projName, preCellId, postCellId, weight))
         self.proj_conns[projName] += 1
         self.proj_tot_weight[projName] += weight
         if self.is_cell_level():
             self.proj_individual_weights[projName][preCellId][postCellId] += weight
             self.proj_individual_scaled_weights[projName][preCellId][
                 postCellId
@@ -190,15 +181,14 @@
                        self.proj_individual_scaled_weights[projName][preCellId][postCellId],
                        self.proj_individual_conn_numbers[projName][preCellId][postCellId]))"""
             self.proj_delays[projName][preCellId][postCellId] = delay
 
     def finalise_projection(
         self, projName, prePop, postPop, synapse=None, type="projection"
     ):
-
         # weight = self.proj_tot_weight[projName]
         # self.max_weight = max(self.max_weight, weight)
         # self.min_weight = min(self.min_weight, weight)
         # print_v("Now weights range %s->%s"%(self.min_weight, self.max_weight))
         pass
         # print_v("Projection finalising: "+projName+" from "+prePop+" to "+postPop+" completed")
```

### Comparing `neuromllite-0.5.4/neuromllite/DefaultNetworkHandler.py` & `neuromllite-0.5.6/neuromllite/DefaultNetworkHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 #
 #
 
 from neuromllite.utils import print_v
 
 
 class DefaultNetworkHandler:
-
     #
     #  Internal info method, can be reused in overriding classes for debugging
     #
     def print_location_information(self, id, population_id, component, x, y, z):
         position = "(%s, %s, %s)" % (x, y, z)
         print_v(
             "  Location "
@@ -78,31 +77,28 @@
             + component
         )
 
     #
     #  Should be overridden
     #
     def handle_document_start(self, id, notes):
-
         print_v("Document: %s started..." % id)
         if notes:
             print_v("  Notes: " + notes)
 
     #
     #  Should be overridden
     #
     def finalise_document(self):
-
         print_v("Document ended...")
 
     #
     #  Should be overridden to create network
     #
     def handle_network(self, network_id, notes, temperature=None):
-
         print_v("Network: %s" % network_id)
         if temperature:
             print_v("  Temperature: " + temperature)
         if notes:
             print_v("  Notes: " + notes)
 
     #
@@ -135,15 +131,14 @@
     #
     #  Should be overridden to create specific cell instance
     #
     def handle_location(self, id, population_id, component, x, y, z):
         self.print_location_information(id, population_id, component, x, y, z)
 
     def finalise_population(self, population_id):
-
         pass
 
     #
     #  Should be overridden to create population array
     #
     def handle_projection(
         self,
@@ -153,15 +148,14 @@
         synapse,
         hasWeights=False,
         hasDelays=False,
         type="projection",
         synapse_obj=None,
         pre_synapse_obj=None,
     ):
-
         synInfo = ""
         if synapse_obj:
             synInfo += " (syn: %s)" % synapse_obj.__class__.__name__
 
         if pre_synapse_obj:
             synInfo += " (pre comp: %s)" % pre_synapse_obj.__class__.__name__
 
@@ -194,15 +188,14 @@
         preSegId=0,
         preFract=0.5,
         postSegId=0,
         postFract=0.5,
         delay=0,
         weight=1,
     ):
-
         self.print_connection_information(
             projName, id, prePop, postPop, synapseType, preCellId, postCellId, weight
         )
         if preSegId != 0 or postSegId != 0 or preFract != 0.5 or postFract != 0.5:
             print_v(
                 "Src cell: %d, seg: %f, fract: %f -> Tgt cell %d, seg: %f, fract: %f; weight %s, delay: %s ms"
                 % (
@@ -219,15 +212,14 @@
 
     #
     #  Should be overridden to handle end of network connection
     #
     def finalise_projection(
         self, projName, prePop, postPop, synapse=None, type="projection"
     ):
-
         print_v(
             "Projection: "
             + projName
             + " from "
             + prePop
             + " to "
             + postPop
@@ -236,30 +228,28 @@
 
     #
     #  Should be overridden to create input source array
     #
     def handle_input_list(
         self, inputListId, population_id, component, size, input_comp_obj=None
     ):
-
         self.print_input_information(inputListId, population_id, component, size)
 
         if size < 0:
             self.log.error(
                 "Error! Need a size attribute in sites element to create spike source!"
             )
             return
 
     #
     #  Should be overridden to to connect each input to the target cell
     #
     def handle_single_input(
         self, inputListId, id, cellId, segId=0, fract=0.5, weight=1
     ):
-
         print_v(
             "  Input: %s[%s], cellId: %i, seg: %i, fract: %f, weight: %f"
             % (inputListId, id, cellId, segId, fract, weight)
         )
 
     #
     #  Should be overridden to to connect each input to the target cell
```

### Comparing `neuromllite-0.5.4/neuromllite/GraphVizHandler.py` & `neuromllite-0.5.6/neuromllite/GraphVizHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     "f": "fdp",
     "s": "sfdp",
     "p": "patchwork",
 }
 
 
 class GraphVizHandler(ConnectivityHandler):
-
     DEFAULT_POP_SHAPE = "ellipse"
     EXC_POP_SHAPE = "ellipse"
     INH_POP_SHAPE = "ellipse"
 
     EXC_CONN_ARROW_SHAPE = "normal"
     INH_CONN_ARROW_SHAPE = "dot"
     GAP_CONN_ARROW_SHAPE = "tee"
@@ -50,15 +49,14 @@
         show_chem_conns=True,
         show_elect_conns=True,
         show_cont_conns=True,
         min_weight_to_show=0,
         output_format="png",
         view_on_render=True,
     ):
-
         self.nl_network = nl_network
         self.level = level
         self.engine = engine
         self.include_ext_inputs = include_ext_inputs
         self.include_input_pops = include_input_pops
         self.scale_by_post_pop_size = scale_by_post_pop_size
         self.scale_by_post_pop_cond = scale_by_post_pop_cond
@@ -102,15 +100,14 @@
                 ["%s:\t %s" % (k, self.syn_conds_used[k]) for k in syns]
             )
         )
         print_v("*")
         print_v("**************************************")
 
     def get_weight_fraction_and_line(self, w, max_w, min_w):
-
         if max_w == min_w:
             return 1.0, 1.0
         # fractional weight, 0->1
         fweight = (abs(w) - min_w) / (max_w - min_w)
         if fweight < 0:
             fweight = 0
         if fweight > 1:
@@ -118,44 +115,41 @@
 
         # Good weight for line based on fraction
         lweight = 0.7 + fweight * 3.5
 
         return fweight, lweight
 
     def finalise_document(self):
-
         max_abs_weight = {}
         min_abs_weight = {}
 
         for t in [
             "projection",
             "inhibitory",
             "excitatory",
             "electricalProjection",
             "continuousProjection",
         ]:
             max_abs_weight[t] = -1e100
             min_abs_weight[t] = 1e100
 
         if self.is_cell_level() and self.level <= -1:
-
             for projName in self.proj_weights:
                 # ws = self.proj_individual_weights[projName]
                 ws = self.proj_individual_scaled_weights[projName]
                 t = self.proj_types[projName]
                 if np.max(ws) > 0:
                     max_abs_weight[t] = max(
                         max_abs_weight[t], np.max(ws[np.nonzero(ws)])
                     )
                     min_abs_weight[t] = min(
                         min_abs_weight[t], np.min(ws[np.nonzero(ws)])
                     )
 
             for projName in self.proj_weights:
-
                 pre_pop = self.proj_pre_pops[projName]
                 post_pop = self.proj_post_pops[projName]
                 proj_type = self.proj_types[projName]
                 num_pre = self.get_size_pre_pop(projName)
                 num_post = self.get_size_post_pop(projName)
 
                 if self.proj_types[projName] == "electricalProjection":
@@ -205,15 +199,14 @@
                             ]
 
                             num_indiv_conns = self.proj_individual_conn_numbers[
                                 projName
                             ][pre_i][post_i]
 
                             if w != 0:
-
                                 weight_used = w
 
                                 cond_scale = None
                                 if self.scale_by_post_pop_cond:
                                     cond_scale = gbase_nS if gbase_nS != None else 1.0
 
                                 print_v(
@@ -275,25 +268,22 @@
                                     label += ">"
                                 if self.level <= -2:
                                     self.graph.edge(pre_pop_i, post_pop_i, label=label)
                                 else:
                                     self.graph.edge(pre_pop_i, post_pop_i)
 
         else:
-
             for projName in self.proj_tot_weight:
                 t = self.proj_types[projName]
 
                 if self.proj_tot_weight[projName] != 0:
-
                     weight_used = float(self.proj_tot_weight[projName])
                     weight_used = self._scale_population_weight(weight_used, projName)
 
                     if abs(weight_used) >= self.min_weight_to_show:
-
                         max_abs_weight[t] = max(max_abs_weight[t], abs(weight_used))
                         min_abs_weight[t] = min(min_abs_weight[t], abs(weight_used))
                         print_v(
                             "EDGE: %s (%s): weight %s (all so far: %s -> %s)"
                             % (
                                 projName,
                                 t,
@@ -312,25 +302,22 @@
                                 self.min_weight_to_show,
                                 max_abs_weight[t],
                                 min_abs_weight[t],
                             )
                         )
 
             for projName in self.proj_tot_weight:
-
                 proj_type = self.proj_types[projName]
 
                 if self.proj_tot_weight[projName] != 0:
-
                     # weight_used = self.proj_weights[projName]
                     weight_used = float(self.proj_tot_weight[projName])
                     weight_used = self._scale_population_weight(weight_used, projName)
 
                     if abs(weight_used) >= self.min_weight_to_show:
-
                         if max_abs_weight[proj_type] == min_abs_weight[proj_type]:
                             fweight = 1
                             lweight = 1
                         elif self.proj_types[projName] == "electricalProjection":
                             # Dotted lines look bad when thick...
                             fweight = 1
                             lweight = 1
@@ -411,17 +398,15 @@
 
                                 if self.proj_conns[projName] > 0:
                                     label += (
                                         "%s conns<br/> " % self.proj_conns[projName]
                                     )
 
                                 if self.level >= 5:
-
                                     if self.proj_conns[projName] > 0:
-
                                         pre_avg = (
                                             float(self.proj_conns[projName])
                                             / self.pop_sizes[
                                                 self.proj_pre_pops[projName]
                                             ]
                                         )
                                         post_avg = (
@@ -486,15 +471,14 @@
                 "Finished generating graph with params: %s"
                 % [p for p in self.nl_network.parameters]
                 if self.nl_network.parameters is not None
                 else "[]"
             )
 
     def handle_network(self, network_id, notes, temperature=None):
-
         print_v("Network: %s" % network_id)
         self.network_id = network_id
 
         self.graph = Digraph(
             network_id,
             filename="%s.gv" % network_id,
             engine=self.engine,
@@ -566,15 +550,14 @@
 
         self.pop_colors[population_id] = color
 
         label = "<%s" % population_id
         if self.level >= 3:
             label += "<br/><i>%s cell%s</i>" % (size, "" if size == 1 else "s")
         if self.level >= 4:
-
             from neuroml import SpikeSourcePoisson
 
             if component_obj and isinstance(component_obj, SpikeSourcePoisson):
                 start = convert_to_units(component_obj.start, "ms")
                 if start == int(start):
                     start = int(start)
                 duration = convert_to_units(component_obj.duration, "ms")
@@ -588,15 +571,14 @@
 
             else:
                 label += "<br/>%s" % (component)
 
         label += ">"
 
         if properties and "region" in properties:
-
             with self.graph.subgraph(name="cluster_%s" % properties["region"]) as c:
                 c.attr(color="#444444", fontcolor="#444444")
                 c.attr(label=properties["region"])
                 c.attr(
                     "node", color=color, style="filled", fontcolor=fcolor, shape=shape
                 )
 
@@ -627,15 +609,14 @@
         synapse,
         hasWeights=False,
         hasDelays=False,
         type="projection",
         synapse_obj=None,
         pre_synapse_obj=None,
     ):
-
         shape = self.EXC_CONN_ARROW_SHAPE
         line = "solid"
 
         # Could be used in a network with no explicit connections, but weight
         # between populations set at high level projection element in NeuroMLlite
         projection_weight = 1.0
 
@@ -702,36 +683,32 @@
                 (pre_size, post_size)
             )
             self.proj_delays[projName] = np.zeros((pre_size, post_size))
 
     def finalise_projection(
         self, projName, prePop, postPop, synapse=None, type="projection"
     ):
-
         # weight = self.proj_tot_weight[projName]
         # self.max_weight = max(self.max_weight, weight)
         # self.min_weight = min(self.min_weight, weight)
         # print_v("Now weights range %s->%s"%(self.min_weight, self.max_weight))
         pass
         # print_v("Projection finalising: "+projName+" from "+prePop+" to "+postPop+" completed")
 
     def finalise_input_source(self, inputListId):
-
         if self.include_ext_inputs:
             # self.print_input_information('FINAL: '+inputListId, self.pops_ils[inputListId], '...', self.sizes_ils[inputListId])
 
             if self.level >= 2:
-
                 label = "<%s" % inputListId
                 if self.level >= 3:
                     size = self.sizes_ils[inputListId]
                     label += "<br/><i>%s input%s</i>" % (size, "" if size == 1 else "s")
 
                 if self.level >= 4:
-
                     from neuroml import PulseGenerator
                     from neuroml import TransientPoissonFiringSynapse
                     from neuroml import PoissonFiringSynapse
                     from pyneuroml.pynml import convert_to_units
 
                     input_comp_obj = self.input_comp_obj_ils[inputListId]
 
@@ -751,30 +728,28 @@
                             start + duration,
                             amplitude,
                         )
 
                     if input_comp_obj and isinstance(
                         input_comp_obj, PoissonFiringSynapse
                     ):
-
                         average_rate = convert_to_units(
                             input_comp_obj.average_rate, "Hz"
                         )
                         if average_rate == int(average_rate):
                             average_rate = int(average_rate)
 
                         label += "<br/>Syn: %s @ %sHz" % (
                             input_comp_obj.synapse,
                             average_rate,
                         )
 
                     if input_comp_obj and isinstance(
                         input_comp_obj, TransientPoissonFiringSynapse
                     ):
-
                         start = convert_to_units(input_comp_obj.delay, "ms")
                         if start == int(start):
                             start = int(start)
                         duration = convert_to_units(input_comp_obj.duration, "ms")
                         if duration == int(duration):
                             duration = int(duration)
                         average_rate = convert_to_units(
```

### Comparing `neuromllite-0.5.4/neuromllite/MDFHandler.py` & `neuromllite-0.5.6/neuromllite/MDFHandler.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 from modelspec.utils import evaluate
 from pyneuroml.pynml import get_value_in_si
 
 import lems.api as lems  # from pylems
 
 import numpy
 
+DEFAULT_CURRENT_INPUT_PORT = "synapses_i"
+SPIKE_INPUT_PORT_ID = 'spike_input'
+WEIGHTED_SPIKE_INPUTS = 'weighted_inputs'
 
 class MDFHandler(DefaultNetworkHandler):
 
     def __init__(self, nl_network):
         print_v("Initiating MDF handler")
         self.nl_network = nl_network
 
         self.input_list_vs_comps = {}
         self.input_list_vs_pops = {}
 
-    def handle_document_start(self, id, notes):
+        self.pop_ids_vs_size = {}
 
+    def handle_document_start(self, id, notes):
         print_v("Parsing for MDF export: %s" % id)
         self.id = id
 
         self.mdf_info = {}
 
         # from modeci_mdf import MODECI_MDF_VERSION
         MODECI_MDF_VERSION = "0.4"
@@ -41,23 +45,21 @@
         self.mdf_info[self.id] = {}
         self.mdf_info[self.id]["format"] = "ModECI MDF v%s" % MODECI_MDF_VERSION
         self.mdf_info[self.id]["graphs"] = {}
 
         self.pnl_additions = False
 
     def finalise_document(self):
-
         print_v("Writing file for...: %s" % self.id)
 
         save_to_json_file(self.mdf_info, "%s.mdf.json" % self.id, indent=4)
         save_to_yaml_file(self.mdf_info, "%s.mdf.yaml" % self.id, indent=4)
         """save_to_json_file(self.mdf_info_hl, '%s.bids-mdf.highlevel.json'%self.id, indent=4)"""
 
     def handle_network(self, network_id, notes, temperature=None):
-
         print_v("Network: %s" % network_id)
         self.network_id = network_id
 
         if temperature:
             print_v("  Temperature: " + temperature)
         if notes:
             print_v("  Notes: " + notes)
@@ -65,352 +67,478 @@
         self.mdf_graph = {}
         self.mdf_graph["notes"] = notes
         self.mdf_graph["nodes"] = {}
         self.mdf_graph["edges"] = {}
 
         self.mdf_info[self.id]["graphs"][network_id] = self.mdf_graph
 
-    def _convert_value(self, val):
 
+    def _get_input_port_name(self, name):
+        if name=='in': return SPIKE_INPUT_PORT_ID
+        else: return name
+        
+
+    def _convert_value(self, val):
         funcs = ["exp"]
         for f in funcs:
             if "%s(" % f in val:
-                val = val.replace("%s(" % f, "math.%s(" % f)
+                val = val.replace("%s(" % f, "numpy.%s(" % f)
 
         val = evaluate(val)  # catch if it's an int etc.
         return val
 
     def handle_population(
         self, population_id, component, size=-1, component_obj=None, properties={}
     ):
-
         sizeInfo = " as yet unspecified size"
         if size >= 0:
             sizeInfo = ", size: " + str(size) + " cells"
         if component_obj:
             compInfo = " (%s)" % component_obj.__class__.__name__
         else:
             compInfo = ""
 
-        info = "Population: " + population_id + ", component: " + component + compInfo + sizeInfo + ", properties: %s"% properties
+        self.pop_ids_vs_size[population_id] = size
+
+        info = (
+            "Population: "
+            + population_id
+            + ", component: "
+            + component
+            + compInfo
+            + sizeInfo
+            + ", properties: %s" % properties
+        )
+        print_v("  = %s"%info)
 
         node_id = "%s" % (population_id)
 
         cell_comp = self.nl_network.get_child(component, "cells")
 
         if cell_comp is not None:
-            node = self._comp_to_mdf_node(cell_comp, component, node_id, size, properties)
+            node = self._comp_to_mdf_node(
+                nmllite_comp=cell_comp,
+                lems_comp_id=component,
+                size=size,
+                properties=properties,
+            )
 
         self.mdf_graph["nodes"][node_id] = node
 
 
-    def _comp_to_mdf_node(self, nmllite_comp, lems_comp_id, node, pop_size, properties=None):
+    def _comp_to_mdf_node(self, nmllite_comp, lems_comp_id, size=1, properties=None):
+        base_dir = "./"  # for now...
 
-       base_dir = "./"  # for now...
+        node = {}
 
-       node = {}
-       if properties:
-           node["metadata"] = properties
-
-       node["parameters"] = {}
-       node["input_ports"] = {}
-       node["output_ports"] = {}
-
-       if nmllite_comp.lems_source_file:
-           print_v("  It's defined in custom lems..." )
-           fname = locate_file(nmllite_comp.lems_source_file, base_dir)
-           model = MDFHandler._load_lems_file_with_neuroml2_types(fname)
-           lems_comp = model.components.get(lems_comp_id)
-
-       elif hasattr(nmllite_comp,'neuroml2_cell') and nmllite_comp.neuroml2_cell is not None:
-           print_v("  It is a NeuroML2 cell (%s, %s)..." %(nmllite_comp.id, nmllite_comp.neuroml2_cell))
-           model = MDFHandler._get_lems_model_with_neuroml2_types()
-           lems_comp = lems.Component(
-               id_=nmllite_comp.id, type_=nmllite_comp.neuroml2_cell
-           )
-           if nmllite_comp.parameters is not None: 
+        if properties:
+            node["metadata"] = properties
+
+        node["parameters"] = {}
+        node["input_ports"] = {}
+        node["output_ports"] = {}
+
+        if nmllite_comp.lems_source_file:
+            print_v("  It's a component defined in custom lems...")
+            fname = locate_file(nmllite_comp.lems_source_file, base_dir)
+            model = MDFHandler._load_lems_file_with_neuroml2_types(fname)
+            lems_comp = model.components.get(lems_comp_id)
+
+        elif (
+            hasattr(nmllite_comp, "neuroml2_cell")
+            and nmllite_comp.neuroml2_cell is not None
+        ):
+            print_v(
+                "  It is a NeuroML2 cell (%s, %s)..."
+                % (nmllite_comp.id, nmllite_comp.neuroml2_cell)
+            )
+            model = MDFHandler._get_lems_model_with_neuroml2_types()
+            lems_comp = lems.Component(
+                id_=nmllite_comp.id, type_=nmllite_comp.neuroml2_cell
+            )
+            if nmllite_comp.parameters is not None:
                 for p in nmllite_comp.parameters:
                     lems_comp.set_parameter(
                         p,
                         evaluate(
                             nmllite_comp.parameters[p], self.nl_network.parameters
                         ),
                     )
-       elif nmllite_comp.neuroml2_source_file is not None:
-           print_v("  It is a NeuroML2 cell (%s, %s)..." %(nmllite_comp.id, nmllite_comp.neuroml2_source_file))
-           model = MDFHandler._get_lems_model_with_neuroml2_types()
-           lems_comp = lems.Component(
-               id_=nmllite_comp.id, type_=nmllite_comp.neuroml2_cell
-           )
-           if nmllite_comp.parameters is not None: 
+        elif nmllite_comp.neuroml2_source_file is not None:
+            print_v(
+                "  It is a NeuroML2 cell (%s, %s)..."
+                % (nmllite_comp.id, nmllite_comp.neuroml2_source_file)
+            )
+            model = MDFHandler._get_lems_model_with_neuroml2_types()
+            lems_comp = lems.Component(
+                id_=nmllite_comp.id, type_=nmllite_comp.neuroml2_cell
+            )
+            if nmllite_comp.parameters is not None:
                 for p in nmllite_comp.parameters:
                     lems_comp.set_parameter(
                         p,
                         evaluate(
                             nmllite_comp.parameters[p], self.nl_network.parameters
                         ),
                     )
 
-        
-       elif hasattr(nmllite_comp,'pynn_cell'):
-            print_v("  It's a PyNN cell..." )
-            
+        elif hasattr(nmllite_comp, "pynn_cell"):
+            print_v("  It's a PyNN cell...")
+
             nml2_doc_temp = _extract_pynn_components_to_neuroml(self.nl_network)
 
             model = MDFHandler._get_lems_model_with_neuroml2_types(nml2_doc_temp)
 
             lems_comp = model.components[nmllite_comp.id]
-            
+
             for p in nmllite_comp.parameters:
                 lems_comp.set_parameter(
                     p,
-                    evaluate(
-                        nmllite_comp.parameters[p], self.nl_network.parameters
-                    ),
+                    evaluate(nmllite_comp.parameters[p], self.nl_network.parameters),
+                )
+
+        elif hasattr(nmllite_comp, "pynn_synapse_type"):
+            print_v("  It's a PyNN synapse...")
+
+            nml2_doc_temp = _extract_pynn_components_to_neuroml(self.nl_network)
+
+            model = MDFHandler._get_lems_model_with_neuroml2_types(nml2_doc_temp)
+
+            lems_comp = model.components[nmllite_comp.id]
+
+            for p in nmllite_comp.parameters:
+                lems_comp.set_parameter(
+                    p,
+                    evaluate(nmllite_comp.parameters[p], self.nl_network.parameters),
+                )
+
+        elif (
+            hasattr(nmllite_comp, "neuroml2_input")
+            and nmllite_comp.neuroml2_input is not None
+        ):
+            print_v("  It's a NeuroML input...")
+            model = MDFHandler._get_lems_model_with_neuroml2_types()
+            lems_comp = lems.Component(
+                id_=nmllite_comp.id, type_=nmllite_comp.neuroml2_input
+            )
+            for p in nmllite_comp.parameters:
+                lems_comp.set_parameter(
+                    p,
+                    evaluate(nmllite_comp.parameters[p], self.nl_network.parameters),
                 )
 
-       elif hasattr(nmllite_comp,'neuroml2_input') and nmllite_comp.neuroml2_input is not None:
-           print_v("  It's a NeuroML input..." )
-           model = MDFHandler._get_lems_model_with_neuroml2_types()
-           lems_comp = lems.Component(
-               id_=nmllite_comp.id, type_=nmllite_comp.neuroml2_input
-           )
-           for p in nmllite_comp.parameters:
-               lems_comp.set_parameter(
-                   p,
-                   evaluate(
-                       nmllite_comp.parameters[p], self.nl_network.parameters
-                   ),
-               )
-
-       elif hasattr(nmllite_comp,'pynn_input'):
-            print_v("  It's a PyNN input: %s - %s..."%(nmllite_comp.id, nmllite_comp.pynn_input) )
-            
+        elif hasattr(nmllite_comp, "pynn_input"):
+            print_v(
+                "  It's a PyNN input: %s - %s..."
+                % (nmllite_comp.id, nmllite_comp.pynn_input)
+            )
+
             nml2_doc_temp = _extract_pynn_components_to_neuroml(self.nl_network)
 
             model = MDFHandler._get_lems_model_with_neuroml2_types(nml2_doc_temp)
 
             lems_comp = model.components[nmllite_comp.id]
-            '''
+            """
             for p in nmllite_comp.parameters:
                 lems_comp.set_parameter(
                     p,
                     evaluate(
                         nmllite_comp.parameters[p], self.nl_network.parameters
                     ),
-                )'''
+                )"""
+
+        else:
+            raise Exception(
+                "Can't determine the source of the component definition in: %s"
+                % nmllite_comp
+            )
+
+        print_v("All LEMS Components in known LEMS model: %s" % list(model.components.keys()))
+        print_v("This comp: %s" % lems_comp)
+        comp_type_name = lems_comp.type
+        lems_comp_type = model.component_types.get(comp_type_name)
+        print_v("lems_comp_type: %s" % lems_comp_type)
+        notes = "Cell: [%s] is defined in %s and in Lems is: %s" % (
+            nmllite_comp,
+            nmllite_comp.lems_source_file,
+            lems_comp,
+        )
 
-       print_v("All LEMS comps in model: %s" % list(model.components.keys()))
-       print_v("This comp: %s" % lems_comp)
-       comp_type_name = lems_comp.type
-       lems_comp_type = model.component_types.get(comp_type_name)
-       print_v("lems_comp_type: %s" % lems_comp_type)
-       notes = "Cell: [%s] is defined in %s and in Lems is: %s" % (
-           nmllite_comp,
-           nmllite_comp.lems_source_file,
-           lems_comp,
-       )
-
-       node["notes"] = notes
-
-       for p in lems_comp.parameters:
-           node["parameters"][p] = {
-               "value": [get_value_in_si(evaluate(lems_comp.parameters[p]))]*pop_size
-           }
-
-       consts = self._get_all_elements_in_lems(lems_comp_type, model, 'constants')
-       for c in consts:
-            node["parameters"][c.name] = {"value": [get_value_in_si(c.value)]*pop_size}
+        node["notes"] = notes
 
+        for p in lems_comp.parameters:
+            node["parameters"][p] = {
+                "value": [get_value_in_si(evaluate(lems_comp.parameters[p]))] * size
+            }
+
+        properties = self._get_all_elements_in_lems(
+            lems_comp_type, model, "properties"
+        )
+        for prop in properties:
+            node["parameters"][prop.name] = {
+                "value": [get_value_in_si(evaluate(prop.default_value))] * size
+            }
+
+        #if lems_comp_types.is_or_extends()
+
+        consts = self._get_all_elements_in_lems(lems_comp_type, model, "constant")
+        for c in consts:
+            node["parameters"][c.name] = {"value": [get_value_in_si(c.value)] * size}
 
-       if hasattr(lems_comp_type,'dynamics'): 
-            
+        event_ports = self._get_all_elements_in_lems(
+            lems_comp_type, model, "event_port"
+        )
+        for ep in event_ports:
+            if ep.direction == "out":
+                node["parameters"][ep.name] = {"value": [0] * size}
+                node["output_ports"][ep.name] = {"value": ep.name}
+            elif ep.direction == "in":
+                ep_name = self._get_input_port_name(ep.name)
+                node["input_ports"][ep_name] = {"shape": [size], "reduce": "add"}
+
+        if hasattr(lems_comp_type, "dynamics"):
             for sv in lems_comp_type.dynamics.state_variables:
                 node["parameters"][sv.name] = {}
 
             for reg in lems_comp_type.dynamics.regimes:
+                node["parameters"]["ACTIVE_REGIME"] = {"value": [1] * size}
+                node["parameters"]["INACTIVE_REGIME"] = {"value": [0] * size}
 
-                node['parameters']['ACTIVE_REGIME']={'value': [1]*pop_size}
-                node['parameters']['INACTIVE_REGIME']={'value': [0]*pop_size}
+                reg_param = "REGIME_%s" % reg.name
+                # node["parameters"][reg_param] = {"value": 'ACTIVE_REGIME' if reg.initial else 'INACTIVE_REGIME'}
 
-                reg_param = "REGIME_%s"%reg.name
-                #node["parameters"][reg_param] = {"value": 'ACTIVE_REGIME' if reg.initial else 'INACTIVE_REGIME'}
-                
                 if not reg_param in node["parameters"]:
                     node["parameters"][reg_param] = {}
                 node["parameters"][reg_param]["value"] = reg_param
-                node["parameters"][reg_param]["default_initial_value"] = 'ACTIVE_REGIME' if reg.initial else 'INACTIVE_REGIME'
+                node["parameters"][reg_param]["default_initial_value"] = (
+                    "ACTIVE_REGIME" if reg.initial else "INACTIVE_REGIME"
+                )
 
                 node["output_ports"][reg_param] = {"value": reg_param}
 
                 for td in reg.time_derivatives:
                     node["parameters"][td.variable][
                         "time_derivative"
-                    ] = self._convert_value("%s * (%s)"%(reg_param,td.value))
+                    ] = self._convert_value("%s * (%s)" % (reg_param, td.value))
 
                 for eh in reg.event_handlers:
-
-                    print_v("Converting: %s (type: %s)" % (eh, type(eh)))
+                    print_v("Converting the event handler: %s (type: %s)" % (eh, type(eh)))
 
                     if type(eh) == lems.OnCondition:
-                                        
                         # TODO: remove when global t available
-                        node['parameters']['t']={'default_initial_value': 0, 'time_derivative': '1'}
+                        node["parameters"]["t"] = {
+                            "default_initial_value": 0,
+                            "time_derivative": "1",
+                        }
 
-                        test = "(%s == ACTIVE_REGIME) * (%s)" % (reg_param, self._replace_in_condition_test(eh.test))
-                        #test = "%s == ACTIVE_REGIME" % (reg_param)
-                        if (
-                            not "conditions"
-                            in node["parameters"][reg_param]
-                        ):
-                            node["parameters"][reg_param][
-                                "conditions"
-                            ] = {}
+                        test = "(%s == ACTIVE_REGIME) * (%s)" % (
+                            reg_param,
+                            self._replace_in_condition_test(eh.test),
+                        )
+                        # test = "%s == ACTIVE_REGIME" % (reg_param)
+                        if not "conditions" in node["parameters"][reg_param]:
+                            node["parameters"][reg_param]["conditions"] = {}
 
                         node["parameters"][reg_param]["conditions"][
                             "regime_exit_condition"
-                        ] = {"test": test, "value": 'INACTIVE_REGIME'}
-                        
+                        ] = {"test": test, "value": "INACTIVE_REGIME"}
+
                         for a in eh.actions:
                             if type(a) == lems.Transition:
                                 reg_to_id = a.regime
-                                print_v("  Transition: %s -> %s" % (reg_param, reg_to_id))
-                                reg_to_param = "REGIME_%s"%reg_to_id
+                                print_v(
+                                    "  Transition: %s -> %s" % (reg_param, reg_to_id)
+                                )
+                                reg_to_param = "REGIME_%s" % reg_to_id
                                 if not reg_to_param in node["parameters"]:
                                     node["parameters"][reg_to_param] = {}
                                 reg_to = lems_comp_type.dynamics.regimes[reg_to_id]
-                                if (
-                                    not "conditions"
-                                    in node["parameters"][reg_to_param]
-                                ):
-                                    node["parameters"][reg_to_param][
-                                        "conditions"
-                                    ] = {}
+                                if not "conditions" in node["parameters"][reg_to_param]:
+                                    node["parameters"][reg_to_param]["conditions"] = {}
 
                                 node["parameters"][reg_to_param]["conditions"][
                                     "regime_entry_condition"
-                                ] = {"test": test, "value": 'ACTIVE_REGIME'}
+                                ] = {"test": test, "value": "ACTIVE_REGIME"}
 
                                 for eh in reg_to.event_handlers:
-
-                                    print_v("Converting: %s (type: %s)" % (eh, type(eh)))
+                                    print_v(
+                                        "Converting an event handler: %s (type: %s)" % (eh, type(eh))
+                                    )
 
                                     if type(eh) == lems.OnEntry:
                                         for a in eh.actions:
                                             if type(a) == lems.StateAssignment:
                                                 if (
                                                     not "conditions"
                                                     in node["parameters"][a.variable]
                                                 ):
                                                     node["parameters"][a.variable][
                                                         "conditions"
                                                     ] = {}
 
-                                                node["parameters"][a.variable]["conditions"][
-                                                    "entering_regime_%s"%reg_to_id
-                                                ] = {"test": test, "value": a.value}
-
+                                                node["parameters"][a.variable][
+                                                    "conditions"
+                                                ]["entering_regime_%s" % reg_to_id] = {
+                                                    "test": test,
+                                                    "value": a.value,
+                                                }
+
+
+                            if type(a) == lems.EventOut: 
+
+                                del node["parameters"][a.port]["value"]
+                                node["parameters"][a.port] = {"default_initial_value": [0] * size}
+
+                                if not "conditions" in node["parameters"][a.port]:
+                                    node["parameters"][a.port]["conditions"] = {}
+
+                                node["parameters"][a.port]["conditions"][
+                                    "condition_%s_on" % a.port
+                                ] = {"test": test, "value": 1}
+                                node["parameters"][a.port]["conditions"][
+                                    "condition_%s_off" % a.port
+                                ] = {"test": "%s > 0"%a.port, "value": 0}
+                        
 
             for sv in lems_comp_type.dynamics.state_variables:
-                #node["parameters"][sv.name]["value"] = [0]*pop_size
+                # node["parameters"][sv.name]["value"] = [0]*size
 
                 node["output_ports"][sv.name] = {"value": sv.name}
                 if sv.exposure:
                     node["output_ports"][sv.exposure] = {"value": sv.name}
-            
 
             for dv in lems_comp_type.dynamics.derived_variables:
-
                 print_v(
-                    "Converting: %s (exp: %s) = [%s] or [%s]"
+                    "Converting derived variable: %s (exp: %s) = [%s] or [%s]"
                     % (dv.name, dv.exposure, dv.value, dv.select)
                 )
                 if dv.name == "INPUT":
                     node["input_ports"][dv.name] = {}
                 else:
                     if dv.value is not None:
-                        node["parameters"][dv.name] = {
+                        dv_name = dv.name
+                        node["parameters"][dv_name] = {
                             "value": self._convert_value(dv.value)
                         }
                         if dv.exposure:
-                            node["output_ports"][dv.exposure] = {
-                                "value": dv.name
-                            }
+                            node["output_ports"][dv.exposure] = {"value": dv_name}
                     if dv.select is not None:
-                        in_port = dv.select.replace("[*]/", "_")
+                        in_port = dv.select.replace("[*]/", "_").replace("/", "_")
                         node["input_ports"][in_port] = {}
+                        ''' "shape": [size],
+                            "reduce": "add",'''
+                        
                         node["parameters"][dv.name] = {"value": in_port}
 
             conditions = 0
             for eh in lems_comp_type.dynamics.event_handlers:
+                print_v("Converting an event handler: %s (type: %s)" % (eh, type(eh)))
+
+                if type(eh) == lems.OnEvent:
+                    ep_name = self._get_input_port_name(eh.port)
+                    for a in eh.actions:
+                        if type(a) == lems.StateAssignment:
+                            if not "conditions" in node["parameters"][a.variable]:
+                                node["parameters"][a.variable]["conditions"] = {}
 
-                print_v("Converting: %s (type: %s)" % (eh, type(eh)))
+                            to_check = ep_name
+                            if to_check == SPIKE_INPUT_PORT_ID:
+                                to_check = WEIGHTED_SPIKE_INPUTS
+                            node["parameters"][a.variable]["conditions"][
+                                "condition_%s_on_eh" % ep_name
+                            ] = {"test": "%s > 0"%to_check, "value": a.value}
 
                 if type(eh) == lems.OnStart:
                     for a in eh.actions:
                         if type(a) == lems.StateAssignment:
                             node["parameters"][a.variable][
                                 "default_initial_value"
-                            ] = a.value
+                            ] =  a.value 
                         if "value" in node["parameters"][a.variable]:
                             node["parameters"][a.variable].pop("value")
+
                 if type(eh) == lems.OnCondition:
                     test = self._replace_in_condition_test(eh.test)
 
                     for a in eh.actions:
                         if type(a) == lems.StateAssignment:
-                            if (
-                                not "conditions"
-                                in node["parameters"][a.variable]
-                            ):
-                                node["parameters"][a.variable][
-                                    "conditions"
-                                ] = {}
+                            if not "conditions" in node["parameters"][a.variable]:
+                                node["parameters"][a.variable]["conditions"] = {}
 
                             node["parameters"][a.variable]["conditions"][
                                 "condition_%i" % conditions
                             ] = {"test": test, "value": a.value}
+
+                        if type(a) == lems.EventOut: 
+
+                            del node["parameters"][a.port]["value"]
+                            node["parameters"][a.port] = {"default_initial_value": [0] * size}
+                            
+                            if not "conditions" in node["parameters"][a.port]:
+                                node["parameters"][a.port]["conditions"] = {}
+
+                            node["parameters"][a.port]["conditions"][
+                                "condition_%i_on" % conditions
+                            ] = {"test": test, "value": 1}
+                            node["parameters"][a.port]["conditions"][
+                                "condition_%i_off" % conditions
+                            ] = {"test": "%s > 0"%a.port, "value": 0}
+                        
                     conditions += 1
 
             for td in lems_comp_type.dynamics.time_derivatives:
                 node["parameters"][td.variable][
                     "time_derivative"
                 ] = self._convert_value(td.value)
 
-       return node
+                if not "default_initial_value" in node["parameters"][td.variable]:
+                    node["parameters"][td.variable][
+                    "default_initial_value"
+                ] = [0] * size
+
+        return node
 
     def _replace_in_condition_test(self, test):
-        return (test.replace(".gt.", ">")
-                    .replace(".geq.", ">=")
-                    .replace(".lt.", "<")
-                    .replace(".leq.", "<=")
-                    .replace(".eq.", "==")
-                    .replace(".and.", "and"))
+        return (
+            test.replace(".gt.", ">")
+            .replace(".geq.", ">=")
+            .replace(".lt.", "<")
+            .replace(".leq.", "<=")
+            .replace(".eq.", "==")
+            .replace(".and.", "and")
+        )
 
     # TODO: move to pylems!
     @classmethod
     def _get_all_elements_in_lems(cls, component_type, model, child_type):
         ee = []
         if child_type == "exposure":
             for e in component_type.exposures:
                 ee.append(e)
-        if child_type == "constants":
+        elif child_type == "constant":
             for c in component_type.constants:
                 ee.append(c)
+        elif child_type == "event_port":
+            for e in component_type.event_ports:
+                ee.append(e)
+        elif child_type == "properties":
+            for p in component_type.properties:
+                ee.append(p)
+        else:
+            raise Exception("Cannot get child of type: %s in LEMS model"%child_type)
 
         if component_type.extends:
             ect = model.component_types[component_type.extends]
             ee.extend(cls._get_all_elements_in_lems(ect, model, child_type))
 
         return ee
 
     # TODO: move to pyneuroml!
     @classmethod
     def _get_lems_model_with_neuroml2_types(cls, nml_doc=None):
-
         from pyneuroml.pynml import get_path_to_jnml_jar
         from pyneuroml.pynml import read_lems_file
         from lems.parser.LEMS import LEMSFileParser
         import zipfile
 
         lems_model = lems.Model(include_includes=False)
         parser = LEMSFileParser(lems_model)
@@ -432,35 +560,34 @@
         parser.parse(new_lems)
         new_lems = jar.read("NeuroML2CoreTypes/PyNN.xml")
         parser.parse(new_lems)
         new_lems = jar.read("NeuroML2CoreTypes/Inputs.xml")
         parser.parse(new_lems)
 
         if nml_doc is not None:
-
             import io
+
             sf = io.StringIO()
 
             from neuroml.writers import NeuroMLWriter
 
-            
-            print("Adding nml elements from this doc to new lems model: %s"%nml_doc.summary())
+            print(
+                "Adding nml elements from this doc to new lems model: %s"
+                % nml_doc.summary()
+            )
 
             NeuroMLWriter.write(nml_doc, sf, close=False)
             sf.seek(0)
             parser.parse(sf.read())
 
-
-
         return lems_model
 
     # TODO: move to pyneuroml!
     @classmethod
     def _load_lems_file_with_neuroml2_types(cls, lems_filename):
-
         from pyneuroml.pynml import read_lems_file
 
         lems_model = cls._get_lems_model_with_neuroml2_types()
 
         model = read_lems_file(
             lems_filename,
             include_includes=False,
@@ -470,68 +597,118 @@
 
         for cid, c in model.components.items():
             lems_model.components[cid] = c
         for ctid, ct in model.component_types.items():
             lems_model.component_types[ctid] = ct
 
         return lems_model
-    
+
     def handle_location(self, id, population_id, component, x, y, z):
         pass
 
     def finalise_population(self, population_id):
-
         pass
 
     def handle_projection(
         self,
         projName,
         prePop,
         postPop,
         synapse,
         hasWeights=False,
         hasDelays=False,
         type="projection",
         synapse_obj=None,
         pre_synapse_obj=None,
     ):
-        
         synInfo = ""
         if synapse_obj:
             synInfo += " (syn: %s)" % synapse_obj.__class__.__name__
 
         if pre_synapse_obj:
             synInfo += " (pre comp: %s)" % pre_synapse_obj.__class__.__name__
 
         print_v(
-            "Projection: "
+            "  = Projection: "
             + projName
             + " ("
             + type
             + ") from "
             + prePop
             + " to "
             + postPop
             + " with syn: "
             + synapse
             + synInfo
         )
 
-        pre_node_id = "%s" % (prePop)
-        post_node_id = "%s" % (postPop)
-        edge_id = "Edge %s to %s" % (pre_node_id, post_node_id)
-        edge = {}
-        edge["name"] = edge_id
+        syn_node_id = "%s_%s"%(projName,synapse)
+        syn_node = {}
+
+        syn_comp = self.nl_network.get_child(synapse, "synapses")
+
+        print("Converting syn %s; %s" % (synapse_obj, syn_comp))
+
+        pre_pop_size = self.pop_ids_vs_size[prePop]
+        post_pop_size = self.pop_ids_vs_size[postPop]
+
+        syn_node = self._comp_to_mdf_node(
+            nmllite_comp=syn_comp,
+            lems_comp_id=synapse,
+            size=post_pop_size,
+            properties={},
+        )
+        if SPIKE_INPUT_PORT_ID in syn_node['input_ports']:
+            syn_node['input_ports'][SPIKE_INPUT_PORT_ID]['shape'] = [pre_pop_size]
+            syn_node['parameters'][WEIGHTED_SPIKE_INPUTS] = {'value': numpy.zeros([pre_pop_size, post_pop_size]).tolist() }  
+            syn_node['parameters']['weight'] = {}
+            syn_node['parameters']['weight']['function']="MatMul"
+            syn_node['parameters']['weight']['args']={"A": SPIKE_INPUT_PORT_ID, "B": WEIGHTED_SPIKE_INPUTS}
+ 
+        self.mdf_graph["nodes"][syn_node_id] = syn_node
+
+        #### Edge pre_node -> syn 
         
-        edge["sender_port"] = "OUTPUT"
-        edge["receiver_port"] = "INPUT"
-        edge["sender"] = pre_node_id
-        edge["receiver"] = post_node_id
+        pre_node_id = prePop
+        pre_node = self.mdf_graph["nodes"][pre_node_id]
 
-        self.mdf_graph["edges"][edge_id] = edge
+        pre_syn_edge_id = "%s_TO_%s" % (pre_node_id, syn_node_id)
+        pre_syn_edge = {}
+        pre_syn_edge["name"] = pre_syn_edge_id
+
+        pre_ports = list(pre_node["output_ports"].keys())
+        pre_syn_edge["sender_port"] = "OUTPUT" if "OUTPUT" in pre_ports else pre_ports[0]
+
+        post_ports = list(syn_node["input_ports"].keys())
+        pre_syn_edge["receiver_port"] = "INPUT" if "INPUT" in post_ports else post_ports[0]
+        pre_syn_edge["sender"] = pre_node_id
+        pre_syn_edge["receiver"] = syn_node_id
+
+        self.mdf_graph["edges"][pre_syn_edge_id] = pre_syn_edge
+
+
+        #### Edge syn -> post_node
+        
+        post_node_id = postPop
+        post_node = self.mdf_graph["nodes"][post_node_id]
+
+        syn_post_edge_id = "%s_TO_%s" % (syn_node_id,post_node_id)
+        syn_post_edge = {}
+        syn_post_edge["name"] = syn_post_edge_id
+
+        syn_ports = list(syn_node["output_ports"].keys())
+
+        syn_post_edge["sender_port"] = "OUTPUT" if "OUTPUT" in syn_ports else ("i" if "i" in syn_ports else syn_ports[0])
+
+        post_ports = list(post_node["input_ports"].keys())
+        syn_post_edge["receiver_port"] = "INPUT" if "INPUT" in post_ports else ("synapses_i" if "synapses_i" in post_ports else post_ports[0])
+        syn_post_edge["sender"] = syn_node_id
+        syn_post_edge["receiver"] = post_node_id
+
+        self.mdf_graph["edges"][syn_post_edge_id] = syn_post_edge
 
     #
     #  Should be overridden to handle network connection
     #
     def handle_connection(
         self,
         projName,
@@ -544,88 +721,119 @@
         preSegId=0,
         preFract=0.5,
         postSegId=0,
         postFract=0.5,
         delay=0,
         weight=1,
     ):
-
         # self.print_connection_information(projName, id, prePop, postPop, synapseType, preCellId, postCellId, weight)
         print_v(
-            ">>>>>> Src cell: %d, seg: %f, fract: %f -> Tgt cell %d, seg: %f, fract: %f; weight %s, delay: %s ms"
+            ">>>>>> Src pop: %s, cell: %d, seg: %f, fract: %f -> Tgt pop %s, cell %d, seg: %f, fract: %f; syn: %s, weight %s, delay: %s ms"
             % (
+                prePop,
                 preCellId,
                 preSegId,
                 preFract,
+                postPop,
                 postCellId,
                 postSegId,
                 postFract,
+                synapseType,
                 weight,
                 delay,
             )
         )
 
+        if preSegId != 0 or postSegId != 0:
+            raise Exception(
+                "MDF export does not support connections on anything other than segment id = 0"
+            )
+        
+        syn_node_id = "%s_%s"%(projName,synapseType)
+        node = self.mdf_graph["nodes"][syn_node_id]
+        if WEIGHTED_SPIKE_INPUTS in node["parameters"]:
+            # Weight used inside input
+            node["parameters"][WEIGHTED_SPIKE_INPUTS]["value"][preCellId][postCellId] = weight
+            print(node["parameters"][WEIGHTED_SPIKE_INPUTS]["value"])
+        
+
+    def _get_input_list_node_id(self, inputListId):
+        return "InputList_%s" % (inputListId)
+        #return "%s" % (inputListId)
 
     #
     #  Should be overridden to create input source array
     #
     def handle_input_list(
         self, inputListId, population_id, component, size, input_comp_obj=None
     ):
-
         self.input_list_vs_comps[inputListId] = component
         self.input_list_vs_pops[inputListId] = population_id
 
-    #
-    #  Should be overridden to to connect each input to the target cell
-    #
-    def handle_single_input(
-        self, inputListId, id, cellId, segId=0, fract=0.5, weight=1
-    ):
-        component = self.input_list_vs_comps[inputListId]
         print_v(
-            "Input: %s[%s], cellId: %i, seg: %i, fract: %f, weight: %f, component: %s"
-            % (inputListId, id, cellId, segId, fract, weight, component)
+            "InputList: %s, population_id: %s, component: %s, size: %i, input_comp_obj: %s"
+            % (inputListId, population_id, component, size, input_comp_obj)
         )
 
-        node_id = "Input_%s_%i" % (inputListId, id)
+        node_id = self._get_input_list_node_id(inputListId)
 
         comp = self.nl_network.get_child(component, "input_sources")
 
-        node = self._comp_to_mdf_node(comp, component, node_id, 1)
+        node = self._comp_to_mdf_node(nmllite_comp=comp, lems_comp_id=component, size=1)
 
         # TODO: remove when global t available
-        node['parameters']['t']={'default_initial_value': 0, 'time_derivative': '1'}
+        node["parameters"]["t"] = {"default_initial_value": 0, "time_derivative": "1"}
+
+        pop_size = self.pop_ids_vs_size[population_id]
+        node["parameters"]["weight"] = {"value": [0.0] * pop_size}
 
         self.mdf_graph["nodes"][node_id] = node
 
         pre_node_id = node_id
-        post_node_id = "%s" % (self.input_list_vs_pops[inputListId])
+        post_node_id = "%s" % population_id
         edge_id = "Edge %s to %s" % (pre_node_id, post_node_id)
         edge = {}
         edge["name"] = edge_id
         edge["sender_port"] = "i"
-        edge["receiver_port"] = "synapses_i"
+        edge["receiver_port"] = DEFAULT_CURRENT_INPUT_PORT
         edge["sender"] = pre_node_id
         edge["receiver"] = post_node_id
 
-        # Weight used inside input
-        node['parameters']['weight']={'value': weight}
-
         self.mdf_graph["edges"][edge_id] = edge
 
     #
     #  Should be overridden to to connect each input to the target cell
     #
+    def handle_single_input(
+        self, inputListId, id, cellId, segId=0, fract=0.5, weight=1
+    ):
+        if segId != 0:
+            raise Exception(
+                "MDF export does not support inputs on anything other than segment id = 0"
+            )
+
+        component = self.input_list_vs_comps[inputListId]
+        print_v(
+            "Input: %s[%s], cellId: %i, seg: %i, fract: %f, weight: %f, component: %s"
+            % (inputListId, id, cellId, segId, fract, weight, component)
+        )
+
+        node = self.mdf_graph["nodes"][self._get_input_list_node_id(inputListId)]
+
+        # Weight used inside input
+        node["parameters"]["weight"]["value"][cellId] = weight
+
+    #
+    #  Should be overridden to to connect each input to the target cell
+    #
     def finalise_input_source(self, inputName):
         print_v("Input : %s completed" % inputName)
 
 
 if __name__ == "__main__":
-
     lems_model = MDFHandler._load_lems_file_with_neuroml2_types(
         "../../git/MDF/examples/NeuroML/LEMS_SimIzhikevichTest.xml"
     )
 
     print(
         "Loaded LEMS with\n > Dims: %s\n\n > CompTypes: %s\n\n > Comps: %s"
         % (
```

### Comparing `neuromllite-0.5.4/neuromllite/MatrixHandler.py` & `neuromllite-0.5.6/neuromllite/MatrixHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,19 @@
 from neuromllite.utils import evaluate
 from neuromllite.NetworkGenerator import _get_rng_for_network
 
 import numpy as np
 
 
 class MatrixHandler(ConnectivityHandler):
-
     colormaps_used = []
 
     weight_arrays_to_show = {}
 
     def __init__(self, level=10, nl_network=None):
-
         self.nl_network = nl_network
         self.level = level
 
         self.rng, seed = _get_rng_for_network(self.nl_network)
 
         print_v("Initiating Matrix handler, level %i, seed: %s" % (level, seed))
         self.scale_by_post_pop_cond = True
@@ -58,15 +56,14 @@
     def _get_conn_label(self, template, pclass):
         p = pclass[0].upper() + pclass[1:]
         p = p.replace("_", " ")
         label = template % ("%s conns" % p)
         return label
 
     def finalise_document(self):
-
         entries = []
         # print_v('Finals: %s -> %s'%(self.proj_pre_pops, self.proj_post_pops))
         all_pops = []
         for v in self.proj_pre_pops.values():
             all_pops.append(v)
         for v in self.proj_post_pops.values():
             all_pops.append(v)
@@ -140,15 +137,14 @@
                 self._get_conn_label(matrix_total_conns_per_cell, pclass)
             ] = "conductance (nS)"
             cbar_labels[
                 self._get_conn_label(matrix_total_signed_conns_per_cell, pclass)
             ] = "conductance * sign (nS)"
 
         for projName in self.proj_weights:
-
             pre_pop = self.proj_pre_pops[projName]
             post_pop = self.proj_post_pops[projName]
             proj_type = self.proj_types[projName]
             num_pre = self.get_size_pre_pop(projName)
             num_post = self.get_size_post_pop(projName)
 
             gbase_nS, gbase = self._get_gbase_nS(projName, return_orig_string_also=True)
@@ -170,15 +166,14 @@
                     sign,
                     gbase_nS,
                     gbase,
                 )
             )
 
             if self.is_cell_level():
-
                 for pre_i in range(self.pop_sizes[pre_pop]):
                     for post_i in range(self.pop_sizes[post_pop]):
                         pre_pop_i = entries.index(
                             self.get_cell_identifier(pre_pop, pre_i)
                         )
                         post_pop_i = entries.index(
                             self.get_cell_identifier(post_pop, post_i)
@@ -213,15 +208,14 @@
                 self.weight_arrays_to_show[
                     self._get_conn_label(matrix_total_conns, pclass)
                 ][pre_pop_i][post_pop_i] += (abs(self.proj_tot_weight[projName]) * sign)
 
                 if abs(self.proj_tot_weight[projName]) != abs(
                     self.proj_weights[projName]
                 ):
-
                     self.weight_arrays_to_show[
                         self._get_conn_label(matrix_single_conns, pclass)
                     ][pre_pop_i][post_pop_i] += (
                         abs(self.proj_weights[projName]) * sign
                     )
 
                     self.weight_arrays_to_show[
@@ -246,15 +240,14 @@
             weight_array = self.weight_arrays_to_show[proj_type]
 
             print_v(
                 "Plotting proj_type: %s with values from %s to %s"
                 % (proj_type, weight_array.min(), weight_array.max())
             )
             if not (weight_array.max() == 0 and weight_array.min() == 0):
-
                 fig, ax = plt.subplots()
                 title = "%s" % (proj_type)
                 title2 = "%s" % (proj_type)
                 plt.title(title)
                 fig.canvas.set_window_title(title2)
 
                 max_abs_weight = max(weight_array.max(), -1.0 * (weight_array.min()))
@@ -441,15 +434,14 @@
         synapse,
         hasWeights=False,
         hasDelays=False,
         type="projection",
         synapse_obj=None,
         pre_synapse_obj=None,
     ):
-
         weight = 1.0
         self.proj_pre_pops[projName] = prePop
         self.proj_post_pops[projName] = postPop
 
         proj_type = "excitatory"
 
         if prePop in self.pop_types:
@@ -509,20 +501,18 @@
             "New projection: %s, %s->%s, weights? %s, type: %s"
             % (projName, prePop, postPop, weight, proj_type)
         )
 
     def finalise_projection(
         self, projName, prePop, postPop, synapse=None, type="projection"
     ):
-
         pass
         # print_v("Projection finalising: "+projName+" -> "+prePop+" to "+postPop+" completed (%s; w: %s, conns: %s, tot w: %s)" % \
         #           (self.proj_types[projName], self.proj_weights[projName], self.proj_conns[projName], self.proj_tot_weight[projName]))
 
     sizes_ils = {}
     pops_ils = {}
     weights_ils = {}
     input_comp_obj_ils = {}
 
     def finalise_input_source(self, inputListId):
-
         pass
```

### Comparing `neuromllite-0.5.4/neuromllite/NetworkGenerator.py` & `neuromllite-0.5.6/neuromllite/NetworkGenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 
 import lems.api as lems  # from pylems
 
 DEFAULT_NET_GENERATION_SEED = 1234
 DEFAULT_SIMULATION_SEED = 5678
 
 
-
 def __TEMP_CHECK_IF_SET(value):
     """
     Should just be a check for None! Update in modelspec...
     """
-    if value is None: return False
-    if value == '': return False
+    if value is None:
+        return False
+    if value == "":
+        return False
     return True
 
+
 def _get_rng_for_network(nl_model):
     """
     Get a random number generator and the seed used to generate it
     """
     seed = (
         nl_model.seed
         if nl_model and nl_model.seed is not None
@@ -62,15 +64,14 @@
         "Starting net generation for %s%s..."
         % (nl_model.id, " (base dir: %s)" % base_dir if base_dir else "")
     )
 
     rng, seed = _get_rng_for_network(nl_model)
 
     if nl_model.network_reader:
-
         exec(
             "from neuromllite.%s import %s"
             % (nl_model.network_reader.type, nl_model.network_reader.type)
         )
 
         network_reader = eval("%s()" % (nl_model.network_reader.type))
         network_reader.parameters = nl_model.network_reader.parameters
@@ -86,21 +87,24 @@
         notes += "\n    Generation seed: %i" % (seed)
         if nl_model.parameters:
             notes += "\n    NeuroMLlite parameters: "
             for p in sorted(nl_model.parameters.keys()):
                 if not p == "__builtins__":
                     notes += "\n        %s = %s" % (p, nl_model.parameters[p])
         handler.handle_document_start(nl_model.id, notes)
-        temperature = "%sdegC" % nl_model.temperature if nl_model.temperature is not None else None
+        temperature = (
+            "%sdegC" % nl_model.temperature
+            if nl_model.temperature is not None
+            else None
+        )
         handler.handle_network(nl_model.id, nl_model.notes, temperature=temperature)
 
     nml2_doc_temp = _extract_pynn_components_to_neuroml(nl_model)
 
     for c in nl_model.cells:
-
         if c.neuroml2_source_file:
             from pyneuroml import pynml
 
             nml2_doc = pynml.read_neuroml2_file(
                 locate_file(c.neuroml2_source_file, base_dir), include_includes=True
             )
             cell_objects[c.id] = nml2_doc.get_by_id(c.id)
@@ -113,34 +117,32 @@
             from pyneuroml import pynml
 
             nml2_doc = pynml.read_neuroml2_file(
                 locate_file(s.neuroml2_source_file, base_dir), include_includes=True
             )
             synapse_objects[s.id] = nml2_doc.get_by_id(s.id)
 
-        if hasattr(s, 'pynn_synapse') and s.pynn_synapse is not None:
+        if hasattr(s, "pynn_synapse") and s.pynn_synapse is not None:
             synapse_objects[s.id] = nml2_doc_temp.get_by_id(s.id)
 
     for p in nl_model.populations:
-
         size = evaluate(p.size, nl_model.parameters)
         properties = p.properties if p.properties else {}
 
         if p.random_layout:
             properties["region"] = p.random_layout.region
         if p.relative_layout:
             properties["region"] = p.relative_layout.region
 
         if (
             not p.random_layout
             and not p.single_location
             and not p.relative_layout
             and not always_include_props
         ):
-
             # If there are no positions (abstract network), and <property>
             # is added to <population>, jLems doesn't like it... (it has difficulty
             # interpreting pop0[0]/v, etc.)
             # So better not to give properties...
             properties = {}
 
         if p.notes:
@@ -193,15 +195,14 @@
                 handler.handle_location(i, p.id, p.component, x, y, z)
 
         if hasattr(handler, "finalise_population"):
             handler.finalise_population(p.id)
 
     if include_connections:
         for p in nl_model.projections:
-
             type = p.type if p.type else "projection"
 
             synapse_obj = (
                 synapse_objects[p.synapse] if p.synapse in synapse_objects else None
             )
             pre_synapse_obj = (
                 synapse_objects[p.pre_synapse]
@@ -238,15 +239,14 @@
                             flip = rng.random()
                             # print("Is cell %i conn to %i, prob %s - %s"%(pre_i, post_i, flip, p.random_connectivity.probability))
                             if flip < evaluate(
                                 p.random_connectivity.probability,
                                 nl_model.parameters,
                                 rng,
                             ):
-
                                 delay = (
                                     evaluate(p.delay, nl_model.parameters, rng)
                                     if p.delay
                                     else 0
                                 )
                                 weight = (
                                     evaluate(p.weight, nl_model.parameters, rng)
@@ -268,17 +268,15 @@
                                     postFract=0.5,
                                     delay=delay,
                                     weight=weight,
                                 )
                                 conn_count += 1
 
                 if p.convergent_connectivity:
-
                     for post_i in range(len(pop_locations[p.postsynaptic])):
-
                         for count in range(int(p.convergent_connectivity.num_per_post)):
                             found = False
                             while not found:
                                 pre_i = int(
                                     rng.random() * len(pop_locations[p.presynaptic])
                                 )
                                 if p.presynaptic == p.postsynaptic and pre_i == post_i:
@@ -318,15 +316,14 @@
                 elif p.one_to_one_connector:
                     for i in range(
                         min(
                             len(pop_locations[p.presynaptic]),
                             len(pop_locations[p.postsynaptic]),
                         )
                     ):
-
                         # print_v("Adding connection %i with weight: %s, delay: %s"%(conn_count, weight, delay))
                         handler.handle_connection(
                             p.id,
                             conn_count,
                             p.presynaptic,
                             p.postsynaptic,
                             p.synapse,
@@ -343,15 +340,14 @@
 
                 handler.finalise_projection(
                     p.id, p.presynaptic, p.postsynaptic, p.synapse
                 )
 
     if include_inputs:
         for input in nl_model.inputs:
-
             handler.handle_input_list(
                 input.id,
                 input.population,
                 input.input_source,
                 size=0,
                 input_comp_obj=None,
             )
@@ -361,15 +357,19 @@
             if __TEMP_CHECK_IF_SET(input.cell_ids):
                 if __TEMP_CHECK_IF_SET(input.percentage):
                     raise Exception(
                         "On the input: %s, only one of percentage or cell_ids is allowed"
                         % input
                     )
                 for i in input.cell_ids:
-                    weight = input.weight if input.weight else 1
+                    weight = (
+                        evaluate(input.weight, nl_model.parameters, rng)
+                        if input.weight
+                        else 1
+                    )
 
                     if input.number_per_cell and input.segment_ids:
                         raise Exception(
                             "On input: %s, only one of number_per_cell or segment_ids is allowed"
                             % input
                         )
 
@@ -385,29 +385,36 @@
 
                     for seg_id in seg_ids:
                         handler.handle_single_input(
                             input.id,
                             input_count,
                             i,
                             segId=seg_id,
-                            weight=evaluate(weight, nl_model.parameters),
+                            weight = (
+                                evaluate(input.weight, nl_model.parameters, rng)
+                                if input.weight
+                                else 1
+                            )
                         )
                         input_count += 1
 
             if __TEMP_CHECK_IF_SET(input.percentage):
                 if __TEMP_CHECK_IF_SET(input.cell_ids):
                     raise Exception(
                         "On input: %s, only one of percentage or cell_ids is allowed"
                         % input
                     )
                 for i in range(len(pop_locations[input.population])):
                     flip = rng.random()
-                    weight = input.weight if input.weight else 1
+                    weight = (
+                        evaluate(input.weight, nl_model.parameters, rng)
+                        if input.weight
+                        else 1
+                    )
                     if flip * 100.0 < input.percentage:
-
                         if input.number_per_cell and input.segment_ids:
                             raise Exception(
                                 "On input: %s, only one of number_per_cell or segment_ids is allowed"
                                 % input
                             )
 
                         if input.number_per_cell:
@@ -422,15 +429,19 @@
 
                         for seg_id in seg_ids:
                             handler.handle_single_input(
                                 input.id,
                                 input_count,
                                 i,
                                 segId=seg_id,
-                                weight=evaluate(weight, nl_model.parameters),
+                                weight = (
+                                    evaluate(input.weight, nl_model.parameters, rng)
+                                    if input.weight
+                                    else 1
+                                )
                             )
                             input_count += 1
 
             handler.finalise_input_source(input.id)
 
     if hasattr(handler, "finalise_document"):
         handler.finalise_document()
@@ -498,40 +509,39 @@
     elif "-pnl" in argv or "-psyneulink" in argv:
         generate_and_run(sim, simulator="psyneulink")
 
     elif "-mdf" in argv:
         generate_and_run(sim, simulator="mdf")
 
     elif "-nml" in argv or "-neuroml" in argv:
-
         network = load_network(sim.network)
         generate_neuroml2_from_network(network, simulation=sim, validate=True)
 
     elif "-nmlh5" in argv or "-neuromlh5" in argv:
-
         network = load_network(sim.network)
         generate_neuroml2_from_network(
             network, simulation=sim, validate=True, format="hdf5"
         )
 
     else:
         for a in argv:
-
             if "-jnmlnetpyne" in a:
                 num_processors = 1
                 if len(a) > len("-jnmlnetpyne"):
                     num_processors = int(a[12:])
                 generate_and_run(
                     sim, simulator="jNeuroML_NetPyNE", num_processors=num_processors
                 )
             elif "graph" in a:  # e.g. -graph3c
                 show_graph = True
                 if "-nogui" in argv:
                     show_graph = False
-                generate_and_run(sim, simulator=a[1:], nogui= not show_graph)  # Will not "run" obviously...
+                generate_and_run(
+                    sim, simulator=a[1:], nogui=not show_graph
+                )  # Will not "run" obviously...
             elif "matrix" in a:  # e.g. -matrix2
                 generate_and_run(sim, simulator=a[1:])  # Will not "run" obviously...
 
 
 def _extract_pynn_components_to_neuroml(nl_model, nml_doc=None):
     """
     Parse the NeuroMLlite description for cell, synapses and inputs described as
@@ -544,23 +554,21 @@
     if nml_doc == None:
         from neuroml import NeuroMLDocument
 
         nml_doc = NeuroMLDocument(id="temp")
 
     for c in nl_model.cells:
         if c.pynn_cell:
-
             if nml_doc.get_by_id(c.id) == None:
                 import pyNN.neuroml
 
                 cell_params = copy.deepcopy(c.parameters) if c.parameters else {}
                 for p in cell_params:
                     cell_params[p] = evaluate(cell_params[p], nl_model.parameters)
                 for proj in nl_model.projections:
-
                     synapse = nl_model.get_child(proj.synapse, "synapses")
                     post_pop = nl_model.get_child(proj.postsynaptic, "populations")
                     if post_pop.component == c.id:
                         # print("--------- Cell %s in post pop %s of %s uses %s"%(c.id,post_pop.id, proj.id, synapse))
 
                         if synapse.pynn_receptor_type == "excitatory":
                             post = "_E"
@@ -568,26 +576,26 @@
                             post = "_I"
                         for p in synapse.parameters:
                             cell_params["%s%s" % (p, post)] = evaluate(
                                 synapse.parameters[p], nl_model.parameters
                             )
 
                 temp_cell = eval("pyNN.neuroml.%s(**cell_params)" % c.pynn_cell)
-                if c.pynn_cell != "SpikeSourcePoisson":
+                
+                if c.pynn_cell != "SpikeSourcePoisson" and c.pynn_cell != "HH_cond_exp":
                     temp_cell.default_initial_values["v"] = temp_cell.parameter_space[
                         "v_rest"
                     ].base_value
 
                 cell_id = temp_cell.add_to_nml_doc(nml_doc, None)
                 cell = nml_doc.get_by_id(cell_id)
                 cell.id = c.id
 
     for s in nl_model.synapses:
         if nml_doc.get_by_id(s.id) == None:
-
             if s.pynn_synapse_type and s.pynn_receptor_type:
                 import neuroml
 
                 tau_syn = evaluate(s.parameters["tau_syn"], nl_model.parameters)
                 if "e_rev" in s.parameters:
                     e_rev = evaluate(s.parameters["e_rev"], nl_model.parameters)
                 if s.pynn_synapse_type == "cond_exp":
@@ -602,15 +610,14 @@
                     syn = neuroml.ExpCurrSynapse(id=s.id, tau_syn=tau_syn)
                     nml_doc.exp_curr_synapses.append(syn)
                 elif s.pynn_synapse_type == "curr_alpha":
                     syn = neuroml.AlphaCurrSynapse(id=s.id, tau_syn=tau_syn)
                     nml_doc.alpha_curr_synapses.append(syn)
 
     for i in nl_model.input_sources:
-
         if i.pynn_input:
             import pyNN.neuroml
 
             input_params = copy.deepcopy(i.parameters) if i.parameters else {}
             for ip in input_params:
                 input_params[ip] = evaluate(input_params[ip], nl_model.parameters)
             temp_input = eval("pyNN.neuroml.%s(**input_params)" % (i.pynn_input))
@@ -669,28 +676,27 @@
             )
         if simulation.duration is not None:
             nml_doc.networks[0].properties.append(
                 neuroml.Property("recommended_duration_ms", simulation.duration)
             )
 
     for i in nl_model.input_sources:
-
         if i.lems_source_file:
             fname = locate_file(i.lems_source_file, base_dir)
 
             print_v(
                 "Need to use for this input parameters: %s in %s from %s (%s); will place in %s"
                 % (i.parameters, i.id, i.lems_source_file, fname, extra_lems_file)
             )
             model = lems.Model()
             model.import_from_file(fname)
             for comp in model.components:
                 if i.id == comp.id:
                     print_v("Found a component: %s in %s" % (comp, fname))
-                    if hasattr(i, 'parameters') and len(i.parameters) > 0:
+                    if hasattr(i, "parameters") and len(i.parameters) > 0:
                         for p in i.parameters:
                             comp.set_parameter(
                                 p, evaluate(i.parameters[p], nl_model.parameters)
                             )
                     extra_lems_components.add(comp)
 
             for d in model.dimensions:
@@ -709,22 +715,21 @@
 
             incl = neuroml.IncludeType(extra_lems_file)
             if not incl in nml_doc.includes:
                 nml_doc.includes.append(incl)
 
         if nml_doc.get_by_id(i.id) == None:
             if i.neuroml2_source_file:
-
                 incl = neuroml.IncludeType(
                     locate_file(i.neuroml2_source_file, base_dir)
                 )
                 if not incl in nml_doc.includes:
                     nml_doc.includes.append(incl)
 
-            if hasattr(i, 'neuroml2_input') and i.neuroml2_input is not None:
+            if hasattr(i, "neuroml2_input") and i.neuroml2_input is not None:
                 input_params = i.parameters if i.parameters else {}
 
                 # TODO make more generic...
 
                 if i.neuroml2_input.lower() == "pulsegenerator":
                     input = neuroml.PulseGenerator(id=i.id)
                     nml_doc.pulse_generators.append(input)
@@ -741,15 +746,14 @@
                     exec(
                         'input.%s = "%s"'
                         % (p, evaluate(input_params[p], nl_model.parameters))
                     )
 
     for c in nl_model.cells:
         if c.neuroml2_source_file:
-
             incl = neuroml.IncludeType(locate_file(c.neuroml2_source_file, base_dir))
             found_cell = False
             for cell in nml_doc.cells:
                 if cell.id == c.id:
                     nml_doc.cells.remove(
                         cell
                     )  # Better to use imported cell file; will have channels, etc.
@@ -798,15 +802,14 @@
                 extra_lems_components.add(inc)
 
             incl = neuroml.IncludeType(extra_lems_file)
             if not incl in nml_doc.includes:
                 nml_doc.includes.append(incl)
 
         if c.neuroml2_cell:
-
             cell_params = c.parameters if c.parameters else {}
             # TODO make more generic...
             if c.neuroml2_cell.lower() == "spikegenerator":
                 cell = neuroml.SpikeGenerator(id=c.id)
                 nml_doc.spike_generators.append(cell)
             elif c.neuroml2_cell.lower() == "spikegeneratorpoisson":
                 cell = neuroml.SpikeGeneratorPoisson(id=c.id)
@@ -906,15 +909,14 @@
 
     print_v("Written NeuroML to %s" % nml_file_name)
 
     if len(extra_lems_components.components) > 0:
         extra_lems_components.export_to_file(extra_lems_file)
 
     if validate and format == "xml":
-
         from pyneuroml import pynml
 
         success = pynml.validate_neuroml2(nml_file_name, verbose_validate=False)
         if success:
             print_v("Generated file is valid NeuroML2!")
         else:
             print_v("Generated file is NOT valid NeuroML2!")
@@ -994,15 +996,14 @@
     for dir_for_mod_files in dirs_for_mod_files:
         if not dir_for_mod_files in locations_mods_loaded_from:
             print_v(
                 "Generated NEURON code; loading mechanisms from %s (cwd: %s; already loaded: %s)"
                 % (dir_for_mod_files, os.getcwd(), locations_mods_loaded_from)
             )
             try:
-
                 from neuron import load_mechanisms
 
                 if os.getcwd() == dir_for_mod_files:
                     print_v(
                         "That's current dir => importing neuron module loads mods here..."
                     )
                 else:
@@ -1037,15 +1038,14 @@
     print_v(
         "Generating network %s and running in simulator: %s..."
         % (network.id, simulator)
     )
 
     try:
         if simulator == "NEURON":  # NOT YET WORKING...
-
             _generate_neuron_files_from_neuroml(network, dir_for_mod_files=target_dir)
 
             from neuromllite.NeuronHandler import NeuronHandler
 
             nrn_handler = NeuronHandler()
 
             for c in network.cells:
@@ -1056,23 +1056,21 @@
             generate_network(network, nrn_handler, generate_network, base_dir)
             if return_results:
                 raise NotImplementedError(
                     "Reloading results not supported in Neuron yet..."
                 )
 
         elif simulator.lower() == "mdf":
-
             from neuromllite.MDFHandler import MDFHandler
 
             mdf_handler = MDFHandler(nl_network=network)
 
             generate_network(network, mdf_handler)
 
         elif simulator.lower() == "psyneulink":
-
             from neuromllite.PsyNeuLinkHandler import PsyNeuLinkHandler
 
             pnl_handler = PsyNeuLinkHandler(nl_network=network)
 
             generate_network(network, pnl_handler)
             from neuromllite import __version__ as nmlliteversion
 
@@ -1154,30 +1152,28 @@
             run_pnl_file = open("run_pnl_%s.py" % network.id, "w")
 
             run_pnl_file.write(run_pnl_script)
 
             print_v("Done with PsyNeuLink...")
 
         elif simulator.lower() == "sonata":
-
             target_simulator = "NEST"
 
             from neuromllite.SonataHandler import SonataHandler
 
             sonata_handler = SonataHandler()
 
             generate_network(
                 network, sonata_handler, always_include_props=True, base_dir=base_dir
             )
 
             import pyNN.neuroml
 
             for c in network.cells:
                 if c.pynn_cell:
-
                     cell_params = {}
                     if c.parameters:
                         for p in c.parameters:
                             cell_params[p] = evaluate(
                                 c.parameters[p], network.parameters
                             )
 
@@ -1250,15 +1246,15 @@
             temp_nml_doc = _extract_pynn_components_to_neuroml(network)
 
             summary = temp_nml_doc.summary()
             from pyneuroml.pynml import convert_to_units
 
             sim_file_info["inputs"] = {}
             for input in sonata_handler.input_info:
-                print('Handling: %s: %s'%(input, sonata_handler.input_info[input]))
+                print("Handling: %s: %s" % (input, sonata_handler.input_info[input]))
                 sim_file_info["inputs"][input] = {}
                 input_comp = sonata_handler.input_info[input][1]
                 c = temp_nml_doc.get_by_id(input_comp)
                 ref = "inputset_%s_%s" % (input, input_comp)
                 if c.__class__.__name__ == "PulseGenerator":
                     sim_file_info["inputs"][input]["input_type"] = "current_clamp"
                     sim_file_info["inputs"][input]["module"] = "IClamp"
@@ -1316,43 +1312,42 @@
 
             run_bmtk_file = open("run_bmtk.py", "w")
             run_bmtk_file.write(run_bmtk_template % (target_simulator))
 
             print_v("Done with Sonata...")
 
         elif simulator.lower().startswith("graph"):  # Will not "run" obviously...
-
             from neuromllite.GraphVizHandler import GraphVizHandler, engines
 
             try:
                 if simulator[-1].isalpha():
-
                     engine = engines[simulator[-1]]
                     level = int(simulator[5:-1])
                 else:
                     engine = "dot"
                     level = int(simulator[5:])
 
             except Exception as e:
                 print_v("Error parsing: %s: %s" % (simulator, e))
                 print_v(
                     "Graphs of the network structure can be generated at many levels of detail (1-6, required) and laid out using GraphViz engines (d - dot (default); c - circo; n - neato; f - fdp), so use: -graph3c, -graph2, -graph4f etc."
                 )
                 return
 
-            handler = GraphVizHandler(level, engine=engine, nl_network=network, view_on_render = not nogui)
+            handler = GraphVizHandler(
+                level, engine=engine, nl_network=network, view_on_render=not nogui
+            )
 
             generate_network(
                 network, handler, always_include_props=True, base_dir=base_dir
             )
 
             print_v("Done with GraphViz...")
 
         elif simulator.lower().startswith("matrix"):  # Will not "run" obviously...
-
             from neuromllite.MatrixHandler import MatrixHandler
 
             try:
                 level = int(simulator[6:])
             except:
                 print_v("Error parsing: %s" % simulator)
                 print_v(
@@ -1365,15 +1360,14 @@
             generate_network(
                 network, handler, always_include_props=True, base_dir=base_dir
             )
 
             print_v("Done with MatrixHandler...")
 
         elif simulator == "BindsNET":
-
             from neuromllite.BindsNETHandler import BindsNETHandler
             import bindsnet
 
             print("\n   ********************************************************")
             print("   *** Warning: Support for BindsNET is very preliminary!! ***")
             print("   ********************************************************\n")
 
@@ -1430,15 +1424,14 @@
             print_v("Finished BindsNET simulation")
             _print_result_info(traces, events)
 
             if return_results:
                 return traces, events
 
         elif simulator == "Arbor":
-
             from neuromllite.ArborHandler import ArborHandler
             import arbor
 
             print("\n   *********************************************************")
             print("   *** Warning: Support for Arbor is very preliminary!!! ***")
             print("   *********************************************************\n")
 
@@ -1480,15 +1473,15 @@
             )
 
             # arbor_model.run(tfinal=simulation.duration)
 
             # (12) Create a default execution context, domain decomposition and simulation
             context = arbor.context()
             decomp = arbor.partition_load_balance(arbor_recipe, context)
-            sim = arbor.simulation(arbor_recipe, decomp, context)
+            sim = arbor.simulation(arbor_recipe, domains=decomp, context=context)
 
             # (13) Set spike generators to record
             sim.record(arbor.spike_recording.all)
 
             # (14) Attach a sampler to the voltage probe on cell 0.
             handles = [
                 sim.sample((gid, 0), arbor.regular_schedule(simulation.dt))
@@ -1503,15 +1496,14 @@
 
             traces = {}
             events = {}
 
             for pop_id in trace_pop_indices_seg_ids:
                 indices = trace_pop_indices_seg_ids[pop_id].keys()
                 for index in indices:
-
                     filename = "%s.%s.%s.v.dat" % (simulation.id, pop_id, index)
                     # all_columns = []
                     gid = arbor_recipe.get_gid(pop_id, index)
 
                     samples, meta = sim.samples(handles[gid])[0]
 
                     data = samples[:, 1]
@@ -1561,25 +1553,23 @@
                 ff.close()"""
 
             if return_results:
                 _print_result_info(traces, events)
                 return traces, events
 
         elif simulator.startswith("PyNN"):
-
             # _generate_neuron_files_from_neuroml(network)
             simulator_name = simulator.split("_")[1].lower()
 
             from neuromllite.PyNNHandler import PyNNHandler
 
             pynn_handler = PyNNHandler(simulator_name, simulation.dt, network.id)
 
             syn_cell_params = {}
             for proj in network.projections:
-
                 synapse = network.get_child(proj.synapse, "synapses")
                 post_pop = network.get_child(proj.postsynaptic, "populations")
 
                 if not post_pop.component in syn_cell_params:
                     syn_cell_params[post_pop.component] = {}
                 for p in synapse.parameters:
                     post = ""
@@ -1629,15 +1619,14 @@
             for s in network.synapses:
                 if s.pynn_receptor_type:
                     receptor_types[s.id] = s.pynn_receptor_type
 
             pynn_handler.set_receptor_types(receptor_types)
 
             for input_source in network.input_sources:
-
                 # TODO: change this when noisyCurrentSource is integrated into the core of NeuroML
                 if input_source.pynn_input or input_source.lems_source_file:
                     pynn_handler.add_input_source(input_source, network)
 
             generate_network(
                 network, pynn_handler, always_include_props=True, base_dir=base_dir
             )
@@ -1682,21 +1671,22 @@
             print_v("Finished PyNN simulation")
             pynn_handler.sim.end()
 
             traces = {}
             events = {}
 
             if not "NeuroML" in simulator:
-
                 # Temp! See https://github.com/NeuralEnsemble/PyNN/pull/762
                 def get_source_id(spiketrain):
-                    if 'source_id' in spiketrain.annotations:
-                        return spiketrain.annotations['source_id']
-                    elif 'channel_id' in spiketrain.annotations: # See https://github.com/NeuralEnsemble/PyNN/pull/762
-                        return spiketrain.annotations['channel_id']
+                    if "source_id" in spiketrain.annotations:
+                        return spiketrain.annotations["source_id"]
+                    elif (
+                        "channel_id" in spiketrain.annotations
+                    ):  # See https://github.com/NeuralEnsemble/PyNN/pull/762
+                        return spiketrain.annotations["channel_id"]
 
                 for pop_id in trace_pop_indices_seg_ids:
                     pynn_pop = pynn_handler.populations[pop_id]
                     indices = trace_pop_indices_seg_ids[pop_id].keys()
 
                     filename = "%s.%s.v.dat" % (simulation.id, pop_id)
                     all_columns = []
@@ -1769,15 +1759,14 @@
                     ff.close()
 
             if return_results:
                 _print_result_info(traces, events)
                 return traces, events
 
         elif simulator == "NetPyNE":
-
             if target_dir == None:
                 target_dir = "./"
 
             _generate_neuron_files_from_neuroml(network, dir_for_mod_files=target_dir)
 
             from netpyne import specs
             from netpyne import sim
@@ -1864,15 +1853,14 @@
                     "Creating connections for %s (%s): %s->%s via %s"
                     % (projName, ptype, prePop, postPop, synapse)
                 )
 
                 preComp = netpyne_handler.pop_ids_vs_components[prePop]
 
                 for conn in netpyne_handler.connections[projName]:
-
                     (
                         pre_id,
                         pre_seg,
                         pre_fract,
                         post_id,
                         post_seg,
                         post_fract,
@@ -1886,15 +1874,14 @@
                         "weight": weight,
                         "synsPerConn": 1,
                         "sec": post_seg,
                         "loc": post_fract,
                     }
 
                     if ptype == "electricalProjection":
-
                         if weight != 1:
                             raise Exception(
                                 "Cannot yet support inputs where weight !=1!"
                             )
                         connParam = {
                             "synsPerConn": 1,
                             "sec": post_seg,
@@ -2003,15 +1990,14 @@
             simulator == "jNeuroML"
             or simulator == "jNeuroML_norun"
             or simulator == "jNeuroML_NEURON"
             or simulator == "jNeuroML_NetPyNE"
             or simulator == "jNeuroML_Brian2"
             or simulator == "EDEN"
         ):
-
             from pyneuroml.lems import generate_lems_file_for_neuroml
             from pyneuroml import pynml
 
             lems_file_name = "LEMS_%s.xml" % simulation.id
 
             nml_file_name, nml_doc = generate_neuroml2_from_network(
                 network, simulation=simulation, base_dir=base_dir, target_dir=target_dir
@@ -2049,15 +2035,14 @@
             rate_pop_indices = get_pops_vs_cell_indices_seg_ids(
                 simulation.record_rates, network
             )
 
             pops = network.populations
             pops.sort(key=id)
             for p in pops:
-
                 if p.id in spike_pop_indices:
                     pops_spike_save.append(p.id)
 
                     save_ref = "%s.%s.spikes" % (simulation.id, p.id)
                     gen_spike_saves_for_cells[save_ref] = []
 
                     for i in spike_pop_indices[p.id].keys():
```

### Comparing `neuromllite-0.5.4/neuromllite/NeuronHandler.py` & `neuromllite-0.5.6/neuromllite/NeuronHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,37 +11,34 @@
 #    though as a means of loading in and positioning cells for checking 3D
 #    layout
 #
 ################################################################################
 
 
 class NeuronHandler(DefaultNetworkHandler):
-
     h = hoc.HocObject()
 
     globalPreSynId = 10000000
 
     preSectionsVsGids = dict()
 
     #
     #   Helper function for printing hoc before executing it
     #
     def executeHoc(self, command):
-
         cmdPrefix = "hoc >>>>>>>>>>: "
 
         if len(command) > 0:
             print_v(cmdPrefix + command)
             self.h(command)
 
     #
     #  Overridden from NetworkHandler
     #
     def handlePopulation(self, population_id, component, size=-1, component_obj=None):
-
         if size >= 0:
             sizeInfo = ", size " + str(size) + " cells"
 
             print_v(
                 "Creating population: "
                 + population_id
                 + ", component: "
@@ -52,15 +49,14 @@
             self.executeHoc("{ n_" + population_id + " = " + str(size) + " }")
             self.executeHoc("{ n_" + population_id + "_local = 0 } ")
             self.executeHoc(
                 "objectvar a_" + population_id + "[n_" + population_id + "]"
             )
 
         else:
-
             print_v(
                 "Population: "
                 + population_id
                 + ", component: "
                 + component
                 + " specifies no size. Will lead to errors!"
             )
@@ -132,15 +128,14 @@
         synapse,
         hasWeights=False,
         hasDelays=False,
         type="projection",
         synapse_obj=None,
         pre_synapse_obj=None,
     ):
-
         print_v("Projection: " + projName + " from " + prePop + " to " + postPop)
 
     #
     #  Overridden from NetworkHandler
     #
     def handleConnection(
         self,
@@ -154,15 +149,14 @@
         preSegId=0,
         preFract=0.5,
         postSegId=0,
         postFract=0.5,
         delay=0,
         weight=1,
     ):
-
         # self.printConnectionInformation(projName, id, prePop, postPop, synapseType, preCellId, postCellId, localWeight)
 
         print_v(
             "\n           --------------------------------------------------------------"
         )
         print_v(
             "Going to create a connection of type "
```

### Comparing `neuromllite-0.5.4/neuromllite/PsyNeuLinkHandler.py` & `neuromllite-0.5.6/neuromllite/PsyNeuLinkHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,39 +10,35 @@
 from neuromllite.utils import locate_file
 from neuromllite.utils import evaluate
 
 import lems.api as lems  # from pylems
 
 
 class PsyNeuLinkHandler(DefaultNetworkHandler):
-
     bids_mdf_info = {}
     bids_mdf_info["graphs"] = []
 
     bids_mdf_info_hl = {}
     bids_mdf_info_hl["graphs"] = []
 
     def __init__(self, nl_network):
         print_v("Initiating PsyNeuLink handler")
         self.nl_network = nl_network
 
     def handle_document_start(self, id, notes):
-
         print_v("Parsing for PsyNeuLink export: %s" % id)
         self.id = id
 
     def finalise_document(self):
-
         print_v("Writing file for...: %s" % self.id)
 
         save_to_json_file(self.bids_mdf_info, "%s.bids-mdf.json" % self.id, indent=4)
         """save_to_json_file(self.bids_mdf_info_hl, '%s.bids-mdf.highlevel.json'%self.id, indent=4)"""
 
     def handle_network(self, network_id, notes, temperature=None):
-
         print_v("Network: %s" % network_id)
         self.network_id = network_id
 
         if temperature:
             print_v("  Temperature: " + temperature)
         if notes:
             print_v("  Notes: " + notes)
@@ -67,15 +63,14 @@
         self.bids_mdf_graph_hl["edges"] = {}
         self.bids_mdf_graph_hl["parameters"] = {}
         self.bids_mdf_info_hl["graphs"].append(self.bids_mdf_graph_hl)
 
     def handle_population(
         self, population_id, component, size=-1, component_obj=None, properties={}
     ):
-
         sizeInfo = " as yet unspecified size"
         if size >= 0:
             sizeInfo = ", size: " + str(size) + " cells"
         if component_obj:
             compInfo = " (%s)" % component_obj.__class__.__name__
         else:
             compInfo = ""
@@ -168,15 +163,14 @@
             pop_node["functions"] = {}
             self.bids_mdf_graph_hl["nodes"][pop_node_id] = pop_node
 
     def handle_location(self, id, population_id, component, x, y, z):
         pass
 
     def finalise_population(self, population_id):
-
         pass
 
     #
     #  Should be overridden to handle network connection
     #
     def handle_connection(
         self,
@@ -190,15 +184,14 @@
         preSegId=0,
         preFract=0.5,
         postSegId=0,
         postFract=0.5,
         delay=0,
         weight=1,
     ):
-
         # self.print_connection_information(projName, id, prePop, postPop, synapseType, preCellId, postCellId, weight)
         print_v(
             ">>>>>> Src cell: %d, seg: %f, fract: %f -> Tgt cell %d, seg: %f, fract: %f; weight %s, delay: %s ms"
             % (
                 preCellId,
                 preSegId,
                 preFract,
@@ -231,24 +224,22 @@
 
     #
     #  Should be overridden to create input source array
     #
     def handle_input_list(
         self, inputListId, population_id, component, size, input_comp_obj=None
     ):
-
         pass
 
     #
     #  Should be overridden to to connect each input to the target cell
     #
     def handle_single_input(
         self, inputListId, id, cellId, segId=0, fract=0.5, weight=1
     ):
-
         print_v(
             "Input: %s[%s], cellId: %i, seg: %i, fract: %f, weight: %f"
             % (inputListId, id, cellId, segId, fract, weight)
         )
 
     #
     #  Should be overridden to to connect each input to the target cell
```

### Comparing `neuromllite-0.5.4/neuromllite/PsyNeuLinkReader.py` & `neuromllite-0.5.6/neuromllite/PsyNeuLinkReader.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,35 +3,32 @@
 from neuroml.hdf5.NetworkContainer import *
 from neuromllite import NetworkReader
 
 from neuromllite.utils import print_v, load_json
 
 
 class PsyNeuLinkReader(NetworkReader):
-
     component_objects = {}  # Store cell ids vs objects, e.g. NeuroML2 based object
 
     PRE_SYN = "silentSyn"
     POST_SYN = "rsDL"
 
     def __init__(self, **parameters):
-
         print_v("Creating PsyNeuLinkReader with %s..." % parameters)
         self.parameters = parameters
         self.current_population = None
         self.pre_pop = None
         self.post_pop = None
 
     def _generate_id(self, name):
         return (
             name.replace(" ", "_").replace("[", "_").replace("]", "_").replace("-", "_")
         )
 
     def parse(self, handler):
-
         FORMAT = "BIDS-MDF"
         filename = os.path.abspath(self.parameters["filename"])
         id = filename.split("/")[-1].split(".")[0]
 
         self.handler = handler
 
         bids_mdf = load_json(filename)
@@ -262,15 +259,14 @@
                                          self.post_pop,
                                          synapse)
 
             self.post_pop=None"""
 
 
 if __name__ == "__main__":
-
     test_files = [
         "../../neuroConstruct/osb/showcase/PsyNeuLinkShowcase/PsyNeuLink/model_with_simple_graph.json"
     ]
     test_files.append(
         "../../neuroConstruct/osb/showcase/PsyNeuLinkShowcase/NeuroML2/ABC.bids-mdf.json"
     )
     test_files.append(
```

### Comparing `neuromllite-0.5.4/neuromllite/PyNNHandler.py` & `neuromllite-0.5.6/neuromllite/PyNNHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from pyneuroml.pynml import convert_to_units
 
 from importlib import import_module
 
 
 class PyNNHandler(DefaultNetworkHandler):
-
     populations = {}
     projections = {}
     input_sources = {}
     input_info = {}
 
     def __init__(self, simulator, dt, reference):
         print_v("Initiating PyNN with simulator %s" % simulator)
@@ -76,29 +75,26 @@
                 'self.input_sources["%s"] = self.sim.%s(**input_params)'
                 % (input_source.id, input_source.pynn_input)
             )
 
         # print(['%s (%s): %s'%(i, type(self.input_sources[i]),self.input_sources[i].simple_parameters()) for i in self.input_sources])
 
     def handle_document_start(self, id, notes):
-
         print_v("Document: %s" % id)
 
     def handle_network(self, network_id, notes, temperature=None):
-
         print_v("Network: %s" % network_id)
         if temperature:
             print_v("  Temperature: " + temperature)
         if notes:
             print_v("  Notes: " + notes)
 
     def handle_population(
         self, population_id, component, size=-1, component_obj=None, properties={}
     ):
-
         sizeInfo = " as yet unspecified size"
         if size >= 0:
             sizeInfo = ", size: " + str(size) + " cells"
         if component_obj:
             compInfo = " (%s)" % component_obj.__class__.__name__
         else:
             compInfo = ""
@@ -137,15 +133,14 @@
         synapse,
         hasWeights=False,
         hasDelays=False,
         type="projection",
         synapse_obj=None,
         pre_synapse_obj=None,
     ):
-
         synInfo = ""
         if synapse_obj:
             synInfo += " (syn: %s)" % synapse_obj.__class__.__name__
 
         if pre_synapse_obj:
             synInfo += " (pre comp: %s)" % pre_synapse_obj.__class__.__name__
 
@@ -180,30 +175,28 @@
         preSegId=0,
         preFract=0.5,
         postSegId=0,
         postFract=0.5,
         delay=0,
         weight=1,
     ):
-
         # self.print_connection_information(projName, id, prePop, postPop, synapseType, preCellId, postCellId, weight)
         # print_v("Src cell: %d, seg: %f, fract: %f -> Tgt cell %d, seg: %f, fract: %f; weight %s, delay: %s ms" % (preCellId,preSegId,preFract,postCellId,postSegId,postFract, weight, delay))
 
         exec(
             "self.projection__%s_conns.append((%s,%s,float(%s),float(%s)))"
             % (projName, preCellId, postCellId, weight, delay)
         )
 
     #
     #  Should be overridden to handle end of network connection
     #
     def finalise_projection(
         self, projName, prePop, postPop, synapse=None, type="projection"
     ):
-
         print_v(
             "Projection finalising: "
             + projName
             + " from "
             + prePop
             + " to "
             + postPop
@@ -229,15 +222,14 @@
 
     #
     #  Should be overridden to create input source array
     #
     def handle_input_list(
         self, inputListId, population_id, component, size, input_comp_obj=None
     ):
-
         self.print_input_information(inputListId, population_id, component, size)
 
         if size < 0:
             self.log.error(
                 "Error! Need a size attribute in sites element to create spike source!"
             )
             return
@@ -246,15 +238,14 @@
 
     #
     #  Should be overridden to to connect each input to the target cell
     #
     def handle_single_input(
         self, inputListId, id, cellId, segId=0, fract=0.5, weight=1
     ):
-
         # print_v("Input: %s[%s], cellId: %i, seg: %i, fract: %f, weight: %f" % (inputListId,id,cellId,segId,fract,weight))
 
         population_id, component = self.input_info[inputListId]
 
         # exec('print  self.POP_%s'%(population_id))
         # exec('print  self.POP_%s[%s]'%(population_id,cellId))
```

### Comparing `neuromllite-0.5.4/neuromllite/SonataHandler.py` & `neuromllite-0.5.6/neuromllite/SonataHandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,27 @@
 import h5py
 import numpy as np
 from modelspec.utils import save_to_json_file
 import os
 
 
 class SonataHandler(DefaultNetworkHandler):
-
     positions = {}
     pop_indices = {}
 
     DEFAULT_NODE_GROUP_ID = 0
     pop_type_ids = {}
     node_type_csv_info = {}
 
     input_info = {}
 
     def __init__(self):
         print_v("Initiating Sonata handler")
 
     def handle_document_start(self, id, notes):
-
         print_v("Parsing for Sonata export: %s" % id)
 
         self.config_file_info = {}
         self.config_file_info["network"] = "./circuit_config.json"
         self.config_file_info["simulation"] = "./simulation_config.json"
 
         self.circuit_file_info = {}
@@ -60,15 +58,14 @@
             os.mkdir("./components/point_neuron_models_dir")
 
         self.circuit_file_info["networks"] = {}
         self.circuit_file_info["networks"]["nodes"] = []
         self.circuit_file_info["networks"]["nodes"].append({})
 
     def finalise_document(self):
-
         print_v("Writing file...: %s" % id)
         self.sonata_nodes.close()
 
         node_type_filename = "%s_node_types.csv" % self.network_id
 
         self.circuit_file_info["networks"]["nodes"][0]["node_types_file"] = (
             "$NETWORK_DIR/%s" % node_type_filename
@@ -93,15 +90,14 @@
 
         node_type_file.close()
 
         save_to_json_file(self.config_file_info, "config.json", indent=2)
         save_to_json_file(self.circuit_file_info, "circuit_config.json", indent=2)
 
     def handle_network(self, network_id, notes, temperature=None):
-
         print_v("Network: %s" % network_id)
         self.network_id = network_id
 
         if temperature:
             print_v("  Temperature: " + temperature)
         if notes:
             print_v("  Notes: " + notes)
@@ -119,15 +115,14 @@
         )
         self.sonata_nodes.attrs.create("version", [0, 1], dtype=np.uint32)
         self.sonata_nodes.attrs.create("magic", np.uint32(0x0A7A))
 
     def handle_population(
         self, population_id, component, size=-1, component_obj=None, properties={}
     ):
-
         sizeInfo = " as yet unspecified size"
         if size >= 0:
             sizeInfo = ", size: " + str(size) + " cells"
         if component_obj:
             compInfo = " (%s)" % component_obj.__class__.__name__
         else:
             compInfo = ""
@@ -155,28 +150,26 @@
         self.node_type_csv_info[population_id]["model_template"] = "nest:iaf_psc_alpha"
         self.node_type_csv_info[population_id]["model_type"] = "point_process"
         self.node_type_csv_info[population_id]["dynamics_params"] = (
             "%s.json" % component
         )
 
     def handle_location(self, id, population_id, component, x, y, z):
-
         if not population_id in self.positions:
             self.positions[population_id] = np.array([[x, y, z]])
             self.pop_indices[population_id] = np.array([id])
         else:
             self.positions[population_id] = np.concatenate(
                 (self.positions[population_id], [[x, y, z]])
             )
             self.pop_indices[population_id] = np.concatenate(
                 (self.pop_indices[population_id], [id])
             )
 
     def finalise_population(self, population_id):
-
         self.sonata_nodes.create_dataset(
             "nodes/%s/0/positions" % population_id, data=self.positions[population_id]
         )
         self.sonata_nodes.create_dataset(
             "nodes/%s/node_group_index" % population_id,
             data=self.pop_indices[population_id],
         )
@@ -198,15 +191,14 @@
 
     #
     #  Should be overridden to create input source array
     #
     def handle_input_list(
         self, inputListId, population_id, component, size, input_comp_obj=None
     ):
-
         self.print_input_information(inputListId, population_id, component, size)
 
         if size < 0:
             self.log.error(
                 "Error! Need a size attribute in sites element to create spike source!"
             )
             return
@@ -215,15 +207,14 @@
 
     #
     #  Should be overridden to to connect each input to the target cell
     #
     def handle_single_input(
         self, inputListId, id, cellId, segId=0, fract=0.5, weight=1
     ):
-
         print_v(
             "Input: %s[%s], cellId: %i, seg: %i, fract: %f, weight: %f"
             % (inputListId, id, cellId, segId, fract, weight)
         )
 
         self.input_info[inputListId][2].append(cellId)
```

### Comparing `neuromllite-0.5.4/neuromllite/SonataReader.py` & `neuromllite-0.5.6/neuromllite/SonataReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 DUMMY_CELL = "dummy_cell"
 DEFAULT_NEST_SPIKE_SYN = "DEFAULT_NEST_SPIKE_SYN"
 
 REPORT_FILE = "report.txt"
 
 
 def _get_default_nest_syn(nml_doc):
-
     if nml_doc.get_by_id(DEFAULT_NEST_SPIKE_SYN):
         return nml_doc.get_by_id(DEFAULT_NEST_SPIKE_SYN)
 
     from neuroml import AlphaCurrSynapse
 
     nest_syn = AlphaCurrSynapse(id=DEFAULT_NEST_SPIKE_SYN, tau_syn="2")
     nml_doc.alpha_curr_synapses.append(nest_syn)
@@ -86,15 +85,14 @@
     """
 
     component_objects = {}  # Store cell ids vs objects, e.g. NeuroML2 based object
 
     nml_includes = ["PyNN.xml"]
 
     def __init__(self, **parameters):
-
         print_v("Creating SonataReader with %s..." % parameters)
         self.parameters = parameters
 
         self.current_sonata_pop = None
         self.current_node_group = None
         self.cell_info = {}
         self.node_set_mappings = {}
@@ -357,33 +355,30 @@
                         )
                         pop.properties.append(neuroml.Property("region", "L6"))
                 except:
                     pass  # Don't specify a particular color, use random, not a problem...
 
                 properties["color"] = color
                 if True or not "locations" in self.cell_info[sonata_pop]["0"]:
-
                     properties = {}  #############  temp for LEMS...
 
                 if model_type != "virtual":
-
                     self.handler.handle_population(
                         nml_pop_id,
                         pop_comp,
                         size,
                         component_obj=None,
                         properties=properties,
                     )
 
                 types_vs_pops[type] = nml_pop_id
             self.cell_info[sonata_pop]["pop_count"] = {}
             self.cell_info[sonata_pop]["pop_map"] = {}
 
             for i in self.cell_info[sonata_pop]["types"]:
-
                 pop = types_vs_pops[self.cell_info[sonata_pop]["types"][i]]
 
                 if not pop in self.cell_info[sonata_pop]["pop_count"]:
                     self.cell_info[sonata_pop]["pop_count"][pop] = 0
 
                 index = self.cell_info[sonata_pop]["pop_count"][pop]
                 self.cell_info[sonata_pop]["pop_map"][i] = (pop, index)
@@ -408,15 +403,14 @@
 
                 self.cell_info[sonata_pop]["pop_count"][pop] += 1
 
         ########################################################################
         #  Load simulation info into self.simulation_config
 
         if self.simulation_config:
-
             if self.simulation_config:
                 for m in self.simulation_config["manifest"]:
                     path = self.subs(self.simulation_config["manifest"][m])
                     self.substitutes[m] = path
 
             for s1 in ["output"]:
                 for k in self.simulation_config[s1]:
@@ -501,24 +495,22 @@
 
             self.input_comp_info[input] = {}
             self.input_comp_info[input][info["input_type"]] = {}
 
             node_set = info["node_set"]
 
             if info["input_type"] == "current_clamp":
-
                 comp = "PG_%s" % input
                 self.input_comp_info[input][info["input_type"]][comp] = {
                     "amp": info["amp"],
                     "delay": info["delay"],
                     "duration": info["duration"],
                 }
 
                 for nml_pop_id in self.node_set_mappings[node_set]:
-
                     input_list_id = "il_%s_%s" % (input, nml_pop_id)
                     indices = self.node_set_mappings[node_set][nml_pop_id]
 
                     self.handler.handle_input_list(
                         input_list_id, nml_pop_id, comp, len(indices)
                     )
                     count = 0
@@ -575,15 +567,14 @@
                 )
 
         ########################################################################
         #  Use extracted edge info to create connections
 
         projections_created = []
         for conn in self.conn_info:
-
             pre_node = self.conn_info[conn]["pre_node"]
             post_node = self.conn_info[conn]["post_node"]
 
             for i in range(len(self.conn_info[conn]["pre_id"])):
                 pre_id = self.conn_info[conn]["pre_id"][i]
                 post_id = self.conn_info[conn]["post_id"][i]
                 nsyns = (
@@ -659,15 +650,14 @@
                     self.edges_info[conn][type]["delay"]
                     if "delay" in self.edges_info[conn][type]
                     else 0
                 )
 
                 if not pop_type_pre == "virtual":
                     if not proj_id in projections_created:
-
                         self.handler.handle_projection(
                             proj_id, pre_pop, post_pop, synapse
                         )
 
                         projections_created.append(proj_id)
 
                     self.handler.handle_connection(
@@ -739,15 +729,14 @@
                 if g._v_name == "edges":
                     edge_id = node._v_name.replace("-", "_")
                     # print('  Found edge: %s'%edge_id)
                     self.current_edge = edge_id
                     self.conn_info[self.current_edge] = {}
 
                 if g._v_name == self.current_edge:
-
                     self.current_pre_node = g._v_name.split("_to_")[0]
                     self.current_post_node = g._v_name.split("_to_")[1]
                     # print('  Found edge %s -> %s'%(self.current_pre_node, self.current_post_node))
                     self.conn_info[self.current_edge][
                         "pre_node"
                     ] = self.current_pre_node
                     self.conn_info[self.current_edge][
@@ -781,15 +770,14 @@
                 self.cell_info[self.current_sonata_pop][self.current_node_group][
                     "locations"
                 ][i][d.name] = d[i]
 
         elif (
             self.current_sonata_pop
         ):  # e.g. parent group is cortex with child datasets node_id etc.
-
             if d.name == "node_group_id":
                 for i in range(0, d.shape[0]):
                     if not d[i] == 0:
                         raise Exception(
                             "Error: currently only support node_group_id==0!"
                         )
             if d.name == "node_id":
@@ -853,15 +841,14 @@
 
             print_v(" - Adding %s: %s" % (model_template, info))
 
             if (
                 info["model_type"] == "point_process"
                 and model_template == "nest:iaf_psc_alpha"
             ):
-
                 is_nest = True
                 from neuroml import IF_curr_alpha
 
                 pynn0 = IF_curr_alpha(
                     id=c,
                     cm=info["dynamics_params"]["C_m"] / 1000.0,
                     i_offset="0",
@@ -877,15 +864,14 @@
 
                 nml_doc.IF_curr_alpha.append(pynn0)
 
             elif (
                 info["model_type"] == "point_process"
                 and model_template == "NEURON_IntFire1"
             ):
-
                 contents = """<Lems>
     <intFire1Cell id="%s" thresh="1mV" reset="0mV" tau="%sms" refract="%sms"/>
 </Lems>""" % (
                     c,
                     info["dynamics_params"]["tau"] * 1000,
                     info["dynamics_params"]["refrac"] * 1000,
                 )
@@ -897,15 +883,14 @@
 
                 self.nml_includes.append(cell_file_name)
                 self.nml_includes.append(
                     "../../../examples/sonatatest/IntFireCells.xml"
                 )
 
             else:
-
                 from neuroml import IafRefCell
 
                 IafRefCell0 = IafRefCell(
                     id=DUMMY_CELL,
                     C=".2 nF",
                     thresh="1mV",
                     reset="0mV",
@@ -943,15 +928,14 @@
                 # print("Adding syn: %s"%syn)
                 nml_doc.exp_two_synapses.append(syn)
 
             elif (
                 "level_of_detail" in dyn_params
                 and dyn_params["level_of_detail"] == "instanteneous"
             ):
-
                 contents = """<Lems>
     <impulseSynapse id="%s"/>
 </Lems>""" % (
                     s
                 )
 
                 syn_file_name = "%s.xml" % s
@@ -1160,28 +1144,26 @@
         help="Execute the generated LEMS/NeuroML2 model with jNeuroML_NEURON",
     )
 
     return parser.parse_args()
 
 
 def _get_nml_pop_id(quantity):
-
     if "[" in quantity:
         nml_pop = quantity.split("[")[0]
         nml_index = int(quantity.split("[")[1].split("]")[0])
         return nml_pop, nml_index
 
     else:
         nml_pop = quantity.split("/")[0]
         nml_index = int(quantity.split("/")[1])
         return nml_pop, nml_index
 
 
 def run(args):
-
     print_v(
         "Reading Sonata file: %s and generating network: %s"
         % (args.sonata_config_file, args.network_reference)
     )
 
     sr, lems_file_name, nml_file_name, nml_doc = get_neuroml_from_sonata(
         args.sonata_config_file,
@@ -1193,31 +1175,28 @@
     # pp.pprint(sr.cell_info)
     # pp.pprint(sr.nml_ids_vs_gids)
 
     print_v("Generated NeuroML 2 network: %s" % (nml_file_name))
     print_v("Generated LEMS file to run network: %s" % (lems_file_name))
 
     if args.jnml or args.neuron:
-
         traces = None
         events = None
 
         if args.jnml:
-
             from pyneuroml import pynml
 
             traces, events = pynml.run_lems_with_jneuroml(
                 lems_file_name,
                 nogui=True,
                 verbose=True,
                 load_saved_data=True,
                 reload_events=True,
             )
         if args.neuron:
-
             from pyneuroml import pynml
 
             traces, events = pynml.run_lems_with_jneuroml_neuron(
                 lems_file_name,
                 nogui=True,
                 verbose=True,
                 load_saved_data=True,
@@ -1241,26 +1220,24 @@
             time_stop = t[-1] * 1000.0
             time_dt = (t[1] - t[0]) * 1000.0
             time = [time_start, time_stop, time_dt]
 
             nml_q_vs_node_id = {}
 
             for nml_q in traces.keys():
-
                 if nml_q != "t":
                     nml_pop, nml_index = _get_nml_pop_id(nml_q)
                     (sonata_node, sonata_node_id) = sr.nml_ids_vs_gids[nml_pop][
                         nml_index
                     ]
                     nml_q_vs_node_id[nml_q] = sonata_node_id
 
             ordered = sorted(nml_q_vs_node_id, key=nml_q_vs_node_id.get)
 
             for nml_q in ordered:
-
                 if nml_q != "t":
                     v = traces[nml_q]
                     nml_pop, nml_index = _get_nml_pop_id(nml_q)
                     (sonata_node, sonata_node_id) = sr.nml_ids_vs_gids[nml_pop][
                         nml_index
                     ]
 
@@ -1269,15 +1246,14 @@
                         node_info[sonata_node]["data"] = []
                         node_info[sonata_node]["gids"] = []
 
                     node_info[sonata_node]["data"].append([vv * 1000.0 for vv in v])
                     node_info[sonata_node]["gids"].append(sonata_node_id)
 
             for sonata_node in node_info:
-
                 node_grp = h5file.create_group(report_grp, sonata_node)
                 mapping_grp = h5file.create_group(node_grp, "mapping")
 
                 # node_grp = h5file.root
                 # mapping_grp = h5file.create_group(report_grp, 'mapping')
                 gids = node_info[sonata_node]["gids"]
                 h5file.create_array(mapping_grp, "gids", gids)
@@ -1330,15 +1306,14 @@
             )
             from shutil import copyfile
 
             copyfile(REPORT_FILE, log_file)
 
 
 def main(args=None):
-
     if "-test" in sys.argv:
         id = "9_cells"
         id = "300_cells"
         # id = '5_cells_iclamp'
 
         id = "300_intfire"
         id = "small_intfire"
@@ -1364,15 +1339,14 @@
         nml_file_name = '%s.net.nml'%id
         nml_file_name += '.h5'
 
         from neuroml.writers import NeuroMLHdf5Writer
         NeuroMLHdf5Writer.write(nml_doc,nml_file_name)
         print('Written to: %s'%nml_file_name) """
     else:
-
         if args is None:
             args = process_args()
         run(args=args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `neuromllite-0.5.4/neuromllite/__init__.py` & `neuromllite-0.5.6/neuromllite/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import collections
 
-__version__ = "0.5.4"
+__version__ = "0.5.6"
 
 # import pyNN
 # import nest
 
 from typing import List, Dict, Any, Optional, Union, Tuple, Callable, TypeVar, Type
 
 import modelspec
@@ -37,14 +37,15 @@
     def get_locations(self):
         return self.pop_locations
 
 
 @modelspec.define
 class NMLBase(Base):
     """Base class for NeuroML objects."""
+
     notes: str = field(kw_only=True, default=None, validator=optional(instance_of(str)))
 
 
 @modelspec.define
 class Cell(NMLBase):
     """
     A Cell definition.
@@ -55,17 +56,22 @@
         neuroml2_source_file: File name of NeuroML2 file defining the cell
         lems_source_file: File name of LEMS file defining the cell
         neuroml2_cell: Name of standard NeuroML2 cell type
         pynn_cell: Name of standard PyNN cell type
         arbor_cell: Name of standard Arbor cell type
         bindsnet_node: Name of standard BindsNET node
     """
+
     id: str = field(validator=instance_of(str))
-    parameters: Dict[str, Any] = field(default=None, validator=optional(instance_of(dict)))
-    neuroml2_source_file: str = field(default=None, validator=optional(instance_of(str)))
+    parameters: Dict[str, Any] = field(
+        default=None, validator=optional(instance_of(dict))
+    )
+    neuroml2_source_file: str = field(
+        default=None, validator=optional(instance_of(str))
+    )
     lems_source_file: str = field(default=None, validator=optional(instance_of(str)))
     neuroml2_cell: str = field(default=None, validator=optional(instance_of(str)))
     pynn_cell: str = field(default=None, validator=optional(instance_of(str)))
     arbor_cell: str = field(default=None, validator=optional(instance_of(str)))
     bindsnet_node: str = field(default=None, validator=optional(instance_of(str)))
 
 
@@ -78,20 +84,30 @@
         id: Unique identifier for this Synapse
         parameters: Dictionary of parameters for the synapse
         neuroml2_source_file: File name of NeuroML2 file defining the synapse
         lems_source_file: File name of LEMS file defining the synapse
         pynn_synapse_type: The pynn synapse type. Valid values are: "curr_exp", "curr_alpha", "cond_exp", "cond_alpha".
         pynn_receptor_type: The pynn receptor type. Valid values are: "excitatory", "inhibitory".
     """
+
     id: str = field(validator=instance_of(str))
-    parameters: Dict[str, Any] = field(default=None, validator=optional(instance_of(dict)))
-    neuroml2_source_file: str = field(default=None, validator=optional(instance_of(str)))
+    parameters: Dict[str, Any] = field(
+        default=None, validator=optional(instance_of(dict))
+    )
+    neuroml2_source_file: str = field(
+        default=None, validator=optional(instance_of(str))
+    )
     lems_source_file: str = field(default=None, validator=optional(instance_of(str)))
-    pynn_synapse_type: str = field(default=None, validator=optional(in_(["curr_exp", "curr_alpha", "cond_exp", "cond_alpha"])))
-    pynn_receptor_type: str = field(default=None, validator=optional(in_(["excitatory", "inhibitory"])))
+    pynn_synapse_type: str = field(
+        default=None,
+        validator=optional(in_(["curr_exp", "curr_alpha", "cond_exp", "cond_alpha"])),
+    )
+    pynn_receptor_type: str = field(
+        default=None, validator=optional(in_(["excitatory", "inhibitory"]))
+    )
 
 
 @modelspec.define
 class InputSource(NMLBase):
     """
     An InputSource definition.
 
@@ -99,17 +115,22 @@
         id: Unique identifier for this InputSource
         parameters: Dictionary of parameters for the InputSource
         neuroml2_source_file: File name of NeuroML2 file defining the input source
         neuroml2_input: Name of standard NeuroML2 input
         lems_source_file: File name of LEMS file defining the input source
         pynn_input: Name of PyNN input
     """
+
     id: str = field(validator=instance_of(str))
-    parameters: Dict[str, Any] = field(default=None, validator=optional(instance_of(dict)))
-    neuroml2_source_file: str = field(default=None, validator=optional(instance_of(str)))
+    parameters: Dict[str, Any] = field(
+        default=None, validator=optional(instance_of(dict))
+    )
+    neuroml2_source_file: str = field(
+        default=None, validator=optional(instance_of(str))
+    )
     neuroml2_input: str = field(default=None, validator=optional(instance_of(str)))
     lems_source_file: str = field(default=None, validator=optional(instance_of(str)))
     pynn_input: str = field(default=None, validator=optional(instance_of(str)))
 
 
 @modelspec.define
 class RectangularRegion(NMLBase):
@@ -121,14 +142,15 @@
         x: x coordinate of corner of region
         y: y coordinate of corner of region
         z: z coordinate of corner of region
         width: width of the rectangular region
         height: height of the rectangular region
         depth: depth of the rectangular region
     """
+
     id: str = field(validator=instance_of(str))
     x: float = field(validator=instance_of(float), converter=convert2float)
     y: float = field(validator=instance_of(float), converter=convert2float)
     z: float = field(validator=instance_of(float), converter=convert2float)
     width: float = field(validator=instance_of(float), converter=convert2float)
     height: float = field(validator=instance_of(float), converter=convert2float)
     depth: float = field(validator=instance_of(float), converter=convert2float)
@@ -138,28 +160,30 @@
 class RandomLayout(NMLBase):
     """
     A RandomLayout definition.
 
     Args:
         region: Region in which to place population
     """
+
     region: str = field(validator=instance_of(str))
 
 
 @modelspec.define
 class RelativeLayout(NMLBase):
     """
     A RelativeLayout definition.
 
     Args:
         region: The Region relative to which population should be positioned.
         x: x position relative to x coordinate of Region
         y: y position relative to y coordinate of Region
         z: z position relative to z coordinate of Region
     """
+
     region: str = field(validator=instance_of(str))
     x: float = field(validator=instance_of(float), converter=convert2float)
     y: float = field(validator=instance_of(float), converter=convert2float)
     z: float = field(validator=instance_of(float), converter=convert2float)
 
 
 @modelspec.define
@@ -168,27 +192,29 @@
     A Location definition.
 
     Args:
         x: x coordinate of location
         y: y coordinate of location
         z: z coordinate of location
     """
+
     x: float = field(validator=instance_of(float), converter=convert2float)
     y: float = field(validator=instance_of(float), converter=convert2float)
     z: float = field(validator=instance_of(float), converter=convert2float)
 
 
 @modelspec.define
 class SingleLocation(NMLBase):
     """
     A SingleLocation definition.
 
     Args:
         location: Location of the single Cell.
     """
+
     location: Location = field(validator=instance_of(Location))
 
 
 @modelspec.define
 class Population(NMLBase):
     """
     A Population definition.
@@ -198,21 +224,30 @@
         size: The size of the population.
         component: The type of Cell to use in this population.
         properties: A dictionary of properties (metadata) for this population.
         random_layout: Layout in the random RectangularRegion.
         relative_layout: Position relative to RectangularRegion.
         single_location: Explicit location of the one Cell in the population
     """
+
     id: str = field(validator=instance_of(str))
     size: ValueExprType = field(validator=instance_of(value_expr_types))
     component: str = field(validator=instance_of(str))
-    properties: Dict[str, Any] = field(default=None, validator=optional(instance_of(dict)))
-    random_layout: RandomLayout = field(default=None, validator=optional(instance_of(RandomLayout)))
-    relative_layout: RelativeLayout = field(default=None, validator=optional(instance_of(RelativeLayout)))
-    single_location: SingleLocation = field(default=None, validator=optional(instance_of(SingleLocation)))
+    properties: Dict[str, Any] = field(
+        default=None, validator=optional(instance_of(dict))
+    )
+    random_layout: RandomLayout = field(
+        default=None, validator=optional(instance_of(RandomLayout))
+    )
+    relative_layout: RelativeLayout = field(
+        default=None, validator=optional(instance_of(RelativeLayout))
+    )
+    single_location: SingleLocation = field(
+        default=None, validator=optional(instance_of(SingleLocation))
+    )
 
     def has_positions(self):
         """
         Returns True if the population has a position.
 
         Returns:
             True if the population has a position.
@@ -231,34 +266,37 @@
 class RandomConnectivity(NMLBase):
     """
     A RandomConnectivity definition.
 
     Args:
         probability: Random probability of connection.
     """
+
     probability: ValueExprType = field(validator=instance_of(value_expr_types))
 
 
 @modelspec.define
 class OneToOneConnector(NMLBase):
     """
     A OneToOneConnector definition.
     """
+
     pass
 
 
 # Temp! to redefine more generally!
 @modelspec.define
 class ConvergentConnectivity(NMLBase):
     """
     A ConvergentConnectivity definition.
 
     Args:
         num_per_post: Number per post-synaptic neuron.
     """
+
     num_per_post: float = field(validator=instance_of(float), converter=convert2float)
 
 
 @modelspec.define
 class Projection(NMLBase):
     """
     A Projection definition.
@@ -274,25 +312,36 @@
         delay: Delay to use (default: 0)
         weight: Weight to use (default: 1)
         random_connectivity: Use random connectivity
         convergent_connectivity: Use convergent connectivity
         one_to_one_connector: Connect cell index i in pre pop to cell index i in post pop for all i
 
     """
+
     id: str = field(validator=instance_of(str))
     presynaptic: str = field(validator=optional(instance_of(str)))
     postsynaptic: str = field(validator=optional(instance_of(str)))
     synapse: str = field(validator=optional(instance_of(str)))
     pre_synapse: str = field(default=None, validator=optional(instance_of(str)))
     type: str = field(default="projection", validator=optional(instance_of(str)))
-    delay: ValueExprType = field(default=None, validator=optional(instance_of(value_expr_types)))
-    weight: ValueExprType = field(default=None, validator=optional(instance_of(value_expr_types)))
-    random_connectivity: RandomConnectivity = field(default=None, validator=optional(instance_of(RandomConnectivity)))
-    convergent_connectivity: ConvergentConnectivity = field(default=None, validator=optional(instance_of(ConvergentConnectivity)))
-    one_to_one_connector: OneToOneConnector = field(default=None, validator=optional(instance_of(OneToOneConnector)))
+    delay: ValueExprType = field(
+        default=None, validator=optional(instance_of(value_expr_types))
+    )
+    weight: ValueExprType = field(
+        default=None, validator=optional(instance_of(value_expr_types))
+    )
+    random_connectivity: RandomConnectivity = field(
+        default=None, validator=optional(instance_of(RandomConnectivity))
+    )
+    convergent_connectivity: ConvergentConnectivity = field(
+        default=None, validator=optional(instance_of(ConvergentConnectivity))
+    )
+    one_to_one_connector: OneToOneConnector = field(
+        default=None, validator=optional(instance_of(OneToOneConnector))
+    )
 
 
 @modelspec.define
 class Input(NMLBase):
     """
     An Input definition.
 
@@ -306,32 +355,45 @@
         segment_ids: Which segments to target (default: [0])
         weight: Weight to use (default: 1)
     """
 
     id: str = field(validator=instance_of(str))
     input_source: str = field(default=None, validator=optional(instance_of(str)))
     population: str = field(default=None, validator=optional(instance_of(str)))
-    cell_ids: ValueExprType = field(default="", validator=optional(instance_of(value_expr_types)))
-    percentage: float = field(default=None, validator=optional(instance_of(float)), converter=convert2float)
-    number_per_cell: ValueExprType = field(default="", validator=optional(instance_of(value_expr_types)))
-    segment_ids: ValueExprType = field(default="", validator=optional(instance_of(value_expr_types)))
-    weight: ValueExprType = field(default=None, validator=optional(instance_of(value_expr_types)))
+    cell_ids: ValueExprType = field(
+        default="", validator=optional(instance_of(value_expr_types))
+    )
+    percentage: float = field(
+        default=None, validator=optional(instance_of(float)), converter=convert2float
+    )
+    number_per_cell: ValueExprType = field(
+        default="", validator=optional(instance_of(value_expr_types))
+    )
+    segment_ids: ValueExprType = field(
+        default="", validator=optional(instance_of(value_expr_types))
+    )
+    weight: ValueExprType = field(
+        default=None, validator=optional(instance_of(value_expr_types))
+    )
 
 
 @modelspec.define
 class NetworkReader(NMLBase):
     """
     A NetworkReader definition.
 
     Args:
         type: The type of NetworkReader
         parameters: Dictionary of parameters for the NetworkReader
     """
+
     type: str = field(default=None, validator=optional(instance_of(str)))
-    parameters: Dict[str, Any] = field(default=None, validator=optional(instance_of(dict)))
+    parameters: Dict[str, Any] = field(
+        default=None, validator=optional(instance_of(dict))
+    )
 
 
 @modelspec.define
 class Simulation(NMLBase):
     """
     A Simulation definition.
 
@@ -345,24 +407,43 @@
         record_traces: Record traces?
         record_spikes: Record spikes?
         record_rates: Record rates?
         record_variables: Record named variables?
         plots2D: Work in progress...
         plots3D: Work in progress...
     """
+
     id: str = field(validator=instance_of(str))
-    version: str = field(default=f"NeuroMLlite v{__version__}", validator=optional(instance_of(str)), metadata={"omit_if_default": False})
+    version: str = field(
+        default=f"NeuroMLlite v{__version__}",
+        validator=optional(instance_of(str)),
+        metadata={"omit_if_default": False},
+    )
     network: str = field(default=None, validator=optional(instance_of(str)))
-    duration: float = field(default=None, validator=optional(instance_of(float)), converter=convert2float)
-    dt: float = field(default=None, validator=optional(instance_of(float)), converter=convert2float)
-    seed: int = field(default=None, validator=optional(instance_of(int)), converter=convert2int)
-    record_traces: Dict[str, Any] = field(default=None, validator=optional(instance_of(dict)))
-    record_spikes: Dict[str, Any] = field(default=None, validator=optional(instance_of(dict)))
-    record_rates: Dict[str, Any] = field(default=None, validator=optional(instance_of(dict)))
-    record_variables: Dict[str, Any] = field(default=None, validator=optional(instance_of(dict)))
+    duration: float = field(
+        default=None, validator=optional(instance_of(float)), converter=convert2float
+    )
+    dt: float = field(
+        default=None, validator=optional(instance_of(float)), converter=convert2float
+    )
+    seed: int = field(
+        default=None, validator=optional(instance_of(int)), converter=convert2int
+    )
+    record_traces: Dict[str, Any] = field(
+        default=None, validator=optional(instance_of(dict))
+    )
+    record_spikes: Dict[str, Any] = field(
+        default=None, validator=optional(instance_of(dict))
+    )
+    record_rates: Dict[str, Any] = field(
+        default=None, validator=optional(instance_of(dict))
+    )
+    record_variables: Dict[str, Any] = field(
+        default=None, validator=optional(instance_of(dict))
+    )
     plots2D: Dict[str, Any] = field(default=None, validator=optional(instance_of(dict)))
     plots3D: Dict[str, Any] = field(default=None, validator=optional(instance_of(dict)))
 
 
 @modelspec.define
 class Network(NMLBase):
     """
@@ -382,30 +463,37 @@
         seed: Seed for random number generator used when building network
         temperature: Temperature at which to run network (float in deg C)
         network_reader: A class which can read in a network (e.g. from a structured format)
         notes: Human readable notes about the network
     """
 
     id: str = field(validator=instance_of(str))
-    parameters: Dict[str, Any] = field(default=None, validator=optional(instance_of(dict)))
+    parameters: Dict[str, Any] = field(
+        default=None, validator=optional(instance_of(dict))
+    )
     cells: List[Cell] = field(factory=list, validator=instance_of(list))
     synapses: List[Synapse] = field(factory=list, validator=instance_of(list))
     input_sources: List[InputSource] = field(factory=list, validator=instance_of(list))
     regions: List[RectangularRegion] = field(factory=list, validator=instance_of(list))
     populations: List[Population] = field(factory=list, validator=instance_of(list))
     projections: List[Projection] = field(factory=list, validator=instance_of(list))
     inputs: List[Input] = field(factory=list, validator=instance_of(list))
-    version: str = field(default=f"NeuroMLlite v{__version__}", validator=instance_of(str), metadata={"omit_if_default": False})
+    version: str = field(
+        default=f"NeuroMLlite v{__version__}",
+        validator=instance_of(str),
+        metadata={"omit_if_default": False},
+    )
     seed: int = field(default=None, validator=optional(instance_of(int)))
-    temperature: float = field(default=None, validator=optional(instance_of(float)), converter=convert2float)
+    temperature: float = field(
+        default=None, validator=optional(instance_of(float)), converter=convert2float
+    )
     network_reader: NetworkReader = field(default=None)
 
 
 if __name__ == "__main__":
-
     net = Network(id="net")
     doc = net.generate_documentation(format="markdown")
     print(doc)
     with open("../docs/README.md", "w") as d:
         d.write(doc)
 
     import json
```

### Comparing `neuromllite-0.5.4/neuromllite/gui/NMLliteUI.py` & `neuromllite-0.5.6/neuromllite/gui/NMLliteUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,44 +18,40 @@
 from neuromllite.utils import is_spiking_input_population
 from pyneuroml.utils.plot import get_next_hex_color
 
 from functools import partial
 
 
 class ParameterSpinBox(QDoubleSpinBox):
-
-    value_type=float
+    value_type = float
 
     def __init__(self, value, value_type=float):
-
         super(QDoubleSpinBox, self).__init__()
         self.value_type = value_type
         self.setDecimals(18)
         self.setMaximum(1e16)
         self.setMinimum(-1e16)
-        if self.value_type==int:
+        if self.value_type == int:
             self.setSingleStep(1)
         else:
             self.setSingleStep(value / 20.0)
         self.setValue(value_type(value))
 
-
-        #print('ParameterSpinBox: %s/%s (%s/%s), %s'%(value, self.value(), value_type, type(self.value()),self.singleStep()))
+        # print('ParameterSpinBox: %s/%s (%s/%s), %s'%(value, self.value(), value_type, type(self.value()),self.singleStep()))
 
     # TODO: handle a spinner on values like -60mV etc.
     def textFromValue(self, value):
-        return "%i" % value if self.value_type==int else "%s" % value
+        return "%i" % value if self.value_type == int else "%s" % value
 
     # TODO: handle a spinner on values like -60mV etc.
     def final_value(self):
         return self.value_type(self.value())
 
 
 class NMLliteUI(QWidget):
-
     default_vals = {}
 
     simulators = [
         "jNeuroML",
         "jNeuroML_NEURON",
         "jNeuroML_NetPyNE",
         "EDEN",
@@ -86,24 +82,22 @@
 
         self.update_net_sim()
         if self.tabs.currentWidget() == self.nmlliteTab:
             self.update_network_json()
             self.update_simulation_json()
 
     def update_network_json(self):
-
         self.nmlliteNetText.clear()
         try:
             j = self.network.to_json()
             self.nmlliteNetText.insertPlainText(j)
         except Exception as e:
             self.nmlliteNetText.insertPlainText("Error parsing model: %s" % e)
 
     def update_simulation_json(self):
-
         self.nmlliteSimText.clear()
         try:
             j = self.simulation.to_json()
             self.nmlliteSimText.insertPlainText(j)
         except Exception as e:
             self.nmlliteSimText.insertPlainText("Error parsing model: %s" % e)
 
@@ -125,15 +119,14 @@
         name,
         parent_tab_holder,
         image=False,
         figure=False,
         toolbar=False,
         options=False,
     ):
-
         if name in self.all_tabs:
             raise Exception("The name for a tab: %s is already taken!" % name)
 
         thisTab = QWidget()
         parent_tab_holder.addTab(thisTab, name)
         self.all_tabs[name] = thisTab
 
@@ -166,21 +159,21 @@
                 if toolbar:
                     topLayout.addWidget(thisToolbar)
 
         if image:
             label = QLabel(
                 "An image will be generated here. Push the appropriate button on the left"
             )
-            #label.setBackgroundRole(QPalette.Base)
-            #label.setSizePolicy(QSizePolicy.Ignored, QSizePolicy.Ignored)
+            # label.setBackgroundRole(QPalette.Base)
+            # label.setSizePolicy(QSizePolicy.Ignored, QSizePolicy.Ignored)
             label.setScaledContents(True)
             self.all_image_qlabels[name] = label
 
             scrollArea = QScrollArea()
-            #scrollArea.setBackgroundRole(QPalette.Light)
+            # scrollArea.setBackgroundRole(QPalette.Light)
             scrollArea.setWidget(label)
             scrollArea.setVisible(True)
 
             scroolLayout = QGridLayout()
             topLayout.addLayout(scroolLayout, 1, 0)
             scroolLayout.addWidget(scrollArea, 0, 0)
 
@@ -240,15 +233,14 @@
         if simple:
             entry = QLineEdit()
             entry_map[name] = entry
             entry.setText(str(value))
             entry.textChanged.connect(self.updated_param)
 
         else:
-
             try:
                 entry = ParameterSpinBox(value, value_type)
                 entry_map[name] = entry
                 entry.valueChanged.connect(self.updated_param)
 
             except Exception as e:
                 print_v("Error: %s" % e)
@@ -297,15 +289,17 @@
 
         self.sim_base_dir = dirname(nml_sim_file)
 
         if len(self.sim_base_dir) == 0:
             self.sim_base_dir = "."
 
         if self.simulation.network is None:
-            print_v(f"ERROR: The provided simulation file, {nml_sim_file}, does not refer to a network.")
+            print_v(
+                f"ERROR: The provided simulation file, {nml_sim_file}, does not refer to a network."
+            )
             print_v("Please provide a NeuroMLlite simulation file.")
             sys.exit(-1)
 
         self.network = load_network_json(
             "%s/%s" % (self.sim_base_dir, self.simulation.network)
         )
 
@@ -334,29 +328,27 @@
 
         self.tracesTab = QWidget()
         self.plotTabs.addTab(self.tracesTab, "Traces")
         self.heatmapTab = QWidget()
         self.plotTabs.addTab(self.heatmapTab, "Heatmap")
 
         if self.simulation.plots2D is not None:
-
             self.plot2DTab = QTabWidget()
             self.plotTabs.addTab(self.plot2DTab, "2D plots")
 
             self.plot2DTabLayout = QGridLayout()
             self.plot2DTab.setLayout(self.plot2DTabLayout)
 
             for plot2D in self.simulation.plots2D:
                 info = self.simulation.plots2D[plot2D]
                 pLayout = self.add_tab(
                     plot2D, self.plot2DTab, figure=True, toolbar=True, options=True
                 )
 
         if self.simulation.plots3D is not None:
-
             self.plot3DTab = QTabWidget()
             self.plotTabs.addTab(self.plot3DTab, "3D plots")
 
             self.plot3DTabLayout = QGridLayout()
             self.plot3DTab.setLayout(self.plot3DTabLayout)
 
             for plot3D in self.simulation.plots3D:
@@ -538,15 +530,17 @@
                 paramLayout.addWidget(entry, rows, 1)
 
         if self.network.seed is not None:
             rows += 1
             pval = self.network.seed
             label = QLabel("Net generation seed")
             paramLayout.addWidget(label, rows, 0)
-            entry = self.get_value_entry("seed", pval, self.param_entries, value_type=int)
+            entry = self.get_value_entry(
+                "seed", pval, self.param_entries, value_type=int
+            )
             paramLayout.addWidget(entry, rows, 1)
 
         if self.network.temperature is not None:
             rows += 1
             pval = self.network.temperature
             label = QLabel("Temperature")
             paramLayout.addWidget(label, rows, 0)
@@ -598,16 +592,18 @@
 
         for s in svars:
             rows += 1
             sval = self.simulation.__getattribute__(s)
             if sval is not None:
                 label = QLabel("%s" % s)
                 paramLayout.addWidget(label, rows, 0)
-                value_type=int if s=='seed' else float
-                entry = self.get_value_entry(s, sval, self.sim_entries,value_type=value_type)
+                value_type = int if s == "seed" else float
+                entry = self.get_value_entry(
+                    s, sval, self.sim_entries, value_type=value_type
+                )
                 paramLayout.addWidget(entry, rows, 1)
 
         rows += 1
 
         paramLayout.addWidget(QLabel("Simulator:"), rows, 0)
 
         self.simulatorComboBox = QComboBox(self)
@@ -802,16 +798,16 @@
 
             self.add_image(genFile, self.GRAPH_TAB)
 
     def update_net_sim(self):
         """Set the parameters in the network/simulation from the GUI values"""
 
         for p in self.param_entries:
-            #print("Updating: %s to %s (%s)" % (p, self.param_entries[p], type(self.param_entries[p])))
-            if type(self.param_entries[p])==QLineEdit:
+            # print("Updating: %s to %s (%s)" % (p, self.param_entries[p], type(self.param_entries[p])))
+            if type(self.param_entries[p]) == QLineEdit:
                 v = self.param_entries[p].text()
             else:
                 v = self.param_entries[p].final_value()
 
             print_("Setting param %s to %s" % (p, v), self.verbose)
             if p == "seed":
                 self.network.seed = v
@@ -851,14 +847,15 @@
                 return_results=True,
                 base_dir=self.sim_base_dir,
             )
 
             self.replotSimResults()
         except Exception as e:
             import traceback
+
             print(traceback.format_exc())
             self.dialog_popup("Error: %s" % e)
 
     def _get_sorted_population_ids(self, include_input_pops=True):
         all_pop_ids = []
         for pop in self.network.populations:
             if not include_input_pops and is_spiking_input_population(
@@ -870,28 +867,26 @@
         return sorted(all_pop_ids)
 
     def _get_pop_size(self, pop_id):
         pop = self.network.get_child(pop_id, "populations")
         return evaluate(pop.size, self.network.parameters)
 
     def _get_pop_id_cell_id(self, quantity):
-
         if "[" in quantity:
             # e.g. Epop[5]/v
             pop_id = quantity.split("[")[0]
             cell_id = int(quantity.split("[")[1].split("]")[0])
         else:
             # e.g. Epop/0/iafcell/v
             pop_id = quantity.split("/")[0]
             cell_id = int(quantity.split("/")[1])
 
         return pop_id, cell_id
 
     def traceSelect(self):
-
         print_v(
             "traceSelect button was clicked. Traces shown: %s; colours: %s"
             % (self.current_traces_shown, self.current_traces_colours)
         )
 
         dialog = QDialog(self)
         dialog.setWindowTitle("Select which traces to plot")
@@ -926,15 +921,14 @@
                 count += 1
 
         layout.addWidget(buttonBox, count, 1)
         dialog.exec()
         self.replotSimResults()
 
     def traceSelectClicked(self, key):
-
         cb = self.all_cbs[key]
         # print('Clicked: %s, %s, key: %s'%(cb.text(),cb.isChecked(), key))
         self.current_traces_shown[key] = cb.isChecked()
 
     def _eval_at_all(self, expr, parameters, traces):
         tr_present = []
         for t in traces:
@@ -961,15 +955,14 @@
         print_(
             "Generated: %s->%s (#%s)" % (ret_val[0], ret_val[-1], len(ret_val)),
             self.verbose,
         )
         return ret_val
 
     def replotSimResults(self):
-
         simulator = str(self.simulatorComboBox.currentText())
         self.traceSelectButton.setEnabled(True)
 
         info = "Data from sim of %s%s" % (
             self.simulation.id,
             " (%s)" % simulator if simulator else "",
         )
@@ -991,15 +984,14 @@
         ys = []
         labels = []
         colors = []
         colors_used = []
         heat_array = []
 
         for key in sorted(self.current_traces.keys()):
-
             if not key in self.current_traces_shown:
                 self.current_traces_shown[key] = True
 
             if key != "t":
                 heat_array.append(self.current_traces[key])
                 pop_id = key.split("/")[0]
 
@@ -1061,15 +1053,14 @@
                 self.heatmapColorbar.set_label("Firing rate")
 
             self.heatmapCanvas.draw()
 
         ## Plot 2D
 
         if self.simulation.plots2D is not None:
-
             for plot2D in self.simulation.plots2D:
                 info = self.simulation.plots2D[plot2D]
                 fig = self.all_figures[plot2D]
 
                 ax_2d = fig.add_subplot(111)
                 ax_2d.clear()
 
@@ -1126,15 +1117,14 @@
                 fig.legend()
 
                 self.all_canvases[plot2D].draw()
 
         ## Plot 3D
 
         if self.simulation.plots3D is not None:
-
             for plot3D in self.simulation.plots3D:
                 info = self.simulation.plots3D[plot3D]
                 fig = self.all_figures[plot3D]
 
                 # ax_3d = fig.add_subplot(111)
                 from mpl_toolkits.mplot3d import Axes3D
 
@@ -1200,15 +1190,14 @@
                 for t in spikes:
                     ids_for_pop[pop_id].append(cell_id)
                     ts_for_pop[pop_id].append(t)
 
         max_id = 0
 
         for pop_id in sorted(ids_for_pop.keys()):
-
             if pop_id in pop_colors:
                 c = pop_colors[pop_id]
             else:
                 c = get_next_hex_color()
 
             if pop_id in ts_for_pop:
                 shifted_ids = [id + max_id for id in ids_for_pop[pop_id]]
@@ -1329,15 +1318,14 @@
     nmlui = NMLliteUI(nml_sim_file)
     nmlui.show()
 
     sys.exit(app.exec())
 
 
 def usage():
-
     from neuromllite import __version__ as version
 
     MAIN_CLA = "nmllite-ui"
     USAGE = """
 NMLlite-UI v{0}: A GUI for loading NeuroMLlite files
 
 Usage:
```

### Comparing `neuromllite-0.5.4/neuromllite/sweep/GenerateTests.py` & `neuromllite-0.5.6/neuromllite/sweep/GenerateTests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from neuromllite import *
 from neuromllite.NetworkGenerator import *
 from neuromllite.utils import create_new_model
 import sys
 
 
 if __name__ == "__main__":
-
     hhcell = Cell(
         id="hhcell", neuroml2_source_file="../../examples/test_files/hhcell.cell.nml"
     )
 
     iclamp = InputSource(
         id="iclamp_0",
         neuroml2_input="PulseGenerator",
```

### Comparing `neuromllite-0.5.4/neuromllite/sweep/ParameterSweep.py` & `neuromllite-0.5.6/neuromllite/sweep/ParameterSweep.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         save_plot_all_to=None,
         heatmap_all=False,
         save_heatmap_to=None,
         heatmap_lims=None,
         show_plot_already=False,
         peak_threshold=0,
     ):
-
         self.sim = load_simulation_json(runner.nmllite_sim)
 
         self.colormap = "jet"
 
         ps_id = "ParamSweep_%s_%s" % (
             self.sim.id,
             time.ctime().replace(" ", "_").replace(":", "."),
@@ -115,15 +114,14 @@
 
     def _rem_key(self, d, key):
         r = dict(d)
         del r[key]
         return r
 
     def _sweep(self, v, f, reference=""):
-
         keys = list(v)
 
         if len(keys) > 1:
             vals = v[keys[0]]
             others = v
             others = self._rem_key(others, keys[0])
             for val in vals:
@@ -155,29 +153,27 @@
     def _get_sim_duration_ms(self, parameters):
         if "duration" in parameters:
             return parameters["duration"]
         else:
             return self.sim.duration
 
     def _run_all(self):
-
         import pp
 
         ppservers = ()
         job_server = pp.Server(self.num_parallel_runs, ppservers=ppservers)
         print_v(
             "\n  == Running %i jobs across %i local processes\n "
             % (self.total_todo, job_server.get_ncpus())
         )
         jobs = []
         job_refs = {}
 
         submitted = 0
         for ref in self.report["Simulations"]:
-
             report_here = self.report["Simulations"][ref]
 
             params = report_here["parameters"]
             print_v("---- Submitting %s: %s" % (ref, params))
 
             job_dir = os.path.join(self.result_dir, ref)
             os.mkdir(job_dir)
@@ -329,27 +325,25 @@
             )
 
         job_server.print_stats()
         job_server.destroy()
         print_v("-------------------------------------------")
 
     def run(self):
-
         print_v("Running...")
         self._sweep(self.vary, self.fixed)
         self._run_all()
 
         if self.plot_all and self.save_plot_all_to:
             print_v(
                 "Saving image to %s of plot" % (os.path.abspath(self.save_plot_all_to))
             )
             plt.savefig(self.save_plot_all_to, bbox_inches="tight")
 
         if self.heatmap_all:
-
             self.hm_fig, self.hm_ax = plt.subplots()
             z = np.array(self.hm_z)
 
             print_v(
                 "Plotting x: %s->%s (%i), y: %s->%s (%i), z: %s->%s (%i)"
                 % (
                     self.hm_x[0],
@@ -405,30 +399,28 @@
 
         if self.show_plot_already:
             plt.show()
 
         return self.report
 
     def print_report(self):
-
         print_v("--- REPORT:")
         import json
 
         print_v(json.dumps(self.report, indent=4))
 
     def plotLines(
         self,
         first_param,
         value,
         second_param=None,
         save_figure_to=None,
         logx=False,
         logy=False,
     ):
-
         all_pvals = OrderedDict()
         all_lines = OrderedDict()
 
         all_traces = []
 
         DEFAULT_TRACE = self.sim.id
         if not second_param:
@@ -486,15 +478,14 @@
         ys = []
         labels = []
         markers = []
         colors = []
         maxy = -1 * sys.float_info.max
 
         for t in all_traces:
-
             for ref in all_lines[t]:
                 print_v("Add data %s, %s" % (t, ref))
 
                 xs.append(all_pvals[t][ref])
                 ys.append(all_lines[t][ref])
 
                 maxy = max(maxy, max(all_lines[t][ref]))
@@ -542,15 +533,14 @@
             show_plot_already=False,
             legend_position="right",
             save_figure_to=save_figure_to,
         )  # Save figure
 
 
 def run_instance(runner, i, total, job_dir, params):
-
     print(
         "============================================================= \n\n"
         + "     Instance (%s of %s): %s\n" % (i, total, params)
     )
 
     return runner.run_once(job_dir, **params)
 
@@ -560,28 +550,26 @@
     multiple supported simulators, potentially with some parameters changed, and can plot
     the activity of the cells in the simulations
 """
 
 
 class NeuroMLliteRunner:
     def __init__(self, nmllite_sim, simulator="jNeuroML"):
-
         real_sim = os.path.realpath(nmllite_sim)
         print_v("Created NeuroMLliteRunner to run %s in %s" % (real_sim, simulator))
 
         self.base_dir = os.path.dirname(real_sim)
         self.nmllite_sim = nmllite_sim
         self.simulator = simulator
 
     """
         Run a single instance of the simulation, changing the parameters specified
     """
 
     def run_once(self, job_dir, **kwargs):
-
         from neuromllite.utils import print_v
         from neuromllite.utils import load_simulation_json, load_network_json
         from neuromllite.NetworkGenerator import generate_and_run
         from pyneuroml.pynml import get_value_in_si
 
         print_v("Running NeuroMLlite simulation in dir: %s..." % job_dir)
         sim = load_simulation_json(self.nmllite_sim)
@@ -617,15 +605,14 @@
 
         print_v("Returned traces: %s, events: %s" % (traces.keys(), events.keys()))
 
         return traces, events
 
 
 if __name__ == "__main__":
-
     if "-2d" in sys.argv:
         fixed = {"dt": 0.025}
         vary = {
             "stim_amp": ["%spA" % (i) for i in xrange(-40, 220, 40)],
             "stim_del": ["%sms" % (i) for i in xrange(10, 40, 10)],
         }
 
@@ -755,15 +742,14 @@
         )
 
         import matplotlib.pyplot as plt
 
         plt.show()
 
     elif "-run" in sys.argv:
-
         simulator = "jNeuroML_NetPyNE"
         simulator = "jNeuroML"
         # simulator = 'PyNN_NEST'
         nmllr = NeuroMLliteRunner(
             "../../examples/SimExample7.json", simulator=simulator
         )
```

### Comparing `neuromllite-0.5.4/neuromllite/utils.py` & `neuromllite-0.5.6/neuromllite/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
     except OSError as e:
         print_v(f"ERROR opening file: {filename}: {e.strerror}")
 
     return sim
 
 
 def get_pops_vs_cell_indices_seg_ids(recordSpec, network):
-
     pvc = {}
     if recordSpec is not None:
         for p in recordSpec:
             indices = recordSpec[p]
             if p == "all":
                 for pop in network.populations:
                     cell_indices_seg_ids = _generate_cell_indices_seg_ids(
@@ -128,15 +127,14 @@
                 )
                 pvc[p] = cell_indices_seg_ids
 
     return pvc
 
 
 def _generate_cell_indices_seg_ids(pop_id, indices_segids, network):
-
     a = {}
     pop = network.get_child(pop_id, "populations")
 
     if not isinstance(indices_segids, str) or not ":" in indices_segids:
         seg_ids = None
         indices = indices_segids
     else:
@@ -155,15 +153,14 @@
         print_v("Parsed %s (full: %s) as %s" % (indices, indices_segids, l))
         for index in l:
             a[index] = seg_ids
     return a
 
 
 def is_spiking_input_population(population, network):
-
     cell = network.get_child(population.component, "cells")
 
     return is_spiking_input_cell(cell)
 
 
 def is_spiking_input_cell(cell):
     if cell.pynn_cell:
@@ -191,15 +188,14 @@
     color_for_default_population="0.8 0 0",
     input_for_default_population=None,
     synapses=[],
     simulation_seed=12345,
     network_filename=None,
     simulation_filename=None,
 ):
-
     ################################################################################
     ###   Build a new network
 
     net = Network(id=reference)
     net.notes = "A network model: %s" % reference
     net.temperature = temperature  # degC
     if parameters:
@@ -257,15 +253,14 @@
 
     net.projections[0].random_connectivity=RandomConnectivity(probability=0.5)"""
 
     ################################################################################
     ###   Add some inputs
 
     if input_for_default_population:
-
         net.input_sources.append(input_for_default_population)
 
         net.inputs.append(
             Input(
                 id="Stim_%s" % input_for_default_population.id,
                 input_source=input_for_default_population.id,
                 population=pop.id,
```

### Comparing `neuromllite-0.5.4/neuromllite.egg-info/PKG-INFO` & `neuromllite-0.5.6/neuromllite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuromllite
-Version: 0.5.4
+Version: 0.5.6
 Summary: A common JSON/YAML based format for compact network specification, closely tied to NeuroML v2
 Home-page: https://github.com/NeuroML/NeuroMLlite
 Author: Padraig Gleeson
 Author-email: p.gleeson@gmail.com
 License: LICENSE.lesser
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `neuromllite-0.5.4/neuromllite.egg-info/SOURCES.txt` & `neuromllite-0.5.6/neuromllite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.4/setup.py` & `neuromllite-0.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     },
     url="https://github.com/NeuroML/NeuroMLlite",
     license="LICENSE.lesser",
     description="A common JSON/YAML based format for compact network specification, closely tied to NeuroML v2",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     install_requires=[
-        "libNeuroML>=0.4.0",
+        "libNeuroML>=0.5.1",
         "pyyaml",
         "numpy",
         "tables",
         "h5py",
         "modelspec>=0.2.6",
     ],
     classifiers=[
```

