# Comparing `tmp/cimsparql-2.7.2.tar.gz` & `tmp/cimsparql-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cimsparql-2.7.2.tar", max compression
+gzip compressed data, was "cimsparql-2.7.3.tar", max compression
```

## Comparing `cimsparql-2.7.2.tar` & `cimsparql-2.7.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-03-30 05:24:23.401603 cimsparql-2.7.2/LICENSE
--rw-r--r--   0        0        0     5330 2023-03-30 05:24:23.401603 cimsparql-2.7.2/README.md
--rw-r--r--   0        0        0       61 2023-03-30 05:24:50.505994 cimsparql-2.7.2/cimsparql/__init__.py
--rw-r--r--   0        0        0     1320 2023-03-30 05:24:23.401603 cimsparql-2.7.2/cimsparql/async_sparql_wrapper.py
--rw-r--r--   0        0        0     1642 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/constants.py
--rw-r--r--   0        0        0     8200 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/data_models.py
--rw-r--r--   0        0        0    15571 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/graphdb.py
--rw-r--r--   0        0        0    26077 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/model.py
--rw-r--r--   0        0        0     4851 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/ac_lines.sparql
--rw-r--r--   0        0        0      221 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/add_mrid.sparql
--rw-r--r--   0        0        0     1761 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/borders.sparql
--rw-r--r--   0        0        0     1929 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/branch_node_withdraw.sparql
--rw-r--r--   0        0        0     1657 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/bus.sparql
--rw-r--r--   0        0        0      984 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/connections.sparql
--rw-r--r--   0        0        0      676 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/converter_hvdc_bidzones.sparql
--rw-r--r--   0        0        0     2266 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/converters.sparql
--rw-r--r--   0        0        0      588 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/coordinates.sparql
--rw-r--r--   0        0        0     2458 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/dc_active_power_flow.sparql
--rw-r--r--   0        0        0      242 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/disconnected.sparql
--rw-r--r--   0        0        0     3658 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/exchange.sparql
--rw-r--r--   0        0        0     1062 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/full_model.sparql
--rw-r--r--   0        0        0     2786 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/loads.sparql
--rw-r--r--   0        0        0      287 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/market_dates.sparql
--rw-r--r--   0        0        0      429 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/power_flow.sparql
--rw-r--r--   0        0        0      415 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/protective_action.sparql
--rw-r--r--   0        0        0      573 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/regions.sparql
--rw-r--r--   0        0        0     3289 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/series_compensators.sparql
--rw-r--r--   0        0        0      426 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/station_group_code_and_names.sparql
--rw-r--r--   0        0        0      645 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/substation_voltage_level.sparql
--rw-r--r--   0        0        0     2813 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/sv_branch.sparql
--rw-r--r--   0        0        0     3735 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/synchronous_machines.sparql
--rw-r--r--   0        0        0     3127 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/three_winding.sparql
--rw-r--r--   0        0        0     1647 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/three_winding_dummy_nodes.sparql
--rw-r--r--   0        0        0     1656 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/three_winding_loss.sparql
--rw-r--r--   0        0        0      363 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/transformer_windings.sparql
--rw-r--r--   0        0        0     1269 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/transformers.sparql
--rw-r--r--   0        0        0     1844 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/transformers_connected_to_converter.sparql
--rw-r--r--   0        0        0     5276 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/two_winding_transformer.sparql
--rw-r--r--   0        0        0      972 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/two_winding_transformer_angle.sparql
--rw-r--r--   0        0        0      461 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/type_mapper.sparql
--rw-r--r--   0        0        0      814 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/sparql/wind_generating_units.sparql
--rw-r--r--   0        0        0     2918 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/templates.py
--rw-r--r--   0        0        0     5473 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/type_mapper.py
--rw-r--r--   0        0        0     1937 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/url.py
--rw-r--r--   0        0        0      600 2023-03-30 05:24:23.405603 cimsparql-2.7.2/cimsparql/value_mapper.py
--rw-r--r--   0        0        0      459 2023-03-30 05:24:23.413603 cimsparql-2.7.2/pkg_data/blazegraph_repo_config.xml
--rw-r--r--   0        0        0      636 2023-03-30 05:24:23.413603 cimsparql-2.7.2/pkg_data/namespaces.json
--rw-r--r--   0        0        0      805 2023-03-30 05:24:23.413603 cimsparql-2.7.2/pkg_data/native_store_config_template.ttl
--rw-r--r--   0        0        0     2620 2023-03-30 05:24:50.501994 cimsparql-2.7.2/pyproject.toml
--rw-r--r--   0        0        0     6017 1970-01-01 00:00:00.000000 cimsparql-2.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-31 11:59:12.768054 cimsparql-2.7.3/LICENSE
+-rw-r--r--   0        0        0     5330 2023-05-31 11:59:12.768054 cimsparql-2.7.3/README.md
+-rw-r--r--   0        0        0       61 2023-05-31 11:59:46.820465 cimsparql-2.7.3/cimsparql/__init__.py
+-rw-r--r--   0        0        0     1322 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/async_sparql_wrapper.py
+-rw-r--r--   0        0        0     1642 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/constants.py
+-rw-r--r--   0        0        0     8200 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/data_models.py
+-rw-r--r--   0        0        0    15571 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/graphdb.py
+-rw-r--r--   0        0        0    26077 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/model.py
+-rw-r--r--   0        0        0     4851 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/ac_lines.sparql
+-rw-r--r--   0        0        0      221 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/add_mrid.sparql
+-rw-r--r--   0        0        0     1761 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/borders.sparql
+-rw-r--r--   0        0        0     1929 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/branch_node_withdraw.sparql
+-rw-r--r--   0        0        0     1657 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/bus.sparql
+-rw-r--r--   0        0        0      984 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/connections.sparql
+-rw-r--r--   0        0        0      676 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/converter_hvdc_bidzones.sparql
+-rw-r--r--   0        0        0     2266 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/converters.sparql
+-rw-r--r--   0        0        0      588 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/coordinates.sparql
+-rw-r--r--   0        0        0     2458 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/dc_active_power_flow.sparql
+-rw-r--r--   0        0        0      242 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/disconnected.sparql
+-rw-r--r--   0        0        0     3658 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/exchange.sparql
+-rw-r--r--   0        0        0     1062 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/full_model.sparql
+-rw-r--r--   0        0        0     2786 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/loads.sparql
+-rw-r--r--   0        0        0      287 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/market_dates.sparql
+-rw-r--r--   0        0        0      429 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/power_flow.sparql
+-rw-r--r--   0        0        0      415 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/protective_action.sparql
+-rw-r--r--   0        0        0      573 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/regions.sparql
+-rw-r--r--   0        0        0     3289 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/series_compensators.sparql
+-rw-r--r--   0        0        0      426 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/station_group_code_and_names.sparql
+-rw-r--r--   0        0        0      645 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/substation_voltage_level.sparql
+-rw-r--r--   0        0        0     2813 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/sv_branch.sparql
+-rw-r--r--   0        0        0     3735 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/synchronous_machines.sparql
+-rw-r--r--   0        0        0     3127 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/three_winding.sparql
+-rw-r--r--   0        0        0     1647 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/three_winding_dummy_nodes.sparql
+-rw-r--r--   0        0        0     1656 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/three_winding_loss.sparql
+-rw-r--r--   0        0        0      363 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/transformer_windings.sparql
+-rw-r--r--   0        0        0     1269 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/transformers.sparql
+-rw-r--r--   0        0        0     1844 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/transformers_connected_to_converter.sparql
+-rw-r--r--   0        0        0     5276 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/two_winding_transformer.sparql
+-rw-r--r--   0        0        0      972 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/two_winding_transformer_angle.sparql
+-rw-r--r--   0        0        0      461 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/type_mapper.sparql
+-rw-r--r--   0        0        0      814 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/sparql/wind_generating_units.sparql
+-rw-r--r--   0        0        0     2918 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/templates.py
+-rw-r--r--   0        0        0     5473 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/type_mapper.py
+-rw-r--r--   0        0        0     1937 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/url.py
+-rw-r--r--   0        0        0      600 2023-05-31 11:59:12.768054 cimsparql-2.7.3/cimsparql/value_mapper.py
+-rw-r--r--   0        0        0      459 2023-05-31 11:59:12.776054 cimsparql-2.7.3/pkg_data/blazegraph_repo_config.xml
+-rw-r--r--   0        0        0      636 2023-05-31 11:59:12.776054 cimsparql-2.7.3/pkg_data/namespaces.json
+-rw-r--r--   0        0        0      805 2023-05-31 11:59:12.776054 cimsparql-2.7.3/pkg_data/native_store_config_template.ttl
+-rw-r--r--   0        0        0     2620 2023-05-31 11:59:46.816465 cimsparql-2.7.3/pyproject.toml
+-rw-r--r--   0        0        0     6017 1970-01-01 00:00:00.000000 cimsparql-2.7.3/PKG-INFO
```

### Comparing `cimsparql-2.7.2/LICENSE` & `cimsparql-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/README.md` & `cimsparql-2.7.3/README.md`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/async_sparql_wrapper.py` & `cimsparql-2.7.3/cimsparql/async_sparql_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         if self.returnFormat != JSON:
             raise NotImplementedError("Async client only support JSON return format")
 
         request = self._createRequest()
         url = request.get_full_url()
         method = request.get_method()
 
-        args = {"timeout": self.timeout} | {"verify": self.ca_bundle} if self.ca_bundle else {}
+        args = {"timeout": self.timeout} | ({"verify": self.ca_bundle} if self.ca_bundle else {})
         async with httpx.AsyncClient(**args) as client:
             response = await client.request(
                 method, url, headers=request.headers, content=request.data
             )
 
         status = response.status_code
         if status != 200:
```

### Comparing `cimsparql-2.7.2/cimsparql/constants.py` & `cimsparql-2.7.3/cimsparql/constants.py`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/data_models.py` & `cimsparql-2.7.3/cimsparql/data_models.py`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/graphdb.py` & `cimsparql-2.7.3/cimsparql/graphdb.py`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/model.py` & `cimsparql-2.7.3/cimsparql/model.py`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/ac_lines.sparql` & `cimsparql-2.7.3/cimsparql/sparql/ac_lines.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/borders.sparql` & `cimsparql-2.7.3/cimsparql/sparql/borders.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/branch_node_withdraw.sparql` & `cimsparql-2.7.3/cimsparql/sparql/branch_node_withdraw.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/bus.sparql` & `cimsparql-2.7.3/cimsparql/sparql/bus.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/connections.sparql` & `cimsparql-2.7.3/cimsparql/sparql/connections.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/converter_hvdc_bidzones.sparql` & `cimsparql-2.7.3/cimsparql/sparql/converter_hvdc_bidzones.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/converters.sparql` & `cimsparql-2.7.3/cimsparql/sparql/converters.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/coordinates.sparql` & `cimsparql-2.7.3/cimsparql/sparql/coordinates.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/dc_active_power_flow.sparql` & `cimsparql-2.7.3/cimsparql/sparql/dc_active_power_flow.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/exchange.sparql` & `cimsparql-2.7.3/cimsparql/sparql/exchange.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/full_model.sparql` & `cimsparql-2.7.3/cimsparql/sparql/full_model.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/loads.sparql` & `cimsparql-2.7.3/cimsparql/sparql/loads.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/regions.sparql` & `cimsparql-2.7.3/cimsparql/sparql/regions.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/series_compensators.sparql` & `cimsparql-2.7.3/cimsparql/sparql/series_compensators.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/substation_voltage_level.sparql` & `cimsparql-2.7.3/cimsparql/sparql/substation_voltage_level.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/sv_branch.sparql` & `cimsparql-2.7.3/cimsparql/sparql/sv_branch.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/synchronous_machines.sparql` & `cimsparql-2.7.3/cimsparql/sparql/synchronous_machines.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/three_winding.sparql` & `cimsparql-2.7.3/cimsparql/sparql/three_winding.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/three_winding_dummy_nodes.sparql` & `cimsparql-2.7.3/cimsparql/sparql/three_winding_dummy_nodes.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/three_winding_loss.sparql` & `cimsparql-2.7.3/cimsparql/sparql/three_winding_loss.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/transformers.sparql` & `cimsparql-2.7.3/cimsparql/sparql/transformers.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/transformers_connected_to_converter.sparql` & `cimsparql-2.7.3/cimsparql/sparql/transformers_connected_to_converter.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/two_winding_transformer.sparql` & `cimsparql-2.7.3/cimsparql/sparql/two_winding_transformer.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/two_winding_transformer_angle.sparql` & `cimsparql-2.7.3/cimsparql/sparql/two_winding_transformer_angle.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/sparql/wind_generating_units.sparql` & `cimsparql-2.7.3/cimsparql/sparql/wind_generating_units.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/templates.py` & `cimsparql-2.7.3/cimsparql/templates.py`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/type_mapper.py` & `cimsparql-2.7.3/cimsparql/type_mapper.py`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/url.py` & `cimsparql-2.7.3/cimsparql/url.py`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/cimsparql/value_mapper.py` & `cimsparql-2.7.3/cimsparql/value_mapper.py`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/pkg_data/namespaces.json` & `cimsparql-2.7.3/pkg_data/namespaces.json`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/pkg_data/native_store_config_template.ttl` & `cimsparql-2.7.3/pkg_data/native_store_config_template.ttl`

 * *Files identical despite different names*

### Comparing `cimsparql-2.7.2/pyproject.toml` & `cimsparql-2.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 [tool.poetry]
 name = "cimsparql"
-version = "2.7.2"
+version = "2.7.3"
 description = "CIM query utilities"
 readme = "README.md"
 authors = ["Statnett Datascience <Datascience.Drift@Statnett.no>"]
 repository = "https://github.com/statnett/cimsparql.git"
 include = ["pkg_data/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `cimsparql-2.7.2/PKG-INFO` & `cimsparql-2.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cimsparql
-Version: 2.7.2
+Version: 2.7.3
 Summary: CIM query utilities
 Home-page: https://github.com/statnett/cimsparql.git
 Author: Statnett Datascience
 Author-email: Datascience.Drift@Statnett.no
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

