# Comparing `tmp/abjad-ext-nauert-3.8.tar.gz` & `tmp/abjad-ext-nauert-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abjad-ext-nauert-3.8.tar", last modified: Fri Apr  8 15:58:39 2022, max compression
+gzip compressed data, was "abjad-ext-nauert-3.9.tar", last modified: Sun May  1 13:33:33 2022, max compression
```

## Comparing `abjad-ext-nauert-3.8.tar` & `abjad-ext-nauert-3.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-04-08 15:58:39.170492 abjad-ext-nauert-3.8/
--rw-r--r--   0 trevor     (501) staff       (20)     1067 2022-03-01 07:52:43.000000 abjad-ext-nauert-3.8/LICENSE
--rw-r--r--   0 trevor     (501) staff       (20)      101 2022-03-01 07:52:43.000000 abjad-ext-nauert-3.8/MANIFEST.in
--rw-r--r--   0 trevor     (501) staff       (20)      732 2022-04-08 15:58:39.170102 abjad-ext-nauert-3.8/PKG-INFO
--rw-r--r--   0 trevor     (501) staff       (20)       80 2022-03-01 07:52:43.000000 abjad-ext-nauert-3.8/README.md
-drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-04-08 15:58:39.153733 abjad-ext-nauert-3.8/abjad_ext_nauert.egg-info/
--rw-r--r--   0 trevor     (501) staff       (20)      732 2022-04-08 15:58:39.000000 abjad-ext-nauert-3.8/abjad_ext_nauert.egg-info/PKG-INFO
--rw-r--r--   0 trevor     (501) staff       (20)      799 2022-04-08 15:58:39.000000 abjad-ext-nauert-3.8/abjad_ext_nauert.egg-info/SOURCES.txt
--rw-r--r--   0 trevor     (501) staff       (20)        1 2022-04-08 15:58:39.000000 abjad-ext-nauert-3.8/abjad_ext_nauert.egg-info/dependency_links.txt
--rw-r--r--   0 trevor     (501) staff       (20)       11 2022-04-08 15:58:39.000000 abjad-ext-nauert-3.8/abjad_ext_nauert.egg-info/requires.txt
--rw-r--r--   0 trevor     (501) staff       (20)        9 2022-04-08 15:58:39.000000 abjad-ext-nauert-3.8/abjad_ext_nauert.egg-info/top_level.txt
-drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-04-08 15:58:39.154897 abjad-ext-nauert-3.8/abjadext/
--rw-r--r--   0 trevor     (501) staff       (20)      119 2022-03-01 07:52:43.000000 abjad-ext-nauert-3.8/abjadext/__init__.py
-drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-04-08 15:58:39.169324 abjad-ext-nauert-3.8/abjadext/nauert/
--rw-r--r--   0 trevor     (501) staff       (20)     2211 2022-03-01 07:52:43.000000 abjad-ext-nauert-3.8/abjadext/nauert/__init__.py
--rw-r--r--   0 trevor     (501) staff       (20)      131 2022-04-08 15:54:26.000000 abjad-ext-nauert-3.8/abjadext/nauert/_version.py
--rw-r--r--   0 trevor     (501) staff       (20)    12968 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/attackpointoptimizers.py
--rw-r--r--   0 trevor     (501) staff       (20)    15906 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/gracehandlers.py
--rw-r--r--   0 trevor     (501) staff       (20)     2905 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/heuristics.py
--rw-r--r--   0 trevor     (501) staff       (20)     3451 2022-03-01 07:52:43.000000 abjad-ext-nauert-3.8/abjadext/nauert/jobhandlers.py
--rw-r--r--   0 trevor     (501) staff       (20)     2967 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/qeventproxy.py
--rw-r--r--   0 trevor     (501) staff       (20)     6871 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/qevents.py
--rw-r--r--   0 trevor     (501) staff       (20)    19416 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/qeventsequence.py
--rw-r--r--   0 trevor     (501) staff       (20)    17766 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/qgrid.py
--rw-r--r--   0 trevor     (501) staff       (20)     5963 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/qschemaitems.py
--rw-r--r--   0 trevor     (501) staff       (20)    21199 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/qschemas.py
--rw-r--r--   0 trevor     (501) staff       (20)    18632 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/qtargetitems.py
--rw-r--r--   0 trevor     (501) staff       (20)    16147 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/qtargets.py
--rw-r--r--   0 trevor     (501) staff       (20)     7051 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/quantizationjob.py
--rw-r--r--   0 trevor     (501) staff       (20)    10099 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/quantizer.py
--rw-r--r--   0 trevor     (501) staff       (20)    13736 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.8/abjadext/nauert/searchtrees.py
--rw-r--r--   0 trevor     (501) staff       (20)        0 2022-04-08 14:46:43.000000 abjad-ext-nauert-3.8/abjadext/py.typed
--rw-r--r--   0 trevor     (501) staff       (20)       38 2022-04-08 15:58:39.170601 abjad-ext-nauert-3.8/setup.cfg
--rw-r--r--   0 trevor     (501) staff       (20)     1617 2022-04-08 15:54:26.000000 abjad-ext-nauert-3.8/setup.py
+drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-05-01 13:33:33.299990 abjad-ext-nauert-3.9/
+-rw-r--r--   0 trevor     (501) staff       (20)     1067 2022-03-01 07:52:43.000000 abjad-ext-nauert-3.9/LICENSE
+-rw-r--r--   0 trevor     (501) staff       (20)      101 2022-03-01 07:52:43.000000 abjad-ext-nauert-3.9/MANIFEST.in
+-rw-r--r--   0 trevor     (501) staff       (20)      732 2022-05-01 13:33:33.299458 abjad-ext-nauert-3.9/PKG-INFO
+-rw-r--r--   0 trevor     (501) staff       (20)       80 2022-03-01 07:52:43.000000 abjad-ext-nauert-3.9/README.md
+drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-05-01 13:33:33.282443 abjad-ext-nauert-3.9/abjad_ext_nauert.egg-info/
+-rw-r--r--   0 trevor     (501) staff       (20)      732 2022-05-01 13:33:33.000000 abjad-ext-nauert-3.9/abjad_ext_nauert.egg-info/PKG-INFO
+-rw-r--r--   0 trevor     (501) staff       (20)      799 2022-05-01 13:33:33.000000 abjad-ext-nauert-3.9/abjad_ext_nauert.egg-info/SOURCES.txt
+-rw-r--r--   0 trevor     (501) staff       (20)        1 2022-05-01 13:33:33.000000 abjad-ext-nauert-3.9/abjad_ext_nauert.egg-info/dependency_links.txt
+-rw-r--r--   0 trevor     (501) staff       (20)       11 2022-05-01 13:33:33.000000 abjad-ext-nauert-3.9/abjad_ext_nauert.egg-info/requires.txt
+-rw-r--r--   0 trevor     (501) staff       (20)        9 2022-05-01 13:33:33.000000 abjad-ext-nauert-3.9/abjad_ext_nauert.egg-info/top_level.txt
+drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-05-01 13:33:33.283662 abjad-ext-nauert-3.9/abjadext/
+-rw-r--r--   0 trevor     (501) staff       (20)      119 2022-03-01 07:52:43.000000 abjad-ext-nauert-3.9/abjadext/__init__.py
+drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-05-01 13:33:33.298619 abjad-ext-nauert-3.9/abjadext/nauert/
+-rw-r--r--   0 trevor     (501) staff       (20)     2211 2022-03-01 07:52:43.000000 abjad-ext-nauert-3.9/abjadext/nauert/__init__.py
+-rw-r--r--   0 trevor     (501) staff       (20)      131 2022-05-01 13:31:45.000000 abjad-ext-nauert-3.9/abjadext/nauert/_version.py
+-rw-r--r--   0 trevor     (501) staff       (20)    12968 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.9/abjadext/nauert/attackpointoptimizers.py
+-rw-r--r--   0 trevor     (501) staff       (20)    15908 2022-05-01 13:08:19.000000 abjad-ext-nauert-3.9/abjadext/nauert/gracehandlers.py
+-rw-r--r--   0 trevor     (501) staff       (20)     2905 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.9/abjadext/nauert/heuristics.py
+-rw-r--r--   0 trevor     (501) staff       (20)     3451 2022-03-01 07:52:43.000000 abjad-ext-nauert-3.9/abjadext/nauert/jobhandlers.py
+-rw-r--r--   0 trevor     (501) staff       (20)     2969 2022-05-01 13:08:19.000000 abjad-ext-nauert-3.9/abjadext/nauert/qeventproxy.py
+-rw-r--r--   0 trevor     (501) staff       (20)     6878 2022-05-01 13:08:19.000000 abjad-ext-nauert-3.9/abjadext/nauert/qevents.py
+-rw-r--r--   0 trevor     (501) staff       (20)    19436 2022-05-01 13:08:19.000000 abjad-ext-nauert-3.9/abjadext/nauert/qeventsequence.py
+-rw-r--r--   0 trevor     (501) staff       (20)    17772 2022-05-01 13:08:19.000000 abjad-ext-nauert-3.9/abjadext/nauert/qgrid.py
+-rw-r--r--   0 trevor     (501) staff       (20)     5969 2022-05-01 13:08:19.000000 abjad-ext-nauert-3.9/abjadext/nauert/qschemaitems.py
+-rw-r--r--   0 trevor     (501) staff       (20)    21201 2022-05-01 13:08:19.000000 abjad-ext-nauert-3.9/abjadext/nauert/qschemas.py
+-rw-r--r--   0 trevor     (501) staff       (20)    18636 2022-05-01 13:08:19.000000 abjad-ext-nauert-3.9/abjadext/nauert/qtargetitems.py
+-rw-r--r--   0 trevor     (501) staff       (20)    16147 2022-05-01 13:08:19.000000 abjad-ext-nauert-3.9/abjadext/nauert/qtargets.py
+-rw-r--r--   0 trevor     (501) staff       (20)     7051 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.9/abjadext/nauert/quantizationjob.py
+-rw-r--r--   0 trevor     (501) staff       (20)    10099 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.9/abjadext/nauert/quantizer.py
+-rw-r--r--   0 trevor     (501) staff       (20)    13736 2022-03-20 14:52:57.000000 abjad-ext-nauert-3.9/abjadext/nauert/searchtrees.py
+-rw-r--r--   0 trevor     (501) staff       (20)        0 2022-04-08 14:46:43.000000 abjad-ext-nauert-3.9/abjadext/py.typed
+-rw-r--r--   0 trevor     (501) staff       (20)       38 2022-05-01 13:33:33.300125 abjad-ext-nauert-3.9/setup.cfg
+-rw-r--r--   0 trevor     (501) staff       (20)     1617 2022-05-01 13:31:50.000000 abjad-ext-nauert-3.9/setup.py
```

### Comparing `abjad-ext-nauert-3.8/LICENSE` & `abjad-ext-nauert-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `abjad-ext-nauert-3.8/PKG-INFO` & `abjad-ext-nauert-3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abjad-ext-nauert
-Version: 3.8
+Version: 3.9
 Summary: Nauert extends Abjad with tools for rhythmic quantization.
 Home-page: http://abjad.github.io
 Author: Josiah Wolf Oberholtzer, Tsz Kiu Pang
 Author-email: josiah.oberholtzer@gmail.com, osamupang@gmail.com
 License: MIT
 Keywords: music composition,music notation,lilypond
 Platform: Any
```

### Comparing `abjad-ext-nauert-3.8/abjad_ext_nauert.egg-info/PKG-INFO` & `abjad-ext-nauert-3.9/abjad_ext_nauert.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abjad-ext-nauert
-Version: 3.8
+Version: 3.9
 Summary: Nauert extends Abjad with tools for rhythmic quantization.
 Home-page: http://abjad.github.io
 Author: Josiah Wolf Oberholtzer, Tsz Kiu Pang
 Author-email: josiah.oberholtzer@gmail.com, osamupang@gmail.com
 License: MIT
 Keywords: music composition,music notation,lilypond
 Platform: Any
```

### Comparing `abjad-ext-nauert-3.8/abjad_ext_nauert.egg-info/SOURCES.txt` & `abjad-ext-nauert-3.9/abjad_ext_nauert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/__init__.py` & `abjad-ext-nauert-3.9/abjadext/nauert/__init__.py`

 * *Files identical despite different names*

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/attackpointoptimizers.py` & `abjad-ext-nauert-3.9/abjadext/nauert/attackpointoptimizers.py`

 * *Files identical despite different names*

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/gracehandlers.py` & `abjad-ext-nauert-3.9/abjadext/nauert/gracehandlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
     )
 
     ### INITIALIZER ###
 
     def __init__(
         self,
         discard_grace_rest: bool = True,
-        grace_duration: abjad.DurationTyping = None,
+        grace_duration: abjad.typings.Duration = None,
         replace_rest_with_final_grace_note: bool = True,
     ):
         self._discard_grace_rest = discard_grace_rest
         if grace_duration is None:
             grace_duration = (1, 16)
         grace_duration = abjad.Duration(grace_duration)
         assert grace_duration.is_dyadic_rational
```

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/heuristics.py` & `abjad-ext-nauert-3.9/abjadext/nauert/heuristics.py`

 * *Files identical despite different names*

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/jobhandlers.py` & `abjad-ext-nauert-3.9/abjadext/nauert/jobhandlers.py`

 * *Files identical despite different names*

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/qeventproxy.py` & `abjad-ext-nauert-3.9/abjadext/nauert/qeventproxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     ### CLASS VARIABLES ###
 
     __slots__ = ("_offset", "_q_event")
 
     ### INITIALIZER ###
 
-    def __init__(self, q_event: QEvent | None = None, *offsets: abjad.OffsetTyping):
+    def __init__(self, q_event: QEvent | None = None, *offsets: abjad.typings.Offset):
         if len(offsets) == 1:
             offset = abjad.Offset(offsets[0])
             assert isinstance(q_event, QEvent)
             assert 0 <= offset <= 1
         elif len(offsets) == 2:
             minimum, maximum = (
                 abjad.Offset(offsets[0]),
```

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/qevents.py` & `abjad-ext-nauert-3.9/abjadext/nauert/qevents.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     __slots__ = ("_attachments", "_index", "_offset")
 
     ### INITIALIZER ###
 
     @abc.abstractmethod
     def __init__(
         self,
-        offset: abjad.OffsetTyping = 0,
+        offset: abjad.typings.Offset = 0,
         index: int | None = None,
         attachments: typing.Iterable | None = None,
     ):
         offset = abjad.Offset(offset)
         self._offset = offset
         self._index = index
         self._attachments = tuple(attachments or ())
@@ -93,16 +93,16 @@
 
     __slots__ = ("_attachments", "_index", "_offset", "_pitches")
 
     ### INITIALIZER ###
 
     def __init__(
         self,
-        offset: abjad.OffsetTyping = 0,
-        pitches: typing.Iterable[abjad.Number] | None = None,
+        offset: abjad.typings.Offset = 0,
+        pitches: typing.Iterable[int | float] | None = None,
         attachments: typing.Iterable | None = None,
         index: int | None = None,
     ):
         QEvent.__init__(self, offset=offset, index=index)
         if attachments is None:
             attachments = ()
         else:
@@ -176,15 +176,15 @@
 
     __slots__ = ("_attachments",)
 
     ### INITIALIZER ###
 
     def __init__(
         self,
-        offset: abjad.OffsetTyping = 0,
+        offset: abjad.typings.Offset = 0,
         attachments: typing.Iterable | None = None,
         index: int | None = None,
     ):
         QEvent.__init__(self, offset=offset, index=index)
         if attachments is None:
             attachments = ()
         else:
@@ -238,15 +238,15 @@
 
     ### CLASS VARIABLES ###
 
     __slots__ = ("_offset",)
 
     ### INITIALIZER ###
 
-    def __init__(self, offset: abjad.OffsetTyping = 0):
+    def __init__(self, offset: abjad.typings.Offset = 0):
         QEvent.__init__(self, offset=offset)
 
     ### SPECIAL METHODS ###
 
     def __eq__(self, argument) -> bool:
         """
         Is true when `argument` is a terminal q-event with offset equal to that
```

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/qeventsequence.py` & `abjad-ext-nauert-3.9/abjadext/nauert/qeventsequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         return self._sequence
 
     ### PUBLIC METHODS ###
 
     @classmethod
     def from_millisecond_durations(
         class_,
-        milliseconds: typing.Sequence[abjad.Number],
+        milliseconds: typing.Sequence[int | float],
         fuse_silences: bool = False,
     ) -> "QEventSequence":
         r"""
         Changes sequence of millisecond durations ``durations`` to a ``QEventSequence``:
 
         >>> durations = [-250, 500, -1000, 1250, -1000]
         >>> sequence = nauert.QEventSequence.from_millisecond_durations(
@@ -182,15 +182,15 @@
         PitchedQEvent(offset=Offset((250, 1)), pitches=(NamedPitch("c'"),), index=None, attachments=())
         SilentQEvent(offset=Offset((750, 1)), index=None, attachments=())
         PitchedQEvent(offset=Offset((1750, 1)), pitches=(NamedPitch("c'"),), index=None, attachments=())
         SilentQEvent(offset=Offset((3000, 1)), index=None, attachments=())
         TerminalQEvent(offset=Offset((4000, 1)), index=None, attachments=())
 
         """
-        durations: typing.Sequence[abjad.Number]
+        durations: typing.Sequence[int | float]
         if fuse_silences:
             durations = [
                 _ for _ in abjad.sequence.sum_by_sign(milliseconds, sign=[-1]) if _
             ]
         else:
             durations = milliseconds
         offsets = abjad.math.cumulative_sums([abs(_) for _ in durations])
@@ -206,15 +206,15 @@
                 q_event = PitchedQEvent(offset, [0])
             q_events.append(q_event)
         q_events.append(TerminalQEvent(abjad.Offset(offsets[-1])))
         return class_(q_events)
 
     @classmethod
     def from_millisecond_offsets(
-        class_, offsets: abjad.OffsetSequenceTyping
+        class_, offsets: typing.Sequence[abjad.typings.Offset]
     ) -> "QEventSequence":
         r"""
         Changes millisecond offsets ``offsets`` to a ``QEventSequence``:
 
         >>> offsets = [0, 250, 750, 1750, 3000, 4000]
         >>> sequence = nauert.QEventSequence.from_millisecond_offsets(
         ...     offsets)
@@ -360,15 +360,15 @@
                 q_events.append(PitchedQEvent(offset, [pitches]))
         q_events.append(TerminalQEvent(abjad.Offset(offsets[-1])))
         return class_(q_events)
 
     @classmethod
     def from_tempo_scaled_durations(
         class_,
-        durations: abjad.DurationSequenceTyping,
+        durations: typing.Sequence[abjad.typings.Duration],
         tempo: abjad.MetronomeMark,
     ) -> "QEventSequence":
         r"""
         Changes ``durations``, scaled by ``tempo`` into a ``QEventSequence``:
 
         >>> tempo = abjad.MetronomeMark((1, 4), 174)
         >>> durations = [(1, 4), (-3, 16), (1, 16), (-1, 2)]
@@ -447,15 +447,15 @@
         for rvalue, rgroup in itertools.groupby(
             leaves, lambda x: isinstance(x, (abjad.Rest, abjad.Skip))
         ):
             if rvalue:
                 groups.append(list(rgroup))
             else:
                 for tvalue, tgroup in itertools.groupby(
-                    rgroup, lambda x: abjad._iterate._get_logical_tie_leaves(x)
+                    rgroup, lambda x: abjad._iterlib._get_logical_tie_leaves(x)
                 ):
                     groups.append(list(tgroup))
         # calculate lists of pitches and durations
         durations = []
         pitches = []
         for group in groups:
             # get millisecond cumulative duration
```

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/qgrid.py` & `abjad-ext-nauert-3.9/abjadext/nauert/qgrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Used internally by ``QGrid``.
     """
 
     ### INITIALIZER ###
 
     def __init__(
         self,
-        preprolated_duration: abjad.DurationTyping | int = 1,
+        preprolated_duration: abjad.typings.Duration | int = 1,
         q_event_proxies: typing.Sequence[QEventProxy] | None = None,
         is_divisible: bool = True,
     ):
         uqbar.containers.UniqueTreeNode.__init__(self)
         abjad.rhythmtrees.RhythmTreeMixin.__init__(self, preprolated_duration)
         if q_event_proxies is None:
             self._q_event_proxies = []
@@ -38,15 +38,15 @@
             assert all(isinstance(x, QEventProxy) for x in q_event_proxies)
             self._q_event_proxies = list(q_event_proxies)
         self._is_divisible = bool(is_divisible)
 
     ### SPECIAL METHODS ###
 
     def __call__(
-        self, pulse_duration: abjad.DurationTyping | int
+        self, pulse_duration: abjad.typings.Duration | int
     ) -> list[abjad.Note | abjad.Tuplet]:
         """
         Calls q-grid leaf.
         """
         pulse_duration = abjad.Duration(pulse_duration)
         total_duration = pulse_duration * self.preprolated_duration
         maker = abjad.NoteMaker()
@@ -220,15 +220,15 @@
         self._next_downbeat = next_downbeat
         self._next_downbeat._offset = abjad.Offset(1)
         self._next_downbeat._offsets_are_current = True
 
     ### SPECIAL METHODS ###
 
     def __call__(
-        self, beatspan: abjad.DurationTyping | int
+        self, beatspan: abjad.typings.Duration | int
     ) -> list[abjad.Note | abjad.Tuplet]:
         """
         Calls q-grid.
         """
         result = self.root_node(beatspan)
         result_logical_ties = [
             logical_tie for logical_tie in abjad.iterate.logical_ties(result)
@@ -464,15 +464,15 @@
         """
         for leaf in self.leaves:
             leaf.q_event_proxies.sort(key=lambda x: 0 if x.index is None else x.index)
 
     def subdivide_leaf(
         self,
         leaf: QGridLeaf,
-        subdivisions: typing.Sequence[abjad.DurationTyping | int],
+        subdivisions: typing.Sequence[abjad.typings.Duration | int],
     ) -> list[QEventProxy]:
         r"""Replace the ``QGridLeaf`` ``leaf`` contained in a ``QGrid``
         by a ``QGridContainer`` containing ``QGridLeaves`` with durations
         equal to the ratio described in ``subdivisions``
 
         Returns the ``QEventProxies`` attached to ``leaf``.
         """
@@ -488,15 +488,15 @@
             leaf.parent[index] = [container]
         # otherwise, our root node if just a QGridLeaf
         else:
             self._root_node = container
         return leaf.q_event_proxies
 
     def subdivide_leaves(
-        self, pairs: typing.Sequence[tuple[int, abjad.IntegerPair]]
+        self, pairs: typing.Sequence[tuple[int, tuple[int, int]]]
     ) -> list[QEventProxy]:
         r"""Given a sequence of leaf-index:subdivision-ratio pairs ``pairs``,
         subdivide the ``QGridLeaves`` described by the indices into
         ``QGridContainers`` containing ``QGridLeaves`` with durations
         equal to their respective subdivision-ratios.
 
         Returns the ``QEventProxies`` attached to thus subdivided
```

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/qschemaitems.py` & `abjad-ext-nauert-3.9/abjadext/nauert/qschemaitems.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     ### INITIALIZER ###
 
     @abc.abstractmethod
     def __init__(
         self,
         search_tree: SearchTree | None = None,
-        tempo: abjad.MetronomeMark | abjad.DurationTyping | None = None,
+        tempo: abjad.MetronomeMark | abjad.typings.Duration | None = None,
     ):
         if search_tree is not None:
             assert isinstance(search_tree, SearchTree)
         self._search_tree = search_tree
         if tempo is not None:
             if isinstance(tempo, tuple):
                 tempo = abjad.MetronomeMark(*tempo)
@@ -83,17 +83,17 @@
 
     __slots__ = ("_beatspan",)
 
     ### INITIALIZER ###
 
     def __init__(
         self,
-        beatspan: abjad.DurationTyping | int | None = None,
+        beatspan: abjad.typings.Duration | int | None = None,
         search_tree: SearchTree | None = None,
-        tempo: abjad.MetronomeMark | abjad.DurationTyping | None = None,
+        tempo: abjad.MetronomeMark | abjad.typings.Duration | None = None,
     ):
         QSchemaItem.__init__(self, search_tree=search_tree, tempo=tempo)
         if beatspan is not None:
             beatspan = abjad.Duration(beatspan)
             assert 0 < beatspan
         self._beatspan = beatspan
 
@@ -149,16 +149,16 @@
     __slots__ = ("_time_signature", "_use_full_measure")
 
     ### INITIALIZER ###
 
     def __init__(
         self,
         search_tree: SearchTree | None = None,
-        tempo: abjad.MetronomeMark | abjad.DurationTyping | None = None,
-        time_signature: abjad.IntegerPair | None = None,
+        tempo: abjad.MetronomeMark | abjad.typings.Duration | None = None,
+        time_signature: tuple[int, int] | None = None,
         use_full_measure: bool | None = None,
     ):
         QSchemaItem.__init__(self, search_tree=search_tree, tempo=tempo)
         self._time_signature: abjad.TimeSignature | None
         if time_signature is not None:
             self._time_signature = abjad.TimeSignature(time_signature)
         else:
```

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/qschemas.py` & `abjad-ext-nauert-3.9/abjadext/nauert/qschemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         if items:
             assert 0 <= min(items)
         self._items = dict(items)
         self._lookups = self._create_lookups()
 
     ### SPECIAL METHODS ###
 
-    def __call__(self, duration: abjad.DurationTyping) -> QTarget:
+    def __call__(self, duration: abjad.typings.Duration) -> QTarget:
         """
         Calls QSchema on ``duration``.
         """
         target_items = []
         idx, current_offset = 0, 0
         duration = abjad.Duration(duration)
         while current_offset < duration:
```

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/qtargetitems.py` & `abjad-ext-nauert-3.9/abjadext/nauert/qtargetitems.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,18 +65,18 @@
         "_tempo",
     )
 
     ### INITIALIZER ###
 
     def __init__(
         self,
-        beatspan: abjad.DurationTyping | None = None,
+        beatspan: abjad.typings.Duration | None = None,
         offset_in_ms: abjad.Duration | int | None = None,
         search_tree: SearchTree | None = None,
-        tempo: abjad.MetronomeMark | abjad.DurationTyping | None = None,
+        tempo: abjad.MetronomeMark | abjad.typings.Duration | None = None,
     ):
         beatspan = beatspan or abjad.Duration(0)
         beatspan = abjad.Duration(beatspan)
         offset_in_ms = offset_in_ms or abjad.Duration(0)
         offset_in_ms = abjad.Offset(offset_in_ms)
 
         if search_tree is None:
@@ -340,16 +340,16 @@
 
     ### INITIALIZER ###
 
     def __init__(
         self,
         offset_in_ms: abjad.Duration | int | None = None,
         search_tree: SearchTree | None = None,
-        time_signature: abjad.IntegerPair | None = None,
-        tempo: abjad.MetronomeMark | abjad.DurationTyping | None = None,
+        time_signature: tuple[int, int] | None = None,
+        tempo: abjad.MetronomeMark | abjad.typings.Duration | None = None,
         use_full_measure: bool = False,
     ):
         offset_in_ms = offset_in_ms or 0
         offset_in_ms = abjad.Offset(offset_in_ms)
 
         if search_tree is None:
             search_tree = UnweightedSearchTree()
```

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/qtargets.py` & `abjad-ext-nauert-3.9/abjadext/nauert/qtargets.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                     abjad.attach(grace_container, new_leaf)
                 abjad.mutate.replace(leaf, new_leaf)
                 if not isinstance(new_leaf, abjad.Rest):
                     abjad.annotate(new_leaf, "tie_to_next", True)
                 elif abjad.get.indicator(new_leaf, abjad.Tie):
                     abjad.detach(abjad.Tie, new_leaf)
             else:
-                previous_leaf = abjad._iterate._get_leaf(leaf, -1)
+                previous_leaf = abjad._iterlib._get_leaf(leaf, -1)
                 if isinstance(previous_leaf, abjad.Rest):
                     new_leaf = type(previous_leaf)(leaf.written_duration)
                 elif isinstance(previous_leaf, abjad.Note):
                     new_leaf = type(previous_leaf)(
                         previous_leaf.written_pitch, leaf.written_duration
                     )
                 else:
```

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/quantizationjob.py` & `abjad-ext-nauert-3.9/abjadext/nauert/quantizationjob.py`

 * *Files identical despite different names*

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/quantizer.py` & `abjad-ext-nauert-3.9/abjadext/nauert/quantizer.py`

 * *Files identical despite different names*

### Comparing `abjad-ext-nauert-3.8/abjadext/nauert/searchtrees.py` & `abjad-ext-nauert-3.9/abjadext/nauert/searchtrees.py`

 * *Files identical despite different names*

### Comparing `abjad-ext-nauert-3.8/setup.py` & `abjad-ext-nauert-3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: Implementation :: CPython",
             "Topic :: Artistic Software",
         ],
         description=description,
         include_package_data=True,
         install_requires=[
-            "abjad>=3.8",
+            "abjad>=3.9",
         ],
         license="MIT",
         long_description=pathlib.Path("README.md").read_text(),
         keywords=", ".join(
             [
                 "music composition",
                 "music notation",
```

