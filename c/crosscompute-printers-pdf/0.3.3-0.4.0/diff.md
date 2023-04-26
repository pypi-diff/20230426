# Comparing `tmp/crosscompute-printers-pdf-0.3.3.tar.gz` & `tmp/crosscompute-printers-pdf-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosscompute-printers-pdf-0.3.3.tar", last modified: Fri Oct 28 19:06:12 2022, max compression
+gzip compressed data, was "crosscompute-printers-pdf-0.4.0.tar", last modified: Tue Apr 25 23:01:19 2023, max compression
```

## Comparing `crosscompute-printers-pdf-0.3.3.tar` & `crosscompute-printers-pdf-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2022-10-28 19:06:12.923091 crosscompute-printers-pdf-0.3.3/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)     1057 2022-03-14 16:39:47.000000 crosscompute-printers-pdf-0.3.3/LICENSE.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1956 2022-10-28 19:06:12.923091 crosscompute-printers-pdf-0.3.3/PKG-INFO
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      946 2022-06-28 19:54:25.000000 crosscompute-printers-pdf-0.3.3/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2022-10-28 19:06:12.922091 crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      849 2022-03-21 19:14:30.000000 crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf/__init__.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2022-10-28 19:06:12.923091 crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf/scripts/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4518 2022-10-28 14:55:00.000000 crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf/scripts/print-pdfs.js
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2022-10-28 19:06:12.922091 crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf.egg-info/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)     1956 2022-10-28 19:06:12.000000 crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf.egg-info/PKG-INFO
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      465 2022-10-28 19:06:12.000000 crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf.egg-info/SOURCES.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        1 2022-10-28 19:06:12.000000 crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf.egg-info/dependency_links.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       67 2022-10-28 19:06:12.000000 crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf.egg-info/entry_points.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       41 2022-10-28 19:06:12.000000 crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf.egg-info/requires.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       26 2022-10-28 19:06:12.000000 crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf.egg-info/top_level.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        1 2022-03-14 16:41:31.000000 crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1333 2022-10-28 19:06:12.923091 crosscompute-printers-pdf-0.3.3/setup.cfg
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       39 2022-03-14 16:39:47.000000 crosscompute-printers-pdf-0.3.3/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 23:01:19.337780 crosscompute-printers-pdf-0.4.0/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2022-08-29 00:24:28.000000 crosscompute-printers-pdf-0.4.0/LICENSE.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1931 2023-04-25 23:01:19.337780 crosscompute-printers-pdf-0.4.0/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      921 2023-04-07 11:14:54.000000 crosscompute-printers-pdf-0.4.0/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 23:01:19.335780 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      848 2023-04-05 16:25:37.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf/__init__.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 23:01:19.336780 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf/scripts/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4460 2023-04-25 16:46:40.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf/scripts/print.js
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 23:01:19.336780 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1931 2023-04-25 23:01:19.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      460 2023-04-25 23:01:19.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-04-25 23:01:19.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       67 2023-04-25 23:01:19.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/entry_points.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       42 2023-04-25 23:01:19.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       26 2023-04-25 23:01:19.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-04-01 21:07:32.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1334 2023-04-25 23:01:19.337780 crosscompute-printers-pdf-0.4.0/setup.cfg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2022-08-29 00:24:28.000000 crosscompute-printers-pdf-0.4.0/setup.py
```

### Comparing `crosscompute-printers-pdf-0.3.3/LICENSE.md` & `crosscompute-printers-pdf-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crosscompute-printers-pdf-0.3.3/PKG-INFO` & `crosscompute-printers-pdf-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute-printers-pdf
-Version: 0.3.3
+Version: 0.4.0
 Summary: Print your automations in PDF format.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute-printers-pdf/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-printers-pdf
@@ -42,28 +42,30 @@
 ```
 
 ## Usage
 
 1. Add prints to your configuration file.
 
 ```yaml
-prints:
-  - format: pdf
-    configuration:
-      header-footer:
+print:
+  variables:
+    - id: report
+      view: pdf
+      path: report.pdf
+      configuration:
+        header-footer:
           font-family: sans-serif
           font-size: 8pt
           color: '#808080'
           padding: 0.1in 0.25in
           skip-first: true
-      page-number:
+        page-number:
           location: footer
           alignment: right
-    folder: ~/Documents/attachments/randomize-histograms-{timestamp}
-    name: me{mean}-va{variance}-vc{value_count}-bc{bin_count}.pdf
+        name: 'm{mean}-v{variance}-{timestamp}.pdf'
 ```
 
 2. Run batch print.
 
 ```bash
 crosscompute --print
 ```
```

### Comparing `crosscompute-printers-pdf-0.3.3/README.md` & `crosscompute-printers-pdf-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,28 +17,30 @@
 ```
 
 ## Usage
 
 1. Add prints to your configuration file.
 
 ```yaml
-prints:
-  - format: pdf
-    configuration:
-      header-footer:
+print:
+  variables:
+    - id: report
+      view: pdf
+      path: report.pdf
+      configuration:
+        header-footer:
           font-family: sans-serif
           font-size: 8pt
           color: '#808080'
           padding: 0.1in 0.25in
           skip-first: true
-      page-number:
+        page-number:
           location: footer
           alignment: right
-    folder: ~/Documents/attachments/randomize-histograms-{timestamp}
-    name: me{mean}-va{variance}-vc{value_count}-bc{bin_count}.pdf
+        name: 'm{mean}-v{variance}-{timestamp}.pdf'
 ```
 
 2. Run batch print.
 
 ```bash
 crosscompute --print
 ```
```

### Comparing `crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf/__init__.py` & `crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import json
 import subprocess
+from pathlib import Path
+
 from crosscompute.routines.printer import BatchPrinter
 from invisibleroads_macros_disk import TemporaryStorage
-from pathlib import Path
 
 
 class PdfPrinter(BatchPrinter):
 
-    def render(self, batch_dictionaries, print_definition):
+    view_name = 'pdf'
+
+    def render(self, batch_dictionaries, print_configurations):
         with TemporaryStorage() as storage:
-            path = Path(storage.folder) / 'printer-configuration.json'
+            path = Path(storage.folder) / 'c.json'
             with open(path, 'wt') as f:
                 json.dump({
                     'uri': self.server_uri,
-                    'batch_dictionaries': batch_dictionaries,
-                    'print_definition': print_definition,
+                    'dictionaries': batch_dictionaries,
+                    'configurations': print_configurations,
                 }, f)
             subprocess.run([
                 'node',
                 '--experimental-fetch',
-                PACKAGE_FOLDER / 'scripts' / 'print-pdfs.js',
+                PACKAGE_FOLDER / 'scripts' / 'print.js',
                 path])
 
 
 PACKAGE_FOLDER = Path(__file__).parent
```

### Comparing `crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf/scripts/print-pdfs.js` & `crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf/scripts/print.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -13,27 +13,29 @@
 const d = JSON.parse(fs.readFileSync(dataPath));
 
 let browser, page;
 
 const go = async (
     serverUri,
     batchDictionaries,
-    printDefinition
+    printConfigurations
 ) => {
     await initialize();
     while (batchDictionaries.length) {
         const batchDictionary = batchDictionaries.pop();
         const sourceUri = serverUri + batchDictionary.uri;
         if (isReady(sourceUri)) {
             const targetPath = batchDictionary.path;
             const targetFolder = path.dirname(targetPath);
             fs.mkdirSync(targetFolder, {
                 recursive: true
             });
-            await print(sourceUri + '/o?_print', targetPath, printDefinition);
+            for (const printConfiguration of printConfigurations) {
+                await print(sourceUri + '/o?_print', targetPath, printConfiguration);
+            }
         } else {
             batchDictionaries.push(batchDictionary);
         }
     }
     await browser.close();
 }
 const initialize = async () => {
@@ -42,17 +44,16 @@
 }
 const isReady = async (batchUri) => {
     const response = await fetch(batchUri + '/d/return_code');
     const responseText = await response.text();
     const returnCode = parseInt(responseText);
     return returnCode == 0;
 };
-const print = async (sourceUri, targetPath, printDefinition) => {
+const print = async (sourceUri, targetPath, printConfiguration) => {
     console.log(`printing ${sourceUri} to ${targetPath}`);
-    const printConfiguration = printDefinition['configuration'];
     const headerFooterOptions = printConfiguration['header-footer'];
     const skipFirst = headerFooterOptions?.['skip-first'];
     const pageNumberOptions = printConfiguration['page-number'];
     const pageNumberLocation = pageNumberOptions?.['location'];
     const containerHtml = getContainerHtml(printConfiguration);
     let displayHeaderFooter = false;
     let headerTemplate = '<span />',
@@ -118,30 +119,29 @@
         const bodyPath = temporaryFolder + '/body.pdf';
         await page.pdf({
             path: headPath,
             preferCSSPageSize: true,
             displayHeaderFooter: false,
             pageRanges: '1',
         });
-        await page.pdf({
-            ...pdfOptions,
-            path: bodyPath,
-            pageRanges: '2-'
-        });
         const pdfMerger = new PDFMerger();
-        pdfMerger.add(headPath);
-        pdfMerger.add(bodyPath);
+        await pdfMerger.add(headPath);
+        try {
+            await page.pdf({
+                ...pdfOptions,
+                path: bodyPath,
+                pageRanges: '2-'
+            });
+            await pdfMerger.add(bodyPath);
+        } catch {}
         await pdfMerger.save(pdfOptions['path']);
         fs.rmSync(temporaryFolder, {
             recursive: true
         });
     } else {
         await page.pdf({
             ...pdfOptions
         });
     }
 }
 
-const serverUri = d.uri;
-const batchDictionaries = d.batch_dictionaries;
-const printDefinition = d.print_definition;
-go(serverUri, batchDictionaries, printDefinition);
+go(d.uri, d.dictionaries, d.configurations);
```

### Comparing `crosscompute-printers-pdf-0.3.3/crosscompute_printers_pdf.egg-info/PKG-INFO` & `crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute-printers-pdf
-Version: 0.3.3
+Version: 0.4.0
 Summary: Print your automations in PDF format.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute-printers-pdf/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-printers-pdf
@@ -42,28 +42,30 @@
 ```
 
 ## Usage
 
 1. Add prints to your configuration file.
 
 ```yaml
-prints:
-  - format: pdf
-    configuration:
-      header-footer:
+print:
+  variables:
+    - id: report
+      view: pdf
+      path: report.pdf
+      configuration:
+        header-footer:
           font-family: sans-serif
           font-size: 8pt
           color: '#808080'
           padding: 0.1in 0.25in
           skip-first: true
-      page-number:
+        page-number:
           location: footer
           alignment: right
-    folder: ~/Documents/attachments/randomize-histograms-{timestamp}
-    name: me{mean}-va{variance}-vc{value_count}-bc{bin_count}.pdf
+        name: 'm{mean}-v{variance}-{timestamp}.pdf'
 ```
 
 2. Run batch print.
 
 ```bash
 crosscompute --print
 ```
```

### Comparing `crosscompute-printers-pdf-0.3.3/setup.cfg` & `crosscompute-printers-pdf-0.4.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosscompute-printers-pdf
-version = 0.3.3
+version = 0.4.0
 description = Print your automations in PDF format.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://crosscompute.com
 author = CrossCompute Inc.
 author_email = support@crosscompute.com
 license = MIT
@@ -24,15 +24,15 @@
 	Documentation = https://github.com/crosscompute/crosscompute-printers-pdf
 	Source Code = https://github.com/crosscompute/crosscompute-printers-pdf
 
 [options]
 packages = find:
 python_requires = >=3.9
 install_requires = 
-	crosscompute>=0.9.2.6
+	crosscompute>=0.9.2.10
 zip_safe = True
 
 [options.package_data]
 crosscompute_printers_pdf = 
 	scripts/*.js
 
 [options.entry_points]
```

