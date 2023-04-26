# Comparing `tmp/XMLCit-0.0.8.tar.gz` & `tmp/XMLCit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XMLCit-0.0.8.tar", last modified: Sun Apr 23 18:24:40 2023, max compression
+gzip compressed data, was "XMLCit-0.0.9.tar", last modified: Tue Apr 25 21:13:36 2023, max compression
```

## Comparing `XMLCit-0.0.8.tar` & `XMLCit-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 18:24:40.530737 XMLCit-0.0.8/
--rw-rw-rw-   0        0        0     1086 2023-04-20 02:25:43.000000 XMLCit-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     4453 2023-04-23 18:24:40.530737 XMLCit-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3854 2023-04-23 18:22:55.000000 XMLCit-0.0.8/README.md
--rw-rw-rw-   0        0        0       88 2023-04-21 20:44:49.000000 XMLCit-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      743 2023-04-23 18:24:40.537824 XMLCit-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 18:24:40.503575 XMLCit-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 18:24:40.511571 XMLCit-0.0.8/src/XMLCit/
--rw-rw-rw-   0        0        0        0 2023-04-20 03:24:00.000000 XMLCit-0.0.8/src/XMLCit/__init__.py
--rw-rw-rw-   0        0        0    15638 2023-04-21 20:46:24.000000 XMLCit-0.0.8/src/XMLCit/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-23 18:24:40.529756 XMLCit-0.0.8/src/XMLCit.egg-info/
--rw-rw-rw-   0        0        0     4453 2023-04-23 18:24:40.000000 XMLCit-0.0.8/src/XMLCit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-04-23 18:24:40.000000 XMLCit-0.0.8/src/XMLCit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 18:24:40.000000 XMLCit-0.0.8/src/XMLCit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-23 18:24:40.000000 XMLCit-0.0.8/src/XMLCit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 21:13:36.390511 XMLCit-0.0.9/
+-rw-rw-rw-   0        0        0     1087 2023-04-25 21:11:26.000000 XMLCit-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4450 2023-04-25 21:13:36.390511 XMLCit-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3851 2023-04-25 21:10:00.000000 XMLCit-0.0.9/README.md
+-rw-rw-rw-   0        0        0       88 2023-04-21 20:44:49.000000 XMLCit-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      743 2023-04-25 21:13:36.396025 XMLCit-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 21:13:36.342251 XMLCit-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 21:13:36.349975 XMLCit-0.0.9/src/XMLCit/
+-rw-rw-rw-   0        0        0        0 2023-04-20 03:24:00.000000 XMLCit-0.0.9/src/XMLCit/__init__.py
+-rw-rw-rw-   0        0        0    15638 2023-04-21 20:46:24.000000 XMLCit-0.0.9/src/XMLCit/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:13:36.390511 XMLCit-0.0.9/src/XMLCit.egg-info/
+-rw-rw-rw-   0        0        0     4450 2023-04-25 21:13:36.000000 XMLCit-0.0.9/src/XMLCit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-04-25 21:13:36.000000 XMLCit-0.0.9/src/XMLCit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 21:13:36.000000 XMLCit-0.0.9/src/XMLCit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-25 21:13:36.000000 XMLCit-0.0.9/src/XMLCit.egg-info/top_level.txt
```

### Comparing `XMLCit-0.0.8/LICENSE` & `XMLCit-0.0.9/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 Research Computing Center
+Copyright (c) 2023 Jose Angel Hernandez Perez
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `XMLCit-0.0.8/PKG-INFO` & `XMLCit-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XMLCit
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package was made to edit XML files ( particularly TEI-XML files). The main purpose is to facilitate the tagging and edit of repeated citations and the inclusion of VIAF records
 Home-page: https://github.com/hernandezj1/XMLCit
 Author: Jose Hernandez
 Author-email: jose.hndz.prz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # XMLCit package
 
 ## Purpose
  
-  This packages was developed by staff of the Research Computing Center at Florida State University to serve the needs of our digital humanities community. Therefore the methods and functions in this package were developed with ease of use in mind and to be specifically applicable to TEI-XML standards. TEI-XML specifications can be found here <a href='https://tei-c.org/'>TEI</a>
+  This packages was developed to serve the needs of the digital humanities community particularly those working with repeated citation on TEI-XML texts. Therefore the methods and functions in this package were developed with ease of use in mind and to be specifically applicable to TEI-XML standards. TEI-XML specifications can be found here <a href='https://tei-c.org/'>TEI</a>
 
   The functions and methods here encompassed modify XMl documents on a large scale to avoid tedious work by the researcher. The main goald of this package was to provide a way to do the following: 
 
   1. Tag a specific word within every instance of a specific node of the TEI-XMl document. In our case this was specific citations within the __note__ node.
   
   2. Add attributes to every instance of a specific node based on the presence of an ID number attribute or a specific collection of words inside said node. These attributes where:
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: XMLCit Version: 0.0.8 Summary: This package was
+Metadata-Version: 2.1 Name: XMLCit Version: 0.0.9 Summary: This package was
 made to edit XML files ( particularly TEI-XML files). The main purpose is to
 facilitate the tagging and edit of repeated citations and the inclusion of VIAF
 records Home-page: https://github.com/hernandezj1/XMLCit Author: Jose Hernandez
 Author-email: jose.hndz.prz@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE # XMLCit package ## Purpose This
-packages was developed by staff of the Research Computing Center at Florida
-State University to serve the needs of our digital humanities community.
-Therefore the methods and functions in this package were developed with ease of
-use in mind and to be specifically applicable to TEI-XML standards. TEI-XML
+packages was developed to serve the needs of the digital humanities community
+particularly those working with repeated citation on TEI-XML texts. Therefore
+the methods and functions in this package were developed with ease of use in
+mind and to be specifically applicable to TEI-XML standards. TEI-XML
 specifications can be found here TEI The functions and methods here encompassed
 modify XMl documents on a large scale to avoid tedious work by the researcher.
 The main goald of this package was to provide a way to do the following: 1. Tag
 a specific word within every instance of a specific node of the TEI-XMl
 document. In our case this was specific citations within the __note__ node. 2.
 Add attributes to every instance of a specific node based on the presence of an
 ID number attribute or a specific collection of words inside said node. These
```

### Comparing `XMLCit-0.0.8/README.md` & `XMLCit-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # XMLCit package
 
 ## Purpose
  
-  This packages was developed by staff of the Research Computing Center at Florida State University to serve the needs of our digital humanities community. Therefore the methods and functions in this package were developed with ease of use in mind and to be specifically applicable to TEI-XML standards. TEI-XML specifications can be found here <a href='https://tei-c.org/'>TEI</a>
+  This packages was developed to serve the needs of the digital humanities community particularly those working with repeated citation on TEI-XML texts. Therefore the methods and functions in this package were developed with ease of use in mind and to be specifically applicable to TEI-XML standards. TEI-XML specifications can be found here <a href='https://tei-c.org/'>TEI</a>
 
   The functions and methods here encompassed modify XMl documents on a large scale to avoid tedious work by the researcher. The main goald of this package was to provide a way to do the following: 
 
   1. Tag a specific word within every instance of a specific node of the TEI-XMl document. In our case this was specific citations within the __note__ node.
   
   2. Add attributes to every instance of a specific node based on the presence of an ID number attribute or a specific collection of words inside said node. These attributes where:
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-# XMLCit package ## Purpose This packages was developed by staff of the
-Research Computing Center at Florida State University to serve the needs of our
-digital humanities community. Therefore the methods and functions in this
-package were developed with ease of use in mind and to be specifically
-applicable to TEI-XML standards. TEI-XML specifications can be found here TEI
-The functions and methods here encompassed modify XMl documents on a large
-scale to avoid tedious work by the researcher. The main goald of this package
-was to provide a way to do the following: 1. Tag a specific word within every
-instance of a specific node of the TEI-XMl document. In our case this was
-specific citations within the __note__ node. 2. Add attributes to every
-instance of a specific node based on the presence of an ID number attribute or
-a specific collection of words inside said node. These attributes where: a. A
-VIAF number, webscraped from the VIAF website b. an ID number c. A completed
-citation. __Usage guidelines:__ To import the libary please use the next few
-lines in your code. It is key that for the methods inside the Insert class you
-define an instance of this class beforehand. ``` from XMLCit import functions #
-After this all functions can be found by doing the following: functions.AddVIAF
+# XMLCit package ## Purpose This packages was developed to serve the needs of
+the digital humanities community particularly those working with repeated
+citation on TEI-XML texts. Therefore the methods and functions in this package
+were developed with ease of use in mind and to be specifically applicable to
+TEI-XML standards. TEI-XML specifications can be found here TEI The functions
+and methods here encompassed modify XMl documents on a large scale to avoid
+tedious work by the researcher. The main goald of this package was to provide a
+way to do the following: 1. Tag a specific word within every instance of a
+specific node of the TEI-XMl document. In our case this was specific citations
+within the __note__ node. 2. Add attributes to every instance of a specific
+node based on the presence of an ID number attribute or a specific collection
+of words inside said node. These attributes where: a. A VIAF number, webscraped
+from the VIAF website b. an ID number c. A completed citation. __Usage
+guidelines:__ To import the libary please use the next few lines in your code.
+It is key that for the methods inside the Insert class you define an instance
+of this class beforehand. ``` from XMLCit import functions # After this all
+functions can be found by doing the following: functions.AddVIAF
 functions.Addtag functions.RepeatCitation #To use the class methods do the
 following: instance = functions.Insert() #then you can use this instance to
 call each of the methods and not include the self parameter instance.ID()
 instance.CitbyID() instance.CitbyText() ``` ## Structure Due to the brevity of
 this package only a single module was made to hold one class( with 3 methods)
 and the 3 additional functions. ## Class description : Insert This class
 focuses on the Insertion of attributes into tags in the XML documents. ###
```

### Comparing `XMLCit-0.0.8/setup.cfg` & `XMLCit-0.0.9/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2058 4d4c 4369 740d 0a76 6572 7369   = XMLCit..versi
-00000020: 6f6e 203d 2030 2e30 2e38 0d0a 6175 7468  on = 0.0.8..auth
+00000020: 6f6e 203d 2030 2e30 2e39 0d0a 6175 7468  on = 0.0.9..auth
 00000030: 6f72 203d 204a 6f73 6520 4865 726e 616e  or = Jose Hernan
 00000040: 6465 7a0d 0a61 7574 686f 725f 656d 6169  dez..author_emai
 00000050: 6c20 3d20 6a6f 7365 2e68 6e64 7a2e 7072  l = jose.hndz.pr
 00000060: 7a40 676d 6169 6c2e 636f 6d0d 0a64 6573  z@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2054 6869 7320  cription = This 
 00000080: 7061 636b 6167 6520 7761 7320 6d61 6465  package was made
 00000090: 2074 6f20 6564 6974 2058 4d4c 2066 696c   to edit XML fil
```

### Comparing `XMLCit-0.0.8/src/XMLCit/functions.py` & `XMLCit-0.0.9/src/XMLCit/functions.py`

 * *Files identical despite different names*

### Comparing `XMLCit-0.0.8/src/XMLCit.egg-info/PKG-INFO` & `XMLCit-0.0.9/src/XMLCit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XMLCit
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package was made to edit XML files ( particularly TEI-XML files). The main purpose is to facilitate the tagging and edit of repeated citations and the inclusion of VIAF records
 Home-page: https://github.com/hernandezj1/XMLCit
 Author: Jose Hernandez
 Author-email: jose.hndz.prz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # XMLCit package
 
 ## Purpose
  
-  This packages was developed by staff of the Research Computing Center at Florida State University to serve the needs of our digital humanities community. Therefore the methods and functions in this package were developed with ease of use in mind and to be specifically applicable to TEI-XML standards. TEI-XML specifications can be found here <a href='https://tei-c.org/'>TEI</a>
+  This packages was developed to serve the needs of the digital humanities community particularly those working with repeated citation on TEI-XML texts. Therefore the methods and functions in this package were developed with ease of use in mind and to be specifically applicable to TEI-XML standards. TEI-XML specifications can be found here <a href='https://tei-c.org/'>TEI</a>
 
   The functions and methods here encompassed modify XMl documents on a large scale to avoid tedious work by the researcher. The main goald of this package was to provide a way to do the following: 
 
   1. Tag a specific word within every instance of a specific node of the TEI-XMl document. In our case this was specific citations within the __note__ node.
   
   2. Add attributes to every instance of a specific node based on the presence of an ID number attribute or a specific collection of words inside said node. These attributes where:
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: XMLCit Version: 0.0.8 Summary: This package was
+Metadata-Version: 2.1 Name: XMLCit Version: 0.0.9 Summary: This package was
 made to edit XML files ( particularly TEI-XML files). The main purpose is to
 facilitate the tagging and edit of repeated citations and the inclusion of VIAF
 records Home-page: https://github.com/hernandezj1/XMLCit Author: Jose Hernandez
 Author-email: jose.hndz.prz@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE # XMLCit package ## Purpose This
-packages was developed by staff of the Research Computing Center at Florida
-State University to serve the needs of our digital humanities community.
-Therefore the methods and functions in this package were developed with ease of
-use in mind and to be specifically applicable to TEI-XML standards. TEI-XML
+packages was developed to serve the needs of the digital humanities community
+particularly those working with repeated citation on TEI-XML texts. Therefore
+the methods and functions in this package were developed with ease of use in
+mind and to be specifically applicable to TEI-XML standards. TEI-XML
 specifications can be found here TEI The functions and methods here encompassed
 modify XMl documents on a large scale to avoid tedious work by the researcher.
 The main goald of this package was to provide a way to do the following: 1. Tag
 a specific word within every instance of a specific node of the TEI-XMl
 document. In our case this was specific citations within the __note__ node. 2.
 Add attributes to every instance of a specific node based on the presence of an
 ID number attribute or a specific collection of words inside said node. These
```

