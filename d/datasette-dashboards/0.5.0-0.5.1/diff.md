# Comparing `tmp/datasette_dashboards-0.5.0.tar.gz` & `tmp/datasette_dashboards-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_dashboards-0.5.0.tar", max compression
+gzip compressed data, was "datasette_dashboards-0.5.1.tar", max compression
```

## Comparing `datasette_dashboards-0.5.0.tar` & `datasette_dashboards-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/LICENSE
--rw-r--r--   0        0        0    11575 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/README.md
--rw-r--r--   0        0        0     7837 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/datasette_dashboards/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/datasette_dashboards/py.typed
--rw-r--r--   0        0        0     1358 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/datasette_dashboards/static/dashboards.css
--rw-r--r--   0        0        0     6417 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/datasette_dashboards/static/dashboards.js
--rw-r--r--   0        0        0    64383 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/datasette_dashboards/static/vega-embed.min.js
--rw-r--r--   0        0        0   244624 2023-04-20 16:51:57.823827 datasette_dashboards-0.5.0/datasette_dashboards/static/vega-lite.min.js
--rw-r--r--   0        0        0   510672 2023-04-20 16:51:57.823827 datasette_dashboards-0.5.0/datasette_dashboards/static/vega.min.js
--rw-r--r--   0        0        0     2270 2023-04-20 16:51:57.823827 datasette_dashboards-0.5.0/datasette_dashboards/templates/dashboard_chart.html
--rw-r--r--   0        0        0      617 2023-04-20 16:51:57.823827 datasette_dashboards-0.5.0/datasette_dashboards/templates/dashboard_list.html
--rw-r--r--   0        0        0     4925 2023-04-20 16:51:57.823827 datasette_dashboards-0.5.0/datasette_dashboards/templates/dashboard_view.html
--rw-r--r--   0        0        0     1427 2023-04-20 16:51:57.835827 datasette_dashboards-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    12419 1970-01-01 00:00:00.000000 datasette_dashboards-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-25 17:58:35.291677 datasette_dashboards-0.5.1/LICENSE
+-rw-r--r--   0        0        0    11772 2023-04-25 17:58:35.291677 datasette_dashboards-0.5.1/README.md
+-rw-r--r--   0        0        0     8184 2023-04-25 17:58:35.291677 datasette_dashboards-0.5.1/datasette_dashboards/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:58:35.291677 datasette_dashboards-0.5.1/datasette_dashboards/py.typed
+-rw-r--r--   0        0        0     1400 2023-04-25 17:58:35.291677 datasette_dashboards-0.5.1/datasette_dashboards/static/dashboards.css
+-rw-r--r--   0        0        0     6585 2023-04-25 17:58:35.291677 datasette_dashboards-0.5.1/datasette_dashboards/static/dashboards.js
+-rw-r--r--   0        0        0    64383 2023-04-25 17:58:35.291677 datasette_dashboards-0.5.1/datasette_dashboards/static/vega-embed.min.js
+-rw-r--r--   0        0        0   244624 2023-04-25 17:58:35.295677 datasette_dashboards-0.5.1/datasette_dashboards/static/vega-lite.min.js
+-rw-r--r--   0        0        0   510672 2023-04-25 17:58:35.299677 datasette_dashboards-0.5.1/datasette_dashboards/static/vega.min.js
+-rw-r--r--   0        0        0     2292 2023-04-25 17:58:35.299677 datasette_dashboards-0.5.1/datasette_dashboards/templates/dashboard_chart.html
+-rw-r--r--   0        0        0      617 2023-04-25 17:58:35.299677 datasette_dashboards-0.5.1/datasette_dashboards/templates/dashboard_list.html
+-rw-r--r--   0        0        0     4947 2023-04-25 17:58:35.299677 datasette_dashboards-0.5.1/datasette_dashboards/templates/dashboard_view.html
+-rw-r--r--   0        0        0     1463 2023-04-25 17:58:35.307677 datasette_dashboards-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    12616 1970-01-01 00:00:00.000000 datasette_dashboards-0.5.1/PKG-INFO
```

### Comparing `datasette_dashboards-0.5.0/LICENSE` & `datasette_dashboards-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.0/README.md` & `datasette_dashboards-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -271,18 +271,21 @@
 Then create a new virtual environment and the required dependencies:
 
 ```bash
 poetry install
 poetry shell
 ```
 
-To run the tests:
+To run the QA suite:
 
 ```bash
-pytest
+black --check datasette_dashboards tests
+flake8 datasette_dashboards tests
+mypy datasette_dashboards tests
+pytest -v --cov=datasette_dashboards --cov=tests --cov-branch --cov-report=term-missing tests
 ```
 
 ## Demo
 
 With the developmnent environment setup, you can run the demo locally:
 
 ```bash
```

### Comparing `datasette_dashboards-0.5.0/datasette_dashboards/__init__.py` & `datasette_dashboards-0.5.1/datasette_dashboards/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 async def dashboard_list(request: Request, datasette: "Datasette") -> Response:
     await check_permission_instance(request, datasette)
     config = datasette.plugin_config("datasette-dashboards") or {}
     return Response.html(
         await datasette.render_template(
             "dashboard_list.html",
             {"dashboards": config},
+            request=request,
         )
     )
 
 
 async def _dashboard_view(
     request: Request, datasette: "Datasette", embed: bool = False
 ) -> Response:
@@ -142,20 +143,24 @@
         fill_chart_query_options(chart, query_parameters)
 
     return Response.html(
         await datasette.render_template(
             "dashboard_view.html",
             {
                 "settings": settings,
+                "absolute_url": datasette.absolute_url(
+                    request, datasette.urls.instance()
+                ),
                 "slug": slug,
                 "query_parameters": query_parameters,
                 "query_string": query_string,
                 "dashboard": dashboard,
                 "embed": embed,
             },
+            request=request,
         )
     )
 
 
 async def dashboard_view(request: Request, datasette: "Datasette") -> Response:
     return await _dashboard_view(request, datasette, embed=False)
 
@@ -193,20 +198,24 @@
     query_string = generate_dashboard_filters_qs(request, options_keys)
     fill_chart_query_options(chart, query_parameters)
 
     return Response.html(
         await datasette.render_template(
             "dashboard_chart.html",
             {
+                "absolute_url": datasette.absolute_url(
+                    request, datasette.urls.instance()
+                ),
                 "slug": slug,
                 "query_string": query_string,
                 "dashboard": dashboard,
                 "chart": chart,
                 "embed": embed,
             },
+            request=request,
         )
     )
 
 
 async def dashboard_chart(request: Request, datasette: "Datasette") -> Response:
     return await _dashboard_chart(request, datasette, embed=False)
```

### Comparing `datasette_dashboards-0.5.0/datasette_dashboards/static/dashboards.css` & `datasette_dashboards-0.5.1/datasette_dashboards/static/dashboards.css`

 * *Files 2% similar despite different names*

```diff
@@ -75,7 +75,11 @@
   height: 100%;
 }
 
 .chart-container {
   width: 100%;
   height: 70vh;
 }
+
+#vg-tooltip-element * {
+  all: revert;
+}
```

### Comparing `datasette_dashboards-0.5.0/datasette_dashboards/static/dashboards.js` & `datasette_dashboards-0.5.1/datasette_dashboards/static/dashboards.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-function renderVegaChart(el, chart, query_string, full_height) {
+function renderVegaChart(el, chart, query_string, absolute_url, full_height) {
     const query = encodeURIComponent(chart.query)
     let defaultSignals = [{
         'name': 'width',
         'init': 'isFinite(containerSize()[0]) ? containerSize()[0] : 200',
         'on': [{
             'update': 'isFinite(containerSize()[0]) ? containerSize()[0] : 200',
             'events': 'window:resize'
@@ -24,28 +24,28 @@
         description: chart.title,
         autosize: {
             'type': 'fit',
             'resize': true
         },
         data: [{
             name: 'table',
-            url: `/${chart.db}.csv?sql=${query}&${query_string}`,
+            url: `${absolute_url}${chart.db}.csv?sql=${query}&${query_string}`,
             format: {
                 'type': 'csv',
                 'parse': 'auto'
             }
         }],
         signals: defaultSignals,
         ...chart.display
     };
 
     vegaEmbed(el, spec);
 }
 
-function renderVegaLiteChart(el, chart, query_string, full_height) {
+function renderVegaLiteChart(el, chart, query_string, absolute_url, full_height) {
     const query = encodeURIComponent(chart.query)
     const spec = {
         $schema: 'https://vega.github.io/schema/vega-lite/v5.json',
         description: chart.title,
         width: 'container',
         height: full_height ? 'container' : undefined,
         view: {
@@ -57,28 +57,28 @@
                 innerRadius: 50
             },
             line: {
                 point: true
             }
         },
         data: {
-            url: `/${chart.db}.csv?sql=${query}&${query_string}`,
+            url: `${absolute_url}${chart.db}.csv?sql=${query}&${query_string}`,
             format: {
                 'type': 'csv'
             }
         },
         ...chart.display
     };
 
     vegaEmbed(el, spec);
 }
 
-async function renderMetricChart(el, chart, query_string, full_height) {
+async function renderMetricChart(el, chart, query_string, absolute_url, full_height) {
     const query = encodeURIComponent(chart.query)
-    const results = await fetch(`/${chart.db}.json?sql=${query}&${query_string}&_shape=array`)
+    const results = await fetch(`${absolute_url}${chart.db}.json?sql=${query}&${query_string}&_shape=array`)
     const data = await results.json()
     const metric = data[0][chart.display.field]
 
     const prefix = chart.display.prefix || ''
     const suffix = chart.display.suffix || ''
     const text = `${prefix}${metric}${suffix}`
 
@@ -98,17 +98,17 @@
     wrapper.style.overflow = 'hidden'
     wrapper.style.whiteSpace = 'nowrap'
     wrapper.style.textOverflow = 'ellipsis'
 
     document.querySelector(el).appendChild(wrapper)
 }
 
-async function renderTableChart(el, chart, query_string, full_height) {
+async function renderTableChart(el, chart, query_string, absolute_url, full_height) {
     const query = encodeURIComponent(chart.query)
-    const results = await fetch(`/${chart.db}.json?sql=${query}&${query_string}`)
+    const results = await fetch(`${absolute_url}${chart.db}.json?sql=${query}&${query_string}`)
     const data = await results.json()
 
     const thead = document.createElement('thead')
     const thead_tr = document.createElement('tr')
     data.columns.forEach(col => {
         const thead_th = document.createElement('th')
         thead_th.innerHTML = col
@@ -136,18 +136,18 @@
     wrapper.style.height = '100%'
     wrapper.style.overflow = 'auto'
     wrapper.appendChild(table)
 
     document.querySelector(el).appendChild(wrapper)
 }
 
-async function renderMapChart(el, chart, query_string, full_height) {
+async function renderMapChart(el, chart, query_string, absolute_url, full_height) {
     document.addEventListener("DOMContentLoaded", async () => {
         const query = encodeURIComponent(chart.query)
-        const results = await fetch(`/${chart.db}.json?sql=${query}&${query_string}&_shape=array`)
+        const results = await fetch(`${absolute_url}${chart.db}.json?sql=${query}&${query_string}&_shape=array`)
         const data = await results.json()
 
         const wrapper = document.createElement('div')
         wrapper.style.width = '100%'
         wrapper.style.height = '100%'
         wrapper.style.minHeight = '200px'
         document.querySelector(el).appendChild(wrapper)
@@ -179,25 +179,25 @@
 
         const coords = data.map(row => [row[latitude_column], row[longitude_column]])
         const bounds = new L.LatLngBounds(coords)
         map.fitBounds(bounds)
     })
 }
 
-async function renderChart(el, chart, query_string, full_height = false) {
+async function renderChart(el, chart, query_string, absolute_url, full_height = false) {
     renderers = new Map()
     renderers.set('vega', renderVegaChart)
     renderers.set('vega-lite', renderVegaLiteChart)
     renderers.set('metric', renderMetricChart)
     renderers.set('table', renderTableChart)
     renderers.set('map', renderMapChart)
 
     render = renderers.get(chart.library)
     if (render) {
-        await render(el, chart, query_string, full_height)
+        await render(el, chart, query_string, absolute_url, full_height)
     }
 }
 
 function toggleFullscreen() {
     const el = document.querySelector("section.content")
     if (document.fullscreenElement) {
         document.exitFullscreen()
```

### Comparing `datasette_dashboards-0.5.0/datasette_dashboards/static/vega-embed.min.js` & `datasette_dashboards-0.5.1/datasette_dashboards/static/vega-embed.min.js`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.0/datasette_dashboards/static/vega-lite.min.js` & `datasette_dashboards-0.5.1/datasette_dashboards/static/vega-lite.min.js`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.0/datasette_dashboards/static/vega.min.js` & `datasette_dashboards-0.5.1/datasette_dashboards/static/vega.min.js`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.0/datasette_dashboards/templates/dashboard_chart.html` & `datasette_dashboards-0.5.1/datasette_dashboards/templates/dashboard_chart.html`

 * *Files 4% similar despite different names*

```diff
@@ -63,10 +63,10 @@
 
   <script src="{{ datasette_leaflet_url }}" type="module"></script>
   <script src="{{ urls.static_plugins('datasette_dashboards', 'vega.min.js') }}"></script>
   <script src="{{ urls.static_plugins('datasette_dashboards', 'vega-lite.min.js') }}"></script>
   <script src="{{ urls.static_plugins('datasette_dashboards', 'vega-embed.min.js') }}"></script>
   <script src="{{ urls.static_plugins('datasette_dashboards', 'dashboards.js') }}"></script>
   <script type="text/javascript">
-    renderChart('#chart', {{ chart|tojson }}, '{{ query_string|safe }}', true)
+    renderChart('#chart', {{ chart|tojson }}, '{{ query_string|safe }}', '{{ absolute_url }}', true)
   </script>
 {% endblock %}
```

### Comparing `datasette_dashboards-0.5.0/datasette_dashboards/templates/dashboard_list.html` & `datasette_dashboards-0.5.1/datasette_dashboards/templates/dashboard_list.html`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.0/datasette_dashboards/templates/dashboard_view.html` & `datasette_dashboards-0.5.1/datasette_dashboards/templates/dashboard_view.html`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
   <script src="{{ datasette_leaflet_url }}" type="module"></script>
   <script src="{{ urls.static_plugins('datasette_dashboards', 'vega.min.js') }}"></script>
   <script src="{{ urls.static_plugins('datasette_dashboards', 'vega-lite.min.js') }}"></script>
   <script src="{{ urls.static_plugins('datasette_dashboards', 'vega-embed.min.js') }}"></script>
   <script src="{{ urls.static_plugins('datasette_dashboards', 'dashboards.js') }}"></script>
   <script type="text/javascript">
     {% for chart_slug, chart in dashboard.charts.items() %}
-    renderChart('#chart-{{ chart_slug }}', {{ chart|tojson }}, '{{ query_string|safe }}')
+    renderChart('#chart-{{ chart_slug }}', {{ chart|tojson }}, '{{ query_string|safe }}', '{{ absolute_url }}')
     {% endfor %}
 
     {% if settings.autorefresh %}
     autorefresh({{ settings.autorefresh }})
     {% endif %}
   </script>
 {% endblock %}
```

### Comparing `datasette_dashboards-0.5.0/pyproject.toml` & `datasette_dashboards-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datasette-dashboards"
-version = "0.5.0"
+version = "0.5.1"
 description = "Datasette plugin providing data dashboards from metadata"
 repository = "https://github.com/rclement/datasette-dashboards"
 authors = ["Romain Clement"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 packages = [{include = "datasette_dashboards"}]
 
@@ -18,16 +18,17 @@
 datasette-render-markdown = "*"
 
 [tool.poetry.group.dev.dependencies]
 black = "==23.3.0"
 datasette-block-robots = "==1.1"
 datasette-cluster-map = "==0.17.2"
 datasette-publish-vercel = "==0.14.2"
+datasette-sqlite-http = "==0.1.0a2"
 datasette-vega = "==0.6.2"
-faker = "==18.4.0"
+faker = "==18.5.1"
 flake8 = "==6.0.0"
 mypy = "==1.2.0"
 pytest = "==7.3.1"
 pytest-asyncio = "==0.21.0"
 pytest-cov = "==4.0.0"
 sqlite-utils = "==3.30"
```

### Comparing `datasette_dashboards-0.5.0/PKG-INFO` & `datasette_dashboards-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-dashboards
-Version: 0.5.0
+Version: 0.5.1
 Summary: Datasette plugin providing data dashboards from metadata
 Home-page: https://github.com/rclement/datasette-dashboards
 License: Apache License, Version 2.0
 Author: Romain Clement
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -291,18 +291,21 @@
 Then create a new virtual environment and the required dependencies:
 
 ```bash
 poetry install
 poetry shell
 ```
 
-To run the tests:
+To run the QA suite:
 
 ```bash
-pytest
+black --check datasette_dashboards tests
+flake8 datasette_dashboards tests
+mypy datasette_dashboards tests
+pytest -v --cov=datasette_dashboards --cov=tests --cov-branch --cov-report=term-missing tests
 ```
 
 ## Demo
 
 With the developmnent environment setup, you can run the demo locally:
 
 ```bash
```

