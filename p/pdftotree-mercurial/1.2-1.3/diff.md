# Comparing `tmp/pdftotree-mercurial-1.2.tar.gz` & `tmp/pdftotree-mercurial-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftotree-mercurial-1.2.tar", last modified: Fri Apr 21 18:58:45 2023, max compression
+gzip compressed data, was "pdftotree-mercurial-1.3.tar", last modified: Wed Apr 26 16:53:51 2023, max compression
```

## Comparing `pdftotree-mercurial-1.2.tar` & `pdftotree-mercurial-1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.072572 pdftotree-mercurial-1.2/
--rw-rw-rw-   0        0        0     1090 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/LICENSE
--rw-rw-rw-   0        0        0      930 2023-04-21 18:58:45.072572 pdftotree-mercurial-1.2/PKG-INFO
--rw-rw-rw-   0        0        0    10095 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.034206 pdftotree-mercurial-1.2/bin/
--rw-rw-rw-   0        0        0    15070 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/bin/extract_tables
--rw-rw-rw-   0        0        0     2845 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/bin/pdftotree
-drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.039614 pdftotree-mercurial-1.2/pdftotree/
--rw-rw-rw-   0        0        0    22575 2023-04-21 18:58:14.000000 pdftotree-mercurial-1.2/pdftotree/TreeExtract.py
--rw-rw-rw-   0        0        0     3732 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/TreeVisualizer.py
--rw-rw-rw-   0        0        0      298 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/__init__.py
--rw-rw-rw-   0        0        0       27 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/_version.py
--rw-rw-rw-   0        0        0     2361 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/core.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.041612 pdftotree-mercurial-1.2/pdftotree/ml/
--rw-rw-rw-   0        0        0     5333 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/ml/TableExtractML.py
--rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/ml/__init__.py
--rw-rw-rw-   0        0        0     5759 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/ml/features.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.045613 pdftotree-mercurial-1.2/pdftotree/utils/
--rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/__init__.py
--rw-rw-rw-   0        0        0     5325 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/bbox_utils.py
--rw-rw-rw-   0        0        0     2603 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/display_utils.py
--rw-rw-rw-   0        0        0     5113 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/img_utils.py
--rw-rw-rw-   0        0        0     4484 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/lines_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.052647 pdftotree-mercurial-1.2/pdftotree/utils/pdf/
--rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/__init__.py
--rw-rw-rw-   0        0        0     6720 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/grid.py
--rw-rw-rw-   0        0        0     7810 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/layout_utils.py
--rw-rw-rw-   0        0        0     7752 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/node.py
--rw-rw-rw-   0        0        0    52985 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/pdf_parsers.py
--rw-rw-rw-   0        0        0     9496 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/pdf_utils.py
--rw-rw-rw-   0        0        0     2101 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/render.py
--rw-rw-rw-   0        0        0     6101 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/vector_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.054645 pdftotree-mercurial-1.2/pdftotree/visual/
--rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/visual/__init__.py
--rw-rw-rw-   0        0        0     5318 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/visual/visual_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.067832 pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/
--rw-rw-rw-   0        0        0      930 2023-04-21 18:58:44.000000 pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1060 2023-04-21 18:58:44.000000 pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:58:44.000000 pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-04-21 18:58:44.000000 pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-21 18:58:44.000000 pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      159 2023-04-21 18:58:45.074570 pdftotree-mercurial-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1581 2023-04-21 18:58:40.000000 pdftotree-mercurial-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.071573 pdftotree-mercurial-1.2/tests/
--rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     5811 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/tests/test_basic.py
--rw-rw-rw-   0        0        0      629 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/tests/test_figures.py
--rw-rw-rw-   0        0        0     1028 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/tests/test_table_detection.py
--rw-rw-rw-   0        0        0      681 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/tests/test_text.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:53:51.627679 pdftotree-mercurial-1.3/
+-rw-rw-rw-   0        0        0     1090 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/LICENSE
+-rw-rw-rw-   0        0        0      930 2023-04-26 16:53:51.628683 pdftotree-mercurial-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10095 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-26 16:53:51.569680 pdftotree-mercurial-1.3/bin/
+-rw-rw-rw-   0        0        0    15070 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/bin/extract_tables
+-rw-rw-rw-   0        0        0     2845 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/bin/pdftotree
+drwxrwxrwx   0        0        0        0 2023-04-26 16:53:51.575685 pdftotree-mercurial-1.3/pdftotree/
+-rw-rw-rw-   0        0        0    20852 2023-04-26 16:52:03.000000 pdftotree-mercurial-1.3/pdftotree/TreeExtract.py
+-rw-rw-rw-   0        0        0     3732 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/TreeVisualizer.py
+-rw-rw-rw-   0        0        0      298 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/__init__.py
+-rw-rw-rw-   0        0        0       27 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/_version.py
+-rw-rw-rw-   0        0        0     2361 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/core.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:53:51.581715 pdftotree-mercurial-1.3/pdftotree/ml/
+-rw-rw-rw-   0        0        0     5333 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/ml/TableExtractML.py
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/ml/__init__.py
+-rw-rw-rw-   0        0        0     5759 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/ml/features.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:53:51.587680 pdftotree-mercurial-1.3/pdftotree/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/__init__.py
+-rw-rw-rw-   0        0        0     5325 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/bbox_utils.py
+-rw-rw-rw-   0        0        0     2603 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/display_utils.py
+-rw-rw-rw-   0        0        0     5113 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/img_utils.py
+-rw-rw-rw-   0        0        0     4484 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/lines_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:53:51.598681 pdftotree-mercurial-1.3/pdftotree/utils/pdf/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/pdf/__init__.py
+-rw-rw-rw-   0        0        0     6720 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/pdf/grid.py
+-rw-rw-rw-   0        0        0     7810 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/pdf/layout_utils.py
+-rw-rw-rw-   0        0        0     7752 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/pdf/node.py
+-rw-rw-rw-   0        0        0    52985 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/pdf/pdf_parsers.py
+-rw-rw-rw-   0        0        0     9496 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/pdf/pdf_utils.py
+-rw-rw-rw-   0        0        0     2101 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/pdf/render.py
+-rw-rw-rw-   0        0        0     6101 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/utils/pdf/vector_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:53:51.601681 pdftotree-mercurial-1.3/pdftotree/visual/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/visual/__init__.py
+-rw-rw-rw-   0        0        0     5318 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/pdftotree/visual/visual_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:53:51.620679 pdftotree-mercurial-1.3/pdftotree_mercurial.egg-info/
+-rw-rw-rw-   0        0        0      930 2023-04-26 16:53:51.000000 pdftotree-mercurial-1.3/pdftotree_mercurial.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1060 2023-04-26 16:53:51.000000 pdftotree-mercurial-1.3/pdftotree_mercurial.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 16:53:51.000000 pdftotree-mercurial-1.3/pdftotree_mercurial.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-04-26 16:53:51.000000 pdftotree-mercurial-1.3/pdftotree_mercurial.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-26 16:53:51.000000 pdftotree-mercurial-1.3/pdftotree_mercurial.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      159 2023-04-26 16:53:51.634684 pdftotree-mercurial-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1581 2023-04-26 16:52:03.000000 pdftotree-mercurial-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:53:51.626681 pdftotree-mercurial-1.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     5811 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/tests/test_basic.py
+-rw-rw-rw-   0        0        0      629 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/tests/test_figures.py
+-rw-rw-rw-   0        0        0     1028 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/tests/test_table_detection.py
+-rw-rw-rw-   0        0        0      681 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.3/tests/test_text.py
```

### Comparing `pdftotree-mercurial-1.2/LICENSE` & `pdftotree-mercurial-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/PKG-INFO` & `pdftotree-mercurial-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftotree-mercurial
-Version: 1.2
+Version: 1.3
 Summary: Convert PDF into hOCR with text, tables, and figures being recognized and preserved. (Without sklearn in dependencies)
 Home-page: https://github.com/HazyResearch/pdftotree
 Author: Hazy Research
 Author-email: senwu@cs.stanford.edu
 License: MIT
 Project-URL: Tracker, https://github.com/HazyResearch/pdftotree/issues
 Project-URL: Source, https://github.com/HazyResearch/pdftotree
```

### Comparing `pdftotree-mercurial-1.2/README.rst` & `pdftotree-mercurial-1.3/README.rst`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/bin/extract_tables` & `pdftotree-mercurial-1.3/bin/extract_tables`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/bin/pdftotree` & `pdftotree-mercurial-1.3/bin/pdftotree`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/TreeExtract.py` & `pdftotree-mercurial-1.3/pdftotree/TreeExtract.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,44 +326,14 @@
             boxes.sort(key=cmp_to_key(column_order))
 
             for box in boxes:
                 if box[0] == "table":
                     table = box[1:]  # bbox
                     table_element = self.get_html_table(table, page_num)
                     page.appendChild(table_element)
-                elif box[0] == "figure":
-                    elems: List[LTTextLine] = get_mentions_within_bbox(
-                        box, self.elems[page_num].figures
-                    )
-                    fig_element = doc.createElement("figure")
-                    page.appendChild(fig_element)
-                    top, left, bottom, right = [int(i) for i in box[1:]]
-                    fig_element.setAttribute(
-                        "title", f"bbox {left} {top} {right} {bottom}"
-                    )
-                    for img in [img for elem in elems for img in elem]:
-                        if not isinstance(img, LTImage):
-                            continue
-                        filename = imagewriter.export_image(img)
-                        with open(os.path.join(dirname, filename), "rb") as f:
-                            base64 = b64encode(f.read()).decode("ascii")
-                        if filename.endswith("jpg"):
-                            mediatype = "jpeg"
-                        elif filename.endswith("bmp"):
-                            mediatype = "bmp"
-                        else:
-                            logger.info(f"Skipping an unknown type image: {filename}.")
-                            continue
-                        logger.info(f"Embedding a known type image: {filename}.")
-                        img_element = doc.createElement("img")
-                        fig_element.appendChild(img_element)
-                        img_element.setAttribute("title", bbox2str(img.bbox))
-                        img_element.setAttribute(
-                            "src", f"data:image/{mediatype};base64,{base64}"
-                        )
                 else:
                     element = self.get_html_others(box[0], box[1:], page_num)
                     page.appendChild(element)
         return doc.toprettyxml()
 
     def get_word_boundaries(
         self, mention: LTTextLine
```

### Comparing `pdftotree-mercurial-1.2/pdftotree/TreeVisualizer.py` & `pdftotree-mercurial-1.3/pdftotree/TreeVisualizer.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/core.py` & `pdftotree-mercurial-1.3/pdftotree/core.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/ml/TableExtractML.py` & `pdftotree-mercurial-1.3/pdftotree/ml/TableExtractML.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/ml/features.py` & `pdftotree-mercurial-1.3/pdftotree/ml/features.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/utils/bbox_utils.py` & `pdftotree-mercurial-1.3/pdftotree/utils/bbox_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/utils/display_utils.py` & `pdftotree-mercurial-1.3/pdftotree/utils/display_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/utils/img_utils.py` & `pdftotree-mercurial-1.3/pdftotree/utils/img_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/utils/lines_utils.py` & `pdftotree-mercurial-1.3/pdftotree/utils/lines_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/utils/pdf/grid.py` & `pdftotree-mercurial-1.3/pdftotree/utils/pdf/grid.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/utils/pdf/layout_utils.py` & `pdftotree-mercurial-1.3/pdftotree/utils/pdf/layout_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/utils/pdf/node.py` & `pdftotree-mercurial-1.3/pdftotree/utils/pdf/node.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/utils/pdf/pdf_parsers.py` & `pdftotree-mercurial-1.3/pdftotree/utils/pdf/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/utils/pdf/pdf_utils.py` & `pdftotree-mercurial-1.3/pdftotree/utils/pdf/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/utils/pdf/render.py` & `pdftotree-mercurial-1.3/pdftotree/utils/pdf/render.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/utils/pdf/vector_utils.py` & `pdftotree-mercurial-1.3/pdftotree/utils/pdf/vector_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree/visual/visual_utils.py` & `pdftotree-mercurial-1.3/pdftotree/visual/visual_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/PKG-INFO` & `pdftotree-mercurial-1.3/pdftotree_mercurial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftotree-mercurial
-Version: 1.2
+Version: 1.3
 Summary: Convert PDF into hOCR with text, tables, and figures being recognized and preserved. (Without sklearn in dependencies)
 Home-page: https://github.com/HazyResearch/pdftotree
 Author: Hazy Research
 Author-email: senwu@cs.stanford.edu
 License: MIT
 Project-URL: Tracker, https://github.com/HazyResearch/pdftotree/issues
 Project-URL: Source, https://github.com/HazyResearch/pdftotree
```

### Comparing `pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/SOURCES.txt` & `pdftotree-mercurial-1.3/pdftotree_mercurial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/setup.py` & `pdftotree-mercurial-1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """For pip."""
 from setuptools import find_packages, setup
 
 exec(open("pdftotree/_version.py").read())
 setup(
     name="pdftotree-mercurial",
-    version='1.2',
+    version='1.3',
     description="Convert PDF into hOCR with text, tables, and figures being recognized and preserved. (Without "
                 "sklearn in dependencies)",
     packages=find_packages(),
     install_requires=[
         "IPython",
         "beautifulsoup4",
         "numpy",
```

### Comparing `pdftotree-mercurial-1.2/tests/test_basic.py` & `pdftotree-mercurial-1.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/tests/test_figures.py` & `pdftotree-mercurial-1.3/tests/test_figures.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/tests/test_table_detection.py` & `pdftotree-mercurial-1.3/tests/test_table_detection.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.2/tests/test_text.py` & `pdftotree-mercurial-1.3/tests/test_text.py`

 * *Files identical despite different names*

