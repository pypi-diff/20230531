# Comparing `tmp/satdigitalinvoice-4.0.7.tar.gz` & `tmp/satdigitalinvoice-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-4.0.7.tar", last modified: Mon May  1 16:21:40 2023, max compression
+gzip compressed data, was "satdigitalinvoice-4.0.8.tar", last modified: Wed May 31 02:35:25 2023, max compression
```

## Comparing `satdigitalinvoice-4.0.7.tar` & `satdigitalinvoice-4.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-01 16:21:40.000000 satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-01 16:21:40.000000 satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:21:40.000000 satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-01 16:21:40.000000 satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 16:21:40.000000 satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42176 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14568 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31447 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-31 02:35:25.000000 satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-31 02:35:25.000000 satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 02:35:25.000000 satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-31 02:35:25.000000 satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 02:35:25.000000 satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/tests/test_main.py
```

### Comparing `satdigitalinvoice-4.0.7/PKG-INFO` & `satdigitalinvoice-4.0.8/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.7
+Version: 4.0.8
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/__init__.py` & `satdigitalinvoice-4.0.8/satdigitalinvoice/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 
 DATA_DIRECTORY = ".data"
 ARCHIVOS_DIRECTORY = "archivos"
 METADATA_FILE = os.path.join(ARCHIVOS_DIRECTORY, "metadata.csv")
 TEMPLATES_DIRECTORY = "templates"
 TEMP_DIRECTORY = ".data/temp"
 
-PPD = "PPD"
-PUE = "PUE"
-
 
 def add_file_handler():
     os.makedirs(DATA_DIRECTORY, exist_ok=True)
     fh = logging.FileHandler(
         os.path.join(DATA_DIRECTORY, 'errors.log'),
         mode='a',
         encoding='utf-8',
```

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/__version__.py` & `satdigitalinvoice-4.0.8/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-4.0.8/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/environments.py` & `satdigitalinvoice-4.0.8/satdigitalinvoice/environments.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from datetime import date
 from html import escape as html_escape
 
 import jinja2
 from jinja2 import Environment, Undefined
 from jinja2.filters import do_mark_safe
-# noinspection PyUnresolvedReferences
-from satcfdi.transform.catalog import CATALOGS
 from satcfdi.transform.helpers import iterate as h_iterate
-from satdigitalinvoice.formatting_functions.common import pesos, num_letras, fecha as c_fecha
+import satdigitalinvoice.formatting_functions.common as common
 
 from . import TEMPLATES_DIRECTORY
 
 
 class FacturacionEnvironment(Environment):
     @property
     def filter(self):
@@ -52,27 +50,27 @@
         def bold(k):
             return do_mark_safe(
                 tag(html_escape(str(k)), "b")
             )
 
         @self.filter
         def moneda_nacional(k):
-            return pesos(k)
+            return common.pesos(k)
 
         @self.filter
         def numero(k):
-            return str(k) + ' (' + num_letras(k) + ')'
+            return common.numero(k)
 
         @self.filter
         def porcentaje(k):
-            return str(k) + '% (' + num_letras(k) + ' POR CIENTO)'
+            return common.porcentaje(k)
 
         @self.filter
         def fecha(k):
-            return c_fecha(k)
+            return common.fecha(k)
 
 
 def tag(text, tag):
     return '<' + tag + '>' + text + '</' + tag + '>'
 
 
 facturacion_environment = FacturacionEnvironment()
```

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-4.0.8/satdigitalinvoice/facturacion.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,31 +10,30 @@
 
 from PySimpleGUI import POPUP_BUTTONS_OK_CANCEL, PySimpleGUI as sg, POPUP_BUTTONS_NO_BUTTONS
 from satcfdi import DatePeriod, csf
 from satcfdi.accounting import EmailManager
 from satcfdi.accounting.models import EstadoComprobante
 from satcfdi.accounting.process import complement_invoices
 from satcfdi.create.cfd import cfdi40
+from satcfdi.create.cfd.catalogos import MetodoPago, TipoDeComprobante
 from satcfdi.exceptions import ResponseError
 from satcfdi.pacs import Accept
 from satcfdi.pacs.sat import SAT, EstadoSolicitud
-# noinspection PyUnresolvedReferences
-from satcfdi.transform.catalog import CATALOGS
 from xlsxwriter.exceptions import XlsxFileError
 
-from . import __version__, PPD, PUE, TEMP_DIRECTORY, ARCHIVOS_DIRECTORY, DATA_DIRECTORY, METADATA_FILE
+from . import __version__, TEMP_DIRECTORY, ARCHIVOS_DIRECTORY, DATA_DIRECTORY, METADATA_FILE
 from .client_validation import validar_client, clientes_generar_txt
 from .environments import facturacion_environment
 from .file_data_managers import ClientsManager, FacturasManager
 from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, archivos_folder, period_desc, parse_fecha_pago, parse_importe_pago, preview_cfdis, center_location, \
     CALENDAR_FECHA_FMT, ConsoleErrors, \
-    generate_ajustes
+    generate_ajustes, generar_depositos, generate_pdf_template
 from .layout import make_layout, ActionButtonManager, TipoRecuperar, SearchOptions
 from .localdb import LocalDBSatCFDI, StatusState
-from .log_tools import cfdi_header, header_line, print_yaml
+from .log_tools import header_line, print_yaml
 from .mycfdi import MyCFDI
 from .utils import random_string, to_date_period, load_certificate, to_int, cert_info, add_month, to_uuid, open_file, OS
 
 logging.getLogger("weasyprint").setLevel(logging.ERROR)
 logging.getLogger("fontTools").setLevel(logging.ERROR)
 
 logger = logging.getLogger(__name__)
@@ -44,16 +43,14 @@
     layout = [[sg.Text("New Window", key="new")]]
     window = sg.Window("Launch Window", layout, modal=True, size=(300, 300))
     window.read(timeout=1000)
 
     return window
 
 
-
-
 class FacturacionGUI:
     def __init__(self, config):
         os.makedirs(TEMP_DIRECTORY, exist_ok=True)
         self.email_manager = EmailManager(
             **config['email']
         )
         pac = config['pac']
@@ -64,15 +61,15 @@
         )
         self.csd_signer = load_certificate(config.get('csd')) if 'csd' in config else None
         self.fiel_signer = load_certificate(config.get('fiel')) if 'fiel' in config else None
 
         self.sat_service = SAT(signer=self.fiel_signer)
         self.rfc_prediales = config['rfc_prediales']
 
-        self.all_invoices = None
+        self._all_invoices = None
         self.local_db = LocalDBSatCFDI(
             base_path=DATA_DIRECTORY,
             enviar_a_partir=config['enviar_a_partir'],
             pagar_a_partir=config['pagar_a_partir']
         )
 
         MyCFDI.local_db = self.local_db
@@ -98,25 +95,25 @@
         )
         self.console = self.window["console"]
         self.set_inputs()
 
         self.window.bind("<FocusIn>", "_focus_in")
         self.window.bind("<FocusOut>", "_focus_out")
 
-        for t in ('facturas_periodo', 'emitidas_search', 'ajustes_periodo', 'serie', 'folio', 'serie_pago'):
+        for t in ('facturas_periodo', 'emitidas_search', 'ajustes_periodo', 'depositos_periodo', 'serie', 'folio', 'serie_pago'):
             self.window[t].bind("<Return>", "_enter")
             self.window[t].bind("<FocusOut>", "_enter", propagate=False)
 
         modifier_key = "Command" if OS.get_os() == OS.MACOS else "Control"
 
-        for t in ('facturas_table', 'clientes_table', 'emitidas_table', 'correos_table', 'ajustes_table', 'solicitudes_table'):
+        for t in ('facturas_table', 'clientes_table', 'emitidas_table', 'correos_table', 'ajustes_table', 'depositos_table', 'solicitudes_table'):
             self.window[t].bind(f'<{modifier_key}-a>', '+select_all')
             self.window[t].bind('<BackSpace>', '+delete')  # BackSpace
             # self.window[t].bind('<Double-Button-1>', '_enter')
-            self.window[t].bind('<Return>', '_enter')
+            self.window[t].bind('<Return>', '+enter')
 
     def run(self):
         self.main_loop()
         self.window.close()
 
     def initial_screen(self, emisor_cif):
         self.header("ACERCA DE")
@@ -130,64 +127,67 @@
                 "Environment": str(self.pac_service.environment)
             },
             "fiel": cert_info(self.fiel_signer),
             "csd": cert_info(self.csd_signer),
         })
 
     def get_all_invoices(self):
-        if not self.all_invoices:
-            self.all_invoices = MyCFDI.get_all_cfdi()
-        return self.all_invoices
+        if not self._all_invoices:
+            self._all_invoices = MyCFDI.get_all_cfdi()
+        return self._all_invoices
 
     def add_created_invoice(self, invoice: MyCFDI):
-        self.all_invoices[invoice.uuid] = invoice
-        complement_invoices(self.all_invoices, invoice)
+        self._all_invoices[invoice.uuid] = invoice
+        complement_invoices(self._all_invoices, invoice)
 
     def generate_invoice(self, invoice):
         ref_id = random_string()
+        title = 'Generando factura'
 
         # Add Serie and Folio and signature
         folio = None
         if 'Serie' not in invoice:
             invoice['Serie'] = self.local_db.serie()
             folio = self.local_db.folio()
             invoice['Folio'] = str(folio)
 
         cfdi40.Comprobante.sign(invoice, self.csd_signer)
 
         attempts = 3
-        for i in range(attempts):
-            if i:
-                print(f'Intentando de nuevo... Intento {i + 1} de {attempts}')
-                if not self._read(timeout=2000 * i):
-                    return
-
-            try:
-                res = self.pac_service.stamp(
-                    cfdi=invoice,
-                    accept=Accept.XML_PDF,
-                    ref_id=ref_id
-                )
-            except Exception as ex:
-                self.show_console()
-                message = f"Error al generar factura: {invoice.get('Serie')}{invoice.get('Folio')} {invoice['Receptor']['Rfc']}"
-                logger.exception(message)
-                print(message)
-                if isinstance(ex, ResponseError):
-                    logger.error(f"Status Code: {ex.response.status_code}")
-                    print(f"Status Code: {ex.response.status_code}")
-                    logger.error(f"Response: {ex.response.text}")
-                    print(f"Response: {ex.response.text}")
-                continue
-
-            if folio is not None:
-                self.set_folio(folio + 1)
-            cfdi = MyCFDI.move_to_folder(res.xml, pdf_data=res.pdf)
-            self.add_created_invoice(cfdi)
-            return cfdi
+        try:
+            for i in self.progress_iterate(
+                    title, range(attempts), lambda r: f'Intentando de nuevo... Intento {r + 1} de {attempts}', skip_first=True, delay=2000
+            ):
+                try:
+                    res = self.pac_service.stamp(
+                        cfdi=invoice,
+                        accept=Accept.XML_PDF,
+                        ref_id=ref_id
+                    )
+                except Exception as ex:
+                    self.show_console()
+                    message = f"Error al generar factura: {invoice.get('Serie')}{invoice.get('Folio')} {invoice['Receptor']['Rfc']}"
+                    message += f"\nIntento {i + 1} de {attempts}"
+
+                    logger.exception(message)
+                    print(message)
+                    if isinstance(ex, ResponseError):
+                        logger.error(f"Status Code: {ex.response.status_code}")
+                        print(f"Status Code: {ex.response.status_code}")
+                        logger.error(f"Response: {ex.response.text}")
+                        print(f"Response: {ex.response.text}")
+                    continue
+
+                if folio is not None:
+                    self.set_folio(folio + 1)
+                cfdi = MyCFDI.move_to_folder(res.xml, pdf_data=res.pdf)
+                self.add_created_invoice(cfdi)
+                return cfdi
+        finally:
+            self.progress_cancel(title)
 
     def set_serie(self, serie: str = None):
         if serie:
             self.local_db.serie_set(serie.strip())
         self.set_inputs()
 
     def set_serie_pago(self, serie: str = None):
@@ -227,204 +227,216 @@
         response = self.sat_service.recover_comprobante_request(
             **args
         )
 
         self.local_db.solicitud_merge(response["IdSolicitud"], request=args, response=response)
 
     def recupera_comprobantes(self, response):
-        if response["EstadoSolicitud"] == EstadoSolicitud.Terminada:
+        if response["EstadoSolicitud"] == EstadoSolicitud.TERMINADA:
             for id_paquete in response['IdsPaquetes']:
                 r, paquete = self.sat_service.recover_comprobante_download(
                     id_paquete=id_paquete
                 )
                 print(f"paquete: {id_paquete}")
                 print_yaml(r)
                 if paquete:
                     data = base64.b64decode(paquete)
                     with io.BytesIO(data) as b:
                         self.unzip_cfdi(b)
 
     def unzip_cfdi(self, file):
+        title = 'Descomprimiendo'
         with ZipFile(file, "r") as zf:
-            for fileinfo in self.progress_iterate(zf.infolist(), 'Descomprimiendo'):
-                data = zf.read(fileinfo)
-                match os.path.splitext(fileinfo.filename)[1]:
-                    case ".xml":
-                        self.all_invoices = None
-                        MyCFDI.move_to_folder(data, pdf_data=None)
-                    case ".pdf":
-                        pass
-                    case ".txt":
-                        cfdi_metadata_reader = csv.reader(
-                            (c.decode('utf-8') for c in data.splitlines() if c),
-                            delimiter='~',
-                            quotechar='|'
-                        )
-                        header = next(cfdi_metadata_reader)
-                        for row in cfdi_metadata_reader:
-                            row = dict(zip(header, row))
-                            print_yaml(row)
-                            self.local_db.status_merge(
-                                uuid=row['Uuid'],
-                                estatus=row['Estatus'],
-                                fecha_cancelacion=row['FechaCancelacion']
+            try:
+                for fileinfo in self.progress_iterate(title, zf.infolist()):
+                    data = zf.read(fileinfo)
+                    match os.path.splitext(fileinfo.filename)[1]:
+                        case ".xml":
+                            self._all_invoices = None
+                            MyCFDI.move_to_folder(data, pdf_data=None)
+                        case ".pdf":
+                            pass
+                        case ".txt":
+                            cfdi_metadata_reader = csv.reader(
+                                (c.decode('utf-8') for c in data.splitlines() if c),
+                                delimiter='~',
+                                quotechar='|'
                             )
+                            header = next(cfdi_metadata_reader)
+                            for row in cfdi_metadata_reader:
+                                row = dict(zip(header, row))
+                                print_yaml(row)
+                                self.local_db.status_merge(
+                                    uuid=row['Uuid'],
+                                    estatus=row['Estatus'],
+                                    fecha_cancelacion=row['FechaCancelacion']
+                                )
+            finally:
+                self.progress_cancel(title)
 
     def _read(self, timeout=0):
         event, values = self.window.read(timeout=timeout)
         if event in ("Exit", sg.WIN_CLOSED):
             return False
         return True
 
-    def progress_iterate(self, items, title, fn=None):
-        ln = None
-        if hasattr(items, '__len__'):
-            ln = len(items)
-
-        for i, item in enumerate(items):
-            if not sg.one_line_progress_meter(
-                    'Progress Meter',
-                    i,
-                    ln or (i + 1),
-                    title,
-                    fn(item) if callable(fn) else "",
-                    keep_on_top=True,
-                    no_titlebar=True,
-                    grab_anywhere=True,
-            ):
-                return
-            yield item
-            if not self._read():
-                return
-        sg.one_line_progress_meter_cancel()
+    def progress_iterate(self, title, items, fn=None, skip_first=False, delay=0):
+        ln = len(items)
+        try:
+            for i, item in enumerate(items):
+                if skip_first and i == 0:
+                    pass
+                else:
+                    if not sg.one_line_progress_meter(
+                            '',
+                            i,
+                            ln,
+                            title,
+                            fn(item) if callable(fn) else "",
+                            key=title,
+                            keep_on_top=True,
+                            no_titlebar=True,
+                            grab_anywhere=True,
+                    ):
+                        return
 
-    def action_button(self, action_name, action_items, action_text):
-        match action_name:
-            case 'solicitudes':
-                self.show_console()
-                for solicitud in self.progress_iterate(action_items, action_text):
-                    id_solicitud = solicitud["response"]["IdSolicitud"]
-                    response = self.sat_service.recover_comprobante_status(
-                        id_solicitud=id_solicitud
-                    )
-                    print_yaml(response)
-                    self.local_db.solicitud_merge(id_solicitud, response=response)
-                    self.recupera_comprobantes(response)
-
-            case 'facturas' | 'pago':
-                for invoice in self.progress_iterate(action_items, action_text):
-                    cfdi = self.generate_invoice(invoice=invoice)
-                    if cfdi is None:
-                        break
+                if not self._read(timeout=delay * i):
+                    return
 
-            case 'correos':
-                clients = ClientsManager()
-                emisor = clients[self.csd_signer.rfc]
-                with self.email_manager.sender as s:
-                    for receptor, facturas, facturas_facturas_pendientes_meses_anteriores in self.progress_iterate(action_items, action_text):
-                        def attachments():
-                            for ni in facturas:
-                                yield ni.filename + ".xml"
-                                yield ni.filename + ".pdf"
-
-                        s.send_email(
-                            subject=f"Comprobantes Fiscales {receptor['RazonSocial']} - {receptor['Rfc']}",
-                            to_addrs=receptor["Email"],
-                            html=facturacion_environment.get_template('mail_facturas_template.html').render(
-                                facturas=facturas,
-                                facturas_pendientes_meses_anteriores=facturas_facturas_pendientes_meses_anteriores,
-                                emisor=emisor,
-                                receptor=receptor,
-                            ),
-                            file_attachments=attachments()
-                        )
-                        for r in facturas:
-                            self.local_db.notified_set(r.uuid, True)
+                yield item
+        finally:
+            self.progress_cancel(title)
+
+    @staticmethod
+    def progress_cancel(title):
+        sg.one_line_progress_meter_cancel(
+            key=title
+        )
 
-            case 'ajustes':
-                clients = ClientsManager()
-                emisor = clients[self.csd_signer.rfc]
-                with self.email_manager.sender as s:
-                    for data in self.progress_iterate(action_items, action_text):
-                        if not data['ajuste_porcentaje']:
-                            continue
-
-                        receptor = data['receptor']
-                        file_name = data['file_name']
-
-                        s.send_email(
-                            subject=f"Ajuste Renta {receptor['RazonSocial']} - {receptor['Rfc']}",
-                            to_addrs=receptor["Email"],
-                            html=facturacion_environment.get_template('mail_ajustes_template.html').render(
-                                emisor=emisor,
-                                receptor=receptor,
-                            ),
-                            file_attachments=[file_name]
-                        )
+    def action_button(self, action_name, action_items, action_text):
+        try:
+            match action_name:
+                case 'solicitudes':
+                    for solicitud in self.progress_iterate(action_text, action_items):
+                        id_solicitud = solicitud["response"]["IdSolicitud"]
+                        response = self.sat_service.recover_comprobante_status(
+                            id_solicitud=id_solicitud
+                        )
+                        print_yaml(response)
+                        self.local_db.solicitud_merge(id_solicitud, response=response)
+                        self.recupera_comprobantes(response)
+
+                case 'facturas' | 'pago':
+                    for invoice in self.progress_iterate(action_text, action_items):
+                        if not self.generate_invoice(invoice=invoice):
+                            break
+
+                case 'correos':
+                    clients = ClientsManager()
+                    emisor = clients[self.csd_signer.rfc]
+                    with self.email_manager.sender as s:
+                        for receptor, facturas, facturas_facturas_pendientes_meses_anteriores in self.progress_iterate(action_text, action_items):
+                            def attachments():
+                                for ni in facturas:
+                                    yield ni.filename + ".xml"
+                                    yield ni.filename + ".pdf"
+
+                            s.send_email(
+                                subject=f"Comprobantes Fiscales {receptor['RazonSocial']} - {receptor['Rfc']}",
+                                to_addrs=receptor["Email"],
+                                html=facturacion_environment.get_template('mail_facturas_template.html').render(
+                                    facturas=facturas,
+                                    facturas_pendientes_meses_anteriores=facturas_facturas_pendientes_meses_anteriores,
+                                    emisor=emisor,
+                                    receptor=receptor,
+                                ),
+                                file_attachments=attachments()
+                            )
+                            for r in facturas:
+                                self.local_db.notified_set(r.uuid, True)
 
-            case 'clientes':
-                for client in self.progress_iterate(
-                        action_items, action_text, lambda x: f"Validando: {x['Rfc']}"
-                ):
-                    validar_client(client)
+                case 'ajustes' | 'depositos':
+                    with self.email_manager.sender as s:
+                        for data in self.progress_iterate(action_text, action_items):
+                            if file_name := data['create_fn']():
+                                receptor = data['receptor']
+                                if action_name == 'ajustes':
+                                    subject = f"Ajuste Renta {receptor['RazonSocial']} - {receptor['Rfc']}"
+                                elif action_name == 'depositos':
+                                    subject = f"Depósito Renta {receptor['RazonSocial']} - {receptor['Rfc']}"
+                                else:
+                                    raise NotImplementedError()
+
+                                s.send_email(
+                                    subject=subject,
+                                    to_addrs=receptor["Email"],
+                                    html=facturacion_environment.get_template(f'mail_{action_name}_template.html').render(data),
+                                    file_attachments=[file_name]
+                                )
 
-            case _:
-                raise ValueError(f"Invalid action: {action_name}")
+                case 'clientes':
+                    for client in self.progress_iterate(
+                            action_text, action_items, lambda x: f"Validando: {x['Rfc']}"
+                    ):
+                        validar_client(client)
 
-        sg.one_line_progress_meter_cancel()
+                case _:
+                    raise ValueError(f"Invalid action: {action_name}")
+        finally:
+            self.progress_cancel(action_text)
 
     def set_selected_satcfdis(self, cfdis: list):
         i = cfdis[0] if len(cfdis) == 1 else None
 
         if i:
             estatus = EstadoComprobante(i.estatus)
             self.window["status_sat"].update(
                 estatus.name.center(10),
                 disabled=False,
-                button_color="red4" if estatus != EstadoComprobante.Vigente else "dark green",
+                button_color="red4" if estatus != EstadoComprobante.VIGENTE else "dark green",
             )
         else:
             self.window["status_sat"].update(
                 "".ljust(10), disabled=True, button_color=sg.theme_background_color()
             )
 
         # Email
         is_active = \
             bool(i) \
             and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-            and i.estatus == EstadoComprobante.Vigente
+            and i.estatus == EstadoComprobante.VIGENTE
         if is_active:
             self.window["email_notificada"].update(
                 "Enviada".center(10) if self.local_db.notified(i) else "Por Enviar",
                 disabled=False,
                 button_color="dark green" if self.local_db.notified(i) else "red4",
             )
         else:
             self.window["email_notificada"].update(
                 "".ljust(10), disabled=True, button_color=sg.theme_background_color()
             )
 
         # Pendiente de Pago
         is_pendientable = \
             is_active \
-            and i["TipoDeComprobante"] == "I" \
-            and (i["MetodoPago"] == PUE or i.saldo_pendiente) \
+            and i["TipoDeComprobante"] == TipoDeComprobante.INGRESO \
+            and (i["MetodoPago"] == MetodoPago.PAGO_EN_UNA_SOLA_EXHIBICION or i.saldo_pendiente) \
             and i["Total"]
         if is_pendientable:
             self.window["pendiente_pago"].update(
-                (("Pagada" if i["MetodoPago"] == PUE else "Ignorada")
+                (("Pagada" if i["MetodoPago"] == MetodoPago.PAGO_EN_UNA_SOLA_EXHIBICION else "Ignorada")
                  if self.local_db.liquidated(i) else "Por Pagar").center(10),
                 disabled=False,
-                button_color=("dark green" if i["MetodoPago"] == PUE else "yellow4")
+                button_color=("dark green" if i["MetodoPago"] == MetodoPago.PAGO_EN_UNA_SOLA_EXHIBICION else "yellow4")
                 if self.local_db.liquidated(i) else "red4",
             )
         else:
             is_ppd_pagada = is_active \
-                            and i["TipoDeComprobante"] == "I" \
-                            and i["MetodoPago"] == PPD \
+                            and i["TipoDeComprobante"] == TipoDeComprobante.INGRESO \
+                            and i["MetodoPago"] == MetodoPago.PAGO_EN_PARCIALIDADES_O_DIFERIDO \
                             and i.saldo_pendiente == 0
             if is_ppd_pagada:
                 self.window["pendiente_pago"].update(
                     "Pagada".center(10),
                     disabled=True,
                     button_color="dark green",
                 )
@@ -434,16 +446,16 @@
                     disabled=True,
                     button_color=sg.theme_background_color()
                 )
 
         # PPD
         is_ppd_active = \
             is_active \
-            and i["TipoDeComprobante"] == "I" \
-            and i["MetodoPago"] == PPD \
+            and i["TipoDeComprobante"] == TipoDeComprobante.INGRESO \
+            and i["MetodoPago"] == MetodoPago.PAGO_EN_PARCIALIDADES_O_DIFERIDO \
             and i.saldo_pendiente > 0
 
         self.window["ppd_action_items"].update(visible=is_ppd_active)
         self.window["importe_pago"].update(i.saldo_pendiente if is_ppd_active else '')
         if is_ppd_active:
             self.action_button_manager.set_items("pago", [i])
         else:
@@ -456,15 +468,15 @@
         self._read()
 
     def show_console(self):
         self.window['errores_tab'].select()
 
     def download_invoice(self, uuid: UUID):
         res = self.pac_service.recover(uuid, accept=Accept.XML_PDF)
-        self.all_invoices = None
+        self._all_invoices = None
         return MyCFDI.move_to_folder(res.xml, pdf_data=res.pdf)
 
     def facturas_search(self):
         search_text = self.window["emitidas_search"].get()
         search_text = search_text.strip()
 
         if len(search_text) < 3:
@@ -476,15 +488,15 @@
                     if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                             and self.local_db.liquidated_state(i) == StatusState.PENDING:
                         yield i
             elif search_text == SearchOptions.PorEnviar:
                 for i in self.get_all_invoices().values():
                     if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                             and not self.local_db.notified(i) \
-                            and i.estatus == EstadoComprobante.Vigente:
+                            and i.estatus == EstadoComprobante.VIGENTE:
                         yield i
             elif date_search_text := to_date_period(search_text):
                 for i in self.get_all_invoices().values():
                     if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                             and i["Fecha"] == date_search_text:
                         yield i
             elif uuid_search_text := to_uuid(search_text):
@@ -594,14 +606,38 @@
                 dp_effective=dp_effective,
                 emisor_rfc=self.csd_signer.rfc
             )
             ajustes_table.update(
                 values=ajustes,
             )
 
+    def nuevos_depositos(self, values, force=False):
+        depositos_table = self.window['depositos_table']
+        has_value = bool(depositos_table.metadata)
+        depositos_table.update(values=[])
+        self.window['preparar_depositos_text'].update("")
+
+        if has_value or force:
+            dp = to_date_period(values["depositos_periodo"])
+            if dp is None or dp.month is None:
+                raise ValueError("Periodo no válido")
+
+            self.window['preparar_depositos_text'].update(f"{period_desc(dp)}")
+
+            depositos = generar_depositos(
+                clients=ClientsManager(),
+                facturas=FacturasManager(dp)["Facturas"],
+                dp=dp,
+                emisor_rfc=self.csd_signer.rfc,
+
+            )
+            depositos_table.update(
+                values=depositos,
+            )
+
     def main_tab_group(self, values):
         self.action_button_manager.clear()
 
         match values['main_tab_group']:
             case 'facturas_tab':
                 self.nuevas_facturas(values)
 
@@ -619,15 +655,15 @@
                 clients = ClientsManager()
 
                 def correos():
                     for receptor_rfc, notify_invoices in itertools.groupby(
                             sorted(
                                 (i for i in self.get_all_invoices().values()
                                  if i["Emisor"]["Rfc"] == self.csd_signer.rfc
-                                    and i.estatus == EstadoComprobante.Vigente
+                                    and i.estatus == EstadoComprobante.VIGENTE
                                     and not self.local_db.notified(i)
                                  ),
                                 key=lambda r: r["Receptor"]["Rfc"]
                             ),
                             lambda r: r["Receptor"]["Rfc"]
                     ):
                         notify_invoices = list(notify_invoices)
@@ -650,14 +686,17 @@
                 self.window['correos_table'].update(
                     values=list(correos()),
                 )
 
             case 'ajustes_tab':
                 self.nuevos_ajustes(values)
 
+            case 'depositos_tab':
+                self.nuevos_depositos(values)
+
             case 'solicitudes_tab':
                 solitudes = self.local_db.get_solicitudes()
                 self.window['solicitudes_table'].update(
                     values=list(solitudes.values()),
                 )
 
     def main_loop(self):
@@ -709,68 +748,76 @@
 
                     case "facturas_periodo_enter":
                         self.nuevas_facturas(values, force=True)
 
                     case "ajustes_periodo_enter":
                         self.nuevos_ajustes(values, force=True)
 
+                    case "depositos_periodo_enter":
+                        self.nuevos_depositos(values, force=True)
+
                     case 'main_tab_group':
                         self.main_tab_group(values)
 
-                    case 'facturas_table_enter':
+                    case 'facturas_table+enter':
                         # noinspection PyUnresolvedReferences
                         if s_items := self.window["facturas_table"].selected_items():
                             preview_cfdis(s_items)
 
-                    case 'clientes_table_enter':
+                    case 'clientes_table+enter':
                         # noinspection PyUnresolvedReferences
                         for client in self.window["clientes_table"].selected_items():
                             url = csf.url(rfc=client["Rfc"], id_cif=client["IdCIF"])
                             open_file(url)
 
-                    case 'emitidas_table_enter':
+                    case 'emitidas_table+enter':
                         # noinspection PyUnresolvedReferences
                         if s_items := self.window["emitidas_table"].selected_items():
                             preview_cfdis(s_items)
 
-                    case 'ajustes_table_enter':
+                    case 'ajustes_table+enter' | 'depositos_table+enter':
+                        table = event.split("+")[0]
                         # noinspection PyUnresolvedReferences
-                        for ajuste in self.window["ajustes_table"].selected_items():
-                            open_file(
-                                os.path.abspath(ajuste['file_name'])
-                            )
+                        for items in self.window[table].selected_items():
+                            if file_name := items['create_fn']():
+                                open_file(
+                                    os.path.abspath(file_name)
+                                )
+                            else:
+                                self.error_message("No se pudo crear el archivo")
 
-                    case 'correos_table_enter' | 'solicitudes_table_enter':
+                    case 'correos_table+enter' | 'solicitudes_table+enter':
                         pass
 
-                    case "facturas_table" | "clientes_table" | "correos_table" | "ajustes_table" | "emitidas_table" | "solicitudes_table":
+                    case "facturas_table" | "clientes_table" | "correos_table" | "ajustes_table" | "depositos_table" | "emitidas_table" | "solicitudes_table" | "depositos_table":
                         # noinspection PyUnresolvedReferences
                         s_items = self.window[event].selected_items()
                         if event == "emitidas_table":
                             self.set_selected_satcfdis(s_items)
                         else:
                             self.action_button_manager.set_items(event.split("_")[0], s_items)
 
                     case "facturas_table+select_all" | "clientes_table+select_all" | "correos_table+select_all" | \
-                         "ajustes_table+select_all" | "emitidas_table+select_all" | 'solicitudes_table+select_all':
+                         "ajustes_table+select_all" | "emitidas_table+select_all" | 'solicitudes_table+select_all' | \
+                         'depositos_table+select_all':
                         # noinspection PyUnresolvedReferences
                         self.window[event.split("+")[0]].select_all()
 
                     case "facturas_table+delete" | "clientes_table+delete" | "correos_table+delete" | \
                          "ajustes_table+delete" | "emitidas_table+delete":
                         # noinspection PyUnresolvedReferences
                         # self.window[event.split("+")[0]].delete_selected()
                         pass
 
                     case "solicitudes_table+delete":
                         solitudes = self.local_db.get_solicitudes()
                         # noinspection PyUnresolvedReferences
                         sel = self.window["solicitudes_table"].selected_items()
                         for s in sel:
-                            if s["response"].get("EstadoSolicitud").code < EstadoSolicitud.Terminada:
+                            if s["response"].get("EstadoSolicitud").code < EstadoSolicitud.TERMINADA:
                                 self.error_message("No se puede eliminar una solicitud en proceso")
                                 continue
                             del solitudes[s["response"]["IdSolicitud"]]
                         self.local_db.set_solicitudes(solitudes)
                         self.main_tab_group(values)
 
                     case "status_sat":
@@ -880,15 +927,14 @@
 
                     case "organizar_facturas":
                         MyCFDI.rename_invoices(search_path="**/*.xml")
 
                     case "cargar_zip":
                         zip_file = sg.popup_get_file('', multiple_files=False, no_window=True, file_types=(("ZIP Files", "*.zip"),))
                         if zip_file:
-                            self.header("Cargar ZIP")
                             self.unzip_cfdi(zip_file)
 
                     case 'importar_emitidas':
                         csv_file = sg.popup_get_file('', multiple_files=False, no_window=True, file_types=(("CSV Files", "*.csv"),))
                         if csv_file:
                             all_invoices = self.get_all_invoices()
                             with open(csv_file, newline='', encoding='utf-8') as f:
```

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-4.0.8/satdigitalinvoice/file_data_managers.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,25 +6,21 @@
 import re
 from decimal import Decimal
 
 import jsonschema as jsonschema
 import yaml
 from satcfdi import Code, DatePeriod
 from satcfdi.pacs import sat
-# noinspection PyUnresolvedReferences
-from satcfdi.transform.catalog import CATALOGS
 from satcfdi.transform.helpers import Xint
 from yaml import MappingNode, SafeLoader
 from yaml.constructor import ConstructorError
 
 from . import SOURCE_DIRECTORY
 from .utils import find_best_match, first_duplicate
 
-REGIMEN_FISCAL = CATALOGS['{http://www.sat.gob.mx/sitio_internet/cfd/catalogos}c_RegimenFiscal']
-
 logger = logging.getLogger(__name__)
 sat_manager = sat.SAT()
 
 
 class DuplicateKeySafeLoader(SafeLoader):
     def construct_mapping(self, node, deep=False):
         if isinstance(node, MappingNode):
@@ -107,15 +103,15 @@
 
     def __init__(self):
         super().__init__()
         for k, v in self.items():
             if error := jsonschema.exceptions.best_match(client_validator.iter_errors(v)):
                 raise error
             self[k]["Rfc"] = k
-            self[k]["RegimenFiscal"] = Code(self[k]["RegimenFiscal"], REGIMEN_FISCAL.get(self[k]["RegimenFiscal"]))
+            self[k]["RegimenFiscal"] = self[k]["RegimenFiscal"]
 
 
 class FacturasManager(LocalData):
     file_source = "facturas.yaml"
 
     def __init__(self, dp: DatePeriod | None):
         def loading_function(loader, node):
```

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-4.0.8/satdigitalinvoice/gui_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 from satcfdi import DatePeriod
 from satcfdi.accounting import filter_invoices_iter, filter_payments_iter, invoices_export, payments_export
 from satcfdi.accounting.process import payments_groupby_receptor, payments_retentions_export
 from satcfdi.create.cfd import cfdi40
 from satcfdi.create.cfd.cfdi40 import Comprobante, PagoComprobante
 from satcfdi.pacs import sat
 from satcfdi.printer import Representable
-# noinspection PyUnresolvedReferences
-from satcfdi.transform.catalog import CATALOGS
 from weasyprint import HTML, CSS
 
 from . import SOURCE_DIRECTORY, ARCHIVOS_DIRECTORY, TEMP_DIRECTORY
 from .environments import facturacion_environment
 from .exceptions import ConsoleErrors
 from .formatting_functions.common import fecha_mes
-from .utils import add_month, find_best_match, months_between, clear_directory, open_file
+from .utils import add_month, find_best_match, months_between, open_file
 
 logger = logging.getLogger(__name__)
 logger.level = logging.INFO
 
 sat_manager = sat.SAT()
 
 PERIODICIDAD = {
@@ -209,16 +207,16 @@
             _, mes_aj = parse_periodo_mes_ajuste(concepto['_periodo_mes_ajuste'])
             if mes_aj == mes_ajuste:
                 yield rfc, concepto
 
 
 def generate_ajustes(clients, facturas, dp, dp_effective, emisor_rfc):
     errors = []
-    ajustes_dir = ajustes_directory(DatePeriod(dp.year, dp.month))
-    clear_directory(ajustes_dir)
+    ajustes_dir = os.path.join(archivos_folder(dp), 'ajustes')
+    os.makedirs(ajustes_dir, exist_ok=True)
 
     def ajustes_iter():
         for i, (receptor_rfc, concepto) in enumerate(find_ajustes(facturas, dp_effective.month), start=1):
             try:
                 valor_unitario_raw = concepto["ValorUnitario"]
 
                 if isinstance(valor_unitario_raw, dict):
@@ -238,46 +236,96 @@
                     vu = valor_unitario_raw
                     vun = None
                     num_meses = None
                     ajuste_porcentaje = None
 
                 concepto = format_concepto_desc(concepto, periodo="INMUEBLE")
                 file_name = os.path.join(ajustes_dir, f'AjusteRenta_{receptor_rfc}_{i}.pdf')
-
                 client_receptor = clients[receptor_rfc]  # type: dict
                 data = {
                     "receptor": client_receptor,
                     "emisor": clients[emisor_rfc],
                     "concepto": concepto,
                     "valor_unitario": vu,
                     "valor_unitario_nuevo": vun or '',
                     "ajuste_porcentaje": ajuste_porcentaje or "",
                     "meses": num_meses or '',
                     "efectivo_periodo_desc": periodicidad_desc(dp_effective, concepto['_periodo_mes_ajuste'], concepto.get('_desfase_mes')),
                     "periodo": concepto['_periodo_mes_ajuste'].split('.')[0].upper(),
-                    'file_name': file_name
                 }
+                data['create_fn'] = create_ajuste_fn(ajuste_porcentaje, data, file_name)
 
-                if ajuste_porcentaje:
-                    res = generate_pdf_template(
-                        template_name='incremento_template.md',
-                        fields=data
-                    )
-                    with open(file_name, 'wb') as f:
-                        f.write(res)
                 yield data
             except Exception as e:
                 errors.append(f"{i} {receptor_rfc}: {str(e)}")
 
     cfdis = list(ajustes_iter())
     if errors:
         raise ConsoleErrors("Generar Ajustes Errores", errors=errors)
     return cfdis
 
 
+def create_ajuste_fn(ajuste_porcentaje, data, file_name):
+    def fn():
+        if ajuste_porcentaje:
+            res = generate_pdf_template(
+                template_name='ajuste_template.md',
+                fields=data
+            )
+            with open(file_name, 'wb') as f:
+                f.write(res)
+            return file_name
+    return fn
+
+
+def generar_depositos(clients, facturas, dp, emisor_rfc):
+    errors = []
+    depositos_dir = os.path.join(archivos_folder(dp), 'depositos')
+    os.makedirs(depositos_dir, exist_ok=True)
+
+    def depositos_iter():
+        for i, (receptor_rfc, concepto) in enumerate(find_ajustes(facturas, dp.month), start=1):
+            try:
+                vu = concepto["ValorUnitario"]
+
+                concepto = format_concepto_desc(concepto, periodo="INMUEBLE")
+                file_name = os.path.join(depositos_dir, f'Deposito_{receptor_rfc}_{i}.pdf')
+
+                client_receptor = clients[receptor_rfc]  # type: dict
+                data = {
+                    "receptor": client_receptor,
+                    "emisor": clients[emisor_rfc],
+                    "concepto": concepto,
+                    "valor_unitario": vu,
+                    "periodo": concepto['_periodo_mes_ajuste'].split('.')[0].upper(),
+                }
+                data['create_fn'] = create_deposito_fn(data, file_name)
+                yield data
+            except Exception as e:
+                errors.append(f"{i} {receptor_rfc}: {str(e)}")
+
+    cfdis = list(depositos_iter())
+    if errors:
+        raise ConsoleErrors("Generar Depositos Errores", errors=errors)
+    return cfdis
+
+
+def create_deposito_fn(data, file_name):
+    def fn():
+        res = generate_pdf_template(
+            template_name='deposito_template.md',
+            fields=data
+        )
+        with open(file_name, 'wb') as f:
+            f.write(res)
+        return file_name
+
+    return fn
+
+
 def archivos_folder(dp: DatePeriod):
     if dp.month:
         return os.path.join(ARCHIVOS_DIRECTORY, str(dp.year), str(dp.year) + "-{:02d}".format(dp.month))
     return os.path.join(ARCHIVOS_DIRECTORY, str(dp.year))
 
 
 def archivos_filename(dp: DatePeriod, ext="xlsx"):
@@ -352,18 +400,14 @@
 def mf_pago_fmt(cfdi):
     i = cfdi
     if i['TipoDeComprobante'] == "I":
         return i['TipoDeComprobante'].code + ' ' + i['MetodoPago'].code + ' ' + (i['FormaPago'].code if i['FormaPago'].code != '99' else '  ')
     return i['TipoDeComprobante'].code + '       '
 
 
-def ajustes_directory(dp: DatePeriod):
-    return os.path.join(archivos_folder(dp), 'ajustes')
-
-
 def preview_cfdis(cfdis):
     outfile = os.path.join(TEMP_DIRECTORY, "factura.html")
     Representable.html_write_all(
         objs=cfdis,
         target=outfile,
     )
     open_file(
```

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-4.0.8/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/layout.py` & `satdigitalinvoice-4.0.8/satdigitalinvoice/layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from datetime import date, datetime, timedelta
 from enum import StrEnum
 
 import PySimpleGUI as sg
+from satcfdi import Code
+from satcfdi.catalogs import select_all
 from satcfdi.pacs.sat import TipoDescargaMasivaTerceros
-# noinspection PyUnresolvedReferences
-from satcfdi.transform.catalog import CATALOGS
-from satdigitalinvoice.gui_functions import mf_pago_fmt, CALENDAR_FECHA_FMT
 
-from .log_tools import *
+from satdigitalinvoice.gui_functions import mf_pago_fmt, CALENDAR_FECHA_FMT
 
-FORMA_PAGO = CATALOGS['{http://www.sat.gob.mx/sitio_internet/cfd/catalogos}c_FormaPago']
+FORMA_PAGO = select_all('C756_c_FormaPago')
 TEXT_PADDING = ((5, 0), 3)
 
 # 24 x 24
 FOLDER_ICON = "iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAACXBIWXMAAAsTAAALEwEAmpwYAAAAqElEQVR4nO3UsQnCYBRF4U/EAcRJtHUJcQddwQlsxcpVLF0hOoY2FlaC+SUQQWI0PmwscuF0j3PhFZc2" \
               "/5QR9siRnjhhid6vBVlFXGWHwS8Ft4aCHLPydozFGybo1BV8kl8wLe/muDbcryIFBwzRxbpB/OAcfV8f2y/lD17y7qcbHIPy2oKoILUFqX1RdCpSgMIVHrsUoHDVznVWM9cpQF46imlp8ye5AyE7C1To4" \
               "/HLAAAAAElFTkSuQmCC"
 
@@ -330,14 +329,42 @@
                                         r["efectivo_periodo_desc"]
                                     ]
                                 )
                             ]],
                         key='ajustes_tab'
                     ),
                     sg.Tab(
+                        'Depositos'.center(13),
+                        [
+                            [
+                                sg.Button(image_data=EDIT_ICON, key="editar_depositos", border_width=0, button_color=BUTTON_COLOR),
+                                sg.Text("Periodo:", pad=TEXT_PADDING),
+                                sg.Input(date.today().strftime(PERIODO_FMT), size=(11, 1), key="depositos_periodo"),
+                                sg.Text("", pad=TEXT_PADDING, key="preparar_depositos_text", font=LARGE_FONT),
+                            ],
+                            [
+                                MyTable(
+                                    key="depositos_table",
+                                    headings=[
+                                        "#",
+                                        "Receptor Razon Social",
+                                        "Recep. Rfc",
+                                        "Actual",
+                                    ],
+                                    row_fn=lambda i, r: [
+                                        i,
+                                        r["receptor"]["RazonSocial"],
+                                        r["receptor"]["Rfc"],
+                                        r["valor_unitario"],
+                                    ]
+                                )
+                            ]],
+                        key='depositos_tab'
+                    ),
+                    sg.Tab(
                         'Clientes '.center(13),
                         [
                             [
                                 sg.Button(image_data=EDIT_ICON, key="editar_clientes", border_width=0, button_color=BUTTON_COLOR),
                                 sg.Push(),
                                 sg.Button("Exportar", key="exportar_clientes", border_width=0),
                             ],
@@ -352,15 +379,15 @@
                                         "CP",
                                         "IdCIF"
                                     ],
                                     row_fn=lambda i, r: [
                                         i,
                                         r["RazonSocial"],
                                         r["Rfc"],
-                                        r["RegimenFiscal"].code,
+                                        r["RegimenFiscal"],
                                         r["CodigoPostal"],
                                         r["IdCIF"]
                                     ]
                                 )
                             ]],
                         key='clientes_tab',
                     ),
@@ -378,15 +405,15 @@
                                     sg.Input((datetime.now() - timedelta(days=40)).strftime(CALENDAR_FECHA_FMT), size=(12, 1), key="fecha_inicial"),
 
                                     sg.CalendarButton("Final:", format=CALENDAR_FECHA_FMT, title="Final", no_titlebar=False, target="fecha_final", pad=TEXT_PADDING,
                                                       border_width=0),
                                     sg.Input(datetime.now().strftime(CALENDAR_FECHA_FMT), size=(12, 1), key="fecha_final"),
 
                                     sg.Text("Tipo:", pad=TEXT_PADDING),
-                                    sg.Combo([TipoDescargaMasivaTerceros.CFDI, TipoDescargaMasivaTerceros.Metadata], default_value=TipoDescargaMasivaTerceros.CFDI,
+                                    sg.Combo([TipoDescargaMasivaTerceros.CFDI, TipoDescargaMasivaTerceros.METADATA], default_value=TipoDescargaMasivaTerceros.CFDI,
                                              key="tipo_solicitud", size=(10, 1)),
 
                                     sg.Button("Nueva Solicitud", key="nueva_solicitud", border_width=0),
                                 ]],
                                     expand_x=True
                                 )
                             ],
@@ -430,15 +457,15 @@
                                 sg.Button(image_data=EXCEL_ICON, key="ver_excel", border_width=0, button_color=BUTTON_COLOR),
                                 sg.Button(image_data=FOLDER_ICON, key="ver_carpeta", border_width=0, button_color=BUTTON_COLOR),
                             ]])
                         ]],
                         key='contabilidad_tab',
                     ),
                     sg.Tab(
-                        'Errores'.center(13),
+                        'Consola'.center(13),
                         [
                             [
                                 sg.Push(),
                                 sg.Button(image_data=ABOUT_ICON, key="about", border_width=0, button_color=BUTTON_COLOR),
                             ],
                             [sg.Multiline(
                                 expand_x=True,
```

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/localdb.py` & `satdigitalinvoice-4.0.8/satdigitalinvoice/localdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from enum import Enum
 from uuid import UUID
 
 import diskcache
 from satcfdi import Code
 from satcfdi.accounting import SatCFDI
 from satcfdi.accounting.models import EstadoComprobante
+from satcfdi.create.cfd.catalogos import MetodoPago, TipoDeComprobante
 from satcfdi.pacs import sat
 
-from . import PPD
 from .utils import estado_to_estatus
 
 LIQUIDATED = 0
 NOTIFIED = 2
 STATUS_SAT = 3
 FOLIO = 5
 SERIE = 6
@@ -151,14 +151,16 @@
             return "✔"
         if self.name == "PENDING":
             return ""
         if self.name == "CANCELLED":
             return "❌"
 
 
+
+
 class LocalDBSatCFDI(LocalDB):
     def __init__(self, base_path, enviar_a_partir, pagar_a_partir):
         super().__init__(base_path)
         self.enviar_a_partir = enviar_a_partir
         self.pagar_a_partir = pagar_a_partir
 
     def notified(self, cfdi: SatCFDI):
@@ -196,23 +198,23 @@
             else:
                 raise ValueError("Error al actualizar estado de %s: %s", cfdi.uuid, res)
             return res
         else:
             return super().status(cfdi.uuid)
 
     def liquidated_state(self, cfdi: SatCFDI):
-        if cfdi.estatus == EstadoComprobante.Cancelado:
+        if cfdi.estatus == EstadoComprobante.CANCELADO:
             return StatusState.CANCELLED
 
-        if cfdi["TipoDeComprobante"] != "I":
+        if cfdi["TipoDeComprobante"] != TipoDeComprobante.INGRESO:
             return StatusState.NONE
 
         mpago = cfdi["MetodoPago"]
-        if cfdi['Total'] == 0 or (mpago == PPD and cfdi.saldo_pendiente == 0):
+        if cfdi['Total'] == 0 or (mpago == MetodoPago.PAGO_EN_PARCIALIDADES_O_DIFERIDO and cfdi.saldo_pendiente == 0):
             return StatusState.PAID
 
         if self.liquidated(cfdi):
-            if mpago == PPD:
+            if mpago == MetodoPago.PAGO_EN_PARCIALIDADES_O_DIFERIDO:
                 return StatusState.IGNORED
             return StatusState.PAID
 
         return StatusState.PENDING
```

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-4.0.8/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-4.0.8/satdigitalinvoice/mycfdi.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class MyCFDI(SatCFDI):
     local_db = None
     base_dir = None  # type: str
 
     @SatCFDI.estatus.getter
     def estatus(self) -> EstadoComprobante:
-        return self.consulta_estado().get('Estatus', EstadoComprobante.Vigente)
+        return self.consulta_estado().get('Estatus', EstadoComprobante.VIGENTE)
 
     def consulta_estado(self):
         return self.local_db.status_sat(self)
 
     @SatCFDI.fecha_cancelacion.getter
     def fecha_cancelacion(self) -> datetime | None:
         return self.consulta_estado().get('FechaCancelacion')
```

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-4.0.8/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice/utils.py` & `satdigitalinvoice-4.0.8/satdigitalinvoice/utils.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.7
+Version: 4.0.8
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.7/setup.py` & `satdigitalinvoice-4.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         package: [
             "markdown_styles/*",
             "schemas/*",
             'images/*',
         ],
     },
     install_requires=[
-        'satcfdi==4.0.19',
+        'satcfdi==4.0.27',
         'diskcache',
         'num2words',
         'PyYAML',
         'babel',
         'markdown2',
         'PySimpleGUI',
         'XlsxWriter',
```

### Comparing `satdigitalinvoice-4.0.7/tests/test_crear_facturas.py` & `satdigitalinvoice-4.0.8/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.7/tests/test_localdb.py` & `satdigitalinvoice-4.0.8/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.7/tests/test_main.py` & `satdigitalinvoice-4.0.8/tests/test_main.py`

 * *Files identical despite different names*

