# Comparing `tmp/oncoprinter-0.1.0.tar.gz` & `tmp/oncoprinter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oncoprinter-0.1.0.tar", last modified: Thu Feb  9 06:52:30 2023, max compression
+gzip compressed data, was "oncoprinter-0.2.0.tar", last modified: Wed Apr 26 10:10:16 2023, max compression
```

## Comparing `oncoprinter-0.1.0.tar` & `oncoprinter-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1271 2023-02-09 06:52:05.990382 oncoprinter-0.1.0/.github/workflows/build.yaml
--rw-r--r--   0        0        0     3099 2023-02-09 06:52:05.990382 oncoprinter-0.1.0/.gitignore
--rw-r--r--   0        0        0     1064 2023-02-09 06:52:05.990382 oncoprinter-0.1.0/LICENSE
--rw-r--r--   0        0        0      109 2023-02-09 06:52:05.990382 oncoprinter-0.1.0/README.md
--rw-r--r--   0        0        0      129 2023-02-09 06:52:05.990382 oncoprinter-0.1.0/oncoprinter/__init__.py
--rw-r--r--   0        0        0     7438 2023-02-09 06:52:05.990382 oncoprinter-0.1.0/oncoprinter/core.py
--rw-r--r--   0        0        0     9515 2023-02-09 06:52:05.990382 oncoprinter-0.1.0/oncoprinter/preset.py
--rw-r--r--   0        0        0      441 2023-02-09 06:52:05.990382 oncoprinter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       56 2023-02-09 06:52:05.990382 oncoprinter-0.1.0/setup.py
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 oncoprinter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1271 2023-04-26 10:09:50.452093 oncoprinter-0.2.0/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     3099 2023-04-26 10:09:50.452093 oncoprinter-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1064 2023-04-26 10:09:50.456093 oncoprinter-0.2.0/LICENSE
+-rw-r--r--   0        0        0      109 2023-04-26 10:09:50.456093 oncoprinter-0.2.0/README.md
+-rw-r--r--   0        0        0      129 2023-04-26 10:09:50.456093 oncoprinter-0.2.0/oncoprinter/__init__.py
+-rw-r--r--   0        0        0     8505 2023-04-26 10:09:50.456093 oncoprinter-0.2.0/oncoprinter/core.py
+-rw-r--r--   0        0        0     9542 2023-04-26 10:09:50.456093 oncoprinter-0.2.0/oncoprinter/preset.py
+-rw-r--r--   0        0        0      484 2023-04-26 10:09:50.456093 oncoprinter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-04-26 10:09:50.456093 oncoprinter-0.2.0/setup.py
+-rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 oncoprinter-0.2.0/PKG-INFO
```

### Comparing `oncoprinter-0.1.0/.github/workflows/build.yaml` & `oncoprinter-0.2.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `oncoprinter-0.1.0/.gitignore` & `oncoprinter-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oncoprinter-0.1.0/LICENSE` & `oncoprinter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oncoprinter-0.1.0/oncoprinter/core.py` & `oncoprinter-0.2.0/oncoprinter/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,214 +1,260 @@
 import warnings
 from collections import Counter
-from itertools import count
 from copy import deepcopy
+from dataclasses import dataclass
+from itertools import count
+from typing import Any
 
 import numpy as np
 import pandas as pd
+from marsilea import ClusterBoard
+from marsilea.layers import LayersMesh, FrameRect, Piece
+from marsilea.plotter import Labels, StackBar, Numbers, ColorMesh
+from marsilea.utils import get_canvas_size_by_data
 
-from heatgraphy import ClusterBoard, Heatmap
-from heatgraphy.layers import LayersMesh, FrameRect
-from heatgraphy.plotter import Labels, StackBar
-from heatgraphy.utils import get_canvas_size_by_data
 from .preset import SHAPE_BANK, MATCH_POOL, Alteration
 
 
 def guess_alteration(event: str):
     for alt, rule in MATCH_POOL.items():
         if rule.is_match(event):
             return alt
     return Alteration.OTHER
 
 
+@dataclass(repr=False)
+class LayerData:
+    matrix: np.ndarray
+    piece: Piece
+    color: Any
+    event: Any
+
+    def __repr__(self):
+        return f"{self.piece.label} ({self.color})"
+
+
 class GenomicData:
     """Handle class for genomics data
 
     Parameters
     ----------
     data : pd.DataFrame
         Each column is:
-            1) Patient name
-            2) Track/Gene name
-            3) Alteration event
+            1) Sample ID
+            2) Track name
+            3) Alteration
+
     """
 
+    def __repr__(self):
+        ntrack, nsample = self.shape
+        return f"{ntrack} Tracks, {nsample} Samples with " \
+               f"{len(self.events)} Alterations"
+
     def __init__(self,
                  data,
-                 patients_order=None,
+                 samples_order=None,
                  tracks_order=None,
                  custom_pieces=None,
-                 background_color="#BEBEBE",
                  ):
         self.data = data.copy()
-        self.data.columns = ['patient', 'track', 'event']
+        self.data.columns = ['sample', 'track', 'event']
+
+        if samples_order is None:
+            samples_order = self.data['sample'].unique()
 
-        if patients_order is None:
-            patients_order = self.data['patient'].unique()
-        self.patients = patients_order
-        self._patients_ix = dict(zip(patients_order, count(0, 1)))
+        self.samples = samples_order
+        self._patients_ix = dict(zip(samples_order, count(0, 1)))
 
         if tracks_order is None:
             tracks_order = self.data['track'].unique()
         self.tracks = tracks_order
         self._tracks_ix = dict(zip(tracks_order, count(0, 1)))
 
+        self._shape = (len(self.tracks), len(self.samples))
+
         if custom_pieces is None:
             custom_pieces = {}
-        custom_events = list(custom_pieces.keys())
         self.custom_pieces = custom_pieces
 
+        self._process_alterations()
+
+        layers = {}
+        for e in self.events:
+            layers[e] = np.zeros(self._shape, dtype=bool)
+
+        for _, row in self.data.iterrows():
+            patient, track, event = row
+            row_ix = self._tracks_ix[track]
+            col_ix = self._patients_ix[patient]
+            layers[event][row_ix, col_ix] = True
+
+        self.layers = layers
+
+    def _process_alterations(self):
+        events_alt = dict()
+        custom_events = list(self.custom_pieces.keys())
         raw_events = self.data['event'].unique()
-        self.events_alt = dict()
 
         unknown_alterations = []
         for e in raw_events:
             alt = guess_alteration(e)
             if alt == Alteration.OTHER:
                 alt = e
                 if e not in custom_events:
                     unknown_alterations.append(e)
-            self.events_alt[e] = alt
-        self.data['event'] = [self.events_alt[e] for e in self.data['event']]
+            events_alt[e] = alt
+        self.data['event'] = [events_alt[e] for e in self.data['event']]
         self.events = self.data['event'].unique()
         if len(unknown_alterations) > 0:
-            msg = f"Found unknown alterations: {unknown_alterations}, "\
+            msg = f"Found unknown alterations: {unknown_alterations}, " \
                   f"please specify a piece for this alteration."
             warnings.warn(msg)
 
-        self._shape = (len(self.tracks), len(self.patients))
-        self.background_color = background_color
-
     @property
     def shape(self):
         return self._shape
 
-    def get_layers_pieces(self):
-        layers = {}
-        for e in self.events:
-            layers[e] = np.zeros(self._shape, dtype=bool)
-
-        for _, row in self.data.iterrows():
-            patient, track, event = row
-            row_ix = self._tracks_ix[track]
-            col_ix = self._patients_ix[patient]
-            layers[event][row_ix, col_ix] = True
+    def get_layers_data(self, background_color="#BEBEBE"):
 
         # explicitly make copy
         bg_pieces = deepcopy(SHAPE_BANK[Alteration.BACKGROUND])
-        bg_pieces.background_color = self.background_color
-        new_pieces = [bg_pieces]
-        new_layers = [np.ones(self._shape)]
-        colors = []
+        bg_pieces.background_color = background_color
+
+        # Add background layer
+        layers_data = [LayerData(np.ones(self._shape), bg_pieces,
+                                 background_color, Alteration.BACKGROUND)]
         for alt in self.events:
-            new_layers.append(layers[alt])
+
+            layer = self.layers[alt]
             if not isinstance(alt, Alteration):
                 piece = self.custom_pieces.get(alt)
                 if piece is None:
                     # The default style for OTHER
                     piece = FrameRect(color="pink", label=alt)
-                    piece.background_color = self.background_color
-                    colors.append("pink")
                 else:
                     piece = deepcopy(piece)
-                    piece.background_color = self.background_color
-                    colors.append(piece.color)
-                new_pieces.append(piece)
             else:
-                p = deepcopy(SHAPE_BANK[alt])
-                p.background_color = self.background_color
-                new_pieces.append(p)
-                colors.append(p.color)
+                piece = deepcopy(SHAPE_BANK[alt])
+            color = piece.color
+            piece.background_color = background_color
 
-        return new_layers, new_pieces, colors
+            layers_data.append(LayerData(layer, piece, color, alt))
+
+        return layers_data
 
     def get_track_mutation_rate(self):
         gb = self.data.groupby('track', sort=False, observed=True)
         ts = {}
         for track, df in gb:
-            ts[track] = len(df['patient'].unique())
+            ts[track] = len(df['sample'].unique())
         counts = np.array([ts[t] for t in self.tracks])
-        return counts / len(self.patients)
+        return counts / len(self.samples)
 
     def get_track_mutation_types(self):
         gb = self.data.groupby('track', sort=False, observed=True)
         cs = {}
         for track, df in gb:
             cs[track] = Counter(df['event'])
-        types = [cs[t] for t in self.tracks]
-        return pd.DataFrame(types).loc[::-1, self.events].fillna(0.).T
+        return pd.DataFrame(cs).fillna(0.)
 
-    def get_patient_mutation_types(self):
-        gb = self.data.groupby('patient', sort=False, observed=True)
+    def get_sample_mutation_types(self):
+        gb = self.data.groupby('sample', sort=False, observed=True)
         cs = {}
         for track, df in gb:
             cs[track] = Counter(df['event'])
-        types = [cs[p] for p in self.patients]
-        return pd.DataFrame(types).loc[:, self.events].fillna(0.).T
+        return pd.DataFrame(cs).fillna(0.)
 
 
-class OncoPrint:
+class OncoPrint(ClusterBoard):
 
     def __init__(self, genomic_data=None,
                  patients_order=None,
                  tracks_order=None,
                  pieces=None,
                  background_color="#BEBEBE",
                  shrink=(.8, .8),
                  width=None,
                  height=None,
                  aspect=2.5,
                  legend_kws=None,
                  name=None,
                  ):
         data = GenomicData(genomic_data,
-                           patients_order=patients_order,
+                           samples_order=patients_order,
                            tracks_order=tracks_order,
                            custom_pieces=pieces,
-                           background_color=background_color)
-        self.data = data
+                           )
+        self.genomic_data = data
         width, height = get_canvas_size_by_data(
             data.shape, width=width, height=height, scale=.2, aspect=aspect)
-        self.canvas = ClusterBoard(
+
+        self.canvas = super().__init__(
             name=name,
             cluster_data=np.zeros(data.shape),
             width=width, height=height)
-        layers, pieces, bar_colors = data.get_layers_pieces()
-        track_names = data.tracks
 
-        legend_options = dict(handleheight=aspect, handlelength=1)
+        legend_options = dict(title="Alterations",
+                              handleheight=aspect,
+                              handlelength=1)
         legend_kws = {} if legend_kws is None else legend_kws
         legend_options.update(legend_kws)
 
+        layers, pieces, colors_mapper = [], [], {}
+        for layer in data.get_layers_data(background_color):
+            layers.append(layer.matrix)
+            pieces.append(layer.piece)
+            colors_mapper[layer.event] = layer.color
         mesh = LayersMesh(layers=layers, pieces=pieces,
                           shrink=shrink, legend_kws=legend_options)
-        self.canvas.add_layer(mesh)
-        self.canvas.add_left(Labels(track_names, text_pad=.1))
+        self.add_layer(mesh)
+
+        self.add_left(Labels(data.tracks))
+
         # Add other statistics
         track_mut_rate = data.get_track_mutation_rate()
         # Convert to percentage string
-        rates = [f"{i}%" for i in (np.array(track_mut_rate) * 100).astype(int)]
-        self.canvas.add_right(Labels(rates, text_pad=.1))
-
-        track_counter = data.get_track_mutation_types()
-        track_bar = StackBar(track_counter, colors=bar_colors,
+        rates = [_format_percentage(t) for t in track_mut_rate]
+        self.add_right(Labels(rates))
+        self.add_bottom(Labels(data.samples))
+
+        track_counter = data.get_track_mutation_types().loc[:, ::-1]
+        colors = [colors_mapper[e] for e in track_counter.index]
+        track_bar = StackBar(track_counter, colors=colors,
                              show_value=False)
-        self.canvas.add_right(track_bar, legend=False)
+        self.add_right(track_bar, legend=False)
 
-        patients_counter = data.get_patient_mutation_types()
-        patients_bar = StackBar(patients_counter, colors=bar_colors,
+        patients_counter = data.get_sample_mutation_types()
+        colors = [colors_mapper[e] for e in patients_counter.index]
+        patients_bar = StackBar(patients_counter, colors=colors,
                                 show_value=False)
-        self.canvas.add_top(patients_bar, legend=False, pad=.1)
+        self.add_top(patients_bar, legend=False, pad=.1)
+        self.add_legends()
 
-    def render(self):
-        self.canvas.add_legends()
-        self.canvas.render()
+    clinical_plots = {
+        "bar": Numbers,
+        "stack_bar": StackBar,
+    }
+
+    def add_clinical_data(self, data, plot="bar",
+                          size=None, pad=.1, **kwargs):
+        data = data.loc[self.samples_order]
+        plotter = self.clinical_plots[plot]
+        self.add_bottom(plotter(data, **kwargs), size=size, pad=pad)
+
+    def add_heatmap_data(self, data, size=.2, pad=.1, **kwargs):
+        data = data.loc[self.samples_order]
+        options = {"cmap": "Blues", "label_loc": "left", **kwargs}
+        self.add_bottom(ColorMesh(data, **options), size=size, pad=pad)
 
     @property
-    def patients_order(self):
-        return self.data.patients
+    def samples_order(self):
+        return self.genomic_data.samples
 
     @property
     def tracks_order(self):
-        return self.data.tracks
+        return self.genomic_data.tracks
 
 
+def _format_percentage(t):
+    return f"{float(t) * 100:.2f}".rstrip('0').rstrip('.') + "%"
```

### Comparing `oncoprinter-0.1.0/oncoprinter/preset.py` & `oncoprinter-0.2.0/oncoprinter/preset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from dataclasses import dataclass, field
 from enum import Enum, auto
 from typing import List
 
+import marsilea.layers as mlayers
 import numpy as np
-
-import heatgraphy.layers as hl
-from matplotlib.patches import Rectangle
 from matplotlib.collections import PatchCollection
+from matplotlib.patches import Rectangle
 
 # The preset follows the style of cBioPortal as much as possible
 # https://github.com/cBioPortal/cbioportal-frontend/blob/master/src/shared/components/oncoprint/geneticrules.ts
 MUT_COLOR_MISSENSE = '#008000'
 MUT_COLOR_MISSENSE_PASSENGER = '#53D400'
 MUT_COLOR_INFRAME = '#993404'
 MUT_COLOR_INFRAME_PASSENGER = '#a68028'
@@ -81,23 +80,23 @@
         if self.background_color is not None:
             arts.append(
                 Rectangle((x, y), w, h, facecolor=self.background_color))
         arts.append(self.draw(x, y, w, h, None))
         return PatchCollection(arts, match_original=True)
 
 
-class Rect(_AltPiece, hl.Rect):
+class Rect(_AltPiece, mlayers.Rect):
     pass
 
 
-class FrameRect(_AltPiece, hl.FrameRect):
+class FrameRect(_AltPiece, mlayers.FrameRect):
     pass
 
 
-class FracRect(_AltPiece, hl.FracRect):
+class FracRect(_AltPiece, mlayers.FracRect):
     pass
 
 
 @dataclass(repr=False)
 class MatchRule:
     startswith: str = None
     endswith: str = None
@@ -162,73 +161,123 @@
                                              flexible=True),
     Alteration.SPLICE_PASSENGER: MatchRule(startswith='splice',
                                            contains=['passenger']),
     Alteration.SPLICE: MatchRule(startswith='splice'),
 }
 
 SHAPE_BANK = {
-    Alteration.BACKGROUND: Rect(color=DEFAULT_GREY, label="No alterations",
-                                zorder=-10000),
+    Alteration.BACKGROUND:
+        Rect(color=DEFAULT_GREY,
+             label="No alterations",
+             zorder=-10000),
     # CNA
-    Alteration.AMP: Rect(color=CNA_COLOR_AMP, label="Amplification"),
+    Alteration.AMP:
+        Rect(color=CNA_COLOR_AMP,
+             label="Amplification"),
     # ShapeId.ampRectangle
-    Alteration.GAIN: Rect(color=CNA_COLOR_GAIN, label="Gain"),
+    Alteration.GAIN:
+        Rect(color=CNA_COLOR_GAIN,
+             label="Gain"),
     # ShapeId.gainRectangle
-    Alteration.HOMDEL: Rect(color=CNA_COLOR_HOMDEL, label="Deep Deletion"),
-    Alteration.HETLOSS: Rect(color=CNA_COLOR_HETLOSS,
-                             label="Shallow Deletion"),
+    Alteration.HOMDEL:
+        Rect(color=CNA_COLOR_HOMDEL,
+             label="Deep Deletion"),
+    Alteration.HETLOSS:
+        Rect(color=CNA_COLOR_HETLOSS,
+             label="Shallow Deletion"),
     # mRNA Regulation
-    Alteration.MRNA_HIGH: FrameRect(color=MRNA_COLOR_HIGH, width=.6,
-                                    label="mRNA High", zorder=1000),
-    Alteration.MRNA_LOW: FrameRect(color=MRNA_COLOR_LOW, width=.6,
-                                   label="mRNA Low", zorder=1000),
+    Alteration.MRNA_HIGH:
+        FrameRect(color=MRNA_COLOR_HIGH,
+                  width=1.5,
+                  label="mRNA High",
+                  zorder=1000),
+    Alteration.MRNA_LOW:
+        FrameRect(color=MRNA_COLOR_LOW,
+                  width=1.5,
+                  label="mRNA Low",
+                  zorder=1000),
     # Protein Expression Regulation
-    Alteration.PROTEIN_HIGH: FracRect(color=PROT_COLOR_HIGH, frac=(1., .2),
-                                      label="Protein High", zorder=20),
-    Alteration.PROTEIN_LOW: FracRect(color=PROT_COLOR_LOW, frac=(1., .2),
-                                     label="Protein Low", zorder=20),
+    Alteration.PROTEIN_HIGH:
+        FracRect(color=PROT_COLOR_HIGH,
+                 frac=(1., .2),
+                 label="Protein High",
+                 zorder=100),
+    Alteration.PROTEIN_LOW:
+        FracRect(color=PROT_COLOR_LOW,
+                 frac=(1., .2),
+                 label="Protein Low",
+                 zorder=100),
     # Structural variant
-    Alteration.STRUCTURAL_VARIANT: FracRect(color=STRUCTURAL_VARIANT_COLOR,
-                                            frac=(1., .6),
-                                            label="Structural variant",
-                                            zorder=30),
-    Alteration.STRUCTURAL_VARIANT_PASSENGER: FracRect(
-        color=STRUCTURAL_VARIANT_PASSENGER_COLOR, frac=(1., .6),
-        label="Structural variant (putative passenger)", zorder=30),
-    Alteration.FUSION: FracRect(color=MUT_COLOR_FUSION, frac=(1., .6),
-                                label="Fusion", zorder=30),
+    Alteration.STRUCTURAL_VARIANT:
+        FracRect(color=STRUCTURAL_VARIANT_COLOR,
+                 frac=(1., .6),
+                 label="Structural variant",
+                 zorder=200),
+    Alteration.STRUCTURAL_VARIANT_PASSENGER:
+        FracRect(color=STRUCTURAL_VARIANT_PASSENGER_COLOR,
+                 frac=(1., .6),
+                 label="Structural variant (putative passenger)",
+                 zorder=200),
+    Alteration.FUSION:
+        FracRect(color=MUT_COLOR_FUSION,
+                 frac=(1., .6),
+                 label="Fusion",
+                 zorder=200),
     # Splice
-    Alteration.SPLICE: FracRect(color=MUT_COLOR_SPLICE, frac=(1., .3),
-                                label="Splice Mutation", zorder=40),
-    Alteration.SPLICE_PASSENGER: FracRect(color=MUT_COLOR_SPLICE_PASSENGER,
-                                          frac=(1., .3),
-                                          label="Splice Mutation (putative passenger)",
-                                          zorder=40),
-
-    Alteration.MISSENSE: FracRect(color=MUT_COLOR_MISSENSE, frac=(1., .3),
-                                  label="Mutation (putative driver)",
-                                  zorder=40),
-    Alteration.MISSENSE_PASSENGER: FracRect(color=MUT_COLOR_MISSENSE_PASSENGER,
-                                            frac=(1., .3),
-                                            label="Missense Mutation (putative passenger)",
-                                            zorder=40),
-    Alteration.OTHER: FracRect(color=MUT_COLOR_OTHER, frac=(1., .3),
-                               label="Other Mutation", zorder=40),
-    Alteration.PROMOTER: FracRect(color=MUT_COLOR_PROMOTER, frac=(1., .3),
-                                  label="Promoter Mutation", zorder=40),
-    Alteration.TRUNC: FracRect(color=MUT_COLOR_TRUNC, frac=(1., .3),
-                               label="Truncating Mutation", zorder=40),
-    Alteration.TRUNC_PASSENGER: FracRect(color=MUT_COLOR_TRUNC_PASSENGER,
-                                         frac=(1., .3),
-                                         label="Truncating Mutation (putative passenger)",
-                                         zorder=40),
-    Alteration.INFRAME: FracRect(color=MUT_COLOR_INFRAME, frac=(1., .3),
-                                 label="Inframe Mutation (putative driver)",
-                                 zorder=40),
-    Alteration.INFRAME_PASSENGER: FracRect(color=MUT_COLOR_INFRAME_PASSENGER,
-                                           frac=(1., .3),
-                                           label="Inframe Mutation (putative passenger)",
-                                           zorder=40),
+    Alteration.SPLICE:
+        FracRect(color=MUT_COLOR_SPLICE,
+                 frac=(1., .3),
+                 label="Splice Mutation",
+                 zorder=400),
+    Alteration.SPLICE_PASSENGER:
+        FracRect(color=MUT_COLOR_SPLICE_PASSENGER,
+                 frac=(1., .3),
+                 label="Splice Mutation (putative passenger)",
+                 zorder=400),
+
+    Alteration.MISSENSE:
+        FracRect(color=MUT_COLOR_MISSENSE,
+                 frac=(1., .3),
+                 label="Mutation (putative driver)",
+                 zorder=400),
+    Alteration.MISSENSE_PASSENGER:
+        FracRect(color=MUT_COLOR_MISSENSE_PASSENGER,
+                 frac=(1., .3),
+                 label="Missense Mutation (putative passenger)",
+                 zorder=400),
+    Alteration.OTHER:
+        FracRect(color=MUT_COLOR_OTHER,
+                 frac=(1., .3),
+                 label="Other Mutation",
+                 zorder=400),
+    Alteration.PROMOTER:
+        FracRect(color=MUT_COLOR_PROMOTER,
+                 frac=(1., .3),
+                 label="Promoter Mutation",
+                 zorder=400),
+    Alteration.TRUNC:
+        FracRect(color=MUT_COLOR_TRUNC,
+                 frac=(1., .3),
+                 label="Truncating Mutation",
+                 zorder=400),
+    Alteration.TRUNC_PASSENGER:
+        FracRect(color=MUT_COLOR_TRUNC_PASSENGER,
+                 frac=(1., .3),
+                 label="Truncating Mutation (putative passenger)",
+                 zorder=400),
+    Alteration.INFRAME:
+        FracRect(color=MUT_COLOR_INFRAME,
+                 frac=(1., .3),
+                 label="Inframe Mutation (putative driver)",
+                 zorder=400),
+    Alteration.INFRAME_PASSENGER:
+        FracRect(color=MUT_COLOR_INFRAME_PASSENGER,
+                 frac=(1., .3),
+                 label="Inframe Mutation (putative passenger)",
+                 zorder=400),
     # Germline
-    Alteration.GERMLINE: FracRect(color=MUT_COLOR_GERMLINE, frac=(1., .1),
-                                  label="Germline Mutation", zorder=60),
+    Alteration.GERMLINE:
+        FracRect(color=MUT_COLOR_GERMLINE,
+                 frac=(1., .1),
+                 label="Germline Mutation",
+                 zorder=600),
 }
```

