# Comparing `tmp/analyzethis-0.2.5-py3-none-any.whl.zip` & `tmp/analyzethis-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 40309 bytes, number of entries: 18
+Zip file size: 40478 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      247 b- defN 23-Jan-05 17:22 analyzethis/__init__.py
 -rw-r--r--  2.0 unx     3567 b- defN 23-Jan-02 19:49 analyzethis/ami_sections.py
 -rw-r--r--  2.0 unx     3631 b- defN 23-Jan-11 14:21 analyzethis/analyzetables.py
 -rw-r--r--  2.0 unx     6973 b- defN 23-Jan-08 22:39 analyzethis/analyzethis.py
 -rw-r--r--  2.0 unx      653 b- defN 22-Dec-21 11:09 analyzethis/convert_file.py
 -rw-r--r--  2.0 unx    45325 b- defN 23-Apr-26 18:41 analyzethis/entity_extraction.py
 -rw-r--r--  2.0 unx    12079 b- defN 22-Dec-21 11:09 analyzethis/file_lib.py
 -rw-r--r--  2.0 unx     3626 b- defN 22-Dec-21 11:09 analyzethis/get_html.py
 -rw-r--r--  2.0 unx     1133 b- defN 22-Dec-21 11:09 analyzethis/glob_trail.py
 -rw-r--r--  2.0 unx      329 b- defN 22-Dec-21 12:36 analyzethis/gui.py
 -rw-r--r--  2.0 unx     9771 b- defN 23-Feb-20 23:59 analyzethis/table_analysis.py
 -rw-r--r--  2.0 unx    17681 b- defN 23-Jan-02 19:48 analyzethis/xml_lib.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-26 19:30 analyzethis-0.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    20060 b- defN 23-Apr-26 19:30 analyzethis-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 19:30 analyzethis-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx      108 b- defN 23-Apr-26 19:30 analyzethis-0.2.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-26 19:30 analyzethis-0.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1495 b- defN 23-Apr-26 19:30 analyzethis-0.2.5.dist-info/RECORD
-18 files, 138139 bytes uncompressed, 37867 bytes compressed:  72.6%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-26 19:35 analyzethis-0.2.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    20567 b- defN 23-Apr-26 19:35 analyzethis-0.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 19:35 analyzethis-0.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-26 19:35 analyzethis-0.2.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-26 19:35 analyzethis-0.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1495 b- defN 23-Apr-26 19:35 analyzethis-0.2.6.dist-info/RECORD
+18 files, 138646 bytes uncompressed, 38036 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: analyzethis/table_analysis.py
 Comment: 
 
 Filename: analyzethis/xml_lib.py
 Comment: 
 
-Filename: analyzethis-0.2.5.dist-info/LICENSE
+Filename: analyzethis-0.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: analyzethis-0.2.5.dist-info/METADATA
+Filename: analyzethis-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: analyzethis-0.2.5.dist-info/WHEEL
+Filename: analyzethis-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: analyzethis-0.2.5.dist-info/entry_points.txt
+Filename: analyzethis-0.2.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: analyzethis-0.2.5.dist-info/top_level.txt
+Filename: analyzethis-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: analyzethis-0.2.5.dist-info/RECORD
+Filename: analyzethis-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `analyzethis-0.2.5.dist-info/LICENSE` & `analyzethis-0.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `analyzethis-0.2.5.dist-info/METADATA` & `analyzethis-0.2.6.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analyzethis
-Version: 0.2.5
+Version: 0.2.6
 Summary: extract structured information from ethics paragraphs
 Author: Ayush Garg
 License: Apache License
 Keywords: research automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,17 +13,31 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: abbreviations (==0.2.5)
+Requires-Dist: beautifulsoup4 (==4.12.2)
+Requires-Dist: braceexpand (==0.1.5)
+Requires-Dist: brotlipy (==0.7.0)
+Requires-Dist: colorama (==0.4.6)
+Requires-Dist: dataclasses (==0.8)
 Requires-Dist: spacy
-Requires-Dist: beautifulsoup4
-Requires-Dist: pygetpapers
+Requires-Dist: future (==0.18.3)
+Requires-Dist: nltk (==3.8.1)
+Requires-Dist: pygetpapers (==1.2.5)
+Requires-Dist: pyopenssl (==23.1.1)
+Requires-Dist: pysocks (==1.7.1)
+Requires-Dist: pytest (==7.3.1)
+Requires-Dist: rich (==12.6.0)
+Requires-Dist: scikit-learn (==1.2.2)
+Requires-Dist: shellingham (==1.5.1)
+Requires-Dist: tkinterweb (==3.18.7)
 
 ## docanalysis 
 `docanalysis` is a Command Line Tool that ingests corpora [(CProjects)](https://github.com/petermr/tigr2ess/blob/master/getpapers/TUTORIAL.md#cproject-and-ctrees) and carries out text-analysis of documents, including
 - sectioning
 - NLP/text-mining
 - dictionary generation
```

## Comparing `analyzethis-0.2.5.dist-info/RECORD` & `analyzethis-0.2.6.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 analyzethis/entity_extraction.py,sha256=wpzhlduImoSTbWqwWaU_zlY5EJ6cIbfT_uRAn8xvIHA,45325
 analyzethis/file_lib.py,sha256=emuUnguYqwvgvCyV13tUstG5uM6XqDlyOyNNaAY-Gqg,12079
 analyzethis/get_html.py,sha256=pPlX-NkTTb3hs9fCFAV-z2PRHHM00XuFMrwnILzI3zo,3626
 analyzethis/glob_trail.py,sha256=1TFs0HL1MfWHzKjwetG2XzT-avHPBUQJ-g2rjfZtPtc,1133
 analyzethis/gui.py,sha256=XqHbogj_AAXbuVfwck69qEdHEnvat-tLBd0vh1uiDbA,329
 analyzethis/table_analysis.py,sha256=q0cLS2_L1DZ-VhDN0wq1-QWCTByD1DW2k3ixuRQ0JDo,9771
 analyzethis/xml_lib.py,sha256=ggOLtpsdJhI86ok4VwgO_zUyTpavNkuu3ZfyB7s7MtM,17681
-analyzethis-0.2.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-analyzethis-0.2.5.dist-info/METADATA,sha256=u2ck9ercNibbXbwpPVC9dWg8Y9W6iS5YBq49B-csQhw,20060
-analyzethis-0.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-analyzethis-0.2.5.dist-info/entry_points.txt,sha256=k6daVQpvStC6FhogcXKHbJuBrkknIeeAvcjc_soQOec,108
-analyzethis-0.2.5.dist-info/top_level.txt,sha256=d-h8ihJ2V9R03TKharOSWFGydKoF6wl_xIkI8hjYPnQ,12
-analyzethis-0.2.5.dist-info/RECORD,,
+analyzethis-0.2.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+analyzethis-0.2.6.dist-info/METADATA,sha256=Edh5kX8jZ3KEWJAjOCebHzV3wthoKV21Dn-n3maV0GQ,20567
+analyzethis-0.2.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+analyzethis-0.2.6.dist-info/entry_points.txt,sha256=k6daVQpvStC6FhogcXKHbJuBrkknIeeAvcjc_soQOec,108
+analyzethis-0.2.6.dist-info/top_level.txt,sha256=d-h8ihJ2V9R03TKharOSWFGydKoF6wl_xIkI8hjYPnQ,12
+analyzethis-0.2.6.dist-info/RECORD,,
```

