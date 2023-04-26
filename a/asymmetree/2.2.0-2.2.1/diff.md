# Comparing `tmp/asymmetree-2.2.0.tar.gz` & `tmp/asymmetree-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymmetree-2.2.0.tar", last modified: Mon May 30 09:42:31 2022, max compression
+gzip compressed data, was "asymmetree-2.2.1.tar", last modified: Wed Apr 26 19:03:15 2023, max compression
```

## Comparing `asymmetree-2.2.0.tar` & `asymmetree-2.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-30 09:42:31.322447 asymmetree-2.2.0/
--rwxr-xr-x   0 david      (501) staff       (20)    35149 2020-12-12 17:38:31.000000 asymmetree-2.2.0/LICENSE
--rw-r--r--   0 david      (501) staff       (20)     3298 2022-05-30 09:42:31.322568 asymmetree-2.2.0/PKG-INFO
--rwxr-xr-x   0 david      (501) staff       (20)     2721 2022-05-30 09:39:24.000000 asymmetree-2.2.0/README.md
--rw-r--r--   0 david      (501) staff       (20)       85 2022-05-30 09:39:24.000000 asymmetree-2.2.0/pyproject.toml
--rw-r--r--   0 david      (501) staff       (20)      766 2022-05-30 09:42:31.323002 asymmetree-2.2.0/setup.cfg
--rwxr-xr-x   0 david      (501) staff       (20)       99 2022-05-30 09:39:24.000000 asymmetree-2.2.0/setup.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-30 09:42:31.313498 asymmetree-2.2.0/src/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-30 09:42:31.315441 asymmetree-2.2.0/src/asymmetree/
--rwxr-xr-x   0 david      (501) staff       (20)      849 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-30 09:42:31.317503 asymmetree-2.2.0/src/asymmetree/analysis/
--rwxr-xr-x   0 david      (501) staff       (20)    36508 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/analysis/BestMatches.py
--rwxr-xr-x   0 david      (501) staff       (20)    30006 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/analysis/HGT.py
--rwxr-xr-x   0 david      (501) staff       (20)     1033 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/analysis/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-30 09:42:31.318119 asymmetree-2.2.0/src/asymmetree/file_io/
--rw-r--r--   0 david      (501) staff       (20)     4956 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/file_io/SeqFileIO.py
--rw-r--r--   0 david      (501) staff       (20)     1231 2020-12-17 13:04:17.000000 asymmetree-2.2.0/src/asymmetree/file_io/SubstModelIO.py
--rw-r--r--   0 david      (501) staff       (20)       40 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/file_io/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-30 09:42:31.318448 asymmetree-2.2.0/src/asymmetree/genome/
--rw-r--r--   0 david      (501) staff       (20)     9227 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/genome/GenomeSimulation.py
--rw-r--r--   0 david      (501) staff       (20)      501 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/genome/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-30 09:42:31.320020 asymmetree-2.2.0/src/asymmetree/seqevolve/
--rwxr-xr-x   0 david      (501) staff       (20)     3366 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/seqevolve/Alignment.py
--rwxr-xr-x   0 david      (501) staff       (20)    25070 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/seqevolve/EmpiricalModels.py
--rwxr-xr-x   0 david      (501) staff       (20)    13129 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/seqevolve/Evolver.py
--rwxr-xr-x   0 david      (501) staff       (20)     5268 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/seqevolve/EvolvingSequence.py
--rwxr-xr-x   0 david      (501) staff       (20)     4564 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/seqevolve/HetModel.py
--rwxr-xr-x   0 david      (501) staff       (20)     3812 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/seqevolve/IndelModel.py
--rwxr-xr-x   0 david      (501) staff       (20)    10254 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/seqevolve/SubstModel.py
--rwxr-xr-x   0 david      (501) staff       (20)     1443 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/seqevolve/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-30 09:42:31.320781 asymmetree-2.2.0/src/asymmetree/tools/
--rwxr-xr-x   0 david      (501) staff       (20)     6841 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/tools/DistanceCalculation.py
--rwxr-xr-x   0 david      (501) staff       (20)    25633 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/tools/PhyloTreeTools.py
--rw-r--r--   0 david      (501) staff       (20)    10638 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/tools/Sampling.py
--rwxr-xr-x   0 david      (501) staff       (20)       90 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/tools/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-30 09:42:31.321982 asymmetree-2.2.0/src/asymmetree/treeevolve/
--rwxr-xr-x   0 david      (501) staff       (20)    11232 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/treeevolve/DistanceNoise.py
--rwxr-xr-x   0 david      (501) staff       (20)    27457 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/treeevolve/GeneTree.py
--rw-r--r--   0 david      (501) staff       (20)    15156 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/treeevolve/RateHeterogeneity.py
--rwxr-xr-x   0 david      (501) staff       (20)    36416 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/treeevolve/SpeciesTree.py
--rwxr-xr-x   0 david      (501) staff       (20)     1710 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/treeevolve/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-30 09:42:31.322297 asymmetree-2.2.0/src/asymmetree/visualize/
--rwxr-xr-x   0 david      (501) staff       (20)    14871 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/visualize/TreeVis.py
--rwxr-xr-x   0 david      (501) staff       (20)       82 2022-05-30 09:39:24.000000 asymmetree-2.2.0/src/asymmetree/visualize/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-30 09:42:31.316551 asymmetree-2.2.0/src/asymmetree.egg-info/
--rw-r--r--   0 david      (501) staff       (20)     3298 2022-05-30 09:42:31.000000 asymmetree-2.2.0/src/asymmetree.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     1303 2022-05-30 09:42:31.000000 asymmetree-2.2.0/src/asymmetree.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2022-05-30 09:42:31.000000 asymmetree-2.2.0/src/asymmetree.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)       39 2022-05-30 09:42:31.000000 asymmetree-2.2.0/src/asymmetree.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)       11 2022-05-30 09:42:31.000000 asymmetree-2.2.0/src/asymmetree.egg-info/top_level.txt
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-26 19:03:15.662871 asymmetree-2.2.1/
+-rwxr-xr-x   0 david      (501) staff       (20)    35149 2020-12-12 17:38:31.000000 asymmetree-2.2.1/LICENSE
+-rw-r--r--   0 david      (501) staff       (20)     3219 2023-04-26 19:03:15.662953 asymmetree-2.2.1/PKG-INFO
+-rwxr-xr-x   0 david      (501) staff       (20)     2642 2023-04-26 18:58:09.000000 asymmetree-2.2.1/README.md
+-rw-r--r--   0 david      (501) staff       (20)       85 2022-05-30 09:39:24.000000 asymmetree-2.2.1/pyproject.toml
+-rw-r--r--   0 david      (501) staff       (20)      766 2023-04-26 19:03:15.663322 asymmetree-2.2.1/setup.cfg
+-rwxr-xr-x   0 david      (501) staff       (20)       99 2022-05-30 09:39:24.000000 asymmetree-2.2.1/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-26 19:03:15.653904 asymmetree-2.2.1/src/
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-26 19:03:15.655812 asymmetree-2.2.1/src/asymmetree/
+-rwxr-xr-x   0 david      (501) staff       (20)      849 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-26 19:03:15.657719 asymmetree-2.2.1/src/asymmetree/analysis/
+-rwxr-xr-x   0 david      (501) staff       (20)    36508 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/analysis/BestMatches.py
+-rwxr-xr-x   0 david      (501) staff       (20)    30006 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/analysis/HGT.py
+-rwxr-xr-x   0 david      (501) staff       (20)     1033 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/analysis/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-26 19:03:15.658446 asymmetree-2.2.1/src/asymmetree/file_io/
+-rw-r--r--   0 david      (501) staff       (20)     4956 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/file_io/SeqFileIO.py
+-rw-r--r--   0 david      (501) staff       (20)     1231 2020-12-17 13:04:17.000000 asymmetree-2.2.1/src/asymmetree/file_io/SubstModelIO.py
+-rw-r--r--   0 david      (501) staff       (20)       40 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/file_io/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-26 19:03:15.658794 asymmetree-2.2.1/src/asymmetree/genome/
+-rw-r--r--   0 david      (501) staff       (20)     9227 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/genome/GenomeSimulation.py
+-rw-r--r--   0 david      (501) staff       (20)      501 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/genome/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-26 19:03:15.660442 asymmetree-2.2.1/src/asymmetree/seqevolve/
+-rwxr-xr-x   0 david      (501) staff       (20)     3366 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/seqevolve/Alignment.py
+-rwxr-xr-x   0 david      (501) staff       (20)    25070 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/seqevolve/EmpiricalModels.py
+-rwxr-xr-x   0 david      (501) staff       (20)    13129 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/seqevolve/Evolver.py
+-rwxr-xr-x   0 david      (501) staff       (20)     5268 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/seqevolve/EvolvingSequence.py
+-rwxr-xr-x   0 david      (501) staff       (20)     4564 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/seqevolve/HetModel.py
+-rwxr-xr-x   0 david      (501) staff       (20)     3812 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/seqevolve/IndelModel.py
+-rwxr-xr-x   0 david      (501) staff       (20)    10254 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/seqevolve/SubstModel.py
+-rwxr-xr-x   0 david      (501) staff       (20)     1443 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/seqevolve/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-26 19:03:15.661282 asymmetree-2.2.1/src/asymmetree/tools/
+-rwxr-xr-x   0 david      (501) staff       (20)     6841 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/tools/DistanceCalculation.py
+-rwxr-xr-x   0 david      (501) staff       (20)    24148 2023-04-26 18:58:09.000000 asymmetree-2.2.1/src/asymmetree/tools/PhyloTreeTools.py
+-rw-r--r--   0 david      (501) staff       (20)    10630 2023-04-26 18:58:09.000000 asymmetree-2.2.1/src/asymmetree/tools/Sampling.py
+-rwxr-xr-x   0 david      (501) staff       (20)       90 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/tools/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-26 19:03:15.662352 asymmetree-2.2.1/src/asymmetree/treeevolve/
+-rwxr-xr-x   0 david      (501) staff       (20)    11232 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/treeevolve/DistanceNoise.py
+-rwxr-xr-x   0 david      (501) staff       (20)    27457 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/treeevolve/GeneTree.py
+-rw-r--r--   0 david      (501) staff       (20)    15156 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/treeevolve/RateHeterogeneity.py
+-rwxr-xr-x   0 david      (501) staff       (20)    36416 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/treeevolve/SpeciesTree.py
+-rwxr-xr-x   0 david      (501) staff       (20)     1710 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/treeevolve/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-26 19:03:15.662712 asymmetree-2.2.1/src/asymmetree/visualize/
+-rwxr-xr-x   0 david      (501) staff       (20)    14871 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/visualize/TreeVis.py
+-rwxr-xr-x   0 david      (501) staff       (20)       82 2022-05-30 09:39:24.000000 asymmetree-2.2.1/src/asymmetree/visualize/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-26 19:03:15.656694 asymmetree-2.2.1/src/asymmetree.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)     3219 2023-04-26 19:03:15.000000 asymmetree-2.2.1/src/asymmetree.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     1303 2023-04-26 19:03:15.000000 asymmetree-2.2.1/src/asymmetree.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-04-26 19:03:15.000000 asymmetree-2.2.1/src/asymmetree.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)       39 2023-04-26 19:03:15.000000 asymmetree-2.2.1/src/asymmetree.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       11 2023-04-26 19:03:15.000000 asymmetree-2.2.1/src/asymmetree.egg-info/top_level.txt
```

### Comparing `asymmetree-2.2.0/LICENSE` & `asymmetree-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/PKG-INFO` & `asymmetree-2.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asymmetree
-Version: 2.2.0
+Version: 2.2.1
 Summary: Simulation of phylogenetic trees, sequences and genomes
 Home-page: https://github.com/david-schaller/AsymmeTree
 Author: David Schaller
 Author-email: sdavid@bioinf.uni-leipzig.de
 Project-URL: Bug Tracker, https://github.com/david-schaller/AsymmeTree/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AsymmeTree
 ![Logo](resources/images/logo.png)
 
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![pypi version](https://img.shields.io/badge/pypi-v2.2.0-blue.svg)](https://pypi.org/project/asymmetree/)
+[![pypi version](https://img.shields.io/badge/pypi-v2.2.1-blue.svg)](https://pypi.org/project/asymmetree/)
 
 AsymmeTree is an open-source Python library for the simulation and analysis of phylogenetic scenarios.
 It includes a simulator for species and gene trees with heterogeneous evolution rates, nucleotide and amino acid sequences with or without indels, as well as whole genomes/proteomes.
 
 Moreover, it includes a matplotlib-based visualization of the simulated trees as well as tools for the extraction of information from the simulated scenarios such as orthology, best matches, and xenology.
 
 The library is primarily designed to explore and validate mathematical concepts, and to test inference methods for various steps on the way to more realistically-available data, i.e., dated gene trees, additive distances of gene sets, noisy distances and finally sequences.
@@ -58,11 +58,11 @@
 A user manual with example code can be found in the [Wiki](https://github.com/david-schaller/AsymmeTree/wiki/Manual).
 AsymmeTree is divided into several subpackages and modules, see also the following [documentation](https://david-schaller.github.io/docs/asymmetree/) generated from the source code.
 
 ## Citation
 
 If you use AsymmeTree in your project or code from it, please consider citing:
 
-* **Stadler, P. F., Geiß, M., Schaller, D., López Sánchez, A., González Laffitte, M., Valdivia, D., Hellmuth, M., and Hernández Rosales, M. (2020) From pairs of most similar sequences to phylogenetic best matches. Algorithms for Molecular Biology. doi: 10.1186/s13015-020-00165-2.**
+* **David Schaller, Marc Hellmuth, and Peter F. Stadler. AsymmeTree: A Flexible Python Package for the Simulation of Complex Gene Family Histories. Software 2022, 1(3), 276-298; doi: 10.3390/software1030013**
 
 Please report any bugs and questions in the [Issues](https://github.com/david-schaller/AsymmeTree/issues) section.
 Also, feel free to make suggestions for improvement and/or new functionalities.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asymmetree-2.2.0/README.md` & `asymmetree-2.2.1/src/asymmetree.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,27 @@
+Metadata-Version: 2.1
+Name: asymmetree
+Version: 2.2.1
+Summary: Simulation of phylogenetic trees, sequences and genomes
+Home-page: https://github.com/david-schaller/AsymmeTree
+Author: David Schaller
+Author-email: sdavid@bioinf.uni-leipzig.de
+Project-URL: Bug Tracker, https://github.com/david-schaller/AsymmeTree/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # AsymmeTree
 ![Logo](resources/images/logo.png)
 
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![pypi version](https://img.shields.io/badge/pypi-v2.2.0-blue.svg)](https://pypi.org/project/asymmetree/)
+[![pypi version](https://img.shields.io/badge/pypi-v2.2.1-blue.svg)](https://pypi.org/project/asymmetree/)
 
 AsymmeTree is an open-source Python library for the simulation and analysis of phylogenetic scenarios.
 It includes a simulator for species and gene trees with heterogeneous evolution rates, nucleotide and amino acid sequences with or without indels, as well as whole genomes/proteomes.
 
 Moreover, it includes a matplotlib-based visualization of the simulated trees as well as tools for the extraction of information from the simulated scenarios such as orthology, best matches, and xenology.
 
 The library is primarily designed to explore and validate mathematical concepts, and to test inference methods for various steps on the way to more realistically-available data, i.e., dated gene trees, additive distances of gene sets, noisy distances and finally sequences.
@@ -43,11 +58,11 @@
 A user manual with example code can be found in the [Wiki](https://github.com/david-schaller/AsymmeTree/wiki/Manual).
 AsymmeTree is divided into several subpackages and modules, see also the following [documentation](https://david-schaller.github.io/docs/asymmetree/) generated from the source code.
 
 ## Citation
 
 If you use AsymmeTree in your project or code from it, please consider citing:
 
-* **Stadler, P. F., Geiß, M., Schaller, D., López Sánchez, A., González Laffitte, M., Valdivia, D., Hellmuth, M., and Hernández Rosales, M. (2020) From pairs of most similar sequences to phylogenetic best matches. Algorithms for Molecular Biology. doi: 10.1186/s13015-020-00165-2.**
+* **David Schaller, Marc Hellmuth, and Peter F. Stadler. AsymmeTree: A Flexible Python Package for the Simulation of Complex Gene Family Histories. Software 2022, 1(3), 276-298; doi: 10.3390/software1030013**
 
 Please report any bugs and questions in the [Issues](https://github.com/david-schaller/AsymmeTree/issues) section.
 Also, feel free to make suggestions for improvement and/or new functionalities.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asymmetree-2.2.0/setup.cfg` & `asymmetree-2.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = asymmetree
-version = 2.2.0
+version = 2.2.1
 author = David Schaller
 author_email = sdavid@bioinf.uni-leipzig.de
 description = Simulation of phylogenetic trees, sequences and genomes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/david-schaller/AsymmeTree
 project_urls =
```

### Comparing `asymmetree-2.2.0/src/asymmetree/__init__.py` & `asymmetree-2.2.1/src/asymmetree/__init__.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/analysis/BestMatches.py` & `asymmetree-2.2.1/src/asymmetree/analysis/BestMatches.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/analysis/HGT.py` & `asymmetree-2.2.1/src/asymmetree/analysis/HGT.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/analysis/__init__.py` & `asymmetree-2.2.1/src/asymmetree/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/file_io/SeqFileIO.py` & `asymmetree-2.2.1/src/asymmetree/file_io/SeqFileIO.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/file_io/SubstModelIO.py` & `asymmetree-2.2.1/src/asymmetree/file_io/SubstModelIO.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/genome/GenomeSimulation.py` & `asymmetree-2.2.1/src/asymmetree/genome/GenomeSimulation.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/seqevolve/Alignment.py` & `asymmetree-2.2.1/src/asymmetree/seqevolve/Alignment.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/seqevolve/EmpiricalModels.py` & `asymmetree-2.2.1/src/asymmetree/seqevolve/EmpiricalModels.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/seqevolve/Evolver.py` & `asymmetree-2.2.1/src/asymmetree/seqevolve/Evolver.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/seqevolve/EvolvingSequence.py` & `asymmetree-2.2.1/src/asymmetree/seqevolve/EvolvingSequence.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/seqevolve/HetModel.py` & `asymmetree-2.2.1/src/asymmetree/seqevolve/HetModel.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/seqevolve/IndelModel.py` & `asymmetree-2.2.1/src/asymmetree/seqevolve/IndelModel.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/seqevolve/SubstModel.py` & `asymmetree-2.2.1/src/asymmetree/seqevolve/SubstModel.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/seqevolve/__init__.py` & `asymmetree-2.2.1/src/asymmetree/seqevolve/__init__.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/tools/DistanceCalculation.py` & `asymmetree-2.2.1/src/asymmetree/tools/DistanceCalculation.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/tools/PhyloTreeTools.py` & `asymmetree-2.2.1/src/asymmetree/tools/PhyloTreeTools.py`

 * *Files 14% similar despite different names*

```diff
@@ -426,14 +426,59 @@
      else:
          # assign colors completely randomly
          for leaf in leaves:
              leaf.reconc = random.choice(colors)
              
      return tree
  
+
+def random_ultrametric_timing(tree, inplace=False, adjust_distances=False):
+    """Generate a random ultrametric timing for the tree.
+    
+    Parameters
+    ----------
+    tree : Tree
+        The tree for which a random timing shall be generated.
+    inplace : bool, optional
+        If True, the input tree is modified, otherwise a copy is returned.
+        The default is False.
+    adjust_distances : bool, optional
+        If True, also adjust the dist attribute of the tree nodes to match the
+        differences of the tstamp values. The default is False.
+    
+    Returns
+    -------
+    Tree
+        A random tree whose nodes have tstamp attributes that represent the
+        generated random ultrametric timing.
+    """
+    
+    if not inplace:
+        tree = tree.copy()
+        
+    for v in tree.preorder():
+        if not v.children:
+            v.tstamp = 0.0
+        elif not v.parent:
+            v.tstamp = 1.0
+        else:                               # random walk to a leaf
+            pos = v                         # current position
+            length = 0                      # path length |P|
+            while pos.children:
+                length += 1
+                pos = pos.children[np.random.randint(len(pos.children))]
+            v.tstamp = (
+                v.parent.tstamp * (1 - 2 * np.random.uniform() / (length+1))
+            )
+    
+    if adjust_distances:
+        distance_from_timing(tree)
+             
+    return tree
+ 
     
 def phylo_tree_attributes(tree, inplace=True):
     """Add the attributes for a phylogentic tree if not already set.
     
     Parameters
     ----------
     tree : Tree
@@ -715,97 +760,42 @@
     Do not use this function for serialization and reloading Tree
     objects. Use the `serialize()` function instead.
     Labels and reconciliations that are integer numbers are converted to int.
     The reconciliations (if present in <...> in the string) are parsed as
     strings and need to be converted to integers afterwards if necessary.
     """
     
-    # label<reconc>:distance
-    label_col_dist_regex = re.compile(r"'?([a-zA-Z0-9_]*)'?<(.*)>:(-?[0-9]*\.?[0-9]*[Ee]?-?[0-9]+)")
-    # label<reconc>
-    label_col_regex = re.compile(r"'?([a-zA-Z0-9_]*)'?<(.*)>")
-    # label:distance
-    label_dist_regex = re.compile(r"'?([a-zA-Z0-9_]*)'?:(-?[0-9]*\.?[0-9]*[Ee]?-?[0-9]+)")
-    
     def to_int(item):
         """Trys to convert the string into int."""
         
         return int(item) if item.isdigit() else item
     
-    def parse_subtree(subroot, subtree_string):
-        """Recursive function to parse the subtrees."""
+    tree = Tree.parse_newick(newick)
+    
+    # regex for notation label<reconc>
+    label_col_regex = re.compile(r"'?([a-zA-Z0-9_]*)'?<(.*)>")
+    
+    for node in tree.preorder():
         
-        children = split_children(subtree_string)
-        for child in children:
-            node = TreeNode(event='')
-            subroot.add_child(node)
-            end = -1
-            if child[0] == '(':                                 # the child has subtrees
-                end = child.rfind(')')
-                if end == -1:
-                    raise ValueError('invalid Newick string')
-                parse_subtree(node, child[1:end])               # recursive call 'parse_subtree'
-            child = child[end+1:].strip()
-            label_col_dist = label_col_dist_regex.match(child)
-            if label_col_dist:                                  # CASE 1: label<reconc>:distance
-                node.label = to_int(label_col_dist.group(1))
-                node.reconc = to_int(label_col_dist.group(2))
-                node.dist = float(label_col_dist.group(3))
-            else:
-                label_col = label_col_regex.match(child)
-                label_dist = label_dist_regex.match(child)
-                if label_col:                                   # CASE 2: label<reconc>
-                    node.label = to_int(label_col.group(1))
-                    node.reconc = to_int(label_col.group(2))
-                    node.dist = 1.0
-                elif label_dist:                                # CASE 3: label:distance
-                    node.label = to_int(label_dist.group(1))
-                    node.reconc = None
-                    node.dist = float(label_dist.group(2))
-                else:                                           # CASE 4: label
-                    node.label = to_int(child)
-                    node.reconc = None
-                    node.dist = 1.0
-            # reconc is a tuple
-            if node.reconc and isinstance(node.reconc, str) and node.reconc.find('-') != -1:
-                split_reconc = node.reconc.split('-')
-                node.reconc = (to_int(split_reconc[0]),
-                              to_int(split_reconc[1]))
-                    
-    def split_children(child_string):
-        """Splits a given string by all ',' that are not enclosed by parentheses."""
-        
-        stack = 0
-        children = []
-        current = ""
-        for c in child_string:
-            if (stack == 0) and c == ',':
-                children.append(current)
-                current = ""
-            elif c == '(':
-                stack += 1
-                current += c
-            elif c == ')':
-                if stack <= 0:
-                    raise ValueError('invalid Newick string')
-                stack -= 1
-                current += c
-            else:
-                current += c
-        children.append(current.strip())
-        return children
-    
-    if not isinstance(newick, str):
-        raise TypeError("Newick parser needs a 'str' as input")
-    end = newick.find(";")
-    if end != -1:
-        newick = newick[:end]
-    temp_root = TreeNode(event='')
-    parse_subtree(temp_root, newick)
-    if temp_root.children:
-        root = temp_root.children[0]
-        root.dist = 0.0                 # set distance of the root to 0
-        root.detach()                   # remove the parent temp_root
-                                        # (important for non-recursive to_newick2)
-        return Tree(root)
-    else:
-        raise ValueError('invalid Newick string')
+        node.event = ''
+        
+        if not hasattr(node, 'dist'):
+            node.dist = 1.0
+        
+        label = str(node.label)
+        
+        label_col = label_col_regex.match(label)
+        if label_col:
+            node.label = to_int(label_col.group(1))
+            node.reconc = to_int(label_col.group(2))
+        else:
+            node.reconc = None
+        
+        # reconc is a tuple
+        if (node.reconc and 
+            isinstance(node.reconc, str) and 
+            node.reconc.find('-') != -1):
+            
+            a, b = node.reconc.split('-')
+            node.reconc = (to_int(a), to_int(b))
+    
+    return tree
```

### Comparing `asymmetree-2.2.0/src/asymmetree/tools/Sampling.py` & `asymmetree-2.2.1/src/asymmetree/tools/Sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from scipy.special import zeta
 
 
 __author__ = 'David Schaller'
 
 
 class Sampler:
-    """Campling from from a variety of distributions."""
+    """Sampling from a variety of distributions."""
     
     def __init__(self, params, minimum=None, maximum=None, discrete=False,
                  shift=0):
         """
         Parameters
         ----------
         params : float or tuple
@@ -20,15 +20,15 @@
             available options.
         minimum : float, optional
             Minimum value to be sampled. The default is None.
         maximum : float, optional
             Maximum value to be sampled. The default is None.
         discrete : bool, optional
             If True, round sampled values in case of a continuous
-                distribution. The default is False.
+            distribution. The default is False.
         shift : float, optional
             Shift distribution along x-axis. The default is 0, i.e., the
             distribution is not shifted.
         """
         
         self._params = params
         self._discrete = discrete
@@ -287,8 +287,8 @@
     def _draw_neg_bin(self):
         
         while True:
             x = np.random.negative_binomial(self._r, 1 - self._q) + self._shift
                 
             if ((not self._min or x >= self.min) and
                 (not self._max or x <= self._max)):
-                return x
+                return x
```

### Comparing `asymmetree-2.2.0/src/asymmetree/treeevolve/DistanceNoise.py` & `asymmetree-2.2.1/src/asymmetree/treeevolve/DistanceNoise.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/treeevolve/GeneTree.py` & `asymmetree-2.2.1/src/asymmetree/treeevolve/GeneTree.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/treeevolve/RateHeterogeneity.py` & `asymmetree-2.2.1/src/asymmetree/treeevolve/RateHeterogeneity.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/treeevolve/SpeciesTree.py` & `asymmetree-2.2.1/src/asymmetree/treeevolve/SpeciesTree.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/treeevolve/__init__.py` & `asymmetree-2.2.1/src/asymmetree/treeevolve/__init__.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree/visualize/TreeVis.py` & `asymmetree-2.2.1/src/asymmetree/visualize/TreeVis.py`

 * *Files identical despite different names*

### Comparing `asymmetree-2.2.0/src/asymmetree.egg-info/PKG-INFO` & `asymmetree-2.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,12 @@
-Metadata-Version: 2.1
-Name: asymmetree
-Version: 2.2.0
-Summary: Simulation of phylogenetic trees, sequences and genomes
-Home-page: https://github.com/david-schaller/AsymmeTree
-Author: David Schaller
-Author-email: sdavid@bioinf.uni-leipzig.de
-Project-URL: Bug Tracker, https://github.com/david-schaller/AsymmeTree/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AsymmeTree
 ![Logo](resources/images/logo.png)
 
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![pypi version](https://img.shields.io/badge/pypi-v2.2.0-blue.svg)](https://pypi.org/project/asymmetree/)
+[![pypi version](https://img.shields.io/badge/pypi-v2.2.1-blue.svg)](https://pypi.org/project/asymmetree/)
 
 AsymmeTree is an open-source Python library for the simulation and analysis of phylogenetic scenarios.
 It includes a simulator for species and gene trees with heterogeneous evolution rates, nucleotide and amino acid sequences with or without indels, as well as whole genomes/proteomes.
 
 Moreover, it includes a matplotlib-based visualization of the simulated trees as well as tools for the extraction of information from the simulated scenarios such as orthology, best matches, and xenology.
 
 The library is primarily designed to explore and validate mathematical concepts, and to test inference methods for various steps on the way to more realistically-available data, i.e., dated gene trees, additive distances of gene sets, noisy distances and finally sequences.
@@ -58,11 +43,11 @@
 A user manual with example code can be found in the [Wiki](https://github.com/david-schaller/AsymmeTree/wiki/Manual).
 AsymmeTree is divided into several subpackages and modules, see also the following [documentation](https://david-schaller.github.io/docs/asymmetree/) generated from the source code.
 
 ## Citation
 
 If you use AsymmeTree in your project or code from it, please consider citing:
 
-* **Stadler, P. F., Geiß, M., Schaller, D., López Sánchez, A., González Laffitte, M., Valdivia, D., Hellmuth, M., and Hernández Rosales, M. (2020) From pairs of most similar sequences to phylogenetic best matches. Algorithms for Molecular Biology. doi: 10.1186/s13015-020-00165-2.**
+* **David Schaller, Marc Hellmuth, and Peter F. Stadler. AsymmeTree: A Flexible Python Package for the Simulation of Complex Gene Family Histories. Software 2022, 1(3), 276-298; doi: 10.3390/software1030013**
 
 Please report any bugs and questions in the [Issues](https://github.com/david-schaller/AsymmeTree/issues) section.
 Also, feel free to make suggestions for improvement and/or new functionalities.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asymmetree-2.2.0/src/asymmetree.egg-info/SOURCES.txt` & `asymmetree-2.2.1/src/asymmetree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

