# Comparing `tmp/juno-ai-0.0.2.tar.gz` & `tmp/juno-ai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/juno-ai-0.0.2.tar", last modified: Sun Apr 23 01:53:04 2023, max compression
+gzip compressed data, was "juno-ai-0.0.3.tar", last modified: Tue Apr 25 20:36:07 2023, max compression
```

## Comparing `juno-ai-0.0.2.tar` & `juno-ai-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-23 01:53:04.000000 juno-ai-0.0.2/
--rw-r--r--   0 alexirobbins   (501) staff       (20)      712 2023-04-23 01:53:04.000000 juno-ai-0.0.2/PKG-INFO
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-23 01:53:04.000000 juno-ai-0.0.2/juno_ai.egg-info/
--rw-r--r--   0 alexirobbins   (501) staff       (20)      712 2023-04-23 01:53:03.000000 juno-ai-0.0.2/juno_ai.egg-info/PKG-INFO
--rw-r--r--   0 alexirobbins   (501) staff       (20)      345 2023-04-23 01:53:03.000000 juno-ai-0.0.2/juno_ai.egg-info/SOURCES.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)       34 2023-04-23 01:53:03.000000 juno-ai-0.0.2/juno_ai.egg-info/requires.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)        5 2023-04-23 01:53:03.000000 juno-ai-0.0.2/juno_ai.egg-info/top_level.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)        1 2023-04-23 01:53:03.000000 juno-ai-0.0.2/juno_ai.egg-info/dependency_links.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1219 2023-04-23 01:52:53.000000 juno-ai-0.0.2/setup.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)       38 2023-04-23 01:53:04.000000 juno-ai-0.0.2/setup.cfg
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-23 01:53:04.000000 juno-ai-0.0.2/juno/
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1359 2023-04-23 00:04:48.000000 juno-ai-0.0.2/juno/magic.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     2381 2023-04-16 21:49:54.000000 juno-ai-0.0.2/juno/serialize_context.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1253 2023-04-16 22:35:57.000000 juno-ai-0.0.2/juno/client_setup.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)      473 2023-04-23 01:52:59.000000 juno-ai-0.0.2/juno/version.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)       58 2023-04-09 05:43:26.000000 juno-ai-0.0.2/juno/__init__.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)      873 2023-03-31 21:04:15.000000 juno-ai-0.0.2/juno/output_parser.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)    16128 2023-04-23 01:07:57.000000 juno-ai-0.0.2/juno/event_javascript.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1229 2023-04-22 23:55:05.000000 juno-ai-0.0.2/juno/juno.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     8507 2023-04-23 00:13:02.000000 juno-ai-0.0.2/juno/prompting_javascript.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-25 20:36:07.794567 juno-ai-0.0.3/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-04-25 20:36:07.794196 juno-ai-0.0.3/PKG-INFO
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1940 2023-04-25 20:17:30.000000 juno-ai-0.0.3/README.md
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-25 20:36:07.791521 juno-ai-0.0.3/juno/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       58 2023-04-09 05:43:26.000000 juno-ai-0.0.3/juno/__init__.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1253 2023-04-16 22:35:57.000000 juno-ai-0.0.3/juno/client_setup.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)    16283 2023-04-25 20:15:36.000000 juno-ai-0.0.3/juno/event_javascript.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1387 2023-04-25 20:00:00.000000 juno-ai-0.0.3/juno/juno.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1423 2023-04-25 20:00:24.000000 juno-ai-0.0.3/juno/magic.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      873 2023-03-31 21:04:15.000000 juno-ai-0.0.3/juno/output_parser.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)    10061 2023-04-25 20:15:59.000000 juno-ai-0.0.3/juno/prompting_javascript.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     2381 2023-04-16 21:49:54.000000 juno-ai-0.0.3/juno/serialize_context.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      473 2023-04-25 20:16:52.000000 juno-ai-0.0.3/juno/version.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-25 20:36:07.793786 juno-ai-0.0.3/juno_ai.egg-info/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-04-25 20:36:07.000000 juno-ai-0.0.3/juno_ai.egg-info/PKG-INFO
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      355 2023-04-25 20:36:07.000000 juno-ai-0.0.3/juno_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)        1 2023-04-25 20:36:07.000000 juno-ai-0.0.3/juno_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       34 2023-04-25 20:36:07.000000 juno-ai-0.0.3/juno_ai.egg-info/requires.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)        5 2023-04-25 20:36:07.000000 juno-ai-0.0.3/juno_ai.egg-info/top_level.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       38 2023-04-25 20:36:07.794635 juno-ai-0.0.3/setup.cfg
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1219 2023-04-25 20:16:45.000000 juno-ai-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `juno-ai-0.0.2/PKG-INFO` & `juno-ai-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: juno-ai
-Version: 0.0.2
-Summary: UNKNOWN
+Version: 0.0.3
 Home-page: https://github.com/alexi/juno
 Author: juno
 Author-email: hellojunoai@gmail.com
-License: UNKNOWN
-Description: Juno AI Assistant for Jupyter Notebook
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+
+Juno AI Assistant for Jupyter Notebook
```

### Comparing `juno-ai-0.0.2/juno_ai.egg-info/PKG-INFO` & `juno-ai-0.0.3/juno_ai.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: juno-ai
-Version: 0.0.2
-Summary: UNKNOWN
+Version: 0.0.3
 Home-page: https://github.com/alexi/juno
 Author: juno
 Author-email: hellojunoai@gmail.com
-License: UNKNOWN
-Description: Juno AI Assistant for Jupyter Notebook
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+
+Juno AI Assistant for Jupyter Notebook
```

### Comparing `juno-ai-0.0.2/setup.py` & `juno-ai-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # exec(open(read('juno/version.py')).read())
 print('packages:', [package for package in find_packages()
                 if package.startswith('juno')])
 setup(
     name='juno-ai', 
     # version=__version__, 
-    version='0.0.2',
+    version='0.0.3',
     packages=[package for package in find_packages()
                 if package.startswith('juno')], 
     long_description='Juno AI Assistant for Jupyter Notebook',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Framework :: IPython',
         'Intended Audience :: Developers',
```

### Comparing `juno-ai-0.0.2/juno/magic.py` & `juno-ai-0.0.3/juno/magic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from IPython.core.magic import (Magics, magics_class, line_magic, cell_magic, needs_local_scope)
-from .juno import chat, debug, edit
+from .juno import chat, debug, edit, feedback
 from .serialize_context import variable_description
 from .client_setup import setup
 
 @magics_class
 class Assistant(Magics):
 
     @line_magic
@@ -26,23 +26,28 @@
     def edit(self, line, local_ns=None):
         return edit(line, variable_description(local_ns))
 
     @line_magic
     @needs_local_scope
     def debug(self, line, local_ns=None):
         return debug(line, variable_description(local_ns))
+    
+    @line_magic
+    @needs_local_scope
+    def feedback(self, line, local_ns=None):
+        return feedback(line)
 
 _loaded = False
 def load_ipython_extension(ip, **kwargs):
     """Load the extension in IPython."""
     global _loaded
     if not _loaded:
         ip.register_magics(Assistant)
         setup()
         _loaded = True
+    else:
+        setup()
 
 def unload_ipython_extension(ip):
     global _loaded
     if _loaded:
-        magic = ip.magics_manager.registry.pop('MatlabMagics')
-        magic.Matlab.stop()
         _loaded = False
```

### Comparing `juno-ai-0.0.2/juno/serialize_context.py` & `juno-ai-0.0.3/juno/serialize_context.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.2/juno/client_setup.py` & `juno-ai-0.0.3/juno/client_setup.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.2/juno/output_parser.py` & `juno-ai-0.0.3/juno/output_parser.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.2/juno/event_javascript.py` & `juno-ai-0.0.3/juno/event_javascript.py`

 * *Files 5% similar despite different names*

```diff
@@ -192,33 +192,29 @@
     let row = cell.element.find('.debug-container');
     if(row.length){
         row.remove();
     }
 }
 
 function cellHasErrorOutput(cell) {
-    console.log("checking cell:", cell.cell_id)
     if (!cell.output_area || ! cell.output_area.outputs) {
-        console.log("cell-id:", cell.cell_id, "no outputs")
         return false;
     }
     // if any output has output_type === 'error', then the cell has an error
     for (const output of cell.output_area.outputs) {
         if (output.output_type === 'error') {
             return true;
         }
     }
     return false;
 }
 
 function cleanDebugButtons(addOnly) {    
     let cells = Jupyter.notebook.get_cells();
-    for (let i = 0; i < cells.length; i++) {
-        let cell = cells[i];
-        console.log("cell:", cell)
+    for (const [i, cell] of cells.entries()) {
         let shouldShowDebugButton = cellHasErrorOutput(cell) && !window.JunoEditZones.isEditCell(cell);
         if (shouldShowDebugButton ) {
             addFixButton(cell, i);
         }
         else if (!addOnly && !shouldShowDebugButton) {
             removeFixButton(cell);
         }
@@ -453,27 +449,28 @@
 if(!window.JunoEditZones){
     window.JunoEditZones = new EditZoneManager();
 }
 if(!window.juno_initialized){
     window.openEditor = openEditor;
     Jupyter.notebook.events.off('output_appended.OutputArea');
     Jupyter.notebook.events.off('execute.CodeCell');
-    Jupyter.notebook.events.on('output_appended.OutputArea', null, () => {
-            console.log("output appended")
+    Jupyter.notebook.events.on('output_appended.OutputArea', ( data) => {
             setTimeout(() => cleanDebugButtons(true), 400)
             setTimeout(() => cleanDebugButtons(false), 800)
+            setTimeout(() => cleanDebugButtons(false), 2000)
         }
     );
     Jupyter.notebook.events.on('execute.CodeCell', null, () => setTimeout(() => cleanDebugButtons(false), 400));
     // when cell is created, add edit button
     Jupyter.notebook.events.on('create.Cell', () => {
         setTimeout(() => addEditButtons(), 150)
         setTimeout(() => addEditButtons(), 400)
     });
     setInterval(() => addEditButtons(), 3000);
+    setInterval(() => cleanDebugButtons(true), 3000);
     // when cell is deleted call JunoEditZones.handleDeleteCell
     Jupyter.notebook.events.on('delete.Cell', (event, data) => JunoEditZones.handleDeleteCell(data.cell));
     addEditButtons();
     setTimeout(() => addEditButtons(), 600);
     console.log("loaded listener js");
     window.juno_initialized = true;
 }
@@ -494,15 +491,17 @@
     junoInfo.style = "margin-top: 10px; margin-bottom: 10px; padding: 10px; border: 1px solid #e6e6e6; border-radius: 3px; background-color: #f9f9f9; font-size: 12px; color: #666;";
     if(version && version !== ""){{
     }}
     // list the commands juno can run with explanations
     junoInfo.innerHTML = "Juno is your data science co-pilot. Here are some things you can do with Juno:<br><br>" +
         "<b>%juno</b> - prompt juno to write code for you<br>" +
         "<b>✎ edit</b> - prompt juno to edit a cell for you<br>" +
-        "<b>🪲 debug</b> - have juno automatically fix your code when it outputs an error<br>"
+        "<b>🪲 debug</b> - have juno automatically fix your code when it outputs an error<br>" +
+        "<div style='display: block;width: 100%;height: 1px;background-color: color(srgb 0.765 0.765 0.765);margin-top: 10px;margin-bottom: 10px;'></div>" +
+        "<b><span style=''>%feedback</span></b> - send us some feedback on the alpha 🙏<br>"
     outputArea.element.append(junoInfo);
 }}
 displayJunoInfo({version});
 
 """
 
 def get_info_injection(version):
```

### Comparing `juno-ai-0.0.2/juno/juno.py` & `juno-ai-0.0.3/juno/juno.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import json
 from IPython.display import Javascript, clear_output, display, HTML
 
 from .event_javascript import BUTTON_HANDLERS, LISTENER_JS, get_info_injection
-from .prompting_javascript import write_edit_stream, write_completion_stream
+from .prompting_javascript import write_edit_stream, write_completion_stream, submit_feedback
 
 
 def chat(command, notebook_state):
     encoded_nb_state = base64.b64encode(json.dumps(notebook_state).encode('utf-8')).decode('utf-8')
     completion_js = write_completion_stream(command, encoded_nb_state, True, 5)
     display(Javascript(LISTENER_JS + completion_js))
     clear_output()
@@ -26,7 +26,12 @@
 
 def debug(_, notebook_state):
     command = ""
     encoded_nb_state = base64.b64encode(json.dumps(notebook_state).encode('utf-8')).decode('utf-8')
     completion_js = write_edit_stream(command, encoded_nb_state, True, 5, True)
     display(Javascript(LISTENER_JS + completion_js))
     clear_output()
+
+def feedback(command):
+    completion_js = submit_feedback(command)
+    display(Javascript(LISTENER_JS + completion_js))
+    clear_output()
```

### Comparing `juno-ai-0.0.2/juno/prompting_javascript.py` & `juno-ai-0.0.3/juno/prompting_javascript.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,17 +33,59 @@
         let error = errorOutputs[0];
         return `${error.ename}: ${error.evalue}`;
     }
     return "";
 }
 """
 
+def submit_feedback(feedback):
+    return """
+
+// Back up one cell from the current selection to get the one with the command
+let startCell = Jupyter.notebook.get_selected_index() - 1;
+let cell = Jupyter.notebook.get_cell(startCell);
+async function sendFeedback() {{
+    let context, errorContent;
+    let startingCellText = cell.get_text()
+    let text = startingCellText.replace("%feedback ", "")
+    // Select the cell with the command
+    let cell_id = cell.cell_id;
+    
+    const payload = {{
+        "message": `{feedback}`,
+        "visitor_id": localStorage.getItem("visitor_id"),
+        "user_id": localStorage.getItem("user_id"),
+        "timestamp": Date.now(),
+    }};
+    await fetch("https://api.struct.network/feedback", {{
+        method: "POST",
+        headers: {{
+            "Content-Type": "application/json"
+        }},
+        body: JSON.stringify(payload),
+        onMessage(message) {{
+            console.log("message")
+        }}
+    }})
+    // add thank you message below cell
+    let outputArea = cell.output_area;
+    let junoInfo = document.createElement("div");
+    junoInfo.id = "juno-info";
+    junoInfo.style = "margin-top: 10px; margin-bottom: 10px; padding: 10px; border: 1px solid #e6e6e6; border-radius: 3px; background-color: #f9f9f9; font-size: 12px; color: #666;";
+    // list the commands juno can run with explanations
+    junoInfo.innerHTML = "Thank you for your feedback!"
+    outputArea.element.append(junoInfo);
+}}
+if ((Date.now() / 1000) - {current_time} < 2) {{
+    sendFeedback();
+}}
+    """.format(feedback=feedback, current_time=round(time()))
+
 GET_ANSWER_CODE = """
 async function getCompletion(callback, endpoint, payload, doneCallback) {{
-    console.log("doneCallback", doneCallback)
 
     payload["visitor_id"] = localStorage.getItem("visitor_id")
     payload["user_id"] = localStorage.getItem("user_id")
 
     await fetchSSE("https://api.struct.network/" + endpoint, {{
         method: "POST",
         headers: {{
```

