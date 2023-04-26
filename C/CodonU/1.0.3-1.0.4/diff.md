# Comparing `tmp/CodonU-1.0.3.tar.gz` & `tmp/CodonU-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodonU-1.0.3.tar", last modified: Tue Apr 25 14:13:01 2023, max compression
+gzip compressed data, was "CodonU-1.0.4.tar", last modified: Wed Apr 26 12:56:33 2023, max compression
```

## Comparing `CodonU-1.0.3.tar` & `CodonU-1.0.4.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-25 14:13:01.500351 CodonU-1.0.3/
-drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-25 14:13:00.827349 CodonU-1.0.3/CodonU/
--rw-rw-r--   0 souro     (1000) souro     (1000)        0 2023-03-05 07:31:25.000000 CodonU-1.0.3/CodonU/__init__.py
-drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-25 14:13:00.838349 CodonU-1.0.3/CodonU/analyzer/
--rw-rw-r--   0 souro     (1000) souro     (1000)      344 2023-04-23 09:03:35.000000 CodonU-1.0.3/CodonU/analyzer/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     2516 2023-04-25 13:05:47.000000 CodonU-1.0.3/CodonU/analyzer/aromaticity_comp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     3287 2023-04-25 09:49:41.000000 CodonU-1.0.3/CodonU/analyzer/cai_comp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     3552 2023-04-25 09:45:02.000000 CodonU-1.0.3/CodonU/analyzer/cbi_comp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     2527 2023-04-25 10:13:24.000000 CodonU-1.0.3/CodonU/analyzer/enc_comp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     6524 2023-03-26 14:18:02.000000 CodonU-1.0.3/CodonU/analyzer/generate_report.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     5901 2023-03-27 11:31:56.000000 CodonU-1.0.3/CodonU/analyzer/generate_report_summary.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     2511 2023-04-25 12:58:07.000000 CodonU-1.0.3/CodonU/analyzer/gravy_comp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     8876 2023-03-21 06:22:22.000000 CodonU-1.0.3/CodonU/analyzer/internal_comp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     3032 2023-04-25 14:00:41.000000 CodonU-1.0.3/CodonU/analyzer/rscu_comp.py
-drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-25 14:13:00.901349 CodonU-1.0.3/CodonU/correspondence_analysis/
--rw-rw-r--   0 souro     (1000) souro     (1000)      123 2023-03-06 12:33:30.000000 CodonU-1.0.3/CodonU/correspondence_analysis/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1774 2023-03-05 12:14:39.000000 CodonU-1.0.3/CodonU/correspondence_analysis/mca_aa_freq.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     2127 2023-03-05 12:06:51.000000 CodonU-1.0.3/CodonU/correspondence_analysis/mca_codon_freq.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1633 2023-03-05 12:06:51.000000 CodonU-1.0.3/CodonU/correspondence_analysis/mca_codon_rscu.py
-drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-25 14:13:01.115350 CodonU-1.0.3/CodonU/cua_errors/
--rw-rw-r--   0 souro     (1000) souro     (1000)      277 2023-03-08 17:10:24.000000 CodonU-1.0.3/CodonU/cua_errors/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      226 2023-02-05 14:22:18.000000 CodonU-1.0.3/CodonU/cua_errors/codon_usage_err.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      302 2023-02-05 14:45:01.000000 CodonU-1.0.3/CodonU/cua_errors/file_not_empty_err.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      421 2023-02-05 14:45:01.000000 CodonU-1.0.3/CodonU/cua_errors/internal_stop_codon_err.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      662 2023-02-05 14:45:01.000000 CodonU-1.0.3/CodonU/cua_errors/no_prot_err.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      616 2023-02-05 14:45:01.000000 CodonU-1.0.3/CodonU/cua_errors/nucleotide_err.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      478 2023-02-05 14:45:01.000000 CodonU-1.0.3/CodonU/cua_errors/ter_seq_err.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      463 2023-03-08 17:18:27.000000 CodonU-1.0.3/CodonU/cua_errors/unsupported_type.py
-drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-25 14:13:01.188350 CodonU-1.0.3/CodonU/cua_warnings/
--rw-rw-r--   0 souro     (1000) souro     (1000)      262 2023-04-24 07:10:51.000000 CodonU-1.0.3/CodonU/cua_warnings/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      361 2023-02-05 14:34:03.000000 CodonU-1.0.3/CodonU/cua_warnings/api_warn.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      165 2023-02-20 11:53:24.000000 CodonU-1.0.3/CodonU/cua_warnings/codon_usage_warns.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      355 2023-02-05 14:34:03.000000 CodonU-1.0.3/CodonU/cua_warnings/email_warn.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      435 2023-02-05 14:22:19.000000 CodonU-1.0.3/CodonU/cua_warnings/missing_codon_warn.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      443 2023-02-20 12:36:46.000000 CodonU-1.0.3/CodonU/cua_warnings/no_codon_warn.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      374 2023-02-05 14:22:18.000000 CodonU-1.0.3/CodonU/cua_warnings/no_syn_codon_warn.py
-drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-25 14:13:01.226350 CodonU-1.0.3/CodonU/extractor/
--rw-rw-r--   0 souro     (1000) souro     (1000)      162 2023-02-05 17:20:46.000000 CodonU-1.0.3/CodonU/extractor/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      772 2023-02-05 17:20:46.000000 CodonU-1.0.3/CodonU/extractor/extract_cds.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      466 2023-02-05 17:20:46.000000 CodonU-1.0.3/CodonU/extractor/extract_cds_lst.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      770 2023-02-05 17:20:45.000000 CodonU-1.0.3/CodonU/extractor/extract_exome.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      876 2023-02-05 17:20:45.000000 CodonU-1.0.3/CodonU/extractor/extract_prot.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      622 2023-02-05 17:20:46.000000 CodonU-1.0.3/CodonU/extractor/internal_comp.py
-drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-25 14:13:01.323351 CodonU-1.0.3/CodonU/file_handler/
--rw-rw-r--   0 souro     (1000) souro     (1000)      299 2023-04-24 07:10:51.000000 CodonU-1.0.3/CodonU/file_handler/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      563 2023-02-07 16:28:20.000000 CodonU-1.0.3/CodonU/file_handler/get_gb.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1943 2023-04-25 07:25:20.000000 CodonU-1.0.3/CodonU/file_handler/internal_comp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      282 2023-02-07 16:29:21.000000 CodonU-1.0.3/CodonU/file_handler/make_dir.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      258 2023-02-07 16:31:13.000000 CodonU-1.0.3/CodonU/file_handler/read_file.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      452 2023-03-06 12:48:19.000000 CodonU-1.0.3/CodonU/file_handler/set_entrez_param.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      793 2023-02-20 11:53:24.000000 CodonU-1.0.3/CodonU/file_handler/write_exome_fasta.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      968 2023-02-20 11:53:24.000000 CodonU-1.0.3/CodonU/file_handler/write_nucleotide_fasta.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      847 2023-02-20 11:53:24.000000 CodonU-1.0.3/CodonU/file_handler/write_protein_fasta.py
-drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-25 14:13:01.367350 CodonU-1.0.3/CodonU/phylogenetic_analysis/
--rw-rw-r--   0 souro     (1000) souro     (1000)      129 2023-04-23 10:39:14.000000 CodonU-1.0.3/CodonU/phylogenetic_analysis/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1314 2023-04-09 16:04:34.000000 CodonU-1.0.3/CodonU/phylogenetic_analysis/clustal_o.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1295 2023-04-09 16:04:53.000000 CodonU-1.0.3/CodonU/phylogenetic_analysis/clustal_w.py
--rw-r--r--   0 souro     (1000) souro     (1000)      805 2023-04-25 14:05:22.000000 CodonU-1.0.3/CodonU/phylogenetic_analysis/generate_phylo_input.py
-drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-25 14:13:01.448351 CodonU-1.0.3/CodonU/vizualizer/
--rw-rw-r--   0 souro     (1000) souro     (1000)      377 2023-04-13 13:58:13.000000 CodonU-1.0.3/CodonU/vizualizer/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1401 2023-04-25 14:00:42.000000 CodonU-1.0.3/CodonU/vizualizer/plot_enc.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     8101 2023-04-25 14:08:24.000000 CodonU-1.0.3/CodonU/vizualizer/plot_funcs.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     2782 2023-04-25 14:00:42.000000 CodonU-1.0.3/CodonU/vizualizer/plot_mca_aa_aroma.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     2771 2023-04-25 14:00:42.000000 CodonU-1.0.3/CodonU/vizualizer/plot_mca_aa_gravy.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     2721 2023-04-25 14:00:42.000000 CodonU-1.0.3/CodonU/vizualizer/plot_mca_codon_freq.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     2688 2023-04-25 14:05:22.000000 CodonU-1.0.3/CodonU/vizualizer/plot_mca_rscu.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1358 2023-02-23 15:35:27.000000 CodonU-1.0.3/CodonU/vizualizer/plot_neutrality.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1070 2023-04-25 14:08:24.000000 CodonU-1.0.3/CodonU/vizualizer/plot_phy_dnd.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1353 2023-04-25 14:08:24.000000 CodonU-1.0.3/CodonU/vizualizer/plot_phy_nex.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1538 2023-02-23 15:35:27.000000 CodonU-1.0.3/CodonU/vizualizer/plot_pr2.py
-drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-25 14:13:00.830349 CodonU-1.0.3/CodonU.egg-info/
--rw-rw-r--   0 souro     (1000) souro     (1000)     3072 2023-04-25 14:13:00.000000 CodonU-1.0.3/CodonU.egg-info/PKG-INFO
--rw-rw-r--   0 souro     (1000) souro     (1000)     2315 2023-04-25 14:13:00.000000 CodonU-1.0.3/CodonU.egg-info/SOURCES.txt
--rw-rw-r--   0 souro     (1000) souro     (1000)        1 2023-04-25 14:13:00.000000 CodonU-1.0.3/CodonU.egg-info/dependency_links.txt
--rw-rw-r--   0 souro     (1000) souro     (1000)        7 2023-04-25 14:13:00.000000 CodonU-1.0.3/CodonU.egg-info/top_level.txt
--rw-rw-r--   0 souro     (1000) souro     (1000)     1077 2023-02-01 15:01:49.000000 CodonU-1.0.3/LICENSE.md
--rw-r--r--   0 souro     (1000) souro     (1000)     3072 2023-04-25 14:13:01.500351 CodonU-1.0.3/PKG-INFO
--rw-rw-r--   0 souro     (1000) souro     (1000)     5677 2023-04-24 07:53:05.000000 CodonU-1.0.3/README.md
--rw-r--r--   0 souro     (1000) souro     (1000)       38 2023-04-25 14:13:01.500351 CodonU-1.0.3/setup.cfg
--rw-rw-r--   0 souro     (1000) souro     (1000)     2178 2023-04-25 14:09:34.000000 CodonU-1.0.3/setup.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-26 12:56:33.783421 CodonU-1.0.4/
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-26 12:56:33.125419 CodonU-1.0.4/CodonU/
+-rw-rw-r--   0 souro     (1000) souro     (1000)        0 2023-03-05 07:31:25.000000 CodonU-1.0.4/CodonU/__init__.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-26 12:56:33.299420 CodonU-1.0.4/CodonU/analyzer/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      344 2023-04-23 09:03:35.000000 CodonU-1.0.4/CodonU/analyzer/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2516 2023-04-25 13:05:47.000000 CodonU-1.0.4/CodonU/analyzer/aromaticity_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     3287 2023-04-25 09:49:41.000000 CodonU-1.0.4/CodonU/analyzer/cai_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     3552 2023-04-25 09:45:02.000000 CodonU-1.0.4/CodonU/analyzer/cbi_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2527 2023-04-25 10:13:24.000000 CodonU-1.0.4/CodonU/analyzer/enc_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     6524 2023-03-26 14:18:02.000000 CodonU-1.0.4/CodonU/analyzer/generate_report.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     5901 2023-03-27 11:31:56.000000 CodonU-1.0.4/CodonU/analyzer/generate_report_summary.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2511 2023-04-25 12:58:07.000000 CodonU-1.0.4/CodonU/analyzer/gravy_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     8876 2023-03-21 06:22:22.000000 CodonU-1.0.4/CodonU/analyzer/internal_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     3032 2023-04-25 14:00:41.000000 CodonU-1.0.4/CodonU/analyzer/rscu_comp.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-26 12:56:33.362420 CodonU-1.0.4/CodonU/correspondence_analysis/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      123 2023-03-06 12:33:30.000000 CodonU-1.0.4/CodonU/correspondence_analysis/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1774 2023-03-05 12:14:39.000000 CodonU-1.0.4/CodonU/correspondence_analysis/mca_aa_freq.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2127 2023-03-05 12:06:51.000000 CodonU-1.0.4/CodonU/correspondence_analysis/mca_codon_freq.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1595 2023-04-25 18:50:11.000000 CodonU-1.0.4/CodonU/correspondence_analysis/mca_codon_rscu.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-26 12:56:33.438420 CodonU-1.0.4/CodonU/cua_errors/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      277 2023-03-08 17:10:24.000000 CodonU-1.0.4/CodonU/cua_errors/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      226 2023-02-05 14:22:18.000000 CodonU-1.0.4/CodonU/cua_errors/codon_usage_err.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      302 2023-02-05 14:45:01.000000 CodonU-1.0.4/CodonU/cua_errors/file_not_empty_err.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      421 2023-02-05 14:45:01.000000 CodonU-1.0.4/CodonU/cua_errors/internal_stop_codon_err.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      662 2023-02-05 14:45:01.000000 CodonU-1.0.4/CodonU/cua_errors/no_prot_err.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      616 2023-02-05 14:45:01.000000 CodonU-1.0.4/CodonU/cua_errors/nucleotide_err.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      478 2023-02-05 14:45:01.000000 CodonU-1.0.4/CodonU/cua_errors/ter_seq_err.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      463 2023-03-08 17:18:27.000000 CodonU-1.0.4/CodonU/cua_errors/unsupported_type.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-26 12:56:33.534421 CodonU-1.0.4/CodonU/cua_warnings/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      262 2023-04-24 07:10:51.000000 CodonU-1.0.4/CodonU/cua_warnings/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      361 2023-02-05 14:34:03.000000 CodonU-1.0.4/CodonU/cua_warnings/api_warn.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      165 2023-02-20 11:53:24.000000 CodonU-1.0.4/CodonU/cua_warnings/codon_usage_warns.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      355 2023-02-05 14:34:03.000000 CodonU-1.0.4/CodonU/cua_warnings/email_warn.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      435 2023-02-05 14:22:19.000000 CodonU-1.0.4/CodonU/cua_warnings/missing_codon_warn.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      443 2023-02-20 12:36:46.000000 CodonU-1.0.4/CodonU/cua_warnings/no_codon_warn.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      374 2023-02-05 14:22:18.000000 CodonU-1.0.4/CodonU/cua_warnings/no_syn_codon_warn.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-26 12:56:33.572421 CodonU-1.0.4/CodonU/extractor/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      162 2023-02-05 17:20:46.000000 CodonU-1.0.4/CodonU/extractor/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      772 2023-02-05 17:20:46.000000 CodonU-1.0.4/CodonU/extractor/extract_cds.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      466 2023-02-05 17:20:46.000000 CodonU-1.0.4/CodonU/extractor/extract_cds_lst.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      770 2023-02-05 17:20:45.000000 CodonU-1.0.4/CodonU/extractor/extract_exome.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      876 2023-02-05 17:20:45.000000 CodonU-1.0.4/CodonU/extractor/extract_prot.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      622 2023-02-05 17:20:46.000000 CodonU-1.0.4/CodonU/extractor/internal_comp.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-26 12:56:33.668421 CodonU-1.0.4/CodonU/file_handler/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      299 2023-04-24 07:10:51.000000 CodonU-1.0.4/CodonU/file_handler/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      563 2023-02-07 16:28:20.000000 CodonU-1.0.4/CodonU/file_handler/get_gb.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1943 2023-04-25 07:25:20.000000 CodonU-1.0.4/CodonU/file_handler/internal_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      282 2023-02-07 16:29:21.000000 CodonU-1.0.4/CodonU/file_handler/make_dir.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      258 2023-02-07 16:31:13.000000 CodonU-1.0.4/CodonU/file_handler/read_file.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      452 2023-03-06 12:48:19.000000 CodonU-1.0.4/CodonU/file_handler/set_entrez_param.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      793 2023-02-20 11:53:24.000000 CodonU-1.0.4/CodonU/file_handler/write_exome_fasta.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      968 2023-02-20 11:53:24.000000 CodonU-1.0.4/CodonU/file_handler/write_nucleotide_fasta.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      847 2023-02-20 11:53:24.000000 CodonU-1.0.4/CodonU/file_handler/write_protein_fasta.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-26 12:56:33.685421 CodonU-1.0.4/CodonU/phylogenetic_analysis/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      129 2023-04-23 10:39:14.000000 CodonU-1.0.4/CodonU/phylogenetic_analysis/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1320 2023-04-26 12:49:51.000000 CodonU-1.0.4/CodonU/phylogenetic_analysis/clustal_o.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1299 2023-04-25 19:29:26.000000 CodonU-1.0.4/CodonU/phylogenetic_analysis/clustal_w.py
+-rw-r--r--   0 souro     (1000) souro     (1000)      805 2023-04-25 14:05:22.000000 CodonU-1.0.4/CodonU/phylogenetic_analysis/generate_phylo_input.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-26 12:56:33.767421 CodonU-1.0.4/CodonU/vizualizer/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      416 2023-04-26 12:49:51.000000 CodonU-1.0.4/CodonU/vizualizer/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1401 2023-04-25 14:00:42.000000 CodonU-1.0.4/CodonU/vizualizer/plot_enc.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     8101 2023-04-25 14:08:24.000000 CodonU-1.0.4/CodonU/vizualizer/plot_funcs.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2782 2023-04-25 14:00:42.000000 CodonU-1.0.4/CodonU/vizualizer/plot_mca_aa_aroma.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2771 2023-04-25 14:00:42.000000 CodonU-1.0.4/CodonU/vizualizer/plot_mca_aa_gravy.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2721 2023-04-25 14:00:42.000000 CodonU-1.0.4/CodonU/vizualizer/plot_mca_codon_freq.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2688 2023-04-25 14:05:22.000000 CodonU-1.0.4/CodonU/vizualizer/plot_mca_rscu.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1358 2023-02-23 15:35:27.000000 CodonU-1.0.4/CodonU/vizualizer/plot_neutrality.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1070 2023-04-25 14:08:24.000000 CodonU-1.0.4/CodonU/vizualizer/plot_phy_dnd.py
+-rw-r--r--   0 souro     (1000) souro     (1000)     1505 2023-04-26 12:49:52.000000 CodonU-1.0.4/CodonU/vizualizer/plot_phy_fas.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1357 2023-04-26 12:41:27.000000 CodonU-1.0.4/CodonU/vizualizer/plot_phy_nex.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1538 2023-02-23 15:35:27.000000 CodonU-1.0.4/CodonU/vizualizer/plot_pr2.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-26 12:56:33.127419 CodonU-1.0.4/CodonU.egg-info/
+-rw-rw-r--   0 souro     (1000) souro     (1000)     3072 2023-04-26 12:56:32.000000 CodonU-1.0.4/CodonU.egg-info/PKG-INFO
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2349 2023-04-26 12:56:32.000000 CodonU-1.0.4/CodonU.egg-info/SOURCES.txt
+-rw-rw-r--   0 souro     (1000) souro     (1000)        1 2023-04-26 12:56:32.000000 CodonU-1.0.4/CodonU.egg-info/dependency_links.txt
+-rw-rw-r--   0 souro     (1000) souro     (1000)        7 2023-04-26 12:56:32.000000 CodonU-1.0.4/CodonU.egg-info/top_level.txt
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1077 2023-02-01 15:01:49.000000 CodonU-1.0.4/LICENSE.md
+-rw-r--r--   0 souro     (1000) souro     (1000)     3072 2023-04-26 12:56:33.783421 CodonU-1.0.4/PKG-INFO
+-rw-rw-r--   0 souro     (1000) souro     (1000)     5677 2023-04-24 07:53:05.000000 CodonU-1.0.4/README.md
+-rw-r--r--   0 souro     (1000) souro     (1000)       38 2023-04-26 12:56:33.783421 CodonU-1.0.4/setup.cfg
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2178 2023-04-26 12:53:14.000000 CodonU-1.0.4/setup.py
```

### Comparing `CodonU-1.0.3/CodonU/analyzer/aromaticity_comp.py` & `CodonU-1.0.4/CodonU/analyzer/aromaticity_comp.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/analyzer/cai_comp.py` & `CodonU-1.0.4/CodonU/analyzer/cai_comp.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/analyzer/cbi_comp.py` & `CodonU-1.0.4/CodonU/analyzer/cbi_comp.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/analyzer/enc_comp.py` & `CodonU-1.0.4/CodonU/analyzer/enc_comp.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/analyzer/generate_report.py` & `CodonU-1.0.4/CodonU/analyzer/generate_report.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/analyzer/generate_report_summary.py` & `CodonU-1.0.4/CodonU/analyzer/generate_report_summary.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/analyzer/gravy_comp.py` & `CodonU-1.0.4/CodonU/analyzer/gravy_comp.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/analyzer/internal_comp.py` & `CodonU-1.0.4/CodonU/analyzer/internal_comp.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/analyzer/rscu_comp.py` & `CodonU-1.0.4/CodonU/analyzer/rscu_comp.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/correspondence_analysis/mca_aa_freq.py` & `CodonU-1.0.4/CodonU/correspondence_analysis/mca_aa_freq.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/correspondence_analysis/mca_codon_freq.py` & `CodonU-1.0.4/CodonU/correspondence_analysis/mca_codon_freq.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/correspondence_analysis/mca_codon_rscu.py` & `CodonU-1.0.4/CodonU/correspondence_analysis/mca_codon_rscu.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 
     :param handle: Handle to the file, or the filename as a string
     :param genetic_table_num: Genetic table number for codon table
     :param min_len_threshold: Minimum length of nucleotide sequence to be considered as gene (optional)
     :param n_components: The number of principal components to compute (optional)
     :return: The contingency table and inertia [inertia values lying between 0 and 1]
     """
-    records = parse(handle, 'fasta')
     codons = [codon for codon, _ in unambiguous_dna_by_id[genetic_table_num].forward_table.items()]
-    rscu_dict = calculate_rscu(records, genetic_table_num, min_len_threshold, gene_analysis=True)
+    rscu_dict = calculate_rscu(handle, genetic_table_num, min_len_threshold, gene_analysis=True)
     gene_names = list(rscu_dict.keys())
     contingency_table = pd.DataFrame(index=gene_names, columns=codons)
     for gene in gene_names:
         for codon in codons:
             contingency_table[codon][gene] = rscu_dict[gene][codon]
     pca = PCA(random_state=42, n_components=n_components)
     pca.fit(contingency_table)
```

### Comparing `CodonU-1.0.3/CodonU/cua_errors/no_prot_err.py` & `CodonU-1.0.4/CodonU/cua_errors/no_prot_err.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/cua_errors/nucleotide_err.py` & `CodonU-1.0.4/CodonU/cua_errors/nucleotide_err.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/extractor/extract_cds.py` & `CodonU-1.0.4/CodonU/extractor/extract_cds.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/extractor/extract_exome.py` & `CodonU-1.0.4/CodonU/extractor/extract_exome.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/extractor/extract_prot.py` & `CodonU-1.0.4/CodonU/extractor/extract_prot.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/extractor/internal_comp.py` & `CodonU-1.0.4/CodonU/extractor/internal_comp.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/file_handler/get_gb.py` & `CodonU-1.0.4/CodonU/file_handler/get_gb.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/file_handler/internal_comp.py` & `CodonU-1.0.4/CodonU/file_handler/internal_comp.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/file_handler/write_exome_fasta.py` & `CodonU-1.0.4/CodonU/file_handler/write_exome_fasta.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/file_handler/write_nucleotide_fasta.py` & `CodonU-1.0.4/CodonU/file_handler/write_nucleotide_fasta.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/file_handler/write_protein_fasta.py` & `CodonU-1.0.4/CodonU/file_handler/write_protein_fasta.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/phylogenetic_analysis/clustal_o.py` & `CodonU-1.0.4/CodonU/phylogenetic_analysis/clustal_o.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     :param bin_path: Path to the binary file of ClustalW
     :param handle: Handle to the file, or the filename as a string
     :param res_folder_path: The path of folder where the file will be saved
     """
     make_dir(res_folder_path)
     identifier = handle.split('/')[-1].split('.')[0]
-    report_file_name = f'{identifier}_aligned_o.nex'
+    report_file_name = f'{identifier}_aligned_o.fasta'
     report_file_path = join(res_folder_path, report_file_name)
     if not is_file(report_file_path) or is_file_empty(report_file_path):
         clustalO_cline = ClustalOmegaCommandline(bin_path, infile=handle, infmt='fasta', outfile=report_file_path,
                                                  outfmt='fasta', seqtype='DNA')
         cmd = clustalO_cline.__str__()
         subprocess.run(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-    print(f'The alignment file can be can be found at: {abspath(report_file_path)}')
+        print(f'The alignment file can be can be found at: {abspath(report_file_path)}')
```

### Comparing `CodonU-1.0.3/CodonU/phylogenetic_analysis/clustal_w.py` & `CodonU-1.0.4/CodonU/phylogenetic_analysis/clustal_w.py`

 * *Files identical despite different names*

```diff
@@ -18,8 +18,8 @@
     report_file_name = f'{identifier}_aligned_w.nex'
     report_file_path = join(res_folder_path, report_file_name)
     if not is_file(report_file_path) or is_file_empty(report_file_path):
         clustalW_cline = ClustalwCommandline(bin_path, infile=handle, outfile=report_file_path, output='NEXUS',
                                              outputtree='nexus')
         cmd = clustalW_cline.__str__()
         subprocess.run(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-    print(f'The alignment file can be can be found at: {abspath(report_file_path)}')
+        print(f'The alignment file can be can be found at: {abspath(report_file_path)}')
```

### Comparing `CodonU-1.0.3/CodonU/phylogenetic_analysis/generate_phylo_input.py` & `CodonU-1.0.4/CodonU/phylogenetic_analysis/generate_phylo_input.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/vizualizer/plot_enc.py` & `CodonU-1.0.4/CodonU/vizualizer/plot_enc.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/vizualizer/plot_funcs.py` & `CodonU-1.0.4/CodonU/vizualizer/plot_funcs.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/vizualizer/plot_mca_aa_aroma.py` & `CodonU-1.0.4/CodonU/vizualizer/plot_mca_aa_aroma.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/vizualizer/plot_mca_aa_gravy.py` & `CodonU-1.0.4/CodonU/vizualizer/plot_mca_aa_gravy.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/vizualizer/plot_mca_codon_freq.py` & `CodonU-1.0.4/CodonU/vizualizer/plot_mca_codon_freq.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/vizualizer/plot_mca_rscu.py` & `CodonU-1.0.4/CodonU/vizualizer/plot_mca_rscu.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/vizualizer/plot_neutrality.py` & `CodonU-1.0.4/CodonU/vizualizer/plot_neutrality.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/vizualizer/plot_phy_dnd.py` & `CodonU-1.0.4/CodonU/vizualizer/plot_phy_dnd.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU/vizualizer/plot_phy_nex.py` & `CodonU-1.0.4/CodonU/vizualizer/plot_phy_nex.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import matplotlib.pyplot as plt
 from CodonU.file_handler import make_dir
 from CodonU.file_handler.internal_comp import is_file_writeable
 
 
 def plot_phy_nex(handle: str, title: str = 'Phylogenetic Tree', save_image: bool = False, folder_path: str = 'Report'):
     """
-    Plots phylogenetic tree from dnd file
-    :param handle: Handle to the dnd file
+    Plots phylogenetic tree from nexus file
+    :param handle: Handle to the nexus file
     :param title: Title of the plot
     :param save_image: Options for saving the image (optional)
     :param folder_path: Folder path where image should be saved (optional)
     """
     cons = DistanceTreeConstructor()
     aln_file = read(open(handle), 'nexus')
     calc = DistanceCalculator('identity')
```

### Comparing `CodonU-1.0.3/CodonU/vizualizer/plot_pr2.py` & `CodonU-1.0.4/CodonU/vizualizer/plot_pr2.py`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/CodonU.egg-info/PKG-INFO` & `CodonU-1.0.4/CodonU.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodonU
-Version: 1.0.3
+Version: 1.0.4
 Summary: This package is designed for helping in genomic analysis
 Home-page: https://github.com/SouradiptoC/codon_usage
 Author: Souradipto Choudhuri
 Author-email: sourochaudhuri@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/SouradiptoC/codon_usage/issues
 Project-URL: Documentation, https://souradiptoc.github.io/CodonU/
```

### Comparing `CodonU-1.0.3/CodonU.egg-info/SOURCES.txt` & `CodonU-1.0.4/CodonU.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -59,9 +59,10 @@
 CodonU/vizualizer/plot_funcs.py
 CodonU/vizualizer/plot_mca_aa_aroma.py
 CodonU/vizualizer/plot_mca_aa_gravy.py
 CodonU/vizualizer/plot_mca_codon_freq.py
 CodonU/vizualizer/plot_mca_rscu.py
 CodonU/vizualizer/plot_neutrality.py
 CodonU/vizualizer/plot_phy_dnd.py
+CodonU/vizualizer/plot_phy_fas.py
 CodonU/vizualizer/plot_phy_nex.py
 CodonU/vizualizer/plot_pr2.py
```

### Comparing `CodonU-1.0.3/LICENSE.md` & `CodonU-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/PKG-INFO` & `CodonU-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodonU
-Version: 1.0.3
+Version: 1.0.4
 Summary: This package is designed for helping in genomic analysis
 Home-page: https://github.com/SouradiptoC/codon_usage
 Author: Souradipto Choudhuri
 Author-email: sourochaudhuri@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/SouradiptoC/codon_usage/issues
 Project-URL: Documentation, https://souradiptoc.github.io/CodonU/
```

### Comparing `CodonU-1.0.3/README.md` & `CodonU-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `CodonU-1.0.3/setup.py` & `CodonU-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         if not line.startswith(('"', "#", "-", "git+"))
     ]
 
 
 PACK_NAME = 'CodonU'
 AUTHOR_NAME = 'Souradipto Choudhuri'
 AUTHOR_EMAIL = 'sourochaudhuri@gmail.com'
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESC = 'This package is designed for helping in genomic analysis'
 
 setup(
     name='CodonU',
     version=VERSION,
     url='https://github.com/SouradiptoC/codon_usage',
     project_urls={
```

