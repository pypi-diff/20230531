# Comparing `tmp/ia_wumpus-0.3.6.tar.gz` & `tmp/ia_wumpus-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia_wumpus-0.3.6.tar", max compression
+gzip compressed data, was "ia_wumpus-0.3.7.tar", max compression
```

## Comparing `ia_wumpus-0.3.6.tar` & `ia_wumpus-0.3.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.6/LICENSE
--rw-r--r--   0        0        0     3968 2023-05-29 00:28:22.597635 ia_wumpus-0.3.6/README.md
--rw-r--r--   0        0        0      636 2023-05-29 00:29:36.243030 ia_wumpus-0.3.6/ia_wumpus/__init__.py
--rw-r--r--   0        0        0     8481 2023-05-28 21:14:28.319582 ia_wumpus-0.3.6/ia_wumpus/agente_reativo_v1.py
--rw-r--r--   0        0        0     8960 2023-05-28 19:01:53.341149 ia_wumpus-0.3.6/ia_wumpus/ambiente.py
--rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.6/ia_wumpus/dinamica_agente_ambiente.py
--rw-r--r--   0        0        0      511 2023-05-29 00:29:07.586488 ia_wumpus-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     4622 1970-01-01 00:00:00.000000 ia_wumpus-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.7/LICENSE
+-rw-r--r--   0        0        0     3968 2023-05-29 00:49:08.214270 ia_wumpus-0.3.7/README.md
+-rw-r--r--   0        0        0      636 2023-05-29 00:49:09.138275 ia_wumpus-0.3.7/ia_wumpus/__init__.py
+-rw-r--r--   0        0        0     8583 2023-05-29 20:11:24.956498 ia_wumpus-0.3.7/ia_wumpus/agente_reativo_v1.py
+-rw-r--r--   0        0        0     8960 2023-05-29 00:49:09.162276 ia_wumpus-0.3.7/ia_wumpus/ambiente.py
+-rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.7/ia_wumpus/dinamica_agente_ambiente.py
+-rw-r--r--   0        0        0      511 2023-05-31 02:32:04.433493 ia_wumpus-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     4622 1970-01-01 00:00:00.000000 ia_wumpus-0.3.7/PKG-INFO
```

### Comparing `ia_wumpus-0.3.6/LICENSE` & `ia_wumpus-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.6/README.md` & `ia_wumpus-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.6/ia_wumpus/__init__.py` & `ia_wumpus-0.3.7/ia_wumpus/__init__.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.6/ia_wumpus/agente_reativo_v1.py` & `ia_wumpus-0.3.7/ia_wumpus/agente_reativo_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from rich.console import Console
 from rich.theme import Theme
 # from loguru import logger
 from typing import List, Tuple
 
 custom_theme = Theme({
     "info": "purple bold",
+    "info2": "red italic bold",
     "info_bold": "purple bold",
     "warning": "yellow bold",
     "green": "green bold",
     "danger": "bold red"
 })
 console = Console(theme=custom_theme)
 
@@ -37,14 +38,17 @@
         self.amb = ambiente
         self.__list_opc_mov_ag: List[Tuple] = []
         self.bala: bool = True
         self.pegou_ouro: bool = False
         self.vitoria: bool = False
         self.morreu: bool = False
 
+    def printw(self, txt):
+        console.print(txt, style="info2")
+
     def get_opcoes_mov(self) -> List:
         """
         Método responsável por obter as possíveis obções de movimentação
         do agente no ambiente.
         """
         pos_agente = self.amb.get_pos_objetos()["agente"][0]
         self.__opcoes_mov_agente(pos_agente=pos_agente)
```

### Comparing `ia_wumpus-0.3.6/ia_wumpus/ambiente.py` & `ia_wumpus-0.3.7/ia_wumpus/ambiente.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.6/ia_wumpus/dinamica_agente_ambiente.py` & `ia_wumpus-0.3.7/ia_wumpus/dinamica_agente_ambiente.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.6/PKG-INFO` & `ia_wumpus-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-wumpus
-Version: 0.3.6
+Version: 0.3.7
 Summary: Projeto O Mundo do Wumpus - Anbiente para estudo da disciplina de Inteligencia Computacional.
 Author: Oseiasdfarias
 Author-email: oseias.dfarias@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

