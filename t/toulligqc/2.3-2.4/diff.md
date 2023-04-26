# Comparing `tmp/toulligqc-2.3.tar.gz` & `tmp/toulligqc-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toulligqc-2.3.tar", last modified: Wed Mar 22 15:03:59 2023, max compression
+gzip compressed data, was "dist/toulligqc-2.4.tar", last modified: Wed Apr 26 15:41:10 2023, max compression
```

## Comparing `toulligqc-2.3.tar` & `toulligqc-2.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:03:59.000000 toulligqc-2.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:03:59.000000 toulligqc-2.3/test/
--rw-r--r--   0 root         (0) root         (0)    15496 2023-03-22 15:03:16.000000 toulligqc-2.3/test/test_sequencing_summary_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:03:59.000000 toulligqc-2.3/toulligqc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:03:59.000000 toulligqc-2.3/toulligqc/resources/
--rw-r--r--   0 root         (0) root         (0)  3478132 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/resources/plotly-latest.min.js
--rw-r--r--   0 root         (0) root         (0)     2339 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/resources/toulligqc.css
--rw-r--r--   0 root         (0) root         (0)     5548 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/resources/toulligqc.png
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1069 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/common.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/configuration.py
--rw-r--r--   0 root         (0) root         (0)     9795 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/fast5_extractor.py
--rw-r--r--   0 root         (0) root         (0)    16480 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/html_report_generator.py
--rw-r--r--   0 root         (0) root         (0)    42298 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/plotly_graph_common.py
--rw-r--r--   0 root         (0) root         (0)    30984 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/plotly_graph_generator.py
--rw-r--r--   0 root         (0) root         (0)    16322 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/plotly_graph_onedsquare_generator.py
--rw-r--r--   0 root         (0) root         (0)     1776 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/report_data_file_generator.py
--rw-r--r--   0 root         (0) root         (0)    19033 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/sequencing_summary_common.py
--rw-r--r--   0 root         (0) root         (0)    22702 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/sequencing_summary_extractor.py
--rw-r--r--   0 root         (0) root         (0)    22833 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/sequencing_summary_onedsquare_extractor.py
--rw-r--r--   0 root         (0) root         (0)     6917 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/sequencing_telemetry_extractor.py
--rw-r--r--   0 root         (0) root         (0)    15412 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/toulligqc.py
--rw-r--r--   0 root         (0) root         (0)     6203 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/toulligqc_info_extractor.py
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-22 15:03:17.000000 toulligqc-2.3/toulligqc/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 15:03:59.000000 toulligqc-2.3/toulligqc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      868 2023-03-22 15:03:59.000000 toulligqc-2.3/toulligqc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      972 2023-03-22 15:03:59.000000 toulligqc-2.3/toulligqc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 15:03:59.000000 toulligqc-2.3/toulligqc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-03-22 15:03:59.000000 toulligqc-2.3/toulligqc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 15:03:59.000000 toulligqc-2.3/toulligqc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      104 2023-03-22 15:03:59.000000 toulligqc-2.3/toulligqc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-22 15:03:59.000000 toulligqc-2.3/toulligqc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-22 15:03:16.000000 toulligqc-2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13970 2023-03-22 15:03:16.000000 toulligqc-2.3/README.md
--rw-r--r--   0 root         (0) root         (0)      111 2023-03-22 15:03:59.000000 toulligqc-2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1772 2023-03-22 15:03:16.000000 toulligqc-2.3/setup.py
--rw-r--r--   0 root         (0) root         (0)      868 2023-03-22 15:03:59.000000 toulligqc-2.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:41:10.000000 toulligqc-2.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:41:10.000000 toulligqc-2.4/test/
+-rw-r--r--   0 root         (0) root         (0)    15496 2023-04-26 15:40:22.000000 toulligqc-2.4/test/test_sequencing_summary_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:41:10.000000 toulligqc-2.4/toulligqc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:41:10.000000 toulligqc-2.4/toulligqc/resources/
+-rw-r--r--   0 root         (0) root         (0)  3478132 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/resources/plotly-latest.min.js
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/resources/toulligqc.css
+-rw-r--r--   0 root         (0) root         (0)     5548 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/resources/toulligqc.png
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/common.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/configuration.py
+-rw-r--r--   0 root         (0) root         (0)    10299 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/fast5_extractor.py
+-rw-r--r--   0 root         (0) root         (0)    17048 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/html_report_generator.py
+-rw-r--r--   0 root         (0) root         (0)    42707 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/plotly_graph_common.py
+-rw-r--r--   0 root         (0) root         (0)    30984 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/plotly_graph_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16322 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/plotly_graph_onedsquare_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1776 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/report_data_file_generator.py
+-rw-r--r--   0 root         (0) root         (0)    19033 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/sequencing_summary_common.py
+-rw-r--r--   0 root         (0) root         (0)    23482 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/sequencing_summary_extractor.py
+-rw-r--r--   0 root         (0) root         (0)    22833 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/sequencing_summary_onedsquare_extractor.py
+-rw-r--r--   0 root         (0) root         (0)     7181 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/sequencing_telemetry_extractor.py
+-rw-r--r--   0 root         (0) root         (0)    15412 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/toulligqc.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/toulligqc_info_extractor.py
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-26 15:40:23.000000 toulligqc-2.4/toulligqc/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:41:10.000000 toulligqc-2.4/toulligqc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      868 2023-04-26 15:41:10.000000 toulligqc-2.4/toulligqc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      972 2023-04-26 15:41:10.000000 toulligqc-2.4/toulligqc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:41:10.000000 toulligqc-2.4/toulligqc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-04-26 15:41:10.000000 toulligqc-2.4/toulligqc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:41:10.000000 toulligqc-2.4/toulligqc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-26 15:41:10.000000 toulligqc-2.4/toulligqc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-26 15:41:10.000000 toulligqc-2.4/toulligqc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-26 15:40:22.000000 toulligqc-2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13970 2023-04-26 15:40:22.000000 toulligqc-2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-26 15:41:10.000000 toulligqc-2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-04-26 15:40:22.000000 toulligqc-2.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)      868 2023-04-26 15:41:10.000000 toulligqc-2.4/PKG-INFO
```

### Comparing `toulligqc-2.3/test/test_sequencing_summary_extractor.py` & `toulligqc-2.4/test/test_sequencing_summary_extractor.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc/resources/plotly-latest.min.js` & `toulligqc-2.4/toulligqc/resources/plotly-latest.min.js`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc/resources/toulligqc.css` & `toulligqc-2.4/toulligqc/resources/toulligqc.css`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc/resources/toulligqc.png` & `toulligqc-2.4/toulligqc/resources/toulligqc.png`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc/common.py` & `toulligqc-2.4/toulligqc/common.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc/configuration.py` & `toulligqc-2.4/toulligqc/configuration.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc/fast5_extractor.py` & `toulligqc-2.4/toulligqc/fast5_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,14 +136,21 @@
         _set_result_dict_value(result_dict, prefix + '.exp.start.time', tracking_id_dict, 'exp_start_time')
         _set_result_dict_value(result_dict, prefix + '.device.id', tracking_id_dict, 'device_id')
         _set_result_dict_value(result_dict, prefix + '.device.type', tracking_id_dict, 'device_type')
         _set_result_dict_value(result_dict, prefix + '.distribution.version', tracking_id_dict, 'distribution_version')
         _set_result_dict_value(result_dict, prefix + '.flow.cell.product.code', tracking_id_dict,
                                'flow_cell_product_code')
 
+        context_tags_dict = self._get_fast5_items(h5py_file, 'context_tags')
+        if len(context_tags_dict) != 0:
+            _set_result_dict_value(result_dict, prefix + '.selected.speed.bases.per.second', context_tags_dict, 'selected_speed_bases_per_second')
+            _set_result_dict_value(result_dict, prefix + '.sample.frequency', context_tags_dict, 'sample_frequency')
+            _set_result_dict_value(result_dict, prefix + '.sequencing.kit.version', context_tags_dict, 'sequencing_kit')
+
+
     def graph_generation(self, result_dict):
         """
         Graph generation
         :return: nothing
         """
         return []
```

### Comparing `toulligqc-2.3/toulligqc/html_report_generator.py` & `toulligqc-2.4/toulligqc/html_report_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,14 +166,16 @@
     flow_cell_id = _get_result_value(result_dict, 'sequencing.telemetry.extractor.flowcell.id', "Unknown")
     experiment_group = _get_result_value(result_dict, 'sequencing.telemetry.extractor.protocol.group.id', "Unknown")
     run_id = _get_result_value(result_dict, 'sequencing.telemetry.extractor.run.id', "Unknown")
     flowcell_version = _get_result_value(result_dict, 'sequencing.telemetry.extractor.flowcell.version', "Unknown")
     kit_version = _get_result_value(result_dict, 'sequencing.telemetry.extractor.kit.version', "Unknown")
     sequencing_kit_version = _get_result_value(result_dict, 'sequencing.telemetry.extractor.sequencing.kit.version', "Unknown")
     barcode_kits_version = _get_result_value(result_dict, 'sequencing.telemetry.extractor.barcode.kits.version', "Unknown")
+    selected_speed_bases_per_second = _get_result_value(result_dict, 'sequencing.telemetry.extractor.selected.speed.bases.per.second', "Unknown")
+    sample_frequency = _get_result_value(result_dict, 'sequencing.telemetry.extractor.sample.frequency', "Unknown")
     basecaller_name = _get_result_value(result_dict, 'sequencing.telemetry.extractor.software.name', "Unknown")
     basecaller_version = _get_result_value(result_dict, 'sequencing.telemetry.extractor.software.version', "Unknown")
     basecaller_analysis = _get_result_value(result_dict, 'sequencing.telemetry.extractor.software.analysis', "Unknown")
     hostname = _get_result_value(result_dict, 'sequencing.telemetry.extractor.hostname', "Unknown")
     device_id = _get_result_value(result_dict, 'sequencing.telemetry.extractor.device.id', "Unknown")
     device_type = _get_result_value(result_dict, 'sequencing.telemetry.extractor.device.type', "Unknown")
     model_file = _get_result_value(result_dict, 'sequencing.telemetry.extractor.model.file', "Unknown")
@@ -202,14 +204,16 @@
               <tr><th>Run duration </th><td>{run_time}</td></tr>
               <tr><th>Flowcell ID</th><td>{flow_cell_id}</td></tr>
               <tr><th>Flowcell product code</th><td>{flow_cell_product_code}</td></tr>
               <tr><th>Flowcell version</th><td>{flowcell_version}</td></tr>
               <tr><th>Kit</th><td>{kit_version}</td></tr>
               <tr><th>Sequencing kit</th><td>{sequencing_kit_version}</td></tr>
               <tr><th>Barcode kits</th><td>{barcode_kits_version}</td></tr>
+              <tr><th>Selected speed (bps)</th><td>{selected_speed_bases_per_second}</td></tr>
+              <tr><th>Sample frequency (Hz)</th><td>{sample_frequency}</td></tr>
               <tr><th>Yield</th><td>{run_yield}</td></tr>
               <tr><th>Read count</th><td>{read_count}</td></tr>
               <tr><th>N50 (bp)</th><td>{n50}</td></tr>
               <tr><th>L50</th><td>{l50}</td></tr>
               </tbody>
             </table>
       </div> <!-- End of "Run-statistics" module -->
@@ -222,14 +226,16 @@
                run_time=run_time,
                flow_cell_id=flow_cell_id,
                flow_cell_product_code=flow_cell_product_code,
                flowcell_version=flowcell_version,
                kit_version=kit_version,
                sequencing_kit_version=sequencing_kit_version,
                barcode_kits_version=barcode_kits_version,
+               selected_speed_bases_per_second=selected_speed_bases_per_second,
+               sample_frequency=sample_frequency,
                run_yield=run_yield,
                read_count=_format_int(read_count),
                n50=_format_int(int(n50)),
                l50=_format_int(int(l50)))
 
     result += """
       <div class="module" id="software_info">
```

### Comparing `toulligqc-2.3/toulligqc/plotly_graph_common.py` & `toulligqc-2.4/toulligqc/plotly_graph_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,24 +391,26 @@
     if quartiles:
         fig.add_trace(go.Scatter(
             x=x,
             y=y[1],
             name="25% quartile",
             mode='lines',
             fill="none",
+            connectgaps=True,
             line=dict(color=color,
                       width=line_width,
                       shape="spline")))
 
         fig.add_trace(go.Scatter(
             x=x,
             y=y[3],
             name="75% quartile",
             mode='lines',
             fill="tonexty",
+            connectgaps=True,
             line=dict(color=color,
                       width=line_width,
                       shape="spline")))
 
         fig.add_trace(go.Scatter(
             x=x,
             y=y[2],
@@ -1055,29 +1057,33 @@
             x = all_length[idx_all],
             y = all_qscore[idx_all],
             colorscale = [[0, 'white'], [0.5, 'khaki'], [1.0, all_color]], 
             reversescale = False,
             xaxis = 'x',
             yaxis = 'y',
             colorbar = dict(
-            title = '<b>Legend</b>',
-            len = 0.4
-        )
+                title = '<b>Legend</b>',
+                len = 0.5)
         ))
 
     fig.add_trace(go.Histogram2dContour(
             x = read_pass_length[idx_pass],
             y = read_pass_qscore[idx_pass],
             colorscale = [[0, 'white'], [0.5, 'honeydew'], [1.0, pass_color]], 
             reversescale = False,
             xaxis = 'x',
             yaxis = 'y',
             colorbar = dict(
-            title = '<b>Legend</b>',
-            len = 0.4
+            #title = '<b>Legend</b>',
+            len = 0.4,
+            title = dict(
+                font= dict(
+                    size = 9
+                )
+            )
         ),
         visible=False
         ))
 
     fig.add_trace(go.Histogram2dContour(
             x = read_fail_length[idx_fail],
             y = read_fail_qscore[idx_fail],
@@ -1178,29 +1184,27 @@
         ),
         height = 600,
         width = 1000,
         bargap = 0,
         paper_bgcolor="#FFFFFF", 
         plot_bgcolor="#FFFFFF",
         hovermode = 'closest',
-        showlegend = False,
-        **_title(graph_name),
-
+        showlegend = False
     )
 
     # Add buttons
     fig.update_layout(
         updatemenus=[
             dict(
                 type="buttons",
                 direction="down",
                 buttons=list([
                     dict(
                         args=[{'visible': [True, False, False, True, True, False, False, False, False]}, {'hovermode': False}],
-                        label="all reads",
+                        label="All reads",
                         method="restyle"
                     ),
                     dict(
                         args=[{'visible': [False, True, False, False, False, True, True, False, False]}, {'hovermode': 'x'}],
                         label="Pass reads",
                         method="restyle"
                     ),
@@ -1216,14 +1220,23 @@
                 xanchor="left",
                 y=1.25,
                 yanchor="top"
             ),
         ]
     )
 
+    fig.update_layout(
+        **_title(graph_name),
+        **_legend(),
+        **default_graph_layout,
+        #hovermode='x',
+        #**_xaxis('PHRED score', dict(rangemode="tozero")),
+        #**_yaxis('Density probability', dict(rangemode="tozero")),
+    )
+
     table_html = None
     div, output_file = _create_and_save_div(fig, result_directory, graph_name)
 
     return graph_name, output_file, table_html, div
 
 
 def interpolation_points(series, graph_name):
```

### Comparing `toulligqc-2.3/toulligqc/plotly_graph_generator.py` & `toulligqc-2.4/toulligqc/plotly_graph_generator.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc/plotly_graph_onedsquare_generator.py` & `toulligqc-2.4/toulligqc/plotly_graph_onedsquare_generator.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc/report_data_file_generator.py` & `toulligqc-2.4/toulligqc/report_data_file_generator.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc/sequencing_summary_common.py` & `toulligqc-2.4/toulligqc/sequencing_summary_common.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc/sequencing_summary_extractor.py` & `toulligqc-2.4/toulligqc/sequencing_summary_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,26 +370,35 @@
                     {'barcode_arrangement': 'category'})
 
                 return pd.read_csv(files[0], sep="\t", usecols=sequencing_summary_columns,
                                    dtype=sequencing_summary_datatypes)
 
             # If multiple files, check if there's a barcoding one and a sequencing one :
             for f in files:
-
                 # check for presence of barcoding files
                 if self._is_barcode_file(f):
                     dataframe = pd.read_csv(
                         f, sep="\t", usecols=barcoding_summary_columns, dtype=barcoding_summary_datatypes)
                     if barcode_dataframe is None:
                         barcode_dataframe = dataframe
                     # if a barcoding file has already been read, append the 2 dataframes
                     else:
                         barcode_dataframe = barcode_dataframe.append(
                             dataframe, ignore_index=True)
 
+                # check for presence of sequencing_summary file with barcode info, if true load column barcode_arrangement and ignore barcoding files.
+                elif self._is_sequencing_summary_with_barcodes(f):
+                    sequencing_summary_columns.append('barcode_arrangement')
+                    sequencing_summary_datatypes.update(
+                        {'barcode_arrangement': 'category'})
+                    sys.stderr.write('Warning: The sequencing summary file {} contains barcode information.'
+                                     ' The barcoding summary files will be skipped.\n'.format(f))
+                    return pd.read_csv(f, sep="\t", usecols=sequencing_summary_columns,
+                                    dtype=sequencing_summary_datatypes)
+
                 # check for presence of sequencing_summary file, if True add column read_id for merging with barcode dataframe
                 else:
                     if self._is_sequencing_summary_file(f):
                         sequencing_summary_columns.append('read_id')
                         sequencing_summary_datatypes.update(
                             {'read_id': object})
```

### Comparing `toulligqc-2.3/toulligqc/sequencing_summary_onedsquare_extractor.py` & `toulligqc-2.4/toulligqc/sequencing_summary_onedsquare_extractor.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc/sequencing_telemetry_extractor.py` & `toulligqc-2.4/toulligqc/sequencing_telemetry_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,16 @@
         if 'opts' in array[0]:
             self._set_result_dict_value(result_dict, '.kit.version', array, 'opts', 'kit')
             self._set_result_dict_value(result_dict, '.sequencing.kit.version', array, 'context_tags', 'sequencing_kit')
             self._set_result_dict_value(result_dict, '.barcode.kits.version', array, 'opts', 'barcode_kits')
             self._set_result_dict_value(result_dict, '.flowcell.version', array, 'opts', 'flowcell')
             self._set_result_dict_value(result_dict, '.model.file', array, 'opts', 'model_file')
             self._set_result_dict_value(result_dict, '.pass.threshold.qscore', array, 'opts', 'min_qscore')
+            self._set_result_dict_value(result_dict, '.selected.speed.bases.per.second', array, 'context_tags', 'selected_speed_bases_per_second')
+            self._set_result_dict_value(result_dict, '.sample.frequency', array, 'context_tags', 'sample_frequency')
 
     def _set_result_dict_value(self, result_dict, key, array, dict_name, dict_key):
 
         final_key = self.get_report_data_file_id() + key
         current_value = None
         new_value = None
```

### Comparing `toulligqc-2.3/toulligqc/toulligqc.py` & `toulligqc-2.4/toulligqc/toulligqc.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc/toulligqc_info_extractor.py` & `toulligqc-2.4/toulligqc/toulligqc_info_extractor.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/toulligqc.egg-info/PKG-INFO` & `toulligqc-2.4/toulligqc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: toulligqc
-Version: 2.3
+Version: 2.4
 Summary: A post sequencing QC tool for Oxford Nanopore sequencers
 Home-page: https://github.com/GenomicParisCentre/toulligQC
 Author: Genomic Paris Centre team
 Author-email: toulligqc@biologie.ens.fr
 License: GPL V3
 Description: See project website for more information.
 Keywords: Nanopore MinION QC report
```

### Comparing `toulligqc-2.3/toulligqc.egg-info/SOURCES.txt` & `toulligqc-2.4/toulligqc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/README.md` & `toulligqc-2.4/README.md`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/setup.py` & `toulligqc-2.4/setup.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.3/PKG-INFO` & `toulligqc-2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: toulligqc
-Version: 2.3
+Version: 2.4
 Summary: A post sequencing QC tool for Oxford Nanopore sequencers
 Home-page: https://github.com/GenomicParisCentre/toulligQC
 Author: Genomic Paris Centre team
 Author-email: toulligqc@biologie.ens.fr
 License: GPL V3
 Description: See project website for more information.
 Keywords: Nanopore MinION QC report
```

