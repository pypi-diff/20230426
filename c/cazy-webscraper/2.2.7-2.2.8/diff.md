# Comparing `tmp/cazy_webscraper-2.2.7.tar.gz` & `tmp/cazy_webscraper-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cazy_webscraper-2.2.7.tar", last modified: Mon Jan 16 12:14:20 2023, max compression
+gzip compressed data, was "cazy_webscraper-2.2.8.tar", last modified: Wed Apr 26 13:33:02 2023, max compression
```

## Comparing `cazy_webscraper-2.2.7.tar` & `cazy_webscraper-2.2.8.tar`

### file list

```diff
@@ -1,99 +1,130 @@
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.396415 cazy_webscraper-2.2.7/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1169 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/LICENSE
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    60072 2023-01-16 12:14:20.396415 cazy_webscraper-2.2.7/PKG-INFO
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    59024 2023-01-11 16:06:13.000000 cazy_webscraper-2.2.7/README.md
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.372414 cazy_webscraper-2.2.7/cazy_webscraper/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    10570 2023-01-15 16:30:38.000000 cazy_webscraper-2.2.7/cazy_webscraper/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.376414 cazy_webscraper-2.2.7/cazy_webscraper/api/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1450 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/api/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    22929 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/api/cw_query_database.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.376414 cazy_webscraper-2.2.7/cazy_webscraper/cazy/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    18900 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/cazy/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    13681 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/cazy_scraper.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.376414 cazy_webscraper-2.2.7/cazy_webscraper/crawler/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4585 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/crawler/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    20748 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/crawler/get_validation_data.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.376414 cazy_webscraper-2.2.7/cazy_webscraper/expand/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2391 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.376414 cazy_webscraper-2.2.7/cazy_webscraper/expand/extract_seqs/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1657 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/extract_seqs/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11472 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/extract_seqs/extract_db_seqs.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.380414 cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1495 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.380414 cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/genomes/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1533 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/genomes/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    24982 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/genomes/entrez.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    23749 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/genomes/get_genome_accs.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.380414 cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/sequences/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1508 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/sequences/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    25103 2023-01-16 11:57:01.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/sequences/get_genbank_sequences.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.380414 cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/taxonomy/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1538 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/taxonomy/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    28267 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/taxonomy/get_ncbi_taxs.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.380414 cazy_webscraper-2.2.7/cazy_webscraper/expand/gtdb/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8409 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/gtdb/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8962 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/gtdb/get_gtdb_tax.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.380414 cazy_webscraper-2.2.7/cazy_webscraper/expand/pdb/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1655 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/pdb/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6715 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/pdb/get_pdb_structures.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.384415 cazy_webscraper-2.2.7/cazy_webscraper/expand/uniprot/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1574 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/uniprot/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    24313 2023-01-11 16:06:13.000000 cazy_webscraper-2.2.7/cazy_webscraper/expand/uniprot/get_uniprot_data.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.384415 cazy_webscraper-2.2.7/cazy_webscraper/ncbi/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2554 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/ncbi/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.384415 cazy_webscraper-2.2.7/cazy_webscraper/ncbi/gene_names/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    10668 2023-01-11 10:36:45.000000 cazy_webscraper-2.2.7/cazy_webscraper/ncbi/gene_names/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.384415 cazy_webscraper-2.2.7/cazy_webscraper/ncbi/genomes/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8789 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/ncbi/genomes/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.384415 cazy_webscraper-2.2.7/cazy_webscraper/ncbi/sequences/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    12894 2023-01-16 10:53:33.000000 cazy_webscraper-2.2.7/cazy_webscraper/ncbi/sequences/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.384415 cazy_webscraper-2.2.7/cazy_webscraper/ncbi/taxonomy/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1486 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/ncbi/taxonomy/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    12045 2023-01-12 15:16:58.000000 cazy_webscraper-2.2.7/cazy_webscraper/ncbi/taxonomy/multiple_taxa.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.384415 cazy_webscraper-2.2.7/cazy_webscraper/sql/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1462 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.384415 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8480 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.388414 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1532 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    14773 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/add_cazyme_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4676 2023-01-11 16:06:13.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/add_genbank_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7642 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/add_genome_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     5492 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/add_gtdb_tax.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6604 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/add_ncbi_tax_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    18748 2023-01-11 10:36:45.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/add_uniprot_data.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.388414 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1535 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    16230 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_api_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6989 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_assemblies.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4774 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_records.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    13821 2023-01-11 16:06:13.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_selected_gbks.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3942 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_selected_pdbs.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    15484 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_table_dicts.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    13770 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_taxonomies.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    17953 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_orm.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.392415 cazy_webscraper-2.2.7/cazy_webscraper/utilities/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2319 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.392415 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parse_configuration/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    21390 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parse_configuration/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3907 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parse_configuration/cazy_class_synonym_dict.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.392415 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1493 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7011 2023-01-11 10:34:14.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/api_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8612 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/cazy_webscraper_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8408 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/extract_seq_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7991 2023-01-11 16:06:13.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/gbk_seq_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7903 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/get_genomes_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7891 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/get_gtdb_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8017 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/pdb_strctre_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7724 2023-01-03 19:20:11.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/tax_ncbi_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     9968 2023-01-11 10:34:14.000000 cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/uniprot_parser.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-01-16 12:14:20.376414 cazy_webscraper-2.2.7/cazy_webscraper.egg-info/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    60072 2023-01-16 12:14:20.000000 cazy_webscraper-2.2.7/cazy_webscraper.egg-info/PKG-INFO
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3316 2023-01-16 12:14:20.000000 cazy_webscraper-2.2.7/cazy_webscraper.egg-info/SOURCES.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)        1 2023-01-16 12:14:20.000000 cazy_webscraper-2.2.7/cazy_webscraper.egg-info/dependency_links.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)      672 2023-01-16 12:14:20.000000 cazy_webscraper-2.2.7/cazy_webscraper.egg-info/entry_points.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)      127 2023-01-16 12:14:20.000000 cazy_webscraper-2.2.7/cazy_webscraper.egg-info/requires.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       16 2023-01-16 12:14:20.000000 cazy_webscraper-2.2.7/cazy_webscraper.egg-info/top_level.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       38 2023-01-16 12:14:20.396415 cazy_webscraper-2.2.7/setup.cfg
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4337 2023-01-15 16:30:45.000000 cazy_webscraper-2.2.7/setup.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.252468 cazy_webscraper-2.2.8/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1169 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/LICENSE
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    60950 2023-04-26 13:33:02.252468 cazy_webscraper-2.2.8/PKG-INFO
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    59902 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/README.md
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.224468 cazy_webscraper-2.2.8/cazy_webscraper/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    10307 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.224468 cazy_webscraper-2.2.8/cazy_webscraper/api/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1450 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/api/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    22929 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/api/cw_query_database.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.224468 cazy_webscraper-2.2.8/cazy_webscraper/cazy/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    18900 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/cazy/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    13681 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/cazy_scraper.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.224468 cazy_webscraper-2.2.8/cazy_webscraper/crawler/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4585 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/crawler/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    20748 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/crawler/get_validation_data.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.224468 cazy_webscraper-2.2.8/cazy_webscraper/expand/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2391 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/extract_seqs/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1657 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/extract_seqs/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11472 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/extract_seqs/extract_db_seqs.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1495 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1533 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    24982 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/entrez.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    24100 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/get_genome_accs.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/sequences/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1508 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/sequences/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    25103 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/sequences/get_genbank_sequences.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/taxonomy/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1538 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/taxonomy/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    30711 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/taxonomy/get_ncbi_taxs.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/gtdb/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8409 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/gtdb/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     9413 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/gtdb/get_gtdb_tax.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/pdb/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1655 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/pdb/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6715 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/pdb/get_pdb_structures.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/expand/uniprot/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1574 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/uniprot/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    24313 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/uniprot/get_uniprot_data.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2554 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/gene_names/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    10668 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/gene_names/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/genomes/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8789 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/genomes/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/sequences/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    12894 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/sequences/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1486 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    21970 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/lineage.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    12045 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/multiple_taxa.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/sql/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1462 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8480 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.236468 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1532 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    14773 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_cazyme_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4676 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_genbank_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7642 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_genome_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5492 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_gtdb_tax.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7599 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_ncbi_tax_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    18748 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_uniprot_data.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.236468 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1535 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    16230 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_api_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6989 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_assemblies.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4774 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_records.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    13821 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_selected_gbks.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3942 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_selected_pdbs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    15484 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_table_dicts.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    13770 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_taxonomies.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    17953 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_orm.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.240468 cazy_webscraper-2.2.8/cazy_webscraper/utilities/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2319 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.240468 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parse_configuration/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    21390 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parse_configuration/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3907 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parse_configuration/cazy_class_synonym_dict.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.240468 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1493 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7011 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/api_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8612 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/cazy_webscraper_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8408 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/extract_seq_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7991 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/gbk_seq_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7903 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/get_genomes_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7891 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/get_gtdb_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8017 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/pdb_strctre_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7724 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/tax_ncbi_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     9968 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/uniprot_parser.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.224468 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    60950 2023-04-26 13:33:02.000000 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/PKG-INFO
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4088 2023-04-26 13:33:02.000000 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)        1 2023-04-26 13:33:02.000000 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)      672 2023-04-26 13:33:02.000000 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/entry_points.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)      127 2023-04-26 13:33:02.000000 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/requires.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       16 2023-04-26 13:33:02.000000 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/top_level.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       38 2023-04-26 13:33:02.252468 cazy_webscraper-2.2.8/setup.cfg
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4337 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/setup.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.252468 cazy_webscraper-2.2.8/tests/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5480 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_add_cazymes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    19877 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_api.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11219 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_cazy_init.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2944 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_crawler.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6180 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_cw_init.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1834 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_expand.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3540 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_extract_seqs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    21513 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_get_ncbi_tax.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    13574 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_gtdb.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3460 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_ncbi.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11718 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_ncbi_genomes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5398 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_orm.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7541 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_parse_config.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4412 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_parsers.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5970 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_pdb.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3398 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_ad_genbank.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5648 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_ad_genomes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5298 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_ad_gtdb.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5723 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_ad_ncbi_tax.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3406 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_interf_gd_get_records.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11054 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_interf_gd_get_tax.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5698 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_interface.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_queries.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4526 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_table_dicts.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6093 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_taxonomy.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6982 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_uniprot.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1827 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_utilities.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    18609 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_validation_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    23129 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_webscraper.py
```

### Comparing `cazy_webscraper-2.2.7/LICENSE` & `cazy_webscraper-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/PKG-INFO` & `cazy_webscraper-2.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cazy_webscraper
-Version: 2.2.7
+Version: 2.2.8
 Summary: A tool to automate retrieving data from CAZy, build a local CAZyme SQL database, and throughly interrogating the data. Also, automate retrieving protein data, sequences, EC numbers and structure files for specific datasets in the CAZyme database from UniProt, GenBank and PDB.
 Home-page: https://github.com/HobnobMancer/cazy_webscraper
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics protein webscraper
 Platform: Posix
@@ -33,15 +33,15 @@
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/cazy_webscraper/badges/version.svg)](https://anaconda.org/bioconda/cazy_webscraper)
 [![Anaconda-Update Badge](https://anaconda.org/bioconda/cazy_webscraper/badges/latest_release_date.svg)](https://anaconda.org/bioconda/cazy_webscraper)  
 [![pyani PyPi version](https://img.shields.io/pypi/v/cazy_webscraper "PyPI version")](https://pypi.python.org/pypi/cazy_webscraper)  
 [![Downloads](https://pepy.tech/badge/cazy-webscraper)](https://pepy.tech/project/cazy-webscraper)
 
 -------------------------------
 
-> `cazy_webscraper` version 1 is depracted. Please ensure you are using `cazy_webscraper` version 2 or newer.  
+> `cazy_webscraper` version 1 is depracted. Please ensure you are using version 2 or newer.  
 > `bioconda` installation is fixed for >= v2.1.3.1
 
 ## cazy_webscraper
 
 `cazy_webscraper` is an application and Python3 package for the automated retrieval of protein data from the [CAZy](http://wwww.cazy.org/) database. The code is distributed under the MIT license.
 
 **`cazy_webscraper` retrieves protein data from the [CAZy database](https://www.cazy.org) and stores the data in a local SQLite3 database.** This enables users to integrate the dataset into analytical pipelines, and interrogate the data in a manner unachievable through the CAZy website.
@@ -76,14 +76,20 @@
 - A FASTA file per extracted protein sequence
 - A local BLASTP database
 
 **The `cazy_webscraper` API facilitates interoggating the local CAZyme database.**
 
 Please see the [full documentation at ReadTheDocs](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest).
 
+## Documentation
+
+For a full description of the operation and examples of use, please see our paper in (BioRxiv)[https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1.full].
+
+> Hobbs, E. E. M., Gloster, T. M., and Pritchard, L. (2022) 'cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets', _bioRxiv_, [https://doi.org/10.1101/2022.12.02.518825](https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1.full)
+
 
 ## Table of Contents
 <!-- TOC -->
 - [`cazy_webscraper`](#cazy_webscraper)
 - [Citation](#citation)
 - [Best practice](#best-practice)
 - [Documentation](#documentation)
@@ -224,14 +230,16 @@
 
 To extract GenBank and/or UniProt protein sequences from a local CAZyme database, use the `cw_extract_db_seqs` command.
 
 #### PDB
 
 To protein structure files from PDB use the `cw_get_pdb_structures` command.
 
+**Note:** PDB structure files are retrieved for the PDB accessions that are *in* a local CAZyme database created using `cazy_webscraper`. A freshly built CAZyme database only contains NCBI protein accessions, taxonomic kingdoms, source organisms, and CAZy family annotations. Therefore, the `cw_get_uniprot_data` command must be used to retrieve PDB accessions from the UniProt database **prior** to using the `cw_get_pdb_structures` command.
+
 #### Interrogate the database
 
 To interrogate the database, use the `cw_query_database` command.
 
 ## Creating a local CAZyme database
 Command line options for `cazy_webscraper`, which is used to scrape CAZy and compile a local SQLite database. 
 Options are written in alphabetical order.
```

### Comparing `cazy_webscraper-2.2.7/README.md` & `cazy_webscraper-2.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/cazy_webscraper/badges/version.svg)](https://anaconda.org/bioconda/cazy_webscraper)
 [![Anaconda-Update Badge](https://anaconda.org/bioconda/cazy_webscraper/badges/latest_release_date.svg)](https://anaconda.org/bioconda/cazy_webscraper)  
 [![pyani PyPi version](https://img.shields.io/pypi/v/cazy_webscraper "PyPI version")](https://pypi.python.org/pypi/cazy_webscraper)  
 [![Downloads](https://pepy.tech/badge/cazy-webscraper)](https://pepy.tech/project/cazy-webscraper)
 
 -------------------------------
 
-> `cazy_webscraper` version 1 is depracted. Please ensure you are using `cazy_webscraper` version 2 or newer.  
+> `cazy_webscraper` version 1 is depracted. Please ensure you are using version 2 or newer.  
 > `bioconda` installation is fixed for >= v2.1.3.1
 
 ## cazy_webscraper
 
 `cazy_webscraper` is an application and Python3 package for the automated retrieval of protein data from the [CAZy](http://wwww.cazy.org/) database. The code is distributed under the MIT license.
 
 **`cazy_webscraper` retrieves protein data from the [CAZy database](https://www.cazy.org) and stores the data in a local SQLite3 database.** This enables users to integrate the dataset into analytical pipelines, and interrogate the data in a manner unachievable through the CAZy website.
@@ -53,14 +53,20 @@
 - A FASTA file per extracted protein sequence
 - A local BLASTP database
 
 **The `cazy_webscraper` API facilitates interoggating the local CAZyme database.**
 
 Please see the [full documentation at ReadTheDocs](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest).
 
+## Documentation
+
+For a full description of the operation and examples of use, please see our paper in (BioRxiv)[https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1.full].
+
+> Hobbs, E. E. M., Gloster, T. M., and Pritchard, L. (2022) 'cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets', _bioRxiv_, [https://doi.org/10.1101/2022.12.02.518825](https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1.full)
+
 
 ## Table of Contents
 <!-- TOC -->
 - [`cazy_webscraper`](#cazy_webscraper)
 - [Citation](#citation)
 - [Best practice](#best-practice)
 - [Documentation](#documentation)
@@ -201,14 +207,16 @@
 
 To extract GenBank and/or UniProt protein sequences from a local CAZyme database, use the `cw_extract_db_seqs` command.
 
 #### PDB
 
 To protein structure files from PDB use the `cw_get_pdb_structures` command.
 
+**Note:** PDB structure files are retrieved for the PDB accessions that are *in* a local CAZyme database created using `cazy_webscraper`. A freshly built CAZyme database only contains NCBI protein accessions, taxonomic kingdoms, source organisms, and CAZy family annotations. Therefore, the `cw_get_uniprot_data` command must be used to retrieve PDB accessions from the UniProt database **prior** to using the `cw_get_pdb_structures` command.
+
 #### Interrogate the database
 
 To interrogate the database, use the `cw_query_database` command.
 
 ## Creating a local CAZyme database
 Command line options for `cazy_webscraper`, which is used to scrape CAZy and compile a local SQLite database. 
 Options are written in alphabetical order.
```

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from pathlib import Path
 
 from saintBioutils.utilities.file_io import make_output_directory
 
 from cazy_webscraper.sql import sql_orm
 
 
-__version__ = "2.2.7"
+__version__ = "2.2.8"
 
 
 VERSION_INFO = f"cazy_webscraper version: {__version__}"
 
 
 CITATION_INFO = (
     "If you use cazy_webscraper in your work, please cite the following publication:\n"
@@ -107,20 +107,15 @@
     Total run time: {total_time}
 
     Version: {VERSION_INFO}
 
     For help with trouble shooting and operating cazy_webscraper please see the documentation:
     README: {WEBSITE}
     Documentation (including tutorials): {DOCUMENTATION}
-
-    We are interested in your views on the operation and addition of new features
-    to cazy_webscraper. Please get in touch with any issues, thanks, recommendations and
-    suggestions. Please submit your suggestions and comments at:
-    GitHub issues: {GITHUB_ISSUES}
-    Email: {AUTHOR_EMAIL}
+    GitHub Issues: {GITHUB_ISSUES}
 
     When publishing work that uses cazy_webscraper please cite:
     Citation: {CITATION_INFO}
     """
 
     if args.verbose:
         logger.info(message)
```

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/api/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/api/cw_query_database.py` & `cazy_webscraper-2.2.8/cazy_webscraper/api/cw_query_database.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/cazy/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/cazy/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/cazy_scraper.py` & `cazy_webscraper-2.2.8/cazy_webscraper/cazy_scraper.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/crawler/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/crawler/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/crawler/get_validation_data.py` & `cazy_webscraper-2.2.8/cazy_webscraper/crawler/get_validation_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/extract_seqs/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/extract_seqs/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/extract_seqs/extract_db_seqs.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/extract_seqs/extract_db_seqs.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/genomes/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/genomes/entrez.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/entrez.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/genomes/get_genome_accs.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/get_genome_accs.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,27 @@
         class_filters,
         family_filters,
         kingdom_filters,
         taxonomy_filter_dict,
         ec_filters,
     ) = parse_configuration.get_expansion_configuration(args)
 
+    with sql_orm.Session(bind=connection) as session:
+        sql_interface.log_scrape_in_db(
+            time_stamp,
+            config_dict,
+            kingdom_filters,
+            taxonomy_filter_dict,
+            ec_filters,
+            'NCBI Assembly',
+            'Genomic assemly accessions',
+            session,
+            args,
+        )
+
     logger.info(f"Retrieving Genbank records from the local db:\n{str(args.database)}")
 
     gbk_dict = get_gbks_of_interest(
         class_filters,
         family_filters,
         kingdom_filters,
         taxonomy_filter_dict,
```

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/sequences/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/sequences/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/sequences/get_genbank_sequences.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/sequences/get_genbank_sequences.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/taxonomy/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/taxonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/genbank/taxonomy/get_ncbi_taxs.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/taxonomy/get_ncbi_taxs.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,27 +43,33 @@
 import json
 import logging
 import sys
 
 import pandas as pd
 
 from datetime import datetime
+from http.client import IncompleteRead
 from typing import List, Optional
 
 from Bio import Entrez
+from Bio.Entrez.Parser import NotXMLError
 from saintBioutils.utilities.logger import config_logger
 from saintBioutils.utilities import file_io
 from saintBioutils.utilities.file_io import make_output_directory
 from saintBioutils.genbank import entrez_retry
 from tqdm import tqdm
 
 from cazy_webscraper import closing_message
 from cazy_webscraper.cazy_scraper import connect_existing_db
 from cazy_webscraper.expand import get_chunks_list
 from cazy_webscraper.ncbi import post_ids
+from cazy_webscraper.ncbi.taxonomy.lineage import (
+    retry_tax_retrieval,
+    get_lineage_data,
+)
 from cazy_webscraper.sql import sql_orm, sql_interface
 from cazy_webscraper.sql.sql_interface.add_data.add_ncbi_tax_data import (
     add_ncbi_taxonomies,
     update_genbank_ncbi_tax,
 )
 from cazy_webscraper.sql.sql_interface.get_data.get_selected_gbks import get_ids, get_genbank_accessions
 from cazy_webscraper.sql.sql_interface.get_data.get_records import get_user_uniprot_sequences
@@ -111,15 +117,15 @@
 
     with sql_orm.Session(bind=connection) as session:
         sql_interface.log_scrape_in_db(
             time_stamp,
             config_dict,
             kingdom_filters,
             taxonomy_filter_dict,
-            set(),  # ec_filters not applied when scraping CAZy
+            ec_filters,  # ec_filters not applied when scraping CAZy
             'NCBI Taxonomy',
             'NCBI taxonomc lineages',
             session,
             args,
         )
 
     if args.cache_dir is not None:  # use user defined cache dir
@@ -127,28 +133,31 @@
         logger.info("Building cache dir")
         make_output_directory(cache_dir, args.force, args.nodelete_cache)
     else:
         logger.info("Building cache dir")
         cache_dir = cache_dir / "ncbi_tax_retrieval"
         make_output_directory(cache_dir, args.force, args.nodelete_cache)
 
+    # Use Cache
     if args.use_lineage_cache is not None:
+        gbk_dict, tax_ids, prot_id_dict = None, None, None
         logger.info("Adding cached lineages to local CAZyme db")
         try:
             with open(args.use_lineage_cache, "r") as fh:
                 tax_prot_dict = json.load(fh)
         except FileNotFoundError:
             logger.error(
                 "Could not find lineage cache at \n"
                 f"{str(args.use_lineage_cache)}\n"
                 "Check path is correct\n"
                 "Terminating program"
             )
             sys.exit(1)
 
+    # Don't use cache
     else:
         gbk_dict = get_db_proteins(
             class_filters,
             family_filters,
             kingdom_filters,
             taxonomy_filter_dict,
             ec_filters,
@@ -268,287 +277,332 @@
 
     :param gbk_dict: dict of gbk accession and local db IDs
     :param cahce_dir: Path to cache dir
     :param args: cmd-line args parser
 
     Return set of NCBI Tax IDs, and dict of NCBI Prot ID valued by Gbk sequence accession
     """
+    tax_ids, prot_id_dict = set(), {}
     logger = logging.getLogger(__name__)
 
     if (args.use_tax_ids is not None) and (args.use_protein_ids is not None):
-        logger.info("Using only cached NCBI Tax and Protein IDs")
-        try:
-            with open(args.use_tax_ids, "r") as fh:
-                tax_ids = [_.replace("\n", "") for _ in fh.read().splitlines() if _ != "\n"]
-        except FileNotFoundError:
-            logger.error(
-                f"Could not find Tax ID cache at:\n{str(args.use_tax_ids)}\n"
-                "Check path is correct\n"
-                "Terminating program"
-            )
-            sys.exit(1)
-
-        try:
-            with open(args.use_protein_ids, "r") as fh:
-                cached_prot_data = fh.read().splitlines()
-        except FileNotFoundError:
-            logger.error(
-                f"Could not find NCBI Protein ID cache at:\n{str(args.use_protein_ids)}\n"
-                "Check path is correct\n"
-                "Terminating program"
-            )
-            sys.exit(1)
-
-        prot_id_dict = {}
-        for line in cached_prot_data:
-            if line == "\n":
-                continue
-            prot_id_dict[line.split("\t")[0].strip()] = line.split("\t")[1].strip().replace("\n", "")
+        # only use ids in files
+        tax_ids = load_tax_ids(args.use_tax_ids)
+        prot_id_dict = load_protein_ids(args.use_protein_ids)
 
         return tax_ids, prot_id_dict
 
-    else:
-        tax_ids, prot_id_dict = get_ncbi_tax_prot_ids(list(gbk_dict.keys()), cache_dir, args)
-
-        if args.use_tax_ids is not None:
-            logger.info("Using cached NCBI Tax IDs")
-            try:
-                with open(args.use_tax_ids, "r") as fh:
-                    tax_ids = [_.replace("\n", "") for _ in fh.read().splitlines() if _ != "\n"]
-            except FileNotFoundError:
-                logger.error(
-                    f"Could not find Tax ID cache at:\n{str(args.use_tax_ids)}\n"
-                    "Check path is correct\n"
-                    "Terminating program"
-                )
-                sys.exit(1)
-
-        if args.use_protein_ids is not None:
-            logger.info("Using cached NCBI Protein IDs")
-            try:
-                with open(args.use_protein_ids, "r") as fh:
-                    cached_prot_data = fh.read().splitlines()
-            except FileNotFoundError:
-                logger.error(
-                    f"Could not find NCBI Protein ID cache at:\n{str(args.use_protein_ids)}\n"
-                    "Check path is correct\n"
-                    "Terminating program"
-                )
-                sys.exit(1)
+    tax_ids, prot_id_dict = get_ncbi_tax_prot_ids(list(gbk_dict.keys()), cache_dir, args)
 
-            prot_id_dict = {}
-            for line in cached_prot_data:
-                if line == "\n":
-                    continue
-                prot_id_dict[line.split("\t")[0].strip()] = line.split("\t")[1].strip().replace("\n", "")
+    if args.use_tax_ids is not None:
+        tax_ids = load_tax_ids(args.use_tax_ids)
 
-    # Returns a set of NCBI Tax ids and dict {ncbi prot id: prot acc}
+    if args.use_protein_ids is not None:
+        prot_id_dict = load_protein_ids(args.use_protein_ids)
 
-    logger.info("Logging retrieved NCBI Taxonomy and Protein IDs")
+    logger.info("caching retrieved NCBI Taxonomy and Protein IDs")
     with open((cache_dir/"tax_ids.out"), "a") as fh:
         for tax_id in tax_ids:
             fh.write(f"{tax_id}\n")
 
-    with open((cache_dir/"protein_ncbi_ids.out"), "a") as fh:
-        for ncbi_prot_id in prot_id_dict:
-            fh.write(f"{ncbi_prot_id}\t{prot_id_dict[ncbi_prot_id]}\n")
+    if prot_id_dict is not None:
+        with open((cache_dir/"protein_ncbi_ids.out"), "a") as fh:
+            for ncbi_prot_id in prot_id_dict:
+                fh.write(f"{ncbi_prot_id}\t{prot_id_dict[ncbi_prot_id]}\n")
 
     return tax_ids, prot_id_dict
 
 
+def load_tax_ids(tax_id_path):
+    """Load NCBI taxonomy ids from plain text file
+
+    :param tax_id_path: Path, path to file of tax ids
+
+    Return list of tax ids
+    """
+    logger = logging.getLogger(__name__)
+    logger.warning(f"Use Tax IDs in {tax_id_path}")
+    try:
+        with open(tax_id_path, "r") as fh:
+            tax_ids = [_.replace("\n", "") for _ in fh.read().splitlines() if _ != "\n"]
+    except FileNotFoundError:
+        logger.error(
+            f"Could not find Tax ID cache at:\n{str(tax_id_path)}\n"
+            "Check path is correct\n"
+            "Terminating program"
+        )
+        sys.exit(1)
+
+    return tax_ids
+
+
+def load_protein_ids(prot_id_path):
+    """Load protein IDs and accessions from tab delimited file
+
+    :param prot_id_path: Path, path to tab delimited file
+
+    Return dict {ID: accession}
+    """
+    logger = logging.getLogger(__name__)
+    logger.warning(f"Use Protein IDs and accessions in {prot_id_path}")
+    try:
+        with open(prot_id_path, "r") as fh:
+            cached_prot_data = fh.read().splitlines()
+    except FileNotFoundError:
+        logger.error(
+            f"Could not find NCBI Protein ID cache at:\n{str(prot_id_path)}\n"
+            "Check path is correct\n"
+            "Terminating program"
+        )
+        sys.exit(1)
+
+    prot_id_dict = {}
+    for line in cached_prot_data:
+        if line == "\n":
+            continue
+        prot_id_dict[line.split("\t")[0].strip()] = line.split("\t")[1].strip().replace("\n", "")
+
+    prot_id_dict
+
+
 def get_ncbi_tax_prot_ids(protein_accessions, cache_dir, args):
     """Retrieve NCBI Taxonomy and Protein database IDs
 
+    Post the protein accession.
+    Then entrez.efetch the protein records to associate each accession with the correct id
+    Then entrez.elink to retrieve all linked taxonomy records - do no associated with the correct 
+    protein accesion at this point.
+
     :param protein_accessions: list of NCBI protein version accessions
     :param cache_dir: Path, path to cache directory
     :param args: cmd-line args parser
 
     Return set of NCBI Tax ids and dict {ncbi prot id: prot acc}
     """
     logger = logging.getLogger(__name__)
 
     # break up list into batches
     batches = get_chunks_list(protein_accessions, args.batch_size)
 
-    failed_batches = {}  # {batch: # of tries}
+    failed_batches = {}  # {protein: tries}
 
-    tax_ids = set()
+    tax_ids = set()  # set of all retrieve tax ids
 
-    protein_ncbi_ids = {}
+    protein_ncbi_ids = {}  # {ncdi prot id : ncbi prot acc}
 
-    for batch in tqdm(batches, desc="Getting NCBI Tax IDs"):
+    for batch in tqdm(batches, desc="Getting NCBI Protein and Taxonomy IDs"):
+        # post the IDs
+        try:
+            query_key, web_env = post_ids(batch, 'Protein', args)
+        except RuntimeError as err:
+            logger.warning(
+                "The batch of protein accessions contains an accession not in NCBI\n"
+                "Will parse the accessions individually later to identify the offending accession\n"
+                f"Batch:\n{batch}"
+            )
+            for protein in batch:
+                failed_batches[protein] = 0
+            continue
+        
+        if query_key is None:
+            for protein in batch:
+                failed_batches[protein] = 0
+            continue
+        
+        # fetch protein ids - associate prot id with prot acc
+        new_protein_ids = get_prot_ids(query_key, web_env, args)
+
+        if new_protein_ids is None:
+            for protein in batch:
+                failed_batches[protein] = 0
+            continue
 
-        new_tax_ids, new_prot_ids, failed_batches = get_ids_from_ncbi(batch, args, failed_batches)
+        protein_ncbi_ids.update(new_protein_ids)
 
-        tax_ids = tax_ids.union(new_tax_ids)
-        protein_ncbi_ids.update(new_prot_ids)
+        new_tax_ids = link_prot_taxs(query_key, web_env, args, batch)
 
-    failed_individuals = {}  # prot_acc: tries
+        if new_tax_ids is None:
+            for protein in batch:
+                failed_batches[protein] = 0
+            continue
+        
+        tax_ids = tax_ids.union(new_tax_ids)
 
-    if len(failed_batches.keys()) != 0:
-        for batch in tqdm(failed_batches, "Retrying failed batches"):
-            batch_proteins = failed_batches[batch]['proteins']
-            for prot in batch_proteins:
-                new_tax_ids, new_prot_ids, failed_individuals = get_ids_from_ncbi(
-                    [prot],
-                    args,
-                    failed_individuals,
-                )
+    # retry failed batches
+    if len(list(failed_batches.keys())) != 0:
+        logger.warning(
+            f"Retrying to retrieve Protein IDs and Taxonomy IDs for {len(list(failed_batches.keys()))} proteins"
+        )
+        while len(list(failed_batches.keys())):
+            for protein in failed_batches:
+                # post ids
+                try:
+                    query_key, web_env = post_ids([protein], 'Protein', args)
+                except RuntimeError as err:
+                    logger.warning(
+                        f"The protein accessions {protein} is not listed in NCBI\n"
+                        "Therefore not retrieve taxonomy data for this protein.\n"
+                        f"Error:\n{err}"
+                    )
+                    del failed_batches[protein]
+                    continue
+                
+                if query_key is None:
+                    failed_batches[protein] += 1
+                    if failed_batches[protein] >= args.retries:
+                        logger.warning(
+                            f"Ran out of connection reattempt for protein accession {protein} while posting IDs\n"
+                            "Therefore not retrieve taxonomy data for this protein."
+                        )
+                        del failed_batches[protein]
+                    continue
 
-                tax_ids = tax_ids.union(new_tax_ids)
-                protein_ncbi_ids.update(new_prot_ids)
+                # fetch prot ids - linked to acc
+                new_protein_ids = get_prot_ids(query_key, web_env, args)
 
-    failed_proteins = set()
+                if new_protein_ids is None:
+                    failed_batches[protein] += 1
+                    if failed_batches[protein] >= args.retries:
+                        logger.warning(
+                            f"Ran out of connection reattempt for protein accession {protein} while fetching Protein IDs\n"
+                            "Therefore not retrieve taxonomy data for this protein."
+                        )
+                        del failed_batches[protein]
+                    continue
 
-    if len(list(failed_individuals.keys())) != 0:
-        prots_to_retry = [failed_individuals[_]['proteins'] for _ in failed_individuals]
+                protein_ncbi_ids.update(new_protein_ids)
 
-        logger.warning(f"Retrying individual failed protein IDs")
+                # fetch linked tax ids - not linked to acc
+                new_tax_ids = link_prot_taxs(query_key, web_env, args, batch)
 
-        while len(list(failed_individuals.keys())) > 0:
-            for prot in prots_to_retry:
-                try:
-                    failed_individuals[prot]
-                except KeyError:
+                if new_tax_ids is None:
+                    failed_batches[protein] += 1
+                    if failed_batches[protein] >= args.retries:
+                        logger.warning(
+                            f"Ran out of connection reattempt for protein accession {protein} while fetching Tax IDs\n"
+                            "Therefore not retrieve taxonomy data for this protein."
+                        )
+                        del failed_batches[protein]
                     continue
-                except TypeError:
-                    try:
-                        failed_individuals[str(prot)]
-                    except KeyError:
-                        continue
-
-                new_tax_ids, new_prot_ids, failed_individuals = get_ids_from_ncbi(
-                    prot,
-                    args,
-                    failed_individuals,
-                )
-
+                
                 tax_ids = tax_ids.union(new_tax_ids)
-                protein_ncbi_ids.update(new_prot_ids)
 
-                try:
-                    if failed_individuals[prot] >= args.retries:
-                        del failed_individuals[prot]
-                        failed_proteins.add(prot)
-                except TypeError:
-                    if failed_individuals[str(prot)]['tries'] >= args.retries:
-                        del failed_individuals[str(prot)]
-                        failed_proteins.add(str(prot))
-
-    if len(failed_proteins) != 0:
-        logger.warning(f"Failed to retrieve lineage data for {len(failed_proteins)} proteins")
-        with open((cache_dir / "failed_protein_accs.txt"), "a") as fh:
-            for prot in failed_proteins:
-                fh.write(f"{prot}\n")
+    failed_prot_accs = [_ for _ in protein_accessions if _ not in set(protein_ncbi_ids.values())]
 
-    logger.info(f"Retrieved {len(tax_ids)} NCBI Taxonomy IDs")
+    if len(failed_prot_accs) != 0:
+        cache_file = cache_dir / "failed_to_retrieve_ids"
+        logger.warning(
+            f"Attempted to retrieve Protein IDs for {len(protein_accessions)} proteins accessions\n"
+            f"Retrieved {len(list(protein_ncbi_ids.keys()))} protein IDs\n"
+            f"Therefore, protein IDs were not retrieved for {len(failed_prot_accs)} protein accessions\n"
+            f"Writing accessions to cache file:{cache_file}"
+        )
+
+        with open(cache_file,'w') as fh:
+            for acc in failed_prot_accs:
+                fh.write(f"{acc}\n")
+    
+    else:
+        logger.warning(
+            f"Success: Attempted to retrieve Protein IDs for {len(protein_accessions)} proteins accessions\n"
+            f"and retrieved {len(list(protein_ncbi_ids.keys()))} protein IDs\n"
+            f"Therefore, retrieved a protein ID for all protein accessions"
+        )
 
     return tax_ids, protein_ncbi_ids
 
 
-def get_ids_from_ncbi(prots, args, failed_batches):
-    """Retrieve NCBI Taxonomy and Protein database IDs, for first time or retried attempts.
+def get_prot_ids(query_key, web_env, args):
+    """Retrieve protein records ids from the NCBI Protein database
 
-    :param protein_accessions: list of NCBI protein version accessions
-    :param args: cmd-line args parser
-    :param round: int, (1) first time, (2) second, (3) continued until reach retry limit
-    :param failed_batches: dict {batch/prots: #ofTries}
+    :param query_key: str, query key from entrez.epost of protein accessions
+    :param web_env: str, web environment from entrez.epost of protein accessions
+    :param args: CLI args parser
 
-    Return set of NCBI Tax ids and set of NCBI Prot ids, and failed_batches dict
+    Return dict {protein ID: protein accession} or None if fails
     """
     logger = logging.getLogger(__name__)
-
-    new_tax_ids, new_protein_ids = set(), set()
-
-    # post protein accessions
+    new_prot_ids = {}  # {id: acc}
     try:
-        query_key, web_env = post_ids(prots, 'Protein', args)
-    except RuntimeError:
-        logger.warning(f"Batch contained invalid protein version accession.\nBatch:\n{prots}")
-        key = str(prots)
-        try:
-            failed_batches[key]['tries'] += 1
-        except KeyError:
-            failed_batches[key] = {'proteins': prots, 'tries': 1}
-
-        return new_tax_ids, new_protein_ids, failed_batches
-
-    if query_key is None:
-        key = str(prots)
-        try:
-            failed_batches[key]['tries'] += 1
-        except KeyError:
-            failed_batches[key] = {'proteins': prots, 'tries': 1}
-
-        return new_tax_ids, new_protein_ids, failed_batches
-
-    # elink proteins to tax records
-    new_tax_ids, new_protein_ids, success = link_prot_taxs(query_key, web_env, args)
+        with entrez_retry(
+            args.retries,
+            Entrez.efetch,
+            query_key=query_key,
+            WebEnv=web_env,
+            db="Protein",
+            rettype='docsum',
+        ) as handle:
+            prot_records = Entrez.read(handle, validate=False)
 
-    if success is False:
+    except (TypeError, AttributeError, RuntimeError,  NotXMLError, IncompleteRead) as err:
         logger.warning(
-            f"Could not retrieve tax link for {','.join(prots)}."
+            "Could not rerieve records from the NCBI Protein database.\n"
+            "Will retry individual records later\n"
+            f"Error message retrieved:\n{err}"
         )
-        key = str(prots)
-        try:
-            failed_batches[key]['tries'] += 1
-        except KeyError:
-            failed_batches[key] = {'proteins': prots, 'tries': 1}
-
-        return new_tax_ids, new_protein_ids, failed_batches
-
-    new_prots_id_dict = {}  # protein ID: protein ACC
+        return None
 
-    for i in range(len(new_protein_ids)):
-        prot_acc = prots[i]
-        prot_id = new_protein_ids[i]
-        new_prots_id_dict[prot_id] = prot_acc
+    for record in prot_records:
+        prot_id = record['Id']
+        prot_acc = record['AccessionVersion']
+        new_prot_ids[prot_id] = prot_acc
 
-    return new_tax_ids, new_prots_id_dict, failed_batches
+    return new_prot_ids
 
 
-def link_prot_taxs(query_key, web_env, args):
+def link_prot_taxs(query_key, web_env, args, batch):
     """Get NCBI tax and protein IDs from elinking protein accs to tax records
 
     :param query_key: str, from Entrez epost
     :param web_env: str, from Entrez epost
     :param args: cmd-line args parser
+    :param batch: list of ncbi protein accs - used in error messages only
 
-    Return set of NCBI tax ids, and set of NCBI protein IDS, and bool TRUE if successful
+    Return set of NCBI tax ids or None if fails
     """
     logger = logging.getLogger(__name__)
 
-    tax_ids, protein_ids = set(), set()
+    tax_ids = set()
 
     try:
         with entrez_retry(
             args.retries,
             Entrez.elink,
             query_key=query_key,
             WebEnv=web_env,
             dbfrom="Protein",
             db="Taxonomy",
             linkname="protein_taxonomy",
         ) as handle:
             tax_links = Entrez.read(handle, validate=False)
-    except RuntimeError:
-        logger.warning("Batch included invalid NCBI protein ids")
-        return tax_ids, protein_ids, False
-
-    for result in tax_links:
+    except RuntimeError as err:
+        logger.warning(
+            "When retrieving taxonomy IDs, the batch included invalid NCBI protein ids\n"
+            "Will try batch components individually later, to identify the offending id\n"
+            f"Batch:\n{batch}\n"
+            f"Error:\n{err}"
+        )
+        return None
+    except (TypeError, AttributeError, NotXMLError, IncompleteRead) as err:
+        logger.warning(
+            "Failed to connect to NCBI.Entrez and download the Entrez.elink result\n"
+            "Will retry later"
+            f"Batch:\n{batch}\n"
+            f"Error:\n{err}"
+        )
+        return None
 
-        for prot_id in result['IdList']:
-            protein_ids.add(prot_id)
 
+    for result in tax_links:
         for item in result['LinkSetDb']:
             links = item['Link']
             for link in links:
                 tax_ids.add(link['Id'])
 
-    return tax_ids, list(protein_ids), True
+    return tax_ids
 
 
 def get_lineage_protein_data(tax_ids, prot_id_dict, gbk_dict, cache_dir, args):
     """Retrieve lineage data from NCBI Taxonomy and associated tax ids with protein ids
 
     :param tax_ids: set of ncbi tax record ids
     :param prot_id_dict: dict {prot_id: prot_acc}
@@ -556,67 +610,51 @@
     :param cache_dir: path to cache directory
     :param args: cmd-line args parser
 
     Return dict {tax_id: {linaege info, 'proteins' {local db protein ids}}
     """
     logger = logging.getLogger(__name__)
     tax_prot_dict = {}  # {ncbi tax id: {phylo_rank: str, proteins: [NCBI protein IDs]}}
+    all_failed_ids = set()  # tax ids for whom data could not be retrieved
 
     # retrieve lineage data from the NCBI Taxonomy database
+    lineage_dict, failed_ids = get_lineage_data(tax_ids, args)
+    logger.warning(
+        f"Queried NCBI with {len(tax_ids)} tax ids\n"
+        f"Retrieved lineages for {len(list(lineage_dict.keys()))} tax ids"
+    )
 
-    failed_lineage_ids = {}
-    lineage_dict = {}  # {ncbi tax id: {rank: str}}
-    completely_failed_tax_ids = set()
-
-    for tax_id in tqdm(tax_ids, desc="Retrieving lineages from NCBI"):
-        # get lineage information
-        lineage_dict, success = get_lineage(tax_id, lineage_dict, args)
-
-        if success is False:
-            failed_lineage_ids[tax_id] = 1  # marks the one failed attempt has been retried
-
-    if len(failed_lineage_ids) != 0:
-        logger.info(f"Retrying retrieving lineage data for failed NCBI Tax IDs")
-        while len(list(failed_lineage_ids.keys())) > 0:
-            for tax_id in tqdm(failed_lineage_ids, desc="Retrying retrieving NCBI lineages"):
-                lineage_dict, success = get_lineage(tax_id, lineage_dict, args)
-
-                if success is False:
-                    failed_lineage_ids[tax_id] += 1  # number of attempts that have failed
+    if len(list(lineage_dict.keys())) == 0:
+        return lineage_dict
 
-                if failed_lineage_ids[tax_id] > args.retries:
-                    logger.warning(
-                        f"Ran out of reattempts to get lineage data for ncbi tax {tax_id}"
-                    )
-                    del failed_lineage_ids[tax_id]
-                    completely_failed_tax_ids.add(f"{tax_id}\tCould not retrieve lineage data")
+    all_failed_ids = all_failed_ids.union(failed_ids)
 
+    # cache the retrieved lineages
     with open((cache_dir/"ncbi_lineages.json"), "w") as fh:
         json.dump(lineage_dict, fh)
 
-    # retrieve proteins linked to taxon record in NCBI
-    tax_prot_dict = {}
+    # retrieve proteins linked to taxon record in NCBI - for only tax ids where lineage data was retrieved
+    tax_prot_dict = {}  # {tax_id: {local db protein ids}}
     failed_linked_ids = {}
 
-    for tax_id in tqdm(tax_ids, desc="Link proteins to NCBI Tax record"):
-        if tax_id in completely_failed_tax_ids:
-            logger.warning(
-                f"Could not retrieved lineage for ncbi tax id {tax_id} "
-                "so not retrieving linked proteins for tax id"
-            )
-            continue
-        tax_prot_dict, success = get_tax_proteins(
+    # must query each tax id individually
+    # Batch querying Entrez.elink combines all the protein ids together for all tax ids
+    # therefore, could not separate out the protein ids for each tax id
+    # batch query returns ... DbFrom': 'taxonomy', 'IdList': ['55207', '204038', '1421545']}]
+    for tax_id in tqdm(lineage_dict, desc="Link proteins to NCBI Tax record"):    
+        new_tax_prot_dict, success = get_tax_proteins(
             tax_id,
             tax_prot_dict,
             prot_id_dict,
             gbk_dict,
             cache_dir,
             args,
         )
         # {tax_id: {local db protein ids}}
+        tax_prot_dict.update(new_tax_prot_dict)        
 
         if success is False:
             failed_linked_ids[tax_id] = 1  # first attempt to conenct failed
 
     if len(failed_linked_ids) != 0:
         logger.info(f"Retrying retrieving linked proteins for failed NCBI Tax IDs")
         while len(list(failed_linked_ids.keys())) > 0:
@@ -634,123 +672,37 @@
                     failed_linked_ids[tax_id] += 1  # number of attempts that have failed
 
                 if failed_linked_ids[tax_id] > args.retries:
                     logger.warning(
                         f"Ran out of reattempts to get linked proteins data for ncbi tax {tax_id}"
                     )
                     del failed_linked_ids[tax_id]
-                    completely_failed_tax_ids.add(f"{tax_id}\tCould not retrieve linked proteins")
+                    all_failed_ids.add(f"{tax_id}\tCould not retrieve linked proteins")
 
     # combine lineage data and proteins into a single dict
     for tax_id in tax_ids:
         try:
             lineage_dict[tax_id]['proteins'] = tax_prot_dict[tax_id]
         except KeyError:
             logger.error(
                 f"Did not retrieve lineage and/or linked proteins for ncbi tax id {tax_id}"
             )
-            if tax_id not in completely_failed_tax_ids:
-                completely_failed_tax_ids.add(
+            if tax_id not in all_failed_ids:
+                all_failed_ids.add(
                     f"{tax_id}\tCould not lineage data and/or retrieve linked proteins"
                 )
 
-    if len(completely_failed_tax_ids) != 0:
+    if len(all_failed_ids) != 0:
         with open((cache_dir / "failed_tax_ids.txt"), "a") as fh:
-            for tax_id in completely_failed_tax_ids:
+            for tax_id in all_failed_ids:
                 fh.write(f"{tax_id}\n")
 
     return lineage_dict
 
 
-def get_lineage(tax_id, lineage_dict, args):
-    """Retrieve lineage from NCBI taxonomy record, and add to lineage dict
-
-    :param tax_id: str, ncbi tax db id
-    :param lineage_dict: dict, {ncbi tax ID: {rank: str}}
-    :param args: cmd-line args parser
-
-    Return dict of lineage data and bool representing if eFetch was performed successfully
-    """
-    logger = logging.getLogger(__name__)
-
-    try:
-        with entrez_retry(
-            args.retries,
-            Entrez.efetch,
-            db="Taxonomy",
-            id=tax_id,
-        ) as handle:
-            tax_records = Entrez.read(handle, validate=False)
-
-    except (TypeError, AttributeError) as err:
-        logger.warning(f"Failed to fetch tax record from NCBI tax for id '{tax_id}'':\n{err}")
-        return lineage_dict, False
-
-    for record in tax_records:
-        record_id = record['TaxId']
-
-        # set lineage data to None
-        kingdom, phylum, tax_class, order, family, genus, species, strain = None, None, None, None, None, None, None, None
-
-        for i in record['LineageEx']:
-            rank = i['Rank']
-
-            if rank == 'superkingdom':
-                kingdom = i['ScientificName']
-
-            elif rank == 'phylum':
-                phylum = i['ScientificName']
-
-            elif rank == 'class':
-                tax_class = i['ScientificName']
-
-            elif rank == 'order':
-                order = i['ScientificName']
-
-            elif rank == 'family':
-                family = i['ScientificName']
-
-            elif rank == 'genus':
-                genus = i['ScientificName']
-
-            elif rank == 'species' or 'species group':
-                species = i['ScientificName']
-
-            elif rank == 'serotype' or 'strain':
-                strain = i['ScientificName']
-
-        scientific_name = record['ScientificName']
-
-        if genus is not None:
-            # drop genus from species name
-            if species is not None:
-                species = species.replace(genus, "").strip()
-
-            # extract strain from scientific name if not retrieved as rank
-            if species is not None and strain is None:
-                strain = scientific_name.replace(f"{genus} {species}", "").strip()
-
-            # extract species from the scientific name if not retrieved as rank
-            elif species is None:
-                species = scientific_name.replace(genus, "").strip()
-
-        lineage_dict[record_id] = {
-            'kingdom': kingdom,
-            'phylum': phylum,
-            'class': tax_class,
-            'order': order,
-            'family': family,
-            'genus': genus,
-            'species': species,
-            'strain': strain,
-        }
-
-    return lineage_dict, True
-
-
 def get_tax_proteins(tax_id, tax_prot_dict, prot_id_dict, gbk_dict, cache_dir, args):
     """Get the proteins linked to a tax id in NCBI, and link the tax id with the local db protein ids
 
     :param tax_id: str, NCBI tax db id
     :param tax_prot_dict: {ncbi tax id: {local db protein ids}}
     :param prot_id_dict: dict {protein ncbi id: prot acc}
     :param gbk_dict: dict, {prot acc: local db id}
@@ -806,9 +758,106 @@
                     continue
 
                 tax_prot_dict[tax_id].add(prot_local_db_id)
 
     return tax_prot_dict, True
 
 
+def check_for_failed_accessions(tax_prot_dict, gbk_dict, cache_dir):
+    """Check to see for how many proteins, taxonomy inforamtion could not be retrieved from NCBI
+    
+    :param tax_prot_dict: {tax_id: {linaege info, 'proteins' {local db protein ids}}
+    :param gbk_dict: dict of ncbi accessions paired with local db IDs
+    :param cache_dir: Path to cache directory
+    
+    Return list of accessions for whom tax data was not retrieved from ncbi
+    """
+    logger = logging.getLogger(__name__)
+    protein_accessions = list(gbk_dict.keys())
+
+    # tax_prot_dict = {tax_id: {linaege info, 'proteins' {local db protein ids}}
+    retrieved_protein_acc = []
+    for tax_id in tax_prot_dict:
+        for protein in tax_prot_dict[tax_id]['proteins']:
+            db_id = protein
+            for acc in gbk_dict:
+                if gbk_dict[acc] == db_id:
+                    protein_acc = acc
+                    break
+            
+            retrieved_protein_acc.append(protein_acc)
+
+    failed_accessions = [_ for _ in protein_accessions if _ not in retrieved_protein_acc]
+    if len(failed_accessions) != 0:
+        cache_file = cache_dir / "failed_to_retrieve_tax_data"
+        logger.warning(
+            f"Attempted to retrieve tax data for {len(protein_accessions)} proteins accessions\n"
+            f"Retrieved tax data for {len(retrieved_protein_acc)} proteins\n"
+            f"Therefore, tax data was not retrieved for {len(failed_accessions)} protein accessions\n"
+            f"Writing accessions to cache file:{cache_file}"
+        )
+
+        with open(cache_file,'w') as fh:
+            for acc in failed_accessions:
+                fh.write(f"{acc}\n")
+    
+    else:
+        logger.warning(
+            f"Success: Attempted to retrieve tax data for {len(protein_accessions)} proteins accessions\n"
+            f"and retrieved tax data for {len(retrieved_protein_acc)} proteins"
+        )
+
+    return failed_accessions
+
+
+def retry_failed_linkages(
+    class_filters,
+    family_filters,
+    kingdom_filters,
+    taxonomy_filter_dict,
+    ec_filters,
+    connection,
+    prot_id_dict,
+    cache_dir,
+    tax_prot_dict,
+    args,
+):
+    """Retry connecting proteins to taxonomy as single linkages
+    Used mostly for debugging retrieval of taxonomy info for all protein accessions
+    """
+    logger = logging.getLogger(__name__)
+    if gbk_dict is None:
+        logger.warning("Loading Genbanks table into dict to check for failed retrievals of tax data")
+        gbk_dict = get_db_proteins(
+            class_filters,
+            family_filters,
+            kingdom_filters,
+            taxonomy_filter_dict,
+            ec_filters,
+            connection,
+            args,
+        )
+        # gbk_dict = {gbk acc: db id}
+
+    # check to see for how many proteins a ncbi taxonomy record could not be retrieved
+    failed_accessions = check_for_failed_accessions(tax_prot_dict, gbk_dict, cache_dir)
+
+    if len(failed_accessions) != 0:
+        # check if failure was due to not getting a protein id from ncbi
+        
+        if prot_id_dict is not None:
+            failed_ids = [_ for _ in failed_accessions if _ not in list(prot_id_dict.values())]
+        else:
+            failed_ids = []
+        
+        if len(failed_ids) != 0:
+            logger.warning(f"Did not retrieved protein IDs for {len(failed_ids)} proteins:\n{failed_ids}")
+
+        # tax_prot_dict = {tax_id: {linaege info, 'proteins' {local db protein ids}}
+        # prot_id_dict = {ncbi prot id: prot acc}
+        tax_prot_dict = retry_tax_retrieval(failed_accessions, failed_ids, prot_id_dict, tax_prot_dict, args, cache_dir)
+
+    return tax_prot_dict
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/gtdb/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/gtdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/gtdb/get_gtdb_tax.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/gtdb/get_gtdb_tax.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,14 +62,16 @@
 from saintBioutils.utilities.file_io import make_output_directory
 from saintBioutils.utilities.logger import config_logger
 from tqdm import tqdm
 
 from cazy_webscraper import closing_message, connect_existing_db
 from cazy_webscraper.expand.gtdb import get_gtdb_data
 from cazy_webscraper.utilities.parse_configuration import get_expansion_configuration
+from cazy_webscraper.sql import sql_orm
+from cazy_webscraper.sql import sql_interface
 from cazy_webscraper.sql.sql_interface.get_data.get_table_dicts import (
     get_gbk_table_dict,
     get_uniprot_table_dict,
 )
 from cazy_webscraper.sql.sql_interface.get_data.get_records import (
     get_user_genbank_sequences,
     get_user_uniprot_sequences
@@ -119,14 +121,27 @@
         class_filters,
         family_filters,
         kingdom_filters,
         taxonomy_filter_dict,
         ec_filters,
     ) = get_expansion_configuration(args)
 
+    with sql_orm.Session(bind=connection) as session:
+        sql_interface.log_scrape_in_db(
+            time_stamp,
+            config_dict,
+            kingdom_filters,
+            taxonomy_filter_dict,
+            ec_filters,
+            'Genome Taxonomy DataBase (GTDB)',
+            'GTDB taxonomc lineages',
+            session,
+            args,
+        )
+
     # get the GenBank verion accessions and local db IDs of proteins matching the config criteria
     gbk_dict = get_gbks_of_interest(
         class_filters,
         family_filters,
         kingdom_filters,
         taxonomy_filter_dict,
         ec_filters,
```

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/pdb/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/pdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/pdb/get_pdb_structures.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/pdb/get_pdb_structures.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/uniprot/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/uniprot/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/expand/uniprot/get_uniprot_data.py` & `cazy_webscraper-2.2.8/cazy_webscraper/expand/uniprot/get_uniprot_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/ncbi/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/ncbi/gene_names/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/gene_names/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/ncbi/genomes/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/ncbi/sequences/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/sequences/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/ncbi/taxonomy/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/ncbi/taxonomy/multiple_taxa.py` & `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/multiple_taxa.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/add_cazyme_data.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_cazyme_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/add_genbank_data.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_genbank_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/add_genome_data.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_genome_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/add_gtdb_tax.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_gtdb_tax.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/add_ncbi_tax_data.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_ncbi_tax_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -146,21 +146,43 @@
 
     :param tax_prot_dict: dict {tax_id: lineage and protein data}
     :param connection: open connection to a sql db
     :param args: cmd-line args parser
 
     Return nothing
     """
+    logger = logging.getLogger(__name__)
+    
     db_ncbi_tax_table = get_ncbi_tax_table(connection)  # {ncbi_tax_id: local db id}
 
     if args.update_gbk:
         with connection.begin():
             for tax_id in tqdm(tax_prot_dict, desc="Updating Genbanks table"):
-                proteins = tax_prot_dict[int(tax_id)]['proteins']
-                tax_db_id = db_ncbi_tax_table[tax_id]
+                try:
+                    proteins = tax_prot_dict[int(tax_id)]['proteins']
+                except KeyError:
+                    try:
+                        proteins = tax_prot_dict[tax_id]['proteins']
+                    except KeyError:
+                        logger.warning(
+                            f"Could not retrieve proteins linked to tax id {tax_id}\n"
+                            "Will not update the respective records in the Genbanks table"
+                        )
+                        continue
+                try:    
+                    tax_db_id = db_ncbi_tax_table[int(tax_id)]
+                except KeyError:
+                    try:
+                        tax_db_id = db_ncbi_tax_table[str(tax_id)]
+                    except KeyError:
+                        logger.warning(
+                            f"Could not retrieve the local db ID for the NCBI tax id {tax_id}\n"
+                            "Will not update the respective records in the Genbanks table"
+                        )
+                        continue
                 for prot_db_id in proteins:
                     connection.execute(
                         text(
                             "UPDATE Genbanks "
                             f"SET ncbi_tax_id = {tax_db_id} "
                             f"WHERE genbank_id = '{prot_db_id}'"
                         )
```

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/add_data/add_uniprot_data.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_uniprot_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_api_data.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_api_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_assemblies.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_assemblies.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_records.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_records.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_selected_gbks.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_selected_gbks.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_selected_pdbs.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_selected_pdbs.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_table_dicts.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_table_dicts.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_interface/get_data/get_taxonomies.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_taxonomies.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/sql/sql_orm.py` & `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_orm.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/parse_configuration/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parse_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/parse_configuration/cazy_class_synonym_dict.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parse_configuration/cazy_class_synonym_dict.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/__init__.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/api_parser.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/api_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/cazy_webscraper_parser.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/cazy_webscraper_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/extract_seq_parser.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/extract_seq_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/gbk_seq_parser.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/gbk_seq_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/get_genomes_parser.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/get_genomes_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/get_gtdb_parser.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/get_gtdb_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/pdb_strctre_parser.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/pdb_strctre_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/tax_ncbi_parser.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/tax_ncbi_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper/utilities/parsers/uniprot_parser.py` & `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/uniprot_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper.egg-info/PKG-INFO` & `cazy_webscraper-2.2.8/cazy_webscraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cazy-webscraper
-Version: 2.2.7
+Version: 2.2.8
 Summary: A tool to automate retrieving data from CAZy, build a local CAZyme SQL database, and throughly interrogating the data. Also, automate retrieving protein data, sequences, EC numbers and structure files for specific datasets in the CAZyme database from UniProt, GenBank and PDB.
 Home-page: https://github.com/HobnobMancer/cazy_webscraper
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics protein webscraper
 Platform: Posix
@@ -33,15 +33,15 @@
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/cazy_webscraper/badges/version.svg)](https://anaconda.org/bioconda/cazy_webscraper)
 [![Anaconda-Update Badge](https://anaconda.org/bioconda/cazy_webscraper/badges/latest_release_date.svg)](https://anaconda.org/bioconda/cazy_webscraper)  
 [![pyani PyPi version](https://img.shields.io/pypi/v/cazy_webscraper "PyPI version")](https://pypi.python.org/pypi/cazy_webscraper)  
 [![Downloads](https://pepy.tech/badge/cazy-webscraper)](https://pepy.tech/project/cazy-webscraper)
 
 -------------------------------
 
-> `cazy_webscraper` version 1 is depracted. Please ensure you are using `cazy_webscraper` version 2 or newer.  
+> `cazy_webscraper` version 1 is depracted. Please ensure you are using version 2 or newer.  
 > `bioconda` installation is fixed for >= v2.1.3.1
 
 ## cazy_webscraper
 
 `cazy_webscraper` is an application and Python3 package for the automated retrieval of protein data from the [CAZy](http://wwww.cazy.org/) database. The code is distributed under the MIT license.
 
 **`cazy_webscraper` retrieves protein data from the [CAZy database](https://www.cazy.org) and stores the data in a local SQLite3 database.** This enables users to integrate the dataset into analytical pipelines, and interrogate the data in a manner unachievable through the CAZy website.
@@ -76,14 +76,20 @@
 - A FASTA file per extracted protein sequence
 - A local BLASTP database
 
 **The `cazy_webscraper` API facilitates interoggating the local CAZyme database.**
 
 Please see the [full documentation at ReadTheDocs](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest).
 
+## Documentation
+
+For a full description of the operation and examples of use, please see our paper in (BioRxiv)[https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1.full].
+
+> Hobbs, E. E. M., Gloster, T. M., and Pritchard, L. (2022) 'cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets', _bioRxiv_, [https://doi.org/10.1101/2022.12.02.518825](https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1.full)
+
 
 ## Table of Contents
 <!-- TOC -->
 - [`cazy_webscraper`](#cazy_webscraper)
 - [Citation](#citation)
 - [Best practice](#best-practice)
 - [Documentation](#documentation)
@@ -224,14 +230,16 @@
 
 To extract GenBank and/or UniProt protein sequences from a local CAZyme database, use the `cw_extract_db_seqs` command.
 
 #### PDB
 
 To protein structure files from PDB use the `cw_get_pdb_structures` command.
 
+**Note:** PDB structure files are retrieved for the PDB accessions that are *in* a local CAZyme database created using `cazy_webscraper`. A freshly built CAZyme database only contains NCBI protein accessions, taxonomic kingdoms, source organisms, and CAZy family annotations. Therefore, the `cw_get_uniprot_data` command must be used to retrieve PDB accessions from the UniProt database **prior** to using the `cw_get_pdb_structures` command.
+
 #### Interrogate the database
 
 To interrogate the database, use the `cw_query_database` command.
 
 ## Creating a local CAZyme database
 Command line options for `cazy_webscraper`, which is used to scrape CAZy and compile a local SQLite database. 
 Options are written in alphabetical order.
```

### Comparing `cazy_webscraper-2.2.7/cazy_webscraper.egg-info/entry_points.txt` & `cazy_webscraper-2.2.8/cazy_webscraper.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.7/setup.py` & `cazy_webscraper-2.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 # get long description from README.md
 with Path("README.md").open("r") as long_description_handle:
     long_description = long_description_handle.read()
 
 
 setuptools.setup(
     name="cazy_webscraper",
-    version="2.2.7",
+    version="2.2.8",
     # Metadata
     author="Emma E. M. Hobbs",
     author_email="eemh1@st-andrews.ac.uk",
     description="".join(
         [
             (
                 "A tool to automate retrieving data from CAZy, "
```

