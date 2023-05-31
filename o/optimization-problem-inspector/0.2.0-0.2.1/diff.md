# Comparing `tmp/optimization_problem_inspector-0.2.0-py3-none-any.whl.zip` & `tmp/optimization_problem_inspector-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 30814 bytes, number of entries: 20
+Zip file size: 30926 bytes, number of entries: 20
 -rw-r--r--  2.0 unx       53 b- defN 20-Feb-02 00:00 optimization_problem_inspector/__about__.py
 -rw-r--r--  2.0 unx       31 b- defN 20-Feb-02 00:00 optimization_problem_inspector/__init__.py
--rw-r--r--  2.0 unx    35700 b- defN 20-Feb-02 00:00 optimization_problem_inspector/app.py
+-rw-r--r--  2.0 unx    36190 b- defN 20-Feb-02 00:00 optimization_problem_inspector/app.py
 -rw-r--r--  2.0 unx     1934 b- defN 20-Feb-02 00:00 optimization_problem_inspector/app_strings.py
 -rw-r--r--  2.0 unx     9974 b- defN 20-Feb-02 00:00 optimization_problem_inspector/coco_interface.py
 -rw-r--r--  2.0 unx     1608 b- defN 20-Feb-02 00:00 optimization_problem_inspector/config.py
--rw-r--r--  2.0 unx      120 b- defN 20-Feb-02 00:00 optimization_problem_inspector/errors.py
+-rw-r--r--  2.0 unx      116 b- defN 20-Feb-02 00:00 optimization_problem_inspector/errors.py
 -rw-r--r--  2.0 unx    15342 b- defN 20-Feb-02 00:00 optimization_problem_inspector/features.py
 -rw-r--r--  2.0 unx      259 b- defN 20-Feb-02 00:00 optimization_problem_inspector/logger.py
 -rw-r--r--  2.0 unx     4836 b- defN 20-Feb-02 00:00 optimization_problem_inspector/models.py
 -rw-r--r--  2.0 unx    19332 b- defN 20-Feb-02 00:00 optimization_problem_inspector/problem.py
 -rw-r--r--  2.0 unx     9459 b- defN 20-Feb-02 00:00 optimization_problem_inspector/sampling.py
--rw-r--r--  2.0 unx     4811 b- defN 20-Feb-02 00:00 optimization_problem_inspector/serialization.py
+-rw-r--r--  2.0 unx     4925 b- defN 20-Feb-02 00:00 optimization_problem_inspector/serialization.py
 -rw-r--r--  2.0 unx       86 b- defN 20-Feb-02 00:00 optimization_problem_inspector/assets/gui-help.md
 -rw-r--r--  2.0 unx      578 b- defN 20-Feb-02 00:00 optimization_problem_inspector/assets/typography.css
-?rw-r--r--  2.0 unx     3794 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx       68 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1157 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.0.dist-info/licenses/LICENSE.txt
-?rw-r--r--  2.0 unx     2014 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.0.dist-info/RECORD
-20 files, 111243 bytes uncompressed, 27396 bytes compressed:  75.4%
+?rw-r--r--  2.0 unx     3794 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx       68 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1157 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.1.dist-info/licenses/LICENSE.txt
+?rw-r--r--  2.0 unx     2014 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.1.dist-info/RECORD
+20 files, 111843 bytes uncompressed, 27508 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: optimization_problem_inspector/assets/gui-help.md
 Comment: 
 
 Filename: optimization_problem_inspector/assets/typography.css
 Comment: 
 
-Filename: optimization_problem_inspector-0.2.0.dist-info/METADATA
+Filename: optimization_problem_inspector-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: optimization_problem_inspector-0.2.0.dist-info/WHEEL
+Filename: optimization_problem_inspector-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: optimization_problem_inspector-0.2.0.dist-info/entry_points.txt
+Filename: optimization_problem_inspector-0.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: optimization_problem_inspector-0.2.0.dist-info/licenses/LICENSE.txt
+Filename: optimization_problem_inspector-0.2.1.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: optimization_problem_inspector-0.2.0.dist-info/RECORD
+Filename: optimization_problem_inspector-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## optimization_problem_inspector/__about__.py

```diff
@@ -1,2 +1,2 @@
 # SPDX-License-Identifier: MIT
-__version__ = '0.2.0'
+__version__ = '0.2.1'
```

## optimization_problem_inspector/app.py

```diff
@@ -458,21 +458,33 @@
                 contents,
                 style={"whiteSpace": "pre-wrap", "wordBreak": "break-all"},
             ),
         ]
     )
 
 
+def logg_function_call(func):
+    def wrapper(*args, **kwargs):
+        logger.debug(
+            f"Function {func.__name__} called with args {args}"
+            f" and kwargs {kwargs}"
+        )
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
 @app.callback(
     Output("output-data-upload", "children"),
     Output("problem-specification", "data"),
     Input("upload-problem-spec", "contents"),
     State("upload-problem-spec", "filename"),
     State("upload-problem-spec", "last_modified"),
 )
+@logg_function_call
 def update_problem_specification_output(contents, filename, dt):
     decoded = None
     if contents is None:
         dim = DEFAULT_PROBLEM_ARGS["dim"]
         obj = DEFAULT_PROBLEM_ARGS["obj"]
         fi = DEFAULT_PROBLEM_ARGS["fi"]
         common_name = REFERENCE_BBOB_NAMES[fi]
@@ -488,28 +500,32 @@
         decoded = base64.b64decode(content_string).decode("utf-8")
 
     if decoded is not None:
         children = [file_to_html_elements(decoded, filename, dt)]
     else:
         return None, None
 
+    with io.StringIO(decoded) as f:
+        serialization.load_spec(f)
+
     return (children, decoded)
 
 
 @app.callback(
     Output("data-table", "data"),
     Output("data-table", "columns"),
     Output("upload-data-alerting", "children"),
     Output("reference-container-alerting", "children"),
     Input("upload-problem-spec", "contents"),
     Input("upload-data", "contents"),
     Input("sample-generation-N-select", "value"),
     Input("sample-generation-method-select", "value"),
     Input("sampling-parameters", "value"),
 )
+@logg_function_call
 def update_data_in_problem_data_table(
     spec_contents,
     data_contents,
     sample_n,
     sample_method_name,
     sampling_parameters_dump,
 ):
@@ -564,14 +580,15 @@
     Input("btn-download-txt", "n_clicks"),
     State("sample-generation-N-select", "value"),
     State("sample-generation-method-select", "value"),
     State("problem-specification", "data"),
     State("sampling-parameters", "value"),
     prevent_initial_call=True,
 )
+@logg_function_call
 def generate_problem_sample_file(
     n_clicks,
     N,
     sample_generation_method_name,
     spec_contents,
     sampling_parameters_dump,
 ):
@@ -593,14 +610,15 @@
     return dict(content=sample.to_csv(index=False), filename="data.csv")
 
 
 @app.callback(
     Output("reference-problem-definitions", "value"),
     Input("problem-specification", "data"),
 )
+@logg_function_call
 def update_reference_problem_specs(problem_spec):
     objs = problem_spec.count("OBJECTIVES")
     dims = problem_spec.count("VARIABLES")
     constraints = problem_spec.count("CONSTRAINTS")
     ref_problems = problem.ReferenceProblemsGBBOB.from_simple_input(
         dimensions=dims, objectives=objs, constraints=constraints
     )
@@ -608,14 +626,15 @@
     return ref_problems_dump
 
 
 @app.callback(
     Output("features-parameters", "value"),
     Input("problem-specification", "data"),
 )
+@logg_function_call
 def update_feature_parameters(problem_spec):
     feature_parameters = {}
     feature_parameters[features.neighbourhood_feats.__name__] = {
         "number_neighbours": 10
     }
     return yaml.dump(feature_parameters)
 
@@ -652,14 +671,15 @@
     Input("features-parameters", "value"),
     State("problem-specification", "data"),
     State("sample-generation-N-select", "value"),
     State("sample-generation-method-select", "value"),
     State("sampling-parameters", "value"),
     Input("reference-feature-selection", "value"),
 )
+@logg_function_call
 def update_reference_problems_and_features(
     problem_data,
     ref_problem_definitions,
     feature_parameters_dump,
     problem_spec,
     n,
     sample_method_name,
@@ -957,14 +977,15 @@
 @app.callback(
     Output("visualization-plot-options-columns", "options"),
     Output("visualization-plot-options-columns", "value"),
     Output("visualization-plot-options-color", "options"),
     Output("visualization-plot-options-color", "value"),
     Input("data-table", "data"),
 )
+@logg_function_call
 def update_plot_options_columns(problem_data):
     df = pd.DataFrame(problem_data)
     values = df.columns.to_list()
     return values, values, values, values[-1]
 
 
 def get_html_figure_encoded(fig: go.Figure) -> str:
@@ -1062,12 +1083,15 @@
 
 
 def main():
     logger.info("Starting server...")
     # we need host="0.0.0.0" (all interfaces) to support serving
     # the application in docker
     # TODO: maybe make configurable from the CLI
-    app.run_server(host="0.0.0.0", debug=True)
+    app.run_server(
+        host="0.0.0.0",
+        debug=True,
+    )
 
 
 if __name__ == "__main__":
     main()
```

## optimization_problem_inspector/errors.py

```diff
@@ -1,4 +1,4 @@
 class OPIError(Exception):
-    """Base class of errors in the Optimization problem inspector framework
-    """
+    """Base class of errors in the Optimization problem inspector framework"""
+
     pass
```

## optimization_problem_inspector/serialization.py

```diff
@@ -125,14 +125,16 @@
         file (TextIOWrapper): File handler from the opened file.
 
     Returns:
         Spec: Optimization problem inspector specification model
     """
     dict_model = yaml.safe_load(file)
     deserialized_kwargs = build_model(dict_model=dict_model)
+    if isinstance(deserialized_kwargs, DataSpec):
+        deserialized_kwargs = {"dataSpec": deserialized_kwargs}
     return Spec(**deserialized_kwargs)
 
 
 def dumps_spec(spec: Spec) -> str:
     """Serialize the Optimization problem inspector specification
     model into a yaml string that can be read back and de-serialized
     into specification model again.
```

## Comparing `optimization_problem_inspector-0.2.0.dist-info/METADATA` & `optimization_problem_inspector-0.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimization-problem-inspector
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool for analysis of industrial optimization problems and their solutions
 Project-URL: Documentation, https://github.com/unknown/optimization-problem-inspector#readme
 Project-URL: Issues, https://github.com/unknown/optimization-problem-inspector/issues
 Project-URL: Source, https://github.com/unknown/optimization-problem-inspector
 Author-email: Jernej Zupančič <88.jernej@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

## Comparing `optimization_problem_inspector-0.2.0.dist-info/licenses/LICENSE.txt` & `optimization_problem_inspector-0.2.1.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `optimization_problem_inspector-0.2.0.dist-info/RECORD` & `optimization_problem_inspector-0.2.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-optimization_problem_inspector/__about__.py,sha256=hQGCoV-4FznNqxFvYtYM9xhvIQUjxKDCpG8s-FpUJ4E,53
+optimization_problem_inspector/__about__.py,sha256=HCrMGMmDNXAw1c5nKre3J9VhwWU-_h5nfoyDyX1on9w,53
 optimization_problem_inspector/__init__.py,sha256=W-Iw-hOna0MxXOaE4ehJxxBNt6owr2n32RFEtLZl4tM,31
-optimization_problem_inspector/app.py,sha256=RLymTWZgMjXYr-UxshBYaROyMzsfqvwkDlQzPQC_clw,35700
+optimization_problem_inspector/app.py,sha256=dAfxTHOTBFDawcY6w9V2rPTkRL4gYRurbdn2WT5Wu4U,36190
 optimization_problem_inspector/app_strings.py,sha256=fgwDkjJb1uPxQCg8kv3-Cv6xnmtzudHNQ7--clfT340,1934
 optimization_problem_inspector/coco_interface.py,sha256=pJHWPDoPYBUQWhyrJYmI5I_QsTlpz3byViqFebJ1PQU,9974
 optimization_problem_inspector/config.py,sha256=dSQ99a4en6xDZELCDsa8_ewlVqQQuuilwfa-dqxzC00,1608
-optimization_problem_inspector/errors.py,sha256=RV3dzSuT4jVDu_SErPQBVjkfvX42tJo2uMoaGgWEf9c,120
+optimization_problem_inspector/errors.py,sha256=r2RHeO9B5edBo8LHUMohLdB_HE_jNjAAvfkRcXE_KAw,116
 optimization_problem_inspector/features.py,sha256=-lOlZIMhh0ridtVwcFStZHf37Okow7_1iKCZi1f9cPg,15342
 optimization_problem_inspector/logger.py,sha256=Sp4yYifCT9YLdJIPn8lFaDmZoIbGFo45b21cLsNI4Lw,259
 optimization_problem_inspector/models.py,sha256=zJesjXbpYxw4nT0lsUPpXzXXwqFlDy1kXAUmraCmk3k,4836
 optimization_problem_inspector/problem.py,sha256=Bno_xSKpfEi4TesDO_VJ5pZpfnnRhTaOWk-13LW0i9E,19332
 optimization_problem_inspector/sampling.py,sha256=NfLfh1EHuTYBQVEK4IRiFvDQh-spnZTG2QKltYEG4yI,9459
-optimization_problem_inspector/serialization.py,sha256=tYgiNGyzfn9QxVNNhBcR0vdpn4TZMx2M3EdmK7chyf0,4811
+optimization_problem_inspector/serialization.py,sha256=QUraACAkt2HPpVoDQuoiaDfFDLlHhlEWozVRgaldMwI,4925
 optimization_problem_inspector/assets/gui-help.md,sha256=V1e1bEYqx48qhYnlxnqtMpAfKPLGxMty_Yye5KXCCnQ,86
 optimization_problem_inspector/assets/typography.css,sha256=JIrxZjJIZl8VySS-ao-HdCcZDpfeU9H1j87zQh6Moyw,578
-optimization_problem_inspector-0.2.0.dist-info/METADATA,sha256=ZgPtAEfpEZO9JTFILmquenBDqat8xj2J1cVBow1s9J4,3794
-optimization_problem_inspector-0.2.0.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
-optimization_problem_inspector-0.2.0.dist-info/entry_points.txt,sha256=CBKAxN7Me5VbviWhbuzvvxNQVo6YB_7mitq8A5m3GMY,68
-optimization_problem_inspector-0.2.0.dist-info/licenses/LICENSE.txt,sha256=o_AcDderANEapBiEJuuDouZOWs9IH3_c2SUyfEcTVPk,1157
-optimization_problem_inspector-0.2.0.dist-info/RECORD,,
+optimization_problem_inspector-0.2.1.dist-info/METADATA,sha256=CJAbSMTelHfTx7KDudGFVwInrxxnA7sAGSzydlQ-CtY,3794
+optimization_problem_inspector-0.2.1.dist-info/WHEEL,sha256=y1bSCq4r5i4nMmpXeUJMqs3ipKvkZObrIXSvJHm1qCI,87
+optimization_problem_inspector-0.2.1.dist-info/entry_points.txt,sha256=CBKAxN7Me5VbviWhbuzvvxNQVo6YB_7mitq8A5m3GMY,68
+optimization_problem_inspector-0.2.1.dist-info/licenses/LICENSE.txt,sha256=o_AcDderANEapBiEJuuDouZOWs9IH3_c2SUyfEcTVPk,1157
+optimization_problem_inspector-0.2.1.dist-info/RECORD,,
```

