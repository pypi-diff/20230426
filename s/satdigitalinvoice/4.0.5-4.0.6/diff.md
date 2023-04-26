# Comparing `tmp/satdigitalinvoice-4.0.5.tar.gz` & `tmp/satdigitalinvoice-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-4.0.5.tar", last modified: Tue Apr 25 07:31:38 2023, max compression
+gzip compressed data, was "satdigitalinvoice-4.0.6.tar", last modified: Wed Apr 26 06:52:39 2023, max compression
```

## Comparing `satdigitalinvoice-4.0.5.tar` & `satdigitalinvoice-4.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.558736 satdigitalinvoice-4.0.5/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    38196 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-04-25 07:31:25.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.558736 satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 07:31:38.000000 satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 07:31:38.000000 satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:31:38.000000 satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 07:31:38.000000 satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 07:31:38.000000 satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:31:38.562736 satdigitalinvoice-4.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-25 07:31:26.000000 satdigitalinvoice-4.0.5/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.731170 satdigitalinvoice-4.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-26 06:52:39.731170 satdigitalinvoice-4.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.727170 satdigitalinvoice-4.0.6/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38644 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.727170 satdigitalinvoice-4.0.6/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.727170 satdigitalinvoice-4.0.6/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.727170 satdigitalinvoice-4.0.6/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.727170 satdigitalinvoice-4.0.6/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.727170 satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-26 06:52:39.000000 satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-26 06:52:39.000000 satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:52:39.000000 satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-26 06:52:39.000000 satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 06:52:39.000000 satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:52:39.731170 satdigitalinvoice-4.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.731170 satdigitalinvoice-4.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/tests/test_main.py
```

### Comparing `satdigitalinvoice-4.0.5/PKG-INFO` & `satdigitalinvoice-4.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.5
+Version: 4.0.6
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/__init__.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/__init__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/__version__.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/environments.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/facturacion.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 
         self.all_invoices = None
         self.local_db = LocalDBSatCFDI(
             base_path=DATA_DIRECTORY,
             enviar_a_partir=config['enviar_a_partir'],
             pagar_a_partir=config['pagar_a_partir']
         )
-        self.facturas_con_serie_folio = config.get('facturas_con_serie_folio', ('I', 'P'))
 
         MyCFDI.local_db = self.local_db
         MyCFDI.base_dir = ARCHIVOS_DIRECTORY
 
         self.window = sg.Window(
             f"Facturación Mensual CFDI 4.0 {self.csd_signer.rfc}",
             make_layout(bool(self.fiel_signer), self.local_db),
@@ -84,29 +83,28 @@
             resizable=True,
             font=("Courier New", 10, "bold"),
             ttk_theme="default",
             margins=(0, 0),
             # use_custom_titlebar=True,
             titlebar_font=("Courier New", 11, "bold"),
             finalize=True,
+            scaling=config.get('scaling', 1.0),
         )
 
         self.action_button_manager = ActionButtonManager(
             button=self.window["crear_facturas"],
             preview=self.window["ver_preview"],
         )
         self.console = self.window["console"]
-
-        self.set_serie()
-        self.set_folio()
+        self.set_inputs()
 
         self.window.bind("<FocusIn>", "_focus_in")
         self.window.bind("<FocusOut>", "_focus_out")
 
-        for t in ('facturas_periodo', 'emitidas_search', 'ajustes_periodo', 'serie', 'folio'):
+        for t in ('facturas_periodo', 'emitidas_search', 'ajustes_periodo', 'serie', 'folio', 'serie_pago'):
             self.window[t].bind("<Return>", "_enter")
             self.window[t].bind("<FocusOut>", "_enter", propagate=False)
 
         modifier_key = "Command" if OS.get_os() == OS.MACOS else "Control"
 
         for t in ('facturas_table', 'clientes_table', 'emitidas_table', 'correos_table', 'ajustes_table', 'solicitudes_table'):
             self.window[t].bind(f'<{modifier_key}-a>', '+select_all')
@@ -143,15 +141,15 @@
         complement_invoices(self.all_invoices, invoice)
 
     def generate_invoice(self, invoice):
         ref_id = random_string()
 
         # Add Serie and Folio and signature
         folio = None
-        if invoice['TipoDeComprobante'] in self.facturas_con_serie_folio:
+        if 'Serie' not in invoice:
             invoice['Serie'] = self.local_db.serie()
             folio = self.local_db.folio()
             invoice['Folio'] = str(folio)
 
         cfdi40.Comprobante.sign(invoice, self.csd_signer)
 
         attempts = 3
@@ -181,27 +179,39 @@
                 self.set_folio(folio + 1)
             cfdi = MyCFDI.move_to_folder(res.xml, pdf_data=res.pdf)
             self.add_created_invoice(cfdi)
             return cfdi
 
     def set_serie(self, serie: str = None):
         if serie:
-            self.local_db.serie_set(serie)
+            self.local_db.serie_set(serie.strip())
+        self.set_inputs()
 
-        serie = serie or self.local_db.serie()
-        self.window['serie'].update(serie)
-        self.window['serie_folio'].update(f"{serie}{self.local_db.folio()}")
+    def set_serie_pago(self, serie: str = None):
+        self.local_db.serie_pago_set(serie.strip())
+        self.set_inputs()
 
     def set_folio(self, folio: int = None):
         if folio:
             self.local_db.folio_set(folio)
+        self.set_inputs()
 
-        folio = folio or self.local_db.folio()
+    def set_inputs(self):
+        folio = self.local_db.folio()
+        serie = self.local_db.serie()
+        serie_pago = self.local_db.serie_pago()
+
+        self.window['serie'].update(serie)
         self.window['folio'].update(folio)
-        self.window['serie_folio'].update(f"{self.local_db.serie()}{folio}")
+        self.window['serie_folio'].update(f"{serie}{folio}")
+
+        self.window['serie_pago'].update(serie_pago)
+        self.window['folio_pago'].update(
+            "Se usara el mismo folio de la factura que se paga" if serie_pago else "Se usar serie y folio de proxima factura"
+        )
 
     def nueva_solicitud(self, values):
         tipo_recuperar = values["tipo_recuperar"]
 
         args = {
             'fecha_inicial': datetime.strptime(values["fecha_inicial"], CALENDAR_FECHA_FMT),
             'fecha_final': datetime.strptime(values["fecha_final"], CALENDAR_FECHA_FMT),
@@ -424,15 +434,15 @@
             and i["TipoDeComprobante"] == "I" \
             and i["MetodoPago"] == PPD \
             and i.saldo_pendiente > 0
 
         self.window["ppd_action_items"].update(visible=is_ppd_active)
         self.window["importe_pago"].update(i.saldo_pendiente if is_ppd_active else '')
         if is_ppd_active:
-            self.action_button_manager.set_items("pago", [None])
+            self.action_button_manager.set_items("pago", [i])
         else:
             self.action_button_manager.clear()
 
     def header(self, name):
         self.window['console_tab'].select()
         self.console.update(header_line(name))
         self._read()
@@ -488,25 +498,26 @@
                     ):
                         yield i
 
         self.window['emitidas_table'].update(
             values=list(fact_iter()),
         )
 
-    def crear_pago(self, values):
+    def crear_pago(self, values, facturas_pagar):
         fecha_pago = parse_fecha_pago(values["fecha_pago"])
         importe_pago = parse_importe_pago(values["importe_pago"])
         self.window["importe_pago"].update(importe_pago)
 
         # noinspection PyUnresolvedReferences
         cfdi = pago_factura(
-            factura_pagar=self.window["emitidas_table"].selected_items()[0],
+            factura_pagar=facturas_pagar[0],
             fecha_pago=fecha_pago,
             forma_pago=values["forma_pago"],
             importe_pago=importe_pago,
+            serie_pago=self.local_db.serie_pago(),
         )
         return [cfdi]
 
     def error_message(self, ex):
         sg.Popup(
             ex,
             no_titlebar=True,
@@ -652,14 +663,17 @@
 
                     case "folio_enter":
                         self.set_folio(to_int(values["folio"]))
 
                     case "serie_enter":
                         self.set_serie(values["serie"])
 
+                    case "serie_pago_enter":
+                        self.set_serie_pago(values["serie_pago"])
+
                     case "about":
                         clients = ClientsManager()
                         self.initial_screen(clients[self.csd_signer.rfc])
 
                     case "nueva_solicitud":
                         self.nueva_solicitud(values)
                         self.main_tab_group(values)
@@ -763,15 +777,15 @@
 
                     case "crear_facturas" | "ver_preview":
                         action_text = self.action_button_manager.text()
                         action_name = self.action_button_manager.name
                         action_items = self.action_button_manager.items
 
                         if action_name == "pago":
-                            action_items = self.crear_pago(values)
+                            action_items = self.crear_pago(values, action_items)
 
                         if event == "ver_preview":
                             if action_name in ("facturas", "pago"):
                                 preview_cfdis(action_items)
 
                         elif event == "crear_facturas":
                             res = sg.popup(
```

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/gui_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,17 +179,19 @@
 def parse_importe_pago(importe_pago: str):
     try:
         return round(Decimal(importe_pago), 2)
     except InvalidOperation:
         raise ValueError("Importe de Pago es invalido")
 
 
-def pago_factura(factura_pagar, fecha_pago: datetime, forma_pago: str, importe_pago: Decimal = None):
+def pago_factura(factura_pagar, fecha_pago: datetime, forma_pago: str, importe_pago: Decimal = None, serie_pago=None):
     c = factura_pagar
     invoice = Comprobante.pago_comprobantes(
+        serie=serie_pago or None,
+        folio=c.get('Folio') if serie_pago else None,
         comprobantes=[
             PagoComprobante(
                 comprobante=c,
                 num_parcialidad=c.ultima_num_parcialidad + 1,
                 imp_saldo_ant=c.saldo_pendiente,
                 imp_pagado=importe_pago
             )
```

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-4.0.6/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/layout.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -454,34 +454,51 @@
                     sg.Tab(
                         'Configuracion'.center(13),
                         [
                             [
                                 sg.Column([[
                                     sg.Button(image_data=EDIT_ICON, key="editar_configurar", border_width=0, button_color=BUTTON_COLOR),
                                     sg.Button(image_data=CONFIG_ICON, key="ver_config", border_width=0, button_color=BUTTON_COLOR),
-                                    sg.Text("Proxima Factura:", pad=TEXT_PADDING),
+                                ]])
+                            ],
+                            [
+                                sg.Column([[
+                                    sg.Text(" Proxima Factura:", pad=TEXT_PADDING),
                                     sg.Text("Serie:", pad=TEXT_PADDING),
                                     sg.Input("", key="serie", size=(8, 1)),
                                     sg.Text("Folio:", pad=TEXT_PADDING),
                                     sg.Input("", key="folio", size=(8, 1)),
                                 ]],
                                     expand_x=True
                                 )
                             ],
                             [
                                 sg.Column([[
+                                    sg.Text("Complemento Pago:", pad=TEXT_PADDING),
+                                    sg.Text("Serie:", pad=TEXT_PADDING),
+                                    sg.Input("", key="serie_pago", size=(8, 1)),
+                                    sg.Text("", key="folio_pago", pad=TEXT_PADDING),
+                                ]],
+                                    expand_x=True
+                                )
+                            ],
+                            [
+                                sg.Column([[]], size=(40, 40))
+                            ],
+                            [
+                                sg.Column([[
                                     sg.Button("Organizar Facturas", key="organizar_facturas", border_width=0),
                                 ]],
                                     expand_x=True
                                 )
                             ],
                             [
                                 sg.Column([[
-                                    sg.Button("Exportar Metadata", key="exportar_metadata", border_width=0),
-                                    sg.Button("Importar Metadata", key="importar_metadata", border_width=0),
+                                    sg.Button("Exportar Metadata ", key="exportar_metadata", border_width=0),
+                                    sg.Button("Importar Metadata ", key="importar_metadata", border_width=0),
                                 ]],
                                     expand_x=True
                                 )
                             ]
                         ],
                         key='configuracion_tab',
                     ),
```

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/localdb.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/localdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .utils import estado_to_estatus
 
 LIQUIDATED = 0
 NOTIFIED = 2
 STATUS_SAT = 3
 FOLIO = 5
 SERIE = 6
+SERIE_PAGO = 7
 SOLICITUDES = 'solicitudes'
 
 sat_manager = sat.SAT()
 
 logger = logging.getLogger(__name__)
 
 
@@ -39,14 +40,20 @@
 
     def serie(self) -> str:
         return self.get(SERIE, 'A')
 
     def serie_set(self, value: str):
         self[SERIE] = value
 
+    def serie_pago(self) -> str:
+        return self.get(SERIE_PAGO, 'P')
+
+    def serie_pago_set(self, value: str):
+        self[SERIE_PAGO] = value
+
     def liquidated(self, uuid: UUID):
         return self.get((LIQUIDATED, uuid))
 
     def liquidated_set(self, uuid: UUID, value: bool):
         self[(LIQUIDATED, uuid)] = value
 
     def notified(self, uuid: UUID):
```

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-4.0.6/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-4.0.6/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice/utils.py` & `satdigitalinvoice-4.0.6/satdigitalinvoice/utils.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.5
+Version: 4.0.6
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.5/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/setup.py` & `satdigitalinvoice-4.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/tests/test_crear_facturas.py` & `satdigitalinvoice-4.0.6/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/tests/test_localdb.py` & `satdigitalinvoice-4.0.6/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.5/tests/test_main.py` & `satdigitalinvoice-4.0.6/tests/test_main.py`

 * *Files identical despite different names*

