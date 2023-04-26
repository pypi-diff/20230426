# Comparing `tmp/abjad-ext-rmakers-3.8.tar.gz` & `tmp/abjad-ext-rmakers-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abjad-ext-rmakers-3.8.tar", last modified: Fri Apr  8 15:42:09 2022, max compression
+gzip compressed data, was "abjad-ext-rmakers-3.9.tar", last modified: Sun May  1 13:33:25 2022, max compression
```

## Comparing `abjad-ext-rmakers-3.8.tar` & `abjad-ext-rmakers-3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-04-08 15:42:09.780749 abjad-ext-rmakers-3.8/
--rw-r--r--   0 trevor     (501) staff       (20)     1067 2022-01-30 15:34:21.000000 abjad-ext-rmakers-3.8/LICENSE
--rw-r--r--   0 trevor     (501) staff       (20)      101 2022-01-30 15:34:21.000000 abjad-ext-rmakers-3.8/MANIFEST.in
--rw-r--r--   0 trevor     (501) staff       (20)      910 2022-04-08 15:42:09.780267 abjad-ext-rmakers-3.8/PKG-INFO
--rw-r--r--   0 trevor     (501) staff       (20)      304 2022-01-30 15:34:21.000000 abjad-ext-rmakers-3.8/README.md
-drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-04-08 15:42:09.775780 abjad-ext-rmakers-3.8/abjad_ext_rmakers.egg-info/
--rw-r--r--   0 trevor     (501) staff       (20)      910 2022-04-08 15:42:09.000000 abjad-ext-rmakers-3.8/abjad_ext_rmakers.egg-info/PKG-INFO
--rw-r--r--   0 trevor     (501) staff       (20)      393 2022-04-08 15:42:09.000000 abjad-ext-rmakers-3.8/abjad_ext_rmakers.egg-info/SOURCES.txt
--rw-r--r--   0 trevor     (501) staff       (20)        1 2022-04-08 15:42:09.000000 abjad-ext-rmakers-3.8/abjad_ext_rmakers.egg-info/dependency_links.txt
--rw-r--r--   0 trevor     (501) staff       (20)       11 2022-04-08 15:42:09.000000 abjad-ext-rmakers-3.8/abjad_ext_rmakers.egg-info/requires.txt
--rw-r--r--   0 trevor     (501) staff       (20)        9 2022-04-08 15:42:09.000000 abjad-ext-rmakers-3.8/abjad_ext_rmakers.egg-info/top_level.txt
-drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-04-08 15:42:09.776626 abjad-ext-rmakers-3.8/abjadext/
--rw-r--r--   0 trevor     (501) staff       (20)      119 2022-01-30 15:34:21.000000 abjad-ext-rmakers-3.8/abjadext/__init__.py
--rw-r--r--   0 trevor     (501) staff       (20)        0 2022-04-08 07:41:20.000000 abjad-ext-rmakers-3.8/abjadext/py.typed
-drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-04-08 15:42:09.778296 abjad-ext-rmakers-3.8/abjadext/rmakers/
--rw-r--r--   0 trevor     (501) staff       (20)     3237 2022-02-04 11:59:58.000000 abjad-ext-rmakers-3.8/abjadext/rmakers/__init__.py
--rw-r--r--   0 trevor     (501) staff       (20)    11799 2022-02-22 15:56:28.000000 abjad-ext-rmakers-3.8/abjadext/rmakers/_todo.py
--rw-r--r--   0 trevor     (501) staff       (20)      131 2022-04-08 15:30:19.000000 abjad-ext-rmakers-3.8/abjadext/rmakers/_version.py
--rw-r--r--   0 trevor     (501) staff       (20)   630464 2022-04-05 09:38:06.000000 abjad-ext-rmakers-3.8/abjadext/rmakers/rmakers.py
--rw-r--r--   0 trevor     (501) staff       (20)       38 2022-04-08 15:42:09.780913 abjad-ext-rmakers-3.8/setup.cfg
--rw-r--r--   0 trevor     (501) staff       (20)     1484 2022-04-08 15:30:26.000000 abjad-ext-rmakers-3.8/setup.py
+drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-05-01 13:33:25.680942 abjad-ext-rmakers-3.9/
+-rw-r--r--   0 trevor     (501) staff       (20)     1067 2022-01-30 15:34:21.000000 abjad-ext-rmakers-3.9/LICENSE
+-rw-r--r--   0 trevor     (501) staff       (20)      101 2022-01-30 15:34:21.000000 abjad-ext-rmakers-3.9/MANIFEST.in
+-rw-r--r--   0 trevor     (501) staff       (20)      910 2022-05-01 13:33:25.680533 abjad-ext-rmakers-3.9/PKG-INFO
+-rw-r--r--   0 trevor     (501) staff       (20)      304 2022-01-30 15:34:21.000000 abjad-ext-rmakers-3.9/README.md
+drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-05-01 13:33:25.663078 abjad-ext-rmakers-3.9/abjad_ext_rmakers.egg-info/
+-rw-r--r--   0 trevor     (501) staff       (20)      910 2022-05-01 13:33:25.000000 abjad-ext-rmakers-3.9/abjad_ext_rmakers.egg-info/PKG-INFO
+-rw-r--r--   0 trevor     (501) staff       (20)      393 2022-05-01 13:33:25.000000 abjad-ext-rmakers-3.9/abjad_ext_rmakers.egg-info/SOURCES.txt
+-rw-r--r--   0 trevor     (501) staff       (20)        1 2022-05-01 13:33:25.000000 abjad-ext-rmakers-3.9/abjad_ext_rmakers.egg-info/dependency_links.txt
+-rw-r--r--   0 trevor     (501) staff       (20)       11 2022-05-01 13:33:25.000000 abjad-ext-rmakers-3.9/abjad_ext_rmakers.egg-info/requires.txt
+-rw-r--r--   0 trevor     (501) staff       (20)        9 2022-05-01 13:33:25.000000 abjad-ext-rmakers-3.9/abjad_ext_rmakers.egg-info/top_level.txt
+drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-05-01 13:33:25.664131 abjad-ext-rmakers-3.9/abjadext/
+-rw-r--r--   0 trevor     (501) staff       (20)      119 2022-01-30 15:34:21.000000 abjad-ext-rmakers-3.9/abjadext/__init__.py
+-rw-r--r--   0 trevor     (501) staff       (20)        0 2022-04-08 07:41:20.000000 abjad-ext-rmakers-3.9/abjadext/py.typed
+drwxr-xr-x   0 trevor     (501) staff       (20)        0 2022-05-01 13:33:25.666705 abjad-ext-rmakers-3.9/abjadext/rmakers/
+-rw-r--r--   0 trevor     (501) staff       (20)     3237 2022-02-04 11:59:58.000000 abjad-ext-rmakers-3.9/abjadext/rmakers/__init__.py
+-rw-r--r--   0 trevor     (501) staff       (20)    11799 2022-02-22 15:56:28.000000 abjad-ext-rmakers-3.9/abjadext/rmakers/_todo.py
+-rw-r--r--   0 trevor     (501) staff       (20)      131 2022-05-01 13:29:42.000000 abjad-ext-rmakers-3.9/abjadext/rmakers/_version.py
+-rw-r--r--   0 trevor     (501) staff       (20)   630495 2022-04-22 08:32:11.000000 abjad-ext-rmakers-3.9/abjadext/rmakers/rmakers.py
+-rw-r--r--   0 trevor     (501) staff       (20)       38 2022-05-01 13:33:25.681088 abjad-ext-rmakers-3.9/setup.cfg
+-rw-r--r--   0 trevor     (501) staff       (20)     1484 2022-05-01 13:29:52.000000 abjad-ext-rmakers-3.9/setup.py
```

### Comparing `abjad-ext-rmakers-3.8/LICENSE` & `abjad-ext-rmakers-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `abjad-ext-rmakers-3.8/PKG-INFO` & `abjad-ext-rmakers-3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abjad-ext-rmakers
-Version: 3.8
+Version: 3.9
 Summary: Rhythm-makers extend Abjad with tools for rhythmic construction.
 Home-page: http://abjad.github.io
 Author: Trevor Bača
 Author-email: trevor.baca@gmail.com
 License: MIT
 Keywords: music composition,music notation,lilypond
 Platform: Any
```

### Comparing `abjad-ext-rmakers-3.8/abjad_ext_rmakers.egg-info/PKG-INFO` & `abjad-ext-rmakers-3.9/abjad_ext_rmakers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abjad-ext-rmakers
-Version: 3.8
+Version: 3.9
 Summary: Rhythm-makers extend Abjad with tools for rhythmic construction.
 Home-page: http://abjad.github.io
 Author: Trevor Bača
 Author-email: trevor.baca@gmail.com
 License: MIT
 Keywords: music composition,music notation,lilypond
 Platform: Any
```

### Comparing `abjad-ext-rmakers-3.8/abjadext/rmakers/__init__.py` & `abjad-ext-rmakers-3.9/abjadext/rmakers/__init__.py`

 * *Files identical despite different names*

### Comparing `abjad-ext-rmakers-3.8/abjadext/rmakers/_todo.py` & `abjad-ext-rmakers-3.9/abjadext/rmakers/_todo.py`

 * *Files identical despite different names*

### Comparing `abjad-ext-rmakers-3.8/abjadext/rmakers/rmakers.py` & `abjad-ext-rmakers-3.9/abjadext/rmakers/rmakers.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,21 +110,21 @@
                     ]
                     r16
                 }
             >>
 
     """
 
-    body_ratio: abjad.RatioTyping = (1,)
+    body_ratio: abjad.typings.Ratio = (1,)
     fill_with_rests: bool = False
     outer_divisions_only: bool = False
-    prefix_counts: abjad.IntegerSequence = ()
-    prefix_talea: abjad.IntegerSequence = ()
-    suffix_counts: abjad.IntegerSequence = ()
-    suffix_talea: abjad.IntegerSequence = ()
+    prefix_counts: typing.Sequence[int] = ()
+    prefix_talea: typing.Sequence[int] = ()
+    suffix_counts: typing.Sequence[int] = ()
+    suffix_talea: typing.Sequence[int] = ()
     talea_denominator: int | None = None
 
     __documentation_section__ = "Specifiers"
 
     def __post_init__(self):
         self.prefix_talea = tuple(self.prefix_talea or ())
         assert self._is_integer_tuple(self.prefix_talea)
@@ -183,17 +183,17 @@
         ...     stop_duration=(1, 16),
         ...     written_duration=(1, 16),
         ... )
         Interpolation(start_duration=Duration(1, 4), stop_duration=Duration(1, 16), written_duration=Duration(1, 16))
 
     """
 
-    start_duration: abjad.DurationTyping = (1, 8)
-    stop_duration: abjad.DurationTyping = (1, 16)
-    written_duration: abjad.DurationTyping = (1, 16)
+    start_duration: abjad.typings.Duration = (1, 8)
+    stop_duration: abjad.typings.Duration = (1, 16)
+    written_duration: abjad.typings.Duration = (1, 16)
 
     __documentation_section__ = "Specifiers"
 
     def __post_init__(self) -> None:
         self.start_duration = abjad.Duration(self.start_duration)
         self.stop_duration = abjad.Duration(self.stop_duration)
         self.written_duration = abjad.Duration(self.written_duration)
@@ -453,16 +453,16 @@
                     r8
                     r8
                 }
             >>
 
     """
 
-    forbidden_note_duration: abjad.DurationTyping | None = None
-    forbidden_rest_duration: abjad.DurationTyping | None = None
+    forbidden_note_duration: abjad.typings.Duration | None = None
+    forbidden_rest_duration: abjad.typings.Duration | None = None
     increase_monotonic: bool = False
 
     __documentation_section__ = "Specifiers"
 
     def __post_init__(self):
         if self.forbidden_note_duration is not None:
             self.forbidden_note_duration = abjad.Duration(self.forbidden_note_duration)
@@ -539,16 +539,16 @@
         Duration(-1, 4)
         Duration(1, 1)
 
     """
 
     counts: typing.Sequence[int | str]
     denominator: int
-    end_counts: abjad.IntegerSequence = ()
-    preamble: abjad.IntegerSequence = ()
+    end_counts: typing.Sequence[int] = ()
+    preamble: typing.Sequence[int] = ()
 
     __documentation_section__ = "Specifiers"
 
     def __post_init__(self):
         self.counts = tuple(self.counts)
         for count in self.counts:
             assert isinstance(count, int) or count in "+-", repr(count)
@@ -853,17 +853,17 @@
             counts=counts,
             denominator=self.denominator,
             preamble=preamble_,
         )
 
 
 def interpolate(
-    start_duration: abjad.DurationTyping,
-    stop_duration: abjad.DurationTyping,
-    written_duration: abjad.DurationTyping,
+    start_duration: abjad.typings.Duration,
+    stop_duration: abjad.typings.Duration,
+    written_duration: abjad.typings.Duration,
 ) -> Interpolation:
     """
     Makes interpolation.
     """
     return Interpolation(start_duration, stop_duration, written_duration)
 
 
@@ -890,15 +890,15 @@
         assert isinstance(self.previous_state, dict), repr(self.previous_state)
         assert isinstance(self.spelling, Spelling), repr(self.spelling)
         assert isinstance(self.state, dict), repr(self.state)
         assert isinstance(self.tag, abjad.Tag), repr(self.tag)
 
     def __call__(
         self,
-        divisions: typing.Sequence[abjad.IntegerPair],
+        divisions: typing.Sequence[tuple[int, int]],
         previous_state: dict = None,
     ) -> list[abjad.Component]:
         self.previous_state = dict(previous_state or [])
         time_signatures = [abjad.TimeSignature(_) for _ in divisions]
         divisions = [abjad.NonreducedFraction(_) for _ in divisions]
         staff = self._make_staff(time_signatures)
         music = self._make_music(divisions)
@@ -2547,16 +2547,16 @@
                                 indent = 0
                                 ragged-right = ##t
                             }
                         }
                     \times 1/1
                     {
                         \once \override Beam.grow-direction = #right
-                        \time 4/8
                         \override Staff.Stem.stemlet-length = 0.75
+                        \time 4/8
                         r16 * 63/32
                         [
                         c'16 * 115/64
                         c'16 * 91/64
                         c'16 * 35/32
                         c'16 * 29/32
                         \revert Staff.Stem.stemlet-length
@@ -2599,16 +2599,16 @@
                                 indent = 0
                                 ragged-right = ##t
                             }
                         }
                     \times 1/1
                     {
                         \once \override Beam.grow-direction = #left
-                        \time 3/8
                         \override Staff.Stem.stemlet-length = 0.75
+                        \time 3/8
                         c'16 * 5/8
                         [
                         c'16 * 43/64
                         c'16 * 51/64
                         c'16 * 65/64
                         c'16 * 85/64
                         \revert Staff.Stem.stemlet-length
@@ -2651,16 +2651,16 @@
                                 indent = 0
                                 ragged-right = ##t
                             }
                         }
                     \times 1/1
                     {
                         \once \override Beam.grow-direction = #right
-                        \time 4/8
                         \override Staff.Stem.stemlet-length = 0.75
+                        \time 4/8
                         c'16 * 63/32
                         [
                         c'16 * 115/64
                         c'16 * 91/64
                         c'16 * 35/32
                         c'16 * 29/32
                         \revert Staff.Stem.stemlet-length
@@ -2703,16 +2703,16 @@
                                 indent = 0
                                 ragged-right = ##t
                             }
                         }
                     \times 1/1
                     {
                         \once \override Beam.grow-direction = #left
-                        \time 3/8
                         \override Staff.Stem.stemlet-length = 0.75
+                        \time 3/8
                         c'16 * 5/8
                         [
                         c'16 * 43/64
                         c'16 * 51/64
                         c'16 * 65/64
                         c'16 * 85/64
                         \revert Staff.Stem.stemlet-length
@@ -6211,16 +6211,16 @@
         >>> state = stack.maker.state
         >>> state
         {'divisions_consumed': 10, 'logical_ties_produced': 29}
 
     """
 
     denominator: str | int = "from_counts"
-    denominators: abjad.IntegerSequence = (8,)
-    extra_counts: abjad.IntegerSequence = (0,)
+    denominators: typing.Sequence[int] = (8,)
+    extra_counts: typing.Sequence[int] = (0,)
 
     def __post_init__(self):
         RhythmMaker.__post_init__(self)
         assert abjad.math.all_are_nonnegative_integer_powers_of_two(self.denominators)
         self.denominators = tuple(self.denominators or ())
         self.extra_counts = tuple(self.extra_counts or ())
         assert all(isinstance(_, int) for _ in self.extra_counts)
@@ -6901,15 +6901,15 @@
                     %! INCISED_RHYTHM_MAKER
                     }
                 }
             >>
 
     """
 
-    extra_counts: abjad.IntegerSequence = ()
+    extra_counts: typing.Sequence[int] = ()
     incise: Incise = Incise()
 
     def __post_init__(self):
         RhythmMaker.__post_init__(self)
         self.extra_counts = tuple(self.extra_counts or ())
         assert abjad.math.all_are_nonnegative_integer_equivalent_numbers(
             self.extra_counts
@@ -7433,15 +7433,15 @@
                     s1 * 1/3
                 }
             >>
 
     """
 
     prototype: type = abjad.Note
-    duration: abjad.DurationTyping = (1, 1)
+    duration: abjad.typings.Duration = (1, 1)
 
     _prototypes = (abjad.MultimeasureRest, abjad.Note, abjad.Rest, abjad.Skip)
 
     def __post_init__(self):
         RhythmMaker.__post_init__(self)
         if self.prototype not in self._prototypes:
             message = "must be note, (multimeasure) rest, skip:\n"
@@ -9011,51 +9011,51 @@
             <<
                 \context RhythmicStaff = "Staff"
                 \with
                 {
                     \override Clef.stencil = ##f
                 }
                 {
-                    \time 3/8
                     \override Staff.Stem.stemlet-length = 0.75
+                    \time 3/8
                     c'16
                     [
                     c'16
                     c'16
                     r16
                     c'16
                     \revert Staff.Stem.stemlet-length
                     c'16
                     ]
-                    \time 4/8
                     \override Staff.Stem.stemlet-length = 0.75
+                    \time 4/8
                     c'16
                     [
                     r16
                     c'16
                     c'16
                     c'16
                     r16
                     c'16
                     \revert Staff.Stem.stemlet-length
                     c'16
                     ]
-                    \time 3/8
                     \override Staff.Stem.stemlet-length = 0.75
+                    \time 3/8
                     c'16
                     [
                     r16
                     c'16
                     c'16
                     c'16
                     \revert Staff.Stem.stemlet-length
                     r16
                     ]
-                    \time 4/8
                     \override Staff.Stem.stemlet-length = 0.75
+                    \time 4/8
                     c'16
                     [
                     c'16
                     c'16
                     r16
                     c'16
                     c'16
@@ -11562,15 +11562,15 @@
                     c'16
                     ]
                 }
             >>
 
     """
 
-    extra_counts: abjad.IntegerSequence = ()
+    extra_counts: typing.Sequence[int] = ()
     read_talea_once_only: bool = False
     spelling: Spelling = Spelling()
     talea: Talea = Talea(counts=[1], denominator=16)
 
     def __post_init__(self):
         RhythmMaker.__post_init__(self)
         self.extra_counts = tuple(self.extra_counts or ())
@@ -13978,16 +13978,16 @@
                         c'2..
                     }
                 }
             >>
 
     """
 
-    denominator: int | abjad.DurationTyping | None = None
-    tuplet_ratios: abjad.RatioSequenceTyping = ()
+    denominator: int | abjad.typings.Duration | None = None
+    tuplet_ratios: typing.Sequence[abjad.typings.Ratio] = ()
 
     def __post_init__(self):
         RhythmMaker.__post_init__(self)
         if self.denominator is not None:
             if isinstance(self.denominator, tuple):
                 self.denominator = abjad.Duration(self.denominator)
             prototype = (abjad.Duration, int)
@@ -14006,15 +14006,15 @@
                 division, ratio, tag=self.tag
             )
             tuplets.append(tuplet)
         return tuplets
 
 
 def accelerando(
-    *interpolations: typing.Sequence[abjad.DurationTyping],
+    *interpolations: typing.Sequence[abjad.typings.Duration],
     spelling: Spelling = Spelling(),
     tag: abjad.Tag = abjad.Tag(),
 ) -> AccelerandoRhythmMaker:
     """
     Makes accelerando rhythm-maker.
     """
     interpolations_ = []
@@ -14023,18 +14023,18 @@
         interpolations_.append(interpolation_)
     return AccelerandoRhythmMaker(
         interpolations=interpolations_, spelling=spelling, tag=tag
     )
 
 
 def even_division(
-    denominators: abjad.IntegerSequence,
+    denominators: typing.Sequence[int],
     *,
     denominator: str | int = "from_counts",
-    extra_counts: abjad.IntegerSequence = (0,),
+    extra_counts: typing.Sequence[int] = (0,),
     spelling: Spelling = Spelling(),
     tag: abjad.Tag = abjad.Tag(),
 ) -> EvenDivisionRhythmMaker:
     """
     Makes even-division rhythm-maker.
     """
     return EvenDivisionRhythmMaker(
@@ -14043,22 +14043,22 @@
         extra_counts=extra_counts,
         spelling=spelling,
         tag=tag,
     )
 
 
 def incised(
-    extra_counts: abjad.IntegerSequence = (),
-    body_ratio: abjad.RatioTyping = abjad.Ratio((1,)),
+    extra_counts: typing.Sequence[int] = (),
+    body_ratio: abjad.typings.Ratio = abjad.Ratio((1,)),
     fill_with_rests: bool = False,
     outer_divisions_only: bool = False,
-    prefix_talea: abjad.IntegerSequence = (),
-    prefix_counts: abjad.IntegerSequence = (),
-    suffix_talea: abjad.IntegerSequence = (),
-    suffix_counts: abjad.IntegerSequence = (),
+    prefix_talea: typing.Sequence[int] = (),
+    prefix_counts: typing.Sequence[int] = (),
+    suffix_talea: typing.Sequence[int] = (),
+    suffix_counts: typing.Sequence[int] = (),
     talea_denominator: int = None,
     spelling: Spelling = Spelling(),
     tag: abjad.Tag = abjad.Tag(),
 ) -> IncisedRhythmMaker:
     """
     Makes incised rhythm-maker
     """
@@ -14078,15 +14078,15 @@
         tag=tag,
     )
 
 
 def multiplied_duration(
     prototype: type = abjad.Note,
     *,
-    duration: abjad.DurationTyping = (1, 1),
+    duration: abjad.typings.Duration = (1, 1),
     tag: abjad.Tag = abjad.Tag(),
 ) -> MultipliedDurationRhythmMaker:
     """
     Makes multiplied-duration rhythm-maker.
     """
     return MultipliedDurationRhythmMaker(
         prototype=prototype, duration=duration, tag=tag
@@ -14099,20 +14099,20 @@
     """
     Makes note rhythm-maker.
     """
     return NoteRhythmMaker(spelling=spelling, tag=tag)
 
 
 def talea(
-    counts: abjad.IntegerSequence,
+    counts: typing.Sequence[int],
     denominator: int,
     advance: int = 0,
-    end_counts: abjad.IntegerSequence = (),
-    extra_counts: abjad.IntegerSequence = (),
-    preamble: abjad.IntegerSequence = (),
+    end_counts: typing.Sequence[int] = (),
+    extra_counts: typing.Sequence[int] = (),
+    preamble: typing.Sequence[int] = (),
     read_talea_once_only: bool = False,
     spelling: Spelling = Spelling(),
     tag: abjad.Tag = abjad.Tag(),
 ) -> TaleaRhythmMaker:
     """
     Makes talea rhythm-maker.
     """
@@ -14129,17 +14129,17 @@
         spelling=spelling,
         tag=tag,
         talea=talea,
     )
 
 
 def tuplet(
-    tuplet_ratios: abjad.RatioSequenceTyping,
+    tuplet_ratios: typing.Sequence[abjad.typings.Ratio],
     # TODO: remove in favor of dedicated denominator control commands:
-    denominator: int | abjad.DurationTyping | None = None,
+    denominator: int | abjad.typings.Duration | None = None,
     spelling: Spelling = Spelling(),
     tag: abjad.Tag = abjad.Tag(),
 ) -> TupletRhythmMaker:
     """
     Makes tuplet rhythm-maker.
     """
     return TupletRhythmMaker(
@@ -14271,15 +14271,15 @@
 
 @dataclasses.dataclass(slots=True)
 class DenominatorCommand(Command):
     """
     Denominator command.
     """
 
-    denominator: int | abjad.DurationTyping | None = None
+    denominator: int | abjad.typings.Duration | None = None
 
     def __post_init__(self):
         Command.__post_init__(self)
         if isinstance(self.denominator, tuple):
             self.denominator = abjad.Duration(self.denominator)
         if self.denominator is not None:
             prototype = (int, abjad.Duration)
@@ -14327,15 +14327,15 @@
 @dataclasses.dataclass(slots=True)
 class WrittenDurationCommand(Command):
     """
     Written duration command.
     """
 
     selector: typing.Callable | None = lambda _: abjad.select.leaf(_, 0)
-    duration: abjad.DurationTyping | None = None
+    duration: abjad.typings.Duration | None = None
 
     def __post_init__(self):
         Command.__post_init__(self)
         self.duration = abjad.Duration(self.duration)
 
     def __call__(self, voice, *, tag: abjad.Tag = abjad.Tag()) -> None:
         selection = voice
@@ -14376,15 +14376,15 @@
 @dataclasses.dataclass(slots=True)
 class FeatherBeamCommand(Command):
     """
     Feather beam command.
     """
 
     beam_rests: bool = False
-    stemlet_length: abjad.Number | None = None
+    stemlet_length: int | float | None = None
 
     def __post_init__(self):
         Command.__post_init__(self)
         if self.beam_rests is not None:
             self.beam_rests = bool(self.beam_rests)
         if self.stemlet_length is not None:
             assert isinstance(self.stemlet_length, int | float)
@@ -14590,15 +14590,15 @@
 
 @dataclasses.dataclass(slots=True)
 class ForceRepeatTieCommand(Command):
     """
     Force repeat-tie command.
     """
 
-    threshold: bool | abjad.IntegerPair | typing.Callable = False
+    threshold: bool | tuple[int, int] | typing.Callable = False
     inequality: typing.Callable = dataclasses.field(init=False, repr=False)
 
     def __post_init__(self):
         Command.__post_init__(self)
         if callable(self.threshold):
             inequality = self.threshold
         elif self.threshold in (None, False):
@@ -14845,15 +14845,15 @@
 
 @dataclasses.dataclass(slots=True)
 class GraceContainerCommand(Command):
     """
     Grace container command.
     """
 
-    counts: abjad.IntegerSequence | None = None
+    counts: typing.Sequence[int] | None = None
     class_: type = abjad.BeforeGraceContainer
     beam_and_slash: bool = False
     talea: Talea = Talea([1], 8)
 
     _classes = (abjad.BeforeGraceContainer, abjad.AfterGraceContainer)
 
     def __post_init__(self):
@@ -14910,16 +14910,16 @@
 
 @dataclasses.dataclass(slots=True)
 class OnBeatGraceContainerCommand(Command):
     """
     On-beat grace container command.
     """
 
-    counts: abjad.IntegerSequence | None = None
-    leaf_duration: abjad.DurationTyping | None = None
+    counts: typing.Sequence[int] | None = None
+    leaf_duration: abjad.typings.Duration | None = None
     talea: Talea = Talea([1], 8)
 
     def __post_init__(self):
         Command.__post_init__(self)
         assert all(isinstance(_, int) for _ in self.counts), repr(self.counts)
         if self.leaf_duration is not None:
             self.leaf_duration = abjad.Duration(self.leaf_duration)
@@ -15177,15 +15177,15 @@
     Split measures command.
     """
 
     def __call__(
         self,
         voice,
         *,
-        durations: typing.Sequence[abjad.DurationTyping] = (),
+        durations: typing.Sequence[abjad.typings.Duration] = (),
         tag: abjad.Tag = abjad.Tag(),
     ) -> None:
         if not durations:
             # TODO: implement abjad.get() method for measure durations
             staff = abjad.get.parentage(voice).parent
             assert isinstance(staff, abjad.Staff)
             voice_ = staff["TimeSignatureVoice"]
@@ -15303,15 +15303,15 @@
         result = abjad.select.tuplets(argument, level=level)
         return [abjad.select.leaves(_, grace=False) for _ in result]
 
     return selector
 
 
 def after_grace_container(
-    counts: abjad.IntegerSequence,
+    counts: typing.Sequence[int],
     selector: typing.Callable | None = None,
     *,
     beam_and_slash: bool = False,
     talea: Talea = Talea([1], 8),
 ) -> GraceContainerCommand:
     r"""
     Makes after-grace container command.
@@ -15522,15 +15522,15 @@
         beam_rests=beam_rests,
         stemlet_length=stemlet_length,
         tag=tag,
     )
 
 
 def before_grace_container(
-    counts: abjad.IntegerSequence,
+    counts: typing.Sequence[int],
     selector: typing.Callable | None = None,
     *,
     talea: Talea = Talea([1], 8),
 ) -> GraceContainerCommand:
     r"""
     Makes grace container command.
 
@@ -15673,15 +15673,15 @@
     """
     Makes cache state command.
     """
     return CacheStateCommand()
 
 
 def denominator(
-    denominator: int | abjad.DurationTyping,
+    denominator: int | abjad.typings.Duration,
     selector: typing.Callable | None = lambda _: abjad.select.tuplets(_),
 ) -> DenominatorCommand:
     r"""
     Makes tuplet denominator command.
 
     ..  container:: example
 
@@ -16397,15 +16397,15 @@
     """
     Makes force note command.
     """
     return ForceNoteCommand(selector=selector)
 
 
 def force_repeat_tie(
-    threshold: bool | abjad.IntegerPair | typing.Callable = True,
+    threshold: bool | tuple[int, int] | typing.Callable = True,
     selector: typing.Callable | None = None,
 ) -> ForceRepeatTieCommand:
     """
     Makes force repeat-ties command.
     """
     return ForceRepeatTieCommand(selector=selector, threshold=threshold)
 
@@ -16421,18 +16421,18 @@
     """
     Makes invisible music command.
     """
     return InvisibleMusicCommand(selector=selector)
 
 
 def on_beat_grace_container(
-    counts: abjad.IntegerSequence,
+    counts: typing.Sequence[int],
     selector: typing.Callable | None = None,
     *,
-    leaf_duration: abjad.DurationTyping = None,
+    leaf_duration: abjad.typings.Duration = None,
     talea: Talea = Talea([1], 8),
 ) -> OnBeatGraceContainerCommand:
     r"""
     Makes on-beat grace container command.
 
     ..  container:: example
 
@@ -18456,15 +18456,15 @@
             >>
 
     """
     return UntieCommand(selector=selector)
 
 
 def written_duration(
-    duration: abjad.DurationTyping,
+    duration: abjad.typings.Duration,
     selector: typing.Callable | None = lambda _: abjad.select.leaves(_),
 ) -> WrittenDurationCommand:
     """
     Makes written duration command.
     """
     return WrittenDurationCommand(selector=selector, duration=duration)
 
@@ -18613,15 +18613,15 @@
         assert isinstance(self.tag, abjad.Tag), repr(self.tag)
         if self.tag.string:
             self.maker = dataclasses.replace(self.maker, tag=self.tag)
         self.commands = tuple(self.commands or ())
 
     def __call__(
         self,
-        time_signatures: typing.Sequence[abjad.IntegerPair],
+        time_signatures: typing.Sequence[tuple[int, int]],
         previous_state: dict = None,
     ) -> list[abjad.Component]:
         time_signatures_ = [abjad.TimeSignature(_) for _ in time_signatures]
         divisions_ = [abjad.NonreducedFraction(_) for _ in time_signatures]
         staff = RhythmMaker._make_staff(time_signatures_)
         music_voice = staff["Rhythm_Maker_Music_Voice"]
         divisions = self._apply_division_expression(divisions_)
```

### Comparing `abjad-ext-rmakers-3.8/setup.py` & `abjad-ext-rmakers-3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
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

