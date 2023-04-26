# Comparing `tmp/dl_track_us-0.1.2.1.tar.gz` & `tmp/dl_track_us-0.1.2.2.tar.gz`

## Comparing `dl_track_us-0.1.2.1.tar` & `dl_track_us-0.1.2.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/.DS_Store
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/.gitattributes
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/.readthedocs.yml
--rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/README.md
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/environment.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/requirements.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/setup.cfg
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/setup.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/.github/workflows/draft-pdf.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/.vscode/settings.json
--rw-r--r--   0        0        0    64168 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/DL_Track_US_GUI.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/__main__.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/__init__.py
--rw-r--r--   0        0        0    29061 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/calculate_architecture.py
--rw-r--r--   0        0        0    24000 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/calculate_architecture_video.py
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/calibrate.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/calibrate_video.py
--rw-r--r--   0        0        0    23434 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/do_calculations.py
--rw-r--r--   0        0        0    27202 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/do_calculations_video.py
--rw-r--r--   0        0        0   151070 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/home_im.ico
--rw-r--r--   0        0        0    37179 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/manual_tracing.py
--rw-r--r--   0        0        0    27656 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/model_training.py
--rw-r--r--   0        0        0    33610 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/Figures/Figure_B-A.png
--rw-r--r--   0        0        0   149706 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/Figures/Figure_GUI.png
--rw-r--r--   0        0        0   175264 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/Figures/Figure_analysis.png
--rw-r--r--   0        0        0   494274 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/Figures/Figure_video.png
--rw-r--r--   0        0        0   134843 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/Figures/home_im.png
--rw-r--r--   0        0        0   175264 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/Paper/figure1.png
--rw-r--r--   0        0        0   149706 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/Paper/figure2.png
--rw-r--r--   0        0        0    28350 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/Paper/paper.bib
--rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/Paper/paper.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/changelog.d/20221107_105509_paul.ritsche_pip_package_pr.rst
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/changelog.d/20221114_112818_paul.ritsche.rst
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/changelog.d/20230401_211702_paul.ritsche.rst
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/.DS_Store
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/make.bat
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/image_labelling/Image_Labeling_DLTrack.ijm
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/source/DL_Track_US.gui_helpers.rst
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/source/DL_Track_US.rst
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/source/conf.py
--rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/source/contribute.rst
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/source/index.rst
--rw-r--r--   0        0        0    10436 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/source/installation.rst
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/source/modules.rst
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/source/requirements.txt
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/source/tests.rst
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/source/usage.rst
--rw-r--r--   0        0        0  6497682 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/docs/usage/DL_Track_US_tutorial.pdf
--rw-r--r--   0        0        0  1418858 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/tests/DL_Track_US_tests.pdf
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/LICENSE
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/README_Pypi.md
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/pyproject.toml
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/.DS_Store
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/.gitattributes
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/.readthedocs.yml
+-rw-r--r--   0        0        0     6376 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/README.md
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/environment.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/requirements.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/setup.cfg
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/setup.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/.github/workflows/draft-pdf.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0    64114 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/DL_Track_US_GUI.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/__main__.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/__init__.py
+-rw-r--r--   0        0        0    29061 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/calculate_architecture.py
+-rw-r--r--   0        0        0    23978 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/calculate_architecture_video.py
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/calibrate.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/calibrate_video.py
+-rw-r--r--   0        0        0    23483 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/do_calculations.py
+-rw-r--r--   0        0        0    27202 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/do_calculations_video.py
+-rw-r--r--   0        0        0   151070 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/home_im.ico
+-rw-r--r--   0        0        0    37179 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/manual_tracing.py
+-rw-r--r--   0        0        0    27656 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/model_training.py
+-rw-r--r--   0        0        0    33610 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/Figures/Figure_B-A.png
+-rw-r--r--   0        0        0   149706 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/Figures/Figure_GUI.png
+-rw-r--r--   0        0        0   175264 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/Figures/Figure_analysis.png
+-rw-r--r--   0        0        0   494274 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/Figures/Figure_video.png
+-rw-r--r--   0        0        0   134843 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/Figures/home_im.png
+-rw-r--r--   0        0        0   175264 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/Paper/figure1.png
+-rw-r--r--   0        0        0   149706 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/Paper/figure2.png
+-rw-r--r--   0        0        0    28350 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/Paper/paper.bib
+-rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/Paper/paper.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/changelog.d/20221107_105509_paul.ritsche_pip_package_pr.rst
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/changelog.d/20221114_112818_paul.ritsche.rst
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/changelog.d/20230401_211702_paul.ritsche.rst
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/.DS_Store
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/make.bat
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/image_labelling/Image_Labeling_DLTrack.ijm
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/source/DL_Track_US.gui_helpers.rst
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/source/DL_Track_US.rst
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/source/conf.py
+-rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/source/contribute.rst
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/source/index.rst
+-rw-r--r--   0        0        0    10466 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/source/installation.rst
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/source/modules.rst
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/source/requirements.txt
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/source/tests.rst
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/source/usage.rst
+-rw-r--r--   0        0        0  7373079 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/docs/usage/DL_Track_US_tutorial.pdf
+-rw-r--r--   0        0        0  1389121 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/tests/DL_Track_US_tests.pdf
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/LICENSE
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/README_Pypi.md
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 dl_track_us-0.1.2.2/PKG-INFO
```

### Comparing `dl_track_us-0.1.2.1/.DS_Store` & `dl_track_us-0.1.2.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/.readthedocs.yml` & `dl_track_us-0.1.2.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/README.md` & `dl_track_us-0.1.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # DL_Track_US
 
 [![Documentation Status](https://readthedocs.org/projects/dltrack/badge/?version=latest)](https://dltrack.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7805896.svg)](https://doi.org/10.5281/zenodo.7805896)
 
 ![DL_Track_US image](./Figures/home_im.png)
 
-The DL_Track_US package provides an easy to use graphical user interface (GUI) for deep learning based analysis of muscle architectural parameters from longitudinal ultrasonography images of human lower limb muscles. Please take a look at our [documentation](https://dltrack.readthedocs.io/en/latest/index.html) for more information (note that agressive ad-blockers might break the visualization of the repository description as well as the online documentation).
+The DL_Track_US package provides an easy to use graphical user interface (GUI) for deep learning based analysis of muscle architectural parameters from longitudinal ultrasonography images of human lower limb muscles. Please take a look at our [documentation](https://dltrack.readthedocs.io/en/latest/index.html) for more information (note that aggressive ad-blockers might break the visualization of the repository description as well as the online documentation).
 This code is based on a previously published [algorithm](https://github.com/njcronin/DL_Track) and replaces it. We have extended the functionalities of the previously proposed code. The previous code will not be updated and future updates will be included in this repository. 
 
 ## Getting started
 
 For detailled information about installaion of the DL_Track_US python package we refer you to our [documentation](https://dltrack.readthedocs.io/en/latest/installation.html). There you will finde guidelines not only for the installation procedure of DL_Track_US, but also concerding conda and GPU setup.
 
 ## Quickstart
@@ -50,8 +50,8 @@
 
 ## Related Work
 
 The DL_Track_US package can only be used for the automatic analysis of longitudinal muscle ultrasonography images containing muscle architectural parameters. However, in order to assess muscle anatomical cross-sectional area (ACSA), panoramic ultrasonography images in the transversal plane are required. We recently published [DeepACSA](https://journals.lww.com/acsm-msse/Abstract/2022/12000/DeepACSA__Automatic_Segmentation_of.21.aspx), an open source algorithm for automatic analysis of muscle ACSA in panoramic ultrasonography images of the human vastus lateralis, rectus femoris and gastrocnemius medialis. The repository containing the code and installation as well as usage instructions is locate [here](https://github.com/PaulRitsche/DeepACSA).
 
 ## Community guidelines
 
-Wheter you want to contribute, report a bug or have troubles with the DL_Track_US package, take a look at the provided [instructions](https://dltrack.readthedocs.io/en/latest/contribute.html) how to best do so. You can also contact us via email at paul.ritsche@unibas.ch, but we would prefer you to open a discussion as described in the instructions.
+Wheter you want to contribute, report a bug or have troubles with the DL_Track_US package, take a look at the provided [instructions](https://dltrack.readthedocs.io/en/latest/contribute.html) how to best do so.
```

### Comparing `dl_track_us-0.1.2.1/setup.py` & `dl_track_us-0.1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/.github/workflows/draft-pdf.yml` & `dl_track_us-0.1.2.2/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/DL_Track_US/DL_Track_US_GUI.py` & `dl_track_us-0.1.2.2/DL_Track_US/DL_Track_US_GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,27 +499,27 @@
         no_scaling.grid(column=4, row=14, sticky=(W, E))
         self.scaling.set("Bar")
 
         # Comboboxes
         # Filetype
         self.filetype = StringVar()
         filetype = (
-            "/**/*.tif",
-            "/**/*.tiff",
-            "/**/*.png",
-            "/**/*.bmp",
-            "/**/*.jpeg",
-            "/**/*.jpg",
+            "/*.tif",
+            "/*.tiff",
+            "/*.png",
+            "/*.bmp",
+            "/*.jpeg",
+            "/*.jpg",
         )
         filetype_entry = ttk.Combobox(self.main, width=10,
                                       textvariable=self.filetype)
         filetype_entry["values"] = filetype
         # filetype_entry["state"] = "readonly"
         filetype_entry.grid(column=2, row=13, sticky=(W, E))
-        self.filetype.set("/**/*.tiff")
+        self.filetype.set("/*.tiff")
 
         # Spacing
         self.spacing = StringVar()
         spacing = (5, 10, 15, 20)
         spacing_entry = ttk.Combobox(self.main, width=10,
                                      textvariable=self.spacing)
         spacing_entry["values"] = spacing
@@ -639,21 +639,21 @@
         )
         flip_n.grid(column=3, row=16, sticky=(W, E))
         self.flip.set("flip")
 
         # Comboboxes
         # Filetype
         self.filetype = StringVar()
-        filetype = ("/**/*.avi", "/**/*.mp4")
+        filetype = ("/*.avi", "/*.mp4")
         filetype_entry = ttk.Combobox(self.main, width=10,
                                       textvariable=self.filetype)
         filetype_entry["values"] = filetype
         # filetype_entry["state"] = "readonly"
         filetype_entry.grid(column=2, row=13, sticky=(W, E))
-        self.filetype.set("/**/*.avi")
+        self.filetype.set("/*.avi")
 
         # Spacing
         self.spacing = StringVar()
         spacing = (5, 10, 15, 20)
         spacing_entry = ttk.Combobox(self.main, width=10,
                                      textvariable=self.spacing)
         spacing_entry["values"] = spacing
@@ -712,28 +712,28 @@
             column=1, row=18, columnspan=6, sticky=(W, E), ipady=7
         )
 
         # Comboboxes
         # Filetype
         self.filetype = StringVar()
         filetype = (
-            "/**/*.tif",
-            "/**/*.tiff",
-            "/**/*.png",
-            "/**/*.bmp",
-            "/**/*.jpeg",
-            "/**/*.jpg",
-            "/**/*.avi",
+            "/*.tif",
+            "/*.tiff",
+            "/*.png",
+            "/*.bmp",
+            "/*.jpeg",
+            "/*.jpg",
+            "/*.avi",
         )
         filetype_entry = ttk.Combobox(self.main, width=10,
                                       textvariable=self.filetype)
         filetype_entry["values"] = filetype
         # filetype_entry["state"] = "readonly"
         filetype_entry.grid(column=2, row=13, sticky=(W, E))
-        self.filetype.set("/**/*.tif")
+        self.filetype.set("/*.tif")
 
     def video_manual(self):
         """Instance method to display the required parameters
         that need to be entered by the user when videos are
         evaluated manually.
         - File path:
                     The user must specify the absolute path to the
```

### Comparing `dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/__init__.py` & `dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/calculate_architecture.py` & `dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/calculate_architecture.py`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/calculate_architecture_video.py` & `dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/calculate_architecture_video.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,14 @@
 
     Examples
     --------
     >>> importVideo(vpath="C:/Users/Dokuments/videos/video1.avi")
     """
     # Video properties (do not edit)
     cap = cv2.VideoCapture(vpath)
-    print(type(cap))
     vid_len = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
     vid_fps = int(cap.get(cv2.CAP_PROP_FPS))
     vid_width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
     vid_height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
     filename = os.path.splitext(os.path.basename(vpath))[0]
     outpath = str(vpath[0:-4] + "_proc" + ".avi")
     vid_out = cv2.VideoWriter(
```

### Comparing `dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/calibrate.py` & `dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/calibrate.py`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/calibrate_video.py` & `dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/calibrate_video.py`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/do_calculations.py` & `dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/do_calculations.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,25 +570,27 @@
                     pennation.append(Apoangle - FascAng)
                     x_low1.append(coordsX[0].astype("int32"))
                     x_high1.append(coordsX[-1].astype("int32"))
                     coords = np.array(
                         list(zip(coordsX.astype("int32"),
                                  coordsY.astype("int32")))
                     )
-                    plt.plot(coordsX, coordsY, ":w", linewidth=6)
-        # cv2.polylines(imgT, [coords], False, (20, 15, 200), 3)
-
+                    plt.plot(coordsX, coordsY, color="red", alpha=0.3,
+                             linewidth=4)
+        
         # DISPLAY THE RESULTS
         plt.imshow(img_copy, cmap="gray")
         plt.title(f"Image ID: {filename}" + f"\n{scale_statement}",
                   fontsize=25)
         plt.plot(
-            low_x, low_y_new, marker="p", color="w", linewidth=10
+            low_x, low_y_new, marker="p", color="blue", linewidth=10,
+            alpha=0.1
         )  # Plot the aponeuroses
-        plt.plot(upp_x, upp_y_new, marker="p", color="w", linewidth=10)
+        plt.plot(upp_x, upp_y_new, marker="p", color="blue", linewidth=10,
+                 alpha=0.1)
 
         xplot = 125
         yplot = 700
 
         # Store the results for each frame and normalise using scale factor
         # (if calibration was done above)
         try:
```

### Comparing `dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/do_calculations_video.py` & `dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/do_calculations_video.py`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/home_im.ico` & `dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/home_im.ico`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/manual_tracing.py` & `dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/manual_tracing.py`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/DL_Track_US/gui_helpers/model_training.py` & `dl_track_us-0.1.2.2/DL_Track_US/gui_helpers/model_training.py`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/Figures/Figure_B-A.png` & `dl_track_us-0.1.2.2/Figures/Figure_B-A.png`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/Figures/Figure_GUI.png` & `dl_track_us-0.1.2.2/Figures/Figure_GUI.png`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/Figures/Figure_analysis.png` & `dl_track_us-0.1.2.2/Figures/Figure_analysis.png`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/Figures/Figure_video.png` & `dl_track_us-0.1.2.2/Figures/Figure_video.png`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/Figures/home_im.png` & `dl_track_us-0.1.2.2/Figures/home_im.png`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/Paper/figure1.png` & `dl_track_us-0.1.2.2/Paper/figure1.png`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/Paper/figure2.png` & `dl_track_us-0.1.2.2/Paper/figure2.png`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/Paper/paper.bib` & `dl_track_us-0.1.2.2/Paper/paper.bib`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/Paper/paper.md` & `dl_track_us-0.1.2.2/Paper/paper.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,10 +43,10 @@
 ![Process from original input image to output result for images of two muscles, gastrocnemius medialis (GM) and vastus lateralis (VL). Subsequent to inputting the original images into the models, predictions are generated by the models for the aponeuroses (apo) and fascicles as displayed in the binary images. Based on the binary image, the output result is calculated by post-processing operations, fascicles and aponeuroses are drawn and the values for fascicle length, pennation angle and muscle thickness are displayed.\label{fig:1}](figure1.png)
 
 All `DL_Track_US` functionalities are embedded in a graphical user interface (GUI) to allow easy and intuitive usage. Apart from automated analysis, a manual analysis option is included in the GUI as well. This is provided in case the pre-trained CNNs perform badly on input images or videos and subsequently to avoid switching between softwares. The start window of the GUI is presented in \autoref{fig:2} and more information on usage can be found in our repository.
 
 ![Start window of the DL_Track_US graphical user interface. Here, the input and model directories can be specified, the analysis type (image, video, image manual, video manual) selected and the analysis parameters specified. Moreover, users can choose to train their own models based on their own input images using the "Train Model" button to open a seperate window.\label{fig:2}](figure2.png)
 
 Although we included images of the human gastrocnemius medialis, tibialis anterior, soleus and vastus lateralis from four different devices, it is likely the provided pre-trained CNNs fail when images from different muscles or devices are analyzed. However, an option to train CNNs bases on user data is also included in the GUI. Users are thereby enabled to train own CNNs based on own image or video data. The training ultrasonography image data, the pre-trained CNNs, example usage files as well as usage and testing instructions are provided.
-`DL_Track_US` was developed to automatically segment muscle architectural parameters in longitudinal ultrasonography images or videos. Nevertheless, ultrasonography can be used to assess muscle anatomical cross-sectional area (ACSA) as well. We recently published DeepACSA [@ritsche], the counterpiece of DL_Track_US. DeepACSA was developed for automatic segmentation of muscle ACSA in transversal, panoramic ultrasonography images of the human rectus femoris, vastus lateralis and gastrocnemius muscles. 
+`DL_Track_US` was developed to automatically segment muscle architectural parameters in longitudinal ultrasonography images or videos. Nevertheless, ultrasonography can be used to assess muscle anatomical cross-sectional area (ACSA) as well. We recently published DeepACSA [@ritsche2022], the counterpiece of `DL_Track_US`. DeepACSA was developed for automatic segmentation of muscle ACSA in transversal, panoramic ultrasonography images of the human rectus femoris, vastus lateralis and gastrocnemius muscles. 
 
 # References
```

### Comparing `dl_track_us-0.1.2.1/changelog.d/20221107_105509_paul.ritsche_pip_package_pr.rst` & `dl_track_us-0.1.2.2/changelog.d/20221107_105509_paul.ritsche_pip_package_pr.rst`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/changelog.d/20221114_112818_paul.ritsche.rst` & `dl_track_us-0.1.2.2/changelog.d/20221114_112818_paul.ritsche.rst`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/changelog.d/20230401_211702_paul.ritsche.rst` & `dl_track_us-0.1.2.2/changelog.d/20230401_211702_paul.ritsche.rst`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/docs/.DS_Store` & `dl_track_us-0.1.2.2/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/docs/Makefile` & `dl_track_us-0.1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/docs/make.bat` & `dl_track_us-0.1.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/docs/image_labelling/Image_Labeling_DLTrack.ijm` & `dl_track_us-0.1.2.2/docs/image_labelling/Image_Labeling_DLTrack.ijm`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/docs/source/DL_Track_US.gui_helpers.rst` & `dl_track_us-0.1.2.2/docs/source/DL_Track_US.gui_helpers.rst`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/docs/source/conf.py` & `dl_track_us-0.1.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/docs/source/contribute.rst` & `dl_track_us-0.1.2.2/docs/source/contribute.rst`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/docs/source/index.rst` & `dl_track_us-0.1.2.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/docs/source/installation.rst` & `dl_track_us-0.1.2.2/docs/source/installation.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Installation
 ============
 
-We offer two possible installation approaches for our DL_Track software. The first option is to download the DL_Track executable file. The second option we describe is DL_Track package installation via Github and pythons package manager pip. We want to inform you that there are more ways to install the package. However, we do not aim to be complete and rather demonstrate an (in our opinion) user friendly way for the installation of DL_Track. Moreover, we advise users with less programming experience to make use of the first option and download the executable file.
+We offer two possible installation approaches for our DL_Track_US software. The first option is to download the DL_Track_US executable file. The second option we describe is DL_Track package installation via Github and pythons package manager pip. We want to inform you that there are more ways to install the package. However, we do not aim to be complete and rather demonstrate an (in our opinion) user friendly way for the installation of DL_Track_US. Moreover, we advise users with less programming experience to make use of the first option and download the executable file.
 
 Download the DL\_Track\_US executable
 -------------------------------------
 
-1. Got to the Zenodo webpage containing the DL_Track executable, the pre-trained models and the example files using this `link <https://zenodo.org/record/7318089#.Y3S2qKSZOUk>`_.
+1. Got to the Zenodo webpage containing the DL_Track_US executable, the pre-trained models and the example files using this `link <https://zenodo.org/record/7866598#.ZEjuSMrP2Um>`_.
 2. Download the DL_Track_US_example.zip folder and unpack the file.
-3. Find the DL_Track_US.exe executable located in the DLTrack_example/executable folder.
-4. Open the DL_Track_US_GUI by double clicking the DL_Track.exe file and start with the testing procedure to check that everything works properly (see `Examples <https://dltrack.readthedocs.io/en/latest/usage.html>`_ and `Testing <https://dltrack.readthedocs.io/en/latest/tests.html>`_). In case you get an anti-virus notification, trust us and click it away. We assure you the software is harmless. 
+3. Find the DL_Track_US.exe executable located in the DL_Track_US_example/executable folder.
+4. Open the DL_Track_US_GUI by double clicking the DL_Track_US.exe file and start with the testing procedure to check that everything works properly (see `Examples <https://dltrack.readthedocs.io/en/latest/usage.html>`_ and `Testing <https://dltrack.readthedocs.io/en/latest/tests.html>`_). In case you get an anti-virus notification, trust us and click it away. We assure you the software is harmless. 
 
 Install DL_Track_US via Github, pip and Pypi.org
 ------------------------------------------------
 
-In case you want to use this way to install and run DL_Track, we advise you to setup conda (see step 1) and download the environment.yml file from the repo (see steps 5-8). If you want to actively contribute to the project or customize the code, it might be usefull to you to do all of the following steps (for more information see `Contributing Guidelines <https://dltrack.readthedocs.io/en/latest/contribute.html>`_).
+In case you want to use this way to install and run DL_Track_US, we advise you to setup conda (see step 1) and download the environment.yml file from the repo (see steps 5-8). If you want to actively contribute to the project or customize the code, it might be usefull to you to do all of the following steps (for more information see `Contributing Guidelines <https://dltrack.readthedocs.io/en/latest/contribute.html>`_).
 
 *Step 1.* Anaconda setup (only before first usage and if Anaconda/minicoda is not already installed).
 
 Install `Anaconda <https://www.anaconda.com/distribution/>`_ (click ‘Download’ and be sure to choose ‘Python 3.X Version’ (where the X represents the latest version being offered. IMPORTANT: Make sure you tick the ‘Add Anaconda to my PATH environment variable’ box).
 
-*Step 2.* **(Only required for MacOS users, contributing or development)** Git setup (only before first usage and if Git is not already installed). This is optional and only required when you want to clone the whole DL_Track Github repository.
+*Step 2.* **(Only required for MacOS users, contributing or development)** Git setup (only before first usage and if Git is not already installed). This is optional and only required when you want to clone the whole DL_Track_US Github repository.
 
 In case you have never used Git before on you computer, please install it using the instructions provided `here <https://git-scm.com/download>`_.
 
 *Step 3.* **(Only required for MacOS users, contributing or development)** Create a directory for DL_Track.
 
-On your computer create a specific directory for DL_Track (for example "DL_Track_US") and navigate there. You can use Git as a version control system. Once there open a git bash with right click and then "Git Bash Here". In the bash terminal, type the following:
+On your computer create a specific directory for DL_Track_US (for example "DL_Track_US") and navigate there. You can use Git as a version control system. Once there open a git bash with right click and then "Git Bash Here". In the bash terminal, type the following:
 
 ``git init``
 
 This will initialize a git repository and allows you to continue. If run into problems, check this `website <https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository>`_.
 
 *Step 4.* **(Only required for MacOS users, contributing or development)** Clone the DL_Track_US Github repository into a pre-specified folder (for example "DL_Track_US") by typing the following code in your bash window:
 
@@ -56,15 +56,15 @@
 
 *Step 7.* Install the DL_Track_US package.
 
 **Attention: The next part of Step 7 is NOT relevant for MacOS users:**
 
 You can directly install the DL_Track_US package from Pypi. To do so, type the following command in your bash terminal:
 
-``pip install DL-Track-US==0.1.2`` 
+``pip install DL-Track-US==0.1.2.1`` 
 
 All the package dependencies will be installed automatically. You can verify whether the environment was correctly created by typing the following command in your bash terminal:
 
 ``conda list``
 
 Now, all packages included in the DL_Track_US environment will be listed and you can check if all packages listed in the "DL_Track_US/environment.yml" file under the section "- pip" are included in the DL_Track environment.
 If you run into problems open a discussion in the Q&A section of `DL_Track_US discussions <https://github.com/PaulRitsche/DL_Track_US/discussions/categories/q-a>`_ and assign the label "Problem".
```

### Comparing `dl_track_us-0.1.2.1/docs/source/modules.rst` & `dl_track_us-0.1.2.2/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/docs/source/usage.rst` & `dl_track_us-0.1.2.2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/docs/usage/DL_Track_US_tutorial.pdf` & `dl_track_us-0.1.2.2/docs/usage/DL_Track_US_tutorial.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 10% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,1674 +1,2078 @@
 DL_Track_US
 v0.1.2
 
+26.04.2023
+
+DL_Track_US python package - Tutorial
+
+1
+
 Preface
 Welcome to the DL_Track_US python package tutorial. In the next roughly 80
 pages, you will learn how to automatically and manually analyse
 ultrasonography images and videos of human lower limb muscles. You will do
 so by making extensive use of the graphical user interface provided by the in
 the DL_Track_US package. Moreover, you will learn how to train your own
 neural networks using the graphical user interface as well. Have fun!
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 2
 
 Content
 1.
 2.
 3.
 4.
 5.
 6.
 7.
+8.
 
-Good to know… _________________________4
-Starting the graphical user interface_________5
-Automated Image Analysis________________8
-Manual Image Analysis__________________26
-Automated Video Analysis________________43
-Manual Video Analysis___________________60
-Training your own network_______________65
+Good to know__________________________4
+Starting the graphical user interface
+5
+Automated Image Analysis
+8
+Manual Image Analysis
+26
+Automated Video Analysis
+43
+Manual Video Analysis
+60
+Training your own network
+65
+Image Labels___________________________74
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 3
 
-Good To Know…
+Good to know
 All relevant instructions and guidelines for the installation of the DL_Track_US
 software package are described in our documentation, so please take a look
 there if anything is unclear. We have also provided information on what to do
 when you encounter problems during the installation process, encounter
 errors during the analysis process that are not caught by the GUI (no error
 message pop ups and advises you what to do), if you want to contribute to the
 DL_Track_US software package, and how you can reach us.
 Before we start with this tutorial, here are some important tips:
-• In case you plan an analysis on images taken from different muscles, we
-strongly advise to test the algorithm first and in case of bad performance,
-train your own models. We have provided extensive documentation on how
-to do so in the section “Training your own network” in this tutorial.
-• Although we used extensive data augmentation during the model training
-process, we must caution you about the generalizability of our models. Deep
-learning is no magic! Even though our model demonstrated good
-performance on unseen images during testing, we cannot confidently claim
-that they will work fine on all lower limb ultrasonography images. It is
-possible that even for images of muscles represented in our training data
-set, different device types, different muscle regions and even different
-settings of ultrasonography devices during image acquisition might offset
-model performance.
-• Quality matters! Please pay attention that the images you want to analyse
-with DL_Track_US are of high quality. High quality means good image
-contrast, appropriate image brightness, clearly visible fascicles and
-aponeurosis and clear alignment of the probe with the fascicle plain. If the
-quality of the images you want to analyse is bad, the results will be as well.
-• Bad model performance can be detected. The first and easiest step to take is
-to visually inspect the output of the models. If the segmentation results and
-the actual fascicles and aponeuroses overlap on most of the analysed
-images, model performance is good. If not, adapt the analysis parameters
-(how to do so is covered in the tutorials) or train a separate model. Secondly,
-you should manually analyse a few of your images and compare the model
-results to your manual results. If both results are similar, model performance
-is good. If not, adapt the analysis parameters (how to do so is covered in the
-tutorials) or train a separate model.
-• Lastly, we advise to follow the provided testing procedures in the
-DL_Track_US/tests folder. This ensures that the DL_Track_US package is
-working properly on you computer.
+• Test the algorithm first and train your own models if necessary, especially if
+you plan to analyze images taken from different muscles.
+• Be cautious about the generalizability of the models, even though
+extensive data augmentation was used during the model training process.
+Different device types, muscle regions, and settings during image
+acquisition may impact model performance.
+• Image quality is crucial. The images should have good contrast, appropriate
+brightness, clearly visible fascicles and aponeuroses, and clear alignment of
+the probe with the fascicle plane.
+• If model performance is poor, visually inspect the output of the models and
+compare them to manual analysis results. Adjust analysis parameters or
+train a separate model if necessary.
+• Follow the provided testing procedures in the DL_Track_US/tests folder to
+ensure proper functionality on your computer.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 4
 
-Starting the Graphical User Interface
-In the very first step of this tutorial, we will take a look at how to start the
-graphical user interface (GUI) once it was installed. We have provided two
-different installation procedures: 1. downloading the DL_Track_US_GUI.exe file
-and 2. installing the DL_Track_US python package using pip, Github and Pypi.
-Let’s begin with 1., how to start the GUI when you downloaded the
-DL_Track_US_GUI.exe:
-• It doesn’t get any easier than this. Navigate to the downloads folder and
-place the DL_Track_US_GUI.exe file somewhere you can easily find it again.
-Done so, you just have to double click the DL_Track_US_GUI.exe file with
-your left mouse button to start the GUI. Once you’ve done that, the GUI
-should open and you are ready to start an analysis.
-
-Double-click this icon
-to start the GUI.
+Starting the GUI
+For installation of DL_Track_US and starting the graphical user interface we
+refer you to the online documenation. In the installation chapter, all
+different possibilities for installing DL_Track_US and starting the GUI are
+described.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 5
 
-Now to 2., how to start the GUI when you installed the DL_Track_US python
-package via Pip, Github and Pypi:
-There are essentially two ways you can start the GUI. But first lets make sure
-that the package was correctly installed. The package should be automatically
-installed when you create the conda virtual environment. Therefore activate
-the environment by typing “conda activate DL_Track_US”:
-
-You should see the activated environment now in the left round brackets.
-Next type “conda list” to see all packages installed in the DL_Track_US
-environment:
-
-When you pressed enter, all packages installed in the environment should be
-listed. When DL_Track_US is included, you are good to go.
-
-In case the DL_Track_US package is not installed in your environment, please
-take a look at the installation guidelines again. If you still encounter a problem,
-ask a question in the Q&A discussion section of DL_Track_US on Github and
-add the Label “Problem”.
+Automated Image
+Analysis
+The first analysis type this tutorial covers is the automated image analysis. The
+images are evaluated without user input and may be scaled. Scaling the images
+will ensure estimated muscle architectural parameters are converted to
+centimetre units. For this type of analysis, single images (not videos) are a
+prerequisite. These images should be contained in a single folder, like in the
+“DL_Track_US_example/images” folder. If you haven’t downloaded this folder,
+please do so now (link: DL_Track_US - Examples & Models | Zenodo). Unzip the
+folder and put it somewhere accessible. We will make use of the included
+example files extensively during this tutorial. In the next few pages, we
+will look at every required step to successfully perform automated image
+analysis with DL_Track_US.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 6
 
-Alright, let’s actually start the GUI now once you’ve made sure that the
-DL_Track_US package is included in your active environment. As mentioned,
-you can do this in two ways. First option, you can run the DL_Track_US package
-from the command prompt. For this, type “python –m DL_Track_US” in the
-command prompt. When you press enter, the GUI should open.
-
-Neither to activate the environment (see previous page) nor to start the
-package do you need to be in a specific folder. The only prerequisite for this
-method is an active environment containing all dependencies for as well as the
-DL_Track_US package itself.
-Second option, you run the python file containing the main GUI manually.
-Therefore you need all the source files from the Github repository. Please take
-a look at the installation guidelines on how to get them. It is required that the
-environment containing all dependencies for as well as the DL_Track_US
-package itself is active (see previous page) and that you are in the folder
-containing the DL_Track_US_GUI.py module. To navigate to the folder type “cd
-yourpathtofile” in the command prompt. By pressing enter, the path is
-changed to the folder containing the DL_Track_US_GUI.py file.
+1.
 
-06.04.2023
+Creating Image Directory & FlipFlag.txt File
+
+•
+
+All images you want to analyze shoule be placed in one folder.
+
+•
+
+The “DL_Track_US/images“ folder contains 4 images and a flip_flag.txt file.
+It is not required to have the flip_flag.txt file in the same folder as the
+images to be analysed, but it is convenient.
+
+•
+
+Lets take a closer look at the flip_flags.txt file. Below you can see an the
+flip_flag.txt file in the directory.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 7
 
-To start the GUI, type “python DL_Track_US_GUI.py” in the command prompt
-once you have activated the environment containing the DL_Track_US package
-and all its dependencies and navigated to the folder that contains the
-DL_Track_US_GUI.py file. By pressing enter, the GUI should start.
-
-Congrats, you now know all the ways how to start the DL_Track_US GUI! Which
-way you use to start the GUI might be dependent on your usage intentions. If
-you just want to use the GUI and analyse images / videos, it is completely
-enough to download the DL_Track_US_GUI.exe and start right away. This is
-definitely the easiest way to start the GUI. However, if you want to customize
-the code and maybe even contribute to further releases, you are required to
-download all the source files in order to be able to change anything. To directly
-see your implemented changes use the last option explained below to start the
-GUI.
+•
+
+For every image there must be a flip-flag. If the number of flip-flags
+and images doesn’t match, an error is raised.
+
+•
+
+Another possible way to specify is displayed below. This is relevant when
+multiple subfolders are included, as each line then represents a subfolder.
+
+•
+
+The flip-flag determines if an image is flipped during analysis or not. A
+“0” stands for no flipping, whereas “1” means flip the image.
+
+•
+
+None of the example images must be flipped. Their fascicle orientation is
+correct, with fascicles originating at the bottom left and inserting on the
+top right.
+
+•
+
+Below is a visual representation of a correct fascicle orientation. If the
+fascicles in your images are orientated differently, please specify a “1” as
+a flip-flag for those images.
+
+Insertion
 
-06.04.2023
+Origin
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 8
 
-Automated Image
-Analysis
-The DL_Track_US python software package offers several different analysis
-types for analysis of human lower limb longitudinal ultrasonography images.
-The first analysis type this tutorial covers is the automated image analysis. The
-images are evaluated without user input and may be scaled. Scaling the images
-will ensure estimated muscle architectural parameters are converted to
-centimetre units. For this type of analysis, single images (not videos) are a
-prerequisite. These images should be contained in a single folder, like in the
-“DL_Track_US_example/images” folder. If you haven’t downloaded this folder,
-please do so now (link: DL_Track_US - Examples & Models | Zenodo). Unzip the
-folder and put it somewhere accessible, for example on your desktop. We will
-make use of the included example files extensively during this tutorial.
-Moreover, a FlipFlag.txt file is needed. Such a file is included in the
-“DL_Track_US_example/images” folder as well. In the next few pages, we will
-look at every required step to successfully perform automated image analysis
-with DL_Track_US.
+•
+
+For this tutorial we will use the example images folder
+“DL_Track_US_examples/images” with it’s contained images and
+flip_flag.txt file.
+
+2. Creating Neural Network Directories
+•
+
+The folder containing the images for this tutorial (in this case the
+“DL_Track_US_examples/images” folder) is already included in the
+“DL_Track_US_example” folder.
+
+•
+
+The pre-trained aponeurosis and fascicle neural networks are located in the
+“DL_Track_US_example/models” folder. You can make use of these neural
+networks later as well, when you analyse your own images outside of this
+tutorial.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 9
 
-1.
-
-Creating Image Directory & FlipFlag.txt File
+3. Specifying Input Directories in the GUI
+Once the GUI is openend, the first step of every analysis type in DL_Track_US
+is to specify the input directories in the graphical user interface (GUI).
+•
+
+First, specify the path to the folder containing the images to be analysed.
+Remember this was the folder “DL_Track_US_example/images”.
+o By clicking on the Input button a selection window opens were you
+need to select the images folder.
 
-In order for DL_Track_US to recognize your images, they should best be in a
-single folder (though one subfolder structure is acceptable as well). Take a look
-how you might structure this:
-
-You can see in the picture above that the folder contains 5 images, a flip_flag.txt
-file and is located on the desktop. This structure is already included in the
-“DL_Track_US_example” folder. It is not required to have the flip_flag.txt file in
-the same folder as the images to be analysed, but it is convenient.
-Lets take a closer look at the flip_flags.txt file and how this should look like in
-order for the analysis to work. Below you can see an the flip_flag.txt file in the
-directory.
+o Click select folder to specify the path in the GUI.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 10
 
-In the flip_flag.txt file you can see the respective flip-flag for each image. For
-every image there must be a flip-flag. If the number of flip-flags and images
-doesn’t match, an error is raised. Another possible way to specify is displayed
-below. This is relevant when multiple subfolders are included, as each line then
-represents a subfolder.
-
-The flip-flag determines if an image is flipped during analysis or not. A “0”
-stands for no flipping, whereas “1” means please flip the image. The flip-flags
-enable that each image can be automatically flipped or not. None of the
-example images must be flipped. Their fascicle orientation is correct, with
-fascicles originating at the bottom left and inserting on the top right. Here is a
-visual representation of a correct fascicle orientation. If the fascicles in your
-images are orientated differently, please specify a “1” as a flip-flag for those
-images.
+•
 
-Insertion
-
-Origin
+Secondly, specify the absolute path to the aponeurosis neural network
+in the “DL_Track_US_example/models”.
+o By clicking on the Apo Model button, a selection window opens were
+you need to select the aponeurosis neural network.
+o Click open to specify the path to the aponeurosis neural network in the
+GUI.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 11
 
-Once you have created a directory containing a flip_flag.txt file with a flip-flag
-for each image in the directory that containes “0” for images with correct
-orientation and “1” for incorrectly orientated images, we can get to the
-analysis part. (You actually do not need to anything at this point, because you
-can use the example images folder “DL_Track_US_examples/images” with it’s
-contained images and flip_flag.txt file.)
+•
 
-2. Creating Neural Network Directories
-Before we start with the analysis, we need to create a directory for the pretrained neural networks. The folder containing the images (in this case the
-“DL_Track_US_examples/images” folder) is already included in the
-“DL_Track_US_example” folder. We will now create a separate folder for the
-pre-trained aponeurosis and fascicle neural networks. In case you have not
-downloaded the models, please do so now (link: DL_Track_US - Examples &
-Models | Zenodo). Place them in a subfolder of the “DL_Track_US_example”
-folder for the moment, like “DL_Track_US_example/models”. You will make
-use of these neural networks later as well, when you analyse your own
-images outside of this tutorial. Of course you can move them to a different
-folder then. Your folder structure inside the “DL_Track_US_example” folder
-should now look something like this with the neural networks placed in the
-models folder.
+Thirdly, specify the absolute path to the fascicle neural network in
+the “DL_Track_US_example/models”.
+o By clicking on the Fasc Model button, a selection window opens were
+you need to select the fascicle neural network.
+o Click open to specify the path to the fascicle neural network in the GUI.
+
+In the next section you will specify all relevant analysis parameters,
+including the analysis type. We will also explain what each parameter is used
+for.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 12
 
-3. Specifying Input Directories in the GUI
-Finally you can start with the actual analysis! The first step of every analysis
-type in DL_Track_US is to specify the input directories in the graphical user
-interface (GUI). We assume that you have already opened the GUI. (If not, take
-a look at the previous chapter of this document “Starting the GUI”.).
-You will begin with specifying the path to the folder containing the images to
-be analysed. Remember this was the folder “DL_Track_US_example/images”.
-By clicking on the Input button in the GUI a selection window opens were you
-need to select the images folder. Click select folder to specify the path in the
-GUI.
+4. Specifying Relevant Parameters
+As a first step, you will select the right analysis type in the GUI.
+•
+
+S elect the Image radiobutton.
+
+•
+
+You can see that the GUI unfolds and several other parameters appear.
 
-06.04.2023
+•
+
+You will set those in the next steps on the next page.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 13
 
-Next, you will specify the absolute path to the aponeurosis neural network.
-Remember that you placed it in the “DL_Track_US_example/models”. By
-clicking on the Apo Model button in the GUI a selection window opens were
-you need to select the aponeurosis neural network in the models folder. Click
-open to specify the path to the aponeurosis neural network in the GUI.
+Next, you need to specify the Image Type.
+
+•
+
+The ending of the Image Type must match the ending of your images,
+otherwise no files are found by DL_Track_US.
+
+•
 
-06.04.2023
+You can either select a pre-specified ending from the dropdown list or
+type your own ending.
+
+•
+
+Please keep the formatting similar to those Image Types provided
+the dropdown list.
+
+•
+
+All
+the
+images
+in
+the “DL_Track_US_example/images” folder
+are of the Image Type “.tif”. Thus, you should select the “/*.tif” Image
+Type.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
+in
+
 14
 
-Next, you will specify the absolute path to the fascicle neural network.
-Remember that you placed it in the “DL_Track_US_example/models”. By
-clicking on the Fasc Model button in the GUI a selection window opens were
-you need to select the fascicle neural network in the models folder. Click open
-to specify the path to the fascicle neural network in the GUI.
-
-You have now successfully defined all the input directories required for
-automated image analyses with DL_Track_US. In the next section you will
-specify all relevant analysis parameters, including the analysis type. We will
-also explain what each parameter is used for.
+Subsequently, you need to specify the image Scaling Type.
+
+•
 
-06.04.2023
+Scaling in general has the huge advantage that the resulting estimated
+muscle architectural features are in centimetre units rather than pixel
+units.
+
+•
+
+There are three Scaling Types in the DL_Track_US package.
+
+•
+
+For this tutorial however, you will select the “No Scaling” option as
+displayed below.
+
+•
+
+We will explain the other two Scaling Types in the next pages.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 15
 
-4. Specifying Relevant Parameters
-As a first step, you will select the right analysis type in the GUI. Since this
-section is about automated image analysis, please select the Image
-radiobutton. You can see that the GUI unfolds and several other parameters
-appear. You will set those in the next steps on the next page.
+•
 
-06.04.2023
+Another Scaling Type except “No Scaling” is “Bar”. This Scaling Type is
+only applicable if there are scaling bars in the right side of the
+ultrasonography image:
+
+o The scaling bars do not need to look exactly like the ones in the
+above image. They just need to be next to the image and clearly
+separated from each other.
+o We advise you to try this Scaling type on a few of your images and find
+out for yourself if it works.
+o Files that cannot be analysed with this Scaling type will be recorded in
+an failed_images.txt file in the image input folder.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 16
 
-Next, you need to specify the Image Type. The ending of the Image Type must
-match the ending of your images, otherwise no files are found by DL_Track_US.
-You can either select a pre-specified ending from the dropdown list or type
-your own ending. Please keep the formatting similar to those Image Types
-provided in the dropdown list. All the images in the
-“DL_Track_US_example/images” folder are of the Image Type “.tif”. Thus, you
-should select the “/**/*.tif” Image Type.
+•
 
-06.04.2023
+The last of the three Scaling Types is “Manual”.
+o This Scaling Type requires input from the user.
+o When you choose “Manual” as your Scaling type, you need to
+manually place two points on the image using the left mouse button
+First point
+
+Second point
+
+o Just click one time with your left mouse button to record the first point
+(nothing will be displayed on the images during actual analysis).
+o Place the second point at a known distance of either 5, 10, 15 or 20
+millimetre.
+o The distance you chose must be represented in the Spacing (see next
+page) parameter in the GUI.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 17
 
-Subsequently, you need to specify the image Scaling Type. Scaling in general
-has the huge advantage that the resulting estimated muscle architectural
-features are in centimetre units rather than pixel units. There are three Scaling
-Types in the DL_Track_US package. For this tutorial however, you will select the
-“No Scaling” option as displayed below. We will explain the other two Scaling
-Types in the next pages.
+•
+
+Whenever you use “Bar” or “Manual” as your Scaling Type, make sure
+that the minimal distance between the scaling bars or the known
+distance between the manually specified points is represented in
+the Spacing parameter.
+
+•
+
+Select the Spacing parameter from the dropdown list as 5, 10, 15 or 20
+millimetre. For this tutorial it is not necessary to select anything, as the
+Spacing parameter is not used during an analysis with Scaling Type
+“No Scaling”.
+
+•
+
+The minimal distance between the scaling bars in an image. This is simply
+the distance in millimeter between the two nearest scaling bars in the
+image. If you do not know this distance, please use “Manual” or “No
+Scaling” Scaling Type. For example in the image from before, the
+distance between the nearest bars is 5 millimetre.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
 18
 
-Another Scaling Type except “No Scaling” is “Bar”. This Scaling Type is only
-applicable if there are scaling bars in the right side of the ultrasonography
-image:
-
-It is not important if the scaling bars look exactly like the ones in the above
-image. They just need to be next to the image and clearly separated from each
-other. We advise you to try this Scaling type on a few of your images and find
-out for yourself if it works. Files that cannot be analysed with this Scaling type
-will be recorded in an failed_images.txt file in the image input folder.
+•
 
-06.04.2023
+Next, specify the absolute path to the flip_flag.txt file.
+
+•
+
+By clicking the Flip Flags button, a dialogue will pop up and you can
+select the flip_flag.txt file.
+
+•
+
+In
+this
+example,
+the
+flip_flag.txt
+“DL_Track_US_example/images”.
+
+•
+
+Remember, the amount of flip-flags in the flip_flag.txt file must equal the
+amount of images in the images folder.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
+file
+
+is
+
+located
+
+at
+
 19
 
-The last of the three Scaling Types is “Manual”. This Scaling Type requires
-input from the user. When you choose “Manual” as your Scaling type, you
-need to manually place two points on the image using the left mouse button.
-First point
+5. Specifying Analysis Parameters
+As a last step, you need to specify the analysis parameters for the
+aponeurosis and fascicle neural networks.
+•
 
-Second point
+When you press the Analysis Parameters button, a separate window will
+pop-up.
 
-No worries, you do not actually need to draw on the image. Just click one time
-with your left mouse button to record the first point (nothing will be displayed
-on the images during actual analysis). Place the second point at a known
-distance of either 5, 10, 15 or 20 millimetre. The distance you chose must be
-represented in the Spacing (see next page) parameter in the GUI.
+o
 
-06.04.2023
+In the Analysis Parameter window, all parameters used by the aponeurosis and
+fascicles neural networks during inference are specified.
 
-DL_Track_US python package - Tutorial
+o
 
-20
+The Apo Threshold parameters determines the threshold of the minimal
+acceptable probability by which a pixel is predicted as aponeurosis. The lower,
+the more pixels will be classified as aponeurosis.
 
-Whenever you use “Bar” or “Manual” as your Scaling Type, please make sure
-that the minimum distance between the scaling bars or the known distance
-between you manually specified points is represented in the Spacing
-parameter. For the “No Scaling” Scaling type, this is not necessary.
-
-You can select the Spacing parameter only from the dropdown list as 5, 10, 15
-or 20 millimetre. For this tutorial it is not necessary to select anything, as the
-Spacing parameter is not used during an analysis with Scaling Type “No
-Scaling”.
-So far, we haven’t explained how to determine the minimal distance between
-the scaling bars in an image. This is simply the distance in millimeter between
-the two nearest scaling bars in the image. If you do not know this distance,
-please use “Manual” or “No Scaling” Scaling Type. For example in the image
-from before, the distance between the nearest bars is 5 millimetre. We know
-that because the distance between the bigger bars is always 10 millimetre.
+o
 
-06.04.2023
+The Fasc Threshold is the same thing just for fascicle segments.
 
-DL_Track_US python package - Tutorial
+o
 
-21
+The lower the Fasc Cont Threshold, the shorted the minimal acceptable length of
+detected fascicle segments to be included in the results.
 
-The next step in the image analysis using the DL_Track_US package is to specify
-the absolute path to the flip_flag.txt file. This is actually the same procedure
-than selecting the absolute to the aponeurosis and fascicle neural networks
-before. By clicking the Flip Flags button, a dialogue will pop up and you can
-select the flip_flag.txt file to retrieve it’s path. In this example, the flip_flag.txt
-file is located at “DL_Track_US_example/images”. Remember, the amount of
-flip-flags in the flip_flag.txt file must equal the amount of images in the images
-folder.
+o
 
-06.04.2023
+The Minimal Width determined the minimal acceptable distance between
+superficial and deep aponeurosis.
 
-DL_Track_US python package - Tutorial
+o
 
-22
+Minimal and Maximal Pennation describe the respective minimal and maximal
+pennation angle that is physiologically possible in the analysed image/muscle.
 
-5. Specifying Analysis Parameters
-Awesome, you have now successfully selected all relevant parameters in the
-main GUI window. As a LAST step, you need to specify the analysis parameters
-for the aponeurosis and fascicle neural networks. When you press the
-Analysis Parameters button, a separate window will pop-up.
-
-In the Analysis Parameter window, all parameters used by the aponeurosis
-and fascicles neural networks during inference are specified. We will give a
-short explanation to each of those parameters. The Apo Threshold parameters
-determines the threshold of the minimal acceptable probability by which a
-pixel is predicted as aponeurosis. The lower, the more pixels will be classified
-as aponeurosis. The Fasc Threshold is the same thing just for fascicle segments.
-The lower the Fasc Cont Threshold, the shorted the minimal acceptable length
-of detected fascicle segments to be included in the results. The Minimal Width
-determined the minimal acceptable distance between superficial and deep
-aponeurosis. Minimal and Maximal Pennation describe the respective minimal
-and maximal pennation angle that is physiologically possible in the analysed
-image/muscle.
-For this example, you can leave all parameters the way they are. You can set
-the parameters by clicking the Set parameters button, the Analysis Parameter
-window will then close automatically. Please make sure to adapt these
-parameters according to your images in analyses outside of this example. For
-future analyses, it’s best you test the ideal parameter configuration to get the
-best prediction results on your images in a small sample prior to the actual
-analysis.
+•
+
+For this tutorial, you can leave all parameters the way they are.
+
+•
+
+You can set the parameters by clicking the Set parameters button. Adapt
+these parameters according to your images in analyses.
+
+•
+
+For future analyses, it’s best you test the ideal parameter configuration in
+a small sample of your images prior to the actual analysis.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-23
+20
 
 6. Running / Breaking DL_Track_US
-Now its time to start the actual analysis of the example images in the
-“DL_Track_US_example/images” folder. You can do so by clicking the Run
-button in the main GUI window.
-
-When you started the GUI using the command prompt in any way, you will see
-that the analysis is started by the statements printed in the prompt. When you
-started the GUI using the executable, you will just have to believe us that the
-analysis is started.
-Moreover, you can see that there is a Break button placed in the GUI as well.
-Clicking the Break button allows you to stop the analysis at any point. The
-currently evaluated image will be processed and then the analysis is
-terminated.
-Take a look at the next page to see what happens when the analysis is finished.
+•
+
+•
+•
 
-06.04.2023
+By clicking the Run button in the main GUI window, you can start the
+analysis.
+
+Moreover, you can see that there is a Break button placed in the GUI as
+well.
+Clicking the Break button allows you to stop the analysis at any point.
+The currently evaluated image will be processed and then the
+analysis is terminated.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-24
+21
 
-Subsequently to clicking the Run button in the main GUI, navigate again to the
-“DL_Track_US_example/images” folder in your explorer. You will see that two
-files will be / have been created, ResultImages.pdf and Results.xlsx. The
-ResultImages.pdf file contains each original input image and concomitant
-prediction results with fascicles and aponeurosis displayed. This file allows you
-to visually inspect the model outputs. In your future analysis outside of this
-tutorial, you should always visually inspect the ResultImages.pdf file. The
-Results.xlsx file contains the actual architectural parameter estimates for each
-input image. There, the median value of all detected muscle fascicle length and
-pennation angles as well a the calculated muscle thickness will be displayed.
-Each input image is displayed in a separate row. Note that the
-ResultImages.pdf file can be opened only after the Results.xlsx was created.
-
-When both files can be opened and you can see the analysis results, original
-image and the prediction result, we must congratulate you! You have now
-officially and successfully completed the DL_Track_US tutorial for automated
-image analysis! There is one more thing though, error handling. Take a look at
-the next section to get more information.
+•
+
+In the “DL_Track_US_example/images” folder, you will see that two files
+will be / have been created, ResultImages.pdf and Results.xlsx.
+
+•
+
+The ResultImages.pdf file contains each original input image and
+concomitant prediction results with fascicles and aponeurosis displayed.
+
+•
 
-06.04.2023
+The Results.xlsx file contains the actual architectural parameter estimates
+for each input image. There, the median value of all detected muscle
+fascicle length and pennation angles as well a the calculated muscle
+thickness will be displayed. Each input image is displayed in a
+separate row.
+
+•
+
+Note that the ResultImages.pdf file can be opened only after the
+Results.xlsx was created.
+
+You have now completed the DL_Track_US tutorial for automated image
+analysis! There is one more thing though, error handling. Take a look at the
+next section to get more information.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-25
+22
 
-7. Error handling
+7. Error Handling
 Whenever an error occurs during the analysis process, the DL_Track_US GUI
 will open a messagebox. This looks always similar to this:
 
-We tried to formulate these messageboxes as concise as possible. Just follow
-their instructions to fix the error and run the analysis anew. In case an error
-occurs that is not caught by an error messagebox, don’t hesitate to report this
-in the Q&A section in the DL_Track_US discussion forum. Please take a look
-here how do best do this. Otherwise, you can contact us by email at
-paul.ritsche@unibas.ch, but we would prefer the other way.
+We tried to formulate these messageboxes as concise as possible. Just
+follow their instructions to fix the error and run the analysis anew. In case
+an error occurs that is not caught by an error messagebox, don’t hesitate to
+report this in the Q&A section in the DL_Track_US discussion forum. Please
+take a look here how do best do this.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-26
+23
 
-Manual Image
+M a n u a l Image
 Analysis
-The DL_Track_US python software package offers several different analysis
-types for analysis of human lower limb longitudinal ultrasonography images.
 The next analysis type this tutorial covers is the manual image analysis. The
 images are evaluated manually by drawing the muscle thickness, fascicle length
-and pennation angles directly on the Image. Scaling the images will ensure
-estimated muscle architectural parameters are converted to centimetre units.
-For this type of analysis, single images (not videos) are a prerequisite. These
-images should be contained in a single folder, like in the
+and pennation angles directly on the Image. For this type of analysis, single
+images (not videos) are a prerequisite. These images
+should
+be
+contained
+in
+a
+single
+folder,
+like
+in
+the
 “DL_Track_US_example/images_manual” folder. If you haven’t downloaded
 this folder, please do so now (link: DL_Track_US - Examples & Models |
-Zenodo). Unzip the folder and put it somewhere accessible, for example on
-your desktop. We will make use of the included example files extensively
-during this tutorial. In the next few pages, we will look at every required step
-to successfully perform automated image analysis with DL_Track_US.
+Zenodo). Unzip the folder and put it somewhere accessible. We will
+make use of the included example file included in the
+DL_Track_US_examples folder extensively during this tutorial. In the next few
+pages, we will look at every required step to successfully perform manual
+image analysis with DL_Track_US.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-27
+24
 
 1.
+•
 
 Creating Image Directory
 
-In order for DL_Track_US to recognize your images, they should best be in a
-single folder (though one subfolder structure is acceptable as well). Take a look
-how you might structure this:
-
-You can see in the picture above that the folder contains 2 images and is located
-on the desktop. This structure is already included in the
-“DL_Track_US_example” folder. In contrast to automated image analysis, you do
-not need a flip_flag.txt file nor do you need neural networks that do predictions.
-Here, you are the neural network. So, the next step is to specify the input
-directory in the GUI.
+All images to be analyzed should be in a single folder.
+
+•
+
+The “DL_Track_US/image_manual“ folder contains 2 images.
 
-06.04.2023
+•
+
+In contrast to automated image analysis, you do not need a flip_flag.txt file
+nor do you need neural networks that do predictions.
+
+•
+
+In manual image analysis, you are the neural network.
+
+•
+
+The next step is to specify the input directory in the GUI.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-28
+25
 
 2. Specifying Input Directories in the GUI
-You can start with the actual analysis! The first step of every analysis type in
-DL_Track_US is to specify the input directories in the graphical user interface
-(GUI). We assume that you have already opened the GUI. (If not, take a look at
-the first chapter of this document “Starting the GUI”.).
-You will begin with specifying the path to the folder containing the images to
-be
-analysed.
-Remember
-this
-is
-the
-folder
-“DL_Track_US_example/images_manual”. By clicking on the Input button in
-the GUI a selection window opens were you need to select the images folder.
+•
+
+•
+•
+
+•
+
+You will begin with specifying the path to the folder containing the
+images to be analysed, the “DL_Track_US_example/images_manual”
+folder.
+By clicking on the Input button in the GUI a selection window opens
+were you need to select the images folder.
 Click select folder to specify the path in the GUI.
 
-Once that is done, the path will be displayed in the entry filed and you can
-start to specify the relevant parameters for the analysis.
-06.04.2023
+Once that is done, the path will be displayed in the entry filed and you
+can start to specify the relevant parameters for the analysis.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-29
+26
 
 3. Specifying Relevant Parameters
-As a first step, you will select the right analysis type in the GUI. Since this
-section is about manual image analysis, please select the Image Manual
-radiobutton. You can see that the GUI unfolds and another parameter appear.
+•
+
+Please select the Image Manual radiobutton.
+
+•
+
+You can see that the GUI unfolds and another parameter appear.
+
+•
+
 You will set this one in the next step on the next page.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-30
+27
 
-Next, you need to specify the Image Type. The ending of the Image Type must
-match the ending of your images, otherwise no files are found by DL_Track_US.
-You can either select a pre-specified ending from the dropdown list or type
-your own ending. Please keep the formatting similar to those Image Types
-provided in the dropdown list. All the images in the
-“DL_Track_US_example/images_manual” folder are of the Image Type “.tif”.
-Thus, you should select the “/**/*.tif” Image Type.
+Next, you need to specify the Image Type.
 
-Allright, once you have specified the Image Type, you can start with the
-analysis
-of
-the
-images
-contained
-I
-the
-“DL_Track_US_example/images_manual” folder.
+•
+
+The ending of the Image Type must match the ending of your images,
+otherwise no files are found by DL_Track_US.
+
+•
+
+You can either select a pre-specified ending from the dropdown list or
+type your own ending.
+
+•
+
+Please keep the formatting similar to those Image Types provided n
+the dropdown list.
+
+•
+
+All the images in the “DL_Track_US_example/images_manual” folder
+are of the Image Type “.tif”.
 
-06.04.2023
+•
+
+Thus, you should select the “/*.tif” Image Type.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-31
+28
+
+•
 
-Allright, once you have specified the Image Type, you can start with the
+Once you have specified the Image Type, you can start with the
 analysis
 of
 the
 images
 contained
-I
+in
 the
-“DL_Track_US_example/images_manual” folder. You can start the analysis by
-clicking the Run button in the main GUI.
+“DL_Track_US_example/images_manual” folder.
+
+•
+
+You can start the analysis by clicking the Run button in the main GUI.
+
+•
 
-Take a look at the next page to see how to continue in the “Manual Analysis
-window” that pops up.
+Take a look at the next page to see how to continue in the “Manual
+Analysis window” that pops up.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-32
+29
 
 4. Manual Analysis of Images
 Subsequent to clicking the Run button in the main GUI, the “Manual Analysis
-window” opens. Here you can analysis the image by marking the respective
-architectural parameter you want to analyse directly on the image. We will
-guide you through that on the next pages. But first of all, here is how the
-“Manual Analysis window” looks like:
-
-It is of utmost importance to keep in mind that the lines you are about to draw
-on the image are only there to help you remember what it did. The actual lines
-are not used during the computation of the architectural parameters. The
-start- and endpoints of each line are relevant. The start point is defined as the
-point where you clicked the left mouse button to start drawing the line. The
-endpoint is defined as the point where you released the left mouse button to
-stop drawing the line. The line follows the cursor as long as the left mouse
-button is pressed. The calculations of the scaling line length, muscle thickness,
-fascicle length and pennation angle are dependent on the number of specified
-lines/segments. Do NOT click somewhere random on the image during the
-analysis of a parameter and exactly follow the instructions. If additional clicks
-happened, start the analysis anew by selecting the radiobutton representing
-the parameter again. If you do not follow the instructions presented in this
-tutorial, we cannot guarantee the correctness of the analysis results.
+window” opens. H ere is how it looks like:
 
-06.04.2023
+Important to note:
+• The actual lines you draw are not used during the computation of the
+architectural parameters.
+• The start- and endpoints of each line are relevant.
+• The start point is defined as the point where you clicked the left mouse
+button to start drawing the line.
+• The endpoint is defined as the point where you released the left mouse
+button to stop drawing the line.
+• The line follows the cursor as long as the left mouse button is pressed.
+• The calculations of the scaling line length, muscle thickness, fascicle length
+and pennation angle are dependent on the number of specified
+lines/segments.
+• Do NOT click somewhere random on the image during the analysis of
+a parameter and exactly follow the instructions. If additional clicks
+happened, start the analysis anew by selecting the radiobutton
+representing the parameter again.
+• If you do not follow the instructions presented in this tutorial, we
+cannot guarantee the correctness of the analysis results.
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-33
+30
 
 First of all, you will scale the images manually so that the calculated
-architectural parameters are returned in centimetre rather than pixel units. For
-the scaling, please draw a one centimetre long straight line in the image. The
-distance of one centimetre is usually recognizable in the scaling bars in the
-image. You can initiate the scaling process by selecting the Scale Image
-radiobutton in the “Manual Analysis window”. A messagebox will appear
-advising you what to do. The drawn line should look like this.
+architectural parameters are returned in centimetre rather than pixel units.
+• Draw a one centimetre long straight line in the image.
+•
+
+The distance of one centimetre is usually recognizable in the scaling
+bars in the image.
+You can initiate the scaling process by selecting the Scale Image
+radiobutton in the “Manual Analysis window”.
+A messagebox will appear advising you what to do.
 
-06.04.2023
+•
+•
+
+•
+
+The drawn line should look like this.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-34
+31
 
 As a next step you have the option to extend the muscle aponeuroses to ease
-the extrapolation of fascicles extending outside of the image. This however not
-required, merely an option. You can do by selecting the Draw Aponeurosis
-button in the “Manual Analysis window” and draw the aponeurosis lines on
-the image as shown below. A messagebox will appear advising you what to do.
+the extrapolation of fascicles extending outside of the image.
 
-06.04.2023
+•
+
+Select the Draw Aponeurosis button in the “Manual Analysis window”
+and draw the aponeurosis lines on the image as shown below.
+
+•
+
+A messagebox will appear advising you what to do.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-35
+32
 
-Once the image is scaled and aponeuroses structures extended, you can start
-analysing the muscle architectural parameters. You will start with the muscle
-thickness. Therefore, select the Muscle Thickness radiobutton in the “Manual
-Analysis window”. A messagebox will appear advising you what to do. We
-advise to you to now draw three straight lines reaching from the superficial to
-the deep aponeurosis in the middle, right and left portion of the muscle image.
+Now you can start with the muscle thickness assessment.
+• Select the Muscle Thickness radiobutton in the “Manual Analysis
+window”.
+• A messagebox will appear advising you what to do.
+• Draw three straight lines reaching from the superficial to the deep
+aponeurosis in the middle right and left portion of the muscle image.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-36
+33
+
+Next you can mark single fascicles on the image.
+•
+
+Select the Muscle Fascicles radiobutton in the “Manual Analysis
+window”.
+
+•
+
+A messagebox will appear advising you what to do.
+
+•
+
+Draw at least three fascicles per image in different regions of the image.
+
+•
+
+It is possible to extrapolate the fascicles outside of the image region.
+
+•
+
+Each fascicle MUST consist of three segments.
+
+•
+
+Do not draw more or less segments per fascicle and pay attention to avoid
+any extra unwanted mouse clicks.
+
+•
 
-Next you can mark single fascicles on the image by selecting the Muscle
-Fascicles radiobutton in the “Manual Analysis window”. A messagebox will
-appear advising you what to do. We advise to draw at least three fascicles per
-image in different regions of the image. Please consider that these fascicles
-must be clearly visible and not guessed. It is possible to extrapolate the
-fascicles outside of the image region. Each fascicle MUST consist of three
-segments. Do not draw more or less segments per fascicle and pay attention to
-avoid any extra unwanted mouse clicks. One segment MUST start where the
-previous segment ended. Take a look at the image sequence below to see how
-it is done:
+One segment MUST start where the previous segment ended.
+
+•
+
+Take a look at the image sequence below to see how it is done:
 
 1st Fascicle
 segment
 
-2nd Fascicle
+3rd Fascicle
 segment
-All three
-Fascicles
 
-3rd Fascicle
+26.04.2023
+
+2nd Fascicle
 segment
-06.04.2023
+
+All three Fascicles
 
 DL_Track_US python package - Tutorial
 
-37
+34
 
-The last architectural parameter that you can manually analyse using the
-DL_Track_US package is the muscle pennation angle. Please select the
-radiobutton Pennation Angle. A messagebox will appear advising you what to
-do. We advise you to draw at least three pennation angles per image at
-different regions of the image. As with the fascicles, these should be clearly
-visible. Each drawn pennation angle MUST consist of two segments. The first
-segment should follow the orientation of the fascicle, the second segment
-should follow the orientation of the deep aponeurosis. The segments should
-both originate at the insertion of the fascicle in the deep aponeurosis. Please
-pay attention to avoid unwanted clicks on the image. Here is how its done:
+Next you can manually analyse the pennation angle.
+• Select the radiobutton Pennation Angle.
+• A messagebox will appear advising you what to do.
+• Draw at least three pennation angles per image at different regions of
+the image.
+•
+
+•
+
+Each drawn pennation angle MUST consist of two segments. The first
+segment should follow the orientation of the fascicle, the second
+segment should follow the orientation of the deep aponeurosis. The
+segments should both originate at the insertion of the fascicle in the
+deep aponeurosis.
+Please pay attention to avoid unwanted clicks on the image.
 
 2nd Pennation angle
 segment
 
 1st Pennation angle
 segment
 
 All pennation angles
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-38
+35
 
 5. Saving / Breaking / Next Image
-Great, you have now successfully analysed all muscle architectural parameters
-using the DL_Track_US manual image analysis tool. However, there are three
-buttons in the “Manual Analysis window” left to explain. The first button is the
-Save Results button. The Save Results button is a very important button!
-Before you have pressed this button, none of your analysis results are saved.
-Therefore, please press the Save Results button once you have analyzed all
-parameters that you wanted to analyze and before continuing with the next
-image. An excel file with the name Manual_Results.xlsx is saved in the
-directory of the input images upon pressing the Save Results button. Therein,
-all analysis results are stored. In your case the file is saved in the
+There are three buttons in the “Manual Analysis window” left to explain.
+•
+
+The first button is the Save Results button.
+o The Save Results button is a very important button!
+o Press the Save Results button once you have analyzed all parameters
+that you wanted to analyze and before continuing with the next
+image.
+o An excel file with the name Manual_Results.xlsx is saved in the
+directory of the input images upon pressing the Save Results button.
+Therein, all analysis results are stored. Moreover, by pressing the
+Save Results, a screenshot of your current analysis is captured and
+stored. (Note: The image may look strange, as we can only approximate
+the coordinates and size of the manual analysis on your screen.)
+o In
+your
+case
+all
+files
+are
 “DL_Track_US_example/images_manual” folder.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-39
+saved
+
+in
+
+the
+
+36
 
-The second button we haven’t explained yet is the Next Image button. By
-clicking this button, you can proceed to the next image in the input folder (in
-your case the “DL_Track_US_example/images_manual” folder). Please
-remember to press the Save Results button prior to proceeding to the next
-images, otherwise you analysis results for this image will be lost. When the
-Next Image button is pressed, the displayed image is updated.
+•
 
-06.04.2023
+The second button we haven’t explained yet is the Next Image
+button.
+o By clicking this button, you can proceed to the next image in the input
+folder (in your case the “DL_Track_US_example/images_manual”
+folder).
+o Please remember to press the Save Results button prior to
+proceeding to the next images, otherwise you analysis results for this
+image will be lost.
+o When the Next Image button is pressed, the displayed image is
+updated.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-40
+37
 
-The last button we need to explain is the Break Analysis button. Pressing this
-button allows you to terminate the analysis and return to the main GUI
-window. A messagebox will appear asking you if you really want to stop the
-analysis. Once the Break Analysis button is pressed and you answered the
-messagebox with “YES”, the “Manual Analysis window” will be automatically
-closed. Remember to save your analysis results before doing so. We think you
-know which very important button can do just that!
+•
+
+The last button we need to explain is the Break Analysis button.
+o Pressing this button allows you to terminate the analysis and
+return to the main GUI window.
+o A messagebox will appear asking you if you really want to stop the
+analysis.
+o Once the Break Analysis button is pressed and you answered the
+messagebox with “YES”, the “Manual Analysis window” will be
+automatically closed.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-41
+38
 
 When you have saved your results clicking the very important button and
 followed our instructions during this tutorial, your input directory
-“DL_Track_US_example/images_manual” should look like this. It should
-contain the images as well as the Manual_Results.xlsx file.
-
-Congrats are in order! You have now officially and successfully completed the
-DL_Track_US tutorial for manual image analysis! There is one more thing
-though, error handling. Take a look at the next section to get more information.
+“DL_Track_US_example/images_manual” should look like this. It should contain
+the images, saved screenshots, as well as the Manual_Results.xlsx file.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-42
+39
 
-6. Error handling
+6. Error Handling
 Whenever an error occurs during the manual image analysis process, the
 DL_Track_US GUI will open a messagebox. This looks always similar to this:
 
 We tried to formulate these messageboxes as concise as possible. Just follow
 their instructions to fix the error and run the analysis anew. In case an error
 occurs that is not caught by an error messagebox, don’t hesitate to report this
 in the Q&A section in the DL_Track_US discussion forum. Please take a look
-here how do best do this. Otherwise, you can contact us by email at
-paul.ritsche@unibas.ch, but we would prefer the other way.
+here how do best do this.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-43
+40
 
 Automated Video
 Analysis
-The DL_Track_US python software package offers several different analysis
-types for analysis of human lower limb longitudinal ultrasonography images.
-This section of the tutorial covers the automated video analysis. The videos are
-evaluated without user input and may be scaled. Scaling the images will ensure
-estimated muscle architectural parameters are converted to centimetre units.
-For this type of analysis, videos are a prerequisite. These videos should be
-contained in a single folder, like in the “DL_Track_US_example/videos” folder. If
-you haven’t downloaded this folder, please do so now (link: DL_Track_US Examples & Models | Zenodo). Unzip the folder and put it somewhere
-accessible, for example on your desktop. We will make use of the included
-example files extensively during this tutorial. The automated video analysis is
-very similar to the automated image analysis. In fact, the inputted video is
-analysed frame by frame and each frame is therefore treated like an
-independent image. Moreover, only few analysis parameters are different
-between both analysis types. In the next few pages, we will look at every
-required step to successfully perform automated video analysis with
-DL_Track_US.
+This section of the tutorial covers the automated video analysis. The videos
+are evaluated without user input and may be scaled. The videos should be
+contained in a single folder, like in the “DL_Track_US_example/videos” folder.
+If you haven’t downloaded this folder, please do so now (link:
+DL_Track_US - Examples & Models | Zenodo). Unzip the folder and
+put it somewhere accessible. We will make use of the included example
+files extensively during this tutorial. The automated video analysis is very
+similar to the automated image analysis. In fact, the inputted video is
+analysed frame by frame and each frame is therefore treated like
+an independent image. Moreover, only few analysis parameters are
+different between both analysis types. Once the analysis of the video file is
+finished, a „proc.avi“ file will be created at the directoy of the input video.
+The „proc.avi“ file can be openend with, i.e., VLC-Player on windows and
+Omni-Player on macOS. In the next few pages, we will look at every
+required step to successfully perform automated video analysis
+with DL_Track_US.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-44
+41
 
-1.
+•
+
+1.
 
 Creating Video and Network Directories
 
-In order for DL_Track_US to recognize your videos, they should best be in a
-single folder (though one subfolder structure is acceptable as well). Take a look
-how you might structure this:
-
-You can see in the picture above that the folder contains one video and is
-located on the desktop. This structure is already included in the
-“DL_Track_US_example” folder. We will continue with demonstrating how to
-create folders for the aponeurosis and fascicle neural networks on the next
-page.
+•
+
+In order for DL_Track_US to recognize your videos, they should best be
+in a single folder.
 
-06.04.2023
+The “DL_Track_US_example/videos“ folder contains one video.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-45
+42
+
+•
+
+The folder containing the video is the “DL_Track_US_example/video”
+folder.
+
+•
+
+The pre-trained aponeurosis and fascicle neural networks are located in
+the “DL_Track_US_example/models” folder.
 
-The folder containing the video (in this case the
-“DL_Track_US_example/video” folder) is already included in the
-“DL_Track_US_example” folder. We will now create a separate folder for the
-pre-trained aponeurosis and fascicle neural networks. In case you have not
-downloaded the models, please do so now (link: ). Place them in a subfolder
-of the “DL_Track_US_example” folder for the moment, like
-“DL_Track_US_example/models”. You will make use of these neural networks
-later as well, when you analyse your own images outside of this tutorial. Of
-course you can move them to a different folder then. Your folder structure
-inside the “DL_Track_US_example” folder should now look something like this
-with the neural networks placed in the models folder.
+•
 
-06.04.2023
+You can make use of these neural networks later as well, when you
+analyse your own videos outside of this tutorial.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-46
+43
 
 2. Specifying Input Directories in the GUI
-Finally you can start with the actual analysis! The first step of every analysis
-type in DL_Track_US is to specify the input directories in the graphical user
-interface (GUI). We assume that you have already opened the GUI. (If not, take
-a look at the first chapter of this document “Starting the GUI”.).
-You will begin with specifying the path to the folder containing the video to be
-analysed. Remember this was the folder “DL_Track_US_example/video”. By
-clicking on the Input button in the GUI a selection window opens were you
-need to select the images folder. Click select folder to specify the path in the
-GUI.
+Once the GUI is openend, the first step of every analysis type in DL_Track_US
+is to specify the input directories in the graphical user interface (GUI).
+•
+
+Start the analysis with specifying the path to the folder containing the
+video to be analysed.
+o Remember this was the folder “DL_Track_US_example/video”. By
+clicking on the Input button in the GUI a selection window opens
+were you need to select the images folder.
+o Click select folder to specify the path in the GUI.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-47
+44
+
+•
 
-Now, you will specify the absolute path to the aponeurosis neural network.
-Remember that you placed it in the “DL_Track_US_example/models”. By
-clicking on the Apo Model button in the GUI a selection window opens were
-you need to select the aponeurosis neural network in the models folder. Click
-open to specify the path to the aponeurosis neural network in the GUI.
+Now, you will specify the absolute path to the aponeurosis neural
+network.
+• Remember that the model is in the “DL_Track_US_example/models”
+folder.
+• By clicking on the Apo Model button in the GUI a selection window
+opens were you need to select the aponeurosis neural network in the
+models folder.
+• Click open to specify the path to the aponeurosis neural network in the
+GUI.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-48
+45
 
-Next, you will specify the absolute path to the fascicle neural network.
-Remember that you placed it in the “DL_Track_US_example/models”. By
-clicking on the Fasc Model button in the GUI a selection window opens were
-you need to select the fascicle neural network in the models folder. Click open
-to specify the path to the fascicle neural network in the GUI.
-
-You have now successfully defined all the input directories required for
-automated image analyses with DL_Track_US. In the next section you will
-specify all relevant analysis parameters, including the analysis type. We will
-also explain what each parameter is used for.
+•
 
-06.04.2023
+Next, you will specify the absolute path to the fascicle neural
+network.
+o The model is in the “DL_Track_US_example/models” folder.
+o By clicking on the Fasc Model button in the GUI a selection window
+opens were you need to select the fascicle neural network in the
+models folder.
+o Click open to specify the path to the fascicle neural network in the GUI.
+
+In the next section you will specify all relevant analysis parameters,
+including the analysis type. We will also explain what each parameter is used
+for.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-49
+46
 
 3. Specifying Relevant Parameters
-As a first step, you will select the right analysis type in the GUI. Since this
-section is about automated video analysis, please select the Video
-radiobutton. You can see that the GUI unfolds and several other parameters
-appear. You will set those in the next steps on the next page.
+As a first step, you will select the right analysis type in the GUI.
+•
+
+Please select the Video radiobutton.
 
-06.04.2023
+•
+
+You can see that the GUI unfolds and several other parameters appear.
+
+•
+
+You will set those in the next steps on the next page.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-50
+47
+
+You now need to specify the Video Type.
+
+•
+
+The ending of the Video Type must match the ending of your videos,
+otherwise no files are found by DL_Track_US.
+
+•
 
-You now need to specify the Video Type. The ending of the Video Type must
-match the ending of your videos, otherwise no files are found by DL_Track_US.
-You can either select a pre-specified ending from the dropdown list or type
-your own ending. Please keep the formatting similar to those Video Type
-provided in the dropdown list. The video in the “DL_Track_US_example/video”
-folder are of the Video Type “.mp4”. Thus, you should select the “/**/*.mp4”
-Video Type.
+You can either select a pre-specified ending from the dropdown list or
+type your own ending.
 
-06.04.2023
+•
+
+Please keep the formatting similar to those Video Type provided in the
+dropdown list.
+
+•
+
+The video in the “DL_Track_US_example/video” folder are of the Video
+Type “.mp4”. Thus, you should select the “/*.mp4” Video Type.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-51
+48
+
+Subsequently, you need to specify the video Scaling Type.
+
+•
+
+Scaling in general has the advantage that the resulting estimated
+muscle architectural features are in centimetre units rather than pixel
+units.
+
+•
 
-Subsequently, you need to specify the video Scaling Type. Scaling in general
-has the huge advantage that the resulting estimated muscle architectural
-features are in centimetre units rather than pixel units. There are two Scaling
-Types in the DL_Track_US package. For this tutorial however, you will select the
-“No Scaling” option as displayed below. We will explain the other Scaling Type
-on the next.
+There are two Scaling Types in the DL_Track_US package.
 
-06.04.2023
+•
+
+For this tutorial however, you will select the “No Scaling” option as
+displayed below. We will explain the other Scaling Type on the next.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-52
+49
 
-The other Scaling Types is “Manual”. This Scaling Type requires input from the
-user. When you choose “Manual” as your Scaling type, you need to manually
-place two points on the first video frame using the left mouse button. This step
-is similar to the “Manual” scaling option for automated and manual image
-analysis.
+•
+
+The other Scaling Types is “Manual”.
+o This Scaling Type requires input from the user.
+o When you choose “Manual” as your Scaling type, you need to
+manually place two points on the first video frame using the left mouse
+button.
+o This step is similar to the “Manual” scaling option for automated
+and manual image analysis.
 First point
 
 Second point
 
-No worries, you do not actually need to draw on the video frame. Just click one
-time with your left mouse button to record the first point (nothing will be
-displayed on the video frames during actual analysis). Place the second point
-at a known distance of either 5, 10, 15 or 20 millimetre. The distance you chose
-must be represented in the Scaling (see next page) parameter in the GUI.
+o Just click one time with your left mouse button to record the first
+point (nothing will be displayed on the video frames during actual
+analysis).
+o Place the second point at a known distance of either 5, 10, 15 or 20
+millimetre.
+o The distance you chose must be represented in the Scaling (see next
+page) parameter in the GUI.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-53
+50
 
-Whenever you use “Manual” as your Scaling Type, please make sure that the
-minimum distance between the scaling bars or the known distance between
-your manually specified points is represented in the Spacing parameter. For the
-“No Scaling” Scaling type, this is not necessary.
-
-You can select the Spacing parameter only from the dropdown list as 5, 10, 15
-or 20 millimetre. For this tutorial it is not necessary to select anything, as the
-Spacing parameter is not used during an analysis with Scaling Type “No
-Scaling”.
-So far, we haven’t explained how to determine the minimal distance between
-the scaling bars in a video frame. This is simply the distance in millimeter
-between the two nearest scaling bars in the frame. If you do not know this
-distance, please use “Manual” or “No Scaling” Scaling Type. For example in
-the frame from before, the distance between the nearest bars is 5 millimetre.
-We know that because the distance between the bigger bars is always 10
-millimetre.
+•
+
+Whenever you use “Manual” as your Scaling Type, please make sure that
+the minimum distance between the scaling bars or the known distance
+between your manually specified points is represented in the Spacing
+parameter.
+
+•
+
+You can select the Spacing parameter only from the dropdown list as 5,
+10, 15 or 20 millimetre. For this tutorial it is not necessary to select
+anything, as the Spacing parameter is not used during an analysis
+with Scaling Type “No Scaling”.
+
+•
+
+The minimal distance is simply the distance in millimeter between the
+two nearest scaling bars in the frame. If you do not know this distance,
+please use “Manual” or “No Scaling” Scaling Type. For example in the
+frame from before, the distance between the nearest bars is 5 millimetre.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-54
+51
 
-Another parameter that you need to specify is the Flip Options parameters. The
-Flip Options parameter determines if the whole video is flipped along the
-vertical axis. “Flip” stands for flipping the video, whereas “Don’t Flip” means
-please do not flip the video. The example video must be flipped. Its fascicle
-orientation is incorrect, with fascicles originating at the bottom right and
-inserting on the top left. This would confuse our models. Below is a visual
-representation of a correct fascicle orientation. The fascicles are originating at
-the bottom left and are inserting on the top right. If the fascicles in your video
-outside of this tutorial are orientated differently, please specify “Flip” in the Flip
-Options parameter for those videos. Note that all videos in the specified input
-folder, in this case the DL_Track_US_example/video” folder, MUST have the
-same fascicle orientation, since the Flip Option is applied to all of them. It does
-however not matter if this is the correct or incorrect fascicle orientation.
+Another parameter that you need to specify is the Flip Options parameters.
+• The Flip Options parameter determines if the whole video is flipped
+along the vertical axis. “Flip” stands for flipping the video, whereas
+“Don’t Flip” means please do not flip the video.
+• The example video must be flipped.
+•
+•
+•
+•
+
+Its fascicle orientation is incorrect, with fascicles originating at the
+bottom right and inserting on the top left.
+Below is a visual representation of a correct fascicle orientation.
+The fascicles are originating at the bottom left and are inserting on the top
+right.
+Note that all videos in the specified input folder, in this case the
+DL_Track_US_example/video” folder, MUST have the same fascicle
+orientation, since the Flip Option is applied to all of them.
 
 Insertion
 
 Origin
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-55
+52
 
-The next step in the automated video analysis using the DL_Track_US package
-is to specify the Frame Steps. You can either select a pre-specified Frame Step
-from the dropdown list or type your Frame Step. The Frame Step is used
-during the analysis as a step size while iterating through all the frames in a
-video. In this tutorial you should specify a Frame Step of 1. This means that
-every video frame is analysed. With a Frame Step of 3, every 3rd frame is
-analysed. With a Frame Step of 10, every 10th frame an so on. Although
-information is lost when you skip frames during the analysis, it also reduces
-the overall analysis time. IMPORTANT: when you skip frames in videos outside
-of this tutorial, the frame rate with which the video was acquired should be
-high a enough and the captured motion a slow one. Otherwise, too much
-relevant information is lost.
+The next step is to specify the Frame Steps.
+• You can either select a pre-specified Frame Step from the dropdown list
+or type your Frame Step.
+• The Frame Step is used during the analysis as a step size while iterating
+through all the frames in a video.
+• In this tutorial you should specify a Frame Step of 1. This means that
+every video frame is analysed. With a Frame Step of 3, every 3rd
+frame is analysed. With a Frame Step of 10, every 10th frame an so
+on.
+• Although information is lost when you skip frames during the analysis, it
+also reduces the overall analysis time.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-56
+53
 
 4. Specifying Analysis Parameters
-Awesome, you have now successfully selected all relevant parameters in the
-main GUI window. As a LAST step, you need to specify the analysis parameters
-for the aponeurosis and fascicle neural networks. When you press the
-Analysis Parameters button, a separate window will pop-up.
-
-In the Analysis Parameter window, all parameters used by the aponeurosis
-and fascicles neural networks during inference are specified. We will give a
-short explanation to each of those parameters. The Apo Threshold parameters
-determines the threshold of the minimal acceptable probability by which a
-pixel is predicted as aponeurosis. The lower, the more pixels will be classified
-as aponeurosis. The Fasc Threshold is the same thing just for fascicle segments.
-The lower the Fasc Cont Threshold, the shorted the minimal acceptable length
-of detected fascicle segments to be included in the results. The Minimal Width
-determined the minimal acceptable distance between superficial and deep
-aponeurosis. Minimal and Maximal Pennation describe the respective minimal
-and maximal pennation angle that is physiologically possible in the analysed
-video frame/muscle.
-For this example, you can leave all parameters the way they are. You can set
-the parameters by clicking the Set parameters button, the Analysis Parameter
-window will then close automatically. Please make sure to adapt these
-parameters according to your images in analyses outside of this example. For
-future analyses, it’s best you test the ideal parameter configuration to get the
-best prediction results on your images in a small sample prior to the actual
+As a last step, you need to specify the analysis parameters for the
+aponeurosis and fascicle neural networks.
+•
+
+When you press the Analysis Parameters button, a separate window will
+pop-up.
+
+o
+
+The Apo Threshold parameters determines the threshold of the minimal
+acceptable probability by which a pixel is predicted as aponeurosis. The lower,
+the more pixels will be classified as aponeurosis.
+
+o
+
+The Fasc Threshold is the same thing just for fascicle segments.
+
+o
+
+The lower the Fasc Cont Threshold, the shorted the minimal acceptable length of
+detected fascicle segments to be included in the results.
+
+o
+
+The Minimal Width determined the minimal acceptable distance between
+superficial and deep aponeurosis.
+
+o
+
+Minimal and Maximal Pennation describe the respective minimal and maximal
+pennation angle that is physiologically possible in the analysed video
+frame/muscle.
+
+•
+
+For this tutorial, you can leave all parameters the way they are.
+
+•
+
+You can set the parameters by clicking the Set parameters button, the
+Analysis Parameter window will then close automatically.
+
+•
+
+Please make sure to adapt these parameters according to your images
+in analyses outside of this tutorial. For future analyses, it’s best you test
+the ideal parameter configuration in a small sample prior to the actual
 analysis.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-57
+54
 
 5. Running / Breaking DL_Track_US
-Now its time to start the actual analysis of the example video in the
-“DL_Track_US_example/video” folder. You can do so by clicking the Run button
-in the main GUI window.
-
-When you started the GUI using the command prompt in any way, you will see
-that the analysis is started by the statements printed in the prompt. Moreover
-the currently analysed frame with the segmentation results will pop up. When
-you started the GUI using the executable, you can see only the current frame
-with the segmentation results pop up. Moreover, you can see that there is a
-Break button placed in the GUI as well. Clicking the Break button allows you to
-stop the analysis at any point. The currently evaluated frame will be processed
-and then the analysis is terminated.
-Take a look at the next pages to see what happens during the analysis and once
-the analysis is finished.
+•
+
+•
+•
 
-06.04.2023
+You can start the analysis by clicking the Run button in the main GUI
+window.
+
+Moreover, you can see that there is a Break button placed in the GUI as
+well.
+Clicking the Break button allows you to stop the analysis at any point. The
+currently evaluated frame will be processed and then the analysis is
+terminated.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-58
+55
 
 Subsequently to clicking the Run button in the main GUI, navigate again to the
-“DL_Track_US_example/video” folder in your explorer. You will see that two
-files will be / have been created, calf_raise_proc.avi and calf_raise.xlsx. The
-calf_raise_proc.avi file contains each the input video with overlaid segmented
-fascicles and aponeurosis. This file allows you to visually inspect the model
-outputs. In your future analysis outside of this tutorial, you should always
-visually inspect the calf_raise_proc.avi file. The calf_raise.xlsx file contains the
-actual architectural parameter estimates for each video frame. There, all
-detected muscle fascicle lengths and pennation angles as well a the calculated
-muscle thickness will be displayed. Each video frame is displayed in a separate
-row. Note that the calf_raise_proc.avi file can be opened only after the
+“DL_Track_US_example/video”.
+•
+
+You will see that two files will
+calf_raise_proc.avi and calf_raise.xlsx.
+
+•
+
+The calf_raise_proc.avi file contains each the input video with overlaid
+segmented fascicles and aponeurosis. This file allows you to visually
+inspect the model outputs.
+
+•
+
+The calf_raise.xlsx file contains the actual architectural parameter
+estimates for each video frame. There, all detected muscle fascicle
+lengths and pennation angles as well a the calculated muscle thickness will
+be displayed. Each video frame is displayed in a separate row.
+
+•
+
+Note that the calf_raise_proc.avi file can be opened only after the
 calf_raise.xlsx. was created.
 
-When both files can be opened and you can see the analysis results, original
-image and the prediction result, we must congratulate you! You have now
-officially and successfully completed the DL_Track_US tutorial for automated
-video analysis! There is one more thing though, error handling. Take a look at
-the next section to get more information.
+26.04.2023
 
-06.04.2023
+be
 
 DL_Track_US python package - Tutorial
 
-59
+/
 
-6. Error handling
-Whenever an error occurs during the analysis process, the DL_Track_US GUI
-will open a messagebox. This looks always similar to this:
+have
+
+been
+
+created,
+
+56
+
+6. Error Handling
+Whenever an error occurs during the video analysis process, the
+DL_Track_US GUI will open a messagebox. This looks always similar to this:
 
 We tried to formulate these messageboxes as concise as possible. Just follow
 their instructions to fix the error and run the analysis anew. In case an error
 occurs that is not caught by an error messagebox, don’t hesitate to report this
 in the Q&A section in the DL_Track_US discussion forum. Please take a look
-here how do best do this. Otherwise, you can contact us by email at
-paul.ritsche@unibas.ch, but we would prefer the other way.
+here how do best do this.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-60
+57
 
-Manual Video
+M a n u a l Video
 Analysis
-The DL_Track_US python software package offers several different analysis
-types for analysis of human lower limb longitudinal ultrasonography images.
 The next and last analysis type this tutorial covers is the manual video analysis.
-The images are evaluated manually by drawing the muscle thickness, fascicle
-length and pennation angles directly on the Image. Scaling the images will
-ensure estimated muscle architectural parameters are converted to centimetre
-units. For this type of analysis, single videos are a prerequisite. These videos
-should
+The video frames are evaluated manually by drawing the muscle thickness,
+fascicle length and pennation angles directly on the Image. For this type of
+analysis, single videos are a prerequisite. These videos should
 be
 contained
 in
 a
 single
 folder,
 like
 in
 the
 “DL_Track_US_example/videos_manual” folder. If you haven’t downloaded this
 folder, please do so now (link: DL_Track_US - Examples & Models | Zenodo).
-Unzip the folder and put it somewhere accessible, for example on your
-desktop. We will make use of the included example files extensively during this
-tutorial. The manual video analysis type is identical to the manual image
-analysis type. The only difference is that the absolute video path must be
-specified instead of the File Type. The video is first converted and all the
-contained frames are separately stored as single images. Then, each frame
-image is analysed separately. In the next few pages, we will look at every
-required step to successfully perform manual video analysis with DL_Track_US.
+Unzip the folder and put it somewhere accessible. We will make use of
+the included example files extensively during this tutorial. The manual video
+analysis type is identical to the manual image analysis type. The only
+difference is that the absolute video path must be specified instead of the
+File Type. The video is first converted and all the contained frames are
+separately stored as single images. Then, each frame image is analysed
+separately. In the next few pages, we will look at every required step to
+successfully perform manual video analysis with DL_Track_US.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-61
+58
 
 1.
+•
+
+•
 
 Creating a Video Directory
 
-In order for DL_Track_US to recognize your videos, they should best be in a
-single folder (though one subfolder structure is acceptable as well). Take a look
-how you might structure this:
-
-You can see in the picture above that the folder contains one video and is
-located on the desktop. This structure is already included in the
-“DL_Track_US_example” folder. We will continue with demonstrating how to
-create folders for the aponeurosis and fascicle neural networks on the next
-page.
+All videos to be analyzed should be in a single folder.
+
+The “DL_Track_US_example/video_manual“ folder contains one video file.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-62
+59
 
 2. Specifying Relevant Parameters
-For the manual video analysis DL_Track_US analysis type, you do not need to
-specify any directories. Therefore, as a first step already, you will select the
-right analysis type in the GUI. Since this section is about manual video analysis,
-please select the Video Manual radiobutton. You can see that the GUI unfolds
-and another parameter appears. You will set this one in the next step on the
-next page.
+•
 
-06.04.2023
+Please select the Video Manual radiobutton.
 
-DL_Track_US python package - Tutorial
+•
 
-63
+You can see that the GUI unfolds and another parameter appears.
 
-Next, you need to specify the absolute File Path of the video file to be
-analysed. Remember that the example video file is placed in the
-“DL_Track_US_example/video_manual” folder. By clicking on the Video Path
-button in the GUI, a selection window opens were you need to select the
-example video file in the video_manual. Click open to specify the path to the
-video file in the GUI.
+•
 
-06.04.2023
+You will set this one in the next step on the next page.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-64
+60
 
-Allright, once you have specified the video file path, you can start with the
-analysis
-of
-the
+Next, you need to specify the absolute File Path of the video file to be
+analysed.
+•
+
+The
 example
 video
-contained
+file
+is
+“DL_Track_US_example/video_manual” folder.
+
+•
+
+By clicking on the Video Path button in the GUI, a selection window
+opens were you need to select the example video file in the
+video_manual.
+
+•
+
+Click open to specify the path to the video file in the GUI.
+
+26.04.2023
+
+DL_Track_US python package - Tutorial
+
+placed
+
 in
+
 the
-“DL_Track_US_example/video_manual” folder. You can start the analysis by
-clicking the Run button in the main GUI.
 
-Once you clicked the Run button, the “Manual Analysis window” will pop up. If
-this happens, congrats to you! You have entered all relevant parameters for the
-manual video analysis correctly!
-From here, all further steps are identical with the manual image analysis. The
-only difference though is that in the folder of the inputted video, a new folder
-is created containing all the single image frames.
-The scaling of the image, extending of the aponeuroses, single segment muscle
-thickness measurements, three segment muscle fascicle measurement and
-two segment pennation angle measurement are identical. Saving the results
-(with the very important button), continuing to the next image frame,
-terminating the analysis process and error handling is identical. Therefore, we
-kindly refer you to section 4 of this tutorial Manual Image Analysis (because
-we don’t want to repeat ourselves) to see how the all the architectural
-parameters are analysed. We are confident that you can do this on your own
-now!
+61
+
+•
+
+You can start the analysis by clicking the Run button in the main GUI.
+
+•
+
+Once you clicked the Run button, the “Manual Analysis window” will pop
+up.
+
+•
+
+From here, all further steps are identical with the manual image analysis.
+
+•
+
+The only difference though is that in the folder of the inputted video, a
+new folder is created containing all the single image frames.
 
-06.04.2023
+•
+
+The scaling of the image, extending of the aponeuroses, single segment
+muscle thickness measurements, three segment muscle fascicle
+measurement and two segment pennation angle measurement are
+identical.
+
+•
+
+Saving the results (with the very important button), continuing to
+the next image frame, terminating the analysis process and error
+handling is identical.
+
+•
+
+Therefore, we kindly refer you to section 4 of this tutorial Manual Image
+Analysis (because we don’t want to repeat ourselves) to see how the
+all the architectural parameters are analysed.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-65
+62
 
 Training Your Own
 Networks
-Not only does the DL_Track_US python software package offer four different
-analysis types for musculoskeletal ultrasonography images and videos of
-human lower limb muscles. The package also includes the possibility to train
-your own neural networks that may be better suited for images with different
-characteristics than those in our training data. This is also embedded in the
-GUI. It is advantageous to have a working GPU setup, otherwise model training
-will take much longer. How to setup you GUI for DL_Track_US is described in
-the installation guidelines of our Github repository. In the next few pages, you
-will learn to train your own neural to train your own neural networks. This is
-also the last part of this tutorial. After completion of this chapter, you will
-know the DL_Track_US GUI as well as the back of your hand. If you don’t have
-any experience with training deep neural networks, we strongly advise to work
-with the pre-defined settings. Otherwise, you are of course free to choose. For
-this introductory tutorial, we would however like you to use the pre-defined
-settings no matter what your experience level is. Although you can generally
-adapt a number of parameters during training, you cannot change the neural
-network architecture from the GUI (of course you could modify source code to
-do so). This is because during experimenting with different model
-architectures, we found a combination of a on imagenet pre-trained VGG16
-encoder and a standard U-net decoder to be the best performing model. Thus,
-all the models trained using the GUI will have this architecture. To explain you
-the parameters used during model training that are adaptable from the GUI is
-out of the scope of this tutorial. However, we would like to refer you to this
-excellent introductory course in case you are a deep learning beginner. Training
-your own networks for muscle architecture analysis requires pairs of original
-images and manually labelled masks. Examples are provided for you in the
-“DL_Track_US_example/model_training” folder. If you haven’t downloaded
-this folder, please do so now (link: ). Unzip the folder and put it somewhere
-accessible, for example on your desktop. We will make use of the included
-example files extensively during this tutorial. In this tutorial, you will only learn
-to train model that segment the muscle aponeuroses. Yes that’s right, segment
-the fascicles requires a separate model because the task is so different.
-However, everything works the same, you just need to use fascicle images and
-masks instead of aponeurosis images and masks. Examples of those are
-provided in the “DL_Track_US_example/model_training” folder as well.
-Anyway, enough said. Let’s get to the model training part. The most important
-part is data preparation and labelling. This is where you will start.
-06.04.2023
+The DL_Track_US package GUI includes the possibility to train your own
+neural networks. We we will demonstrate how to do this, with a few notes at
+the beginning:
+•
+
+It is advantageous to have a working GPU setup, otherwise model training
+will take much longer. Take a look at our Github repository for further
+instructions.
+
+•
+
+If you don’t have any experience with training deep neural networks,
+please refer to this course. We advise you to start with the pre-defined
+settings. However, DL_Track_US does not allow to change the
+architecture of the trained neural networks.
+
+The paired original images and labeled masks required for the network
+training are located in the “DL_Track_US_example/model_training” folder. If
+you haven’t downloaded this folder, please do so now (link: DL_Track_US Examples & Models | Zenodo). Unzip the folder and put it somewhere
+accessible. We will demonstrate how to train a model that segments the
+muscle aponeuroses.
+Please keep in mind that the model training process will be illustrated by
+training a model for aponeurosis segmentation. The process is exactly the
+same for training a fascicle segmentation model. Solely the images and masks
+should then contain fascicles and fascicle labels.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-66
+63
 
 1.
 
 Data Preparation and Image Labeling
 
-In order for DL_Track_US to recognize your aponeurosis images and
-aponeurosis masks, they should best be in different single folders. Take a look
-how you might structure this:
-
-You
-can
-see
-in
-the
-picture
-above
-that
-the
-“DL_Track_US_example/model_training” folder contains two subfolders,
-“apo_img_example” and “apo_mask_example”. The original images are
-located in the “apo_img_example” folder whereas the corresponding masks
-are located in the “apo_maks_example” folder. We advise you to keep a
-similar folder structure when you train your own models outside of this
-tutorial. When you take a look below, you can see that the original image and
-the corresponding masks have exactly the same name. This is SUPER MEGA
-important. Otherwise, the model is trained using the wrong masks for the
-images. You do not want this!
+•
 
-06.04.2023
+Your prepared aponeurosis images and aponeurosis masks should be in
+different folders.
 
-DL_Track_US python package - Tutorial
+•
 
-67
+The «DL_Track_US_example/model_training” folder contains to subfolders,
+apo_img_example” and “apo_mask_example”.
+The original images are located in the “apo_img_example” folder.
+The corresponding masks are located in the “apo_maks_example”
+folder.
+We advise you to keep a similar folder structure when you train
+your own models outside of this tutorial.
+Below you can see that the original image and the corresponding masks
+have exactly the same name. This is SUPER MEGA important. Otherwise,
+the model is trained using the wrong masks for the images.
 
-Caution, this section is not part of the tutorial. It is merely additional
-information for you that is not required to run the GUI and follow the
-example model training tutorial. The actual tutorial continues on page 72.
-When you want to train your own networks outside of this tutorial, you need
-to label your original ultrasonography images of the lower limbs. We have
-prepared you the instructions how to use the automated script that we
-provide (this script does not automatically label the images, but automates the
-selection processes and image / mask saving). The software you will perform
-the labelling in is called ImageJ / Fiji. You can download the software here. The
-automated script “Image_Labeling_DL_Track_US.ijm” is located in the folder
-“DL_Track_US/docs/labeling/” in our Github repository.
-The easiest way to run the “Image_Labeling_DL_Track_US.ijm” script is by
-simply drag and drop it in the Fiji / ImageJ window. Therefore, Fiji / ImageJ
-must be already running. As a result, the script will opened.
+•
+•
 
-06.04.2023
+•
+•
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-68
+64
 
-Before you can start the labelling process however, you need to create four
-folders in an easily accessible place (perhaps your desktop?). One folder
-containing the original images you want to label. Then create three more
-folders, one named “output_images”, the second called “fascicle_masks” and
-the third called “aponeurosis_masks”. In the “output_images” the original
-images are saved with an adapted name. In the “fascicle_masks” and
-“aponeurosis_masks” folder the respective masks are saved with the same
-name as the corresponding image in “output_images”.
+2. Specifying Relevant Directories
+•
 
-Take a look at the next page on how to continue once you created the above
-demonstrated folder structure.
+As a next step, you can start the GUI.
 
-06.04.2023
+•
 
-DL_Track_US python package - Tutorial
+Once you started the GUI and the main GUI window opened, click on the
+Train Model button to select the relevant directories and model
+training parameters.
 
-69
+•
 
-Once you created the above demonstrated folder structure, simply press the
-Run
-button
-in
-the
-Fiji
-/
-ImageJ
-API
-to
-start
-the
-“Image_labelling_DL_Track_US.ijm” script.
+The separate “Model Training window” will pop up.
 
-Please follow the instructions appearing in the messageboxes. To begin with,
-you need to specify the four directories. The first directory you need to select is
-the original image folder (called input dir). The second folder is the
-“aponeurosis_masks” folder (called apo mask dir). The third is the
-“fascicle_masks” folder (called fasc mask dir). The last folder you need to
-specify is the “output_images” folder (called image dir). Subsequent to
-specifying the directories, you are required to create the masks. First the
-aponeurosis mask, then the fascicle mask. How to do this is demonstrated on
-the next page.
+•
 
-06.04.2023
+We will explain this window on the next page.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-70
+65
 
-The polygon tool is selected automatically for you to draw around the
-superficial aponeurosis. Again, follow the instructions in the messagebox.
-Draw around the superficial aponeurosis (double click to start drawing, click to
-add a segment, double click do stop drawing) and once you are finished, click
-the OK button in the messagebox to proceed to the selection of the lower
-aponeurosis Please be careful to only include aponeurosis tissue in your
-selection and no surrounding tissue. The result should look like this for the
-upper and lower aponeurosis:
+Firstly, select the “Image Directory”.
+•
 
-Once you have selected the lower aponeurosis, click the OK button in the
-messagebox to proceed to the fascicle labelling. Take a look on the next page
-to see how this is done.
+Click th button Images.
 
-06.04.2023
+•
 
-DL_Track_US python package - Tutorial
+A selection window will appear and you can select the folder
+containing the original images.
 
-71
+•
 
-The segmented line tool is selected automatically for you to follow the visible
-fascicle segments. Again, simply follow the instructions in the messagebox. It is
-of utmost importance that you draw only over the actually visible parts of the
-fascicle segment. Make sure that you only label bright fascicle tissue that is
-clearly visible. Once you drew one fascicle with segmented line tool (double
-click to start drawing, click to add a segment, double click do stop drawing)
-click the OK button in the messagebox to proceed to the next fascicle segment.
-Draw as many segments as are clearly visible on the image. When you press
-the OK button in the messagebox without making a further selection, you will
-proceed to the next image in the original image folder and start again with the
-aponeurosis labelling. The result of you labelling should look something like
-this:
-
-When you read this, you now how to label images to train your own neural
-networks with your own lower limb ultrasonography images! Congrats! We will
-now continue with the example tutorial on how to train your own networks
-with the example images and masks provided.
+Select the
+folder.
+
+26.04.2023
 
-06.04.2023
+“DL_Track_US_example/model_training/apo_img_example”
 
 DL_Track_US python package - Tutorial
 
-72
+66
 
-2. Specifying Relevant Directories
-Caution, the actual tutorial continues here!
-Please keep in mind that the model training process will be illustrated by
-training a model for aponeurosis segmentation. The process is exactly the
-same for training a fascicle segmentation model. Solely the images and masks
-should then contain fascicles and fascicle labels.
-As a next step, you can start the GUI. If you do not know how to do this, please
-take a look at section two of this tutorial, Starting the GUI.
-Once you started the GUI and the main GUI window opened, click on the Train
-Model button to select the relevant directories and model training
-parameters. The separate “Model Training window” will pop up. We will
-explain this window on the next page.
+Your next step is to select the “Mask Directory”.
 
-06.04.2023
+•
 
-DL_Track_US python package - Tutorial
+the button Masks.
 
-73
+•
 
-Once the “Model Training window” opened up, you first step is to select the
-“Image Directory” by clicking the button Images. A selection window will
-appear and you can select the folder containing the original images. In this
-tutorial,
-select
-the
-“DL_Track_US_example/model_training/apo_img_example” folder.
+A selection window will appear to select the folder
+mask images.
+
+•
+
+Select the “DL_Track_US_example/model_training/apo_mask_example”
+folder.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-74
+containing
 
-Your next step is to select the “Mask Directory” by clicking the button Masks.
-A selection window will appear and, you guessed correctly, you can select the
-folder containing the mask images. In this tutorial, select the
-“DL_Track_US_example/model_training/apo_mask_example” folder.
+the
 
-06.04.2023
+67
 
-DL_Track_US python package - Tutorial
+The last directory you need to select for training your own network
+is the “Output Directory”.
+•
 
-75
+Click the button Output.
 
-The last directory you need to select for training your own network is the
-“Output Directory” by clicking the button Output. In the Output directory, the
-trained model, the corresponding loss calculation results and a graphic
-displaying plotting the training epochs against the loss values will be saved. A
-selection window will appear and you can select any folder you like. In this
-tutorial,
-for
-simplicity
-reasons,
-please
-select
-the
-“DL_Track_US_example/model_training” folder.
+•
+
+In the Output directory, the trained model, the corresponding loss
+calculation results and a graphic displaying plotting the training
+epochs against the loss values will be saved.
+
+•
+
+A selection window will appear and you can select any folder you
+like.
 
-Great, you have selected all relevant directories for model training! Now we
-shall take a look at the training parameters on the next page.
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-76
+68
 
 3. Specifying Training Parameters
-Now to specifying the training parameters. You actually don’t have to do
-anything at this point, just leave the pre-specified selections as they are. If you
-do not know what these training parameters mean, take a look at the videos
-we mentioned in the introductory text of this chapter. The only thing we have
-to say is that you must NEVER use only three Epochs for actual model training.
-Such a small number of training Epochs is only acceptable for demonstration
-and testing purposes. For actual training of your own neural networks, go with
-at least 60 Epochs (or maybe 42 is the better choice?).
+Now to specifying the training parameters.
+•
+
+For the tutorial leave the pre-specified selections as they are.
+
+•
+
+If you do not know what these training parameters mean, take a look at
+this course.
 
-Take a look at the next page to learn how to continue from here.
+•
 
-06.04.2023
+The only thing we have to say is that you must NEVER use only three
+Epochs for actual model training.
+
+•
+
+Such a small number of training Epochs is only acceptable for
+demonstration and testing purposes.
+
+•
+
+For actual training of your own neural networks, go with at least 60
+Epochs.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-77
+69
 
 The only thing you have left to do for the training process to start is to click the
 Start Training button.
 
-During the training process, three messageboxes will pop up. The first one will
-tell you that the images and masks were successfully loaded for further
-processing. The second one will tell you that the model was successfully
-compiled and can now be trained. The last one will tell you that the training
-process was completed. You do have a choice in each messagebox of clicking
-“OK” or “Cancel”. Clicking “OK” will continue the training process, whereas
-clicking “Cancel” will be cancelling the ongoing training process.
+•
+
+During the training process, three messageboxes will pop up.
+
+•
+
+The first one will tell you that the images and masks were
+successfully loaded for further processing.
+
+•
 
-06.04.2023
+The second one will tell you that the model was successfully
+compiled and can now be trained.
+
+•
+
+The last one will tell you that the training process was completed.
+
+•
+
+You do have a choice in each messagebox of clicking “OK” or “Cancel”.
+
+•
+
+Clicking “OK” will continue the training process, whereas clicking
+“Cancel” will be cancelling the ongoing training process.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-78
+70
 
-Once the model training process is completed, there will three new files in
-your selected output directory. Remember, you specified the
-“DL_Track_US_example/model_training” folder as your output directory.
-These new files are the trained model as a Test_Apo.h5 file, the
-corresponding loss values for each epoch as Test_apo.csv file and a graphical
-representation of the training process as Training_Results.tif file.
-
-In case you can open the loss values and the graphical training representation,
-we congratulate you! You have successfully trained your first own neural
-network using the DL_Track_US package. Awesome! This is also the end of this
-tutorial, as Training Your Own Networks was the final chapter. Have a look at
-the closing remarks for a few more things. And, before it is forgotten, there is
-one more section on the next page. Error handling.
+Once the training process in finished, three new files will be placed in your
+output directory.
+• The trained model as Test_Apo.h5 file.
+• The corresponding loss values for each epoch as Test_apo.csv file
+• The graphical representation of the training process as Training_Results.tif
+file.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-79
+71
 
 4. Using Your Own Networks
-Once you have trained your aponeurosis or fascicle segmentation model (in
-case of this tutorial to model was called “Test_Apo.h5”), it is time to start using
-it. You have previously learned how to do that, in section 3 “Automated Image
-Analysis” on page 14 and 15 of this tutorial to be precise. Simply select the
-path to your model (or the “Test_Apo.h5” model) by clicking the Apo Model or
-Fasc Model buttons in the GUI, depending which kind of model you have
-trained. In our case, we would click the Apo Model button, since we trained
-the “Test_Apo.h5” model on aponeurosis images and labels. Subsequently to
-specifying all other relevant parameters for your analysis in the GUI (as you
-have learned a couple pages ago), DL_Track_US will analyse your data using
-your own model (or the “Test_Apo.h5” model we have trained together).
-
-Lastly, a short disclaimer when training your own model. It is called bad
-practice when using the same images for model training and inference. At least
-during the model evaluation phase (checking how good your model actually is).
-Without going into details (see the introductory course we mentioned at the
-beginning), the model should not be used for analysing images it was trained
-on because it already knows the characteristics of these images. Since you
-should ALWAYS compare the results of your model to a manual evaluation on a
-few of your own images, use different images (best from different individuals)
-for model training and comparison to manual analysis. If this seems strange to
-you, don’t hesitate to ask for further clarification in the DL_Track_US discussion
-forum.
+How do you use you previously trained neural network?
+•
+
+Simply select the path to your model by clicking the Apo Model or Fasc
+Model buttons in the GUI, depending on which model you want to
+import.
+
+•
+
+Subsequently to specifying all other relevant parameters for your
+analysis in the GUI (as you have learned a couple pages ago).
+
+•
+
+DL_Track_US will now analyse your data using your own model.
+
+Lastly, a short disclaimer when training your own model.
+•
+
+It is bad practice using the same images for model training and inference.
+
+•
+
+The model should not be used for analysing images it was trained on
+because it already knows the characteristics of these images.
 
-06.04.2023
+•
+
+ALWAYS compare the results of your model to a manual evaluation on a
+few of your own images. Use different images (best from different
+individuals) for model training and comparison to manual analysis.
+
+•
+
+If this seems strange to you, don’t hesitate to ask for further clarification in
+the DL_Track_US discussion forum.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-80
+72
 
-5. Error handling
+5. Error Handling
 Whenever an error occurs during the analysis process, the DL_Track_US GUI
 will open a messagebox. This looks always similar to this:
 
 We tried to formulate these messageboxes as concise as possible. Just follow
 their instructions to fix the error and run the analysis anew. In case an error
 occurs that is not caught by an error messagebox, don’t hesitate to report this
 in the Q&A section in the DL_Track_US discussion forum. Please take a look
-here how do best do this. Otherwise, you can contact us by email at
-paul.ritsche@unibas.ch, but we would prefer the other way.
+here how do best do this.
 
-06.04.2023
+This is the end of the main tutorial. The next chapter covers how to label your
+aponeurosis and fascicle images used for model training.
+
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-81
+73
+
+Image Labels
+When you train your own networks, you need to label your original
+ultrasonography images.
+•
+
+We provide an automated script for image labellig.
+
+•
+
+This script does not automatically label the images, but automates the
+selection processes and image / mask saving.
+
+•
+
+The software you will perform the labelling in is called ImageJ / Fiji. You
+can download ithere.
+
+•
+
+The automated script “Image_Labeling_DL_Track_US.ijm” is located in
+the folder “DL_Track_US/docs/labeling/” in our Github repository.
+The easiest way to run the “Image_Labeling_DL_Track_US.ijm” script
+is by simply drag and drop it in the running Fiji / ImageJ window.
+
+•
+
+26.04.2023
+
+DL_Track_US python package - Tutorial
+
+74
+
+Before you can start the labelling process:
+•
+
+Create four folders in an easily accessible place.
+
+•
+
+One folder containing the original images you want to label.
+
+•
+
+Then create three more folders, one named “output_images”, the
+second
+called
+“fascicle_masks”
+and
+the
+third
+called
+“aponeurosis_masks”.
+
+•
+
+In the “output_images” the original images
+adapted name.
+
+•
+
+In
+the
+“fascicle_masks”
+and “aponeurosis_masks” folder the
+respective masks are saved with the same name as the corresponding
+image in “output_images”.
+
+26.04.2023
+
+DL_Track_US python package - Tutorial
+
+are
+
+saved
+
+with
+
+an
+
+75
+
+When you have created all folders, press the Run button in the Fiji /
+ImageJ API to start the “Image_labelling_DL_Track_US.ijm” script.
+
+Follow the instructions appearing in the messageboxes.
+•
+
+To begin with, you need to specify the four directories.
+
+•
+
+The first directory you need to select is the original image folder (called
+input dir).
+
+•
+
+The second folder is the “aponeurosis_masks” folder (called apo
+mask dir).
+
+•
+
+The third is the “fascicle_masks” folder (called fasc mask dir).
+
+•
+
+The last folder you need to specify is the “output_images” folder
+(called image dir).
+
+•
+
+Subsequent
+the masks.
+
+•
+
+First the aponeurosis mask, then the fascicle mask.
+
+•
+
+How to do this is demonstrated on the next page.
+
+26.04.2023
+
+to specifying the directories, you are required to create
+
+DL_Track_US python package - Tutorial
+
+76
+
+•
+
+Firstly, draw the superficial aponeurosis using the selected polygon tool
+by following the instructions in the messagebox.
+
+•
+
+Draw around the superficial aponeurosis (double click to start drawing,
+click to add a segment, double click do stop drawing).
+
+•
+
+Once you are finished, click the OK button in the messagebox to
+proceed to the selection of the lower aponeurosis.
+
+•
+
+Please be careful to only include aponeurosis tissue in your selection
+and no surrounding tissue.
+
+•
+
+The result should look like this for the upper and lower aponeurosis:
+
+Once you have selected the lower aponeurosis, click the OK button in the
+messagebox to proceed to the fascicle labelling. Take a look on the next page
+to see how this is done.
+26.04.2023
+
+DL_Track_US python package - Tutorial
+
+77
+
+The segmented line tool is selected automatically for you to follow the visible
+fascicle segments.
+• Follow the instructions in the messagebox.
+• It is of utmost importance that you draw only over the actually visible
+parts of the fascicle segment.
+• Make sure that you only label bright fascicle tissue that is clearly visible.
+• Once you drew one fascicle with segmented line tool (double click to
+start drawing, click to add a segment, double click do stop drawing)
+click the OK button in the messagebox to proceed to the next fascicle
+segment.
+• Draw as many segments as are clearly visible on the image.
+• When you press the OK button in the messagebox without making a
+further selection, you will proceed to the next image in the original image
+folder and start again with the aponeurosis labelling.
+• The result of you labelling should look something like this:
+
+26.04.2023
+
+DL_Track_US python package - Tutorial
+
+78
 
 Closing remarks
 Thanks for checking out the DL_Track_US python package tutorial. We hope
 you were able to enjoy it a bit. Moreover, we hope it was clear, concise and
 easy to follow. We tried to put our biases aside and to start from scratch. In
 case we failed to do so at some point and something was not clearly illustrated,
 please let us know. Don’t hesitate to report this in the Q&A section in the
 DL_Track_US discussion forum. Otherwise, you can contact us by email at
-paul.ritsche@unibas.ch, but we would prefer the other way.
+paul.ritsche@unibas.ch.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tutorial
 
-82
+79
```

### Comparing `dl_track_us-0.1.2.1/tests/DL_Track_US_tests.pdf` & `dl_track_us-0.1.2.2/tests/DL_Track_US_tests.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,183 +1,201 @@
 DL_Track_US
 v0.1.2
 
 Preface
-Welcome to the DL_Track_US python package tests. In the next roughly 20
-pages, we will demonstrate how you can objectively test the functionality of
-DL_Track_US when automatically and manually analysing ultrasonography
-images and videos of human lower limb muscles. Because we have not (yet)
+Welcome to the DL_Track_US python package tests. Because we have not (yet)
 integrated unit testing in the DL_Track_US python package, we have prepared
-specific instructions and provided example results. This testing tutorial works
-in the way that you will perform several analyses and compare your results to
-the test result we provided. If the results are comparable, the DL_Track_US
-python package is functional. Have fun!
+specific instructions and provided example results. You will perform several
+analyses and compare your results to the test result we provided. If the results
+are comparable, the DL_Track_US python package is functional. Have fun!
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 2
 
 Content
 1.
 2.
 3.
 4.
 5.
 
-Good to know… _________________________4
+Good to know___________________________4
 Automated Image Analysis Test_____________5
 Manual Image / Video Analysis Test_________8
 Automated Video Analysis Test____________12
 Model Training Test_____________________15
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 3
 
-Good to know…
+Good to know
 All relevant instructions and guidelines for the installation of the DL_Track_US
 software package are described in our Github repository, so please take a look
 there if anything is unclear.
-
 Before we start with testing, here are some important points to consider:
 • Please exactly follow the instruction we provide!
 • We assume that you have looked at the “DL_Track_US_tutorial.pdf” file prior
 to working through these test instructions. We therefore won’t explain the
 core functionalities of the DL_Track_US GUI.
 • All of the test files required for testing procedures are in the
 “DL_Track_US_example/tests” folder. If you have not downloaded the
 “DL_Track_US_example” folder, you can do so here. Unzip it and put it
 somewhere you can easily access it, you will use it extensively during testing.
-• During the testing process, you will need our pre-trained models. If you have
-not downladed them already, you can do so here. Unzip the folder, put it
-somewhere you can easily access it and select the included aponeurosis and
-fascicle model for the testing procedures.
+
 • In case you encounter problems during the testing process or your test
 results deviate from the ones we provided without reasonable explanation,
-please report it. Take a look here how to best do this. Otherwise contact us
-at paul.ritsche@unibas.ch, but we would prefer the other way.
+please report it. Take a look here how to best do this.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 4
 
 Automated Image
 Analysis Test
-The DL_Track_US python software package offers several different analysis
-types for analysis of human lower limb longitudinal ultrasonography images.
 The first analysis type you are going to test is the automated image analysis.
-The images are evaluated without user input and may be scaled. However, we
-will not scale the images during testing. For this test, single images (not videos)
-are a prerequisite. The test images and the flip_flag.txt file you must use for
-this
-test
-are
-located
-in
-the
-“DL_Track_US_example/tests/test_images_automatic” folder. In the next few
-pages, we will look at every required step to successfully perform automated
-image analysis testing.
+• The images are evaluated without user input.
+• For this test, single images (not videos) are a prerequisite.
+• The test images and the flip_flag.txt file you must use for this test are
+located in the “DL_Track_US_example/tests/test_images_automatic” folder.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 5
 
 For this test make sure that the files used and parameters specified are exactly
-as demonstrated below. Moreover, keep the pre-specified parameter settings
-in the “Analysis Parameter window” as they are. Once you made sure to use
-the right images (“DL_Track_US_example/tests/test_images_automated”), the
-provided pre-trained models and the right flip_flag.txt file
-(“DL_Track_US_example/tests/test_images_automated/flip_flags.txt”),
-click
-the Select parameters button to set the analysis parameters and then the Run
-button to start the analysis.
+as demonstrated below.
+• Keep the pre-specified parameter settings in the “Analysis Parameter
+window” as they are.
+• Make
+sure
+to
+use
+the
+right
+(“DL_Track_US_example/tests/test_images_automated”).
+
+images
 
-06.04.2023
+• Make
+sure
+to
+use
+provided
+(“DL_Track_US_example/DLTrack_models”).
+
+models
+
+pre-trained
+
+• Make
+sure
+to
+use
+the
+right
+flip_flag.txt
+(“DL_Track_US_example/tests/test_images_automated/flip_flags.txt”).
+
+file
+
+• Click the Select parameters button to set the analysis parameters and then
+the Run button to start the analysis.
+
+26.04.2023
 
 DL_Track_US python package - Tests
 
 6
 
 Once the analysis is complete, two new files were created in the
-“DL_Track_US_example/tests/test_images_automated”
-folder.
-The
-ResultImages.pdf file and the Results.xlsx file. You can disregard the
-ResultImages.pdf for this test.
+“DL_Track_US_example/tests/test_images_automated” folder.
+• The ResultImages.pdf file.
+• The Results.xlsx file.
+
+•
+•
 
 Open the Results.xlsx file and compare the analysis results to the ones
-demonstrated below. If the results are similar, the DL_Track_US package works
-properly for automated images analysis! Yay!
+demonstrated below.
+If the results are similar, the DL_Track_US package works properly for
+automated images analysis!
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 7
 
 Manual Image /
 Video Analysis Test
-The DL_Track_US python software package offers several different analysis
-types for analysis of human lower limb longitudinal ultrasonography images.
 The next analysis type you are going to test is the manual image / video
-analysis. The images are evaluated by manually segmenting the architectural
-parameters directly on the image. For this test, single images (not videos) are a
-prerequisite. The test image you must use for this test is located in the
-“DL_Track_US_example/tests/test_images_manual” folder. In the next few
-pages, we will look at every required step to successfully perform manual
-image / video analysis testing. No worries, we do not talk about a new analysis
-type you haven’t heard of. The analysis types manual image analysis and
-manual video analysis make use of the same python class (called
-“ManualAnalysis” and located in the manual_tracing.py file) and therefore use
-the same functionalities to determine architectural parameters in single
-images or video frames. In our opinion, it is thus not necessary to test both
-analysis types.
+analysis.
+• For this test, single images (not videos) are a prerequisite.
+• The test image you must use for this test is located in the
+“DL_Track_US_example/tests/test_images_manual” folder.
+
+• The analysis types manual image analysis and manual video analysis make
+use of the same python class (called “ManualAnalysis” and located in the
+manual_tracing.py file).
+• In our opinion, it is thus not necessary to test both analysis types.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 8
 
 For this test make sure that the files used and parameters specified are exactly
-as demonstrated below. Once you made sure to use the right image
-(“DL_Track_US_example/tests/test_image_manual”), click the Run button to
-start the analysis.
+as demonstrated below.
+• Make
+sure
+to
+use
+the
+(“DL_Track_US_example/tests/test_image_manual”).
 
-Take a look at the next page to see how to continue.
+right
 
-06.04.2023
+image
+
+• Click the Run button to start the analysis.
+
+26.04.2023
 
 DL_Track_US python package - Tests
 
 9
 
 The “Manual Analysis window” should pop up containing the image as
 demonstrated below.
 
 For testing the DL_Track_US manual image / video analysis, simply reanalyse
-the drawn lines. First, scale the image by following the one centimetre long
-scaling line in the left of the image. Then, redraw the superficial and deep
-aponeurosis extension lines. Subsequently, re-analyse the three vertical muscle
-thickness lines using one segment each, the three diagonal fascicle lines using
-three segments each and the three pennation angles using two segments each.
-Always choose the Radiobutton corresponding to the parameter you are
-analysing. Once you have re-analysed all the lines image, click on the Save
-Results button to save your analysis results.
+the drawn lines.
+• First, scale the image by following the one centimetre long scaling line in the
+left of the image.
+• Then, redraw the superficial and deep aponeurosis extension lines.
+• Subsequently, re-analyse the three vertical muscle thickness lines using one
+segment each, the three diagonal fascicle lines using three segments each
+and the three pennation angles using two segments each.
+• Always choose the Radiobutton corresponding to the parameter you are
+analysing.
+• Once you have re-analysed all the lines image, click on the Save Results
+button to save your analysis results.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 10
 
 One
 new
@@ -187,145 +205,169 @@
 in
 the
 “DL_Track_US_example/tests/test_image_manual”, the Manual_Results.xlsx
 file.
 
 Open the Manual_Results.xlsx file and compare the analysis results to the
 ones demonstrated below. If the results are similar, the DL_Track_US package
-works properly for manual image / video analysis! Awesome!
+works properly for manual image / video analysis!
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 11
 
 Automated Video
 Analysis Test
-The DL_Track_US python software package offers several different analysis
-types for analysis of human lower limb longitudinal ultrasonography images.
 The next analysis type you are going to test is the automated video analysis.
-Single video frames are evaluated automatically without user input. For this
-test, videos are a prerequisite. The test video you must use for this test is
-located in the “DL_Track_US_example/tests/test_video_automated” folder. In
-the next few pages, we will look at every required step to successfully perform
-automated video analysis testing.
+• Single video frames are evaluated automatically without user input.
+• For this test, videos are a prerequisite.
+• The test video you must use for this test is located in the
+“DL_Track_US_example/tests/test_video_automated” folder.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 12
 
 For this test make sure that the files used and parameters specified are exactly
-as demonstrated below. Moreover, keep the pre-specified parameter settings
-in the “Analysis Parameter window” as they are. Once everything looks like
-illustrated below and you made sure to use the right video
-(“DL_Track_US_example/tests/test_video_automated”) and the provided pretrained model files (model-apo-VGG16-BCE-512.h5 & model-fasc-VGG16-BCE512.h5), click the Select parameters button to set the analysis parameters and
-then the Run button to start the analysis.
+as demonstrated below
+• Make
+sure
+to
+use
+the
+right
+(“DL_Track_US_example/tests/test_video_automated”).
+
+video
 
-06.04.2023
+• Make sure to use the provided pre-trained model files (model-apo-VGG16BCE-512.h5 & model-fasc-VGG16-BCE-512.h5).
+• Keep the pre-specified parameter settings in the “Analysis Parameter
+window” as they are.
+• Click the Select parameters button to set the analysis parameters.
+• Click the Run button to start the analysis.
+
+26.04.2023
 
 DL_Track_US python package - Tests
 
 13
 
 When the analysis is complete, two new files were created in the
-“DL_Track_US_example/tests/test_video_automated”
-folder.
-The
-calf_raise_proc.avi file and the calf_raise.xlsx file. You can disregard the
-calf_raise_proc.avi for this test.
-
-Open the calf_raise.xlsx file. Take the average value from all calculated fascicle
-length values in all frames, all calculated pennation angles in all frames, all
-calculated muscle thickness values in all frames and all calculated upper
-(x_high) and lower (x_low) aponeuroses edge coordinates in all frames. If the
-results are similar to those demonstrated below, the DL_Track_US package
-works properly for automated images analysis! Wohoo!
+“DL_Track_US_example/tests/test_video_automated” folder.
+• The calf_raise_proc.avi file.
+• The calf_raise.xlsx file.
+
+•
+
+Open the calf_raise.xlsx file.
+
+•
 
-06.04.2023
+Take the average value from all calculated fascicle length values in all
+frames, all calculated pennation angles in all frames, all calculated muscle
+thickness values in all frames and all calculated upper (x_high) and lower
+(x_low) aponeuroses edge coordinates in all frames.
+
+•
+
+If the results are similar to those demonstrated below, the DL_Track_US
+package works properly for automated images analysis!
+
+26.04.2023
 
 DL_Track_US python package - Tests
 
 14
 
 Model Training Test
-Not only does the DL_Track_US python software package offer four different
-analysis types for musculoskeletal ultrasonography images and videos of
-human lower limb muscles. The package also includes the possibility to train
-your own neural networks that may be better suited for images with different
-characteristics than those in our training data. This is also embedded in the
-GUI. It is advantageous for model training testing to have a working GPU setup,
-otherwise model training takes much longer. How to setup you GUI for
-DL_Track_US is described in the installation guidelines of our Github
-repository. In the next few pages, you will test the neural network training
-functionality of DL_Track_US. The test training images and masks you must use
-for this test are located at “DL_Track_US_example/tests/model_training”
-folder. This is the last part of the test instructions. After completion of this
-chapter, you will have tested DL_Track_US thoroughly!
+In the next few pages, you are going to test the model training using the GUI.
+• It is advantageous for model training testing to have a working GPU setup,
+otherwise model training takes much longer.
+• How to setup you GUI for DL_Track_US is described in the installation
+guidelines of our Github repository.
+• The test training images and masks you must use for this test are located at
+“DL_Track_US_example/tests/model_training” folder.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 15
 
 For this test make sure that the files used and parameters specified are exactly
-as demonstrated below. Since you will only make use of the “Model Training
-window” you can disregard the main GUI. Everything specified there is
-irrelevant for model training. Keep the pre-specified parameter settings in the
-“Model Training window” as they are shown below. Especially make sure that
-the number of Epochs is 3 (otherwise training for test purposes takes to long)
-Once everything looks like illustrated below and you made sure to use the right
+as demonstrated below.
+• Click on the “Train Model” button in the main GUI.
+• Since you will only make use of the “Model Training window” you can
+disregard the main GUI.
+• Keep the pre-specified parameter settings in the “Model Training window”
+as they are shown below.
+• Especially make sure that the number of Epochs is 3 (otherwise training for
+test purposes takes to long).
+• made
+sure
+to
+use
+the
+right
 training
 images
-and
+(“DL_Track_US_example/tests/model_training/apo_img_example”)
+
+• Make
+sure
+to
+use
+the
+right
+training
 masks
-(“DL_Track_US_example/tests/model_training/apo_img_example”
-&
-“DL_Track_US_example/tests/model_training/apo_mask_example”) click the
-Start Training button to start the training process.
+“DL_Track_US_example/tests/model_training/apo_mask_example”).
+• Click the Start Training button to start the training process.
 
 Several messageboxes will appear during the training process. Always click
 “OK”. The messageboxes simply tell you that the images and masks have
 successfully been loaded, the model was successfully compiled and that the
 analysis was successfully completed.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 16
 
-When the analysis is complete, three new files were created in the
-“DL_Track_US_example/tests/model_training” folder. The Test_apo.xlsx, the
-Test_apo.h5 file and the Training_results.tif file.
+When the analysis is complete, three new files were created in the specified
+output folder.
+• The Test_apo.xlsx file.
+• The Test_apo.h5 file.
+• The Training_results.tif file.
 
 Since each training process results in slightly different models, we cannot
-directly compare your results to ours. However, if the three files were created
-in the “DL_Track_US_example/tests/model_training” folder, the DL_Track_US
-package works properly model training! Yipiee!
+directly compare your results to ours. However, if the three files were
+created in the “DL_Track_US_example/tests/model_training” folder, the
+DL_Track_US package works properly model training!
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 17
 
 Closing remarks
 Thanks for checking out the DL_Track_US python package test instructions. We
 sincerely hope that all tests were successful and you were also able to enjoy it
 a bit. Moreover, we hope our instructions were clear, concise and easy to
-follow when you have worked through the DL_Track_US_turorial.pdf file
-before. In case something was not clearly illustrated at some point, please let
+follow. In case something was not clearly illustrated at some point, please let
 us know. Don’t hesitate to report this in the Q&A section in the DL_Track_US
 discussion_forum. Otherwise, you can contact us by email at
-paul.ritsche@unibas.ch, but we would prefer the other way.
+paul.ritsche@unibas.ch.
 
-06.04.2023
+26.04.2023
 
 DL_Track_US python package - Tests
 
 18
```

### Comparing `dl_track_us-0.1.2.1/LICENSE` & `dl_track_us-0.1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_track_us-0.1.2.1/README_Pypi.md` & `dl_track_us-0.1.2.2/README_Pypi.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # DL_Track_US
 
 [![Documentation Status](https://readthedocs.org/projects/dltrack/badge/?version=latest)](https://dltrack.readthedocs.io/en/latest/?badge=latest)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7805896.svg)](https://doi.org/10.5281/zenodo.7805896)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7866598.svg)](https://doi.org/10.5281/zenodo.7866598)
 
 The DL_Track_US package provides an easy to use graphical user interface (GUI) for deep learning based analysis of muscle architectural parameters from longitudinal ultrasonography images of human lower limb muscles. Please take a look at our [documentation](https://dltrack.readthedocs.io/en/latest/index.html) for more information.
 This code is based on a previously published [algorithm](https://github.com/njcronin/DL_Track) and replaces it. We have extended the functionalities of the previously proposed code. The previous code will not be updated and future updates will be included in this repository.
 
 ## Getting started
 
 For detailled information about installaion of the DL_Track_US python package we refer you to our [documentation](https://dltrack.readthedocs.io/en/latest/installation.html). There you will finde guidelines not only for the installation procedure of DL_Track_US, but also concerning conda and GPU setup.
@@ -30,8 +30,8 @@
 
 ## Previous research
 
 The previously published [algorithm](https://github.com/njcronin/DL_Track) was developed with the aim to compare the performance of the trained deep learning models with manual analysis of muscle fascicle length, muscle fascicle pennation angle and muscle thickness. The results were presented in a published [preprint](https://arxiv.org/pdf/2009.04790.pdf). The results demonstrated in the article described the DL_Track_US algorithm to be comparable with manual analysis of muscle fascicle length, muscle fascicle pennation angle and muscle thickness in ultrasonography images as well as videos.
 
 ## Community guidelines
 
-Wheter you want to contribute, report a bug or have troubles with the DL_Track_US package, take a look at the provided [instructions](https://dltrack.readthedocs.io/en/latest/contribute.html) how to best do so. You can also contact us via email at paul.ritsche@unibas.ch, but we would prefer you to open a discussion as described in the instructions.
+Wheter you want to contribute, report a bug or have troubles with the DL_Track_US package, take a look at the provided [instructions](https://dltrack.readthedocs.io/en/latest/contribute.html) how to best do so.
```

### Comparing `dl_track_us-0.1.2.1/pyproject.toml` & `dl_track_us-0.1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 444c 5f54 7261 636b 5f55 5322 0d0a   "DL_Track_US"..
 00000070: 7665 7273 696f 6e20 3d20 2230 2e31 2e32  version = "0.1.2
-00000080: 2e31 220d 0a61 7574 686f 7273 203d 205b  .1"..authors = [
+00000080: 2e32 220d 0a61 7574 686f 7273 203d 205b  .2"..authors = [
 00000090: 0d0a 2020 7b20 6e61 6d65 3d22 5061 756c  ..  { name="Paul
 000000a0: 2052 6974 7363 6865 222c 2065 6d61 696c   Ritsche", email
 000000b0: 3d22 7061 756c 2e72 6974 7363 6865 4075  ="paul.ritsche@u
 000000c0: 6e69 6261 732e 6368 2220 7d2c 0d0a 2020  nibas.ch" },..  
 000000d0: 7b20 6e61 6d65 3d22 4f6c 6976 6965 7220  { name="Olivier 
 000000e0: 5365 796e 6e65 7322 2c20 656d 6169 6c3d  Seynnes", email=
 000000f0: 226f 6c69 7669 6572 7340 6e69 682e 6e6f  "oliviers@nih.no
```

### Comparing `dl_track_us-0.1.2.1/PKG-INFO` & `dl_track_us-0.1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DL_Track_US
-Version: 0.1.2.1
+Version: 0.1.2.2
 Summary: Automatic analysis of logitudinal muscle ultrasonography images
 Project-URL: Homepage, https://github.com/PaulRitsche/DL_Track_US
 Project-URL: Bug Tracker, https://github.com/PaulRitsche/DL_Track_US/issues
 Author-email: Paul Ritsche <paul.ritsche@unibas.ch>, Olivier Seynnes <oliviers@nih.no>, Neil Cronin <neil.j.cronin@jyu.fi>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -25,15 +25,15 @@
 Requires-Dist: tensorflow==2.10.0
 Requires-Dist: tqdm==4.64.1
 Description-Content-Type: text/markdown
 
 # DL_Track_US
 
 [![Documentation Status](https://readthedocs.org/projects/dltrack/badge/?version=latest)](https://dltrack.readthedocs.io/en/latest/?badge=latest)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7805896.svg)](https://doi.org/10.5281/zenodo.7805896)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7866598.svg)](https://doi.org/10.5281/zenodo.7866598)
 
 The DL_Track_US package provides an easy to use graphical user interface (GUI) for deep learning based analysis of muscle architectural parameters from longitudinal ultrasonography images of human lower limb muscles. Please take a look at our [documentation](https://dltrack.readthedocs.io/en/latest/index.html) for more information.
 This code is based on a previously published [algorithm](https://github.com/njcronin/DL_Track) and replaces it. We have extended the functionalities of the previously proposed code. The previous code will not be updated and future updates will be included in this repository.
 
 ## Getting started
 
 For detailled information about installaion of the DL_Track_US python package we refer you to our [documentation](https://dltrack.readthedocs.io/en/latest/installation.html). There you will finde guidelines not only for the installation procedure of DL_Track_US, but also concerning conda and GPU setup.
@@ -58,8 +58,8 @@
 
 ## Previous research
 
 The previously published [algorithm](https://github.com/njcronin/DL_Track) was developed with the aim to compare the performance of the trained deep learning models with manual analysis of muscle fascicle length, muscle fascicle pennation angle and muscle thickness. The results were presented in a published [preprint](https://arxiv.org/pdf/2009.04790.pdf). The results demonstrated in the article described the DL_Track_US algorithm to be comparable with manual analysis of muscle fascicle length, muscle fascicle pennation angle and muscle thickness in ultrasonography images as well as videos.
 
 ## Community guidelines
 
-Wheter you want to contribute, report a bug or have troubles with the DL_Track_US package, take a look at the provided [instructions](https://dltrack.readthedocs.io/en/latest/contribute.html) how to best do so. You can also contact us via email at paul.ritsche@unibas.ch, but we would prefer you to open a discussion as described in the instructions.
+Wheter you want to contribute, report a bug or have troubles with the DL_Track_US package, take a look at the provided [instructions](https://dltrack.readthedocs.io/en/latest/contribute.html) how to best do so.
```

