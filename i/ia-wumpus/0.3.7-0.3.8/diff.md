# Comparing `tmp/ia_wumpus-0.3.7.tar.gz` & `tmp/ia_wumpus-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia_wumpus-0.3.7.tar", max compression
+gzip compressed data, was "ia_wumpus-0.3.8.tar", max compression
```

## Comparing `ia_wumpus-0.3.7.tar` & `ia_wumpus-0.3.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.7/LICENSE
--rw-r--r--   0        0        0     3968 2023-05-29 00:49:08.214270 ia_wumpus-0.3.7/README.md
--rw-r--r--   0        0        0      636 2023-05-29 00:49:09.138275 ia_wumpus-0.3.7/ia_wumpus/__init__.py
--rw-r--r--   0        0        0     8583 2023-05-29 20:11:24.956498 ia_wumpus-0.3.7/ia_wumpus/agente_reativo_v1.py
--rw-r--r--   0        0        0     8960 2023-05-29 00:49:09.162276 ia_wumpus-0.3.7/ia_wumpus/ambiente.py
--rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.7/ia_wumpus/dinamica_agente_ambiente.py
--rw-r--r--   0        0        0      511 2023-05-31 02:32:04.433493 ia_wumpus-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     4622 1970-01-01 00:00:00.000000 ia_wumpus-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.8/LICENSE
+-rw-r--r--   0        0        0     4260 2023-05-31 03:35:24.780713 ia_wumpus-0.3.8/README.md
+-rw-r--r--   0        0        0      636 2023-05-29 00:49:09.138275 ia_wumpus-0.3.8/ia_wumpus/__init__.py
+-rw-r--r--   0        0        0     8583 2023-05-31 03:35:25.048720 ia_wumpus-0.3.8/ia_wumpus/agente_reativo_v1.py
+-rw-r--r--   0        0        0     8960 2023-05-29 00:49:09.162276 ia_wumpus-0.3.8/ia_wumpus/ambiente.py
+-rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.8/ia_wumpus/dinamica_agente_ambiente.py
+-rw-r--r--   0        0        0      511 2023-05-31 03:35:25.108722 ia_wumpus-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     4914 1970-01-01 00:00:00.000000 ia_wumpus-0.3.8/PKG-INFO
```

### Comparing `ia_wumpus-0.3.7/LICENSE` & `ia_wumpus-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.7/README.md` & `ia_wumpus-0.3.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
+# Mundo do Wumpus - Intelegência Computacional
 
-<img src="https://github.com/Oseiasdfarias/IA_mundo_do_wumpus/blob/main/utils/logo.png?raw=true" alt="Logo UFPA" style="width:50px">
-
-
-<strong>Universidade Federal do Pará</strong>\
-<strong>Campus Universitário de Tucuruí</strong>\
-<strong>Faculdade de Engenharia Elétrica</strong>
+Ambiente para estudo de modelos de Apredizagem de Máquina da disciplina de Inteligência Computacional.
 
 <br>
 
-# Mundo do Wumpus - Intelegência Computacional
+## Documentação
 
-Ambiente para estudo de modelos de Apredizagem de Máquina da disciplina de Inteligência Computacional.
+### [Documentação ia-wumpus](https://oseiasdfarias.github.io/IA_mundo_do_wumpus/)
 
 <br>
 
 # Versões do Projeto
 
 <img src="https://raw.githubusercontent.com/Oseiasdfarias/IA_mundo_do_wumpus/340951a7d59c7ce6e3c981455b77638781b23d52/docs/static/img/code_demo.svg" alt="Ambiente Mundo do Wumpus." style="width:900px">
 
@@ -28,14 +24,22 @@
   <li>Tamanho (n) = ordem(n) da matriz quadrada (n >= 3). Linha e coluna = (n - 1);</li>
   <li>Objetos: poços (p), Wumpus (W) e ouro (o). Quantidade? [São parâmetros definidos pelo usuário (p, W, o >= O). E, também, podem ser atribuídos automaticamente, de acordo com o tamanho do ambiente (n), via a definição de alguma regra].</li>
   <li>A partir dos objetos, posicionar no ambiente, também, as percepções geradas por cada um deles.</li>
   <li>A casa (0,0) é a única que não pode ter nenhum objeto, pois é a posição inicial do Agente</li>
   <li>Onde houver poço não pode ser posicionado o ouro e o Wumpus. No entanto, estes podem ser posicionados em quaisquer uma das outras casas.</li>
 </ul>
 
+```python title=main.py
+from ia_wumpus import Ambiente
+
+
+amb = Ambiente(dimensao_ambiente=3)
+amb.mostrar_ambiente()
+amb.mostrar_percepcoes()
+```
 
 <br>
 
 ## [Link Versão 01](https://github.com/Oseiasdfarias/IA_mundo_do_wumpus/tree/versao_1)
 
 **Etapa 2 - Agente Reativo (Versão 1).**
 
@@ -45,14 +49,27 @@
       <li>Se < percepções > então < ação >.</li>
     </ul>
   <li>Este conjunto de regras (ou Base de Conhecimento) deve ser especificado por meio de uma tabela, aos moldes da que foi especificada, inicialmente, na “Aula 04';</li>
   <li>A partir da especificação, o próximo passo é codificar o Agente e integrar ao “Gerador Aleatório de Ambientes, de forma a ossibilitar a realização de testes de validação para posterior avaliação de performance;</li>
   <li>Obs.: Serão projetadas várias versões deste Agente. Nesta primeira versão, ele utiliza apenas o conjunto de regras como base de conhecimento. Ou seja, não tem memória e nenhum outro mecanismo mais sofisticado para escolher qual das possíveis regras utilizar. Para isto, deve ser uma escolha aleatória. Além disso, ele tem apenas uma única flecha.</li>
 </ul>
 
+```python title=main.py
+from ia_wumpus import AgenteReativoV1
+from ia_wumpus import Ambiente
+
+amb = Ambiente(dimensao_ambiente=3)
+agente = AgenteReativoV1(amb)
+agente.verificar_atirar_wumpus()
+
+amb.mostrar_ambiente()
+pos_mov = agente.sortear_pos(agente.get_opcoes_mov())
+amb.atualiza_pos_agente(pos_mov)
+amb.mostrar_ambiente()
+```
 
 
 <br>
 
 ## [Link Versão 02](https://github.com/Oseiasdfarias/IA_mundo_do_wumpus/tree/versao_2)
 
 **Etapa 3 - Agente Reativo (Versão 2).**
```

### Comparing `ia_wumpus-0.3.7/ia_wumpus/__init__.py` & `ia_wumpus-0.3.8/ia_wumpus/__init__.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.7/ia_wumpus/agente_reativo_v1.py` & `ia_wumpus-0.3.8/ia_wumpus/agente_reativo_v1.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.7/ia_wumpus/ambiente.py` & `ia_wumpus-0.3.8/ia_wumpus/ambiente.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.7/ia_wumpus/dinamica_agente_ambiente.py` & `ia_wumpus-0.3.8/ia_wumpus/dinamica_agente_ambiente.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.7/PKG-INFO` & `ia_wumpus-0.3.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: ia-wumpus
-Version: 0.3.7
+Version: 0.3.8
 Summary: Projeto O Mundo do Wumpus - Anbiente para estudo da disciplina de Inteligencia Computacional.
 Author: Oseiasdfarias
 Author-email: oseias.dfarias@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Description-Content-Type: text/markdown
 
+# Mundo do Wumpus - Intelegência Computacional
 
-<img src="https://github.com/Oseiasdfarias/IA_mundo_do_wumpus/blob/main/utils/logo.png?raw=true" alt="Logo UFPA" style="width:50px">
-
-
-<strong>Universidade Federal do Pará</strong>\
-<strong>Campus Universitário de Tucuruí</strong>\
-<strong>Faculdade de Engenharia Elétrica</strong>
+Ambiente para estudo de modelos de Apredizagem de Máquina da disciplina de Inteligência Computacional.
 
 <br>
 
-# Mundo do Wumpus - Intelegência Computacional
+## Documentação
 
-Ambiente para estudo de modelos de Apredizagem de Máquina da disciplina de Inteligência Computacional.
+### [Documentação ia-wumpus](https://oseiasdfarias.github.io/IA_mundo_do_wumpus/)
 
 <br>
 
 # Versões do Projeto
 
 <img src="https://raw.githubusercontent.com/Oseiasdfarias/IA_mundo_do_wumpus/340951a7d59c7ce6e3c981455b77638781b23d52/docs/static/img/code_demo.svg" alt="Ambiente Mundo do Wumpus." style="width:900px">
 
@@ -45,14 +41,22 @@
   <li>Tamanho (n) = ordem(n) da matriz quadrada (n >= 3). Linha e coluna = (n - 1);</li>
   <li>Objetos: poços (p), Wumpus (W) e ouro (o). Quantidade? [São parâmetros definidos pelo usuário (p, W, o >= O). E, também, podem ser atribuídos automaticamente, de acordo com o tamanho do ambiente (n), via a definição de alguma regra].</li>
   <li>A partir dos objetos, posicionar no ambiente, também, as percepções geradas por cada um deles.</li>
   <li>A casa (0,0) é a única que não pode ter nenhum objeto, pois é a posição inicial do Agente</li>
   <li>Onde houver poço não pode ser posicionado o ouro e o Wumpus. No entanto, estes podem ser posicionados em quaisquer uma das outras casas.</li>
 </ul>
 
+```python title=main.py
+from ia_wumpus import Ambiente
+
+
+amb = Ambiente(dimensao_ambiente=3)
+amb.mostrar_ambiente()
+amb.mostrar_percepcoes()
+```
 
 <br>
 
 ## [Link Versão 01](https://github.com/Oseiasdfarias/IA_mundo_do_wumpus/tree/versao_1)
 
 **Etapa 2 - Agente Reativo (Versão 1).**
 
@@ -62,14 +66,27 @@
       <li>Se < percepções > então < ação >.</li>
     </ul>
   <li>Este conjunto de regras (ou Base de Conhecimento) deve ser especificado por meio de uma tabela, aos moldes da que foi especificada, inicialmente, na “Aula 04';</li>
   <li>A partir da especificação, o próximo passo é codificar o Agente e integrar ao “Gerador Aleatório de Ambientes, de forma a ossibilitar a realização de testes de validação para posterior avaliação de performance;</li>
   <li>Obs.: Serão projetadas várias versões deste Agente. Nesta primeira versão, ele utiliza apenas o conjunto de regras como base de conhecimento. Ou seja, não tem memória e nenhum outro mecanismo mais sofisticado para escolher qual das possíveis regras utilizar. Para isto, deve ser uma escolha aleatória. Além disso, ele tem apenas uma única flecha.</li>
 </ul>
 
+```python title=main.py
+from ia_wumpus import AgenteReativoV1
+from ia_wumpus import Ambiente
+
+amb = Ambiente(dimensao_ambiente=3)
+agente = AgenteReativoV1(amb)
+agente.verificar_atirar_wumpus()
+
+amb.mostrar_ambiente()
+pos_mov = agente.sortear_pos(agente.get_opcoes_mov())
+amb.atualiza_pos_agente(pos_mov)
+amb.mostrar_ambiente()
+```
 
 
 <br>
 
 ## [Link Versão 02](https://github.com/Oseiasdfarias/IA_mundo_do_wumpus/tree/versao_2)
 
 **Etapa 3 - Agente Reativo (Versão 2).**
```

