# Comparing `tmp/cmem_plugin_pyshacl-4.2.0rc2.tar.gz` & `tmp/cmem_plugin_pyshacl-4.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_pyshacl-4.2.0rc2.tar", max compression
+gzip compressed data, was "cmem_plugin_pyshacl-4.2.0rc3.tar", max compression
```

## Comparing `cmem_plugin_pyshacl-4.2.0rc2.tar` & `cmem_plugin_pyshacl-4.2.0rc3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11334 2023-05-05 09:08:21.676634 cmem_plugin_pyshacl-4.2.0rc2/LICENSE
--rw-r--r--   0        0        0     4312 2023-05-05 09:08:21.676634 cmem_plugin_pyshacl-4.2.0rc2/README-public.md
--rwxr-xr-x   0        0        0       46 2023-05-05 09:08:51.840615 cmem_plugin_pyshacl-4.2.0rc2/cmem_plugin_pyshacl/__init__.py
--rw-r--r--   0        0        0    27570 2023-05-05 09:08:21.676634 cmem_plugin_pyshacl-4.2.0rc2/cmem_plugin_pyshacl/plugin_pyshacl.py
--rw-r--r--   0        0        0     1875 2023-05-05 09:08:51.836615 cmem_plugin_pyshacl-4.2.0rc2/pyproject.toml
--rw-r--r--   0        0        0     5684 1970-01-01 00:00:00.000000 cmem_plugin_pyshacl-4.2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-05-31 19:23:02.012192 cmem_plugin_pyshacl-4.2.0rc3/LICENSE
+-rw-r--r--   0        0        0     4312 2023-05-31 19:23:02.012192 cmem_plugin_pyshacl-4.2.0rc3/README-public.md
+-rwxr-xr-x   0        0        0       46 2023-05-31 19:23:30.688567 cmem_plugin_pyshacl-4.2.0rc3/cmem_plugin_pyshacl/__init__.py
+-rw-r--r--   0        0        0    26844 2023-05-31 19:23:02.012192 cmem_plugin_pyshacl-4.2.0rc3/cmem_plugin_pyshacl/plugin_pyshacl.py
+-rw-r--r--   0        0        0     1875 2023-05-31 19:23:30.680567 cmem_plugin_pyshacl-4.2.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     5684 1970-01-01 00:00:00.000000 cmem_plugin_pyshacl-4.2.0rc3/PKG-INFO
```

### Comparing `cmem_plugin_pyshacl-4.2.0rc2/LICENSE` & `cmem_plugin_pyshacl-4.2.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_pyshacl-4.2.0rc2/README-public.md` & `cmem_plugin_pyshacl-4.2.0rc3/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_plugin_pyshacl-4.2.0rc2/cmem_plugin_pyshacl/plugin_pyshacl.py` & `cmem_plugin_pyshacl-4.2.0rc3/cmem_plugin_pyshacl/plugin_pyshacl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,271 +1,291 @@
 """
 CMEM plugin for SHACl validation using pySHACL
 """
 from os import remove
-from os.path import getsize, basename
+from os.path import getsize
 from time import time
 from datetime import datetime
 from uuid import uuid4
 from collections import OrderedDict
 from validators import url as validator_url
-from rdflib import Graph, URIRef, Literal, BNode, RDF, SH, PROV, XSD, RDFS, SKOS,\
-    Namespace
+from rdflib import (
+    Graph,
+    URIRef,
+    Literal,
+    BNode,
+    RDF,
+    SH,
+    PROV,
+    XSD,
+    RDFS,
+    SKOS,
+    Namespace,
+)
 from pyshacl import validate
 from strtobool import strtobool
 from cmem.cmempy.dp.proxy.graph import get, post_streamed
 from cmem_plugin_base.dataintegration.context import ExecutionContext
 from cmem_plugin_base.dataintegration.utils import setup_cmempy_user_access
-from cmem_plugin_base.dataintegration.description import Plugin, \
-    PluginParameter
-from cmem_plugin_base.dataintegration.types import BoolParameterType, \
-    StringParameterType
-from cmem_plugin_base.dataintegration.parameter.graph import GraphParameterType, \
-    get_graphs_list
+from cmem_plugin_base.dataintegration.description import Plugin, PluginParameter
+from cmem_plugin_base.dataintegration.types import (
+    BoolParameterType,
+    StringParameterType,
+)
+from cmem_plugin_base.dataintegration.parameter.graph import (
+    GraphParameterType,
+    get_graphs_list,
+)
 from cmem_plugin_base.dataintegration.parameter.choice import ChoiceParameterType
 from cmem_plugin_base.dataintegration.plugins import WorkflowPlugin
-from cmem_plugin_base.dataintegration.entity import Entities, Entity, EntitySchema, \
-    EntityPath
+from cmem_plugin_base.dataintegration.entity import (
+    Entities,
+    Entity,
+    EntitySchema,
+    EntityPath,
+)
 from cmem_plugin_base.dataintegration.discovery import discover_plugins_in_module
 
 SKOSXL = Namespace("http://www.w3.org/2008/05/skos-xl#")
 DATA_GRAPH_TYPES = [
-                    "https://vocab.eccenca.com/di/Dataset",
-                    "http://rdfs.org/ns/void#Dataset",
-                    "https://vocab.eccenca.com/shui/ShapeCatalog",
-                    "http://www.w3.org/2002/07/owl#Ontology",
-                    "https://vocab.eccenca.com/dsm/ThesaurusProject"
+    "https://vocab.eccenca.com/di/Dataset",
+    "http://rdfs.org/ns/void#Dataset",
+    "https://vocab.eccenca.com/shui/ShapeCatalog",
+    "http://www.w3.org/2002/07/owl#Ontology",
+    "https://vocab.eccenca.com/dsm/ThesaurusProject",
 ]
 
 
 def e_t(start):
     """
     calculate rounded elapsed time
     """
     return round(time() - start, 3)
 
 
 def get_label(graph, subject):
     """
     get preferred label
     """
-    labels = preferred_label(graph, subject, label_properties=(
-        RDFS.label,
-        SKOSXL.prefLabel/SKOSXL.literalForm,
-        SKOS.prefLabel
-    ))
+    labels = preferred_label(graph, subject)
     if labels:
         return labels[0][1]
     return None
 
 
 def preferred_label(
-        graph,
-        subject,
-        lang=None,
-        default=None,
-        label_properties=(SKOS.prefLabel, RDFS.label)
-        ):
+    graph,
+    subject,
+    lang=None,
+    default=None,
+    label_properties=(
+        RDFS.label,
+        SKOSXL.prefLabel / SKOSXL.literalForm,
+        SKOS.prefLabel,
+    ),
+):
     """
     adapted from rdflib 6.1.1, function removed in rdflib 6.2.0
     """
     if default is None:
         default = []
     # setup the language filtering
     if lang is not None:
         if lang == "":  # we only want not language-tagged literals
+
             def langfilter(lbl):
                 return lbl.language is None
+
         else:
+
             def langfilter(lbl):
                 return lbl.language == lang
+
     else:  # we don't care about language tags
+
         def langfilter(lbl):
             lbl = True
             return lbl
+
     for label_prop in label_properties:
         labels = list(filter(langfilter, graph.objects(subject, label_prop)))
         if len(labels) == 0:
             continue
         return [(label_prop, lbl) for lbl in labels]
     return default
 
 
 @Plugin(
     label="SHACL validation with pySHACL",
     plugin_id="shacl-pyshacl",
     description="Performs SHACL validation with pySHACL.",
     documentation="Performs SHACL validation with "
-                  "[pySHACL](https://github.com/RDFLib/pySHACL). Select a "
-                  "__Data graph__ and a __SHACL shapes graph__ to get started. The "
-                  "plugin can output __Entities__, and/or produce a more detailed "
-                  "__Validation graph__ by specifying a __Validation graph URI__. "
-                  "Additional configuration parameters can be set to control the "
-                  "output generated by the plugin. Refer to each parameter "
-                  "description for details.",
+    "[pySHACL](https://github.com/RDFLib/pySHACL). Select a "
+    "__Data graph__ and a __SHACL shapes graph__ to get started. The "
+    "plugin can output __Entities__, and/or produce a more detailed "
+    "__Validation graph__ by specifying a __Validation graph URI__. "
+    "Additional configuration parameters can be set to control the "
+    "output generated by the plugin. Refer to each parameter "
+    "description for details.",
     parameters=[
         PluginParameter(
             param_type=GraphParameterType(classes=DATA_GRAPH_TYPES),
             name="data_graph_uri",
             label="Data graph URI",
             description="The URI of the graph to be validated. The graph URI is "
-                        "selected from a list of graphs of types `void:Dataset`, "
-                        "`shui:ShapeCatalog`, `owl:Ontology` and "
-                        "`dsm:ThesaurusProject`."
+            "selected from a list of graphs of types `void:Dataset`, "
+            "`shui:ShapeCatalog`, `owl:Ontology` and "
+            "`dsm:ThesaurusProject`.",
         ),
         PluginParameter(
-            param_type=GraphParameterType(classes=[
-                "https://vocab.eccenca.com/shui/ShapeCatalog"
-            ]),
+            param_type=GraphParameterType(
+                classes=["https://vocab.eccenca.com/shui/ShapeCatalog"]
+            ),
             name="shacl_graph_uri",
             label="SHACL shapes graph URI",
             description="The URI of the graph containing the SHACL shapes to be "
-                        "validated against. The graph URI is selected from a list of "
-                        "graphs of type `shui:ShapeCatalog`."
+            "validated against. The graph URI is selected from a list of "
+            "graphs of type `shui:ShapeCatalog`.",
         ),
         PluginParameter(
             param_type=StringParameterType(),
             name="validation_graph_uri",
             label="Validation graph URI",
             description="If the `Generate validation graph` option is enabled the "
-                        "validation graph is posted to the CMEM instance with this "
-                        "graph URI.",
-            default_value=""
+            "validation graph is posted to the CMEM instance with this "
+            "graph URI.",
+            default_value="",
         ),
         PluginParameter(
             param_type=BoolParameterType(),
             name="generate_graph",
             label="Generate validation graph",
             description="If enabled, the validation graph is posted to the CMEM "
-                        "instance with the graph URI specified with the `Validation "
-                        "graph URI` option.",
-            default_value=False
+            "instance with the graph URI specified with the `Validation "
+            "graph URI` option.",
+            default_value=False,
         ),
         PluginParameter(
             param_type=BoolParameterType(),
             name="output_entities",
             label="Output entities",
             description="If enabled, the plugin outputs the validation results as "
-                        "entities and can be connected to, for instance, a CSV "
-                        "dataset to produce a results table.",
-            default_value=False
+            "entities and can be connected to, for instance, a CSV "
+            "dataset to produce a results table.",
+            default_value=False,
         ),
         PluginParameter(
             param_type=BoolParameterType(),
             name="clear_validation_graph",
             label="Clear validation graph",
             description="If enabled, the validation graph is cleared before workflow "
-                        "execution.",
-            default_value=True
+            "execution.",
+            default_value=True,
         ),
         PluginParameter(
             param_type=BoolParameterType(),
             name="owl_imports",
             label="Resolve owl:imports",
             description="If enabled, the graph tree defined with owl:imports in the "
-                        "data graph is resolved.",
+            "data graph is resolved.",
             default_value=True,
-            advanced=True
+            advanced=True,
         ),
         PluginParameter(
             param_type=BoolParameterType(),
             name="skolemize",
             label="Blank node skolemization",
             description="If enabled, blank nodes in the validation graph are "
-                        "skolemized into URIs.",
+            "skolemized into URIs.",
             default_value=True,
-            advanced=True
+            advanced=True,
         ),
         PluginParameter(
             param_type=BoolParameterType(),
             name="add_labels",
             label="Add labels",
             description="If enabled, `rdfs:label` triples are added to the validation "
-                        "graph for instances of `sh:ValidationReport` and "
-                        "`sh:ValidationResult`.",
+            "graph for instances of `sh:ValidationReport` and "
+            "`sh:ValidationResult`.",
             default_value=True,
-            advanced=True
+            advanced=True,
         ),
         PluginParameter(
             param_type=BoolParameterType(),
             name="include_graphs_labels",
             label="Add labels to focus nodes and values",
             description="If enabled along with the `Add labels` option, `rdfs:label` "
-                        "triples are added for the focus nodes, values and SHACL "
-                        "shapes in the validation graph. The labels are taken from "
-                        "the specified data and SHACL graphs.",
+            "triples are added for the focus nodes, values and SHACL "
+            "shapes in the validation graph. The labels are taken from "
+            "the specified data and SHACL graphs.",
             default_value=False,
-            advanced=True
+            advanced=True,
         ),
         PluginParameter(
             param_type=BoolParameterType(),
             name="add_shui_conforms",
             label="Add shui:conforms flag to focus node resources.",
             description="If enabled, `shui:conforms false` triples are added to the "
-                        "focus nodes in the validation graph.",
+            "focus nodes in the validation graph.",
             default_value=False,
-            advanced=True
+            advanced=True,
         ),
         PluginParameter(
             param_type=BoolParameterType(),
             name="meta_shacl",
             label="Meta-SHACL",
             description="If enabled, the SHACL shapes graph is validated against the "
-                        "SHACL-SHACL shapes graph before validating the data graph.",
+            "SHACL-SHACL shapes graph before validating the data graph.",
             default_value=False,
-            advanced=True
+            advanced=True,
         ),
         PluginParameter(
-            param_type=GraphParameterType(classes=[
-                "http://www.w3.org/2002/07/owl#Ontology"
-            ]),
+            param_type=GraphParameterType(
+                classes=["http://www.w3.org/2002/07/owl#Ontology"]
+            ),
             name="ontology_graph_uri",
             label="Ontology graph URI",
             description="The URI of a graph containing extra ontological information. "
-                        "RDFS and OWL definitions from this are used to inoculate the "
-                        "data graph. The graph URI is selected from a list of graphs "
-                        "of type `owl:Ontology`.",
+            "RDFS and OWL definitions from this are used to inoculate the "
+            "data graph. The graph URI is selected from a list of graphs "
+            "of type `owl:Ontology`.",
             default_value="",
-            advanced=True
+            advanced=True,
         ),
         PluginParameter(
             param_type=ChoiceParameterType(
                 OrderedDict(
-                    {
-                        "none": "None",
-                        "rdfs": "RDFS",
-                        "owlrl": "OWLRL",
-                        "both": "Both"
-                    }
+                    {"none": "None", "rdfs": "RDFS", "owlrl": "OWLRL", "both": "Both"}
                 )
             ),
             name="inference",
             label="Inference",
             description="If enabled, OWL inferencing expansion of the data graph is "
-                        "performed before validation. Options are RDFS, OWLRL, Both, "
-                        "None.",
+            "performed before validation. Options are RDFS, OWLRL, Both, "
+            "None.",
             default_value="none",
-            advanced=True
+            advanced=True,
         ),
         PluginParameter(
             param_type=BoolParameterType(),
             name="advanced",
             label="SHACL Advanced Features",
             description="Enable SHACL Advanced Features.",
             default_value=False,
-            advanced=True
-        )
-    ]
+            advanced=True,
+        ),
+    ],
 )
 # pylint: disable-msg=too-many-instance-attributes
 # pylint: disable-msg=too-many-arguments
 class ShaclValidation(WorkflowPlugin):
     """
     Plugin class
     """
+
     def __init__(
         self,
         data_graph_uri,
         shacl_graph_uri,
         ontology_graph_uri,
         generate_graph,
         validation_graph_uri,
@@ -274,15 +294,15 @@
         owl_imports,
         skolemize,
         add_labels,
         include_graphs_labels,
         add_shui_conforms,
         meta_shacl,
         inference,
-        advanced
+        advanced,
     ) -> None:
         self.data_graph_uri = data_graph_uri
         self.shacl_graph_uri = shacl_graph_uri
         self.ontology_graph_uri = ontology_graph_uri
         self.validation_graph_uri = validation_graph_uri
         self.generate_graph = generate_graph
         self.output_entities = output_entities
@@ -295,155 +315,154 @@
         self.meta_shacl = meta_shacl
         self.inference = inference
         self.advanced = advanced
 
         discover_plugins_in_module("cmem_plugin_pyshacl")
         this_plugin = Plugin.plugins[0]
 
-        self.bool_parameters = [p.name for p in this_plugin.parameters if
-                                isinstance(p.param_type, BoolParameterType)]
-        self.graph_parameters = [p.name for p in this_plugin.parameters if
-                                 isinstance(p.param_type, GraphParameterType)]
+        self.bool_parameters = [
+            p.name
+            for p in this_plugin.parameters
+            if isinstance(p.param_type, BoolParameterType)
+        ]
+        self.graph_parameters = [
+            p.name
+            for p in this_plugin.parameters
+            if isinstance(p.param_type, GraphParameterType)
+        ]
 
     def add_prov(self, validation_graph, utctime):
         """
         add provenance data
         """
         self.log.info("Adding PROV information validation graph")
         validation_report_uri = validation_graph.value(
-            predicate=RDF.type,
-            object=SH.ValidationReport
+            predicate=RDF.type, object=SH.ValidationReport
+        )
+        validation_graph.add(
+            (validation_report_uri, PROV.wasDerivedFrom, URIRef(self.data_graph_uri))
+        )
+        validation_graph.add(
+            (validation_report_uri, PROV.wasInformedBy, URIRef(self.shacl_graph_uri))
+        )
+        validation_graph.add(
+            (
+                validation_report_uri,
+                PROV.generatedAtTime,
+                Literal(utctime, datatype=XSD.dateTime),
+            )
         )
-        validation_graph.add((
-            validation_report_uri,
-            PROV.wasDerivedFrom,
-            URIRef(self.data_graph_uri)
-        ))
-        validation_graph.add((
-            validation_report_uri,
-            PROV.wasInformedBy,
-            URIRef(self.shacl_graph_uri)
-        ))
-        validation_graph.add((
-            validation_report_uri,
-            PROV.generatedAtTime,
-            Literal(utctime, datatype=XSD.dateTime)
-        ))
         return validation_graph
 
     def add_labels_val(
-            self,
-            validation_graph,
-            data_graph,
-            shacl_graph,
-            validation_result_uris):
+        self, validation_graph, data_graph, shacl_graph, validation_result_uris
+    ):
         """
         add labels
         """
         self.log.info("Adding labels to validation graph")
         focus_nodes = []
         validation_report_uri = validation_graph.value(
-            predicate=RDF.type,
-            object=SH.ValidationReport
+            predicate=RDF.type, object=SH.ValidationReport
         )
         conforms = validation_graph.value(
-            subject=validation_report_uri,
-            predicate=SH.conforms
+            subject=validation_report_uri, predicate=SH.conforms
         )
-        label = "SHACL validation report, conforms" if conforms == "true" \
+        label = (
+            "SHACL validation report, conforms"
+            if conforms == "true"
             else "SHACL validation report, nonconforms"
+        )
         validation_graph.add((validation_report_uri, RDFS.label, Literal(label)))
         for validation_result_uri in validation_result_uris:
-            message = str(validation_graph.value(
-                subject=validation_result_uri,
-                predicate=SH.resultMessage
-            ))
-            # result_path = str(validation_graph.value(
-            #     subject=validation_result_uri,
-            #     predicate=SH.resultPath
-            # )).split("/")[-1]
-            result_path = basename(validation_graph.value(
-                subject=validation_result_uri,
-                predicate=SH.resultPath
-            ))
-            label = f"SHACL: {result_path}: {message}"
+            message = str(
+                validation_graph.value(
+                    subject=validation_result_uri, predicate=SH.resultMessage
+                )
+            )
+            result_path = validation_graph.value(
+                subject=validation_result_uri, predicate=SH.resultPath
+            )
+            result_path_string = f"{result_path}: " if result_path else ""
+            label = f"SHACL: {result_path_string}{message}"
             validation_graph.add((validation_result_uri, RDFS.label, Literal(label)))
             if self.include_graphs_labels:
                 focus_node = validation_graph.value(
-                    subject=validation_result_uri,
-                    predicate=SH.focusNode
+                    subject=validation_result_uri, predicate=SH.focusNode
                 )
                 if self.add_shui_conforms:
                     focus_nodes.append(focus_node)
                 label = get_label(data_graph, focus_node)
                 if label:
                     validation_graph.add((focus_node, RDFS.label, label))
                 value = validation_graph.value(
-                    subject=validation_result_uri,
-                    predicate=SH.value
+                    subject=validation_result_uri, predicate=SH.value
                 )
                 if value:
                     if isinstance(value, (URIRef, BNode)):
                         label = get_label(data_graph, value)
                         if label:
                             validation_graph.add((value, RDFS.label, label))
                 source_shape = validation_graph.value(
-                    subject=validation_result_uri,
-                    predicate=SH.sourceShape
+                    subject=validation_result_uri, predicate=SH.sourceShape
                 )
                 label = get_label(shacl_graph, source_shape)
                 if label:
                     validation_graph.add((source_shape, RDFS.label, label))
         return validation_graph, focus_nodes
 
     def add_shui_conforms_val(
-            self,
-            validation_graph,
-            validation_result_uris,
-            focus_nodes
+        self, validation_graph, validation_result_uris, focus_nodes
     ):
         """
         add shui conforms flag
         """
         self.log.info("Adding shui:conforms flags to validation graph")
         itr = focus_nodes if focus_nodes else validation_result_uris
         for i in itr:
-            subj = i if focus_nodes else validation_graph.value(
-                subject=i,
-                predicate=SH.focusNode
-            )
-            validation_graph.add((
-                subj,
-                URIRef("https://vocab.eccenca.com/shui/conforms"),
-                Literal(False, datatype=XSD.boolean)
-            ))
+            subj = (
+                i
+                if focus_nodes
+                else validation_graph.value(subject=i, predicate=SH.focusNode)
+            )
+            validation_graph.add(
+                (
+                    subj,
+                    URIRef("https://vocab.eccenca.com/shui/conforms"),
+                    Literal(False, datatype=XSD.boolean),
+                )
+            )
         return validation_graph
 
     def post_graph(self, validation_graph):
         """
         post validation graph to cmem
         """
         self.log.info("Posting SHACL validation graph...")
         temp_file = f"{uuid4()}.nt"
         validation_graph.serialize(temp_file, format="nt", encoding="utf-8")
-        self.log.info(f"Created temporary file {temp_file} with size "
-                      f"{getsize(temp_file)} bytes")
+        self.log.info(
+            f"Created temporary file {temp_file} with size "
+            f"{getsize(temp_file)} bytes"
+        )
         res = post_streamed(
             self.validation_graph_uri,
             temp_file,
             replace=self.clear_validation_graph,
-            content_type="application/n-triples"
+            content_type="application/n-triples",
         )
         remove(temp_file)
         self.log.info("Deleted temporary file")
         if res.status_code == 204:
             self.log.info("Successfully posted SHACL validation graph")
         else:
-            self.log.info("Error posting SHACL validation graph: "
-                          f"status code {res.status_code}")
+            self.log.info(
+                "Error posting SHACL validation graph: "
+                f"status code {res.status_code}"
+            )
 
     # pylint: disable-msg=too-many-arguments
     # pylint: disable-msg=too-many-branches
     def check_object(self, graph, subj, pred, data_graph, shacl_graph):
         """
         format RDF objects for entities output
         """
@@ -453,16 +472,16 @@
             label_g = data_graph
         val = graph.value(subject=subj, predicate=pred)
         obj = val if val else None
         res_val = ""
         if obj:
             if isinstance(obj, URIRef):
                 if self.include_graphs_labels and pred not in (
-                        SH.sourceConstraintComponent,
-                        SH.resultSeverity
+                    SH.sourceConstraintComponent,
+                    SH.resultSeverity,
                 ):
                     label = get_label(label_g, obj)
                     res_val = str(label) if label else obj
                 else:
                     res_val = obj
             elif isinstance(obj, BNode):
                 if self.include_graphs_labels:
@@ -473,16 +492,17 @@
                     # first 50 lines of turtle CBD
                     res_val = graph.cbd(obj).serialize(format="turtle")
                     cbd_lines = res_val.split("\n")
                     if len(cbd_lines) > 50:
                         res_val = "\n".join(cbd_lines[:50]) + "\n..."
             elif isinstance(obj, Literal):
                 if pred == SH.value:
-                    res_val = f'"{obj}"^^<{obj.datatype}>' \
-                        if obj.datatype else f'"{obj}"'
+                    res_val = (
+                        f'"{obj}"^^<{obj.datatype}>' if obj.datatype else f'"{obj}"'
+                    )
                 elif pred == SH.resultMessage:
                     res_val = str(obj)
         return res_val
 
     def make_entities(self, validation_graph, data_graph, shacl_graph, utctime):
         """
         create entities
@@ -492,55 +512,53 @@
             "focusNode",
             "resultPath",
             "value",
             "sourceShape",
             "sourceConstraintComponent",
             # "detail",
             "resultMessage",
-            "resultSeverity"
+            "resultSeverity",
         ]
         entities = []
         conforms = list(validation_graph.objects(predicate=SH.conforms))[0]
-        for validation_result in list(validation_graph.subjects(
-                RDF.type,
-                SH.ValidationResult
-        )):
-            values = [[self.check_object(
-                validation_graph,
-                validation_result,
-                SH[p],
-                data_graph,
-                shacl_graph
-            )] for p in shp] + [
-                [conforms],
-                [self.data_graph_uri],
-                [self.shacl_graph_uri],
-                [utctime]
-            ]
+        for validation_result in list(
+            validation_graph.subjects(RDF.type, SH.ValidationResult)
+        ):
+            values = [
+                [
+                    self.check_object(
+                        validation_graph,
+                        validation_result,
+                        SH[p],
+                        data_graph,
+                        shacl_graph,
+                    )
+                ]
+                for p in shp
+            ] + [[conforms], [self.data_graph_uri], [self.shacl_graph_uri], [utctime]]
             entities.append(Entity(uri=validation_result, values=values))
         paths = [EntityPath(path=SH[p]) for p in shp] + [
-                    EntityPath(path=SH.conforms),
-                    EntityPath(path=PROV.wasDerivedFrom),
-                    EntityPath(path=PROV.wasInformedBy),
-                    EntityPath(path=PROV.generatedAtTime)
-                ]
+            EntityPath(path=SH.conforms),
+            EntityPath(path=PROV.wasDerivedFrom),
+            EntityPath(path=PROV.wasInformedBy),
+            EntityPath(path=PROV.generatedAtTime),
+        ]
         return Entities(
             entities=entities,
-            schema=EntitySchema(type_uri=SH.ValidationResult, paths=paths)
+            schema=EntitySchema(type_uri=SH.ValidationResult, paths=paths),
         )
 
     def get_graph(self, uri):
         """
         get graph from cmem
         """
         graph = Graph()
-        graph.parse(data=get(
-                uri,
-                owl_imports_resolution=self.owl_imports).text,
-                format="turtle")
+        graph.parse(
+            data=get(uri, owl_imports_resolution=self.owl_imports).text, format="turtle"
+        )
         return graph
 
     def process_inputs(self, inputs):
         """
         process input parameters
         """
         paths = [e.path for e in inputs[0].schema.paths]
@@ -554,55 +572,67 @@
     # pylint: disable-msg=too-many-branches
     def check_parameters(self):
         """
         validate plugin parameters
         """
         self.log.info("Validating parameters...")
         if not self.output_entities and not self.generate_graph:
-            raise ValueError("Generate validation graph or Output values parameter "
-                             "needs to be set to true")
+            raise ValueError(
+                "Generate validation graph or Output values parameter "
+                "needs to be set to true"
+            )
         if not validator_url(self.data_graph_uri):
             raise ValueError("Data graph URI parameter is invalid")
         if not validator_url(self.shacl_graph_uri):
             raise ValueError("SHACL graph URI parameter is invalid")
-        graphs_dict = {graph["iri"]: graph["assignedClasses"]
-                       for graph in get_graphs_list()}
+        graphs_dict = {
+            graph["iri"]: graph["assignedClasses"] for graph in get_graphs_list()
+        }
 
         if self.ontology_graph_uri:
             if not validator_url(self.ontology_graph_uri):
                 raise ValueError("Ontology graph URI parameter is invalid")
             if self.ontology_graph_uri not in graphs_dict:
                 raise ValueError(
                     f"Ontology graph <{self.ontology_graph_uri}> not found"
                 )
-            if "http://www.w3.org/2002/07/owl#Ontology" not in \
-                    graphs_dict[self.ontology_graph_uri]:
-                raise ValueError("Invalid graph type for Ontology graph "
-                                 f"<{self.ontology_graph_uri}>")
+            if (
+                "http://www.w3.org/2002/07/owl#Ontology"
+                not in graphs_dict[self.ontology_graph_uri]
+            ):
+                raise ValueError(
+                    "Invalid graph type for Ontology graph "
+                    f"<{self.ontology_graph_uri}>"
+                )
 
         if self.data_graph_uri not in graphs_dict:
             raise ValueError(f"Data graph <{self.data_graph_uri}> not found")
         if self.shacl_graph_uri not in graphs_dict:
             raise ValueError(f"SHACL graph <{self.shacl_graph_uri}> not found")
         if not any(
-                check in graphs_dict[self.data_graph_uri] for check in DATA_GRAPH_TYPES
+            check in graphs_dict[self.data_graph_uri] for check in DATA_GRAPH_TYPES
         ):
-            raise ValueError("Invalid graph type for data graph "
-                             f"<{self.data_graph_uri}>")
-        if "https://vocab.eccenca.com/shui/ShapeCatalog" not in \
-                graphs_dict[self.shacl_graph_uri]:
-            raise ValueError("Invalid graph type for SHACL graph "
-                             f"<{self.shacl_graph_uri}>")
+            raise ValueError(
+                "Invalid graph type for data graph " f"<{self.data_graph_uri}>"
+            )
+        if (
+            "https://vocab.eccenca.com/shui/ShapeCatalog"
+            not in graphs_dict[self.shacl_graph_uri]
+        ):
+            raise ValueError(
+                "Invalid graph type for SHACL graph " f"<{self.shacl_graph_uri}>"
+            )
         for param in self.bool_parameters:
             if not isinstance(self.__dict__[param], bool):
                 try:
                     self.__dict__[param] = bool(strtobool(self.__dict__[param]))
                 except ValueError as err:
-                    raise ValueError(f"Invalid truth value for parameter {param}") \
-                        from err
+                    raise ValueError(
+                        f"Invalid truth value for parameter {param}"
+                    ) from err
         if self.generate_graph:
             if not validator_url(self.validation_graph_uri):
                 raise ValueError("Validation graph URI parameter is invalid")
             if self.validation_graph_uri in graphs_dict:
                 self.log.warning(f"Graph <{self.validation_graph_uri}> already exists")
         if not self.add_labels:
             self.include_graphs_labels = False
@@ -632,64 +662,57 @@
         self.log.info(f"Finished loading data graph in {e_t(start)} seconds")
         self.log.info(f"Loading SHACL graph <{self.shacl_graph_uri}> into memory...")
         start = time()
         shacl_graph = self.get_graph(self.shacl_graph_uri)
         self.log.info(f"Finished loading SHACL graph in {e_t(start)} seconds")
 
         if self.ontology_graph_uri:
+            self.log.info(
+                f"Loading ontology graph <{self.ontology_graph_uri}> into memory..."
+            )
             ontology_graph = self.get_graph(self.ontology_graph_uri)
             self.log.info(f"Finished loading ontology graph in {e_t(start)} seconds")
         else:
             ontology_graph = None
 
         self.log.info("Starting SHACL validation...")
         start = time()
         _conforms, validation_graph, _results_text = validate(
             data_graph,
             shacl_graph=shacl_graph,
             ont_graph=ontology_graph,
             meta_shacl=self.meta_shacl,
             inference=self.inference,
             advanced=self.advanced,
-            inplace=True
+            inplace=True,
         )
         self.log.info(f"Finished SHACL validation in {e_t(start)} seconds")
         utctime = str(datetime.fromtimestamp(int(time()))).replace(" ", "T") + "Z"
         if self.output_entities:
             entities = self.make_entities(
-                validation_graph,
-                data_graph,
-                shacl_graph,
-                utctime
+                validation_graph, data_graph, shacl_graph, utctime
             )
         if self.generate_graph:
             if self.skolemize:
                 self.log.info("Skolemizing validation graph")
                 validation_graph = validation_graph.skolemize(
                     basepath=self.validation_graph_uri
                 )
-            if self.add_labels or \
-                    self.add_shui_conforms:
+            if self.add_labels or self.add_shui_conforms:
                 validation_graph_uris = validation_graph.subjects(
-                    RDF.type,
-                    SH.ValidationResult
+                    RDF.type, SH.ValidationResult
                 )
                 focus_nodes = None
                 if self.add_labels:
                     validation_graph, focus_nodes = self.add_labels_val(
-                        validation_graph,
-                        data_graph,
-                        shacl_graph,
-                        validation_graph_uris
+                        validation_graph, data_graph, shacl_graph, validation_graph_uris
                     )
                 if self.add_shui_conforms:
                     validation_graph = self.add_shui_conforms_val(
-                        validation_graph,
-                        validation_graph_uris,
-                        focus_nodes
+                        validation_graph, validation_graph_uris, focus_nodes
                     )
             validation_graph = self.add_prov(validation_graph, utctime)
             self.post_graph(validation_graph)
         if self.output_entities:
             self.log.info("Outputting entities")
             return entities
         return None
```

### Comparing `cmem_plugin_pyshacl-4.2.0rc2/pyproject.toml` & `cmem_plugin_pyshacl-4.2.0rc3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-pyshacl"
-version = "4.2.0rc2"
+version = "4.2.0rc3"
 license = "Apache-2.0"
 description = "Validate your Knowledge Graphs based on tests generated from SHACL shapes."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules"
```

### Comparing `cmem_plugin_pyshacl-4.2.0rc2/PKG-INFO` & `cmem_plugin_pyshacl-4.2.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-pyshacl
-Version: 4.2.0rc2
+Version: 4.2.0rc3
 Summary: Validate your Knowledge Graphs based on tests generated from SHACL shapes.
 Home-page: https://github.com/eccenca/cmem-plugin-pyshacl
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,SHACL
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
```

