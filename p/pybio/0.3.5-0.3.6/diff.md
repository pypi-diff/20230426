# Comparing `tmp/pybio-0.3.5.tar.gz` & `tmp/pybio-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybio-0.3.5.tar", last modified: Tue Apr 25 18:41:11 2023, max compression
+gzip compressed data, was "pybio-0.3.6.tar", last modified: Wed Apr 26 11:02:01 2023, max compression
```

## Comparing `pybio-0.3.5.tar` & `pybio-0.3.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 gregor    (1028) urpp      (1011)        0 2023-04-25 18:41:11.221349 pybio-0.3.5/
--rw-r--r--   0 gregor    (1028) urpp      (1011)     8895 2023-04-25 18:41:11.221349 pybio-0.3.5/PKG-INFO
--rw-r--r--   0 gregor    (1028) urpp      (1011)     8664 2023-04-25 16:49:23.000000 pybio-0.3.5/README.md
-drwxr-xr-x   0 gregor    (1028) urpp      (1011)        0 2023-04-25 18:41:11.217349 pybio-0.3.5/pybio/
--rw-r--r--   0 gregor    (1028) urpp      (1011)     7928 2023-04-25 18:17:54.000000 pybio-0.3.5/pybio/__init__.py
-drwxr-xr-x   0 gregor    (1028) urpp      (1011)        0 2023-04-25 18:41:11.221349 pybio-0.3.5/pybio/config/
--rw-r--r--   0 gregor    (1028) urpp      (1011)     2060 2023-04-25 18:12:49.000000 pybio-0.3.5/pybio/config/__init__.py
-drwxr-xr-x   0 gregor    (1028) urpp      (1011)        0 2023-04-25 18:41:11.221349 pybio-0.3.5/pybio/core/
--rw-r--r--   0 gregor    (1028) urpp      (1011)       98 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/core/__init__.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)    26695 2023-04-25 18:40:31.000000 pybio-0.3.5/pybio/core/genomes.py
-drwxr-xr-x   0 gregor    (1028) urpp      (1011)        0 2023-04-25 18:41:11.221349 pybio-0.3.5/pybio/data/
--rw-r--r--   0 gregor    (1028) urpp      (1011)      877 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/Bam.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)    16391 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/Bedgraph.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)     4675 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/Bedgraph2.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)     1912 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/Fasta.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)     1244 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/Fastq.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)     1591 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/Gene.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)      177 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/GeneFeature.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)     3238 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/Gff3.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)     2777 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/Gtf.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)      186 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/Sequence.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)      906 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/Sissrs.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)      956 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/TabReader.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)     2019 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/Wig.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)     2168 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/data/__init__.py
-drwxr-xr-x   0 gregor    (1028) urpp      (1011)        0 2023-04-25 18:41:11.221349 pybio-0.3.5/pybio/expression/
--rw-r--r--   0 gregor    (1028) urpp      (1011)     8831 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/expression/__init__.py
-drwxr-xr-x   0 gregor    (1028) urpp      (1011)        0 2023-04-25 18:41:11.221349 pybio-0.3.5/pybio/map/
--rw-r--r--   0 gregor    (1028) urpp      (1011)     2257 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/map/STAR.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)      131 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/map/__init__.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)     1438 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/map/bowtie.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)      580 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/map/nano.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)     1061 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/map/sege.py
-drwxr-xr-x   0 gregor    (1028) urpp      (1011)        0 2023-04-25 18:41:11.221349 pybio-0.3.5/pybio/maths/
--rw-r--r--   0 gregor    (1028) urpp      (1011)      974 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/maths/__init__.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)    37335 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/maths/pstat.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)   151400 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/maths/stats.py
-drwxr-xr-x   0 gregor    (1028) urpp      (1011)        0 2023-04-25 18:41:11.221349 pybio-0.3.5/pybio/path/
--rw-r--r--   0 gregor    (1028) urpp      (1011)      347 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/path/__init__.py
--rwxr-xr-x   0 gregor    (1028) urpp      (1011)     5075 2023-04-25 18:15:29.000000 pybio-0.3.5/pybio/pybio
--rw-r--r--   0 gregor    (1028) urpp      (1011)      100 2023-04-25 18:40:38.000000 pybio-0.3.5/pybio/pybio.config.example
-drwxr-xr-x   0 gregor    (1028) urpp      (1011)        0 2023-04-25 18:41:11.221349 pybio-0.3.5/pybio/sequence/
--rw-r--r--   0 gregor    (1028) urpp      (1011)     5566 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/sequence/__init__.py
-drwxr-xr-x   0 gregor    (1028) urpp      (1011)        0 2023-04-25 18:41:11.221349 pybio-0.3.5/pybio/utils/
--rw-r--r--   0 gregor    (1028) urpp      (1011)    10199 2023-04-14 17:12:19.000000 pybio-0.3.5/pybio/utils/__init__.py
--rw-r--r--   0 gregor    (1028) urpp      (1011)        6 2023-04-25 18:41:03.000000 pybio-0.3.5/pybio/version
-drwxr-xr-x   0 gregor    (1028) urpp      (1011)        0 2023-04-25 18:41:11.221349 pybio-0.3.5/pybio.egg-info/
--rw-r--r--   0 gregor    (1028) urpp      (1011)     8895 2023-04-25 18:41:11.000000 pybio-0.3.5/pybio.egg-info/PKG-INFO
--rw-r--r--   0 gregor    (1028) urpp      (1011)      892 2023-04-25 18:41:11.000000 pybio-0.3.5/pybio.egg-info/SOURCES.txt
--rw-r--r--   0 gregor    (1028) urpp      (1011)        1 2023-04-25 18:41:11.000000 pybio-0.3.5/pybio.egg-info/dependency_links.txt
--rw-r--r--   0 gregor    (1028) urpp      (1011)        1 2023-04-15 19:56:14.000000 pybio-0.3.5/pybio.egg-info/not-zip-safe
--rw-r--r--   0 gregor    (1028) urpp      (1011)       32 2023-04-25 18:41:11.000000 pybio-0.3.5/pybio.egg-info/requires.txt
--rw-r--r--   0 gregor    (1028) urpp      (1011)        6 2023-04-25 18:41:11.000000 pybio-0.3.5/pybio.egg-info/top_level.txt
--rw-r--r--   0 gregor    (1028) urpp      (1011)       38 2023-04-25 18:41:11.221349 pybio-0.3.5/setup.cfg
--rw-r--r--   0 gregor    (1028) urpp      (1011)      949 2023-04-25 16:49:23.000000 pybio-0.3.5/setup.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.891271 pybio-0.3.6/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8857 2023-04-26 11:02:01.890771 pybio-0.3.6/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8626 2023-04-26 07:30:50.000000 pybio-0.3.6/README.md
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.854579 pybio-0.3.6/pybio/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     7792 2023-04-26 10:49:44.000000 pybio-0.3.6/pybio/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.861527 pybio-0.3.6/pybio/config/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2060 2023-04-26 07:30:50.000000 pybio-0.3.6/pybio/config/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.863365 pybio-0.3.6/pybio/core/
+-rw-rw-r--   0 rotg     (2023757) games       (20)       98 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/core/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    26823 2023-04-26 07:30:50.000000 pybio-0.3.6/pybio/core/genomes.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.876113 pybio-0.3.6/pybio/data/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      877 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Bam.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    16391 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Bedgraph.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     4675 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Bedgraph2.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1912 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Fasta.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1244 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Fastq.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1591 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Gene.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      177 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/GeneFeature.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3238 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Gff3.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2777 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Gtf.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      186 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Sequence.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      906 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Sissrs.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      956 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/TabReader.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2019 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Wig.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2168 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.877376 pybio-0.3.6/pybio/expression/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8831 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/expression/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.882805 pybio-0.3.6/pybio/map/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2257 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/map/STAR.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      131 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/map/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1438 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/map/bowtie.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      580 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/map/nano.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1061 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/map/sege.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.885662 pybio-0.3.6/pybio/maths/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      974 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/maths/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    37335 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/maths/pstat.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)   151400 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/maths/stats.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.887907 pybio-0.3.6/pybio/path/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      347 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/path/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5203 2023-04-26 10:51:08.000000 pybio-0.3.6/pybio/pybio
+-rw-rw-r--   0 rotg     (2023757) games       (20)      100 2023-04-26 07:30:50.000000 pybio-0.3.6/pybio/pybio.config.example
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.888689 pybio-0.3.6/pybio/sequence/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5566 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/sequence/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.889739 pybio-0.3.6/pybio/utils/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    10199 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/utils/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-04-26 11:01:54.000000 pybio-0.3.6/pybio/version
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.860600 pybio-0.3.6/pybio.egg-info/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8857 2023-04-26 11:02:01.856244 pybio-0.3.6/pybio.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)      892 2023-04-26 11:02:01.856810 pybio-0.3.6/pybio.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-26 11:02:01.857955 pybio-0.3.6/pybio.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-18 08:10:15.000000 pybio-0.3.6/pybio.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) games       (20)       32 2023-04-26 11:02:01.860144 pybio-0.3.6/pybio.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-04-26 11:02:01.860911 pybio-0.3.6/pybio.egg-info/top_level.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-04-26 11:02:01.891362 pybio-0.3.6/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) games       (20)      949 2023-04-17 08:00:52.000000 pybio-0.3.6/setup.py
```

### Comparing `pybio-0.3.5/PKG-INFO` & `pybio-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,8 @@
-Metadata-Version: 2.1
-Name: pybio
-Version: 0.3.5
-Summary: pybio genomics
-Home-page: https://github.com/grexor/pybio
-Author: Gregor Rot
-Author-email: gregor.rot@gmail.com
-Keywords: pybio,bioinformatics
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-
+<picture><img src="media/pybio.png" width="70"/></picture>
 ## pybio: basic genomics toolset
 
 pybio is a Python framework for handling genomics operations and a direct interface to Ensembl genomes.
 
 Downloading an Ensembl genome+annotation takes one line: `pybio genome homo_sapiens`.
 
 Features include genome+annotation download from Ensembl and processing with STAR and salmon, support of Fasta, Fastq, bedGraph and other file formats, motif sequence searches, and specific APA feautes like alternative polyadenylation site-pair classification (same-exon, skipped-exon, composite-exon) and more.
@@ -20,16 +10,15 @@
 ## Contents
 
 * [Installation](#installation)
 * [Quick Start](#Quick-Start)
 * [Documentation](#documentation)
   * [Downloading Ensembl genomes](#downloading-Ensembl-genomes)
   * [Retrieving genomic sequences](#retrieving-genomic-sequences)
-  * [Annotate genomic position](#annotate-genomic-position)
-  * [Importing genome annotation](#importing-genome-annotation)
+  * [Annotating genomic positions](#annotating-genomic-positions)
   * [File formats](#file-formats)
   * [Genomic Coordinates](#Genomic-Coordinates)
 * [Authors](#authors)
 * [Reporting problems](#reporting-problems)
 
 ### Installation
 
@@ -60,15 +49,15 @@
 Searching a genomic position for features is easy in python, for example:
 
 ```
 import pybio
 genes, transcripts, exons, UTR5, UTR3 = annotate("homo_sapiens", "1", "+", 11012344)
 ```
 
-This will return a list of feature objects (genes, transctipts, exons, 3'-UTR and 5'-UTR) (check [core/genomes.py](core/genomes.py) classes to see details of these objects).
+This will return a list of feature objects (genes, transctipts, exons, 3'-UTR and 5'-UTR) (check [pybio/core/genomes.py](pybio/core/genomes.py) classes to see details of these objects).
 
 If you would like to know all genes that span the provided position, you could then write:
 
 ```
 for gene in genes:
    print(gene.gene_id, gene.gene_name, gene.start, gene.stop)
 ```
@@ -180,15 +169,15 @@
 seq = pybio.core.genomes.seq("homo_sapiens", "1", "+", 450000, -20, 20)
 ```
 
 The above command fetches the chr 1 sequence from 450000-20..450000+20, the resulting sequence is of length 41, `TACCCTGATTCTGAAACGAAAAAGCTTTACAAAATCCAAGA`.
 
 #### Annotating genomic positions
 
-Given a genomic position, we can quickly retrieve the gene, transcript, exon and utr5/3 information at the given position. If there are several features (genes, transcripts, exons, UTR regions) at the specified position, they are all returned.
+Given a genomic position, we can quickly retrieve the gene, transcript, exon and utr5/3 information at the given position. If there are several features (genes, transcripts, exons, UTR regions) at the specified position, they are all reported by pybio.
 
 ```
 # annotate position
 genes, transcripts, exons, utr5, utr3 = pybio.genomes.annotate("hg38", "1", "+", 11012344)
 
 # print all genes that cover the position
 for gene in genes:
@@ -198,15 +187,15 @@
 The above command would return:
 
 ```
 [pybio] loading genome annotation for homo_sapiens with Ensembl version 109
 ENSG00000120948, TARDBP, 11012343, 11030527
 ```
 
-You can also easily access all transcripts of each gene with `gene.transcripts` and all exons of each transcript with `transcript.exons`.
+We can also easily access all transcripts of each gene with `gene.transcripts` and all exons of each transcript with `transcript.exons`.
 
 #### Dependencies
 
 Basic dependencies include [pysam](https://pysam.readthedocs.io/en/latest/api.html), [numpy](https://numpy.org/) and [samtools](http://www.htslib.org) and should be installed automatically by pip when you install pybio over `pip install pybio`.
 
 Optional dependencies include [STAR](https://github.com/alexdobin/STAR) and [salmon](https://combine-lab.github.io/salmon/getting_started/) if you would like to build genome/transcriptome indices and align reads.
```

### Comparing `pybio-0.3.5/README.md` & `pybio-0.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,18 @@
-<picture><img src="media/pybio.png" width="70"/></picture>
+Metadata-Version: 2.1
+Name: pybio
+Version: 0.3.6
+Summary: pybio genomics
+Home-page: https://github.com/grexor/pybio
+Author: Gregor Rot
+Author-email: gregor.rot@gmail.com
+Keywords: pybio,bioinformatics
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+
 ## pybio: basic genomics toolset
 
 pybio is a Python framework for handling genomics operations and a direct interface to Ensembl genomes.
 
 Downloading an Ensembl genome+annotation takes one line: `pybio genome homo_sapiens`.
 
 Features include genome+annotation download from Ensembl and processing with STAR and salmon, support of Fasta, Fastq, bedGraph and other file formats, motif sequence searches, and specific APA feautes like alternative polyadenylation site-pair classification (same-exon, skipped-exon, composite-exon) and more.
@@ -10,16 +20,15 @@
 ## Contents
 
 * [Installation](#installation)
 * [Quick Start](#Quick-Start)
 * [Documentation](#documentation)
   * [Downloading Ensembl genomes](#downloading-Ensembl-genomes)
   * [Retrieving genomic sequences](#retrieving-genomic-sequences)
-  * [Annotate genomic position](#annotate-genomic-position)
-  * [Importing genome annotation](#importing-genome-annotation)
+  * [Annotating genomic positions](#annotating-genomic-positions)
   * [File formats](#file-formats)
   * [Genomic Coordinates](#Genomic-Coordinates)
 * [Authors](#authors)
 * [Reporting problems](#reporting-problems)
 
 ### Installation
 
@@ -50,15 +59,15 @@
 Searching a genomic position for features is easy in python, for example:
 
 ```
 import pybio
 genes, transcripts, exons, UTR5, UTR3 = annotate("homo_sapiens", "1", "+", 11012344)
 ```
 
-This will return a list of feature objects (genes, transctipts, exons, 3'-UTR and 5'-UTR) (check [core/genomes.py](core/genomes.py) classes to see details of these objects).
+This will return a list of feature objects (genes, transctipts, exons, 3'-UTR and 5'-UTR) (check [pybio/core/genomes.py](pybio/core/genomes.py) classes to see details of these objects).
 
 If you would like to know all genes that span the provided position, you could then write:
 
 ```
 for gene in genes:
    print(gene.gene_id, gene.gene_name, gene.start, gene.stop)
 ```
@@ -170,15 +179,15 @@
 seq = pybio.core.genomes.seq("homo_sapiens", "1", "+", 450000, -20, 20)
 ```
 
 The above command fetches the chr 1 sequence from 450000-20..450000+20, the resulting sequence is of length 41, `TACCCTGATTCTGAAACGAAAAAGCTTTACAAAATCCAAGA`.
 
 #### Annotating genomic positions
 
-Given a genomic position, we can quickly retrieve the gene, transcript, exon and utr5/3 information at the given position. If there are several features (genes, transcripts, exons, UTR regions) at the specified position, they are all returned.
+Given a genomic position, we can quickly retrieve the gene, transcript, exon and utr5/3 information at the given position. If there are several features (genes, transcripts, exons, UTR regions) at the specified position, they are all reported by pybio.
 
 ```
 # annotate position
 genes, transcripts, exons, utr5, utr3 = pybio.genomes.annotate("hg38", "1", "+", 11012344)
 
 # print all genes that cover the position
 for gene in genes:
@@ -188,15 +197,15 @@
 The above command would return:
 
 ```
 [pybio] loading genome annotation for homo_sapiens with Ensembl version 109
 ENSG00000120948, TARDBP, 11012343, 11030527
 ```
 
-You can also easily access all transcripts of each gene with `gene.transcripts` and all exons of each transcript with `transcript.exons`.
+We can also easily access all transcripts of each gene with `gene.transcripts` and all exons of each transcript with `transcript.exons`.
 
 #### Dependencies
 
 Basic dependencies include [pysam](https://pysam.readthedocs.io/en/latest/api.html), [numpy](https://numpy.org/) and [samtools](http://www.htslib.org) and should be installed automatically by pip when you install pybio over `pip install pybio`.
 
 Optional dependencies include [STAR](https://github.com/alexdobin/STAR) and [salmon](https://combine-lab.github.io/salmon/getting_started/) if you would like to build genome/transcriptome indices and align reads.
```

### Comparing `pybio-0.3.5/pybio/__init__.py` & `pybio-0.3.6/pybio/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,24 +19,19 @@
 import pybio.sequence
 import pybio.core
 
 pybio_path = os.path.abspath(__file__)
 pybio_folder = os.path.dirname(pybio_path)
 version = open(os.path.join(pybio_folder, "version"), "rt").readlines()[0].replace("\n", "").replace("\r", "")
 
-print(f"[pybio] v{version}, https://github.com/grexor/pybio")
-
 # initialize path module
 pybio.config.init()
 pybio.path.init()
 pybio.core.genomes.init()
 
-print(f"[pybio] genomes folder: {pybio.config.genomes_folder}")
-print()
-
 def genome_download(species, genome_version, args):
     print(f"[pybio genome_download] species {species} and version {genome_version}")
     genomes_ready_fname = os.path.join(pybio.config.genomes_folder, "genomes_ready.json")
     if os.path.exists(genomes_ready_fname):
         genomes_ready = json.load(open(genomes_ready_fname, "rt"))
     else:
         genomes_ready = {}
```

### Comparing `pybio-0.3.5/pybio/config/__init__.py` & `pybio-0.3.6/pybio/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/core/genomes.py` & `pybio-0.3.6/pybio/core/genomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -258,16 +258,16 @@
         fasta_url = f"{ftp_address}/release-{ensembl_version}/fasta/{species}/dna/{species_capital}.{assembly}.dna.toplevel.fa.gz"
     # no? download nonchromosomal
     if not url_exists(fasta_url):
         fasta_url = f"{ftp_address}/release-{ensembl_version}/fasta/{species}/dna/{species_capital}.{assembly}.dna.nonchromosomal.fa.gz"
     print(fasta_url)
     script = """
 cd {gdir}
-rm {species}.assembly.{genome_version}/*
-mkdir {species}.assembly.{genome_version}
+rm {species}.assembly.{genome_version}/* >/dev/null 2>&1
+mkdir {species}.assembly.{genome_version} >/dev/null 2>&1
 cd {species}.assembly.{genome_version}
 wget {fasta_url} -O {species}.fasta.gz
 gunzip -f {species}.fasta.gz
 python3 -c "import pybio; pybio.data.Fasta('{species}.fasta').split()"
 """
 
     # download FASTA and split
@@ -292,16 +292,16 @@
     fasta_url = f"{ftp_address}/release-{ensembl_version}/gtf/{species}/{species_capital}.{assembly}.{ensembl_version}.chr.gtf.gz"
     # no? download the toplevel
     if not url_exists(fasta_url):
         fasta_url = f"{ftp_address}/release-{ensembl_version}/gtf/{species}/{species_capital}.{assembly}.{ensembl_version}.gtf.gz"
 
     script = """
 cd {gdir}
-rm {species}.annotation.{genome_version}/*
-mkdir {species}.annotation.{genome_version}
+rm {species}.annotation.{genome_version}/* >/dev/null 2>&1
+mkdir {species}.annotation.{genome_version} >/dev/null 2>&1
 cd {species}.annotation.{genome_version}
 # https://www.biostars.org/p/279235/#279238
 wget {fasta_url} -O {species}.gtf.gz
 """
     # download GTF
     print(f"[pybio.core.genomes] download annotation GTF for {species}.{genome_version}")
     command = script.format(fasta_url=fasta_url, gdir=pybio.config.genomes_folder, species=species, genome_version=genome_version)
@@ -310,16 +310,16 @@
 def star_index(species, genome_version):
     species_capital = species.capitalize()
     assembly = species_db[species]["assembly"]
     ensembl_version = genome_version.replace("ensembl", "")
     ensembl_version = ensembl_version.replace("genomes", "")
     script = """
 cd {gdir}
-rm {species}.assembly.{genome_version}.star/*
-mkdir {species}.assembly.{genome_version}.star
+rm {species}.assembly.{genome_version}.star/* >/dev/null 2>&1
+mkdir {species}.assembly.{genome_version}.star >/dev/null 2>&1
 cd {species}.assembly.{genome_version}.star
 gunzip ../{species}.annotation.{genome_version}/{species}.gtf.gz
 STAR --runMode genomeGenerate --genomeSAindexNbases {genomeSAindexNbases} --genomeDir ../{species}.assembly.{genome_version}.star --genomeFastaFiles ../{species}.assembly.{genome_version}/{species}.fasta --runThreadN 4 --sjdbGTFfile ../{species}.annotation.{genome_version}/{species}.gtf
 gzip -f ../{species}.annotation.{genome_version}/{species}.gtf
 """
     fasta_file = f"{pybio.config.genomes_folder}/{species}.assembly.{genome_version}/{species}.fasta"
     fasta_size = os.path.getsize(fasta_file)
@@ -335,16 +335,16 @@
     ftp_address = providers_ftp[species_db[species]["provider"]]
     subfolder = species_db[species]["provider_subfolder"]
     if subfolder!="":
         ftp_address = f"{ftp_address}/{subfolder}"
     
     script = """
 cd {gdir}
-rm {species}.transcripts.{genome_version}/*
-mkdir {species}.transcripts.{genome_version}
+rm {species}.transcripts.{genome_version}/* >/dev/null 2>&1
+mkdir {species}.transcripts.{genome_version} >/dev/null 2>&1
 cd {species}.transcripts.{genome_version}
 wget {ftp_address}/release-{ensembl_version}/fasta/{species}/cdna/{species_capital}.{assembly}.cdna.all.fa.gz -O {species}.transcripts.fasta.gz
 
 cd {gdir}
 salmon index -t {species}.transcripts.{genome_version}/{species}.transcripts.fasta.gz -i {species}.transcripts.{genome_version}.salmon
 """
     command = script.format(ftp_address=ftp_address, gdir=pybio.config.genomes_folder, species=species, species_capital=species_capital, assembly=assembly, ensembl_version=ensembl_version, genome_version=genome_version)
```

### Comparing `pybio-0.3.5/pybio/data/Bam.py` & `pybio-0.3.6/pybio/data/Bam.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/data/Bedgraph.py` & `pybio-0.3.6/pybio/data/Bedgraph.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/data/Bedgraph2.py` & `pybio-0.3.6/pybio/data/Bedgraph2.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/data/Fasta.py` & `pybio-0.3.6/pybio/data/Fasta.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/data/Fastq.py` & `pybio-0.3.6/pybio/data/Fastq.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/data/Gene.py` & `pybio-0.3.6/pybio/data/Gene.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/data/Gff3.py` & `pybio-0.3.6/pybio/data/Gff3.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/data/Gtf.py` & `pybio-0.3.6/pybio/data/Gtf.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/data/Sissrs.py` & `pybio-0.3.6/pybio/data/Sissrs.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/data/TabReader.py` & `pybio-0.3.6/pybio/data/TabReader.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/data/Wig.py` & `pybio-0.3.6/pybio/data/Wig.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/data/__init__.py` & `pybio-0.3.6/pybio/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/expression/__init__.py` & `pybio-0.3.6/pybio/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/map/STAR.py` & `pybio-0.3.6/pybio/map/STAR.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/map/bowtie.py` & `pybio-0.3.6/pybio/map/bowtie.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/map/nano.py` & `pybio-0.3.6/pybio/map/nano.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/map/sege.py` & `pybio-0.3.6/pybio/map/sege.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/maths/__init__.py` & `pybio-0.3.6/pybio/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/maths/pstat.py` & `pybio-0.3.6/pybio/maths/pstat.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/maths/stats.py` & `pybio-0.3.6/pybio/maths/stats.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/pybio` & `pybio-0.3.6/pybio/pybio`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,20 @@
 Example:
 
 $ pybio genome homo_sapiens
 
 The above will download the latest Ensembl human genome.
 """
 
+print(f"[pybio] v{pybio.version}, https://github.com/grexor/pybio")
+print(f"[pybio] genomes folder: {pybio.config.genomes_folder}")
+print()
+
 if args.version:
-    print(f"Version: v{pybio.version}")
+    sys.exit(0)
 
 def is_known_species(species):
     species = species.lower()
     return species in pybio.core.genomes.species_db
 
 def determine_species(species):
     provided_species = species
@@ -43,40 +47,42 @@
         if display_name.find(species)!=-1 or species_id.find(species)!=-1:
             potential_hits.append((len(display_name), species_id, display_name))
     potential_hits.sort()
     if len(potential_hits)>0:
         return potential_hits
     return []
 
+def display_potential_hits(potential_hits, search_text):
+    print(f"We found {len(potential_hits)} genome hits for your provided genome species `{search_text}`.\nPlease choose the species genome you would like to download:\n")
+    for hit in potential_hits:
+        print(f"Species = '{hit[1]}', display name = '{hit[2]}'")
+    if len(potential_hits)>0:
+        print(f"\nFor example, to download the first hit from the list above, you could write:\n")
+        print(f"$ pybio genome {potential_hits[0][1]}")
+        print()
+    sys.exit(1)
+
 if len(args.commands)>0:
 
     if args.commands[0]=="species":
         if len(args.commands)>1:
-            search = args.commands[1]
-            os.system(f"cat {pybio.config.genomes_folder}/genome_species.tab | grep {search}")
-        else:
-            os.system(f"cat {pybio.config.genomes_folder}/genome_species.tab")
+            potential_hits = determine_species(args.commands[1])
+            display_potential_hits(potential_hits, args.commands[1])
 
     if args.commands[0]=="genome":
         if len(args.commands)==1:
             print("All genomes data stored at: " + pybio.config.genomes_folder)
             print(help_genome)
             sys.exit()
         species = args.commands[1]
         known_species = is_known_species(species)
         if not known_species:
             potential_hits = determine_species(species)
             if len(potential_hits)>1:
-                print(f"We found >1 genome hits for your provided genome species `{species}`.\nPlease choose the species genome you would like to download:\n")
-                for hit in potential_hits:
-                    print(f"Species = '{hit[1]}', display name = '{hit[2]}'")
-                print(f"\nFor example, to download the first hit from the list above, you could write:\n")
-                print(f"$ pybio genome {potential_hits[0][1]}")
-                print()
-                sys.exit(1)
+                display_potential_hits(potential_hits, species)
             elif len(potential_hits)==1:
                 species = potential_hits[0][1]
         if args.genome_version!=None:
             genome_version = args.genome_version
         else:
             try:
                 genome_version = args.commands[2]
```

### Comparing `pybio-0.3.5/pybio/sequence/__init__.py` & `pybio-0.3.6/pybio/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio/utils/__init__.py` & `pybio-0.3.6/pybio/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/pybio.egg-info/PKG-INFO` & `pybio-0.3.6/pybio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybio
-Version: 0.3.5
+Version: 0.3.6
 Summary: pybio genomics
 Home-page: https://github.com/grexor/pybio
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: pybio,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -20,16 +20,15 @@
 ## Contents
 
 * [Installation](#installation)
 * [Quick Start](#Quick-Start)
 * [Documentation](#documentation)
   * [Downloading Ensembl genomes](#downloading-Ensembl-genomes)
   * [Retrieving genomic sequences](#retrieving-genomic-sequences)
-  * [Annotate genomic position](#annotate-genomic-position)
-  * [Importing genome annotation](#importing-genome-annotation)
+  * [Annotating genomic positions](#annotating-genomic-positions)
   * [File formats](#file-formats)
   * [Genomic Coordinates](#Genomic-Coordinates)
 * [Authors](#authors)
 * [Reporting problems](#reporting-problems)
 
 ### Installation
 
@@ -60,15 +59,15 @@
 Searching a genomic position for features is easy in python, for example:
 
 ```
 import pybio
 genes, transcripts, exons, UTR5, UTR3 = annotate("homo_sapiens", "1", "+", 11012344)
 ```
 
-This will return a list of feature objects (genes, transctipts, exons, 3'-UTR and 5'-UTR) (check [core/genomes.py](core/genomes.py) classes to see details of these objects).
+This will return a list of feature objects (genes, transctipts, exons, 3'-UTR and 5'-UTR) (check [pybio/core/genomes.py](pybio/core/genomes.py) classes to see details of these objects).
 
 If you would like to know all genes that span the provided position, you could then write:
 
 ```
 for gene in genes:
    print(gene.gene_id, gene.gene_name, gene.start, gene.stop)
 ```
@@ -180,15 +179,15 @@
 seq = pybio.core.genomes.seq("homo_sapiens", "1", "+", 450000, -20, 20)
 ```
 
 The above command fetches the chr 1 sequence from 450000-20..450000+20, the resulting sequence is of length 41, `TACCCTGATTCTGAAACGAAAAAGCTTTACAAAATCCAAGA`.
 
 #### Annotating genomic positions
 
-Given a genomic position, we can quickly retrieve the gene, transcript, exon and utr5/3 information at the given position. If there are several features (genes, transcripts, exons, UTR regions) at the specified position, they are all returned.
+Given a genomic position, we can quickly retrieve the gene, transcript, exon and utr5/3 information at the given position. If there are several features (genes, transcripts, exons, UTR regions) at the specified position, they are all reported by pybio.
 
 ```
 # annotate position
 genes, transcripts, exons, utr5, utr3 = pybio.genomes.annotate("hg38", "1", "+", 11012344)
 
 # print all genes that cover the position
 for gene in genes:
@@ -198,15 +197,15 @@
 The above command would return:
 
 ```
 [pybio] loading genome annotation for homo_sapiens with Ensembl version 109
 ENSG00000120948, TARDBP, 11012343, 11030527
 ```
 
-You can also easily access all transcripts of each gene with `gene.transcripts` and all exons of each transcript with `transcript.exons`.
+We can also easily access all transcripts of each gene with `gene.transcripts` and all exons of each transcript with `transcript.exons`.
 
 #### Dependencies
 
 Basic dependencies include [pysam](https://pysam.readthedocs.io/en/latest/api.html), [numpy](https://numpy.org/) and [samtools](http://www.htslib.org) and should be installed automatically by pip when you install pybio over `pip install pybio`.
 
 Optional dependencies include [STAR](https://github.com/alexdobin/STAR) and [salmon](https://combine-lab.github.io/salmon/getting_started/) if you would like to build genome/transcriptome indices and align reads.
```

### Comparing `pybio-0.3.5/pybio.egg-info/SOURCES.txt` & `pybio-0.3.6/pybio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybio-0.3.5/setup.py` & `pybio-0.3.6/setup.py`

 * *Files identical despite different names*

