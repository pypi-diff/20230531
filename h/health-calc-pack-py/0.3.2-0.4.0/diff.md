# Comparing `tmp/health_calc_pack_py-0.3.2.tar.gz` & `tmp/health_calc_pack_py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "health_calc_pack_py-0.3.2.tar", max compression
+gzip compressed data, was "health_calc_pack_py-0.4.0.tar", max compression
```

## Comparing `health_calc_pack_py-0.3.2.tar` & `health_calc_pack_py-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0        0 2023-05-17 01:13:19.681769 health_calc_pack_py-0.3.2/health_calc_pack_py/__init__.py
--rw-r--r--   0        0        0     2198 2023-05-17 02:07:50.108989 health_calc_pack_py-0.3.2/health_calc_pack_py/app.py
--rw-r--r--   0        0        0      114 2023-05-17 01:13:20.285768 health_calc_pack_py-0.3.2/health_calc_pack_py/imc.py
--rw-r--r--   0        0        0      869 2023-05-17 01:29:17.749957 health_calc_pack_py-0.3.2/health_calc_pack_py/macronutrientes.py
--rw-r--r--   0        0        0     2988 2023-05-17 01:52:51.016461 health_calc_pack_py-0.3.2/health_calc_pack_py/static/swagger.json
--rw-r--r--   0        0        0      234 2023-05-17 01:13:21.222773 health_calc_pack_py-0.3.2/health_calc_pack_py/test_imc.py
--rw-r--r--   0        0        0      568 2023-05-22 22:23:53.511991 health_calc_pack_py-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1602 2023-05-22 22:24:08.055486 health_calc_pack_py-0.3.2/README.md
--rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 health_calc_pack_py-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-30 22:03:13.370702 health_calc_pack_py-0.4.0/health_calc_pack_py/__init__.py
+-rw-r--r--   0        0        0     2203 2023-05-30 23:08:23.834321 health_calc_pack_py-0.4.0/health_calc_pack_py/app.py
+-rw-r--r--   0        0        0      162 2023-05-31 00:07:57.687152 health_calc_pack_py-0.4.0/health_calc_pack_py/estrategia.py
+-rw-r--r--   0        0        0      300 2023-05-31 00:08:40.884630 health_calc_pack_py-0.4.0/health_calc_pack_py/ganho_massa_muscular.py
+-rw-r--r--   0        0        0      985 2023-05-30 23:07:50.916475 health_calc_pack_py-0.4.0/health_calc_pack_py/imc.py
+-rw-r--r--   0        0        0     1116 2023-05-31 00:07:21.207765 health_calc_pack_py-0.4.0/health_calc_pack_py/macronutrientes.py
+-rw-r--r--   0        0        0      295 2023-05-31 00:08:30.695083 health_calc_pack_py-0.4.0/health_calc_pack_py/manutencao_peso.py
+-rw-r--r--   0        0        0      297 2023-05-31 00:08:33.404643 health_calc_pack_py-0.4.0/health_calc_pack_py/perda_gordura.py
+-rw-r--r--   0        0        0      313 2023-05-31 00:08:35.544284 health_calc_pack_py-0.4.0/health_calc_pack_py/perda_peso_ganho_massa_muscular.py
+-rw-r--r--   0        0        0     2988 2023-05-30 22:03:13.413699 health_calc_pack_py-0.4.0/health_calc_pack_py/static/swagger.json
+-rw-r--r--   0        0        0      234 2023-05-30 22:03:13.416693 health_calc_pack_py-0.4.0/health_calc_pack_py/test_imc.py
+-rw-r--r--   0        0        0      568 2023-05-31 00:09:20.185820 health_calc_pack_py-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1602 2023-05-22 22:24:08.055486 health_calc_pack_py-0.4.0/README.md
+-rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 health_calc_pack_py-0.4.0/PKG-INFO
```

### Comparing `health_calc_pack_py-0.3.2/health_calc_pack_py/app.py` & `health_calc_pack_py-0.4.0/health_calc_pack_py/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,18 @@
         altura = float(altura)
     except ValueError:
         return jsonify({"erro": "Os campos 'peso' e 'altura' devem ser numéricos"}), 400
 
     if peso <= 0 or altura <= 0:
         return jsonify({"erro": "Os campos 'peso' e 'altura' devem ser maiores que zero"}), 400
 
-    imc = calcular_imc(peso, altura)
+    resultado = calcular_imc(peso, altura)
+
+    return jsonify(resultado)
 
-    return jsonify({"IMC": imc})
 
 @app.route('/calcular_macronutrientes', methods=['POST'])
 def macronutrientes():
     data = request.get_json()
 
     if not data:
         return jsonify({"erro": "JSON inválido"}), 400
```

### Comparing `health_calc_pack_py-0.3.2/health_calc_pack_py/static/swagger.json` & `health_calc_pack_py-0.4.0/health_calc_pack_py/static/swagger.json`

 * *Files identical despite different names*

### Comparing `health_calc_pack_py-0.3.2/pyproject.toml` & `health_calc_pack_py-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "health-calc-pack-py"
-version = "0.3.2"
+version = "0.4.0"
 description = "Uma API para calcular IMC e macronutrientes"
 authors = ["Angelo Diniz <angelo.jose.7l@hotmail.com>", "Daniel Bernardes <danielaugustobernardes@yahoo.com.br>"]
 readme = "README.md"
 packages = [{include = "health_calc_pack_py"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `health_calc_pack_py-0.3.2/README.md` & `health_calc_pack_py-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `health_calc_pack_py-0.3.2/PKG-INFO` & `health_calc_pack_py-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: health-calc-pack-py
-Version: 0.3.2
+Version: 0.4.0
 Summary: Uma API para calcular IMC e macronutrientes
 Author: Angelo Diniz
 Author-email: angelo.jose.7l@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

