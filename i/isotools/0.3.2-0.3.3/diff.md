# Comparing `tmp/isotools-0.3.2.tar.gz` & `tmp/isotools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isotools-0.3.2.tar", last modified: Tue Dec 20 13:56:13 2022, max compression
+gzip compressed data, was "isotools-0.3.3.tar", last modified: Tue Apr 25 11:57:25 2023, max compression
```

## Comparing `isotools-0.3.2.tar` & `isotools-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-sr-x   0     2263      542        0 2022-12-20 13:56:13.000000 isotools-0.3.2/
--rw-rw----   0     2263      542     8454 2022-12-16 16:19:29.000000 isotools-0.3.2/CHANGELOG.md
--rw-r--r--   0     2263      542     1069 2021-07-05 21:13:24.000000 isotools-0.3.2/LICENSE.txt
--rw-r--r--   0     2263      542       66 2021-07-06 21:43:48.000000 isotools-0.3.2/MANIFEST.in
--rw-r--r--   0     2263      542     3682 2022-12-20 13:56:13.000000 isotools-0.3.2/PKG-INFO
--rw-r--r--   0     2263      542     3094 2022-07-25 20:40:02.000000 isotools-0.3.2/README.md
--rw-rw----   0     2263      542        6 2022-12-20 13:41:09.000000 isotools-0.3.2/VERSION.txt
--rw-r--r--   0     2263      542      499 2021-11-03 16:29:14.000000 isotools-0.3.2/pyproject.toml
--rw-rw----   0     2263      542      139 2022-10-21 15:40:11.000000 isotools-0.3.2/requirements.txt
--rw-rw----   0     2263      542     1101 2022-12-20 13:56:13.000000 isotools-0.3.2/setup.cfg
--rw-r--r--   0     2263      542       69 2022-03-15 10:42:16.000000 isotools-0.3.2/setup.py
-drwxr-sr-x   0     2263      542        0 2022-12-20 13:56:03.000000 isotools-0.3.2/src/
-drwxr-sr-x   0     2263      542        0 2022-12-20 13:56:10.000000 isotools-0.3.2/src/isotools/
--rw-r-----   0     2263      542     1392 2022-12-14 16:19:11.000000 isotools-0.3.2/src/isotools/__init__.py
--rw-rw----   0     2263      542    35998 2022-12-16 16:12:04.000000 isotools-0.3.2/src/isotools/_gene_plots.py
--rw-rw----   0     2263      542    16755 2022-12-14 16:24:18.000000 isotools-0.3.2/src/isotools/_transcriptome_filter.py
--rw-rw----   0     2263      542    90024 2022-10-21 15:40:11.000000 isotools-0.3.2/src/isotools/_transcriptome_io.py
--rw-rw----   0     2263      542    45649 2022-12-16 14:07:05.000000 isotools-0.3.2/src/isotools/_transcriptome_stats.py
--rw-rw----   0     2263      542    17812 2022-10-21 15:40:11.000000 isotools-0.3.2/src/isotools/_utils.py
--rw-r--r--   0     2263      542     1816 2021-11-08 07:31:42.000000 isotools-0.3.2/src/isotools/decorators.py
--rw-rw----   0     2263      542    21136 2022-12-20 13:55:47.000000 isotools-0.3.2/src/isotools/domains.py
--rw-rw----   0     2263      542    43553 2022-12-12 16:35:12.000000 isotools-0.3.2/src/isotools/gene.py
--rw-r-----   0     2263      542    19483 2022-12-12 16:17:26.000000 isotools-0.3.2/src/isotools/plots.py
--rw-r-----   0     2263      542    19824 2022-12-12 16:17:26.000000 isotools-0.3.2/src/isotools/run_isotools.py
--rw-r-----   0     2263      542     3791 2022-08-30 17:56:01.000000 isotools-0.3.2/src/isotools/short_read.py
--rwxrwx---   0     2263      542    58360 2022-12-09 16:21:18.000000 isotools-0.3.2/src/isotools/splice_graph.py
--rw-rw----   0     2263      542    11241 2022-10-21 15:40:11.000000 isotools-0.3.2/src/isotools/transcriptome.py
-drwxr-sr-x   0     2263      542        0 2022-12-20 13:56:12.000000 isotools-0.3.2/src/isotools.egg-info/
--rw-r-----   0     2263      542     3682 2022-12-20 13:56:01.000000 isotools-0.3.2/src/isotools.egg-info/PKG-INFO
--rw-r-----   0     2263      542      721 2022-12-20 13:56:02.000000 isotools-0.3.2/src/isotools.egg-info/SOURCES.txt
--rw-r-----   0     2263      542        1 2022-12-20 13:56:01.000000 isotools-0.3.2/src/isotools.egg-info/dependency_links.txt
--rw-r-----   0     2263      542       60 2022-12-20 13:56:01.000000 isotools-0.3.2/src/isotools.egg-info/entry_points.txt
--rw-r-----   0     2263      542      193 2022-12-20 13:56:02.000000 isotools-0.3.2/src/isotools.egg-info/requires.txt
--rw-r-----   0     2263      542        9 2022-12-20 13:56:02.000000 isotools-0.3.2/src/isotools.egg-info/top_level.txt
+drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-04-25 11:57:25.748769 isotools-0.3.3/
+-rw-rw----   0 lienhard  (2263) 42grp      (542)     8837 2023-04-20 10:09:55.000000 isotools-0.3.3/CHANGELOG.md
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)     1069 2021-07-05 21:13:24.000000 isotools-0.3.3/LICENSE.txt
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)       66 2021-07-06 21:43:48.000000 isotools-0.3.3/MANIFEST.in
+-rw-r-----   0 lienhard  (2263) 42grp      (542)     3682 2023-04-25 11:57:25.757769 isotools-0.3.3/PKG-INFO
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)     3094 2022-07-25 20:40:02.000000 isotools-0.3.3/README.md
+-rw-rw----   0 lienhard  (2263) 42grp      (542)        6 2023-04-25 11:54:34.000000 isotools-0.3.3/VERSION.txt
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)      499 2021-11-03 16:29:14.000000 isotools-0.3.3/pyproject.toml
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)      144 2022-12-20 14:36:28.000000 isotools-0.3.3/requirements.txt
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)     1106 2023-04-25 11:57:25.815769 isotools-0.3.3/setup.cfg
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)       69 2022-03-15 10:42:16.000000 isotools-0.3.3/setup.py
+drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-04-25 11:57:23.572777 isotools-0.3.3/src/
+drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-04-25 11:57:25.345771 isotools-0.3.3/src/isotools/
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)     1392 2022-12-20 14:05:25.000000 isotools-0.3.3/src/isotools/__init__.py
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)    35998 2022-12-20 14:05:26.000000 isotools-0.3.3/src/isotools/_gene_plots.py
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)    16950 2023-04-25 11:54:19.000000 isotools-0.3.3/src/isotools/_transcriptome_filter.py
+-rw-rw----   0 lienhard  (2263) 42grp      (542)    92705 2023-04-25 11:55:17.000000 isotools-0.3.3/src/isotools/_transcriptome_io.py
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)    45711 2023-04-20 09:20:25.000000 isotools-0.3.3/src/isotools/_transcriptome_stats.py
+-rw-rw----   0 lienhard  (2263) 42grp      (542)    18257 2023-02-21 16:14:10.000000 isotools-0.3.3/src/isotools/_utils.py
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)     1816 2021-11-08 07:31:42.000000 isotools-0.3.3/src/isotools/decorators.py
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)    21716 2023-04-25 11:55:14.000000 isotools-0.3.3/src/isotools/domains.py
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)    46312 2023-04-20 09:21:31.000000 isotools-0.3.3/src/isotools/gene.py
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)    19493 2023-02-27 10:02:46.000000 isotools-0.3.3/src/isotools/plots.py
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)    19824 2022-12-20 14:05:28.000000 isotools-0.3.3/src/isotools/run_isotools.py
+-rw-r-----   0 lienhard  (2263) 42grp      (542)     3791 2022-08-30 17:56:01.000000 isotools-0.3.3/src/isotools/short_read.py
+-rwxr-xr-x   0 lienhard  (2263) 42grp      (542)    58449 2023-02-21 14:29:36.000000 isotools-0.3.3/src/isotools/splice_graph.py
+-rw-rw----   0 lienhard  (2263) 42grp      (542)    11241 2022-10-21 15:40:11.000000 isotools-0.3.3/src/isotools/transcriptome.py
+drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-04-25 11:57:25.708770 isotools-0.3.3/src/isotools.egg-info/
+-rw-r-----   0 lienhard  (2263) 42grp      (542)     3682 2023-04-25 11:57:23.000000 isotools-0.3.3/src/isotools.egg-info/PKG-INFO
+-rw-r-----   0 lienhard  (2263) 42grp      (542)      721 2023-04-25 11:57:23.000000 isotools-0.3.3/src/isotools.egg-info/SOURCES.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)        1 2023-04-25 11:57:23.000000 isotools-0.3.3/src/isotools.egg-info/dependency_links.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)       60 2023-04-25 11:57:23.000000 isotools-0.3.3/src/isotools.egg-info/entry_points.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)      198 2023-04-25 11:57:23.000000 isotools-0.3.3/src/isotools.egg-info/requires.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)        9 2023-04-25 11:57:23.000000 isotools-0.3.3/src/isotools.egg-info/top_level.txt
```

### Comparing `isotools-0.3.2/CHANGELOG.md` & `isotools-0.3.3/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Change Log
 
 ## TODO: ideas, issues and planed extensions or changes that are not yet implemented
 * optimize add_qc_metrics for run after new samples have been added - should not recompute everything
 * planned new feature: during import of long reads, (optionally) correct for short exon alignment issues. 
 * separate new read import and classification of isoforms.
 
+## [0.3.3]
+* fixed bug in filter_ref_transcripts with no query
+* export gtf with long read transcripts as well uncovered as reference transcripts
+* fix warning in plot_diff_results
+* changed export to rMATS: events report complete flanking exons of top covered isoform
+* fixed bug with transcript_id_col parameter in add_sample_from_csv
+* fixed handling of interpro protein domains
+
 ## [0.3.2]
 * restructured tutorials
 * new feature: add domains to differential splicing result tables.
 * new feature: min_coverage and max_coverage for iter_genes function.
 
 ## [0.3.1]
 * new feature: add protein domains from 3 different sources and depict them with Gene.plot_domains()
```

### Comparing `isotools-0.3.2/LICENSE.txt` & `isotools-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `isotools-0.3.2/PKG-INFO` & `isotools-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isotools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Framework for the analysis of long read transcriptome sequencing data
 Home-page: https://github.com/MatthiasLienhard/isotools
 Author: Matthias Lienhard
 Author-email: lienhard@molgen.mpg.de
 Project-URL: Bug Tracker, https://github.com/MatthiasLienhard/isotools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `isotools-0.3.2/README.md` & `isotools-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `isotools-0.3.2/setup.cfg` & `isotools-0.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	tqdm
 	intervaltree
 	matplotlib
 	seaborn
 	biopython
 	pysam
 	umap-learn
-	sklearn
+	scikit-learn
 	scipy
 	statsmodels
 	pyhmmer
 	requests
 
 [options.packages.find]
 where = src
```

### Comparing `isotools-0.3.2/src/isotools/__init__.py` & `isotools-0.3.3/src/isotools/__init__.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.2/src/isotools/_gene_plots.py` & `isotools-0.3.3/src/isotools/_gene_plots.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.2/src/isotools/_transcriptome_filter.py` & `isotools-0.3.3/src/isotools/_transcriptome_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,16 @@
     if not any(old):
         logger.error('filter tag %s not found', tag)
 
 
 def add_filter(self, tag, expression, context='transcript', update=False):
     '''Defines a new filter for gene, transcripts and reference transcripts.
 
-    The provided expressions is evaluated during filtering in the provided context.
+    The provided expressions is evaluated during filtering in the provided context, when specified in a query string of a function that supports filtering.
+    Importantly, filtering does not modify the original data; rather, it is only applied when specifying the query string.
     For examples, see the default filter definitions isotools.DEFAULT_GENE_FILTER,
     isotools.DEFAULT_TRANSCRIPT_FILTER and isotools.DEFAULT_REF_TRANSCRIPT_FILTER.
 
     :param tag: Unique tag identifer for this filter. Must be a single word.
     :param expression: Expression to be evaluated on gene, transcript, or reference transcript.
     :param context: The context for the filter expression, either "gene", "transcript" or "reference".
     :param update: If set, the already present definition of the provided tag gets overwritten.'''
```

### Comparing `isotools-0.3.2/src/isotools/_transcriptome_io.py` & `isotools-0.3.3/src/isotools/_transcriptome_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 # from numpy.lib.function_base import percentile, quantile
 import pandas as pd
 from os import path
 from intervaltree import IntervalTree, Interval
 from collections.abc import Iterable
+from collections import Counter
 from pysam import TabixFile, AlignmentFile, FastaFile
 from tqdm import tqdm
 from contextlib import ExitStack
 from .short_read import Coverage
 from ._utils import junctions_from_cigar, splice_identical, is_same_gene, has_overlap, get_overlap, pairwise, \
     cigar_string2tuples, rc, get_intersects, _find_splice_sites, _get_overlap, get_quantiles  # , _get_exonic_region
 from .gene import Gene
@@ -125,25 +126,25 @@
 
     if transcript_id_col is None:
         if 'transcript_id' in cov_tab.columns:
             pass
         elif 'gene_id' in cov_tab.columns and 'transcript_nr' in cov_tab.columns:
             cov_tab['transcript_id'] = cov_tab.gene_id+'_'+cov_tab.transcript_nr.astype(str)
         else:
-            raise ValueError('"transcript_id_cols" not specified, and coverage table does not contain "transcript_id", nor "gene_id" and "transcript_nr"')
-        transcript_id_cols = 'transcript_id'
+            raise ValueError('"transcript_id_col" not specified, and coverage table does not contain "transcript_id", nor "gene_id" and "transcript_nr"')
+        transcript_id_col = 'transcript_id'
     elif isinstance(transcript_id_col, list):
         assert all(c in cov_tab for c in transcript_id_col), 'missing specified transcript_id_col'
         cov_tab['transcript_id'] = ['_'.join(str(v) for v in row.values()) for _, row in cov_tab[transcript_id_col].iterrows()]
-        transcript_id_cols = 'transcript_id'
+        transcript_id_col = 'transcript_id'
     else:
         assert transcript_id_col in cov_tab, 'missing specified transcript_id_col'
         cov_tab['transcript_id'] = cov_tab[transcript_id_col]
     known_sa = set(samples).intersection(self.samples)
-    assert transcript_id_cols == 'transcript_id'  # could be optimized, but code is easier when the id column always is transcript_id
+    assert transcript_id_col == 'transcript_id'  # could be optimized, but code is easier when the id column always is transcript_id
     assert not known_sa, 'Attempt to add known samples: %s' % known_sa
     # cov_tab.set_index('transcript_id')
     # assert cov_tab.index.is_unique, 'ambigous transcript ids in %s' % coverage_csv_file
     # check sample properties
     if sample_properties is None:
         sample_properties = {sa: {} for sa in samples}
     elif isinstance(sample_properties, pd.DataFrame):
@@ -257,18 +258,19 @@
 def add_sample_from_bam(self, fn, sample_name=None, barcode_file=None, fuzzy_junction=5, add_chromosomes=True, min_mapqual=0,
                         min_align_fraction=.75, chimeric_mincov=2, min_exonic_ref_coverage=.25, use_satag=False, save_readnames=False, progress_bar=True,
                         **kwargs):
     '''Imports expressed transcripts from bam and adds it to the 'Transcriptome' object.
 
     :param fn: The bam filename of the new sample
     :param sample_name: Name of the new sample. If specified, all reads are assumed to belong to this sample.
-    :param barcode_file: For barcoded samples, ath to file with assignment of sequencing barcodes to sample names.
+    :param barcode_file: For barcoded samples, a file with assignment of sequencing barcodes to sample names.
         This file should be a tab seperated text file with two columns: the barcode and the sample name
         Barcodes not listed in this file will be ignored.
-        If sample_name is specified in addition to bacode_file, it will be used as a prefix
+        If sample_name is specified in addition to bacode_file, it will be used as a prefix.
+        Barcodes will be read from the XC tag of the bam file.
     :param fuzzy_junction: maximum size for fuzzy junction correction
     :param add_chromosomes: If True, genes from chromosomes which are not in the Transcriptome yet are added.
     :param min_mapqual: Minimum mapping quality of the read to be considdered.
         A mapping quality of 0 usually means ambigous alignment.
     :param min_align_fraction: Minimum fraction of the read sequence matching the reference.
     :param chimeric_mincov: Minimum number of reads for a chimeric transcript to be considered
     :param min_exonic_ref_coverage: Minimal fraction of exonic overlap to assign to reference transcript if no splice junctions match.
@@ -1474,21 +1476,23 @@
             for setA, setB, nodeX, nodeY, splice_type in seg_graph.find_splice_bubbles(types=('ES', '3AS', '5AS', 'IR', 'ME')):
                 if not reference:
                     junction_cov = g.coverage[np.ix_(sidx, setA)].sum(1)
                     total_cov = g.coverage[np.ix_(sidx, setB)].sum(1) + junction_cov
                     if total_cov.sum() < min_total or (not min_alt_fraction < junction_cov.sum() / total_cov.sum() < 1 - min_alt_fraction):
                         continue
                 st = types[splice_type]
-                lines = alt_splice_export(setA, setB, nodeX, nodeY, st, seg_graph, g, count[st])
+                lines = alt_splice_export(setA, setB, nodeX, nodeY, st, reference, g, count[st])
                 if lines:
                     count[st] += len(lines)
                     fh[st].write('\n'.join(('\t'.join(str(field) for field in line) for line in lines)) + '\n')
 
 
-def _miso_alt_splice_export(setA, setB, nodeX, nodeY, st, seg_graph, g, offset):
+def _miso_alt_splice_export(setA, setB, nodeX, nodeY, st, reference, g, offset):
+    seg_graph = g.ref_segment_graph if reference else g.segment_graph
+
     event_id = f'{g.chrom}:{seg_graph[nodeX].end}-{seg_graph[nodeY].start}_st'
     # TODO: Mutually exclusives extend beyond nodeY - and have potentially multiple A "mRNAs"
     # TODO: is it possible to extend exons at nodeX and Y - if all/"most" tr from setA and B agree?
     # if st=='ME':
     #    nodeY=min(seg_graph._pas[setA])
     lines = []
     lines.append([g.chrom, st, 'gene', seg_graph[nodeX].start, seg_graph[nodeY].end, '.', g.strand, '.', f'ID={event_id};gene_name={g.name};gene_id={g.id}'])
@@ -1506,50 +1510,89 @@
         lines[0][3] = min(lines[0][3], lines[-1][3])
         lines[0][4] = max(lines[0][4], lines[-1][4])
         for j, e in enumerate(exons):
             lines.append((g.chrom, st, 'exon', e[0], e[1], '.', g.strand, '.', f'Parent={event_id}.B{i};ID={event_id}.B{i}.{j}'))
     return lines
 
 
-def _mats_alt_splice_export(setA, setB, nodeX, nodeY, st, seg_graph, g, offset):
+def _mats_alt_splice_export(setA, setB, nodeX, nodeY, st, reference, g, offset,  use_top_isoform=True, use_top_alternative=True):
+    # use_top_isoform and use_top_alternative are ment to simplify the output, in order to not confuse rMATS with to many options
     # 'ID','GeneID','geneSymbol','chr','strand'
     # and ES/EE for the relevant exons
     # in case of 'SE':['skipped', 'upstream', 'downstream'],
     # in case of 'RI':['retained', 'upstream', 'downstream'],
     # in case of 'MXE':['1st','2nd', 'upstream', 'downstream'],
     # in case of 'A3SS':['long','short', 'flanking'],
     # in case of 'A5SS':['long','short', 'flanking']}
+    # upstream and downstream/ 1st/snd are with respect to the genome strand
+    # offset is the event id offset
+    seg_graph = g.ref_segment_graph if reference else g.segment_graph
+
     lines = []
     if g.chrom[: 3] != 'chr':
         chrom = 'chr' + g.chrom
     else:
         chrom = g.chrom
-    exonsA = ((seg_graph[nodeX].start, seg_graph[nodeX].end), (seg_graph[nodeY].start, seg_graph[nodeY].end))
-    for exonsB in {tuple(seg_graph._get_all_exons(nodeX, nodeY, b_tr)) for b_tr in setB}:
-        exons_sel = None
+    if use_top_isoform:  # use flanking exons from top isoform
+        all_transcript_ids = setA+setB
+        if not reference:
+            # most covered isoform
+            top_isoform = all_transcript_ids[g.coverage[:, all_transcript_ids].sum(0).argmax()]  # top covered isoform across all samples
+            nodeX_start = seg_graph._get_exon_start(top_isoform, nodeX)
+            nodeY_end = seg_graph._get_exon_end(top_isoform, nodeY)
+        else:
+            # for reference: most frequent
+            nodeX_start = Counter([seg_graph._get_exon_start(n, nodeX) for n in all_transcript_ids]).most_common(1)[0][0]
+            nodeY_end = Counter([seg_graph._get_exon_end(n, nodeY) for n in all_transcript_ids]).most_common(1)[0][0]
+
+        exonsA = ((seg_graph[nodeX_start].start, seg_graph[nodeX].end), (seg_graph[nodeY].start, seg_graph[nodeY_end].end))  # flanking/outer "exons" of setA()
+    else:
+        exonsA = ((seg_graph[nodeX].start, seg_graph[nodeX].end), (seg_graph[nodeY].start, seg_graph[nodeY].end))  # flanking/outer "exons" of setA
+
+    # _get_all_exons does not extend the exons beyond the nodeX/Y
+    alternatives = [tuple(seg_graph._get_all_exons(nodeX, nodeY, b_tr)) for b_tr in setB]
+    if use_top_alternative:
+        if reference:
+            c = Counter(alternatives)
+        else:
+            weights = [g.coverage[:, b_tr].sum() for b_tr in setB]
+            c = Counter()
+            for alt, w in zip(alternatives, weights):
+                c.update({alt: w})
+        alternatives = [c.most_common(1)[0][0]]
+    else:
+        alternatives = set(alternatives)
+    for exonsB in alternatives:
+        exons_sel = []
         if st in ['A3SS', 'A5SS'] and len(exonsB) == 2:
-            if exonsA[0][1] == exonsB[0][1]:
-                exons_sel = [exonsB[1], exonsA[1], exonsA[0]]  # long short flanking
-            else:
-                exons_sel = [exonsB[0], exonsA[0], exonsA[1]]  # long short flanking
+            if exonsA[0][1] == exonsB[0][1]:  # A5SS on - strand or A3SS on + strand
+                exons_sel.append([(exonsB[1][0], exonsA[1][1]), exonsA[1], exonsA[0]])  # long short flanking
+            else:  # A5SS on + strand or A3SS on - strand
+                exons_sel.append([(exonsA[0][0], exonsB[0][1]), exonsA[0], exonsA[1]])  # long short flanking
         elif st == 'SE' and len(exonsB) == 3:
-            assert exonsA[0] == exonsB[0] and exonsA[1] == exonsB[2], f'invalid exon skipping {exonsA} vs {exonsB}'  # just to be sure everything is consistent
-            # e_order=(1,0,2) if g.strand=='+' else (1,2,0)
-            e_order = (1, 0, 2)
-            exons_sel = [exonsB[i] for i in e_order]
+            # just to be sure everything is consistent
+            assert exonsA[0][1] == exonsB[0][1] and exonsA[1][0] == exonsB[2][0], f'invalid exon skipping {exonsA} vs {exonsB}'
+            # e_order = (1, 0, 2) if g.strand == '+' else (1, 2, 0)
+            exons_sel.append([exonsB[i] for i in (1, 0, 2)])  # skipped, upstream, downstream
         elif st == 'RI' and len(exonsB) == 1:
-            exons_sel = [exonsB[0], exonsA[0], exonsA[1]]  # if g.strand=='+' else [exonsB[0], exonsA[1], exonsA[0]]
+            exons_sel.append([(exonsA[0][0], exonsA[1][1]), exonsA[0], exonsA[1]])  # retained, upstream, downstream
+            # if g.strand == '+' else [exonsB[0], exonsA[1], exonsA[0]])
         elif st == 'MXE' and len(exonsB) == 3:
             # nodeZ=next(idx for idx,n in enumerate(seg_graph) if n.start==exonsB[-1][0])
-            for exonsA in {tuple(seg_graph._get_all_exons(nodeX, nodeY, a_tr)) for a_tr in setA}:
-                assert len(exonsA) == 3 and exonsA[0] == exonsB[0] and exonsA[2] == exonsB[2]  # should always be true
-                lines.append([f'"{g.id}"', f'"{g.name}"', chrom, g.strand, exonsB[1][0], exonsB[1][1], exonsA[1]
-                             [0], exonsA[1][1], exonsA[0][0], exonsA[0][1], exonsA[2][0], exonsA[2][1]])
-        if exons_sel is not None:
-            lines.append([f'"{g.id}"', f'"{g.name}"', chrom, g.strand] + [pos for e in exons_sel for pos in e])
+            # multiple exonA possibilities, so we need to check all of them
+            for exonsA_ME in {tuple(seg_graph._get_all_exons(nodeX, nodeY, a_tr)) for a_tr in setA}:
+                if len(exonsA_ME) != 3:  # complex events are not possible in rMATS
+                    continue
+                assert exonsA_ME[0] == exonsB[0] and exonsA_ME[2] == exonsB[2]  # should always be true
+                # assert exonsA_ME[0][1] == exonsA[0][1] and exonsA_ME[2][0] == exonsA[1][0]  # should always be true
+                # '1st','2nd', 'upstream', 'downstream'
+                exons_sel.append([exonsB[1], exonsA_ME[1], exonsA[0], exonsA[1]])
+        for exons in exons_sel:  # usually there is only one rMATS event per exonB, but for MXE we may get several
+            # lines.append([f'"{g.id}"', f'"{g.name}"', chrom, g.strand] + [pos for e in exons for pos in ((e[1],e[0]) if g.strand == '-' else e)])
+            lines.append([f'"{g.id}"', f'"{g.name}"', chrom, g.strand] + [pos for e in exons for pos in e])  # no need to reverse the order of exon start/end
     return [[offset + count] + l for count, l in enumerate(lines)]
 
 
 def get_gff_chrom_dict(gff, chromosomes):
     'fetch chromosome ids - in case they use ids in gff for the chormosomes'
     chrom = {}
     for c in gff.contigs:
```

### Comparing `isotools-0.3.2/src/isotools/_transcriptome_stats.py` & `isotools-0.3.3/src/isotools/_transcriptome_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,15 +358,15 @@
     '''Summary statistics for novel alternative splicing.
 
     This function counts the novel alternative splicing events of LRTS isoforms with respect to the reference annotation.
     The result can be depicted by isotools.plots.plot_bar.
 
     :param groups: A dict {group_name:[sample_name_list]} specifying sample groups. If omitted, the samples are analyzed individually.
     :param weight_by_coverage: If True, each transcript is weighted by the coverage.
-    :param min_coverage: Threshold to ignore poorly covered transcripts.
+    :param min_coverage: Threshold to ignore poorly covered transcripts. This parameter gets applied for each sample group seperately.
     :param tr_filter: Filter dict, that is passed to self.iter_transcripts().
     :return: Table with numbers of novel alternative splicing events, and suggested parameters for isotools.plots.plot_bar().'''
     weights = dict()
     # if groups is not None:
     #    gi={r:i for i,r in enumerate(runs)}
     #    groups={gn:[gi[r] for r in gr] for gn,gr in groups.items()}
     current = None
```

### Comparing `isotools-0.3.2/src/isotools/_utils.py` & `isotools-0.3.3/src/isotools/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 cigar = 'MIDNSHP=XB'
 cigar_lup = {c: i for i, c in enumerate(cigar)}
 
 compl = {'A': 'T', 'T': 'A', 'C': 'G', 'G': 'C'}
 
 
 def rc(seq):
-    '''reverse complement of seq'''
+    '''reverse complement of seq
+    :param seq: sequence
+    :return: reverse complement of seq'''
     return ''.join(reversed([compl[c] if c in compl else 'N' for c in seq]))
 
 
 def get_error_rate(bam_fn, n=1000):
     qual = 0
     total_len = 0
     with AlignmentFile(bam_fn, "rb", check_sq=False) as align:
@@ -35,15 +37,22 @@
                 pbar.update(1)
                 if i+1 >= n:
                     break
     return (qual/total_len)*100
 
 
 def basequal_hist(bam_fn, qual_bins=10**(np.linspace(-7, 0, 30)), len_bins=None, n=10000):
-    '''compute summary base quality statistics from base file, optionally dependent on read length'''
+    '''calculates base quality statistics for a bam file:
+
+    :param bam_fn: path to bam file
+    :param qual_bins: list of quality thresholds for binning
+    :param len_bins: list of read length thresholds for binning
+    :param n: number of reads to use for statistics
+    :return: pandas Series or DataFrame with base quality statistics'''
+
     n_len_bins = 1 if len_bins is None else len(len_bins)+1
     qual = np.zeros((len(qual_bins)+1, n_len_bins), dtype=int)
     len_i = 0
     i = 0
     with AlignmentFile(bam_fn, "rb") as align:
         if n is None:
             stats = align.get_index_statistics()
@@ -74,14 +83,18 @@
     "s -> (s0,s1), (s1,s2), (s2, s3), ..."
     a, b = itertools.tee(iterable)
     next(b, None)
     return zip(a, b)
 
 
 def cigar_string2tuples(cigarstring):
+    '''converts cigar string to tuples ((operator_id, length), ...)
+    :param cigarstring: cigar string
+    :return: tuple of tuples'''
+
     res = re.findall(f'(\\d+)([{cigar}]+)', cigarstring)
     return tuple((cigar_lup[c], int(n)) for n, c in res)
 
 
 def junctions_from_cigar(cigartuples, offset):
     'returns the exon positions'
     exons = list([[offset, offset]])
@@ -97,15 +110,15 @@
             exons[-1][1] += cigar[1]
     if exons[-1][0] == exons[-1][1]:  # delete 0 length exons at the end
         del exons[-1]
     return exons
 
 
 def is_same_gene(tr1, tr2, spj_iou_th=0, reg_iou_th=.5):
-    'checks whether tr1 and tr2 are the same gene by calculating intersection over union of the intersects'
+    'Checks whether tr1 and tr2 are the same gene by calculating intersection over union of the intersects'
     # current default definition of "same gene": at least one shared splice site
     # or more than 50% exonic overlap
     spj_i, reg_i = get_intersects(tr1, tr2)
     total_spj = (len(tr1)+len(tr2)-2)*2
     spj_iou = spj_i/(total_spj-spj_i) if total_spj > 0 else 0
     if spj_iou > spj_iou_th:
         return True
```

### Comparing `isotools-0.3.2/src/isotools/decorators.py` & `isotools-0.3.3/src/isotools/decorators.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.2/src/isotools/domains.py` & `isotools-0.3.3/src/isotools/domains.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         domains = []
         g = transcriptome[row[id_col]]
         if filter_kwargs:
             valid_transcripts = set(g.filter_transcripts(**filter_kwargs))
         domain_sets = {}
         for tr_col in tr_cols:
             domain_sets[tr_col] = set()
-            trids = set(row[tr_col]) & valid_transcripts if filter_kwargs else row[tr_col]
+            trids = set(row[tr_col]) & valid_transcripts if filter_kwargs else set(row[tr_col])
             for trid in trids:
                 for dom in g.transcripts[trid].get('domain', {}).get(source, []):
                     if categories is not None and dom[2] not in categories:
                         continue
                     if overlap_only and not has_overlap(dom[4], (row.start, row.end)):
                         continue
                     domain_sets[tr_col].add(str(dom[label_idx]))
@@ -281,48 +281,53 @@
     requestUrl = baseUrl + u'/run/'
     current_jobs = {}
     if isinstance(seqs, str):
         seqs = [seqs]
     domains = [None]*len(seqs)
     i = 0
     with tqdm(unit='proteins', disable=not progress_bar, total=len(seqs)) as pbar:
-        while seqs or current_jobs:
-            while seqs and len(current_jobs) < max_jobs:
-                params = {u'email': email, u'sequence': seqs.pop()}
-                resp = requests.post(requestUrl, data=params)
-                # todo: error handling - what if request fails?
-                current_jobs[resp.content.decode()] = i
-                pbar.set_description(f'waiting for {len(current_jobs)} jobs')
-                i += 1
-            time.sleep(poll_time)
-            done = set()
-            for job_id, idx in current_jobs.items():
-                url = baseUrl + u'/status/' + job_id
-                resp = requests.get(url)
-                if not resp.ok:  # todo: error handling: e.g. timeout error?
-                    continue
-                status = resp.content.decode()
-                if status in ('PENDING', 'RUNNING'):
-                    continue
-                if status == 'FINISHED':
-                    url = baseUrl + u'/result/' + job_id + '/json'
+        try:
+            while seqs or current_jobs:  # still something to do
+                while seqs and len(current_jobs) < max_jobs:  # start more jobs
+                    params = {u'email': email, u'sequence': seqs.pop()}
+                    resp = requests.post(requestUrl, data=params)
+                    # todo: error handling - what if request fails?
+                    current_jobs[resp.content.decode()] = i
+                    pbar.set_description(f'waiting for {len(current_jobs)} jobs')
+                    i += 1
+                time.sleep(poll_time)
+                done = set()
+                for job_id, idx in current_jobs.items():  # check the current jobs
+                    url = baseUrl + u'/status/' + job_id
                     resp = requests.get(url)
-                    if resp.ok:
-                        domains[idx] = resp.json()['results']  # else?
-                        pbar.update(1)
+                    if not resp.ok:  # todo: error handling: e.g. timeout error?
+                        continue
+                    status = resp.content.decode()
+                    if status in ('PENDING', 'RUNNING'):
+                        continue
+                    elif status == 'FINISHED':
+                        url = baseUrl + u'/result/' + job_id + '/json'
+                        resp = requests.get(url)
+                        if resp.ok:
+                            domains[idx] = resp.json()['results']  # else?
+                            pbar.update(1)
+                        else:
+                            domains[idx] = [{'status': 'FAILED', 'reason': 'resp_not_ok', 'jobid': job_id}]
+                        done.add(job_id)
+                    elif status == 'FAILED':  # try again?
+                        logger.warning(f'Failed to get response for sequence {idx}')
+                        done.add(job_id)
+                        domains[idx] = [{'status': 'FAILED', 'reason': 'job failed', 'jobid': job_id}]
                     else:
-                        domains[idx] = [{'status': 'FAILED', 'reason': 'resp_not_ok', 'jobid': job_id}]
-                    done.add(job_id)
-                elif status == 'FAILED':  # try again?
-                    logger.warning(f'Failed to get response for sequence {idx}')
-                    done.add(job_id)
-                    domains[idx] = [{'status': 'FAILED', 'reason': 'job failed', 'jobid': job_id}]
-            for job_id in done:
-                current_jobs.pop(job_id)
-            pbar.set_description(f'waiting for {len(current_jobs)} jobs')
+                        logger.warning(f'unhandled status for sequence {idx}: jobid={job_id}')
+                for job_id in done:  # remove the finished jobs
+                    current_jobs.pop(job_id)
+                pbar.set_description(f'waiting for {len(current_jobs)} jobs')
+        except KeyboardInterrupt:
+            logger.warning(f'Interrupting retrieval of {len(current_jobs)} jobs: [{",".join(current_jobs)}]')  # give the user the chance to check the jobs
     return domains
 
 # method of isotools.Gene
 
 
 def add_interpro_domains(self, genome, email, baseUrl='http://www.ebi.ac.uk/Tools/services/rest/iprscan5',  max_jobs=25, poll_time=5,
                          query=True, ref_query=False, min_coverage=None, max_coverage=None,  progress_bar=True):
@@ -367,10 +372,11 @@
                              (loc['start']*3, loc['end']*3),  # position
                              loc.get('hmmBounds')))  # completeness
                 # todo: potentially add more relevant information here
         for reference in range(2):
             for trid in seqs[dom['sequence']].get('reference' if reference else 'isotools', []):
                 tr = self.ref_transcripts[trid] if reference else self.transcripts[trid]
                 orf = sorted(self.find_transcript_positions(trid, tr.get('CDS', tr.get('ORF'))[:2], reference=reference))
-                pos_map = genomic_position([p+orf[0] for d in domL for p in d[2]], tr['exons'], self.strand == '-')
-                trdom = tuple((*d[:3], (pos_map[d[2][0]+orf[0]], pos_map[d[2][1]+orf[0]]), *d[3:]) for d in domL)
+                pos_map = genomic_position([p+orf[0] for dom in domL for p in dom[3]], tr['exons'], self.strand == '-')
+                trdom = tuple((*dom[:4], (pos_map[dom[3][0]+orf[0]], pos_map[dom[3][1]+orf[0]]), *dom[4:]) for dom in domL)
+
                 tr.setdefault('domain', {})['interpro'] = trdom
```

### Comparing `isotools-0.3.2/src/isotools/gene.py` & `isotools-0.3.3/src/isotools/gene.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
     from ._gene_plots import sashimi_plot, gene_track, sashimi_plot_short_reads, sashimi_figure, plot_domains
     from .domains import add_interpro_domains
 
     def short_reads(self, idx):
         '''Returns the short read coverage profile for a short read sample.
 
-        :param idx: The index of the short read sample. '''
+        :param idx: The index of the short read sample.
+        :returns: The short read coverage profile.'''
 
         try:
             return self.data['short_reads'][idx]
         except (KeyError, IndexError):
             srdf = self._transcriptome.infos['short_reads']  # raises key_error if no short reads added
             self.data.setdefault('short_reads', [])
             for i in range(len(self.data['short_reads']), len(srdf)):
@@ -59,44 +60,47 @@
         '''Corrects for splicing shifts.
 
          This function looks for "shifted junctions", e.g. same difference compared to reference annotaiton at both donor and acceptor)
          presumably caused by ambigous alignments. In these cases the positions are adapted to the reference position (if modify is set).
 
          :param trid: The index of the transcript to be checked.
          :param size: The maximum shift to be corrected.
-         :param modify: If set, the exon positions are corrected according to the reference.'''
+         :param modify: If set, the exon positions are corrected according to the reference.
+         :returns: A dictionary with the exon id as keys and the shifted bases as values.'''
 
         exons = trid['exons']
         shifts = self.ref_segment_graph.fuzzy_junction(exons, size)
         if shifts and modify:
             for i, sh in shifts.items():
                 if exons[i][0] <= exons[i][1] + sh and exons[i + 1][0] + sh <= exons[i + 1][1]:
                     exons[i][1] += sh
                     exons[i + 1][0] += sh
             trid['exons'] = [e for e in exons if e[0] < e[1]]  # remove zero length exons
         return shifts
 
-    def _to_gtf(self, trids, source='isoseq'):
+    def _to_gtf(self, trids, ref_trids=None, source='isoseq', ref_source='annotation'):
         '''Creates the gtf lines of the gene as strings.'''
         donotshow = {'transcripts', 'short_exons', 'segment_graph'}
         info = {'gene_id': self.id, 'gene_name': self.name}
         lines = [None]
         starts = []
         ends = []
+        ref_fsm = []
         for i in trids:
             tr = self.transcripts[i]
             info['transcript_id'] = f'{info["gene_id"]}_{i}'
             starts.append(tr['exons'][0][0] + 1)
             ends.append(tr['exons'][-1][1])
             trinfo = info.copy()
             if 'downstream_A_content' in tr:
                 trinfo['downstream_A_content'] = f'{tr["downstream_A_content"]:0.3f}'
             if tr['annotation'][0] == 0:  # FSM
                 refinfo = {}
                 for refid in tr['annotation'][1]['FSM']:
+                    ref_fsm.append(refid)
                     for k in self.ref_transcripts[refid]:
                         if k == 'exons':
                             continue
                         elif k == 'CDS':
                             if self.strand == '+':
                                 cds_start, cds_end = self.ref_transcripts[refid]['CDS']
                             else:
@@ -116,14 +120,42 @@
                 exon_info = info.copy()
                 exon_info['exon_id'] = f'{info["gene_id"]}_{i}_{enr}'
                 if enr in noncanonical:
                     exon_info['noncanonical_donor'] = noncanonical[enr][:2]
                 if enr+1 in noncanonical:
                     exon_info['noncanonical_acceptor'] = noncanonical[enr+1][2:]
                 lines.append((self.chrom, source, 'exon', pos[0] + 1, pos[1], '.', self.strand, '.', '; '.join(f'{k} "{v}"' for k, v in exon_info.items())))
+        if ref_trids:
+            # add reference transcripts not covered by FSM
+            for i, tr in enumerate(self.ref_transcripts):
+                if i in ref_fsm:
+                    continue
+                starts.append(tr['exons'][0][0] + 1)
+                ends.append(tr['exons'][-1][1])
+                info['transcript_id'] = f'{info["gene_id"]}_ref{i}'
+                refinfo = info.copy()
+                for k in tr:
+                    if k == 'exons':
+                        continue
+                    elif k == 'CDS':
+                        if self.strand == '+':
+                            cds_start, cds_end = tr['CDS']
+                        else:
+                            cds_end, cds_start = tr['CDS']
+                        refinfo['CDS_start'] = str(cds_start)
+                        refinfo['CDS_end'] = str(cds_end)
+                    else:
+                        refinfo.setdefault(k, []).append(str(tr[k]))
+                    lines.append((self.chrom, ref_source, 'transcript', tr['exons'][0][0] + 1, tr['exons'][-1][1], '.',
+                                  self.strand, '.', '; '.join(f'{k} "{v}"' for k, v in refinfo.items())))
+                    for enr, pos in enumerate(tr['exons']):
+                        exon_info = info.copy()
+                        exon_id = f'{info["gene_id"]}_ref{i}_{enr}'
+                        lines.append((self.chrom, ref_source, 'exon', pos[0] + 1, pos[1], '.', self.strand, '.', f'exon_id "{exon_id}"'))
+
         if len(lines) > 1:
             # add gene line
             if 'reference' in self.data:
                 info.update({k: v for k, v in self.data['reference'].items() if k not in donotshow})  # add reference gene specific fields
             lines[0] = (self.chrom, source, 'gene', min(starts), max(ends), '.', self.strand, '.', '; '.join(f'{k} "{v}"' for k, v in info.items()))
             return lines
         return []
@@ -213,15 +245,17 @@
     def get_sequence(self, genome_fh, trids=None, reference=False, protein=False):
         '''Returns the nucleotide sequence of the specified transcripts.
 
         :param genome_fh: The path to the genome fasta file, or FastaFile handle.
         :param trids: List of transcript ids for which the sequence are requested.
         :param reference: Specifiy whether the sequence is fetched for reference transcripts (True)
             or long read transcripts (False, default).
-        :param protein: Return protein sequences instead of transcript sequences.'''
+        :param protein: Return protein sequences instead of transcript sequences.
+        :returns: A dictionary of transcript ids and their sequences.
+        '''
 
         trL = [(i, tr) for i, tr in enumerate(self.ref_transcripts if reference else self.transcripts) if trids is None or i in trids]
         if not trL:
             return {}
         pos = (min(tr['exons'][0][0] for _, tr in trL), max(tr['exons'][-1][1] for _, tr in trL))
         try:  # assume its a FastaFile file handle
             seq = genome_fh.fetch(self.chrom, *pos)
@@ -257,14 +291,26 @@
         trL = self.ref_transcripts if reference else self.transcripts
         for (_, orfs), tr in zip(self.get_all_orf(genome_fh, reference, minlen, start_codons, stop_codons), trL):
             if orfs:
                 tr["ORF"] = max(orfs, key=lambda x: x[2]['length'])
 
     def get_all_orf(self, genome_fh, reference=False, minlen=30, start_codons=["ATG"], stop_codons=['TAA', 'TAG', 'TGA']):
         ''' Predicts ORF.
+
+        :param genome_fh: The path to the genome fasta file, or FastaFile handle.
+        :param reference: Specifiy whether the sequence is fetched for reference transcripts (True)
+            or long read transcripts (False, default).
+        :param minlen: The minimum length of the ORF.
+        :param start_codons: List of start codons.
+        :param stop_codons: List of stop codons.
+        :returns: A list of (transcript_id, list_of_orfs) tuples. Each orf is a tuple of (genomic_start, genomic_end, orf_properties).
+        The orf_properties is a dictionary with keys 'start', 'length', 'start_codon', 'stop_codon' and 'NMD'.
+        NMD is True if the ORF is predicted to be degraded by nonsense-mediated decay,
+        as defined by the 55 bases rule, e.g. there is at least one splice site upstream the stop codon,
+        and the distance of the stop codon to the last upstrame splice site is less than 55 bases.
         '''
         orf_list = []
         trL = self.ref_transcripts if reference else self.transcripts
         for trid, tr_seq in self.get_sequence(genome_fh, reference=reference).items():
             tr = trL[trid]
             tr_start = tr['exons'][0][0]
             cum_exon_len = np.cumsum([end-start for start, end in tr['exons']])  # cummulative exon length
@@ -527,16 +573,16 @@
         return Gene, (self.start, self.end, self.data, self._transcriptome)
 
     def copy(self):
         'Returns a shallow copy of self.'
         return self.__copy__()
 
     def filter_transcripts(self, query=None, min_coverage=None, max_coverage=None):
-        tr_filter = self._transcriptome.filter['transcript']
         if query:
+            tr_filter = self._transcriptome.filter['transcript']
             # used_tags={tag for tag in re.findall(r'\b\w+\b', query) if tag not in BOOL_OP}
             query_fun, used_tags = _filter_function(query)
             msg = 'did not find the following filter rules: {}\nvalid rules are: {}'
             assert all(f in tr_filter for f in used_tags), msg.format(
                 ', '.join(f for f in used_tags if f not in tr_filter), ', '.join(tr_filter))
             tr_filter_fun = {tag: _filter_function(tr_filter[tag])[0] for tag in used_tags if tag in tr_filter}
         trids = []
@@ -547,24 +593,24 @@
                 continue
             if query is None or query_fun(
                     **{tag: f(g=self, trid=i, **tr) for tag, f in tr_filter_fun.items()}):
                 trids.append(i)
         return trids
 
     def filter_ref_transcripts(self, query=None):
-        tr_filter = self._transcriptome.filter['reference']
         if query:
+            tr_filter = self._transcriptome.filter['reference']
             # used_tags={tag for tag in re.findall(r'\b\w+\b', query) if tag not in BOOL_OP}
             query_fun, used_tags = _filter_function(query)
             msg = 'did not find the following filter rules: {}\nvalid rules are: {}'
             assert all(f in tr_filter for f in used_tags), msg.format(
                 ', '.join(f for f in used_tags if f not in tr_filter), ', '.join(tr_filter))
             tr_filter_fun = {tag: _filter_function(tr_filter[tag])[0] for tag in used_tags if tag in tr_filter}
         else:
-            return list(range(len(self.transcripts)))
+            return list(range(len(self.ref_transcripts)))
         trids = []
         for i, tr in enumerate(self.ref_transcripts):
             if query_fun(**{tag: f(g=self, trid=i, **tr) for tag, f in tr_filter_fun.items()}):
                 trids.append(i)
         return trids
 
     def _find_splice_sites(exons, transcripts):
```

### Comparing `isotools-0.3.2/src/isotools/plots.py` & `isotools-0.3.3/src/isotools/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     :param sample_colors: Specify the colors for the samples (e.g. the dots) as a dict. Defaults to the corresponding group color.
     :param pt_size: Specify the size for the data points in the plot.
     :param lw: Specify witdh of the lines. See matplotlib Line2D for details.
     :param ls: Specify style of the lines. See matplotlib Line2D for details.
     :return: figure, axes and list of plotted events
     '''
 
-    plotted = pd.DataFrame(columns=result_table.columns)
+    plotted = {}  # pd.DataFrame(columns=result_table.columns)
     if isinstance(splice_types, str):
         splice_types = [splice_types]
     f, axs = plt.subplots(*grid_shape)
     axs = axs.flatten()
     x = [i / 100 for i in range(101)]
     group_names = [c[:-4] for c in result_table.columns if c.endswith('_PSI')][:2]
     groups = {gn: [c[:c.rfind(gn)-1] for c in result_table.columns if c.endswith(gn + '_total_cov')] for gn in group_names}
@@ -50,15 +50,15 @@
     sample_colors = {sa: sample_colors.get(sa, group_colors[gn]) for gn in group_names for sa in groups[gn]}
     other = {group_names[0]: group_names[1], group_names[1]: group_names[0]}
     logger.debug('groups: %s', str(groups))
     for idx, row in result_table.iterrows():
         logger.debug('plotting %s: %s', idx, row.gene)
         if splice_types is not None and row.splice_type not in splice_types:
             continue
-        if row.gene in set(plotted.gene):
+        if row.gene in plotted:
             continue
         params_alt = {gn: (row[f'{gn}_PSI'], row[f'{gn}_disp']) for gn in group_names}
         # select only samples covered >= min_cov
         # psi_gr = {gn: [row[f'{sa}_in_cov'] / row[f'{sa}_total_cov'] for sa in gr if row[f'{sa}_total_cov'] >= min_cov] for gn, gr in groups.items()}
         psi_gr_list = [(sa, gn, row[f'{sa}_{gn}_in_cov'] / row[f'{sa}_{gn}_total_cov'])
                        for gn, gr in groups.items() for sa in gr if row[f'{sa}_{gn}_total_cov'] >= min_cov]
         psi_gr = pd.DataFrame(psi_gr_list, columns=['sample', 'group', 'psi'])
@@ -85,18 +85,18 @@
                 y[max_i] = beta(*params).pdf(params_alt[gn][0])
             else:
                 y = np.zeros(len(x))
                 y[max_i] = 1  # point mass
             ax2.plot(x, y, color=group_colors[gn], lw=lw, ls=ls)
             ax2.tick_params(right=False, labelright=False)
         ax.set_title(f'{row.gene} {row.splice_type}\nFDR={row.padj:.5f}')
-        plotted = plotted.append(row)
+        plotted[row.gene] = row
         if len(plotted) == len(axs):
             break
-    return f, axs, plotted
+    return f, axs, pd.concat(plotted.values())
 
 
 def plot_embedding(splice_bubbles, method='PCA', prior_count=3,
                    top_var=500, min_total=100, min_alt_fraction=.1, plot_components=(1, 2),
                    splice_types='all', labels=True, groups=None, colors=None, pt_size=20, ax=None, **kwargs):
     ''' Plots embedding of alternative splicing events.
```

### Comparing `isotools-0.3.2/src/isotools/run_isotools.py` & `isotools-0.3.3/src/isotools/run_isotools.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.2/src/isotools/short_read.py` & `isotools-0.3.3/src/isotools/short_read.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.2/src/isotools/splice_graph.py` & `isotools-0.3.3/src/isotools/splice_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -939,18 +939,19 @@
         :return: True, if the position overlaps with an exon, else False.'''
         for n in self:
             if n[0] <= position and n[1] >= position:
                 return True
         return False
 
     def _get_all_exons(self, nodeX, nodeY, tr):
-        'get all exons from nodeX to nodeY for transcripts tr'
+        'get all exonic regions between (including) nodeX to nodeY for transcripts tr'
         # TODO: add option to extend first and last exons
         n = max(nodeX, self._tss[tr])  # if tss>nodeX start there
         if tr not in self[n].pre and self._tss[tr] != n:  # nodeX is not part of tr
+            # find first node in tr after nodeX but before nodeY
             for i in range(n, nodeY + 1):
                 if tr in self[n].suc:
                     n = i
                     break
             else:
                 return []
         if n > nodeY:
```

### Comparing `isotools-0.3.2/src/isotools/transcriptome.py` & `isotools-0.3.3/src/isotools/transcriptome.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.2/src/isotools.egg-info/PKG-INFO` & `isotools-0.3.3/src/isotools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isotools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Framework for the analysis of long read transcriptome sequencing data
 Home-page: https://github.com/MatthiasLienhard/isotools
 Author: Matthias Lienhard
 Author-email: lienhard@molgen.mpg.de
 Project-URL: Bug Tracker, https://github.com/MatthiasLienhard/isotools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `isotools-0.3.2/src/isotools.egg-info/SOURCES.txt` & `isotools-0.3.3/src/isotools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

