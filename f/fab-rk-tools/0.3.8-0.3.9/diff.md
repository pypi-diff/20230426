# Comparing `tmp/fab-rk-tools-0.3.8.tar.gz` & `tmp/fab_rk_tools-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fab-rk-tools-0.3.8.tar", max compression
+gzip compressed data, was "fab_rk_tools-0.3.9.tar", max compression
```

## Comparing `fab-rk-tools-0.3.8.tar` & `fab_rk_tools-0.3.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2022-08-03 15:03:48.620664 fab-rk-tools-0.3.8/fab_rk_tools/__init__.py
--rw-r--r--   0        0        0       39 2022-08-03 15:03:48.621662 fab-rk-tools-0.3.8/fab_rk_tools/assets/__init__.py
--rw-r--r--   0        0        0    20735 2022-11-11 15:11:53.612568 fab-rk-tools-0.3.8/fab_rk_tools/assets/opt_plotly_theme.py
--rw-r--r--   0        0        0    12848 2022-08-03 15:03:48.622662 fab-rk-tools-0.3.8/fab_rk_tools/assets/plotly_theme.py
--rw-r--r--   0        0        0    14662 2022-08-03 15:03:48.623662 fab-rk-tools-0.3.8/fab_rk_tools/assets/plotly_theme_to_remove.py
--rw-r--r--   0        0        0        0 2022-08-03 15:03:48.624662 fab-rk-tools-0.3.8/fab_rk_tools/common/__init__.py
--rw-r--r--   0        0        0      282 2022-08-03 15:03:48.624662 fab-rk-tools-0.3.8/fab_rk_tools/common/constants.py
--rw-r--r--   0        0        0      692 2022-08-29 13:24:22.338801 fab-rk-tools-0.3.8/fab_rk_tools/common/utils.py
--rw-r--r--   0        0        0       61 2022-08-03 15:03:48.625662 fab-rk-tools-0.3.8/fab_rk_tools/data/__init__.py
--rw-r--r--   0        0        0     8837 2022-08-03 15:49:03.772734 fab-rk-tools-0.3.8/fab_rk_tools/data/deriveddata.py
--rw-r--r--   0        0        0        0 2022-08-03 15:03:48.626662 fab-rk-tools-0.3.8/fab_rk_tools/data/test/__init__.py
--rw-r--r--   0        0        0     1102 2022-08-03 15:03:48.626662 fab-rk-tools-0.3.8/fab_rk_tools/data/test/deriveddata_test.py
--rw-r--r--   0        0        0        0 2022-08-03 15:03:48.627662 fab-rk-tools-0.3.8/fab_rk_tools/exceptions/__init__.py
--rw-r--r--   0        0        0      322 2022-08-03 15:03:48.627662 fab-rk-tools-0.3.8/fab_rk_tools/exceptions/data.py
--rw-r--r--   0        0        0      236 2022-08-03 15:03:48.628663 fab-rk-tools-0.3.8/fab_rk_tools/graphs/__init__.py
--rw-r--r--   0        0        0     3995 2022-08-29 13:24:22.340426 fab-rk-tools-0.3.8/fab_rk_tools/graphs/basic_bar.py
--rw-r--r--   0        0        0     3742 2022-08-29 13:24:22.341452 fab-rk-tools-0.3.8/fab_rk_tools/graphs/discrete_distro_bar.py
--rw-r--r--   0        0        0     3708 2022-08-29 13:24:22.342482 fab-rk-tools-0.3.8/fab_rk_tools/graphs/mirror_bar.py
--rw-r--r--   0        0        0     8446 2022-08-29 13:24:22.343522 fab-rk-tools-0.3.8/fab_rk_tools/graphs/scatter_quantile_fan.py
--rw-r--r--   0        0        0     3912 2022-08-29 13:24:22.344620 fab-rk-tools-0.3.8/fab_rk_tools/graphs/trafficlight_scatter.py
--rw-r--r--   0        0        0        0 2022-08-03 15:03:48.631234 fab-rk-tools-0.3.8/fab_rk_tools/stats/__init__.py
--rw-r--r--   0        0        0     2953 2022-08-03 15:03:48.632234 fab-rk-tools-0.3.8/fab_rk_tools/stats/distribution.py
--rw-r--r--   0        0        0      549 2022-11-14 15:43:30.610469 fab-rk-tools-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      812 2022-11-14 15:43:37.701846 fab-rk-tools-0.3.8/setup.py
--rw-r--r--   0        0        0      400 2022-11-14 15:43:37.701846 fab-rk-tools-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/__init__.py
+-rw-r--r--   0        0        0       38 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/assets/__init__.py
+-rw-r--r--   0        0        0    20189 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/assets/opt_plotly_theme.py
+-rw-r--r--   0        0        0    12458 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/assets/plotly_theme.py
+-rw-r--r--   0        0        0    14253 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/assets/plotly_theme_to_remove.py
+-rw-r--r--   0        0        0        0 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/common/__init__.py
+-rw-r--r--   0        0        0      265 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/common/constants.py
+-rw-r--r--   0        0        0      671 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/common/utils.py
+-rw-r--r--   0        0        0       57 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/data/__init__.py
+-rw-r--r--   0        0        0     8525 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/data/deriveddata.py
+-rw-r--r--   0        0        0        0 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/data/test/__init__.py
+-rw-r--r--   0        0        0     1060 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/data/test/deriveddata_test.py
+-rw-r--r--   0        0        0        0 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/exceptions/__init__.py
+-rw-r--r--   0        0        0      311 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/exceptions/data.py
+-rw-r--r--   0        0        0      231 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/graphs/__init__.py
+-rw-r--r--   0        0        0     3864 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/graphs/basic_bar.py
+-rw-r--r--   0        0        0     3615 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/graphs/discrete_distro_bar.py
+-rw-r--r--   0        0        0     3580 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/graphs/mirror_bar.py
+-rw-r--r--   0        0        0     8169 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/graphs/scatter_quantile_fan.py
+-rw-r--r--   0        0        0     3773 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/graphs/trafficlight_scatter.py
+-rw-r--r--   0        0        0        0 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/stats/__init__.py
+-rw-r--r--   0        0        0     2846 2022-11-14 15:46:00.988268 fab_rk_tools-0.3.9/fab_rk_tools/stats/distribution.py
+-rw-r--r--   0        0        0      522 2022-11-14 15:46:00.992268 fab_rk_tools-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      822 1970-01-01 00:00:00.000000 fab_rk_tools-0.3.9/setup.py
+-rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 fab_rk_tools-0.3.9/PKG-INFO
```

### Comparing `fab-rk-tools-0.3.8/fab_rk_tools/assets/plotly_theme.py` & `fab_rk_tools-0.3.9/fab_rk_tools/assets/plotly_theme.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,390 +1,390 @@
-import plotly.graph_objects as go
-import plotly.io as pio
-
-# ______________________________________
-# Define themes
-# ______________________________________
-#
-
-DEFAULT_THEME = "dark"
-
-# Themes are defined globally
-
-_theme_def = dict()
-_theme_pallette = dict()
-_theme_element_colours = dict()
-_theme_trafficlight = dict()
-
-#
-# Dark theme pallette and element colours
-#
-
-_theme_def["dark"] = "plotly_dark"
-
-_theme_pallette["dark"] = [
-    "#ff707a",
-    "#ab82e0",
-    "#008fd1",
-    "#ffa600",
-    "#688ce1",
-    "#ff6aa8",
-    "#e374cc",
-    "#ff8749",
-]
-
-_theme_trafficlight["dark"] = dict(
-    GREEN="rgb(74,163,44)",
-    YELLOW="rgb(255,200,32)",
-    RED="rgb(174,32,18)",
-    default="rgb(226,205,141)",
-)
-
-_theme_element_colours["dark"] = dict(
-    bar_below="#BF481D",
-    bar_above="#7CB259",
-    app_background="#222",
-    text="#fafafa",
-    # box_background= "#303030",
-    box_background="#262730",
-    axis="#fafafa",
-    axis_line="#fafafa",
-    grid_line="#777777",
-    spikes="#97aec2",
-    pallette=_theme_pallette["dark"],
-    rangeslider_border="#b1c3d4",
-    rangeslider_bg="#444",
-    now_line="#AAAAAA",
-    button_bg="#444",
-    button_bg_focus="#28415b",
-    endpoint_colour=_theme_pallette["dark"][1],
-    bar_marker_line="#AAAAAA",
-    bar_marker_line_highlight="orange",
-    table_odd_row="#555",
-    table_even_row="#555",
-    table_firstcol_odd="#555",
-    table_firstcol_even="#555",
-    table_header="#444",
-    table_border="#303030",
-)
-
-#
-# light theme pallette and element colours
-#
-
-_theme_def["light"] = "plotly"
-_theme_pallette["light"] = ["#dd7230", "#2e1f27", "#009ec2", "#ecd444", "#90708c"]
-
-_theme_trafficlight["light"] = _theme_trafficlight["dark"].copy()
-
-_theme_element_colours["light"] = dict(
-    bar_below="#BF481D",
-    bar_above="#7CB259",
-    app_background="#FFFFFF",
-    text="#25211E",
-    box_background="#F2F2F2",
-    axis="#25211E",
-    axis_line="#25211E",
-    grid_line="#70645B",
-    spikes="#70645B",
-    now_line="#70645B",
-    pallette=_theme_pallette["light"],
-    rangeslider_border="#b1c3d4",
-    rangeslider_bg="#444",
-    button_bg="#444",
-    button_bg_focus="#28415b",
-    endpoint_colour=_theme_pallette["light"][1],
-    bar_marker_line="#AAAAAA",
-    bar_marker_line_highlight="orange",
-    table_odd_row="#555",
-    table_even_row="#555",
-    table_firstcol_odd="#555",
-    table_firstcol_even="#555",
-    table_header="#444",
-    table_border="#303030",
-)
-
-# ______________________________________
-# Define structure
-# ______________________________________
-#
-# Structure (margins etc) is defined globally
-
-# plot margins
-_plot_margins_default = dict(l=50, r=50, b=50, t=50, pad=4)
-
-_plot_margins_streamlit = dict(l=5, r=5, b=5, t=5, pad=1)
-
-_table_structure_default = dict(
-    width_firstcol=3,
-    width_col=1,
-    cell_height=30,
-    line_width=2,
-    outer_margins=dict(l=20, r=20, b=50, t=50, pad=4),
-)
-
-# ______________________________________
-# Define legends
-# ______________________________________
-#
-# Legend options are defined globally
-# These should be accessed directly by the user/graph functions
-_legend_layout = dict()
-_legend_layout["right_vertical"] = go.Layout(
-    legend=dict(
-        orientation="v", yanchor="top", xanchor="left", x=1.02, y=1, font=dict(size=12)
-    )
-)
-
-_legend_layout["top_right_horizontal"] = go.Layout(
-    legend=dict(
-        orientation="h",
-        yanchor="bottom",
-        xanchor="right",
-        x=1.02,
-        y=1,
-        font=dict(size=12),
-    )
-)
-
-_legend_layout["bottom_centre_horizontal"] = go.Layout(
-    legend=dict(
-        orientation="h",
-        yanchor="top",
-        xanchor="center",
-        x=0.5,
-        y=-0.1,
-        font=dict(size=12),
-    )
-)
-
-# ______________________________________
-# Theme class
-# ______________________________________
-#
-
-
-class FabPlotlyTheme:
-    def __init__(self, graphformat, legendlayout=None, theme=None):
-        theme = theme.lower()
-        graphformat = graphformat.lower()
-
-        # availble stuff
-
-        self.available_themes = list(_theme_def.keys())
-        self.available_legend_layouts = list(_legend_layout.keys())
-
-        # make sure legal theme
-        if theme is None:
-            theme = self.available_themes[0]
-        elif theme not in self.available_themes:
-            msg = "Invalid theme provided. Cannot initialise."
-            raise ValueError(msg)
-
-        # initialise plotly templates (themes)
-        for t, base in _theme_def.items():
-            self._theme_formatting(t, base)
-
-        # set theme
-        self.set_plotly_theme(theme)
-
-        # set graph format
-        self.set_default_graph_format(graphformat=graphformat)
-
-        # set default legend layout
-        self.set_default_legend_layout(legendlayout)
-
-    def set_plotly_theme(self, theme=None):
-        """
-        Set the default theme to use for plotly graphs
-        """
-
-        # make sure legal theme
-        if theme is None:
-            theme = self.available_themes[0]
-        else:
-            theme = theme.lower()
-
-        if theme not in self.available_themes:
-            msg = "Invalid theme provided. Cannot set plotly theme."
-            raise ValueError(msg)
-        pio.templates.default = theme
-        self.active_theme = theme
-        self.pallette = _theme_pallette[theme]
-        self.element_colours = _theme_element_colours[theme]
-        self.trafficlight = _theme_trafficlight[theme]
-        # need to redefine the graph formats so they have the right paper colours
-        self._set_graph_formats()
-        # set legend layouts
-        self.legend_layout = _legend_layout
-
-    def set_default_graph_format(self, graphformat):
-        """
-        Set the (default) graph format (size etc)
-            format => ["standard", "large"]
-
-        You can choose to override these by specifying the formats for specific graphs
-
-        """
-        if graphformat is None:
-            graphformat = self.available_graph_formats[0]
-        else:
-            graphformat = graphformat.lower()
-        if graphformat not in self.available_graph_formats:
-            msg = f"Invalid graph format provided"
-            raise ValueError(msg)
-        self.default_graph_format = self.graph_format[graphformat]
-
-    def set_default_legend_layout(self, legendlayout=None):
-        """
-        Set the (default) legend layout (position etc)
-            format => ["standard", "large"]
-
-        You can choose to override these by specifying the formats for specific graphs
-
-        """
-
-        if legendlayout is None:
-            legendlayout = "right_vertical"
-        else:
-            legendlayout = legendlayout.lower()
-        if legendlayout not in self.available_legend_layouts:
-            msg = f"Invalid graph format provided"
-            raise ValueError(msg)
-        self.default_legend_layout = _legend_layout[legendlayout]
-
-    # ______________________________________
-    # General layout formatting
-    # ______________________________________
-
-    def _theme_formatting(self, theme, base_theme):
-        # make sure legal theme
-        if theme not in self.available_themes:
-            msg = "Invalid theme provided. Cannot initialise."
-            raise ValueError(msg)
-
-        pio.templates[theme] = pio.templates[base_theme]
-        this_theme = pio.templates[theme]
-        this_element_colours = _theme_element_colours[theme]
-
-        # plot background
-        this_theme["layout"]["paper_bgcolor"] = this_element_colours["box_background"]
-        this_theme["layout"]["plot_bgcolor"] = this_element_colours["box_background"]
-
-        # axes. Here use the color property to set everything at once. Maybe control finer later.
-        this_theme["layout"]["xaxis"]["color"] = this_element_colours["axis"]
-        this_theme["layout"]["yaxis"]["color"] = this_element_colours["axis"]
-        this_theme["layout"]["xaxis"]["linecolor"] = this_element_colours["axis"]
-        this_theme["layout"]["yaxis"]["linecolor"] = this_element_colours["axis"]
-        this_theme["layout"]["xaxis"]["linewidth"] = 1
-        this_theme["layout"]["yaxis"]["linewidth"] = 1
-        this_theme["layout"]["xaxis"]["showline"] = True
-        this_theme["layout"]["yaxis"]["showline"] = True
-        this_theme.layout.xaxis.type = "-"
-
-        # xaxis rangeslider formatting
-        this_theme.layout.xaxis.rangeslider.visible = False
-        this_theme.layout.xaxis.rangeslider.borderwidth = 0
-        this_theme.layout.xaxis.rangeslider.bordercolor = this_element_colours[
-            "rangeslider_border"
-        ]
-        this_theme.layout.xaxis.rangeslider.thickness = 0.20
-        this_theme.layout.xaxis.rangeslider.bgcolor = this_element_colours[
-            "rangeslider_bg"
-        ]
-
-        # xaxis rangeselector formatting
-        this_theme.layout.xaxis.rangeselector.visible = False
-        this_theme.layout.xaxis.rangeselector.font.color = this_element_colours["text"]
-        this_theme.layout.xaxis.rangeselector.bgcolor = this_element_colours[
-            "button_bg"
-        ]
-        this_theme.layout.xaxis.rangeselector.activecolor = this_element_colours[
-            "button_bg"
-        ]
-        this_theme.layout.xaxis.rangeselector.borderwidth = 0
-
-        # axis spikes
-        this_theme["layout"]["yaxis"]["showspikes"] = False
-        this_theme["layout"]["xaxis"]["showspikes"] = True
-        this_theme["layout"]["xaxis"]["spikethickness"] = 1
-        this_theme["layout"]["xaxis"]["spikedash"] = "dot"
-        this_theme.layout.xaxis.spikesnap = "data"
-        this_theme["layout"]["xaxis"]["spikecolor"] = this_element_colours["spikes"]
-        this_theme.layout.spikedistance = 5000
-
-        # grid
-        this_theme["layout"]["yaxis"]["gridcolor"] = this_element_colours["grid_line"]
-        this_theme["layout"]["yaxis"]["showgrid"] = True
-        this_theme["layout"]["xaxis"]["showgrid"] = False
-
-        # get rid of zerolines
-        this_theme["layout"]["xaxis"]["zeroline"] = False
-        this_theme["layout"]["yaxis"]["zeroline"] = False
-
-        # margin
-        # this_theme.layout.margin = _plot_margins_default
-        this_theme.layout.margin = _plot_margins_default
-
-        # hover
-        this_theme.layout.hovermode = "x"
-        this_theme.layout.xaxis.hoverformat = "%{x:.2f}"
-        this_theme.layout.hoverdistance = 100
-
-        # graph series colours
-        this_theme.layout.colorway = this_element_colours["pallette"]
-
-        # Plot-type specific formatting
-
-        # scatter plots
-        this_theme.data.scatter = [
-            go.Scatter(
-                hovertemplate="%{y:.2f}",
-                line=dict(shape="linear", dash="solid", width=1),
-            )
-        ]
-
-        # bar plots
-        # this_theme.layout.barmode='stack'
-        this_theme.layout.bargap = 0.1
-        this_theme.data.bar = [
-            go.Bar(
-                # hovertemplate="%{y:.2f}<extra></extra>",
-                hovertemplate="%{y:.2f}",
-                marker=dict(opacity=0.9, line={"width": 1}),
-            )
-        ]
-
-        # tables
-        this_theme.data.table = [go.Table(hoverinfo="x+y")]
-
-    # ______________________________________
-    # Graph formats
-    # ______________________________________
-    #
-    # These are NOT defined as globals, as we have to overwrite the paper colours
-    # if we update the theme (as streamlit will overwrite them otherwise)
-
-    def _set_graph_formats(self):
-
-        self.graph_format = dict()
-        this_element_colours = _theme_element_colours[self.active_theme]
-
-        self.graph_format["standard"] = go.Layout(
-            # height = 300,
-            xaxis=dict(tickfont={"size": 12}, titlefont={"size": 12}),
-            yaxis=dict(tickfont={"size": 12}, titlefont={"size": 12}),
-            # have to explicitly specify the paper colours since streamlit overwrites the theme
-            # paper_bgcolor=this_element_colours["box_background"],
-            # plot_bgcolor=this_element_colours["box_background"]
-        )
-
-        self.graph_format["large"] = go.Layout(
-            height=350,
-            xaxis=dict(tickfont={"size": 12}, titlefont={"size": 12}),
-            yaxis=dict(tickfont={"size": 12}, titlefont={"size": 12}),
-            # have to explicitly specify the paper colours since streamlit overwrites the theme
-            # paper_bgcolor=this_element_colours["box_background"],
-            # plot_bgcolor=this_element_colours["box_background"]
-        )
-
-        self.available_graph_formats = self.graph_format.keys()
+import plotly.graph_objects as go
+import plotly.io as pio
+
+# ______________________________________
+# Define themes
+# ______________________________________
+#
+
+DEFAULT_THEME = "dark"
+
+# Themes are defined globally
+
+_theme_def = dict()
+_theme_pallette = dict()
+_theme_element_colours = dict()
+_theme_trafficlight = dict()
+
+#
+# Dark theme pallette and element colours
+#
+
+_theme_def["dark"] = "plotly_dark"
+
+_theme_pallette["dark"] = [
+    "#ff707a",
+    "#ab82e0",
+    "#008fd1",
+    "#ffa600",
+    "#688ce1",
+    "#ff6aa8",
+    "#e374cc",
+    "#ff8749",
+]
+
+_theme_trafficlight["dark"] = dict(
+    GREEN="rgb(74,163,44)",
+    YELLOW="rgb(255,200,32)",
+    RED="rgb(174,32,18)",
+    default="rgb(226,205,141)",
+)
+
+_theme_element_colours["dark"] = dict(
+    bar_below="#BF481D",
+    bar_above="#7CB259",
+    app_background="#222",
+    text="#fafafa",
+    # box_background= "#303030",
+    box_background="#262730",
+    axis="#fafafa",
+    axis_line="#fafafa",
+    grid_line="#777777",
+    spikes="#97aec2",
+    pallette=_theme_pallette["dark"],
+    rangeslider_border="#b1c3d4",
+    rangeslider_bg="#444",
+    now_line="#AAAAAA",
+    button_bg="#444",
+    button_bg_focus="#28415b",
+    endpoint_colour=_theme_pallette["dark"][1],
+    bar_marker_line="#AAAAAA",
+    bar_marker_line_highlight="orange",
+    table_odd_row="#555",
+    table_even_row="#555",
+    table_firstcol_odd="#555",
+    table_firstcol_even="#555",
+    table_header="#444",
+    table_border="#303030",
+)
+
+#
+# light theme pallette and element colours
+#
+
+_theme_def["light"] = "plotly"
+_theme_pallette["light"] = ["#dd7230", "#2e1f27", "#009ec2", "#ecd444", "#90708c"]
+
+_theme_trafficlight["light"] = _theme_trafficlight["dark"].copy()
+
+_theme_element_colours["light"] = dict(
+    bar_below="#BF481D",
+    bar_above="#7CB259",
+    app_background="#FFFFFF",
+    text="#25211E",
+    box_background="#F2F2F2",
+    axis="#25211E",
+    axis_line="#25211E",
+    grid_line="#70645B",
+    spikes="#70645B",
+    now_line="#70645B",
+    pallette=_theme_pallette["light"],
+    rangeslider_border="#b1c3d4",
+    rangeslider_bg="#444",
+    button_bg="#444",
+    button_bg_focus="#28415b",
+    endpoint_colour=_theme_pallette["light"][1],
+    bar_marker_line="#AAAAAA",
+    bar_marker_line_highlight="orange",
+    table_odd_row="#555",
+    table_even_row="#555",
+    table_firstcol_odd="#555",
+    table_firstcol_even="#555",
+    table_header="#444",
+    table_border="#303030",
+)
+
+# ______________________________________
+# Define structure
+# ______________________________________
+#
+# Structure (margins etc) is defined globally
+
+# plot margins
+_plot_margins_default = dict(l=50, r=50, b=50, t=50, pad=4)
+
+_plot_margins_streamlit = dict(l=5, r=5, b=5, t=5, pad=1)
+
+_table_structure_default = dict(
+    width_firstcol=3,
+    width_col=1,
+    cell_height=30,
+    line_width=2,
+    outer_margins=dict(l=20, r=20, b=50, t=50, pad=4),
+)
+
+# ______________________________________
+# Define legends
+# ______________________________________
+#
+# Legend options are defined globally
+# These should be accessed directly by the user/graph functions
+_legend_layout = dict()
+_legend_layout["right_vertical"] = go.Layout(
+    legend=dict(
+        orientation="v", yanchor="top", xanchor="left", x=1.02, y=1, font=dict(size=12)
+    )
+)
+
+_legend_layout["top_right_horizontal"] = go.Layout(
+    legend=dict(
+        orientation="h",
+        yanchor="bottom",
+        xanchor="right",
+        x=1.02,
+        y=1,
+        font=dict(size=12),
+    )
+)
+
+_legend_layout["bottom_centre_horizontal"] = go.Layout(
+    legend=dict(
+        orientation="h",
+        yanchor="top",
+        xanchor="center",
+        x=0.5,
+        y=-0.1,
+        font=dict(size=12),
+    )
+)
+
+# ______________________________________
+# Theme class
+# ______________________________________
+#
+
+
+class FabPlotlyTheme:
+    def __init__(self, graphformat, legendlayout=None, theme=None):
+        theme = theme.lower()
+        graphformat = graphformat.lower()
+
+        # availble stuff
+
+        self.available_themes = list(_theme_def.keys())
+        self.available_legend_layouts = list(_legend_layout.keys())
+
+        # make sure legal theme
+        if theme is None:
+            theme = self.available_themes[0]
+        elif theme not in self.available_themes:
+            msg = "Invalid theme provided. Cannot initialise."
+            raise ValueError(msg)
+
+        # initialise plotly templates (themes)
+        for t, base in _theme_def.items():
+            self._theme_formatting(t, base)
+
+        # set theme
+        self.set_plotly_theme(theme)
+
+        # set graph format
+        self.set_default_graph_format(graphformat=graphformat)
+
+        # set default legend layout
+        self.set_default_legend_layout(legendlayout)
+
+    def set_plotly_theme(self, theme=None):
+        """
+        Set the default theme to use for plotly graphs
+        """
+
+        # make sure legal theme
+        if theme is None:
+            theme = self.available_themes[0]
+        else:
+            theme = theme.lower()
+
+        if theme not in self.available_themes:
+            msg = "Invalid theme provided. Cannot set plotly theme."
+            raise ValueError(msg)
+        pio.templates.default = theme
+        self.active_theme = theme
+        self.pallette = _theme_pallette[theme]
+        self.element_colours = _theme_element_colours[theme]
+        self.trafficlight = _theme_trafficlight[theme]
+        # need to redefine the graph formats so they have the right paper colours
+        self._set_graph_formats()
+        # set legend layouts
+        self.legend_layout = _legend_layout
+
+    def set_default_graph_format(self, graphformat):
+        """
+        Set the (default) graph format (size etc)
+            format => ["standard", "large"]
+
+        You can choose to override these by specifying the formats for specific graphs
+
+        """
+        if graphformat is None:
+            graphformat = self.available_graph_formats[0]
+        else:
+            graphformat = graphformat.lower()
+        if graphformat not in self.available_graph_formats:
+            msg = f"Invalid graph format provided"
+            raise ValueError(msg)
+        self.default_graph_format = self.graph_format[graphformat]
+
+    def set_default_legend_layout(self, legendlayout=None):
+        """
+        Set the (default) legend layout (position etc)
+            format => ["standard", "large"]
+
+        You can choose to override these by specifying the formats for specific graphs
+
+        """
+
+        if legendlayout is None:
+            legendlayout = "right_vertical"
+        else:
+            legendlayout = legendlayout.lower()
+        if legendlayout not in self.available_legend_layouts:
+            msg = f"Invalid graph format provided"
+            raise ValueError(msg)
+        self.default_legend_layout = _legend_layout[legendlayout]
+
+    # ______________________________________
+    # General layout formatting
+    # ______________________________________
+
+    def _theme_formatting(self, theme, base_theme):
+        # make sure legal theme
+        if theme not in self.available_themes:
+            msg = "Invalid theme provided. Cannot initialise."
+            raise ValueError(msg)
+
+        pio.templates[theme] = pio.templates[base_theme]
+        this_theme = pio.templates[theme]
+        this_element_colours = _theme_element_colours[theme]
+
+        # plot background
+        this_theme["layout"]["paper_bgcolor"] = this_element_colours["box_background"]
+        this_theme["layout"]["plot_bgcolor"] = this_element_colours["box_background"]
+
+        # axes. Here use the color property to set everything at once. Maybe control finer later.
+        this_theme["layout"]["xaxis"]["color"] = this_element_colours["axis"]
+        this_theme["layout"]["yaxis"]["color"] = this_element_colours["axis"]
+        this_theme["layout"]["xaxis"]["linecolor"] = this_element_colours["axis"]
+        this_theme["layout"]["yaxis"]["linecolor"] = this_element_colours["axis"]
+        this_theme["layout"]["xaxis"]["linewidth"] = 1
+        this_theme["layout"]["yaxis"]["linewidth"] = 1
+        this_theme["layout"]["xaxis"]["showline"] = True
+        this_theme["layout"]["yaxis"]["showline"] = True
+        this_theme.layout.xaxis.type = "-"
+
+        # xaxis rangeslider formatting
+        this_theme.layout.xaxis.rangeslider.visible = False
+        this_theme.layout.xaxis.rangeslider.borderwidth = 0
+        this_theme.layout.xaxis.rangeslider.bordercolor = this_element_colours[
+            "rangeslider_border"
+        ]
+        this_theme.layout.xaxis.rangeslider.thickness = 0.20
+        this_theme.layout.xaxis.rangeslider.bgcolor = this_element_colours[
+            "rangeslider_bg"
+        ]
+
+        # xaxis rangeselector formatting
+        this_theme.layout.xaxis.rangeselector.visible = False
+        this_theme.layout.xaxis.rangeselector.font.color = this_element_colours["text"]
+        this_theme.layout.xaxis.rangeselector.bgcolor = this_element_colours[
+            "button_bg"
+        ]
+        this_theme.layout.xaxis.rangeselector.activecolor = this_element_colours[
+            "button_bg"
+        ]
+        this_theme.layout.xaxis.rangeselector.borderwidth = 0
+
+        # axis spikes
+        this_theme["layout"]["yaxis"]["showspikes"] = False
+        this_theme["layout"]["xaxis"]["showspikes"] = True
+        this_theme["layout"]["xaxis"]["spikethickness"] = 1
+        this_theme["layout"]["xaxis"]["spikedash"] = "dot"
+        this_theme.layout.xaxis.spikesnap = "data"
+        this_theme["layout"]["xaxis"]["spikecolor"] = this_element_colours["spikes"]
+        this_theme.layout.spikedistance = 5000
+
+        # grid
+        this_theme["layout"]["yaxis"]["gridcolor"] = this_element_colours["grid_line"]
+        this_theme["layout"]["yaxis"]["showgrid"] = True
+        this_theme["layout"]["xaxis"]["showgrid"] = False
+
+        # get rid of zerolines
+        this_theme["layout"]["xaxis"]["zeroline"] = False
+        this_theme["layout"]["yaxis"]["zeroline"] = False
+
+        # margin
+        # this_theme.layout.margin = _plot_margins_default
+        this_theme.layout.margin = _plot_margins_default
+
+        # hover
+        this_theme.layout.hovermode = "x"
+        this_theme.layout.xaxis.hoverformat = "%{x:.2f}"
+        this_theme.layout.hoverdistance = 100
+
+        # graph series colours
+        this_theme.layout.colorway = this_element_colours["pallette"]
+
+        # Plot-type specific formatting
+
+        # scatter plots
+        this_theme.data.scatter = [
+            go.Scatter(
+                hovertemplate="%{y:.2f}",
+                line=dict(shape="linear", dash="solid", width=1),
+            )
+        ]
+
+        # bar plots
+        # this_theme.layout.barmode='stack'
+        this_theme.layout.bargap = 0.1
+        this_theme.data.bar = [
+            go.Bar(
+                # hovertemplate="%{y:.2f}<extra></extra>",
+                hovertemplate="%{y:.2f}",
+                marker=dict(opacity=0.9, line={"width": 1}),
+            )
+        ]
+
+        # tables
+        this_theme.data.table = [go.Table(hoverinfo="x+y")]
+
+    # ______________________________________
+    # Graph formats
+    # ______________________________________
+    #
+    # These are NOT defined as globals, as we have to overwrite the paper colours
+    # if we update the theme (as streamlit will overwrite them otherwise)
+
+    def _set_graph_formats(self):
+
+        self.graph_format = dict()
+        this_element_colours = _theme_element_colours[self.active_theme]
+
+        self.graph_format["standard"] = go.Layout(
+            # height = 300,
+            xaxis=dict(tickfont={"size": 12}, titlefont={"size": 12}),
+            yaxis=dict(tickfont={"size": 12}, titlefont={"size": 12}),
+            # have to explicitly specify the paper colours since streamlit overwrites the theme
+            # paper_bgcolor=this_element_colours["box_background"],
+            # plot_bgcolor=this_element_colours["box_background"]
+        )
+
+        self.graph_format["large"] = go.Layout(
+            height=350,
+            xaxis=dict(tickfont={"size": 12}, titlefont={"size": 12}),
+            yaxis=dict(tickfont={"size": 12}, titlefont={"size": 12}),
+            # have to explicitly specify the paper colours since streamlit overwrites the theme
+            # paper_bgcolor=this_element_colours["box_background"],
+            # plot_bgcolor=this_element_colours["box_background"]
+        )
+
+        self.available_graph_formats = self.graph_format.keys()
```

### Comparing `fab-rk-tools-0.3.8/fab_rk_tools/assets/plotly_theme_to_remove.py` & `fab_rk_tools-0.3.9/fab_rk_tools/assets/plotly_theme_to_remove.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,409 +1,409 @@
-"""
-docstring
-"""
-import json
-import logging
-
-import pandas as pd
-import plotly.io as pio
-
-logging.basicConfig(level=logging.INFO)
-
-# ______________________________________
-# Define themes
-# ______________________________________
-#
-
-DEFAULT_COLOUR_THEME = "dark"
-DEFAULT_DESIGN_THEME = "optidesign"
-DEFAULT_PIO_THEME = "plotly_dark"  # base theme from pio to base everything on
-OPTIMEERING_THEME = "optitheme"  # name to use in pio. Doesnt matter what it is.
-
-# defaul theme definition
-
-DEFAULT_COLOUR_THEME_JSON = """{
-    "colors": [
-        {"name":"blue_dark","hex":"#415B8C","rgb":"65, 91, 140"},
-        {"name":"blue_mid","hex":"#799BD9","rgb":"121, 155, 217"},
-        {"name":"blue_light","hex":"#BFCFED","rgb":"191, 207, 237"},
-        {"name":"lime_light","hex":"#B5D964","rgb":"181, 217, 100"},
-        {"name":"green_mid","hex":"#9CB36B","rgb":"119, 140, 72"},
-        {"name":"green_dark","hex":"#778C48","rgb":"119, 140, 72"},
-        {"name":"dusky_light","hex":"#D99A8F","rgb":"217, 154, 143"},
-        {"name":"dusky_mid","hex":"#C15B49","rgb":"137, 60, 47"},
-        {"name":"dusky_dark","hex":"#A74A39","rgb":"137, 60, 47"},
-        {"name":"yellow_mid","hex":"#F6DE50","rgb":"137, 60, 47"},
-        {"name":"blue_very_dark","hex":"#0D121C","rgb":"13, 18, 28"},
-        {"name":"off_white","hex":"#F7F8FA","rgb":"247, 248, 250"}
-    ],
-    "roles": {
-        "box_background": "blue_very_dark",
-        "primary_text": "off_white",
-        "graph_sequence": ["blue_mid", "lime_light", "dusky_light", "green_dark", 
-            "blue_light", "dusky_dark", "blue_dark"],
-        "axis": "off_white",
-        "grid_line": "off_white",
-        "spikes": "off_white",
-        "trafficlight": {
-            "GREEN": "green_mid",
-            "YELLOW": "yellow_mid",
-            "RED": "dusky_dark",
-            "default": "blue_mid"
-        }
-    }
-    
-}"""
-
-# default theme structure JSON
-
-DEFAULT_DESIGN_THEME_JSON = """
-{
-    "layout": {
-        "height": 350, 
-        "xaxis": {
-            "tickfont": {
-                "size": 12
-            },
-            "titlefont": {
-                "size": 12
-            }, 
-            "linewidth": 1, 
-            "showline": true, 
-            "type": "-", 
-            "showspikes": true, 
-            "spikethickness": 1, 
-            "spikedash": "dot", 
-            "spikesnap": "data", 
-            "showgrid": false, 
-            "zeroline": false, 
-            "hoverformat": "%{x:.2f}"
-        }, 
-        "yaxis": {
-            "tickfont": {
-                "size": 12
-            }, 
-            "titlefont": {
-                "size": 12
-            }, 
-            "linewidth": 1, 
-            "showline": true, 
-            "showspikes": false, 
-            "showgrid": true, 
-            "zeroline": false,
-            "nticks": 8
-        }, 
-        "spikedistance": 5000, 
-        "bargap": 0.1, 
-        "margin": {
-            "l": 50, 
-            "r": 50, 
-            "b": 50, 
-            "t": 50,
-            "pad": 4
-        }, 
-        "hovermode": "x", 
-        "hoverdistance": 100, 
-        "legend": {
-            "orientation": "v", 
-            "yanchor": "top", 
-            "xanchor": "left", 
-            "x": 1.02, 
-            "y": 1, 
-            "font_size": 12
-        }
-    },
-    "data": {
-        "bar": {
-            "hovertemplate": "%{y:.2f}",
-            "marker": {
-                "opacity": 0.9,
-                "line": {
-                    "width": 1
-                }
-            }
-        },
-        "table": {
-            "hoverinfo": "x+y"
-        },
-        "scatter": {
-            "hovertemplate":"%{y:.2f}",
-            "line": {
-                "shape": "linear",
-                "dash": "solid",
-                "width": 1
-            }
-        }
-    }
-}
-"""
-# ______________________________________
-# Theme class
-# ______________________________________
-#
-
-
-class FabPlotlyTheme:
-    """
-    Depreciated FabPLotlyTheme - do not use this. Rather import opt_plotly_theme instead
-    """
-
-    # pylint: disable=too-many-instance-attributes
-
-    def __init__(
-        self, colour_theme=None, design_theme_adjustments=None, base_theme=None
-    ):
-
-        logging.warning(
-            (
-                "plotly_theme is depreciated, and will be removed in an upcoming "
-                "version of fab_rk_tools. Use opt_plotly_theme instead."
-            )
-        )
-
-        # actives are none at start
-        self.active_base_theme = None
-        self.active_colour_theme = None
-        self.active_design_theme_adjustments = None
-        self._colour_theme_dict = None
-        self._colour_theme_json = None
-        self._colour_theme_name = None
-        self._colours_df = None
-        self._colours_graph = None
-        self._colours_trafficlight_hex = None
-        self._colours_trafficlight_rgb = None
-        self._colours_elements = None
-        self._design_theme_dict = None
-        self._design_theme_json = None
-        self._design_theme_name = None
-        self._colours_graphs = None
-
-        # load the inbuilt colour and design adjustment themes
-        self._colour_theme_json = {}
-        self._design_theme_json = {}
-        # availble stuff
-        self.available_colour_themes = []
-        self.available_design_theme_adjustments = []
-        # load the defaults so we have at least these
-        self.load_colour_theme(
-            colour_theme=DEFAULT_COLOUR_THEME,
-            colour_theme_json=DEFAULT_COLOUR_THEME_JSON,
-        )
-        self.load_design_theme_adjustments(
-            design_theme=DEFAULT_DESIGN_THEME,
-            design_theme_json=DEFAULT_DESIGN_THEME_JSON,
-        )
-
-        # set themes to defualts if none selected
-        if colour_theme is None:
-            colour_theme = DEFAULT_COLOUR_THEME
-        if design_theme_adjustments is None:
-            design_theme_adjustments = DEFAULT_DESIGN_THEME
-
-        # activate the theme, using the defualts where these are not selected
-
-        self.activate_theme(
-            colour_theme=colour_theme,
-            design_theme_adjustments=design_theme_adjustments,
-            base_theme=base_theme,
-        )
-
-    def load_colour_theme(self, colour_theme, colour_theme_json):
-        """
-        Load in a new colour theme
-
-        colour_theme_name: str, name of the new theme
-        colour_theme_json: json, json definition of the theme colours.
-
-        """
-
-        # at some stage we shoudl error check the json
-        self._colour_theme_json[colour_theme] = colour_theme_json
-        # availble stuff
-        self.available_colour_themes.append(DEFAULT_COLOUR_THEME)
-
-    def load_design_theme_adjustments(self, design_theme, design_theme_json):
-        """
-        docstring
-        """
-        self._design_theme_json[design_theme] = design_theme_json
-        # availble stuff
-        self.available_design_theme_adjustments.append(DEFAULT_DESIGN_THEME)
-
-    def _set_colour_theme(self, colour_theme):
-        """
-        Set one of the loaded colour themes to be the colour theme we use
-        """
-        # make sure legal colour theme
-        if colour_theme is None:
-            colour_theme = DEFAULT_COLOUR_THEME
-        colour_theme = colour_theme.lower()
-
-        if colour_theme not in self.available_colour_themes:
-            msg = "Invalid colour theme provided. Cannot set plotly colour theme."
-            raise ValueError(msg)
-
-        # convert colour theme json to dict
-        self._colour_theme_name = colour_theme
-        self._colour_theme_dict = json.loads(self._colour_theme_json[colour_theme])
-
-        # store colours in a dataframe
-        self._colours_df = pd.DataFrame(self._colour_theme_dict["colors"])
-        self._colours_df = self._colours_df.set_index("name")
-
-        # set up a list with graph colours in order
-        gphseq = self._colour_theme_dict["roles"]["graph_sequence"]
-        self._colours_graphs = list(self._colours_df.loc[gphseq].hex)
-
-        # traffic light graph colours
-        tlight = self._colour_theme_dict["roles"]["trafficlight"]
-        self._colours_trafficlight_rgb = {}
-        self._colours_trafficlight_hex = {}
-        for light, colour in tlight.items():
-            self._colours_trafficlight_rgb[
-                light.upper()
-            ] = f"rgb({self._colours_df.loc[colour].rgb})"
-            self._colours_trafficlight_hex[light.upper()] = self._colours_df.loc[
-                colour
-            ].hex
-
-        # set up element colours
-        self._colours_elements = dict(
-            box_background=self._colours_df.loc[
-                self._colour_theme_dict["roles"]["box_background"]
-            ].hex,
-            axis=self._colours_df.loc[self._colour_theme_dict["roles"]["axis"]].hex,
-            spikes=self._colours_df.loc[self._colour_theme_dict["roles"]["spikes"]].hex,
-            grid_line=self._colours_df.loc[
-                self._colour_theme_dict["roles"]["grid_line"]
-            ].hex,
-            primary_text=self._colours_df.loc[
-                self._colour_theme_dict["roles"]["primary_text"]
-            ].hex,
-        )
-
-    def _set_design_theme_adjustments(self, design_theme):
-        """
-        Define the formatting/design adjustments for the theme
-        These will replace/overwrite those of any base pio theme selected
-        """
-        # make sure legal colour theme
-        if design_theme is None:
-            design_theme = DEFAULT_DESIGN_THEME
-        design_theme = design_theme.lower()
-
-        if design_theme not in self.available_design_theme_adjustments:
-            msg = (
-                "Invalid design theme provided. Cannot set make the design adjustments."
-            )
-            raise ValueError(msg)
-
-        # record the design theme name
-        self._design_theme_name = design_theme
-        self._design_theme_dict = json.loads(self._design_theme_json[design_theme])
-
-        # margins
-        # self._plot_margins = self._design_theme_dict["plot"]["margins"]
-        # self._streamlit_plot_margins =
-        #       self._design_theme_dict["plot"]["margins_streamlit"]
-
-        # table
-        # self._table_formatting = self._design_theme_dict["table"]
-
-        # specific formatting components
-
-        # legend
-        # if "legend_layout" in self._design_theme_dict:
-        # self._legend_layout = go.Layout(
-        #               legend =
-        #                   self._design_theme_dict["legend_layout"])
-        #    self._legend_layout = self._design_theme_dict["legend_layout"]
-        # else:
-        #    self._legend_layout = go.Layout()
-
-        # graph format
-        # if "graph_format" in self._design_theme_dict:
-        #    self._graph_format = go.Layout(self._design_theme_dict["graph_format"])
-        # else:
-        #    self._graph_format = go.Layout()
-
-    def activate_theme(
-        self,
-        base_theme=None,
-        colour_theme=None,
-        design_theme_adjustments=None,
-    ):
-        """
-        Activate the theming for the plotly graphs
-
-        Uses the currently set colour and design theme adjustments
-        and legend layout and applies these to the base_theme (if
-        base_theme=None, then uses the default base theme)
-        """
-
-        # make sure legal theme
-        if base_theme is None:
-            base_theme = DEFAULT_PIO_THEME
-        base_theme = base_theme.lower()
-
-        # set the various theme parts as selected (otherwise the
-        # already loaded ones will be used)
-        # Note - we skip "None" so that the user can easily
-        # adjust one of the theme components
-        if colour_theme is not None:
-            self._set_colour_theme(colour_theme)
-        if design_theme_adjustments is not None:
-            self._set_design_theme_adjustments(design_theme_adjustments)
-
-        # store the active base theme, colour and design theme adjustments in use
-        # Note: they are not activated until they are run though
-        # here - so they can be "_set_" but
-        # they wont be used until they are activated with this function
-        self.active_base_theme = base_theme
-        self.active_colour_theme = self._colour_theme_name
-        self.active_design_theme_adjustments = self._design_theme_name
-
-        # store the parts of the theme the user/graphs will want to access directly
-        self.pallette = self._colours_graphs
-        self.trafficlight_rgb = self._colours_trafficlight_rgb
-        self.trafficlight_hex = self._colours_trafficlight_hex
-        # self.legend_layout = self._legend_layout
-        # self.graph_format = self._graph_format
-
-        # load the base theme from pio
-        self._pio_template = pio.templates[base_theme]
-
-        # make changes to the base theme
-        self._format_theme()
-
-        # create/overwrite the optimeering theme in pio & set it as the default
-        pio.templates[OPTIMEERING_THEME] = self._pio_template
-        pio.templates.default = OPTIMEERING_THEME
-
-    # ______________________________________
-    # General layout formatting
-    # ______________________________________
-
-    def _format_theme(self):
-
-        this_theme = self._pio_template  # shorthand
-
-        # set the structural (design) formatting
-        # ======================================
-        this_theme = this_theme.update(self._design_theme_dict)
-
-        # set the colour theme formatting
-        # ================================
-        # plot background
-        this_theme["layout"]["paper_bgcolor"] = self._colours_elements["box_background"]
-        this_theme["layout"]["plot_bgcolor"] = self._colours_elements["box_background"]
-
-        # axes. Here use the color property to set everything at once.
-        # Maybe control finer later.
-        this_theme["layout"]["xaxis"]["color"] = self._colours_elements["axis"]
-        this_theme["layout"]["yaxis"]["color"] = self._colours_elements["axis"]
-        this_theme["layout"]["xaxis"]["spikecolor"] = self._colours_elements["spikes"]
-        this_theme["layout"]["xaxis"]["linecolor"] = self._colours_elements["axis"]
-        this_theme["layout"]["yaxis"]["linecolor"] = self._colours_elements["axis"]
-        this_theme["layout"]["yaxis"]["gridcolor"] = self._colours_elements["grid_line"]
-        # graph series colours
-        this_theme.layout.colorway = self._colours_graphs
+"""
+docstring
+"""
+import json
+import logging
+
+import pandas as pd
+import plotly.io as pio
+
+logging.basicConfig(level=logging.INFO)
+
+# ______________________________________
+# Define themes
+# ______________________________________
+#
+
+DEFAULT_COLOUR_THEME = "dark"
+DEFAULT_DESIGN_THEME = "optidesign"
+DEFAULT_PIO_THEME = "plotly_dark"  # base theme from pio to base everything on
+OPTIMEERING_THEME = "optitheme"  # name to use in pio. Doesnt matter what it is.
+
+# defaul theme definition
+
+DEFAULT_COLOUR_THEME_JSON = """{
+    "colors": [
+        {"name":"blue_dark","hex":"#415B8C","rgb":"65, 91, 140"},
+        {"name":"blue_mid","hex":"#799BD9","rgb":"121, 155, 217"},
+        {"name":"blue_light","hex":"#BFCFED","rgb":"191, 207, 237"},
+        {"name":"lime_light","hex":"#B5D964","rgb":"181, 217, 100"},
+        {"name":"green_mid","hex":"#9CB36B","rgb":"119, 140, 72"},
+        {"name":"green_dark","hex":"#778C48","rgb":"119, 140, 72"},
+        {"name":"dusky_light","hex":"#D99A8F","rgb":"217, 154, 143"},
+        {"name":"dusky_mid","hex":"#C15B49","rgb":"137, 60, 47"},
+        {"name":"dusky_dark","hex":"#A74A39","rgb":"137, 60, 47"},
+        {"name":"yellow_mid","hex":"#F6DE50","rgb":"137, 60, 47"},
+        {"name":"blue_very_dark","hex":"#0D121C","rgb":"13, 18, 28"},
+        {"name":"off_white","hex":"#F7F8FA","rgb":"247, 248, 250"}
+    ],
+    "roles": {
+        "box_background": "blue_very_dark",
+        "primary_text": "off_white",
+        "graph_sequence": ["blue_mid", "lime_light", "dusky_light", "green_dark", 
+            "blue_light", "dusky_dark", "blue_dark"],
+        "axis": "off_white",
+        "grid_line": "off_white",
+        "spikes": "off_white",
+        "trafficlight": {
+            "GREEN": "green_mid",
+            "YELLOW": "yellow_mid",
+            "RED": "dusky_dark",
+            "default": "blue_mid"
+        }
+    }
+    
+}"""
+
+# default theme structure JSON
+
+DEFAULT_DESIGN_THEME_JSON = """
+{
+    "layout": {
+        "height": 350, 
+        "xaxis": {
+            "tickfont": {
+                "size": 12
+            },
+            "titlefont": {
+                "size": 12
+            }, 
+            "linewidth": 1, 
+            "showline": true, 
+            "type": "-", 
+            "showspikes": true, 
+            "spikethickness": 1, 
+            "spikedash": "dot", 
+            "spikesnap": "data", 
+            "showgrid": false, 
+            "zeroline": false, 
+            "hoverformat": "%{x:.2f}"
+        }, 
+        "yaxis": {
+            "tickfont": {
+                "size": 12
+            }, 
+            "titlefont": {
+                "size": 12
+            }, 
+            "linewidth": 1, 
+            "showline": true, 
+            "showspikes": false, 
+            "showgrid": true, 
+            "zeroline": false,
+            "nticks": 8
+        }, 
+        "spikedistance": 5000, 
+        "bargap": 0.1, 
+        "margin": {
+            "l": 50, 
+            "r": 50, 
+            "b": 50, 
+            "t": 50,
+            "pad": 4
+        }, 
+        "hovermode": "x", 
+        "hoverdistance": 100, 
+        "legend": {
+            "orientation": "v", 
+            "yanchor": "top", 
+            "xanchor": "left", 
+            "x": 1.02, 
+            "y": 1, 
+            "font_size": 12
+        }
+    },
+    "data": {
+        "bar": {
+            "hovertemplate": "%{y:.2f}",
+            "marker": {
+                "opacity": 0.9,
+                "line": {
+                    "width": 1
+                }
+            }
+        },
+        "table": {
+            "hoverinfo": "x+y"
+        },
+        "scatter": {
+            "hovertemplate":"%{y:.2f}",
+            "line": {
+                "shape": "linear",
+                "dash": "solid",
+                "width": 1
+            }
+        }
+    }
+}
+"""
+# ______________________________________
+# Theme class
+# ______________________________________
+#
+
+
+class FabPlotlyTheme:
+    """
+    Depreciated FabPLotlyTheme - do not use this. Rather import opt_plotly_theme instead
+    """
+
+    # pylint: disable=too-many-instance-attributes
+
+    def __init__(
+        self, colour_theme=None, design_theme_adjustments=None, base_theme=None
+    ):
+
+        logging.warning(
+            (
+                "plotly_theme is depreciated, and will be removed in an upcoming "
+                "version of fab_rk_tools. Use opt_plotly_theme instead."
+            )
+        )
+
+        # actives are none at start
+        self.active_base_theme = None
+        self.active_colour_theme = None
+        self.active_design_theme_adjustments = None
+        self._colour_theme_dict = None
+        self._colour_theme_json = None
+        self._colour_theme_name = None
+        self._colours_df = None
+        self._colours_graph = None
+        self._colours_trafficlight_hex = None
+        self._colours_trafficlight_rgb = None
+        self._colours_elements = None
+        self._design_theme_dict = None
+        self._design_theme_json = None
+        self._design_theme_name = None
+        self._colours_graphs = None
+
+        # load the inbuilt colour and design adjustment themes
+        self._colour_theme_json = {}
+        self._design_theme_json = {}
+        # availble stuff
+        self.available_colour_themes = []
+        self.available_design_theme_adjustments = []
+        # load the defaults so we have at least these
+        self.load_colour_theme(
+            colour_theme=DEFAULT_COLOUR_THEME,
+            colour_theme_json=DEFAULT_COLOUR_THEME_JSON,
+        )
+        self.load_design_theme_adjustments(
+            design_theme=DEFAULT_DESIGN_THEME,
+            design_theme_json=DEFAULT_DESIGN_THEME_JSON,
+        )
+
+        # set themes to defualts if none selected
+        if colour_theme is None:
+            colour_theme = DEFAULT_COLOUR_THEME
+        if design_theme_adjustments is None:
+            design_theme_adjustments = DEFAULT_DESIGN_THEME
+
+        # activate the theme, using the defualts where these are not selected
+
+        self.activate_theme(
+            colour_theme=colour_theme,
+            design_theme_adjustments=design_theme_adjustments,
+            base_theme=base_theme,
+        )
+
+    def load_colour_theme(self, colour_theme, colour_theme_json):
+        """
+        Load in a new colour theme
+
+        colour_theme_name: str, name of the new theme
+        colour_theme_json: json, json definition of the theme colours.
+
+        """
+
+        # at some stage we shoudl error check the json
+        self._colour_theme_json[colour_theme] = colour_theme_json
+        # availble stuff
+        self.available_colour_themes.append(DEFAULT_COLOUR_THEME)
+
+    def load_design_theme_adjustments(self, design_theme, design_theme_json):
+        """
+        docstring
+        """
+        self._design_theme_json[design_theme] = design_theme_json
+        # availble stuff
+        self.available_design_theme_adjustments.append(DEFAULT_DESIGN_THEME)
+
+    def _set_colour_theme(self, colour_theme):
+        """
+        Set one of the loaded colour themes to be the colour theme we use
+        """
+        # make sure legal colour theme
+        if colour_theme is None:
+            colour_theme = DEFAULT_COLOUR_THEME
+        colour_theme = colour_theme.lower()
+
+        if colour_theme not in self.available_colour_themes:
+            msg = "Invalid colour theme provided. Cannot set plotly colour theme."
+            raise ValueError(msg)
+
+        # convert colour theme json to dict
+        self._colour_theme_name = colour_theme
+        self._colour_theme_dict = json.loads(self._colour_theme_json[colour_theme])
+
+        # store colours in a dataframe
+        self._colours_df = pd.DataFrame(self._colour_theme_dict["colors"])
+        self._colours_df = self._colours_df.set_index("name")
+
+        # set up a list with graph colours in order
+        gphseq = self._colour_theme_dict["roles"]["graph_sequence"]
+        self._colours_graphs = list(self._colours_df.loc[gphseq].hex)
+
+        # traffic light graph colours
+        tlight = self._colour_theme_dict["roles"]["trafficlight"]
+        self._colours_trafficlight_rgb = {}
+        self._colours_trafficlight_hex = {}
+        for light, colour in tlight.items():
+            self._colours_trafficlight_rgb[
+                light.upper()
+            ] = f"rgb({self._colours_df.loc[colour].rgb})"
+            self._colours_trafficlight_hex[light.upper()] = self._colours_df.loc[
+                colour
+            ].hex
+
+        # set up element colours
+        self._colours_elements = dict(
+            box_background=self._colours_df.loc[
+                self._colour_theme_dict["roles"]["box_background"]
+            ].hex,
+            axis=self._colours_df.loc[self._colour_theme_dict["roles"]["axis"]].hex,
+            spikes=self._colours_df.loc[self._colour_theme_dict["roles"]["spikes"]].hex,
+            grid_line=self._colours_df.loc[
+                self._colour_theme_dict["roles"]["grid_line"]
+            ].hex,
+            primary_text=self._colours_df.loc[
+                self._colour_theme_dict["roles"]["primary_text"]
+            ].hex,
+        )
+
+    def _set_design_theme_adjustments(self, design_theme):
+        """
+        Define the formatting/design adjustments for the theme
+        These will replace/overwrite those of any base pio theme selected
+        """
+        # make sure legal colour theme
+        if design_theme is None:
+            design_theme = DEFAULT_DESIGN_THEME
+        design_theme = design_theme.lower()
+
+        if design_theme not in self.available_design_theme_adjustments:
+            msg = (
+                "Invalid design theme provided. Cannot set make the design adjustments."
+            )
+            raise ValueError(msg)
+
+        # record the design theme name
+        self._design_theme_name = design_theme
+        self._design_theme_dict = json.loads(self._design_theme_json[design_theme])
+
+        # margins
+        # self._plot_margins = self._design_theme_dict["plot"]["margins"]
+        # self._streamlit_plot_margins =
+        #       self._design_theme_dict["plot"]["margins_streamlit"]
+
+        # table
+        # self._table_formatting = self._design_theme_dict["table"]
+
+        # specific formatting components
+
+        # legend
+        # if "legend_layout" in self._design_theme_dict:
+        # self._legend_layout = go.Layout(
+        #               legend =
+        #                   self._design_theme_dict["legend_layout"])
+        #    self._legend_layout = self._design_theme_dict["legend_layout"]
+        # else:
+        #    self._legend_layout = go.Layout()
+
+        # graph format
+        # if "graph_format" in self._design_theme_dict:
+        #    self._graph_format = go.Layout(self._design_theme_dict["graph_format"])
+        # else:
+        #    self._graph_format = go.Layout()
+
+    def activate_theme(
+        self,
+        base_theme=None,
+        colour_theme=None,
+        design_theme_adjustments=None,
+    ):
+        """
+        Activate the theming for the plotly graphs
+
+        Uses the currently set colour and design theme adjustments
+        and legend layout and applies these to the base_theme (if
+        base_theme=None, then uses the default base theme)
+        """
+
+        # make sure legal theme
+        if base_theme is None:
+            base_theme = DEFAULT_PIO_THEME
+        base_theme = base_theme.lower()
+
+        # set the various theme parts as selected (otherwise the
+        # already loaded ones will be used)
+        # Note - we skip "None" so that the user can easily
+        # adjust one of the theme components
+        if colour_theme is not None:
+            self._set_colour_theme(colour_theme)
+        if design_theme_adjustments is not None:
+            self._set_design_theme_adjustments(design_theme_adjustments)
+
+        # store the active base theme, colour and design theme adjustments in use
+        # Note: they are not activated until they are run though
+        # here - so they can be "_set_" but
+        # they wont be used until they are activated with this function
+        self.active_base_theme = base_theme
+        self.active_colour_theme = self._colour_theme_name
+        self.active_design_theme_adjustments = self._design_theme_name
+
+        # store the parts of the theme the user/graphs will want to access directly
+        self.pallette = self._colours_graphs
+        self.trafficlight_rgb = self._colours_trafficlight_rgb
+        self.trafficlight_hex = self._colours_trafficlight_hex
+        # self.legend_layout = self._legend_layout
+        # self.graph_format = self._graph_format
+
+        # load the base theme from pio
+        self._pio_template = pio.templates[base_theme]
+
+        # make changes to the base theme
+        self._format_theme()
+
+        # create/overwrite the optimeering theme in pio & set it as the default
+        pio.templates[OPTIMEERING_THEME] = self._pio_template
+        pio.templates.default = OPTIMEERING_THEME
+
+    # ______________________________________
+    # General layout formatting
+    # ______________________________________
+
+    def _format_theme(self):
+
+        this_theme = self._pio_template  # shorthand
+
+        # set the structural (design) formatting
+        # ======================================
+        this_theme = this_theme.update(self._design_theme_dict)
+
+        # set the colour theme formatting
+        # ================================
+        # plot background
+        this_theme["layout"]["paper_bgcolor"] = self._colours_elements["box_background"]
+        this_theme["layout"]["plot_bgcolor"] = self._colours_elements["box_background"]
+
+        # axes. Here use the color property to set everything at once.
+        # Maybe control finer later.
+        this_theme["layout"]["xaxis"]["color"] = self._colours_elements["axis"]
+        this_theme["layout"]["yaxis"]["color"] = self._colours_elements["axis"]
+        this_theme["layout"]["xaxis"]["spikecolor"] = self._colours_elements["spikes"]
+        this_theme["layout"]["xaxis"]["linecolor"] = self._colours_elements["axis"]
+        this_theme["layout"]["yaxis"]["linecolor"] = self._colours_elements["axis"]
+        this_theme["layout"]["yaxis"]["gridcolor"] = self._colours_elements["grid_line"]
+        # graph series colours
+        this_theme.layout.colorway = self._colours_graphs
```

### Comparing `fab-rk-tools-0.3.8/fab_rk_tools/data/deriveddata.py` & `fab_rk_tools-0.3.9/fab_rk_tools/data/deriveddata.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,312 +1,312 @@
-"""
-Fab derived data
-
-These tools are to calculate derived data series.
-They may at a later point be moved to the API??
-
-    - rk_nordic_api -> calculate the LPI (large price index) series.
-            Alternative calc methods enabled.
-"""
-from typing import Union
-
-import archimedes
-
-# import numpy as np
-import pandas as pd
-
-from ..common.constants import PermittedTimeZones
-
-LPI_METHODS = [
-    "constant_abs",
-    "constant_perc",
-]
-
-
-def rk_nordic_lpi(
-    method: str,
-    direction: str,
-    price_areas: Union[list, str],
-    start: Union[pd.Timestamp, str],
-    end: Union[pd.Timestamp, str] = None,
-) -> pd.DataFrame:
-
-    """
-    Calculates and returns the LPI series for rk prices in the given price
-    areas between start and end datetimes.
-
-    Returns the series in a dataframe with a single column for the lpi per
-    price area, indexed by datetime
-
-    The LPI is binary: a value of 1 -> the price deviation is large,
-    0 -> the price deviation is not large
-
-    Parameters:
-        method: str -> {"constant_abs", "constant_perc"},
-        direction: str -> {"up", "dn"},
-        price_areas: Union[list, str] -> list of strings, or single string,
-                price area codes
-        start: Union[pd.Timestamp, str] -> start datetime (timestamp or string)
-        end: Union[pd.Timestamp, str] = None -> end datetime (timestamp
-                or string)
-    """
-    # fix up the parameters
-    method, direction, price_areas, start, end = _rk_nordic_lpi_process_parameters(
-        method, direction, price_areas, start, end
-    )
-
-    # obtain spot and rk price data from archimedes
-    dfspread = _spread_from_rk_data(price_areas, start, end)
-
-    # calculate LPI. Function per method
-    if method == "constant_abs":
-        df_ret = _rk_nordic_lpi_constant_absolute(dfspread, direction)
-    elif method == "constant_perc":
-        df_ret = _rk_nordic_lpi_constant_perc(dfspread, direction)
-
-    return df_ret
-
-
-# -----
-# method: constant absolute
-# -----
-def _rk_nordic_lpi_constant_absolute(
-    dfs: pd.DataFrame,
-    direction: str,
-):
-
-    cutoffs = _get_rk_nordic_constant_cutoffs(dfs.columns, direction)
-    dfx = dfs.copy()
-    for area in dfs.columns:
-        if direction == "up":
-            dfx.loc[dfs[area] <= cutoffs[area], area] = 0
-            dfx.loc[dfs[area] > cutoffs[area], area] = 1
-        else:
-            dfx.loc[dfs[area] >= cutoffs[area], area] = 0
-            dfx.loc[dfs[area] < cutoffs[area], area] = 1
-    return dfx
-
-
-def _get_rk_nordic_constant_cutoffs(price_areas: list, direction: str):
-    """
-    Get constant cutoffs stored in the database
-
-    Currently these are not stored in the DB, so hard coded...
-    """
-    all_cutoffs_up = dict(
-        NO1=20,
-        NO2=20,
-        NO3=20,
-        NO4=20,
-        NO5=20,
-        SE1=20,
-        SE2=20,
-        SE3=20,
-        SE4=20,
-        DK1=20,
-        DK2=20,
-        FI=20,
-    )
-    all_cutoffs_dn = dict(
-        NO1=-20,
-        NO2=-20,
-        NO3=-20,
-        NO4=-20,
-        NO5=-20,
-        SE1=-20,
-        SE2=-20,
-        SE3=-20,
-        SE4=-20,
-        DK1=-20,
-        DK2=-20,
-        FI=-20,
-    )
-    if direction == "up":
-        all_cutoffs = all_cutoffs_up
-    else:
-        all_cutoffs = all_cutoffs_dn
-    cutoffs = {key: value for key, value in all_cutoffs.items() if key in price_areas}
-    return cutoffs
-
-
-# -----
-# method: constant percentage (quantile)
-# -----
-def _rk_nordic_lpi_constant_perc(
-    dfs: pd.DataFrame,
-    direction: str,
-):
-    cutoffs = _get_rk_nordic_perc_cutoffs(dfs.columns)
-    dfs = dfs.copy()
-    for area in dfs.columns:
-
-        if direction == "up":
-            # calc the cut value as quantile (%) of all up regulating prices
-            cut = dfs.loc[dfs[area] > 0, area].quantile(q=1 - cutoffs[area])
-            dfs.loc[dfs[area] <= cut, area] = 0
-            dfs.loc[dfs[area] > cut, area] = 1
-        else:
-            # calc the cut value as quantile (%) of all dn regulating prices
-            cut = dfs.loc[dfs[area] < 0, area].quantile(q=cutoffs[area])
-            dfs.loc[dfs[area] < cut, area] = 1
-            dfs.loc[dfs[area] >= cut, area] = 0
-    return dfs
-
-
-def _get_rk_nordic_perc_cutoffs(price_areas: list):
-    """
-    Get percentage cutoffs stored in the database
-
-    Currently these are not stored in the DB, so hard coded...
-    """
-    all_cutoffs = dict(
-        NO1=0.20,
-        NO2=0.20,
-        NO3=0.20,
-        NO4=0.20,
-        NO5=0.20,
-        SE1=0.20,
-        SE2=0.20,
-        SE3=0.20,
-        SE4=0.20,
-        DK1=0.20,
-        DK2=0.20,
-        FI=0.20,
-    )
-    cutoffs = {key: value for key, value in all_cutoffs.items() if key in price_areas}
-    return cutoffs
-
-
-# -----
-# get spread from arcl
-# -----
-def _spread_from_rk_data(price_areas: list, start: pd.Timestamp, end: pd.Timestamp):
-
-    # read data from archimedes
-    df_prices = archimedes.get(
-        series_ids=[
-            "NP/ConsumptionImbalancePrices",
-            "NP/AreaPrices",
-            "NP/DominatingDirection",
-        ],
-        price_areas=price_areas,
-        end=end,
-        start=start,
-    )
-    # replace the long series names with short versions
-    df_prices.rename(
-        columns={
-            "NP/AreaPrices": "DAM",
-            "NP/ConsumptionImbalancePrices": "rk",
-            "NP/DominatingDirection": "direction",
-        },
-        inplace=True,
-    )
-    df_prices.index = df_prices.index.tz_convert(PermittedTimeZones.TZ_NORDIC)
-    # calc spread and add it in
-    df_tmp = df_prices.rk - df_prices.DAM
-    # df_tmp.columns = pd.MultiIndex.from_product([["spread"], df_tmp.columns])
-    # dfp = df_prices.join(df_tmp)
-    return df_tmp
-
-
-# -----
-# process and error check parameters
-# -----
-def _rk_nordic_lpi_process_parameters(
-    method: str,
-    direction: str,
-    price_areas: Union[list, str],
-    start: Union[pd.Timestamp, str],
-    end: Union[pd.Timestamp, str],
-):
-    """
-    Process the parameters for rk_nordic_lpi and fix if possible
-    """
-    # method
-    method = _process_param_method(method)
-    # direction
-    direction = _process_param_direction(direction)
-    # price areas
-    price_areas = _process_param_price_areas(price_areas)
-    # start
-    start = _process_param_start(start)
-    # end
-    end = _process_param_end(end, start)
-
-    return method, direction, price_areas, start, end
-
-
-def _process_param_method(method):
-    """
-    process method param
-    """
-    if isinstance(method, str):
-        method = method.lower()
-        if method not in LPI_METHODS:
-            msg = f"Parameter <method> must be one of {LPI_METHODS}"
-            raise ValueError(msg)
-    else:
-        msg = f"Parameter <method> must be one of {LPI_METHODS}"
-        raise ValueError(msg)
-    return method
-
-
-def _process_param_direction(direction):
-    """
-    process direction param
-    """
-    if isinstance(direction, str):
-        direction = direction.lower()
-        if direction == "down":
-            direction = "dn"
-        if direction not in ["up", "dn"]:
-            msg = "Direction parameter must be one of ['up', 'dn']"
-            raise ValueError(msg)
-    else:
-        msg = "Parameter <direction> must be one of ['up', 'dn']"
-        raise ValueError(msg)
-    return direction
-
-
-def _process_param_price_areas(price_areas):
-    """
-    process price_area param
-    """
-    if isinstance(price_areas, str):
-        price_areas = [price_areas]
-    if not isinstance(price_areas, list):
-        msg = "Parameter <price_areas> must be a string or list"
-        # For later - should error check list elements and dim
-        raise ValueError(msg)
-    return price_areas
-
-
-def _process_param_start(start):
-    """
-    process start param
-    """
-    if isinstance(start, str):
-        start = pd.to_datetime(start)
-    if not isinstance(start, pd.Timestamp):
-        msg = "Parameter <start> must be a time formatted string or a pandas timestamp"
-        raise ValueError(msg)
-    if start.tzinfo is None:
-        start = start.tz_localize(PermittedTimeZones.TZ_NORDIC)
-    return start
-
-
-def _process_param_end(end, start):
-    """
-    process end param
-    """
-    if isinstance(end, str):
-        end = pd.to_datetime(end)
-    if end is None:
-        end = pd.Timestamp.today()
-    if not isinstance(end, pd.Timestamp):
-        msg = "Parameter <end> must be a time formatted string or a pandas timestamp"
-        raise ValueError(msg)
-    if end.tzinfo is None:
-        end = end.tz_localize(PermittedTimeZones.TZ_NORDIC)
-    end = max(end, start)
-    return end
+"""
+Fab derived data
+
+These tools are to calculate derived data series.
+They may at a later point be moved to the API??
+
+    - rk_nordic_api -> calculate the LPI (large price index) series.
+            Alternative calc methods enabled.
+"""
+from typing import Union
+
+import archimedes
+
+# import numpy as np
+import pandas as pd
+
+from ..common.constants import PermittedTimeZones
+
+LPI_METHODS = [
+    "constant_abs",
+    "constant_perc",
+]
+
+
+def rk_nordic_lpi(
+    method: str,
+    direction: str,
+    price_areas: Union[list, str],
+    start: Union[pd.Timestamp, str],
+    end: Union[pd.Timestamp, str] = None,
+) -> pd.DataFrame:
+
+    """
+    Calculates and returns the LPI series for rk prices in the given price
+    areas between start and end datetimes.
+
+    Returns the series in a dataframe with a single column for the lpi per
+    price area, indexed by datetime
+
+    The LPI is binary: a value of 1 -> the price deviation is large,
+    0 -> the price deviation is not large
+
+    Parameters:
+        method: str -> {"constant_abs", "constant_perc"},
+        direction: str -> {"up", "dn"},
+        price_areas: Union[list, str] -> list of strings, or single string,
+                price area codes
+        start: Union[pd.Timestamp, str] -> start datetime (timestamp or string)
+        end: Union[pd.Timestamp, str] = None -> end datetime (timestamp
+                or string)
+    """
+    # fix up the parameters
+    method, direction, price_areas, start, end = _rk_nordic_lpi_process_parameters(
+        method, direction, price_areas, start, end
+    )
+
+    # obtain spot and rk price data from archimedes
+    dfspread = _spread_from_rk_data(price_areas, start, end)
+
+    # calculate LPI. Function per method
+    if method == "constant_abs":
+        df_ret = _rk_nordic_lpi_constant_absolute(dfspread, direction)
+    elif method == "constant_perc":
+        df_ret = _rk_nordic_lpi_constant_perc(dfspread, direction)
+
+    return df_ret
+
+
+# -----
+# method: constant absolute
+# -----
+def _rk_nordic_lpi_constant_absolute(
+    dfs: pd.DataFrame,
+    direction: str,
+):
+
+    cutoffs = _get_rk_nordic_constant_cutoffs(dfs.columns, direction)
+    dfx = dfs.copy()
+    for area in dfs.columns:
+        if direction == "up":
+            dfx.loc[dfs[area] <= cutoffs[area], area] = 0
+            dfx.loc[dfs[area] > cutoffs[area], area] = 1
+        else:
+            dfx.loc[dfs[area] >= cutoffs[area], area] = 0
+            dfx.loc[dfs[area] < cutoffs[area], area] = 1
+    return dfx
+
+
+def _get_rk_nordic_constant_cutoffs(price_areas: list, direction: str):
+    """
+    Get constant cutoffs stored in the database
+
+    Currently these are not stored in the DB, so hard coded...
+    """
+    all_cutoffs_up = dict(
+        NO1=20,
+        NO2=20,
+        NO3=20,
+        NO4=20,
+        NO5=20,
+        SE1=20,
+        SE2=20,
+        SE3=20,
+        SE4=20,
+        DK1=20,
+        DK2=20,
+        FI=20,
+    )
+    all_cutoffs_dn = dict(
+        NO1=-20,
+        NO2=-20,
+        NO3=-20,
+        NO4=-20,
+        NO5=-20,
+        SE1=-20,
+        SE2=-20,
+        SE3=-20,
+        SE4=-20,
+        DK1=-20,
+        DK2=-20,
+        FI=-20,
+    )
+    if direction == "up":
+        all_cutoffs = all_cutoffs_up
+    else:
+        all_cutoffs = all_cutoffs_dn
+    cutoffs = {key: value for key, value in all_cutoffs.items() if key in price_areas}
+    return cutoffs
+
+
+# -----
+# method: constant percentage (quantile)
+# -----
+def _rk_nordic_lpi_constant_perc(
+    dfs: pd.DataFrame,
+    direction: str,
+):
+    cutoffs = _get_rk_nordic_perc_cutoffs(dfs.columns)
+    dfs = dfs.copy()
+    for area in dfs.columns:
+
+        if direction == "up":
+            # calc the cut value as quantile (%) of all up regulating prices
+            cut = dfs.loc[dfs[area] > 0, area].quantile(q=1 - cutoffs[area])
+            dfs.loc[dfs[area] <= cut, area] = 0
+            dfs.loc[dfs[area] > cut, area] = 1
+        else:
+            # calc the cut value as quantile (%) of all dn regulating prices
+            cut = dfs.loc[dfs[area] < 0, area].quantile(q=cutoffs[area])
+            dfs.loc[dfs[area] < cut, area] = 1
+            dfs.loc[dfs[area] >= cut, area] = 0
+    return dfs
+
+
+def _get_rk_nordic_perc_cutoffs(price_areas: list):
+    """
+    Get percentage cutoffs stored in the database
+
+    Currently these are not stored in the DB, so hard coded...
+    """
+    all_cutoffs = dict(
+        NO1=0.20,
+        NO2=0.20,
+        NO3=0.20,
+        NO4=0.20,
+        NO5=0.20,
+        SE1=0.20,
+        SE2=0.20,
+        SE3=0.20,
+        SE4=0.20,
+        DK1=0.20,
+        DK2=0.20,
+        FI=0.20,
+    )
+    cutoffs = {key: value for key, value in all_cutoffs.items() if key in price_areas}
+    return cutoffs
+
+
+# -----
+# get spread from arcl
+# -----
+def _spread_from_rk_data(price_areas: list, start: pd.Timestamp, end: pd.Timestamp):
+
+    # read data from archimedes
+    df_prices = archimedes.get(
+        series_ids=[
+            "NP/ConsumptionImbalancePrices",
+            "NP/AreaPrices",
+            "NP/DominatingDirection",
+        ],
+        price_areas=price_areas,
+        end=end,
+        start=start,
+    )
+    # replace the long series names with short versions
+    df_prices.rename(
+        columns={
+            "NP/AreaPrices": "DAM",
+            "NP/ConsumptionImbalancePrices": "rk",
+            "NP/DominatingDirection": "direction",
+        },
+        inplace=True,
+    )
+    df_prices.index = df_prices.index.tz_convert(PermittedTimeZones.TZ_NORDIC)
+    # calc spread and add it in
+    df_tmp = df_prices.rk - df_prices.DAM
+    # df_tmp.columns = pd.MultiIndex.from_product([["spread"], df_tmp.columns])
+    # dfp = df_prices.join(df_tmp)
+    return df_tmp
+
+
+# -----
+# process and error check parameters
+# -----
+def _rk_nordic_lpi_process_parameters(
+    method: str,
+    direction: str,
+    price_areas: Union[list, str],
+    start: Union[pd.Timestamp, str],
+    end: Union[pd.Timestamp, str],
+):
+    """
+    Process the parameters for rk_nordic_lpi and fix if possible
+    """
+    # method
+    method = _process_param_method(method)
+    # direction
+    direction = _process_param_direction(direction)
+    # price areas
+    price_areas = _process_param_price_areas(price_areas)
+    # start
+    start = _process_param_start(start)
+    # end
+    end = _process_param_end(end, start)
+
+    return method, direction, price_areas, start, end
+
+
+def _process_param_method(method):
+    """
+    process method param
+    """
+    if isinstance(method, str):
+        method = method.lower()
+        if method not in LPI_METHODS:
+            msg = f"Parameter <method> must be one of {LPI_METHODS}"
+            raise ValueError(msg)
+    else:
+        msg = f"Parameter <method> must be one of {LPI_METHODS}"
+        raise ValueError(msg)
+    return method
+
+
+def _process_param_direction(direction):
+    """
+    process direction param
+    """
+    if isinstance(direction, str):
+        direction = direction.lower()
+        if direction == "down":
+            direction = "dn"
+        if direction not in ["up", "dn"]:
+            msg = "Direction parameter must be one of ['up', 'dn']"
+            raise ValueError(msg)
+    else:
+        msg = "Parameter <direction> must be one of ['up', 'dn']"
+        raise ValueError(msg)
+    return direction
+
+
+def _process_param_price_areas(price_areas):
+    """
+    process price_area param
+    """
+    if isinstance(price_areas, str):
+        price_areas = [price_areas]
+    if not isinstance(price_areas, list):
+        msg = "Parameter <price_areas> must be a string or list"
+        # For later - should error check list elements and dim
+        raise ValueError(msg)
+    return price_areas
+
+
+def _process_param_start(start):
+    """
+    process start param
+    """
+    if isinstance(start, str):
+        start = pd.to_datetime(start)
+    if not isinstance(start, pd.Timestamp):
+        msg = "Parameter <start> must be a time formatted string or a pandas timestamp"
+        raise ValueError(msg)
+    if start.tzinfo is None:
+        start = start.tz_localize(PermittedTimeZones.TZ_NORDIC)
+    return start
+
+
+def _process_param_end(end, start):
+    """
+    process end param
+    """
+    if isinstance(end, str):
+        end = pd.to_datetime(end)
+    if end is None:
+        end = pd.Timestamp.today()
+    if not isinstance(end, pd.Timestamp):
+        msg = "Parameter <end> must be a time formatted string or a pandas timestamp"
+        raise ValueError(msg)
+    if end.tzinfo is None:
+        end = end.tz_localize(PermittedTimeZones.TZ_NORDIC)
+    end = max(end, start)
+    return end
```

### Comparing `fab-rk-tools-0.3.8/fab_rk_tools/graphs/basic_bar.py` & `fab_rk_tools-0.3.9/fab_rk_tools/graphs/basic_bar.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-import numpy as np
-import pandas as pd
-import plotly.graph_objects as go
-from pyparsing import col
-
-from ..assets import opt_plotly_theme as theme
-from ..common.utils import update_fig_traces
-
-
-def basic_bar(
-    df: pd.DataFrame,
-    layout_update=None,
-    series_cols=["price"],
-    yaxis_label=None,
-    y_scale=None,
-    trace_update=None,
-    monochrome=False,
-) -> go.Figure:
-    """
-
-    Construct a bar chart for series provided in the dataframe.
-    The series are provided as columes in the dataframe
-
-    Inputs:
-
-    df -> dataframe for series values, with columns including [from_dt, series_cols]
-    series_cols -> list, the columns in df for the series to graph
-    labels -> list, display labels to use for the series
-    colour_ids -> list, colours to use for hte series
-
-    """
-
-    # get the active graph theme (or create one if there isnt one)
-    # this way we ensure that these graphs are always formatted with the opt_plotly_theme. yay!
-    graph_theme = theme.FabPlotlyTheme()
-
-    _error_check(df, series_cols, yaxis_label, y_scale)
-
-    # the way this is done is that we use two axes - one for the above, one for the below
-
-    # set the graph layout
-
-    layout = _set_layout(
-        yaxis_label=yaxis_label, y_scale=y_scale, layout_update=layout_update
-    )
-
-    # create the figure and add a series for each category
-
-    fig = go.Figure(layout=layout)
-
-    for s in series_cols:
-        new_bar = go.Bar(
-            x=df.from_dt,
-            y=df[s],
-            name=f"{s}",
-            # marker_color = theme.pallette_theme[above_colour_id],
-        )
-        fig.add_trace(new_bar)
-
-    if len(series_cols) == 1:
-        # remove series name from hover
-        fig.update_traces(hovertemplate="%{y:.2f}<extra></extra>")
-
-    # if monochrome update
-    if monochrome == True:
-        col = graph_theme.monochrome_hex
-        fig.update_traces(patch={"marker_color": col})
-
-    # update traces with user defined updates
-    fig = update_fig_traces(fig, trace_update)
-    return fig
-
-
-def _error_check(df, series_cols, yaxis_label, y_scale):
-    if not isinstance(series_cols, list):
-        msg = "Series_cols need to be provided as a list"
-        raise ValueError(msg)
-    if not (isinstance(yaxis_label, str) or yaxis_label is None):
-        msg = "yaxis_label needs to be None or a string"
-        raise ValueError(msg)
-    if not isinstance(df, pd.DataFrame):
-        msg = "df must be a dataframe"
-        raise ValueError(msg)
-    if not (isinstance(y_scale, list) or y_scale is None):
-        msg = "y_scale needs to be provided as a list"
-        raise ValueError(msg)
-
-    if not (set(series_cols) <= set(df.columns)):
-        msg = (
-            "Provided column list in series_cols is not found in the dataframe columns"
-        )
-        raise ValueError(msg)
-    if y_scale is not None and (len(y_scale) < 2 or len(y_scale) > 3):
-        msg = "y_scale needs 2 or 3 elements"
-        raise ValueError(msg)
-
-
-def _set_layout(yaxis_label, layout_update, y_scale=None, barmode="group"):
-    """
-    Generate the layout object for the graph
-    """
-
-    # basic format
-    layout = go.Layout()
-
-    # specific formatting options for this graph
-    layout = layout.update(dict(barmode=barmode))
-
-    layout["yaxis"] = layout["yaxis"].update(
-        dict(
-            title=f"{yaxis_label}",
-            showgrid=True,
-        )
-    )
-    if y_scale is not None:
-        layout["yaxis"] = layout["yaxis"].update(dict(range=y_scale))
-
-    layout["xaxis"] = layout["xaxis"].update(
-        dict(
-            hoverformat="%H:%M",
-            tickformat="%H",  # %d %B (%a)<br>%Y
-            dtick=86400000.0 / 24,
-            title=None,
-        )
-    )
-
-    # update with any user graph formatting instructions
-    if layout_update is not None:
-        layout = layout.update(go.Layout(layout_update))
-
-    return layout
+import numpy as np
+import pandas as pd
+import plotly.graph_objects as go
+from pyparsing import col
+
+from ..assets import opt_plotly_theme as theme
+from ..common.utils import update_fig_traces
+
+
+def basic_bar(
+    df: pd.DataFrame,
+    layout_update=None,
+    series_cols=["price"],
+    yaxis_label=None,
+    y_scale=None,
+    trace_update=None,
+    monochrome=False,
+) -> go.Figure:
+    """
+
+    Construct a bar chart for series provided in the dataframe.
+    The series are provided as columes in the dataframe
+
+    Inputs:
+
+    df -> dataframe for series values, with columns including [from_dt, series_cols]
+    series_cols -> list, the columns in df for the series to graph
+    labels -> list, display labels to use for the series
+    colour_ids -> list, colours to use for hte series
+
+    """
+
+    # get the active graph theme (or create one if there isnt one)
+    # this way we ensure that these graphs are always formatted with the opt_plotly_theme. yay!
+    graph_theme = theme.FabPlotlyTheme()
+
+    _error_check(df, series_cols, yaxis_label, y_scale)
+
+    # the way this is done is that we use two axes - one for the above, one for the below
+
+    # set the graph layout
+
+    layout = _set_layout(
+        yaxis_label=yaxis_label, y_scale=y_scale, layout_update=layout_update
+    )
+
+    # create the figure and add a series for each category
+
+    fig = go.Figure(layout=layout)
+
+    for s in series_cols:
+        new_bar = go.Bar(
+            x=df.from_dt,
+            y=df[s],
+            name=f"{s}",
+            # marker_color = theme.pallette_theme[above_colour_id],
+        )
+        fig.add_trace(new_bar)
+
+    if len(series_cols) == 1:
+        # remove series name from hover
+        fig.update_traces(hovertemplate="%{y:.2f}<extra></extra>")
+
+    # if monochrome update
+    if monochrome == True:
+        col = graph_theme.monochrome_hex
+        fig.update_traces(patch={"marker_color": col})
+
+    # update traces with user defined updates
+    fig = update_fig_traces(fig, trace_update)
+    return fig
+
+
+def _error_check(df, series_cols, yaxis_label, y_scale):
+    if not isinstance(series_cols, list):
+        msg = "Series_cols need to be provided as a list"
+        raise ValueError(msg)
+    if not (isinstance(yaxis_label, str) or yaxis_label is None):
+        msg = "yaxis_label needs to be None or a string"
+        raise ValueError(msg)
+    if not isinstance(df, pd.DataFrame):
+        msg = "df must be a dataframe"
+        raise ValueError(msg)
+    if not (isinstance(y_scale, list) or y_scale is None):
+        msg = "y_scale needs to be provided as a list"
+        raise ValueError(msg)
+
+    if not (set(series_cols) <= set(df.columns)):
+        msg = (
+            "Provided column list in series_cols is not found in the dataframe columns"
+        )
+        raise ValueError(msg)
+    if y_scale is not None and (len(y_scale) < 2 or len(y_scale) > 3):
+        msg = "y_scale needs 2 or 3 elements"
+        raise ValueError(msg)
+
+
+def _set_layout(yaxis_label, layout_update, y_scale=None, barmode="group"):
+    """
+    Generate the layout object for the graph
+    """
+
+    # basic format
+    layout = go.Layout()
+
+    # specific formatting options for this graph
+    layout = layout.update(dict(barmode=barmode))
+
+    layout["yaxis"] = layout["yaxis"].update(
+        dict(
+            title=f"{yaxis_label}",
+            showgrid=True,
+        )
+    )
+    if y_scale is not None:
+        layout["yaxis"] = layout["yaxis"].update(dict(range=y_scale))
+
+    layout["xaxis"] = layout["xaxis"].update(
+        dict(
+            hoverformat="%H:%M",
+            tickformat="%H",  # %d %B (%a)<br>%Y
+            dtick=86400000.0 / 24,
+            title=None,
+        )
+    )
+
+    # update with any user graph formatting instructions
+    if layout_update is not None:
+        layout = layout.update(go.Layout(layout_update))
+
+    return layout
```

### Comparing `fab-rk-tools-0.3.8/fab_rk_tools/graphs/discrete_distro_bar.py` & `fab_rk_tools-0.3.9/fab_rk_tools/graphs/discrete_distro_bar.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-import logging
-from numbers import Number
-
-import numpy as np
-import pandas as pd
-import plotly.graph_objects as go
-
-from ..assets import opt_plotly_theme as theme
-from ..common.utils import update_fig_traces
-
-logging.basicConfig(level=logging.INFO)
-
-
-def discrete_distro_bar(
-    df_fcast: pd.DataFrame,
-    df_obs: pd.DataFrame = None,
-    layout_update=None,
-    fcast_category_col="direction",
-    fcast_value_col="probability",
-    obs_value_col="value",
-    category_order=None,
-    category_direction_map=None,
-    trace_update=None,
-) -> go.Figure:
-    """
-
-    Construct a stacked bar chart for discrete distributions
-
-    Inputs:
-
-    df_fcast -> dataframe for forecasted values, with columns including [from_dt, fcast_category_col, fcast_value_col]
-    df_obs -> dataframe with the actual observations, with columns including [from_dt, obs_value_col]
-
-    Note that the df_obs should not have any other data in it - only the observed outturns
-
-    """
-
-    # get the active graph theme (or create one if there isnt one)
-    # this way we ensure that these graphs are always formatted with the opt_plotly_theme. yay!
-    graph_theme = theme.FabPlotlyTheme()
-
-    # set the graph layout
-
-    layout = _set_layout(layout_update)
-
-    # all nans in the df_obs - just set it to none so it is not graphed
-    if df_obs is not None:
-        if len(df_obs) >= 1:
-            if df_obs[obs_value_col].apply(lambda x: np.isnan(x)).all():
-                df_obs = None
-
-    fig = go.Figure(layout=layout)
-    if category_order is None:
-        category_order = df_fcast[fcast_category_col].unique()
-    count = 0
-    for cat in category_order:
-        df = df_fcast[df_fcast[fcast_category_col] == cat]
-        if isinstance(category_direction_map, dict):
-            # should check that we have the keys
-            direction = category_direction_map[
-                cat
-            ]  # the direction matching the category
-            barcol = graph_theme.direction_hex[
-                direction
-            ]  # the colour for the direction
-        else:
-            barcol = graph_theme.pallette[count]
-            count = count + 1
-        bar = go.Bar(
-            x=df.from_dt,
-            y=df[fcast_value_col],
-            name="{}".format(cat),
-            marker_color=barcol,
-        )
-        fig.add_trace(bar)
-    # add a trace for the actual values if they exist
-    if df_obs is not None:
-        if len(df_obs) > 0:
-            fig.add_trace(
-                go.Scatter(
-                    x=df_obs.from_dt,
-                    y=df_obs[obs_value_col],
-                    name="Actual",
-                    mode="markers",
-                )
-            )
-    # update traces with user defined updates
-    fig = update_fig_traces(fig, trace_update)
-
-    return fig
-
-
-def _set_layout(layout_update):
-    """
-    Generate the layout object for the graph
-    """
-
-    # basic format, to ensure consistency
-    layout = go.Layout()
-
-    # specific formatting options for this graph
-
-    layout = layout.update(dict(barmode="stack"))
-
-    layout["yaxis"] = layout["yaxis"].update(
-        dict(
-            title="Probability",
-            showgrid=True,
-            range=[0, 1.01],
-            # autorange=False
-        )
-    )
-
-    layout["xaxis"] = layout["xaxis"].update(
-        dict(
-            hoverformat="%H:%M",
-            tickformat="%H",  # %d %B (%a)<br>%Y
-            dtick=86400000.0 / 24,
-            title=None,
-        )
-    )
-
-    # update with any user instructions
-    if layout_update is not None:
-        layout = layout.update(go.Layout(layout_update))
-
-    return layout
+import logging
+from numbers import Number
+
+import numpy as np
+import pandas as pd
+import plotly.graph_objects as go
+
+from ..assets import opt_plotly_theme as theme
+from ..common.utils import update_fig_traces
+
+logging.basicConfig(level=logging.INFO)
+
+
+def discrete_distro_bar(
+    df_fcast: pd.DataFrame,
+    df_obs: pd.DataFrame = None,
+    layout_update=None,
+    fcast_category_col="direction",
+    fcast_value_col="probability",
+    obs_value_col="value",
+    category_order=None,
+    category_direction_map=None,
+    trace_update=None,
+) -> go.Figure:
+    """
+
+    Construct a stacked bar chart for discrete distributions
+
+    Inputs:
+
+    df_fcast -> dataframe for forecasted values, with columns including [from_dt, fcast_category_col, fcast_value_col]
+    df_obs -> dataframe with the actual observations, with columns including [from_dt, obs_value_col]
+
+    Note that the df_obs should not have any other data in it - only the observed outturns
+
+    """
+
+    # get the active graph theme (or create one if there isnt one)
+    # this way we ensure that these graphs are always formatted with the opt_plotly_theme. yay!
+    graph_theme = theme.FabPlotlyTheme()
+
+    # set the graph layout
+
+    layout = _set_layout(layout_update)
+
+    # all nans in the df_obs - just set it to none so it is not graphed
+    if df_obs is not None:
+        if len(df_obs) >= 1:
+            if df_obs[obs_value_col].apply(lambda x: np.isnan(x)).all():
+                df_obs = None
+
+    fig = go.Figure(layout=layout)
+    if category_order is None:
+        category_order = df_fcast[fcast_category_col].unique()
+    count = 0
+    for cat in category_order:
+        df = df_fcast[df_fcast[fcast_category_col] == cat]
+        if isinstance(category_direction_map, dict):
+            # should check that we have the keys
+            direction = category_direction_map[
+                cat
+            ]  # the direction matching the category
+            barcol = graph_theme.direction_hex[
+                direction
+            ]  # the colour for the direction
+        else:
+            barcol = graph_theme.pallette[count]
+            count = count + 1
+        bar = go.Bar(
+            x=df.from_dt,
+            y=df[fcast_value_col],
+            name="{}".format(cat),
+            marker_color=barcol,
+        )
+        fig.add_trace(bar)
+    # add a trace for the actual values if they exist
+    if df_obs is not None:
+        if len(df_obs) > 0:
+            fig.add_trace(
+                go.Scatter(
+                    x=df_obs.from_dt,
+                    y=df_obs[obs_value_col],
+                    name="Actual",
+                    mode="markers",
+                )
+            )
+    # update traces with user defined updates
+    fig = update_fig_traces(fig, trace_update)
+
+    return fig
+
+
+def _set_layout(layout_update):
+    """
+    Generate the layout object for the graph
+    """
+
+    # basic format, to ensure consistency
+    layout = go.Layout()
+
+    # specific formatting options for this graph
+
+    layout = layout.update(dict(barmode="stack"))
+
+    layout["yaxis"] = layout["yaxis"].update(
+        dict(
+            title="Probability",
+            showgrid=True,
+            range=[0, 1.01],
+            # autorange=False
+        )
+    )
+
+    layout["xaxis"] = layout["xaxis"].update(
+        dict(
+            hoverformat="%H:%M",
+            tickformat="%H",  # %d %B (%a)<br>%Y
+            dtick=86400000.0 / 24,
+            title=None,
+        )
+    )
+
+    # update with any user instructions
+    if layout_update is not None:
+        layout = layout.update(go.Layout(layout_update))
+
+    return layout
```

### Comparing `fab-rk-tools-0.3.8/fab_rk_tools/graphs/mirror_bar.py` & `fab_rk_tools-0.3.9/fab_rk_tools/graphs/mirror_bar.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-import numpy as np
-import pandas as pd
-import plotly.graph_objects as go
-
-from ..assets import opt_plotly_theme as theme
-from ..common.utils import update_fig_traces
-
-
-def mirror_bar(
-    df_above: pd.DataFrame,
-    df_below: pd.DataFrame,
-    layout_update=None,
-    value_col="indicator",
-    above_label="",
-    below_label="",
-    trace_update=None,
-    monochrome=False,
-) -> go.Figure:
-    """
-
-    Construct a bar chart for two series, where the "above" series is shown above x=0, and the below series is below x=0
-
-    Inputs:
-
-    df_above -> dataframe for above series values, with columns including [from_dt, value_col]
-    df_below -> dataframe with the actual observations, with columns including [from_dt, value_col]
-    value_col -> the value column name
-    above_label, below_label -> labels to use for the two series
-
-    """
-
-    # get the active graph theme (or create one if there isnt one)
-    # this way we ensure that these graphs are always formatted with the opt_plotly_theme. yay!
-    graph_theme = theme.FabPlotlyTheme()
-
-    # the way this is done is that we use two axes - one for the above, one for the below
-
-    # set the graph layout
-
-    layout = _set_layout(above_label, below_label, layout_update)
-
-    # create the figure and add a series for each category
-
-    fig = go.Figure(layout=layout)
-
-    if len(df_above) > 0:
-        above_bar = go.Bar(
-            x=df_above.from_dt,
-            y=df_above[value_col],
-            name="{}".format(above_label),
-        )
-        # above_bar.update(marker_color=graph_theme.element_colours["bar_above"])
-
-        fig.add_trace(above_bar)
-
-    if len(df_below) > 0:
-        df_b = df_below.copy()
-        df_b[value_col] = df_b[value_col]
-        below_bar = go.Bar(
-            x=df_b.from_dt,
-            y=df_b[value_col],
-            xaxis="x",
-            yaxis="y2",
-            name="{}".format(below_label),
-        )
-        # below_bar.update(marker_color=graph_theme.element_colours["bar_below"])
-
-        fig.add_trace(below_bar)
-
-    # if monochrome update all traces to monochrome colour
-    if monochrome == True:
-        col = graph_theme.monochrome_hex
-        fig.update_traces(patch={"marker_color": col})
-
-    # update traces with user defined updates
-    fig = update_fig_traces(fig, trace_update)
-
-    return fig
-
-
-def _set_layout(above_label, below_label, layout_update):
-    """
-    Generate the layout object for the graph
-    """
-
-    # basic format, to ensure consistency
-    layout = go.Layout()
-
-    # specific formatting options for this graph
-
-    layout = layout.update(dict(barmode="overlay"))
-
-    layout["yaxis"] = layout["yaxis"].update(
-        dict(
-            title="{}   ←   Index   →   {}".format(below_label, above_label),
-            showgrid=True,
-            range=[-10.01, 10.01],
-            tickmode="array",
-            tickvals=list(range(-10, 11, 2)),
-            ticktext=[str(abs(i)) for i in list(range(-10, 11, 2))],
-        )
-    )
-
-    layout["yaxis2"] = dict(
-        title=None,
-        range=[10.01, -10.01],
-        # autorange="reversed",
-        # fixedrange=True,
-        anchor="x",
-        overlaying="y",
-        visible=False,
-        side="right",
-    )
-
-    layout["xaxis"] = layout["xaxis"].update(
-        dict(
-            hoverformat="%H:%M",
-            tickformat="%H",  # %d %B (%a)<br>%Y
-            dtick=86400000.0 / 24,
-            title=None,
-        )
-    )
-
-    # update with any user instructions
-    if layout_update is not None:
-        layout = layout.update(go.Layout(layout_update))
-
-    return layout
+import numpy as np
+import pandas as pd
+import plotly.graph_objects as go
+
+from ..assets import opt_plotly_theme as theme
+from ..common.utils import update_fig_traces
+
+
+def mirror_bar(
+    df_above: pd.DataFrame,
+    df_below: pd.DataFrame,
+    layout_update=None,
+    value_col="indicator",
+    above_label="",
+    below_label="",
+    trace_update=None,
+    monochrome=False,
+) -> go.Figure:
+    """
+
+    Construct a bar chart for two series, where the "above" series is shown above x=0, and the below series is below x=0
+
+    Inputs:
+
+    df_above -> dataframe for above series values, with columns including [from_dt, value_col]
+    df_below -> dataframe with the actual observations, with columns including [from_dt, value_col]
+    value_col -> the value column name
+    above_label, below_label -> labels to use for the two series
+
+    """
+
+    # get the active graph theme (or create one if there isnt one)
+    # this way we ensure that these graphs are always formatted with the opt_plotly_theme. yay!
+    graph_theme = theme.FabPlotlyTheme()
+
+    # the way this is done is that we use two axes - one for the above, one for the below
+
+    # set the graph layout
+
+    layout = _set_layout(above_label, below_label, layout_update)
+
+    # create the figure and add a series for each category
+
+    fig = go.Figure(layout=layout)
+
+    if len(df_above) > 0:
+        above_bar = go.Bar(
+            x=df_above.from_dt,
+            y=df_above[value_col],
+            name="{}".format(above_label),
+        )
+        # above_bar.update(marker_color=graph_theme.element_colours["bar_above"])
+
+        fig.add_trace(above_bar)
+
+    if len(df_below) > 0:
+        df_b = df_below.copy()
+        df_b[value_col] = df_b[value_col]
+        below_bar = go.Bar(
+            x=df_b.from_dt,
+            y=df_b[value_col],
+            xaxis="x",
+            yaxis="y2",
+            name="{}".format(below_label),
+        )
+        # below_bar.update(marker_color=graph_theme.element_colours["bar_below"])
+
+        fig.add_trace(below_bar)
+
+    # if monochrome update all traces to monochrome colour
+    if monochrome == True:
+        col = graph_theme.monochrome_hex
+        fig.update_traces(patch={"marker_color": col})
+
+    # update traces with user defined updates
+    fig = update_fig_traces(fig, trace_update)
+
+    return fig
+
+
+def _set_layout(above_label, below_label, layout_update):
+    """
+    Generate the layout object for the graph
+    """
+
+    # basic format, to ensure consistency
+    layout = go.Layout()
+
+    # specific formatting options for this graph
+
+    layout = layout.update(dict(barmode="overlay"))
+
+    layout["yaxis"] = layout["yaxis"].update(
+        dict(
+            title="{}   ←   Index   →   {}".format(below_label, above_label),
+            showgrid=True,
+            range=[-10.01, 10.01],
+            tickmode="array",
+            tickvals=list(range(-10, 11, 2)),
+            ticktext=[str(abs(i)) for i in list(range(-10, 11, 2))],
+        )
+    )
+
+    layout["yaxis2"] = dict(
+        title=None,
+        range=[10.01, -10.01],
+        # autorange="reversed",
+        # fixedrange=True,
+        anchor="x",
+        overlaying="y",
+        visible=False,
+        side="right",
+    )
+
+    layout["xaxis"] = layout["xaxis"].update(
+        dict(
+            hoverformat="%H:%M",
+            tickformat="%H",  # %d %B (%a)<br>%Y
+            dtick=86400000.0 / 24,
+            title=None,
+        )
+    )
+
+    # update with any user instructions
+    if layout_update is not None:
+        layout = layout.update(go.Layout(layout_update))
+
+    return layout
```

### Comparing `fab-rk-tools-0.3.8/fab_rk_tools/graphs/scatter_quantile_fan.py` & `fab_rk_tools-0.3.9/fab_rk_tools/graphs/scatter_quantile_fan.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,277 +1,277 @@
-import numpy as np
-import pandas as pd
-import plotly.graph_objects as go
-
-from ..assets import opt_plotly_theme as theme
-
-# import plotly.io as pio
-from ..common.utils import update_fig_traces
-
-
-def scatter_quantile_fan(
-    df_q: pd.DataFrame,
-    df_l: pd.DataFrame,
-    quantile_col="quantile",
-    quantile_value="value",
-    series_col="series",
-    series_value="value",
-    layout_update=None,
-    trace_update=None,
-    monochrome=False,
-) -> go.Figure:
-    """
-
-    Construct a scatter fan diagram
-
-    Inputs:
-
-    df_q -> dataframe for quantiles, with columns [from_dt, ref_dt, quantile, value]
-    df_l -> dataframe for all other data to graph, with columns [from_dt, series, value]
-
-    The function will graph df_q between min and max quantiles, and the median (0.5) quantile, as a fan
-    Each series in df_l will be graphed as a line
-
-    """
-
-    # get the active graph theme (or create one if there isnt one)
-    graph_theme = theme.FabPlotlyTheme()
-
-    # test params
-    _scatter_quantile_fan_error_test(df_q, df_l)
-
-    # extract the quantiles
-    quantiles = list(df_q[quantile_col].unique())
-    qmax = max(quantiles)
-    qmin = min(quantiles)
-    qmed = _find_middle(quantiles)
-
-    # Create a df for min, max, med. Just makes the graph code slightly easier to read
-    df_min = df_q[(df_q[quantile_col] == qmin)].copy()
-    df_max = df_q[(df_q[quantile_col] == qmax)].copy()
-    df_med = df_q[(df_q[quantile_col] == qmed)].copy()
-
-    # define the graph with our scatter fan layout
-    fig = go.Figure(layout=_scatter_quantile_fan_layout(layout_update))
-
-    # copy the colour palette for graphs
-    palette_colors = list(graph_theme.pio_default_template().layout.colorway)
-
-    # first the fan colour. We want this to be semi-transparent and the same colour as the first trace
-    # get the first colour in the colorway for the active (default) template
-
-    if monochrome:
-        fan_col_base = graph_theme.monochrome_hex
-    else:
-        fan_col_base = graph_theme.fan_hex
-    h = fan_col_base.lstrip("#")
-    fan_col_rgb_transp = list(int(h[i : i + 2], 16) for i in (0, 2, 4))
-    fan_col_rgb_transp.append(0.3)
-    fan_col_rgb_transp = "rgba" + str(tuple(fan_col_rgb_transp))
-
-    # upper and lower lines for the fan. set to be 100% transparent
-    fan_border_line = dict(color="rgba(0,0,0,0)")
-
-    # add the quantile fan
-    name = str(qmin * 100) + "%"
-    label = name
-    fig.add_trace(
-        go.Scatter(
-            y=df_min[quantile_value],
-            x=df_min.from_dt,
-            name=name,
-            mode="lines",
-            line=fan_border_line,
-            showlegend=False,
-            hovertemplate=label + ": %{y:.2f}<extra></extra>",
-        )
-    )
-
-    name = str(qmin * 100) + "%-<br>" + str(qmax * 100) + "%"
-    label = str(qmax * 100) + "%"
-    fig.add_trace(
-        go.Scatter(
-            y=df_max[quantile_value],
-            x=df_max.from_dt,
-            fill="tonexty",
-            fillcolor=fan_col_rgb_transp,
-            mode="lines",
-            line=fan_border_line,
-            name=name,
-            hovertemplate=label + ": %{y:.2f}<extra></extra>",
-        )
-    )
-
-    name = str(qmed * 100) + "%"
-    label = name
-    fig.add_trace(
-        go.Scatter(
-            y=df_med[quantile_value],
-            x=df_med.from_dt,
-            name=name,
-            mode="lines+markers",
-            hovertemplate=label + ": %{y:.2f}<extra></extra>",
-            marker=dict(symbol="circle", opacity=0.5, size=8, color=fan_col_base),
-            line=dict(color=fan_col_base),
-        )
-    )
-
-    # add the lines for the market prices if we have them
-    # remove the fan colour if it is there
-    palette_colors = [
-        palette_color
-        for palette_color in palette_colors
-        if palette_color != fan_col_base
-    ]
-    if len(df_l) > 0:
-        series = list(df_l[series_col].unique())
-        for s in series:
-            # cycle through the colourway like plotly normally does, but skipping fan colour
-            # so other data is never the same colour as the quantile fan
-            srs_col = palette_colors[series.index(s) % len(palette_colors)]
-            df_x = df_l[df_l[series_col] == s]
-            # format the marker
-            line = dict(
-                color=srs_col,
-                width=1,
-            )
-            marker = dict(symbol="circle", color=srs_col, opacity=0.5, size=8)
-            fig.add_trace(
-                go.Scatter(
-                    y=df_x[series_value],
-                    x=df_x.from_dt,
-                    name=str(s),
-                    mode="lines+markers",
-                    line=line,
-                    marker=marker,
-                    hovertemplate=str(s) + ": %{y:.2f}<extra></extra>",
-                )
-            )
-
-    # if monochrome update all traces to monochrome colour
-    if monochrome == True:
-        col = graph_theme.monochrome_hex
-        fig.update_traces(patch={"marker_color": col, "line_color": col})
-
-    # update traces with user defined updates
-    fig = update_fig_traces(fig, trace_update)
-
-    # add vertical line
-    ref_dt = pd.to_datetime(df_q.ref_dt.unique()[0])
-    trace_col = graph_theme.pio_default_template().layout.yaxis.gridcolor
-    fig.add_trace(_scatter_now_line(ref_dt, trace_col))  # temp - fix this
-    return fig
-
-
-def _find_middle(input_list):
-    input_list = sorted(input_list)
-    middle = float(len(input_list)) / 2
-    if middle % 2 != 0:
-        return input_list[int(middle - 0.5)]
-    else:
-        return (input_list[int(middle)], input_list[int(middle - 1)])
-
-
-def _scatter_quantile_fan_error_test(df_q, df_l) -> bool:
-    """
-    Perform error checking. Raise error if not ok
-    """
-    # extract the quantiles
-    quantiles = df_q["quantile"].unique()
-
-    # quantiles
-    # if len(quantiles)!=3:
-    #    msg = "Expected to receive 3 quantiles to graph - a high, low and medium (or equivalent). Received instead: {}".format(quantiles)
-    #    raise ValueError(msg)
-    if not is_numeric(quantiles):
-        msg = "Expected quantiles to be numeric quantiles (check - are they string or simuilar?)"
-        raise ValueError(msg)
-    if not is_fraction(quantiles):
-        msg = "Expected fractional quantiles. Received {}".format(quantiles)
-        raise ValueError(msg)
-
-    # ref_dt
-    ref_dt = df_q.ref_dt.unique()
-    if len(ref_dt) > 1:
-        msg = (
-            "Expected only one ref_dt for the prediction quantiles. Received {}".format(
-                ref_dt
-            )
-        )
-        raise ValueError(msg)
-
-
-def _scatter_quantile_fan_layout(layout_update) -> dict:
-    """
-    Return a layout dict for the figure
-    """
-    # default
-    layout = go.Layout()
-
-    layout["yaxis"] = {"title": "€/MWh"}
-
-    # add the vertical nowline
-    layout["yaxis2"] = {
-        "anchor": "x",
-        "fixedrange": True,
-        "overlaying": "y",
-        "range": [0, 1],
-        "side": "right",
-        "visible": False,  # The secondary yaxis is invisible
-    }
-
-    layout["xaxis"] = layout["xaxis"].update(
-        dict(
-            hoverformat="%H:%M",
-            tickformat="%H",  # %d %B (%a)<br>%Y
-            dtick=86400000.0 / 24,
-            title=None,
-        )
-    )
-
-    # hovertext
-    layout["hoverlabel"] = dict(
-        font_size=10,
-    )
-
-    # update with any user instructions
-    if layout_update is not None:
-        layout = layout.update(go.Layout(layout_update))
-
-    return layout
-
-
-def _scatter_now_line(ref_dt, colour):
-
-    nowline = go.Scatter(
-        x=[ref_dt, ref_dt],
-        y=[0, 1],
-        mode="lines",
-        line=dict(shape="linear", width=1, dash="dot", color=colour),
-        showlegend=False,
-        xaxis="x",
-        yaxis="y2",
-        name="fcast built",
-        hoverinfo="skip",
-        hovertemplate="",
-    )
-    return nowline
-
-
-def is_numeric(obj):
-    try:
-        obj + obj, obj - obj, obj * obj, obj**obj, obj / obj
-    except ZeroDivisionError:
-        return True
-    except Exception:
-        return False
-    else:
-        return True
-
-
-def is_fraction(alist):
-    for l in alist:
-        if l > 1:
-            return False
-        if l < 0:
-            return False
-    return True
+import numpy as np
+import pandas as pd
+import plotly.graph_objects as go
+
+from ..assets import opt_plotly_theme as theme
+
+# import plotly.io as pio
+from ..common.utils import update_fig_traces
+
+
+def scatter_quantile_fan(
+    df_q: pd.DataFrame,
+    df_l: pd.DataFrame,
+    quantile_col="quantile",
+    quantile_value="value",
+    series_col="series",
+    series_value="value",
+    layout_update=None,
+    trace_update=None,
+    monochrome=False,
+) -> go.Figure:
+    """
+
+    Construct a scatter fan diagram
+
+    Inputs:
+
+    df_q -> dataframe for quantiles, with columns [from_dt, ref_dt, quantile, value]
+    df_l -> dataframe for all other data to graph, with columns [from_dt, series, value]
+
+    The function will graph df_q between min and max quantiles, and the median (0.5) quantile, as a fan
+    Each series in df_l will be graphed as a line
+
+    """
+
+    # get the active graph theme (or create one if there isnt one)
+    graph_theme = theme.FabPlotlyTheme()
+
+    # test params
+    _scatter_quantile_fan_error_test(df_q, df_l)
+
+    # extract the quantiles
+    quantiles = list(df_q[quantile_col].unique())
+    qmax = max(quantiles)
+    qmin = min(quantiles)
+    qmed = _find_middle(quantiles)
+
+    # Create a df for min, max, med. Just makes the graph code slightly easier to read
+    df_min = df_q[(df_q[quantile_col] == qmin)].copy()
+    df_max = df_q[(df_q[quantile_col] == qmax)].copy()
+    df_med = df_q[(df_q[quantile_col] == qmed)].copy()
+
+    # define the graph with our scatter fan layout
+    fig = go.Figure(layout=_scatter_quantile_fan_layout(layout_update))
+
+    # copy the colour palette for graphs
+    palette_colors = list(graph_theme.pio_default_template().layout.colorway)
+
+    # first the fan colour. We want this to be semi-transparent and the same colour as the first trace
+    # get the first colour in the colorway for the active (default) template
+
+    if monochrome:
+        fan_col_base = graph_theme.monochrome_hex
+    else:
+        fan_col_base = graph_theme.fan_hex
+    h = fan_col_base.lstrip("#")
+    fan_col_rgb_transp = list(int(h[i : i + 2], 16) for i in (0, 2, 4))
+    fan_col_rgb_transp.append(0.3)
+    fan_col_rgb_transp = "rgba" + str(tuple(fan_col_rgb_transp))
+
+    # upper and lower lines for the fan. set to be 100% transparent
+    fan_border_line = dict(color="rgba(0,0,0,0)")
+
+    # add the quantile fan
+    name = str(qmin * 100) + "%"
+    label = name
+    fig.add_trace(
+        go.Scatter(
+            y=df_min[quantile_value],
+            x=df_min.from_dt,
+            name=name,
+            mode="lines",
+            line=fan_border_line,
+            showlegend=False,
+            hovertemplate=label + ": %{y:.2f}<extra></extra>",
+        )
+    )
+
+    name = str(qmin * 100) + "%-<br>" + str(qmax * 100) + "%"
+    label = str(qmax * 100) + "%"
+    fig.add_trace(
+        go.Scatter(
+            y=df_max[quantile_value],
+            x=df_max.from_dt,
+            fill="tonexty",
+            fillcolor=fan_col_rgb_transp,
+            mode="lines",
+            line=fan_border_line,
+            name=name,
+            hovertemplate=label + ": %{y:.2f}<extra></extra>",
+        )
+    )
+
+    name = str(qmed * 100) + "%"
+    label = name
+    fig.add_trace(
+        go.Scatter(
+            y=df_med[quantile_value],
+            x=df_med.from_dt,
+            name=name,
+            mode="lines+markers",
+            hovertemplate=label + ": %{y:.2f}<extra></extra>",
+            marker=dict(symbol="circle", opacity=0.5, size=8, color=fan_col_base),
+            line=dict(color=fan_col_base),
+        )
+    )
+
+    # add the lines for the market prices if we have them
+    # remove the fan colour if it is there
+    palette_colors = [
+        palette_color
+        for palette_color in palette_colors
+        if palette_color != fan_col_base
+    ]
+    if len(df_l) > 0:
+        series = list(df_l[series_col].unique())
+        for s in series:
+            # cycle through the colourway like plotly normally does, but skipping fan colour
+            # so other data is never the same colour as the quantile fan
+            srs_col = palette_colors[series.index(s) % len(palette_colors)]
+            df_x = df_l[df_l[series_col] == s]
+            # format the marker
+            line = dict(
+                color=srs_col,
+                width=1,
+            )
+            marker = dict(symbol="circle", color=srs_col, opacity=0.5, size=8)
+            fig.add_trace(
+                go.Scatter(
+                    y=df_x[series_value],
+                    x=df_x.from_dt,
+                    name=str(s),
+                    mode="lines+markers",
+                    line=line,
+                    marker=marker,
+                    hovertemplate=str(s) + ": %{y:.2f}<extra></extra>",
+                )
+            )
+
+    # if monochrome update all traces to monochrome colour
+    if monochrome == True:
+        col = graph_theme.monochrome_hex
+        fig.update_traces(patch={"marker_color": col, "line_color": col})
+
+    # update traces with user defined updates
+    fig = update_fig_traces(fig, trace_update)
+
+    # add vertical line
+    ref_dt = pd.to_datetime(df_q.ref_dt.unique()[0])
+    trace_col = graph_theme.pio_default_template().layout.yaxis.gridcolor
+    fig.add_trace(_scatter_now_line(ref_dt, trace_col))  # temp - fix this
+    return fig
+
+
+def _find_middle(input_list):
+    input_list = sorted(input_list)
+    middle = float(len(input_list)) / 2
+    if middle % 2 != 0:
+        return input_list[int(middle - 0.5)]
+    else:
+        return (input_list[int(middle)], input_list[int(middle - 1)])
+
+
+def _scatter_quantile_fan_error_test(df_q, df_l) -> bool:
+    """
+    Perform error checking. Raise error if not ok
+    """
+    # extract the quantiles
+    quantiles = df_q["quantile"].unique()
+
+    # quantiles
+    # if len(quantiles)!=3:
+    #    msg = "Expected to receive 3 quantiles to graph - a high, low and medium (or equivalent). Received instead: {}".format(quantiles)
+    #    raise ValueError(msg)
+    if not is_numeric(quantiles):
+        msg = "Expected quantiles to be numeric quantiles (check - are they string or simuilar?)"
+        raise ValueError(msg)
+    if not is_fraction(quantiles):
+        msg = "Expected fractional quantiles. Received {}".format(quantiles)
+        raise ValueError(msg)
+
+    # ref_dt
+    ref_dt = df_q.ref_dt.unique()
+    if len(ref_dt) > 1:
+        msg = (
+            "Expected only one ref_dt for the prediction quantiles. Received {}".format(
+                ref_dt
+            )
+        )
+        raise ValueError(msg)
+
+
+def _scatter_quantile_fan_layout(layout_update) -> dict:
+    """
+    Return a layout dict for the figure
+    """
+    # default
+    layout = go.Layout()
+
+    layout["yaxis"] = {"title": "€/MWh"}
+
+    # add the vertical nowline
+    layout["yaxis2"] = {
+        "anchor": "x",
+        "fixedrange": True,
+        "overlaying": "y",
+        "range": [0, 1],
+        "side": "right",
+        "visible": False,  # The secondary yaxis is invisible
+    }
+
+    layout["xaxis"] = layout["xaxis"].update(
+        dict(
+            hoverformat="%H:%M",
+            tickformat="%H",  # %d %B (%a)<br>%Y
+            dtick=86400000.0 / 24,
+            title=None,
+        )
+    )
+
+    # hovertext
+    layout["hoverlabel"] = dict(
+        font_size=10,
+    )
+
+    # update with any user instructions
+    if layout_update is not None:
+        layout = layout.update(go.Layout(layout_update))
+
+    return layout
+
+
+def _scatter_now_line(ref_dt, colour):
+
+    nowline = go.Scatter(
+        x=[ref_dt, ref_dt],
+        y=[0, 1],
+        mode="lines",
+        line=dict(shape="linear", width=1, dash="dot", color=colour),
+        showlegend=False,
+        xaxis="x",
+        yaxis="y2",
+        name="fcast built",
+        hoverinfo="skip",
+        hovertemplate="",
+    )
+    return nowline
+
+
+def is_numeric(obj):
+    try:
+        obj + obj, obj - obj, obj * obj, obj**obj, obj / obj
+    except ZeroDivisionError:
+        return True
+    except Exception:
+        return False
+    else:
+        return True
+
+
+def is_fraction(alist):
+    for l in alist:
+        if l > 1:
+            return False
+        if l < 0:
+            return False
+    return True
```

### Comparing `fab-rk-tools-0.3.8/fab_rk_tools/graphs/trafficlight_scatter.py` & `fab_rk_tools-0.3.9/fab_rk_tools/graphs/trafficlight_scatter.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-from enum import Enum
-
-# import fab_rk_tools.assets.plotly_theme as theme
-# from ..assets import plotly_theme as theme
-from importlib import reload
-from math import floor
-
-import numpy as np
-import pandas as pd
-import plotly.graph_objects as go
-
-import fab_rk_tools.assets.opt_plotly_theme as theme
-from fab_rk_tools.common.utils import update_fig_traces
-
-
-def trafficlight_scatter(
-    df, layout_update=None, value_col="marker", marker_size=20, trace_update=None
-):
-    """
-    Traffic light scatter plot. Graphs a coloured circle (marker) per point, where the colours are specified in the input
-    dataframe ("RED", "GREEN" etc). The colour definitions are taken from a opt plotly theme object.
-
-    """
-
-    # Expanded plotly theme. If one is instansiated, then load it otherwise create one and use the default
-    graph_theme = theme.FabPlotlyTheme()
-    colours = graph_theme.hex_to_rgb(graph_theme.trafficlight_hex)
-
-    # fix layout
-    layout = _set_layout(layout_update)
-
-    # new figure
-    fig = go.Figure(layout=layout)
-
-    # specify marker colours for each point, in a df
-    marker_colours = _prepare_marker_colours(df, value_col, colours)
-
-    # marker line size
-    line_size = max(1, floor(marker_size / 3))
-
-    # add the trace for the graph
-
-    fig.add_trace(
-        go.Scatter(
-            x=marker_colours.from_dt,
-            y=np.zeros(len(marker_colours)),
-            mode="markers",
-            marker=dict(
-                color=list(marker_colours.marker_rgb),
-                symbol="circle",
-                size=marker_size,
-                line=dict(color=list(marker_colours.marker_rgba), width=line_size),
-            ),
-            showlegend=False,
-            # hoverinfo='none'
-        ),
-    )
-
-    # update traces with user defined updates
-    fig = update_fig_traces(fig, trace_update)
-
-    return fig
-
-
-def _set_layout(layout_update):
-    """
-    Generate the layout object for the graph
-    """
-
-    # basic layout, before adjustments
-    layout = go.Layout(
-        yaxis=dict(
-            range=[-1, 1],
-            showgrid=False,
-            zeroline=False,
-            visible=False,
-            fixedrange=True,
-        ),
-        height=140,
-        hovermode=False,
-    )
-
-    layout["xaxis"] = layout["xaxis"].update(
-        dict(
-            hoverformat="%H:%M",
-            tickformat="%H",  # %d %B (%a)<br>%Y
-            dtick=86400000.0 / 24,
-            title=None,
-            fixedrange=True,
-        )
-    )
-
-    # hovertext
-    layout["hoverlabel"] = dict(
-        font_size=10,
-    )
-
-    # update with any user instructions
-    if layout_update is not None:
-        layout = layout.update(go.Layout(layout_update))
-
-    return layout
-
-
-def _make_transparent(rgb, opacity=0.7):
-    """
-    make the rgb string into a transparent rgb string
-    """
-    return f"rgba{rgb[3:-1]}, {opacity})"
-
-
-def _prepare_marker_colours(df_data, value_col, colours, opacity=0.7):
-    """
-    Calculate the line and fill marker colours for each row in srs
-    """
-
-    # create dataframe for results
-    df = df_data[["from_dt", value_col]]
-
-    m_solid = "marker_rgb"
-    m_transparent = "marker_rgba"
-
-    if "default" in colours:
-        default_colour = colours["default"]
-    else:
-        default_colour = list(colours.values())[0]
-    # marker & line colours
-    df.loc[:, m_solid] = default_colour  # default to default colour
-    df.loc[:, m_transparent] = _make_transparent(
-        default_colour, opacity
-    )  # default to default colour
-
-    for colour, rgb in colours.items():
-        if colour != "default":
-            df.loc[df[value_col] == colour, m_solid] = rgb
-            df.loc[df[value_col] == colour, m_transparent] = _make_transparent(
-                rgb, opacity
-            )
-    return df
+from enum import Enum
+
+# import fab_rk_tools.assets.plotly_theme as theme
+# from ..assets import plotly_theme as theme
+from importlib import reload
+from math import floor
+
+import numpy as np
+import pandas as pd
+import plotly.graph_objects as go
+
+import fab_rk_tools.assets.opt_plotly_theme as theme
+from fab_rk_tools.common.utils import update_fig_traces
+
+
+def trafficlight_scatter(
+    df, layout_update=None, value_col="marker", marker_size=20, trace_update=None
+):
+    """
+    Traffic light scatter plot. Graphs a coloured circle (marker) per point, where the colours are specified in the input
+    dataframe ("RED", "GREEN" etc). The colour definitions are taken from a opt plotly theme object.
+
+    """
+
+    # Expanded plotly theme. If one is instansiated, then load it otherwise create one and use the default
+    graph_theme = theme.FabPlotlyTheme()
+    colours = graph_theme.hex_to_rgb(graph_theme.trafficlight_hex)
+
+    # fix layout
+    layout = _set_layout(layout_update)
+
+    # new figure
+    fig = go.Figure(layout=layout)
+
+    # specify marker colours for each point, in a df
+    marker_colours = _prepare_marker_colours(df, value_col, colours)
+
+    # marker line size
+    line_size = max(1, floor(marker_size / 3))
+
+    # add the trace for the graph
+
+    fig.add_trace(
+        go.Scatter(
+            x=marker_colours.from_dt,
+            y=np.zeros(len(marker_colours)),
+            mode="markers",
+            marker=dict(
+                color=list(marker_colours.marker_rgb),
+                symbol="circle",
+                size=marker_size,
+                line=dict(color=list(marker_colours.marker_rgba), width=line_size),
+            ),
+            showlegend=False,
+            # hoverinfo='none'
+        ),
+    )
+
+    # update traces with user defined updates
+    fig = update_fig_traces(fig, trace_update)
+
+    return fig
+
+
+def _set_layout(layout_update):
+    """
+    Generate the layout object for the graph
+    """
+
+    # basic layout, before adjustments
+    layout = go.Layout(
+        yaxis=dict(
+            range=[-1, 1],
+            showgrid=False,
+            zeroline=False,
+            visible=False,
+            fixedrange=True,
+        ),
+        height=140,
+        hovermode=False,
+    )
+
+    layout["xaxis"] = layout["xaxis"].update(
+        dict(
+            hoverformat="%H:%M",
+            tickformat="%H",  # %d %B (%a)<br>%Y
+            dtick=86400000.0 / 24,
+            title=None,
+            fixedrange=True,
+        )
+    )
+
+    # hovertext
+    layout["hoverlabel"] = dict(
+        font_size=10,
+    )
+
+    # update with any user instructions
+    if layout_update is not None:
+        layout = layout.update(go.Layout(layout_update))
+
+    return layout
+
+
+def _make_transparent(rgb, opacity=0.7):
+    """
+    make the rgb string into a transparent rgb string
+    """
+    return f"rgba{rgb[3:-1]}, {opacity})"
+
+
+def _prepare_marker_colours(df_data, value_col, colours, opacity=0.7):
+    """
+    Calculate the line and fill marker colours for each row in srs
+    """
+
+    # create dataframe for results
+    df = df_data[["from_dt", value_col]]
+
+    m_solid = "marker_rgb"
+    m_transparent = "marker_rgba"
+
+    if "default" in colours:
+        default_colour = colours["default"]
+    else:
+        default_colour = list(colours.values())[0]
+    # marker & line colours
+    df.loc[:, m_solid] = default_colour  # default to default colour
+    df.loc[:, m_transparent] = _make_transparent(
+        default_colour, opacity
+    )  # default to default colour
+
+    for colour, rgb in colours.items():
+        if colour != "default":
+            df.loc[df[value_col] == colour, m_solid] = rgb
+            df.loc[df[value_col] == colour, m_transparent] = _make_transparent(
+                rgb, opacity
+            )
+    return df
```

### Comparing `fab-rk-tools-0.3.8/fab_rk_tools/stats/distribution.py` & `fab_rk_tools-0.3.9/fab_rk_tools/stats/distribution.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-# Functions for calculating distribution related quantities and stats
-
-# Owner: Gavin Bell, Optimeering AS
-# Date created: 1 February 2022
-
-
-import numbers
-
-import numpy as np
-import pandas as pd
-
-TOL = 1e-4
-MIN_VALUTA = 0.01  # smallest unit of currency
-ROUND_DP = 2  # dp
-
-# -------
-# CUMULATIVE DISTRIBUTION
-# -------
-
-
-def cdf_result_from_quantiles(quantiles, values, test, inverse=False, dp=2):
-    """
-    Calculate either:
-     - value | P(X<=value) = probabiity
-     - probability => P(X<=value)
-
-    from the CDF described by the <quantiles, values> pairs
-
-    Inputs:
-    -------
-    quantiles -> list of quantiles
-    values -> list of values matching the quantiles
-    test -> random variable value or probability
-    inverse -> boolean, inverse or plain cdf. Inverse=True => value is returned, inverse=False => probability is returned
-    dp -> int, dp for result
-
-    Outputs:
-    --------
-    value (inverse=False) or probability (inverse=True)
-
-    """
-
-    # test the quantiles and values
-    if len(quantiles) != len(values):
-        msg = "Quantiles and value lengths must match. Quanitles={} Values = {}".format(
-            quantiles, values
-        )
-        raise ValueError(msg)
-
-    # sort the quantles and values
-    quantiles.sort()
-    values.sort()
-
-    if inverse:
-        if test < 0 or test > 1:
-            msg = f"Parameter test should be a probability (between 0 and 1). Value supplied = {test} "
-            raise ValueError(msg)
-        bracket_vals = quantiles
-        prob_vals = values
-    else:
-        bracket_vals = values
-        prob_vals = quantiles
-
-    # get the row indexes bracketing the sample value
-    idx = _get_bracketing_indexes(bracket_vals, test)
-
-    # interpolate
-    pos = _get_sample_pos(bracket_vals, test, idx)
-    result = pos * prob_vals[idx[1]] + (1 - pos) * prob_vals[idx[0]]
-
-    return round(result, dp)
-
-
-def _get_bracketing_indexes(values, sample_value):
-    """
-    Get the row indexes bracketing the sample value
-
-    If the sample value is less than the min value, returns row 0 only
-    If the sample value is greater than the max value, returns the last row only
-    o.w. returns the indexs of the values immediatley below and above the sample value
-    """
-
-    res = list(filter(lambda i: i > sample_value, values))
-    if res == []:
-        row1 = len(values) - 1
-        row2 = row1
-    elif res == values:
-        row1 = 0
-        row2 = 0
-    else:
-        row2 = values.index(res[0])
-        row1 = row2 - 1
-    return row1, row2
-
-
-def _get_sample_pos(values, sample_value, idx):
-    """
-    Get the position of the sample value relative to the bracketing values
-
-    pos = (s-v1)/(v2-v1)
-
-    """
-    if values[idx[0]] == values[idx[1]]:
-        pos = 1
-    else:
-        pos = (sample_value - values[idx[0]]) / (values[idx[1]] - values[idx[0]])
-    return pos
+# Functions for calculating distribution related quantities and stats
+
+# Owner: Gavin Bell, Optimeering AS
+# Date created: 1 February 2022
+
+
+import numbers
+
+import numpy as np
+import pandas as pd
+
+TOL = 1e-4
+MIN_VALUTA = 0.01  # smallest unit of currency
+ROUND_DP = 2  # dp
+
+# -------
+# CUMULATIVE DISTRIBUTION
+# -------
+
+
+def cdf_result_from_quantiles(quantiles, values, test, inverse=False, dp=2):
+    """
+    Calculate either:
+     - value | P(X<=value) = probabiity
+     - probability => P(X<=value)
+
+    from the CDF described by the <quantiles, values> pairs
+
+    Inputs:
+    -------
+    quantiles -> list of quantiles
+    values -> list of values matching the quantiles
+    test -> random variable value or probability
+    inverse -> boolean, inverse or plain cdf. Inverse=True => value is returned, inverse=False => probability is returned
+    dp -> int, dp for result
+
+    Outputs:
+    --------
+    value (inverse=False) or probability (inverse=True)
+
+    """
+
+    # test the quantiles and values
+    if len(quantiles) != len(values):
+        msg = "Quantiles and value lengths must match. Quanitles={} Values = {}".format(
+            quantiles, values
+        )
+        raise ValueError(msg)
+
+    # sort the quantles and values
+    quantiles.sort()
+    values.sort()
+
+    if inverse:
+        if test < 0 or test > 1:
+            msg = f"Parameter test should be a probability (between 0 and 1). Value supplied = {test} "
+            raise ValueError(msg)
+        bracket_vals = quantiles
+        prob_vals = values
+    else:
+        bracket_vals = values
+        prob_vals = quantiles
+
+    # get the row indexes bracketing the sample value
+    idx = _get_bracketing_indexes(bracket_vals, test)
+
+    # interpolate
+    pos = _get_sample_pos(bracket_vals, test, idx)
+    result = pos * prob_vals[idx[1]] + (1 - pos) * prob_vals[idx[0]]
+
+    return round(result, dp)
+
+
+def _get_bracketing_indexes(values, sample_value):
+    """
+    Get the row indexes bracketing the sample value
+
+    If the sample value is less than the min value, returns row 0 only
+    If the sample value is greater than the max value, returns the last row only
+    o.w. returns the indexs of the values immediatley below and above the sample value
+    """
+
+    res = list(filter(lambda i: i > sample_value, values))
+    if res == []:
+        row1 = len(values) - 1
+        row2 = row1
+    elif res == values:
+        row1 = 0
+        row2 = 0
+    else:
+        row2 = values.index(res[0])
+        row1 = row2 - 1
+    return row1, row2
+
+
+def _get_sample_pos(values, sample_value, idx):
+    """
+    Get the position of the sample value relative to the bracketing values
+
+    pos = (s-v1)/(v2-v1)
+
+    """
+    if values[idx[0]] == values[idx[1]]:
+        pos = 1
+    else:
+        pos = (sample_value - values[idx[0]]) / (values[idx[1]] - values[idx[0]])
+    return pos
```

### Comparing `fab-rk-tools-0.3.8/pyproject.toml` & `fab_rk_tools-0.3.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-[tool.poetry]
-name = "fab-rk-tools"
-version = "0.3.8"
-description = "Gavins rk tools and dinky things"
-authors = ["Gavin Bell"]
-packages = [
-    {include = "fab_rk_tools"}
-]
-
-[tool.poetry.dependencies]
-python = ">=3.9,<3.12"
-pandas = "*"
-numpy = "*"
-plotly = "*"
-archimedes-python-client = "*"
-
-[tool.poetry.dev-dependencies]
-pylint = "^2.14.1"
-isort = "^5.10.1"
-black = "^22.10.0"
-notebook = "*"
-coverage = "*"
-pytest = "^7.1.2"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "fab-rk-tools"
+version = "0.3.9"
+description = "Gavins rk tools and dinky things"
+authors = ["Gavin Bell"]
+packages = [
+    {include = "fab_rk_tools"}
+]
+
+[tool.poetry.dependencies]
+python = ">=3.9,<3.12"
+pandas = "*"
+numpy = "*"
+plotly = "*"
+archimedes-python-client = "*"
+
+[tool.poetry.dev-dependencies]
+pylint = "^2.14.1"
+isort = "^5.10.1"
+black = "^22.10.0"
+notebook = "*"
+coverage = "*"
+pytest = "^7.1.2"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `fab-rk-tools-0.3.8/setup.py` & `fab_rk_tools-0.3.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 {'': ['*']}
 
 install_requires = \
 ['archimedes-python-client', 'numpy', 'pandas', 'plotly']
 
 setup_kwargs = {
     'name': 'fab-rk-tools',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'Gavins rk tools and dinky things',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Gavin Bell',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<3.12',
 }
```

