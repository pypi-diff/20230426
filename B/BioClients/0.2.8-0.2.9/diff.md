# Comparing `tmp/BioClients-0.2.8.tar.gz` & `tmp/BioClients-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioClients-0.2.8.tar", last modified: Tue Oct 11 20:52:33 2022, max compression
+gzip compressed data, was "BioClients-0.2.9.tar", last modified: Fri Feb 17 16:29:44 2023, max compression
```

## Comparing `BioClients-0.2.8.tar` & `BioClients-0.2.9.tar`

### file list

```diff
@@ -1,407 +1,416 @@
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:33.240803 BioClients-0.2.8/
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     2023 2020-10-07 15:35:06.000000 BioClients-0.2.8/.gitignore
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.416777 BioClients-0.2.8/BioClients/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)       87 2021-01-20 16:36:37.000000 BioClients-0.2.8/BioClients/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.428777 BioClients-0.2.8/BioClients/allen/
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       76 2020-09-09 21:04:10.000000 BioClients-0.2.8/BioClients/allen/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.468777 BioClients-0.2.8/BioClients/allen/brain/
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     2710 2020-10-08 17:55:26.000000 BioClients-0.2.8/BioClients/allen/brain/Client.py
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     2790 2020-10-08 17:38:21.000000 BioClients-0.2.8/BioClients/allen/brain/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-09 20:43:23.000000 BioClients-0.2.8/BioClients/allen/brain/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.488777 BioClients-0.2.8/BioClients/amp/
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       93 2020-04-27 16:56:30.000000 BioClients-0.2.8/BioClients/amp/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.524777 BioClients-0.2.8/BioClients/amp/t2d/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2324 2020-04-27 16:56:30.000000 BioClients-0.2.8/BioClients/amp/t2d/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2264 2020-10-08 18:23:14.000000 BioClients-0.2.8/BioClients/amp/t2d/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-27 16:56:30.000000 BioClients-0.2.8/BioClients/amp/t2d/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.548777 BioClients-0.2.8/BioClients/bindingdb/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2341 2021-10-28 14:46:32.000000 BioClients-0.2.8/BioClients/bindingdb/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1691 2021-10-28 14:46:32.000000 BioClients-0.2.8/BioClients/bindingdb/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-09 21:25:39.000000 BioClients-0.2.8/BioClients/bindingdb/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.588777 BioClients-0.2.8/BioClients/biogrid/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3666 2022-07-22 14:18:43.000000 BioClients-0.2.8/BioClients/biogrid/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4122 2022-07-22 14:18:43.000000 BioClients-0.2.8/BioClients/biogrid/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-07-22 14:18:43.000000 BioClients-0.2.8/BioClients/biogrid/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.624777 BioClients-0.2.8/BioClients/bioregistry/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2520 2022-09-07 18:57:14.000000 BioClients-0.2.8/BioClients/bioregistry/Client.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     2032 2022-09-07 20:10:50.000000 BioClients-0.2.8/BioClients/bioregistry/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-07-22 14:20:03.000000 BioClients-0.2.8/BioClients/bioregistry/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.680778 BioClients-0.2.8/BioClients/brenda/
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     8008 2021-10-28 14:46:32.000000 BioClients-0.2.8/BioClients/brenda/Client.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)    16819 2021-10-28 14:46:32.000000 BioClients-0.2.8/BioClients/brenda/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-23 14:20:47.000000 BioClients-0.2.8/BioClients/brenda/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.740778 BioClients-0.2.8/BioClients/cas/
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     1740 2021-11-09 21:23:52.000000 BioClients-0.2.8/BioClients/cas/Client.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     1961 2021-11-10 16:10:30.000000 BioClients-0.2.8/BioClients/cas/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       64 2021-11-09 21:23:52.000000 BioClients-0.2.8/BioClients/cas/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.744778 BioClients-0.2.8/BioClients/cdc/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1816 2021-10-28 14:46:32.000000 BioClients-0.2.8/BioClients/cdc/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1327 2021-10-28 14:46:32.000000 BioClients-0.2.8/BioClients/cdc/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-09 20:19:09.000000 BioClients-0.2.8/BioClients/cdc/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.744778 BioClients-0.2.8/BioClients/cfde/
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)        0 2021-12-14 21:44:13.000000 BioClients-0.2.8/BioClients/cfde/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.760778 BioClients-0.2.8/BioClients/cfde/cfchemdb/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3455 2022-04-15 19:23:31.000000 BioClients-0.2.8/BioClients/cfde/cfchemdb/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5544 2022-04-15 20:11:47.000000 BioClients-0.2.8/BioClients/cfde/cfchemdb/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-12-14 21:52:03.000000 BioClients-0.2.8/BioClients/cfde/cfchemdb/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.820778 BioClients-0.2.8/BioClients/chebi/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2268 2022-05-03 15:06:39.000000 BioClients-0.2.8/BioClients/chebi/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3816 2022-05-03 15:14:25.000000 BioClients-0.2.8/BioClients/chebi/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-05-05 17:17:23.000000 BioClients-0.2.8/BioClients/chebi/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.856778 BioClients-0.2.8/BioClients/chem2bio2rdf/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3261 2021-10-28 14:46:32.000000 BioClients-0.2.8/BioClients/chem2bio2rdf/Client.py
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     9907 2020-05-28 17:35:10.000000 BioClients-0.2.8/BioClients/chem2bio2rdf/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      117 2020-04-27 16:56:30.000000 BioClients-0.2.8/BioClients/chem2bio2rdf/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.884778 BioClients-0.2.8/BioClients/chem2bio2rdf/slap/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3193 2020-04-27 16:56:30.000000 BioClients-0.2.8/BioClients/chem2bio2rdf/slap/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    30595 2020-10-08 17:55:51.000000 BioClients-0.2.8/BioClients/chem2bio2rdf/slap/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       59 2020-04-27 16:56:30.000000 BioClients-0.2.8/BioClients/chem2bio2rdf/slap/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.920779 BioClients-0.2.8/BioClients/chembl/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     7783 2021-10-28 14:46:32.000000 BioClients-0.2.8/BioClients/chembl/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6810 2020-04-07 20:01:15.000000 BioClients-0.2.8/BioClients/chembl/FetchByID.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6549 2020-10-08 18:24:20.000000 BioClients-0.2.8/BioClients/chembl/UnichemClient.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    37371 2022-06-24 22:04:07.000000 BioClients-0.2.8/BioClients/chembl/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/chembl/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.964779 BioClients-0.2.8/BioClients/chemidplus/
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     2487 2021-11-11 17:28:45.000000 BioClients-0.2.8/BioClients/chemidplus/Client.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     3501 2021-11-11 18:29:45.000000 BioClients-0.2.8/BioClients/chemidplus/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       75 2021-11-11 16:24:44.000000 BioClients-0.2.8/BioClients/chemidplus/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.032779 BioClients-0.2.8/BioClients/clinicaltrials/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2411 2022-06-22 15:01:24.000000 BioClients-0.2.8/BioClients/clinicaltrials/Client.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     3812 2022-06-22 15:27:51.000000 BioClients-0.2.8/BioClients/clinicaltrials/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-06-21 21:36:12.000000 BioClients-0.2.8/BioClients/clinicaltrials/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.060779 BioClients-0.2.8/BioClients/diseaseontology/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3939 2021-10-28 14:46:32.000000 BioClients-0.2.8/BioClients/diseaseontology/Client.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.084779 BioClients-0.2.8/BioClients/disgenet/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4030 2021-11-16 21:08:22.000000 BioClients-0.2.8/BioClients/disgenet/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     8399 2021-11-16 21:31:10.000000 BioClients-0.2.8/BioClients/disgenet/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2021-11-16 18:09:48.000000 BioClients-0.2.8/BioClients/disgenet/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.100779 BioClients-0.2.8/BioClients/dnorm/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4301 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/dnorm/Client.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)        0 2020-03-06 21:42:19.000000 BioClients-0.2.8/BioClients/dnorm/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.164780 BioClients-0.2.8/BioClients/drugcentral/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6593 2022-02-18 19:29:10.000000 BioClients-0.2.8/BioClients/drugcentral/Client.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     2136 2020-05-26 20:31:43.000000 BioClients-0.2.8/BioClients/drugcentral/Test.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    24247 2022-04-15 16:03:12.000000 BioClients-0.2.8/BioClients/drugcentral/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-20 17:16:25.000000 BioClients-0.2.8/BioClients/drugcentral/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.180780 BioClients-0.2.8/BioClients/emblebi/
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       27 2022-01-06 19:42:43.000000 BioClients-0.2.8/BioClients/emblebi/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.232780 BioClients-0.2.8/BioClients/emblebi/identifiers/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2973 2022-01-06 21:15:41.000000 BioClients-0.2.8/BioClients/emblebi/identifiers/Client.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     4507 2022-01-06 21:11:52.000000 BioClients-0.2.8/BioClients/emblebi/identifiers/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-01-06 19:43:09.000000 BioClients-0.2.8/BioClients/emblebi/identifiers/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.284780 BioClients-0.2.8/BioClients/emblebi/unichem/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2622 2022-06-16 14:56:32.000000 BioClients-0.2.8/BioClients/emblebi/unichem/Client.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     5484 2022-06-16 16:34:32.000000 BioClients-0.2.8/BioClients/emblebi/unichem/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-05-03 15:46:13.000000 BioClients-0.2.8/BioClients/emblebi/unichem/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.352780 BioClients-0.2.8/BioClients/ensembl/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2248 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/ensembl/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4160 2021-04-05 22:17:12.000000 BioClients-0.2.8/BioClients/ensembl/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       46 2021-01-20 16:40:52.000000 BioClients-0.2.8/BioClients/ensembl/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.392780 BioClients-0.2.8/BioClients/ensembl/biomart/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2701 2021-01-20 16:51:43.000000 BioClients-0.2.8/BioClients/ensembl/biomart/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2882 2021-01-20 16:51:00.000000 BioClients-0.2.8/BioClients/ensembl/biomart/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-01-20 13:59:24.000000 BioClients-0.2.8/BioClients/ensembl/biomart/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.412780 BioClients-0.2.8/BioClients/fda/
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       19 2020-03-06 21:42:19.000000 BioClients-0.2.8/BioClients/fda/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.464781 BioClients-0.2.8/BioClients/fda/aer/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3312 2021-08-03 22:03:40.000000 BioClients-0.2.8/BioClients/fda/aer/Client.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     9980 2021-08-06 00:00:44.000000 BioClients-0.2.8/BioClients/fda/aer/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-06 21:42:19.000000 BioClients-0.2.8/BioClients/fda/aer/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.484781 BioClients-0.2.8/BioClients/geneontology/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1813 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/geneontology/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1677 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/geneontology/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/geneontology/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.520781 BioClients-0.2.8/BioClients/glygen/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2171 2021-12-02 17:30:18.000000 BioClients-0.2.8/BioClients/glygen/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3592 2021-12-02 19:03:33.000000 BioClients-0.2.8/BioClients/glygen/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-05-05 21:25:28.000000 BioClients-0.2.8/BioClients/glygen/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.588781 BioClients-0.2.8/BioClients/gwascatalog/
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     2773 2021-12-14 16:30:12.000000 BioClients-0.2.8/BioClients/gwascatalog/Client.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)    10580 2022-01-31 16:12:16.000000 BioClients-0.2.8/BioClients/gwascatalog/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-11 23:32:44.000000 BioClients-0.2.8/BioClients/gwascatalog/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.612781 BioClients-0.2.8/BioClients/hugo/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2944 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/hugo/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4203 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/hugo/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-06 21:42:19.000000 BioClients-0.2.8/BioClients/hugo/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.624781 BioClients-0.2.8/BioClients/humanbase/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     7183 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/humanbase/Client.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)        0 2020-03-06 21:42:19.000000 BioClients-0.2.8/BioClients/humanbase/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.692782 BioClients-0.2.8/BioClients/icite/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1922 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/icite/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2236 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/icite/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-07 20:01:15.000000 BioClients-0.2.8/BioClients/icite/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.800782 BioClients-0.2.8/BioClients/idg/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2546 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/idg/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2902 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/idg/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       82 2020-11-20 21:40:05.000000 BioClients-0.2.8/BioClients/idg/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:27.972782 BioClients-0.2.8/BioClients/idg/pharos/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2204 2021-09-10 14:55:02.000000 BioClients-0.2.8/BioClients/idg/pharos/Client.py
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     2051 2021-12-17 00:01:25.000000 BioClients-0.2.8/BioClients/idg/pharos/ClientGql.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3308 2021-09-10 14:55:02.000000 BioClients-0.2.8/BioClients/idg/pharos/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-09-09 15:44:02.000000 BioClients-0.2.8/BioClients/idg/pharos/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:28.052783 BioClients-0.2.8/BioClients/idg/rss/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1866 2020-11-20 21:40:05.000000 BioClients-0.2.8/BioClients/idg/rss/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1723 2020-11-20 21:40:05.000000 BioClients-0.2.8/BioClients/idg/rss/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-11-20 21:40:05.000000 BioClients-0.2.8/BioClients/idg/rss/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:28.108783 BioClients-0.2.8/BioClients/idg/tcrd/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6665 2022-02-18 17:48:56.000000 BioClients-0.2.8/BioClients/idg/tcrd/Client.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)    19503 2022-06-23 19:50:54.000000 BioClients-0.2.8/BioClients/idg/tcrd/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-10-20 20:58:20.000000 BioClients-0.2.8/BioClients/idg/tcrd/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:28.284784 BioClients-0.2.8/BioClients/idg/tiga/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4278 2022-02-18 19:39:14.000000 BioClients-0.2.8/BioClients/idg/tiga/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4305 2021-09-23 21:24:28.000000 BioClients-0.2.8/BioClients/idg/tiga/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2021-09-22 22:00:16.000000 BioClients-0.2.8/BioClients/idg/tiga/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:28.444784 BioClients-0.2.8/BioClients/idg/tinx/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4093 2020-11-20 21:40:05.000000 BioClients-0.2.8/BioClients/idg/tinx/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    14947 2020-11-20 21:40:05.000000 BioClients-0.2.8/BioClients/idg/tinx/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-20 17:09:28.000000 BioClients-0.2.8/BioClients/idg/tinx/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:28.480785 BioClients-0.2.8/BioClients/iuphar/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5895 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/iuphar/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    12307 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/iuphar/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/iuphar/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:28.512785 BioClients-0.2.8/BioClients/jensenlab/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2070 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/jensenlab/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2235 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/jensenlab/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-27 16:56:30.000000 BioClients-0.2.8/BioClients/jensenlab/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:28.548785 BioClients-0.2.8/BioClients/lincs/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2944 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/lincs/Client.py
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     5929 2020-10-08 17:53:36.000000 BioClients-0.2.8/BioClients/lincs/Client_lincscloud.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6684 2022-04-13 19:33:09.000000 BioClients-0.2.8/BioClients/lincs/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-05-05 15:28:07.000000 BioClients-0.2.8/BioClients/lincs/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:28.696785 BioClients-0.2.8/BioClients/lincs/clue/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4942 2020-11-25 17:56:33.000000 BioClients-0.2.8/BioClients/lincs/clue/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    11205 2020-11-25 17:56:33.000000 BioClients-0.2.8/BioClients/lincs/clue/Utils.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:28.744785 BioClients-0.2.8/BioClients/lincs/sigcom/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1924 2022-04-13 19:59:02.000000 BioClients-0.2.8/BioClients/lincs/sigcom/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1175 2022-04-13 19:50:07.000000 BioClients-0.2.8/BioClients/lincs/sigcom/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-04-13 19:36:10.000000 BioClients-0.2.8/BioClients/lincs/sigcom/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:28.832786 BioClients-0.2.8/BioClients/maayanlab/
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)        0 2021-06-29 14:35:40.000000 BioClients-0.2.8/BioClients/maayanlab/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:28.908786 BioClients-0.2.8/BioClients/maayanlab/archs4/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1267 2021-06-28 21:58:02.000000 BioClients-0.2.8/BioClients/maayanlab/archs4/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1252 2021-06-28 21:55:32.000000 BioClients-0.2.8/BioClients/maayanlab/archs4/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-06-28 21:53:00.000000 BioClients-0.2.8/BioClients/maayanlab/archs4/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.032787 BioClients-0.2.8/BioClients/maayanlab/harmonizome/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1825 2021-06-28 21:52:47.000000 BioClients-0.2.8/BioClients/maayanlab/harmonizome/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2133 2021-06-28 21:52:02.000000 BioClients-0.2.8/BioClients/maayanlab/harmonizome/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-27 16:56:30.000000 BioClients-0.2.8/BioClients/maayanlab/harmonizome/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.064787 BioClients-0.2.8/BioClients/medline/
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)        0 2021-04-15 20:38:22.000000 BioClients-0.2.8/BioClients/medline/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.088787 BioClients-0.2.8/BioClients/medline/connect/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3107 2021-04-15 20:39:31.000000 BioClients-0.2.8/BioClients/medline/connect/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2228 2021-04-15 20:37:11.000000 BioClients-0.2.8/BioClients/medline/connect/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2021-04-15 20:32:33.000000 BioClients-0.2.8/BioClients/medline/connect/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.136787 BioClients-0.2.8/BioClients/medline/genetics/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3014 2021-04-15 20:43:50.000000 BioClients-0.2.8/BioClients/medline/genetics/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5131 2021-04-15 20:28:15.000000 BioClients-0.2.8/BioClients/medline/genetics/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-04-15 19:00:20.000000 BioClients-0.2.8/BioClients/medline/genetics/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.240787 BioClients-0.2.8/BioClients/mesh/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2606 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/mesh/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3904 2021-05-18 17:02:28.000000 BioClients-0.2.8/BioClients/mesh/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/mesh/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.424788 BioClients-0.2.8/BioClients/monarch/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3604 2020-10-08 17:52:16.000000 BioClients-0.2.8/BioClients/monarch/Biolink.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4603 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/monarch/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     8134 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/monarch/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-22 19:18:52.000000 BioClients-0.2.8/BioClients/monarch/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.468788 BioClients-0.2.8/BioClients/mygene/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1962 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/mygene/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1353 2021-11-16 15:41:45.000000 BioClients-0.2.8/BioClients/mygene/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-09 19:40:04.000000 BioClients-0.2.8/BioClients/mygene/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.504788 BioClients-0.2.8/BioClients/ncbo/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2369 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/ncbo/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2317 2021-02-19 15:28:19.000000 BioClients-0.2.8/BioClients/ncbo/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-02-19 15:28:19.000000 BioClients-0.2.8/BioClients/ncbo/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.616789 BioClients-0.2.8/BioClients/omim/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4527 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/omim/Client.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)        0 2020-03-06 21:42:19.000000 BioClients-0.2.8/BioClients/omim/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.672789 BioClients-0.2.8/BioClients/openphacts/
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     3679 2022-06-23 16:48:03.000000 BioClients-0.2.8/BioClients/openphacts/Client.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     8922 2022-06-23 16:50:29.000000 BioClients-0.2.8/BioClients/openphacts/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-06-23 15:47:27.000000 BioClients-0.2.8/BioClients/openphacts/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.824790 BioClients-0.2.8/BioClients/opentargets/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3067 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/opentargets/Client.py
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     4254 2020-06-19 18:04:44.000000 BioClients-0.2.8/BioClients/opentargets/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-06-19 18:04:44.000000 BioClients-0.2.8/BioClients/opentargets/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.836790 BioClients-0.2.8/BioClients/panther/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4018 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/panther/Client.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)        0 2020-04-16 18:00:39.000000 BioClients-0.2.8/BioClients/panther/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.844790 BioClients-0.2.8/BioClients/pdb/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2918 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/pdb/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    10849 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/pdb/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-06 21:42:19.000000 BioClients-0.2.8/BioClients/pdb/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:29.972790 BioClients-0.2.8/BioClients/pubchem/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5041 2022-01-24 16:19:41.000000 BioClients-0.2.8/BioClients/pubchem/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    35038 2022-07-22 20:57:14.000000 BioClients-0.2.8/BioClients/pubchem/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      103 2020-04-13 20:27:56.000000 BioClients-0.2.8/BioClients/pubchem/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:30.100791 BioClients-0.2.8/BioClients/pubchem/ftp/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1995 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/pubchem/ftp/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6666 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/pubchem/ftp/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/pubchem/ftp/__init__.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    15202 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_actives.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5629 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_assay_fetch.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4221 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_assay_results.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     7900 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_assay_search.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6583 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_assaysim.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     9488 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_compound_assaystats.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     9080 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_gini_index.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:30.156791 BioClients-0.2.8/BioClients/pubchem/rdf/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     9185 2020-10-08 17:57:09.000000 BioClients-0.2.8/BioClients/pubchem/rdf/Client.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)        0 2020-04-07 20:01:15.000000 BioClients-0.2.8/BioClients/pubchem/rdf/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:30.268791 BioClients-0.2.8/BioClients/pubchem/soap/
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     6328 2022-01-25 21:22:25.000000 BioClients-0.2.8/BioClients/pubchem/soap/Client.py
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)    15140 2022-01-25 20:45:35.000000 BioClients-0.2.8/BioClients/pubchem/soap/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2022-01-25 16:45:41.000000 BioClients-0.2.8/BioClients/pubchem/soap/__init__.py
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     6747 2020-06-03 16:30:16.000000 BioClients-0.2.8/BioClients/pubchem/soap/pug_aids2assays.py
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     6638 2020-06-03 16:30:16.000000 BioClients-0.2.8/BioClients/pubchem/soap/pug_ids2mols.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     9796 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/pubchem/soap/pug_substance_search.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:30.312791 BioClients-0.2.8/BioClients/pubmed/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     8705 2020-10-01 21:22:56.000000 BioClients-0.2.8/BioClients/pubmed/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)        0 2020-04-07 20:01:15.000000 BioClients-0.2.8/BioClients/pubmed/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:30.364792 BioClients-0.2.8/BioClients/pubtator/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2645 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/pubtator/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1669 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/pubtator/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-07 20:01:15.000000 BioClients-0.2.8/BioClients/pubtator/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:30.520792 BioClients-0.2.8/BioClients/reactome/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3226 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/reactome/Client.py
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     1108 2020-03-09 15:16:21.000000 BioClients-0.2.8/BioClients/reactome/SMBL_utils.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     7251 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/reactome/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       48 2020-03-09 15:38:06.000000 BioClients-0.2.8/BioClients/reactome/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:30.628793 BioClients-0.2.8/BioClients/rxnorm/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5836 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/rxnorm/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    11857 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/rxnorm/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-07 20:01:15.000000 BioClients-0.2.8/BioClients/rxnorm/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:30.676793 BioClients-0.2.8/BioClients/stringdb/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3747 2022-08-26 22:06:36.000000 BioClients-0.2.8/BioClients/stringdb/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5086 2022-08-26 22:06:42.000000 BioClients-0.2.8/BioClients/stringdb/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-11-20 21:40:05.000000 BioClients-0.2.8/BioClients/stringdb/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:30.720793 BioClients-0.2.8/BioClients/tcga/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2110 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/tcga/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4889 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/tcga/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-28 16:33:19.000000 BioClients-0.2.8/BioClients/tcga/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:30.744793 BioClients-0.2.8/BioClients/umls/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6854 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/umls/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    19343 2021-04-16 21:05:21.000000 BioClients-0.2.8/BioClients/umls/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-27 17:01:05.000000 BioClients-0.2.8/BioClients/umls/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:30.860794 BioClients-0.2.8/BioClients/uniprot/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1938 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/uniprot/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1661 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/uniprot/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-06 21:42:19.000000 BioClients-0.2.8/BioClients/uniprot/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:30.908794 BioClients-0.2.8/BioClients/util/
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      112 2020-10-21 17:44:43.000000 BioClients-0.2.8/BioClients/util/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:31.008794 BioClients-0.2.8/BioClients/util/db/
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     1549 2022-02-18 18:16:05.000000 BioClients-0.2.8/BioClients/util/db/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2022-02-18 17:39:54.000000 BioClients-0.2.8/BioClients/util/db/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:31.080794 BioClients-0.2.8/BioClients/util/graphql/
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)      728 2021-12-17 00:03:23.000000 BioClients-0.2.8/BioClients/util/graphql/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-12-16 21:47:54.000000 BioClients-0.2.8/BioClients/util/graphql/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:31.136795 BioClients-0.2.8/BioClients/util/hdf/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1760 2021-06-28 21:43:01.000000 BioClients-0.2.8/BioClients/util/hdf/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-06-28 21:59:50.000000 BioClients-0.2.8/BioClients/util/hdf/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:31.260795 BioClients-0.2.8/BioClients/util/igraph/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     8378 2022-02-08 22:02:33.000000 BioClients-0.2.8/BioClients/util/igraph/App.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    17764 2022-02-08 22:04:07.000000 BioClients-0.2.8/BioClients/util/igraph/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-12-06 15:00:46.000000 BioClients-0.2.8/BioClients/util/igraph/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:31.508796 BioClients-0.2.8/BioClients/util/neo4j/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2509 2022-07-27 16:21:13.000000 BioClients-0.2.8/BioClients/util/neo4j/App.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1717 2022-07-27 16:21:13.000000 BioClients-0.2.8/BioClients/util/neo4j/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2022-07-26 15:37:07.000000 BioClients-0.2.8/BioClients/util/neo4j/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:31.556796 BioClients-0.2.8/BioClients/util/obo/
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)      808 2022-01-26 17:32:05.000000 BioClients-0.2.8/BioClients/util/obo/App.py
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     1920 2022-01-26 17:30:31.000000 BioClients-0.2.8/BioClients/util/obo/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2022-01-26 17:28:15.000000 BioClients-0.2.8/BioClients/util/obo/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:31.668797 BioClients-0.2.8/BioClients/util/pandas/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     7554 2022-10-11 18:51:33.000000 BioClients-0.2.8/BioClients/util/pandas/App.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3482 2021-09-03 22:00:41.000000 BioClients-0.2.8/BioClients/util/pandas/Csv2Html.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2535 2021-09-09 14:38:00.000000 BioClients-0.2.8/BioClients/util/pandas/Csv2Markdown.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2553 2022-02-08 20:33:58.000000 BioClients-0.2.8/BioClients/util/pandas/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-06-28 22:00:16.000000 BioClients-0.2.8/BioClients/util/pandas/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:31.832797 BioClients-0.2.8/BioClients/util/rdf/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1644 2022-04-01 19:25:45.000000 BioClients-0.2.8/BioClients/util/rdf/App.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2099 2022-04-01 19:24:45.000000 BioClients-0.2.8/BioClients/util/rdf/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2022-03-23 13:55:45.000000 BioClients-0.2.8/BioClients/util/rdf/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:31.928798 BioClients-0.2.8/BioClients/util/rest/
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     4373 2020-10-08 16:50:07.000000 BioClients-0.2.8/BioClients/util/rest/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-10-08 17:36:38.000000 BioClients-0.2.8/BioClients/util/rest/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:31.980798 BioClients-0.2.8/BioClients/util/sparql/
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     3217 2022-07-28 21:41:58.000000 BioClients-0.2.8/BioClients/util/sparql/Client.py
--rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     5322 2022-07-28 21:15:41.000000 BioClients-0.2.8/BioClients/util/sparql/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-11 13:53:06.000000 BioClients-0.2.8/BioClients/util/sparql/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:32.056798 BioClients-0.2.8/BioClients/util/xml/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4414 2020-10-06 19:53:19.000000 BioClients-0.2.8/BioClients/util/xml/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-06-28 21:59:54.000000 BioClients-0.2.8/BioClients/util/xml/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:32.092798 BioClients-0.2.8/BioClients/util/yaml/
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      411 2020-10-21 17:44:43.000000 BioClients-0.2.8/BioClients/util/yaml/Utils.py
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-10-21 17:44:43.000000 BioClients-0.2.8/BioClients/util/yaml/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:32.144799 BioClients-0.2.8/BioClients/wikidata/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1844 2022-08-17 21:12:23.000000 BioClients-0.2.8/BioClients/wikidata/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2390 2022-08-17 20:59:30.000000 BioClients-0.2.8/BioClients/wikidata/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-11 15:42:13.000000 BioClients-0.2.8/BioClients/wikidata/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:32.292799 BioClients-0.2.8/BioClients/wikipathways/
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2733 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/wikipathways/Client.py
--rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1900 2021-10-28 14:46:33.000000 BioClients-0.2.8/BioClients/wikipathways/Utils.py
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-09 19:05:50.000000 BioClients-0.2.8/BioClients/wikipathways/__init__.py
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:26.428777 BioClients-0.2.8/BioClients.egg-info/
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     4510 2022-10-11 20:52:25.000000 BioClients-0.2.8/BioClients.egg-info/PKG-INFO
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     9018 2022-10-11 20:52:26.000000 BioClients-0.2.8/BioClients.egg-info/SOURCES.txt
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)        1 2022-10-11 20:52:25.000000 BioClients-0.2.8/BioClients.egg-info/dependency_links.txt
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       11 2022-10-11 20:52:25.000000 BioClients-0.2.8/BioClients.egg-info/top_level.txt
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     7048 2020-04-09 14:30:34.000000 BioClients-0.2.8/LICENSE
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     4510 2022-10-11 20:52:33.236803 BioClients-0.2.8/PKG-INFO
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     4010 2022-10-11 18:55:24.000000 BioClients-0.2.8/README.md
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:33.192803 BioClients-0.2.8/doc/
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      241 2020-09-09 21:12:43.000000 BioClients-0.2.8/doc/allen.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      278 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/amp_t2d.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      151 2020-09-09 22:16:13.000000 BioClients-0.2.8/doc/bindingdb.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      115 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/biogrid.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      112 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/brenda.md
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      161 2021-11-09 21:23:52.000000 BioClients-0.2.8/doc/cas.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      134 2020-09-09 20:35:32.000000 BioClients-0.2.8/doc/cdc.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     1282 2021-12-14 21:56:45.000000 BioClients-0.2.8/doc/cfde.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      308 2021-05-05 20:41:45.000000 BioClients-0.2.8/doc/chebi.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      501 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/chem2bio2rdf.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      263 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/chembl.md
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      225 2021-11-11 16:45:47.000000 BioClients-0.2.8/doc/chemidplus.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      108 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/disgenet.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      251 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/dnorm.md
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     4517 2021-10-05 17:47:34.000000 BioClients-0.2.8/doc/drugcentral.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     4528 2022-05-03 17:14:30.000000 BioClients-0.2.8/doc/emblebi.md
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      257 2021-01-20 13:59:24.000000 BioClients-0.2.8/doc/ensembl.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      268 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/fda.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       80 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/geneontology.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      185 2021-05-17 20:42:42.000000 BioClients-0.2.8/doc/glygen.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      694 2021-04-14 20:19:24.000000 BioClients-0.2.8/doc/gwascatalog.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       65 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/hugo.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      409 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/humanbase.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      144 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/icite.md
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     6360 2021-09-23 21:27:21.000000 BioClients-0.2.8/doc/idg.md
-drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2022-10-11 20:52:33.216803 BioClients-0.2.8/doc/images/
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)   195140 2020-05-05 15:28:07.000000 BioClients-0.2.8/doc/images/BioClients_logo.png
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      120 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/iuphar.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      325 2020-09-02 21:41:49.000000 BioClients-0.2.8/doc/jensenlab.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      168 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/lincs.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      335 2021-06-28 22:04:55.000000 BioClients-0.2.8/doc/maayanlab.md
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     1971 2021-04-15 20:46:13.000000 BioClients-0.2.8/doc/medline.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      792 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/mesh.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      108 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/monarch.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      172 2020-09-09 19:52:12.000000 BioClients-0.2.8/doc/mygene.md
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      234 2021-02-19 15:28:19.000000 BioClients-0.2.8/doc/ncbo.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      475 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/omim.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      624 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/opentargets.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)       36 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/panther.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      100 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/pdb.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     4711 2022-01-25 21:29:27.000000 BioClients-0.2.8/doc/pubchem.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      253 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/pubmed.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      973 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/pubtator.md
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     1052 2020-11-20 21:40:05.000000 BioClients-0.2.8/doc/reactome.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     2324 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/rxnorm.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     1633 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/stringdb.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      155 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/tcga.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     7238 2021-04-16 20:53:17.000000 BioClients-0.2.8/doc/umls.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      270 2020-06-19 18:04:44.000000 BioClients-0.2.8/doc/uniprot.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     9700 2022-07-28 21:43:57.000000 BioClients-0.2.8/doc/util.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)     1385 2022-08-17 21:09:58.000000 BioClients-0.2.8/doc/wikidata.md
--rw-r--r--   0 jjyang    (1000) jjyang    (1000)      177 2020-09-09 19:52:19.000000 BioClients-0.2.8/doc/wikipathways.md
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       38 2022-10-11 20:52:33.240803 BioClients-0.2.8/setup.cfg
--rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      679 2022-10-11 18:53:47.000000 BioClients-0.2.8/setup.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.639521 BioClients-0.2.9/
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     2023 2020-10-07 15:35:06.000000 BioClients-0.2.9/.gitignore
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.419508 BioClients-0.2.9/BioClients/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)       87 2021-01-20 16:36:37.000000 BioClients-0.2.9/BioClients/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.419508 BioClients-0.2.9/BioClients/allen/
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       76 2020-09-09 21:04:10.000000 BioClients-0.2.9/BioClients/allen/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.423508 BioClients-0.2.9/BioClients/allen/brain/
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     2710 2020-10-08 17:55:26.000000 BioClients-0.2.9/BioClients/allen/brain/Client.py
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     2790 2020-10-08 17:38:21.000000 BioClients-0.2.9/BioClients/allen/brain/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-09 20:43:23.000000 BioClients-0.2.9/BioClients/allen/brain/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.423508 BioClients-0.2.9/BioClients/amp/
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       93 2020-04-27 16:56:30.000000 BioClients-0.2.9/BioClients/amp/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.423508 BioClients-0.2.9/BioClients/amp/t2d/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2324 2020-04-27 16:56:30.000000 BioClients-0.2.9/BioClients/amp/t2d/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2264 2020-10-08 18:23:14.000000 BioClients-0.2.9/BioClients/amp/t2d/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-27 16:56:30.000000 BioClients-0.2.9/BioClients/amp/t2d/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.451508 BioClients-0.2.9/BioClients/bindingdb/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2341 2021-10-28 14:46:32.000000 BioClients-0.2.9/BioClients/bindingdb/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1691 2021-10-28 14:46:32.000000 BioClients-0.2.9/BioClients/bindingdb/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-09 21:25:39.000000 BioClients-0.2.9/BioClients/bindingdb/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.475508 BioClients-0.2.9/BioClients/biogrid/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3666 2022-07-22 14:18:43.000000 BioClients-0.2.9/BioClients/biogrid/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4122 2022-07-22 14:18:43.000000 BioClients-0.2.9/BioClients/biogrid/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-07-22 14:18:43.000000 BioClients-0.2.9/BioClients/biogrid/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.479508 BioClients-0.2.9/BioClients/bioregistry/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2520 2022-09-07 18:57:14.000000 BioClients-0.2.9/BioClients/bioregistry/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     2032 2022-09-07 20:10:50.000000 BioClients-0.2.9/BioClients/bioregistry/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-07-22 14:20:03.000000 BioClients-0.2.9/BioClients/bioregistry/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.479508 BioClients-0.2.9/BioClients/brenda/
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     8008 2021-10-28 14:46:32.000000 BioClients-0.2.9/BioClients/brenda/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)    16819 2021-10-28 14:46:32.000000 BioClients-0.2.9/BioClients/brenda/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-23 14:20:47.000000 BioClients-0.2.9/BioClients/brenda/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.479508 BioClients-0.2.9/BioClients/cas/
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     1740 2021-11-09 21:23:52.000000 BioClients-0.2.9/BioClients/cas/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     1961 2021-11-10 16:10:30.000000 BioClients-0.2.9/BioClients/cas/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       64 2021-11-09 21:23:52.000000 BioClients-0.2.9/BioClients/cas/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.483508 BioClients-0.2.9/BioClients/cdc/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1816 2021-10-28 14:46:32.000000 BioClients-0.2.9/BioClients/cdc/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1327 2021-10-28 14:46:32.000000 BioClients-0.2.9/BioClients/cdc/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-09 20:19:09.000000 BioClients-0.2.9/BioClients/cdc/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.483508 BioClients-0.2.9/BioClients/cfde/
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)        0 2021-12-14 21:44:13.000000 BioClients-0.2.9/BioClients/cfde/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.483508 BioClients-0.2.9/BioClients/cfde/cfchemdb/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3455 2022-04-15 19:23:31.000000 BioClients-0.2.9/BioClients/cfde/cfchemdb/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5544 2022-04-15 20:11:47.000000 BioClients-0.2.9/BioClients/cfde/cfchemdb/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-12-14 21:52:03.000000 BioClients-0.2.9/BioClients/cfde/cfchemdb/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.487508 BioClients-0.2.9/BioClients/chebi/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2268 2022-05-03 15:06:39.000000 BioClients-0.2.9/BioClients/chebi/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3816 2022-05-03 15:14:25.000000 BioClients-0.2.9/BioClients/chebi/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-05-05 17:17:23.000000 BioClients-0.2.9/BioClients/chebi/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.487508 BioClients-0.2.9/BioClients/chem2bio2rdf/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3261 2021-10-28 14:46:32.000000 BioClients-0.2.9/BioClients/chem2bio2rdf/Client.py
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     9907 2020-05-28 17:35:10.000000 BioClients-0.2.9/BioClients/chem2bio2rdf/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      117 2020-04-27 16:56:30.000000 BioClients-0.2.9/BioClients/chem2bio2rdf/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.487508 BioClients-0.2.9/BioClients/chem2bio2rdf/slap/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3193 2020-04-27 16:56:30.000000 BioClients-0.2.9/BioClients/chem2bio2rdf/slap/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    30595 2020-10-08 17:55:51.000000 BioClients-0.2.9/BioClients/chem2bio2rdf/slap/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       59 2020-04-27 16:56:30.000000 BioClients-0.2.9/BioClients/chem2bio2rdf/slap/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.515509 BioClients-0.2.9/BioClients/chembl/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     7783 2021-10-28 14:46:32.000000 BioClients-0.2.9/BioClients/chembl/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6810 2020-04-07 20:01:15.000000 BioClients-0.2.9/BioClients/chembl/FetchByID.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6549 2020-10-08 18:24:20.000000 BioClients-0.2.9/BioClients/chembl/UnichemClient.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    37371 2022-06-24 22:04:07.000000 BioClients-0.2.9/BioClients/chembl/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/chembl/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.515509 BioClients-0.2.9/BioClients/chemidplus/
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     2487 2021-11-11 17:28:45.000000 BioClients-0.2.9/BioClients/chemidplus/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     3501 2021-11-11 18:29:45.000000 BioClients-0.2.9/BioClients/chemidplus/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       75 2021-11-11 16:24:44.000000 BioClients-0.2.9/BioClients/chemidplus/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.519509 BioClients-0.2.9/BioClients/clinicaltrials/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2411 2022-06-22 15:01:24.000000 BioClients-0.2.9/BioClients/clinicaltrials/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     3812 2022-06-22 15:27:51.000000 BioClients-0.2.9/BioClients/clinicaltrials/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-06-21 21:36:12.000000 BioClients-0.2.9/BioClients/clinicaltrials/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.519509 BioClients-0.2.9/BioClients/diseaseontology/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3939 2021-10-28 14:46:32.000000 BioClients-0.2.9/BioClients/diseaseontology/Client.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.519509 BioClients-0.2.9/BioClients/disgenet/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4030 2021-11-16 21:08:22.000000 BioClients-0.2.9/BioClients/disgenet/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     8399 2021-11-16 21:31:10.000000 BioClients-0.2.9/BioClients/disgenet/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2021-11-16 18:09:48.000000 BioClients-0.2.9/BioClients/disgenet/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.519509 BioClients-0.2.9/BioClients/dnorm/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4301 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/dnorm/Client.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)        0 2020-03-06 21:42:19.000000 BioClients-0.2.9/BioClients/dnorm/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.523509 BioClients-0.2.9/BioClients/drugcentral/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6593 2022-02-18 19:29:10.000000 BioClients-0.2.9/BioClients/drugcentral/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     2136 2020-05-26 20:31:43.000000 BioClients-0.2.9/BioClients/drugcentral/Test.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    24247 2022-04-15 16:03:12.000000 BioClients-0.2.9/BioClients/drugcentral/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-20 17:16:25.000000 BioClients-0.2.9/BioClients/drugcentral/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.523509 BioClients-0.2.9/BioClients/emblebi/
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       27 2022-01-06 19:42:43.000000 BioClients-0.2.9/BioClients/emblebi/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.523509 BioClients-0.2.9/BioClients/emblebi/identifiers/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2973 2022-01-06 21:15:41.000000 BioClients-0.2.9/BioClients/emblebi/identifiers/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     4507 2022-01-06 21:11:52.000000 BioClients-0.2.9/BioClients/emblebi/identifiers/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-01-06 19:43:09.000000 BioClients-0.2.9/BioClients/emblebi/identifiers/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.523509 BioClients-0.2.9/BioClients/emblebi/unichem/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2622 2022-06-16 14:56:32.000000 BioClients-0.2.9/BioClients/emblebi/unichem/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     5484 2022-06-16 16:34:32.000000 BioClients-0.2.9/BioClients/emblebi/unichem/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-05-03 15:46:13.000000 BioClients-0.2.9/BioClients/emblebi/unichem/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.559509 BioClients-0.2.9/BioClients/ensembl/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2248 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/ensembl/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4160 2021-04-05 22:17:12.000000 BioClients-0.2.9/BioClients/ensembl/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       46 2021-01-20 16:40:52.000000 BioClients-0.2.9/BioClients/ensembl/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.627510 BioClients-0.2.9/BioClients/ensembl/biomart/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2701 2021-01-20 16:51:43.000000 BioClients-0.2.9/BioClients/ensembl/biomart/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2882 2021-01-20 16:51:00.000000 BioClients-0.2.9/BioClients/ensembl/biomart/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-01-20 13:59:24.000000 BioClients-0.2.9/BioClients/ensembl/biomart/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.683510 BioClients-0.2.9/BioClients/fda/
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       19 2020-03-06 21:42:19.000000 BioClients-0.2.9/BioClients/fda/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.835512 BioClients-0.2.9/BioClients/fda/aer/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3312 2021-08-03 22:03:40.000000 BioClients-0.2.9/BioClients/fda/aer/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     9980 2021-08-06 00:00:44.000000 BioClients-0.2.9/BioClients/fda/aer/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-06 21:42:19.000000 BioClients-0.2.9/BioClients/fda/aer/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.843512 BioClients-0.2.9/BioClients/geneontology/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1813 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/geneontology/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1677 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/geneontology/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/geneontology/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.843512 BioClients-0.2.9/BioClients/glygen/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2171 2021-12-02 17:30:18.000000 BioClients-0.2.9/BioClients/glygen/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3592 2021-12-02 19:03:33.000000 BioClients-0.2.9/BioClients/glygen/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-05-05 21:25:28.000000 BioClients-0.2.9/BioClients/glygen/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.847512 BioClients-0.2.9/BioClients/gwascatalog/
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     2773 2021-12-14 16:30:12.000000 BioClients-0.2.9/BioClients/gwascatalog/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)    10580 2022-01-31 16:12:16.000000 BioClients-0.2.9/BioClients/gwascatalog/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-11 23:32:44.000000 BioClients-0.2.9/BioClients/gwascatalog/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.847512 BioClients-0.2.9/BioClients/hugo/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2944 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/hugo/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4203 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/hugo/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-06 21:42:19.000000 BioClients-0.2.9/BioClients/hugo/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.847512 BioClients-0.2.9/BioClients/humanbase/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     7183 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/humanbase/Client.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)        0 2020-03-06 21:42:19.000000 BioClients-0.2.9/BioClients/humanbase/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.851512 BioClients-0.2.9/BioClients/icite/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1922 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/icite/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2394 2022-11-17 22:09:53.000000 BioClients-0.2.9/BioClients/icite/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-07 20:01:15.000000 BioClients-0.2.9/BioClients/icite/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.863512 BioClients-0.2.9/BioClients/idg/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2546 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/idg/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2902 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/idg/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       82 2020-11-20 21:40:05.000000 BioClients-0.2.9/BioClients/idg/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.875512 BioClients-0.2.9/BioClients/idg/pharos/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3304 2023-02-16 23:10:21.000000 BioClients-0.2.9/BioClients/idg/pharos/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3394 2023-02-16 22:44:09.000000 BioClients-0.2.9/BioClients/idg/pharos/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-09-09 15:44:02.000000 BioClients-0.2.9/BioClients/idg/pharos/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.875512 BioClients-0.2.9/BioClients/idg/rss/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1866 2020-11-20 21:40:05.000000 BioClients-0.2.9/BioClients/idg/rss/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1723 2020-11-20 21:40:05.000000 BioClients-0.2.9/BioClients/idg/rss/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-11-20 21:40:05.000000 BioClients-0.2.9/BioClients/idg/rss/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.887513 BioClients-0.2.9/BioClients/idg/tcrd/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6441 2022-12-13 15:41:10.000000 BioClients-0.2.9/BioClients/idg/tcrd/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)    19636 2022-11-21 14:55:37.000000 BioClients-0.2.9/BioClients/idg/tcrd/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-10-20 20:58:20.000000 BioClients-0.2.9/BioClients/idg/tcrd/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.899513 BioClients-0.2.9/BioClients/idg/tiga/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4278 2022-02-18 19:39:14.000000 BioClients-0.2.9/BioClients/idg/tiga/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4305 2021-09-23 21:24:28.000000 BioClients-0.2.9/BioClients/idg/tiga/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2021-09-22 22:00:16.000000 BioClients-0.2.9/BioClients/idg/tiga/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.919513 BioClients-0.2.9/BioClients/idg/tinx/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4093 2020-11-20 21:40:05.000000 BioClients-0.2.9/BioClients/idg/tinx/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    14947 2020-11-20 21:40:05.000000 BioClients-0.2.9/BioClients/idg/tinx/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-20 17:09:28.000000 BioClients-0.2.9/BioClients/idg/tinx/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.919513 BioClients-0.2.9/BioClients/iuphar/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5895 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/iuphar/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    12307 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/iuphar/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/iuphar/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.923513 BioClients-0.2.9/BioClients/jensenlab/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2070 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/jensenlab/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2235 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/jensenlab/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-27 16:56:30.000000 BioClients-0.2.9/BioClients/jensenlab/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.923513 BioClients-0.2.9/BioClients/lincs/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2944 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/lincs/Client.py
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     5929 2020-10-08 17:53:36.000000 BioClients-0.2.9/BioClients/lincs/Client_lincscloud.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6684 2022-04-13 19:33:09.000000 BioClients-0.2.9/BioClients/lincs/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-05-05 15:28:07.000000 BioClients-0.2.9/BioClients/lincs/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.923513 BioClients-0.2.9/BioClients/lincs/clue/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4942 2020-11-25 17:56:33.000000 BioClients-0.2.9/BioClients/lincs/clue/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    11205 2020-11-25 17:56:33.000000 BioClients-0.2.9/BioClients/lincs/clue/Utils.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.923513 BioClients-0.2.9/BioClients/lincs/sigcom/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1924 2022-04-13 19:59:02.000000 BioClients-0.2.9/BioClients/lincs/sigcom/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1175 2022-04-13 19:50:07.000000 BioClients-0.2.9/BioClients/lincs/sigcom/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-04-13 19:36:10.000000 BioClients-0.2.9/BioClients/lincs/sigcom/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.923513 BioClients-0.2.9/BioClients/maayanlab/
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)        0 2021-06-29 14:35:40.000000 BioClients-0.2.9/BioClients/maayanlab/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.923513 BioClients-0.2.9/BioClients/maayanlab/archs4/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1267 2021-06-28 21:58:02.000000 BioClients-0.2.9/BioClients/maayanlab/archs4/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1252 2021-06-28 21:55:32.000000 BioClients-0.2.9/BioClients/maayanlab/archs4/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-06-28 21:53:00.000000 BioClients-0.2.9/BioClients/maayanlab/archs4/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.927513 BioClients-0.2.9/BioClients/maayanlab/harmonizome/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1825 2021-06-28 21:52:47.000000 BioClients-0.2.9/BioClients/maayanlab/harmonizome/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2133 2021-06-28 21:52:02.000000 BioClients-0.2.9/BioClients/maayanlab/harmonizome/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-27 16:56:30.000000 BioClients-0.2.9/BioClients/maayanlab/harmonizome/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.927513 BioClients-0.2.9/BioClients/medline/
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)        0 2021-04-15 20:38:22.000000 BioClients-0.2.9/BioClients/medline/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.927513 BioClients-0.2.9/BioClients/medline/connect/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3107 2021-04-15 20:39:31.000000 BioClients-0.2.9/BioClients/medline/connect/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2228 2021-04-15 20:37:11.000000 BioClients-0.2.9/BioClients/medline/connect/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2021-04-15 20:32:33.000000 BioClients-0.2.9/BioClients/medline/connect/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.947513 BioClients-0.2.9/BioClients/medline/genetics/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3014 2021-04-15 20:43:50.000000 BioClients-0.2.9/BioClients/medline/genetics/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5131 2021-04-15 20:28:15.000000 BioClients-0.2.9/BioClients/medline/genetics/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-04-15 19:00:20.000000 BioClients-0.2.9/BioClients/medline/genetics/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.947513 BioClients-0.2.9/BioClients/mesh/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2606 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/mesh/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3904 2021-05-18 17:02:28.000000 BioClients-0.2.9/BioClients/mesh/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/mesh/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.979514 BioClients-0.2.9/BioClients/monarch/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3604 2020-10-08 17:52:16.000000 BioClients-0.2.9/BioClients/monarch/Biolink.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4603 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/monarch/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     8134 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/monarch/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-22 19:18:52.000000 BioClients-0.2.9/BioClients/monarch/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.979514 BioClients-0.2.9/BioClients/mygene/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1962 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/mygene/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1353 2021-11-16 15:41:45.000000 BioClients-0.2.9/BioClients/mygene/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-09 19:40:04.000000 BioClients-0.2.9/BioClients/mygene/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.979514 BioClients-0.2.9/BioClients/ncats/
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       20 2022-12-02 17:54:08.000000 BioClients-0.2.9/BioClients/ncats/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.995514 BioClients-0.2.9/BioClients/ncats/gsrs/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2369 2022-12-02 20:21:02.000000 BioClients-0.2.9/BioClients/ncats/gsrs/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     6247 2022-12-05 18:58:55.000000 BioClients-0.2.9/BioClients/ncats/gsrs/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-12-02 17:54:41.000000 BioClients-0.2.9/BioClients/ncats/gsrs/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.995514 BioClients-0.2.9/BioClients/ncbo/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2369 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/ncbo/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2317 2021-02-19 15:28:19.000000 BioClients-0.2.9/BioClients/ncbo/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-02-19 15:28:19.000000 BioClients-0.2.9/BioClients/ncbo/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.995514 BioClients-0.2.9/BioClients/omim/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4527 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/omim/Client.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)        0 2020-03-06 21:42:19.000000 BioClients-0.2.9/BioClients/omim/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.995514 BioClients-0.2.9/BioClients/openphacts/
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     3679 2022-06-23 16:48:03.000000 BioClients-0.2.9/BioClients/openphacts/Client.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     8922 2022-06-23 16:50:29.000000 BioClients-0.2.9/BioClients/openphacts/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2022-06-23 15:47:27.000000 BioClients-0.2.9/BioClients/openphacts/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.999514 BioClients-0.2.9/BioClients/opentargets/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3067 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/opentargets/Client.py
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     4254 2020-06-19 18:04:44.000000 BioClients-0.2.9/BioClients/opentargets/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-06-19 18:04:44.000000 BioClients-0.2.9/BioClients/opentargets/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.011514 BioClients-0.2.9/BioClients/panther/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4018 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/panther/Client.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)        0 2020-04-16 18:00:39.000000 BioClients-0.2.9/BioClients/panther/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.011514 BioClients-0.2.9/BioClients/pdb/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2187 2023-02-13 21:29:39.000000 BioClients-0.2.9/BioClients/pdb/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3862 2023-02-13 21:20:41.000000 BioClients-0.2.9/BioClients/pdb/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-06 21:42:19.000000 BioClients-0.2.9/BioClients/pdb/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.047514 BioClients-0.2.9/BioClients/pubchem/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5517 2023-02-14 20:26:51.000000 BioClients-0.2.9/BioClients/pubchem/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    37059 2023-02-14 20:39:43.000000 BioClients-0.2.9/BioClients/pubchem/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      103 2020-04-13 20:27:56.000000 BioClients-0.2.9/BioClients/pubchem/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.075515 BioClients-0.2.9/BioClients/pubchem/ftp/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1995 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/pubchem/ftp/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6666 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/pubchem/ftp/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/pubchem/ftp/__init__.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    15202 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_actives.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5629 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_assay_fetch.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4221 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_assay_results.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     7900 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_assay_search.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6583 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_assaysim.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     9488 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_compound_assaystats.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     9080 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_gini_index.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.075515 BioClients-0.2.9/BioClients/pubchem/rdf/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     9185 2020-10-08 17:57:09.000000 BioClients-0.2.9/BioClients/pubchem/rdf/Client.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)        0 2020-04-07 20:01:15.000000 BioClients-0.2.9/BioClients/pubchem/rdf/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.079515 BioClients-0.2.9/BioClients/pubchem/soap/
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     6328 2022-01-25 21:22:25.000000 BioClients-0.2.9/BioClients/pubchem/soap/Client.py
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)    15140 2022-01-25 20:45:35.000000 BioClients-0.2.9/BioClients/pubchem/soap/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2022-01-25 16:45:41.000000 BioClients-0.2.9/BioClients/pubchem/soap/__init__.py
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     6747 2020-06-03 16:30:16.000000 BioClients-0.2.9/BioClients/pubchem/soap/pug_aids2assays.py
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     6638 2020-06-03 16:30:16.000000 BioClients-0.2.9/BioClients/pubchem/soap/pug_ids2mols.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     9796 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/pubchem/soap/pug_substance_search.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.079515 BioClients-0.2.9/BioClients/pubmed/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     8705 2020-10-01 21:22:56.000000 BioClients-0.2.9/BioClients/pubmed/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)        0 2020-04-07 20:01:15.000000 BioClients-0.2.9/BioClients/pubmed/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.083515 BioClients-0.2.9/BioClients/pubtator/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2645 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/pubtator/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1669 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/pubtator/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-07 20:01:15.000000 BioClients-0.2.9/BioClients/pubtator/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.083515 BioClients-0.2.9/BioClients/reactome/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3226 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/reactome/Client.py
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     1108 2020-03-09 15:16:21.000000 BioClients-0.2.9/BioClients/reactome/SMBL_utils.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     7251 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/reactome/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       48 2020-03-09 15:38:06.000000 BioClients-0.2.9/BioClients/reactome/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.087515 BioClients-0.2.9/BioClients/rxnorm/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5836 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/rxnorm/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    11857 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/rxnorm/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-07 20:01:15.000000 BioClients-0.2.9/BioClients/rxnorm/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.087515 BioClients-0.2.9/BioClients/stringdb/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3747 2022-08-26 22:06:36.000000 BioClients-0.2.9/BioClients/stringdb/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     5086 2022-08-26 22:06:42.000000 BioClients-0.2.9/BioClients/stringdb/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-11-20 21:40:05.000000 BioClients-0.2.9/BioClients/stringdb/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.087515 BioClients-0.2.9/BioClients/tcga/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2110 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/tcga/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4889 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/tcga/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-04-28 16:33:19.000000 BioClients-0.2.9/BioClients/tcga/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.091515 BioClients-0.2.9/BioClients/umls/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     6854 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/umls/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    19343 2021-04-16 21:05:21.000000 BioClients-0.2.9/BioClients/umls/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-27 17:01:05.000000 BioClients-0.2.9/BioClients/umls/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.091515 BioClients-0.2.9/BioClients/uniprot/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1938 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/uniprot/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1661 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/uniprot/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-03-06 21:42:19.000000 BioClients-0.2.9/BioClients/uniprot/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.091515 BioClients-0.2.9/BioClients/util/
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      112 2020-10-21 17:44:43.000000 BioClients-0.2.9/BioClients/util/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.091515 BioClients-0.2.9/BioClients/util/db/
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     1691 2022-11-29 20:14:04.000000 BioClients-0.2.9/BioClients/util/db/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2022-02-18 17:39:54.000000 BioClients-0.2.9/BioClients/util/db/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.095515 BioClients-0.2.9/BioClients/util/graphql/
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)      839 2023-02-16 23:02:31.000000 BioClients-0.2.9/BioClients/util/graphql/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-12-16 21:47:54.000000 BioClients-0.2.9/BioClients/util/graphql/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.095515 BioClients-0.2.9/BioClients/util/hdf/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1760 2021-06-28 21:43:01.000000 BioClients-0.2.9/BioClients/util/hdf/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-06-28 21:59:50.000000 BioClients-0.2.9/BioClients/util/hdf/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.095515 BioClients-0.2.9/BioClients/util/igraph/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     8378 2022-02-08 22:02:33.000000 BioClients-0.2.9/BioClients/util/igraph/App.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)    17764 2022-02-08 22:04:07.000000 BioClients-0.2.9/BioClients/util/igraph/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-12-06 15:00:46.000000 BioClients-0.2.9/BioClients/util/igraph/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.099515 BioClients-0.2.9/BioClients/util/neo4j/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2509 2022-07-27 16:21:13.000000 BioClients-0.2.9/BioClients/util/neo4j/App.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1717 2022-07-27 16:21:13.000000 BioClients-0.2.9/BioClients/util/neo4j/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2022-07-26 15:37:07.000000 BioClients-0.2.9/BioClients/util/neo4j/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.099515 BioClients-0.2.9/BioClients/util/obo/
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)      808 2022-01-26 17:32:05.000000 BioClients-0.2.9/BioClients/util/obo/App.py
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     1920 2022-01-26 17:30:31.000000 BioClients-0.2.9/BioClients/util/obo/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2022-01-26 17:28:15.000000 BioClients-0.2.9/BioClients/util/obo/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.127515 BioClients-0.2.9/BioClients/util/pandas/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     8710 2023-01-19 20:21:08.000000 BioClients-0.2.9/BioClients/util/pandas/App.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3482 2021-09-03 22:00:41.000000 BioClients-0.2.9/BioClients/util/pandas/Csv2Html.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2535 2021-09-09 14:38:00.000000 BioClients-0.2.9/BioClients/util/pandas/Csv2Markdown.py
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)    14611 2022-12-19 21:20:37.000000 BioClients-0.2.9/BioClients/util/pandas/Csv2Sql.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     3490 2023-01-19 20:35:04.000000 BioClients-0.2.9/BioClients/util/pandas/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-06-28 22:00:16.000000 BioClients-0.2.9/BioClients/util/pandas/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.127515 BioClients-0.2.9/BioClients/util/rdf/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1644 2022-04-01 19:25:45.000000 BioClients-0.2.9/BioClients/util/rdf/App.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2099 2022-04-01 19:24:45.000000 BioClients-0.2.9/BioClients/util/rdf/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2022-03-23 13:55:45.000000 BioClients-0.2.9/BioClients/util/rdf/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.127515 BioClients-0.2.9/BioClients/util/rest/
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     4373 2020-10-08 16:50:07.000000 BioClients-0.2.9/BioClients/util/rest/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-10-08 17:36:38.000000 BioClients-0.2.9/BioClients/util/rest/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.131515 BioClients-0.2.9/BioClients/util/sparql/
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     3217 2022-07-28 21:41:58.000000 BioClients-0.2.9/BioClients/util/sparql/Client.py
+-rwxr-xr-x   0 jjyang    (1000) jjyang    (1000)     5322 2022-07-28 21:15:41.000000 BioClients-0.2.9/BioClients/util/sparql/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-11 13:53:06.000000 BioClients-0.2.9/BioClients/util/sparql/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.131515 BioClients-0.2.9/BioClients/util/xml/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     4414 2020-10-06 19:53:19.000000 BioClients-0.2.9/BioClients/util/xml/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2021-06-28 21:59:54.000000 BioClients-0.2.9/BioClients/util/xml/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.131515 BioClients-0.2.9/BioClients/util/yaml/
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      411 2020-10-21 17:44:43.000000 BioClients-0.2.9/BioClients/util/yaml/Utils.py
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       21 2020-10-21 17:44:43.000000 BioClients-0.2.9/BioClients/util/yaml/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.131515 BioClients-0.2.9/BioClients/wikidata/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1844 2022-08-17 21:12:23.000000 BioClients-0.2.9/BioClients/wikidata/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2390 2022-08-17 20:59:30.000000 BioClients-0.2.9/BioClients/wikidata/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-11 15:42:13.000000 BioClients-0.2.9/BioClients/wikidata/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.135515 BioClients-0.2.9/BioClients/wikipathways/
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     2733 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/wikipathways/Client.py
+-rwxrwxr-x   0 jjyang    (1000) jjyang    (1000)     1900 2021-10-28 14:46:33.000000 BioClients-0.2.9/BioClients/wikipathways/Utils.py
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       21 2020-09-09 19:05:50.000000 BioClients-0.2.9/BioClients/wikipathways/__init__.py
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:43.419508 BioClients-0.2.9/BioClients.egg-info/
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     4486 2023-02-17 16:29:40.000000 BioClients-0.2.9/BioClients.egg-info/PKG-INFO
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     9197 2023-02-17 16:29:43.000000 BioClients-0.2.9/BioClients.egg-info/SOURCES.txt
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)        1 2023-02-17 16:29:40.000000 BioClients-0.2.9/BioClients.egg-info/dependency_links.txt
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       11 2023-02-17 16:29:40.000000 BioClients-0.2.9/BioClients.egg-info/top_level.txt
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     7048 2020-04-09 14:30:34.000000 BioClients-0.2.9/LICENSE
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     4486 2023-02-17 16:29:44.635521 BioClients-0.2.9/PKG-INFO
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     4023 2022-12-02 20:26:29.000000 BioClients-0.2.9/README.md
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.599520 BioClients-0.2.9/doc/
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      241 2020-09-09 21:12:43.000000 BioClients-0.2.9/doc/allen.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      278 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/amp_t2d.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      151 2020-09-09 22:16:13.000000 BioClients-0.2.9/doc/bindingdb.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      115 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/biogrid.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     1100 2022-09-07 20:11:32.000000 BioClients-0.2.9/doc/bioregistry.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      112 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/brenda.md
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      161 2021-11-09 21:23:52.000000 BioClients-0.2.9/doc/cas.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      134 2020-09-09 20:35:32.000000 BioClients-0.2.9/doc/cdc.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     1282 2021-12-14 21:56:45.000000 BioClients-0.2.9/doc/cfde.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      308 2021-05-05 20:41:45.000000 BioClients-0.2.9/doc/chebi.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      501 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/chem2bio2rdf.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      263 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/chembl.md
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      225 2021-11-11 16:45:47.000000 BioClients-0.2.9/doc/chemidplus.md
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      224 2022-06-22 15:32:34.000000 BioClients-0.2.9/doc/clinicaltrials.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      108 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/disgenet.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      251 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/dnorm.md
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     4602 2022-12-05 21:37:02.000000 BioClients-0.2.9/doc/drugcentral.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     4528 2022-05-03 17:14:30.000000 BioClients-0.2.9/doc/emblebi.md
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      257 2021-01-20 13:59:24.000000 BioClients-0.2.9/doc/ensembl.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      268 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/fda.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       80 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/geneontology.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      185 2021-05-17 20:42:42.000000 BioClients-0.2.9/doc/glygen.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      694 2021-04-14 20:19:24.000000 BioClients-0.2.9/doc/gwascatalog.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       65 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/hugo.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      409 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/humanbase.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      144 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/icite.md
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     6565 2023-02-16 23:12:09.000000 BioClients-0.2.9/doc/idg.md
+drwxrwxr-x   0 jjyang    (1000) jjyang    (1000)        0 2023-02-17 16:29:44.619520 BioClients-0.2.9/doc/images/
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)   195140 2020-05-05 15:28:07.000000 BioClients-0.2.9/doc/images/BioClients_logo.png
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      120 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/iuphar.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      325 2020-09-02 21:41:49.000000 BioClients-0.2.9/doc/jensenlab.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      168 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/lincs.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      335 2021-06-28 22:04:55.000000 BioClients-0.2.9/doc/maayanlab.md
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     1971 2021-04-15 20:46:13.000000 BioClients-0.2.9/doc/medline.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      792 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/mesh.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      108 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/monarch.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      172 2020-09-09 19:52:12.000000 BioClients-0.2.9/doc/mygene.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     1199 2022-12-02 20:25:08.000000 BioClients-0.2.9/doc/ncats.md
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      234 2021-02-19 15:28:19.000000 BioClients-0.2.9/doc/ncbo.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      475 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/omim.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      624 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/opentargets.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)       36 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/panther.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      100 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/pdb.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     4711 2022-01-25 21:29:27.000000 BioClients-0.2.9/doc/pubchem.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      253 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/pubmed.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      973 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/pubtator.md
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)     1052 2020-11-20 21:40:05.000000 BioClients-0.2.9/doc/reactome.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     2324 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/rxnorm.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     1633 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/stringdb.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      155 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/tcga.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     7238 2021-04-16 20:53:17.000000 BioClients-0.2.9/doc/umls.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      270 2020-06-19 18:04:44.000000 BioClients-0.2.9/doc/uniprot.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     9700 2022-07-28 21:43:57.000000 BioClients-0.2.9/doc/util.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)     1385 2022-08-17 21:09:58.000000 BioClients-0.2.9/doc/wikidata.md
+-rw-r--r--   0 jjyang    (1000) jjyang    (1000)      177 2020-09-09 19:52:19.000000 BioClients-0.2.9/doc/wikipathways.md
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)       38 2023-02-17 16:29:44.639521 BioClients-0.2.9/setup.cfg
+-rw-rw-r--   0 jjyang    (1000) jjyang    (1000)      679 2022-12-06 21:27:27.000000 BioClients-0.2.9/setup.py
```

### Comparing `BioClients-0.2.8/.gitignore` & `BioClients-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/allen/brain/Client.py` & `BioClients-0.2.9/BioClients/allen/brain/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/allen/brain/Utils.py` & `BioClients-0.2.9/BioClients/allen/brain/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/amp/t2d/Client.py` & `BioClients-0.2.9/BioClients/amp/t2d/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/amp/t2d/Utils.py` & `BioClients-0.2.9/BioClients/amp/t2d/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/bindingdb/Client.py` & `BioClients-0.2.9/BioClients/bindingdb/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/bindingdb/Utils.py` & `BioClients-0.2.9/BioClients/bindingdb/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/biogrid/Client.py` & `BioClients-0.2.9/BioClients/biogrid/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/biogrid/Utils.py` & `BioClients-0.2.9/BioClients/biogrid/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/bioregistry/Client.py` & `BioClients-0.2.9/BioClients/bioregistry/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/bioregistry/Utils.py` & `BioClients-0.2.9/BioClients/bioregistry/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/brenda/Client.py` & `BioClients-0.2.9/BioClients/brenda/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/brenda/Utils.py` & `BioClients-0.2.9/BioClients/brenda/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/cas/Client.py` & `BioClients-0.2.9/BioClients/cas/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/cas/Utils.py` & `BioClients-0.2.9/BioClients/cas/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/cdc/Client.py` & `BioClients-0.2.9/BioClients/cdc/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/cdc/Utils.py` & `BioClients-0.2.9/BioClients/cdc/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/cfde/cfchemdb/Client.py` & `BioClients-0.2.9/BioClients/cfde/cfchemdb/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/cfde/cfchemdb/Utils.py` & `BioClients-0.2.9/BioClients/cfde/cfchemdb/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/chebi/Client.py` & `BioClients-0.2.9/BioClients/chebi/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/chebi/Utils.py` & `BioClients-0.2.9/BioClients/chebi/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/chem2bio2rdf/Client.py` & `BioClients-0.2.9/BioClients/chem2bio2rdf/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/chem2bio2rdf/Utils.py` & `BioClients-0.2.9/BioClients/chem2bio2rdf/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/chem2bio2rdf/slap/Client.py` & `BioClients-0.2.9/BioClients/chem2bio2rdf/slap/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/chem2bio2rdf/slap/Utils.py` & `BioClients-0.2.9/BioClients/chem2bio2rdf/slap/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/chembl/Client.py` & `BioClients-0.2.9/BioClients/chembl/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/chembl/FetchByID.py` & `BioClients-0.2.9/BioClients/chembl/FetchByID.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/chembl/UnichemClient.py` & `BioClients-0.2.9/BioClients/chembl/UnichemClient.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/chembl/Utils.py` & `BioClients-0.2.9/BioClients/chembl/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/chemidplus/Client.py` & `BioClients-0.2.9/BioClients/chemidplus/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/chemidplus/Utils.py` & `BioClients-0.2.9/BioClients/chemidplus/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/clinicaltrials/Client.py` & `BioClients-0.2.9/BioClients/clinicaltrials/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/clinicaltrials/Utils.py` & `BioClients-0.2.9/BioClients/clinicaltrials/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/diseaseontology/Client.py` & `BioClients-0.2.9/BioClients/diseaseontology/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/disgenet/Client.py` & `BioClients-0.2.9/BioClients/disgenet/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/disgenet/Utils.py` & `BioClients-0.2.9/BioClients/disgenet/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/dnorm/Client.py` & `BioClients-0.2.9/BioClients/dnorm/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/drugcentral/Client.py` & `BioClients-0.2.9/BioClients/drugcentral/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/drugcentral/Test.py` & `BioClients-0.2.9/BioClients/drugcentral/Test.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/drugcentral/Utils.py` & `BioClients-0.2.9/BioClients/drugcentral/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/emblebi/identifiers/Client.py` & `BioClients-0.2.9/BioClients/emblebi/identifiers/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/emblebi/identifiers/Utils.py` & `BioClients-0.2.9/BioClients/emblebi/identifiers/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/emblebi/unichem/Client.py` & `BioClients-0.2.9/BioClients/emblebi/unichem/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/emblebi/unichem/Utils.py` & `BioClients-0.2.9/BioClients/emblebi/unichem/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/ensembl/Client.py` & `BioClients-0.2.9/BioClients/ensembl/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/ensembl/Utils.py` & `BioClients-0.2.9/BioClients/ensembl/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/ensembl/biomart/Client.py` & `BioClients-0.2.9/BioClients/ensembl/biomart/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/ensembl/biomart/Utils.py` & `BioClients-0.2.9/BioClients/ensembl/biomart/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/fda/aer/Client.py` & `BioClients-0.2.9/BioClients/fda/aer/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/fda/aer/Utils.py` & `BioClients-0.2.9/BioClients/fda/aer/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/geneontology/Client.py` & `BioClients-0.2.9/BioClients/geneontology/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/geneontology/Utils.py` & `BioClients-0.2.9/BioClients/geneontology/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/glygen/Client.py` & `BioClients-0.2.9/BioClients/glygen/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/glygen/Utils.py` & `BioClients-0.2.9/BioClients/glygen/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/gwascatalog/Client.py` & `BioClients-0.2.9/BioClients/gwascatalog/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/gwascatalog/Utils.py` & `BioClients-0.2.9/BioClients/gwascatalog/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/hugo/Client.py` & `BioClients-0.2.9/BioClients/hugo/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/hugo/Utils.py` & `BioClients-0.2.9/BioClients/hugo/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/humanbase/Client.py` & `BioClients-0.2.9/BioClients/humanbase/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/icite/Client.py` & `BioClients-0.2.9/BioClients/icite/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/icite/Utils.py` & `BioClients-0.2.9/BioClients/icite/Utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python3
 ###
-import sys,os,json,re,logging,tqdm
+import sys,os,json,re,logging,tqdm,requests,urllib.parse
 import pandas as pd
 #
-from ..util import rest
-#
 API_HOST="icite.od.nih.gov"
 API_BASE_PATH="/api/pubs"
 BASE_URL='https://'+API_HOST+API_BASE_PATH
 #
 NCHUNK=100;
 #
 #############################################################################
@@ -19,19 +17,22 @@
   quiet = bool(logging.getLogger().getEffectiveLevel()>15)
   while True:
     if tq is None and not quiet: tq = tqdm.tqdm(total=len(pmids), unit="pmids")
     if n_in>=len(pmids): break
     pmids_this = pmids[n_in:n_in+NCHUNK]
     n_in += (NCHUNK if n_in+NCHUNK < len(pmids) else len(pmids)-n_in)
     url_this = (f"""{base_url}?pmids={(','.join(pmids_this))}""")
-    rval = rest.GetURL(url_this, parse_json=True)
-    if not rval: break
-    logging.debug(json.dumps(rval, indent=2))
-    url_self = rval['links']['self']
-    pubs = rval['data']
+    response = requests.get(url_this)
+    if response.status_code != 200:
+      logging.error(f"status_code: {response.status_code}")
+      break
+    result = response.json()
+    logging.debug(json.dumps(result, indent=2))
+    url_self = result['links']['self']
+    pubs = result['data']
     for pub in pubs:
       if not tags: tags = list(pub.keys())
       df_this = pd.DataFrame({tags[j]:[pub[tags[j]]] for j in range(len(tags))})
       if fout: df_this.to_csv(fout, "\t", index=False, header=bool(n_out==0))
       df = pd.concat([df, df_this])
       n_out+=1
     if not quiet:
@@ -43,18 +44,19 @@
 def GetStats_single(pmids, base_url=BASE_URL, fout=None):
   """Request singly."""
   tags=None; df=pd.DataFrame(); tq=None;
   for pmid in pmids:
     if tq is None: tq = tqdm.tqdm(total=len(pmids), unit="pmids")
     tq.update()
     url = base_url+'/'+pmid
-    pub = rest.GetURL(url, parse_json=True)
-    if not pub:
-      logging.info(f"Not found: {pmid}")
+    response = requests.get(url)
+    if response.status_code != 200:
+      logging.error(f"status_code: {response.status_code}")
       continue
+    pub = response.json()
     if not tags: tags = list(pub.keys())
     df = pd.concat([df, pd.DataFrame({tags[j]:[pub[tags[j]]] for j in range(len(tags))})])
   if fout: df.to_csv(fout, "\t", index=False)
   logging.info(f"n_in: {len(pmids)}; n_out: {df.shape[0]}")
   return df
 
 #############################################################################
```

### Comparing `BioClients-0.2.8/BioClients/idg/Client.py` & `BioClients-0.2.9/BioClients/idg/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/idg/Utils.py` & `BioClients-0.2.9/BioClients/idg/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/idg/pharos/Client.py` & `BioClients-0.2.9/BioClients/idg/rss/Client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,56 @@
 #!/usr/bin/env python3
 """
-Pharos GraphQL API client
-https://pharos.nih.gov/api
+IDG Resource Submission System
+https://rss.ccs.miami.edu/
 """
 ###
-import sys,os,argparse,json,re,time,logging
+import sys,os,re,argparse,time,logging
 #
-from ... import idg
+from ...idg import rss
 #
-#############################################################################
+##############################################################################
 if __name__=='__main__':
-  parser = argparse.ArgumentParser(description='Pharos GraphQL API client')
-  ops = [
-	'get_targets',
-	'get_diseases',
-	'test' ]
-  parser.add_argument("op", choices=ops, help='OPERATION')
-  parser.add_argument("--i", dest="ifile", help="input file, target IDs")
-  parser.add_argument("--ids", dest="ids", help="IDs, target, comma-separated")
+  epilog="""\
+"""
+  parser = argparse.ArgumentParser(description="IDG RSS (Resource Submission System) REST API client)", epilog=epilog)
+  ops = [ "list_targets", "get_target_resources" ]
+  parser.add_argument("op", choices=ops, help="operation")
+  parser.add_argument("--i", dest="ifile", help="input IDs")
+  parser.add_argument("--ids", help="IDs (comma-separated)")
   parser.add_argument("--o", dest="ofile", help="output (TSV)")
-  parser.add_argument("--idtype_target", choices=list(idg.pharos.Utils.IDTYPES_TARGET.keys()), default='sym', help="target ID type")
-  parser.add_argument("--idtype_disease", choices=list(idg.pharos.Utils.IDTYPES_DISEASE.keys()), default='name', help="disease ID type")
-  parser.add_argument("--nmax", type=int, help="max to return")
-  parser.add_argument("--api_endpoint", default=idg.pharos.Utils.API_ENDPOINT)
+  parser.add_argument("--api_host", default=rss.Utils.API_HOST)
+  parser.add_argument("--api_base_path", default=rss.Utils.API_BASE_PATH)
   parser.add_argument("-v", "--verbose", default=0, action="count")
   args = parser.parse_args()
 
   logging.basicConfig(format='%(levelname)s:%(message)s', level=(logging.DEBUG if args.verbose>1 else logging.INFO))
 
-  fout = open(args.ofile, "w+") if args.ofile else sys.stdout
+  fout = open(args.ofile, "w") if args.ofile else sys.stdout
 
-  ids=[];
+  ids=[]
   if args.ifile:
     fin = open(args.ifile)
     while True:
       line = fin.readline()
       if not line: break
       ids.append(line.rstrip())
     fin.close()
   elif args.ids:
-    ids = re.split(r'\s*,\s*', args.ids.strip())
-  logging.info(f"Input IDs: {len(ids)}")
-
-  t0 = time.time()
+    ids = re.split('[,\s]+', args.ids.strip())
+  if ids: logging.info('Input IDs: %d'%(len(ids)))
 
-  if re.match(r'^get_', args.op) and not ids:
-    parser.error(f"{args.op} requires IDs.")
+  t0=time.time()
 
-  if args.op=='get_targets':
-    idg.pharos.Utils.GetTargets(ids, args.idtype_target, args.api_endpoint, fout)
+  base_url = 'https://'+args.api_host+args.api_base_path
 
-  elif args.op=='get_diseases':
-    idg.pharos.Utils.GetDiseases(ids, args.idtype_disease, args.api_endpoint, fout)
+  if args.op=='list_targets':
+    rss.Utils.ListTargets(base_url, fout)
 
-  elif args.op=='test':
-    idg.pharos.Utils.Test(args.api_endpoint, fout)
+  elif args.op=='get_target_resources':
+    if not ids: parser.error(f"--i or --ids required for {args.op}")
+    rss.Utils.GetTargetResources(ids, base_url, fout)
 
   else:
-    logging.error(f"Invalid operation: {args.op}")
+    parser.error(f'Unknown operation: {args.op}')
 
-  logging.info("Elapsed time: "+time.strftime('%Hh:%Mm:%Ss', time.gmtime(time.time()-t0)))
+  logging.info(('elapsed time: %s'%(time.strftime('%Hh:%Mm:%Ss',time.gmtime(time.time()-t0)))))
```

### Comparing `BioClients-0.2.8/BioClients/idg/pharos/ClientGql.py` & `BioClients-0.2.9/BioClients/util/hdf/Utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,55 @@
 #!/usr/bin/env python3
 ###
-import sys,os,json,argparse,logging
 
-from ...util import graphql as util_graphql
+import sys,os,time,argparse,logging
+import numpy as np
+import pandas as pd
+import h5py
 
-#GQL_HOST="ncats-ifx.appspot.com"
-GQL_HOST="pharos-api.ncats.io"
-GQL_BASE_PATH="/graphql"
-GQL_URL="https://"+GQL_HOST+GQL_BASE_PATH
+###
+def h5_type(ob):
+  return "Group" if type(ob) is h5py.Group else "Dataset" if type(ob) is h5py.Dataset else type(ob)
+
+###
+def list_all(name, ob):
+  logging.info(f"{ob.name} ({h5_type(ob)})")
+  if type(ob) is h5py.Dataset:
+    logging.info(f"Dataset dtype: {ob.dtype}; shape: {ob.shape}; size: {ob.size}; ndim: {ob.ndim}; nbytes: {ob.nbytes}")
+  return None
 
 #############################################################################
-def DemoGql():
-  return """\
-{
-  search(term: "gout") {
-    diseaseResult {
-      count
-      facets {
-        facet
-        values {
-          name
-          value
-        }
-      }
-      diseases {
-        name
-        associationCount
-        associations {
-          did
-          name
-          type
-        }
-      }
-    }
-  }
-}
-"""
+def Summary(f):
+  logging.debug(list(f.keys()))
+  for k in list(f.keys()):
+    if type(f[k]) is h5py.Group:
+      logging.debug(f"{f.name}:{f[k].name}")
+      f[k].visititems(list_all)
+    else:
+      logging.info(f"{f[k].name} ({h5_type(f[k])})")
 
 #############################################################################
-if __name__ == "__main__":
-  parser = argparse.ArgumentParser(description='Pharos GraphQL client utility')
-  OPS = ['query', 'demo', 'getSchema']
+if __name__=='__main__':
+  parser = argparse.ArgumentParser(description='H5 file operations', epilog="")
+  OPS = ['summary']
   parser.add_argument("op", choices=OPS, help='OPERATION')
-  parser.add_argument("--i", dest="ifile", help="input file, GraphQL")
-  parser.add_argument("--graphql", help="input GraphQL")
+  parser.add_argument("--i", dest="ifile", required=True, help="input file")
   parser.add_argument("--o", dest="ofile", help="output (TSV)")
-  parser.add_argument("--gql_host", default=GQL_HOST)
-  parser.add_argument("--gql_base_path", default=GQL_BASE_PATH)
-  parser.add_argument("-v", "--verbose", default=0, action="count")
+  parser.add_argument("-v", "--verbose", dest="verbose", action="count", default=0)
   args = parser.parse_args()
 
   logging.basicConfig(format='%(levelname)s:%(message)s', level=(logging.DEBUG if args.verbose>1 else logging.INFO))
 
-  gql_url='https://'+args.gql_host+args.gql_base_path
+  t0 = time.time();
 
-  fout = open(args.ofile) if args.ofile else sys.stdout
+  fout = open(args.ofile, "w") if args.ofile else sys.stdout
 
-  graphql=None;
-  if args.ifile:
-    with open(args.ifile) as fin:
-      graphql = fin.read()
-  elif args.graphql:
-    graphql = args.graphql
-  logging.debug(graphql)
+  finh5 = h5py.File(args.ifile, 'r')
 
-  if args.op == 'query':
-    util_graphql.RunQuery(gql_url, graphql, fout)
-
-  elif args.op == 'demo':
-    util_graphql.RunQuery(gql_url, DemoGql(), fout)
-
-  elif args.op == 'getSchema':
-    parser.error(f"Unimplemented operation: {args.op}")
+  if args.op == "summary":
+    Summary(finh5)
 
   else:
-    parser.error(f"Invalid operation: {args.op}")
+    parser.error(f"Unsupported operation: {args.op}")
+
+  logging.info(f"Elapsed: {time.strftime('%Hh:%Mm:%Ss', time.gmtime(time.time()-t0))}")
```

### Comparing `BioClients-0.2.8/BioClients/idg/pharos/Utils.py` & `BioClients-0.2.9/BioClients/idg/pharos/Utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 ###
 import sys,os,json,re,time,logging
 #
 from python_graphql_client import GraphqlClient
 #
 # curl 'https://pharos-api.ncats.io/graphql' -H 'Accept-Encoding: gzip, deflate, br' -H 'Content-Type: application/json' -H 'Accept: application/json' -H 'Connection: keep-alive' -H 'DNT: 1' -H 'Origin: https://pharos-api.ncats.io' --data-binary '{"query":"query targetDetails {\n  target(q: { sym: \"ACE2\" }) {\n    name\n    tdl\n    fam\n    sym\n    description\n    novelty\n  }\n}\n"}' --compressed
 #
-API_ENDPOINT="https://pharos-api.ncats.io/graphql"
+#API_HOST="ncats-ifx.appspot.com"
+API_HOST="pharos-api.ncats.io"
+API_BASE_PATH="/graphql"
+API_BASE_URL="https://"+API_HOST+API_BASE_PATH
 #
 API_HEADERS = { 'Accept-Encoding': 'gzip, deflate, br',
 	'Content-Type': 'application/json', 'Accept': 'application/json',
 	'Connection': 'keep-alive', 'DNT': '1',
 	'Origin': 'https://pharos-api.ncats.io' }
 #
 IDTYPES_TARGET = {
@@ -26,15 +29,15 @@
 IDTYPES_DISEASE = {
 	'cui':{'type':'String'},
 	'doid':{'type':'String'},
 	'name':{'type':'String'},
 	}
 #
 #############################################################################
-def GetTargets(ids, idtype, ep=API_ENDPOINT, fout=None):
+def GetTargets(ids, idtype, ep=API_BASE_URL, fout=None):
   tags=[]; n_out=0;
   client = GraphqlClient(endpoint=ep, verify=True)
   query = f"""\
 query targetDetails($id: {IDTYPES_TARGET[idtype]['type']}) {{
   target(q: {{ {idtype}: $id }}) {{
     name
     tdl
@@ -57,15 +60,15 @@
       logging.error(e)
       continue
     print(json.dumps(data, indent=2))
     n_out+=1
   logging.info(f"n_in: {len(ids)}; n_out: {n_out}")
 
 #############################################################################
-def GetDiseases(ids, idtype, ep=API_ENDPOINT, fout=None):
+def GetDiseases(ids, idtype, ep=API_BASE_URL, fout=None):
   tags=[]; n_out=0;
   client = GraphqlClient(endpoint=ep, verify=True)
   query = f"""\
 query diseaseDetails($id: String) {{
   disease(name: $id) {{
     name
     dids {{ id, doName, dataSources, doDefinition }}
@@ -93,15 +96,15 @@
       logging.error(e)
       continue
     print(json.dumps(data, indent=2))
     n_out+=1
   logging.info(f"n_in: {len(ids)}; n_out: {n_out}")
 
 #############################################################################
-def Test(ep=API_ENDPOINT, fout=None):
+def Test(ep=API_BASE_URL, fout=None):
   client = GraphqlClient(endpoint=ep, verify=True)
   query = """\
 query diseaseDetails {{
   disease {{
     name
     dids {{
       id(id:"DOID:2841"), doName
```

### Comparing `BioClients-0.2.8/BioClients/idg/rss/Client.py` & `BioClients-0.2.9/BioClients/lincs/sigcom/Client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,47 @@
 #!/usr/bin/env python3
-"""
-IDG Resource Submission System
-https://rss.ccs.miami.edu/
-"""
-###
-import sys,os,re,argparse,time,logging
+#############################################################################
+### https://maayanlab.cloud/sigcom-lincs/#/API 
+#############################################################################
+import sys,os,re,argparse,json,logging
 #
-from ...idg import rss
+from ...lincs import sigcom as sigcom_lincs
 #
-##############################################################################
-if __name__=='__main__':
-  epilog="""\
-"""
-  parser = argparse.ArgumentParser(description="IDG RSS (Resource Submission System) REST API client)", epilog=epilog)
-  ops = [ "list_targets", "get_target_resources" ]
-  parser.add_argument("op", choices=ops, help="operation")
-  parser.add_argument("--i", dest="ifile", help="input IDs")
-  parser.add_argument("--ids", help="IDs (comma-separated)")
+#############################################################################
+if __name__=="__main__":
+  parser = argparse.ArgumentParser(description='CLUE.IO REST API client utility')
+  ops = ['getResources', ]
+  parser.add_argument("op", choices=ops, help='OPERATION')
+  parser.add_argument("--ids", help="IDs, comma-separated")
+  parser.add_argument("--i", dest="ifile", help="input file, IDs")
   parser.add_argument("--o", dest="ofile", help="output (TSV)")
-  parser.add_argument("--api_host", default=rss.Utils.API_HOST)
-  parser.add_argument("--api_base_path", default=rss.Utils.API_BASE_PATH)
-  parser.add_argument("-v", "--verbose", default=0, action="count")
+  parser.add_argument("--nmax", type=int, default=1000, help="max results")
+  parser.add_argument("--skip", type=int, default=0, help="skip results")
+  parser.add_argument("--api_host", default=sigcom_lincs.Utils.API_HOST)
+  parser.add_argument("--api_base_path", default=sigcom_lincs.Utils.API_BASE_PATH)
+  parser.add_argument("-v", "--verbose", dest="verbose", action="count", default=0)
   args = parser.parse_args()
 
   logging.basicConfig(format='%(levelname)s:%(message)s', level=(logging.DEBUG if args.verbose>1 else logging.INFO))
 
-  fout = open(args.ofile, "w") if args.ofile else sys.stdout
+  base_url = 'https://'+args.api_host+args.api_base_path
+
+  fout = open(args.ofile, "w+") if args.ofile else sys.stdout
 
-  ids=[]
   if args.ifile:
     fin = open(args.ifile)
+    ids=[];
     while True:
       line = fin.readline()
       if not line: break
       ids.append(line.rstrip())
     fin.close()
+    logging.info(f"input queries: {len(ids)}")
   elif args.ids:
-    ids = re.split('[,\s]+', args.ids.strip())
-  if ids: logging.info('Input IDs: %d'%(len(ids)))
+    ids = re.split('[, ]+', args.ids.strip())
 
-  t0=time.time()
-
-  base_url = 'https://'+args.api_host+args.api_base_path
-
-  if args.op=='list_targets':
-    rss.Utils.ListTargets(base_url, fout)
-
-  elif args.op=='get_target_resources':
-    if not ids: parser.error(f"--i or --ids required for {args.op}")
-    rss.Utils.GetTargetResources(ids, base_url, fout)
+  if args.op=='getResources':
+    if not ids: parser.error('--ids or --i required.')
+    sigcom_lincs.Utils.GetResources(ids, base_url, fout)
 
   else:
-    parser.error(f'Unknown operation: {args.op}')
-
-  logging.info(('elapsed time: %s'%(time.strftime('%Hh:%Mm:%Ss',time.gmtime(time.time()-t0)))))
+    parser.error(f"Unsupported operation: {args.op}")
```

### Comparing `BioClients-0.2.8/BioClients/idg/rss/Utils.py` & `BioClients-0.2.9/BioClients/idg/rss/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/idg/tcrd/Client.py` & `BioClients-0.2.9/BioClients/idg/tcrd/Client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,50 +42,41 @@
   parser.add_argument("-q", "--quiet", action="store_true", help="Suppress progress notification.")
   args = parser.parse_args()
 
   # logging.PROGRESS = 15 (custom)
   logging.basicConfig(format='%(levelname)s:%(message)s', level=(logging.DEBUG if args.verbose>0 else logging.ERROR if args.quiet else 15))
 
   params = util_yaml.ReadParamFile(args.param_file) if os.path.isfile(args.param_file) else {}
-  if args.dbhost: params['DBHOST'] = args.dbhost 
-  if args.dbport: params['DBPORT'] = args.dbport 
-  if args.dbusr: params['DBUSR'] = args.dbusr 
-  if args.dbpw: params['DBPW'] = args.dbpw
-  if args.dbname: params['DBNAME'] = args.dbname 
+  if args.dbhost is not None: params['DBHOST'] = args.dbhost 
+  if args.dbport is not None: params['DBPORT'] = args.dbport 
+  if args.dbusr is not None: params['DBUSR'] = args.dbusr 
+  if args.dbpw is not None: params['DBPW'] = args.dbpw
+  if args.dbname is not None: params['DBNAME'] = args.dbname 
 
   fout = open(args.ofile, "w+") if args.ofile else sys.stdout
 
   ids=[]
   if args.ifile:
     fin = open(args.ifile)
     while True:
       line = fin.readline()
       if not line: break
       ids.append(line.rstrip())
-    logging.info('Input IDs: %d'%(len(ids)))
+    logging.info(f"Input IDs: {len(ids)}")
     fin.close()
   elif args.ids:
     ids = re.split(r'[,\s]+', args.ids)
 
-#  try:
-#    import mysql.connector as mysql
-#    dbcon = mysql.connect(host=params['DBHOST'], port=params['DBPORT'], user=params['DBUSR'], passwd=params['DBPW'], db=params['DBNAME'])
-#  except Exception as e:
-#    logging.error(f'{e}')
-#    try:
-#      import MySQLdb as mysql
-#      dbcon = mysql.connect(host=params['DBHOST'], port=int(params['DBPORT']), user=params['DBUSR'], passwd=params['DBPW'], db=params['DBNAME'])
-#    except Exception as e2:
-#      logging.error(f'{e2}')
-#      sys.exit(1)
-
   try:
     dbcon = util_db.MySqlConnect(dbhost=params['DBHOST'], dbport=params['DBPORT'], dbusr=params['DBUSR'], dbpw=params['DBPW'], dbname=params['DBNAME'])
   except Exception as e:
-    logging.error(f'{e}')
+    logging.error(f"{e}")
+    dbcon = None
+  if dbcon is None:
+    logging.error(f"""Failed: MySqlConnect(dbhost="{params['DBHOST']}", dbport={params['DBPORT']}, dbusr="{params['DBUSR']}", dbpw="{params['DBPW']}", dbname="{params['DBNAME']}")""")
     sys.exit(1)
 
   if args.op=='listColumns':
     tcrd.Utils.ListColumns(dbcon, fout)
 
   elif args.op=='info':
     tcrd.Utils.Info(dbcon, fout)
```

### Comparing `BioClients-0.2.8/BioClients/idg/tcrd/Utils.py` & `BioClients-0.2.9/BioClients/idg/tcrd/Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,35 +348,38 @@
 def ListDiseases(dbcon, fout=None):
   "Ontologies: DOID, UMLS, MESH, AmyCo, OrphaNet, NCBIGene"
   sql="""
 SELECT
 	disease.name diseaseName,
 	disease.did diseaseId,
 	IF((disease.did REGEXP '^C[0-9]+$'), 'UMLS', SUBSTR(disease.did, 1, LOCATE(':', disease.did)-1)) diseaseOntology,
+	disease.mondoid mondoId,
 	disease.description diseaseDescription,
 	disease.dtype associationType,
 	disease_type.description associationDescription,
 	disease.source associationSource,
 	COUNT(disease.protein_id) nTargetAssociations
 FROM
 	disease
 	LEFT OUTER JOIN disease_type ON disease_type.name = disease.dtype
 GROUP BY
 	disease.dtype,
 	disease_type.description,
 	disease.name,
 	disease.did,
+	disease.mondoid,
 	disease.description,
 	disease.source
 """
   df = pd.read_sql(sql, dbcon)
   if fout is not None: df.to_csv(fout, "\t", index=False)
   logging.info(f"rows: {df.shape[0]}")
   logging.info(f"diseaseIDs: {df.diseaseId.nunique()}")
   logging.info(f"diseaseNames: {df.diseaseName.nunique()}")
+  logging.info(f"mondoIDs: {df.mondoId.nunique()}")
   for ontology in sorted(df.diseaseOntology.unique().astype(str).tolist()):
     if df[df.diseaseOntology==ontology].diseaseId.nunique()>0:
       logging.info(f"[{ontology}] diseaseIDs: {df[df.diseaseOntology==ontology].diseaseId.nunique()}")
   return df
 
 #############################################################################
 def ListDiseaseTypes(dbcon, fout=None):
@@ -392,14 +395,15 @@
 def GetDiseaseAssociations(dbcon, ids, fout=None):
   n_id=0; n_hit=0; df=pd.DataFrame();
   sql = """\
 SELECT
 	disease.name diseaseName,
 	disease.did diseaseId,
 	IF((disease.did REGEXP '^C[0-9]+$'), 'UMLS', SUBSTR(disease.did, 1, LOCATE(':', disease.did)-1)) diseaseOntology,
+	disease.mondoid mondoId,
 	disease.description diseaseDescription,
 	disease.dtype associationType,
 	disease_type.description associationDescription,
 	disease.source associationSource,
 	protein.id tcrdProteinId,
 	protein.uniprot uniprotId,
 	protein.sym tcrdGeneSymbol
@@ -419,15 +423,15 @@
     else: df = pd.concat([df, df_this])
   logging.info(f"n_id: {n_id}; n_hit: {n_hit}")
   if fout is None: return df
 
 #############################################################################
 def GetDiseaseAssociationsPage(dbcon, did, fout=None):
   df = GetDiseaseAssociations(dbcon, [did], None)
-  disease = df[["diseaseName", "diseaseId", "diseaseOntology", "diseaseDescription"]].drop_duplicates().to_dict(orient='records')[0]
+  disease = df[["diseaseName", "diseaseId", "diseaseOntology", "mondoId", "diseaseDescription"]].drop_duplicates().to_dict(orient='records')[0]
   associations = df[["associationType", "associationDescription", "associationSource", "tcrdProteinId", "uniprotId", "tcrdGeneSymbol"]].to_dict(orient='records')
   disease["associations"] = associations
   fout.write(json.dumps(disease, indent=2))
 
 #############################################################################
 def ListPhenotypes(dbcon, fout=None):
   sql="""
```

### Comparing `BioClients-0.2.8/BioClients/idg/tiga/Client.py` & `BioClients-0.2.9/BioClients/idg/tiga/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/idg/tiga/Utils.py` & `BioClients-0.2.9/BioClients/idg/tiga/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/idg/tinx/Client.py` & `BioClients-0.2.9/BioClients/idg/tinx/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/idg/tinx/Utils.py` & `BioClients-0.2.9/BioClients/idg/tinx/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/iuphar/Client.py` & `BioClients-0.2.9/BioClients/iuphar/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/iuphar/Utils.py` & `BioClients-0.2.9/BioClients/iuphar/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/jensenlab/Client.py` & `BioClients-0.2.9/BioClients/jensenlab/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/jensenlab/Utils.py` & `BioClients-0.2.9/BioClients/jensenlab/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/lincs/Client.py` & `BioClients-0.2.9/BioClients/lincs/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/lincs/Client_lincscloud.py` & `BioClients-0.2.9/BioClients/lincs/Client_lincscloud.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/lincs/Utils.py` & `BioClients-0.2.9/BioClients/lincs/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/lincs/clue/Client.py` & `BioClients-0.2.9/BioClients/lincs/clue/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/lincs/clue/Utils.py` & `BioClients-0.2.9/BioClients/lincs/clue/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/lincs/sigcom/Client.py` & `BioClients-0.2.9/BioClients/maayanlab/harmonizome/Client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 #!/usr/bin/env python3
-#############################################################################
-### https://maayanlab.cloud/sigcom-lincs/#/API 
-#############################################################################
-import sys,os,re,argparse,json,logging
+"""
+See: http://amp.pharm.mssm.edu/Harmonizome/documentation
+"""
+###
+import sys,os,re,argparse,time,json,logging
 #
-from ...lincs import sigcom as sigcom_lincs
+from ... import maayanlab
 #
-#############################################################################
-if __name__=="__main__":
-  parser = argparse.ArgumentParser(description='CLUE.IO REST API client utility')
-  ops = ['getResources', ]
-  parser.add_argument("op", choices=ops, help='OPERATION')
-  parser.add_argument("--ids", help="IDs, comma-separated")
-  parser.add_argument("--i", dest="ifile", help="input file, IDs")
+#
+##############################################################################
+if __name__=='__main__':
+  parser = argparse.ArgumentParser(description='MaayanLab Harmonizome REST API client')
+  ops = [ 'get_gene', 'get_gene_associations' ]
+  parser.add_argument("op", choices=ops, help='operation')
+  parser.add_argument("--i", dest="ifile", help="input IDs")
+  parser.add_argument("--ids", help="input IDs (comma-separated)")
   parser.add_argument("--o", dest="ofile", help="output (TSV)")
-  parser.add_argument("--nmax", type=int, default=1000, help="max results")
-  parser.add_argument("--skip", type=int, default=0, help="skip results")
-  parser.add_argument("--api_host", default=sigcom_lincs.Utils.API_HOST)
-  parser.add_argument("--api_base_path", default=sigcom_lincs.Utils.API_BASE_PATH)
-  parser.add_argument("-v", "--verbose", dest="verbose", action="count", default=0)
+  parser.add_argument("--api_host", default=maayanlab.harmonizome.API_HOST)
+  parser.add_argument("--api_base_path", default=maayanlab.harmonizome.API_BASE_PATH)
+  parser.add_argument("-v", "--verbose", default=0, action="count")
   args = parser.parse_args()
 
   logging.basicConfig(format='%(levelname)s:%(message)s', level=(logging.DEBUG if args.verbose>1 else logging.INFO))
 
   base_url = 'https://'+args.api_host+args.api_base_path
 
-  fout = open(args.ofile, "w+") if args.ofile else sys.stdout
+  fout = open(args.ofile,"w") if args.ofile else sys.stdout
+
+  t0=time.time()
 
+  ids=[];
   if args.ifile:
     fin = open(args.ifile)
-    ids=[];
     while True:
       line = fin.readline()
       if not line: break
-      ids.append(line.rstrip())
+      if line.rstrip(): ids.append(line.rstrip())
     fin.close()
-    logging.info(f"input queries: {len(ids)}")
   elif args.ids:
-    ids = re.split('[, ]+', args.ids.strip())
+    ids = re.split(r'[,\s]+', args.ids)
+  logging.info(f"Input queries: {len(ids)}")
 
-  if args.op=='getResources':
-    if not ids: parser.error('--ids or --i required.')
-    sigcom_lincs.Utils.GetResources(ids, base_url, fout)
+  if args.op == "get_gene":
+    maayanlab.harmonizome.Utils.GetGene(ids, base_url, fout)
+
+  elif args.op == "get_gene_associations":
+    maayanlab.harmonizome.Utils.GetGeneAssociations(ids, base_url, fout)
 
   else:
-    parser.error(f"Unsupported operation: {args.op}")
+    parser.error(f"Invalid operation: {args.op}")
+
+  logging.info(f"elapsed time: {time.strftime('%Hh:%Mm:%Ss', time.gmtime(time.time()-t0))}")
```

### Comparing `BioClients-0.2.8/BioClients/lincs/sigcom/Utils.py` & `BioClients-0.2.9/BioClients/lincs/sigcom/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/maayanlab/archs4/Client.py` & `BioClients-0.2.9/BioClients/maayanlab/archs4/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/maayanlab/archs4/Utils.py` & `BioClients-0.2.9/BioClients/maayanlab/archs4/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/maayanlab/harmonizome/Client.py` & `BioClients-0.2.9/BioClients/tcga/Client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 #!/usr/bin/env python3
 """
-See: http://amp.pharm.mssm.edu/Harmonizome/documentation
+See: https://docs.gdc.cancer.gov/API/Users_Guide/
 """
 ###
 import sys,os,re,argparse,time,json,logging
 #
-from ... import maayanlab
+from .. import tcga
 #
+API_HOST='api.gdc.cancer.gov'
+API_BASE_PATH=''
 #
 ##############################################################################
 if __name__=='__main__':
-  parser = argparse.ArgumentParser(description='MaayanLab Harmonizome REST API client')
-  ops = [ 'get_gene', 'get_gene_associations' ]
+  parser = argparse.ArgumentParser(description='TCGA REST API client')
+  ops = [ 'list_projects', 'list_cases', 'list_files', 'list_annotations' ]
   parser.add_argument("op", choices=ops, help='operation')
   parser.add_argument("--i", dest="ifile", help="input IDs")
   parser.add_argument("--ids", help="input IDs (comma-separated)")
   parser.add_argument("--o", dest="ofile", help="output (TSV)")
-  parser.add_argument("--api_host", default=maayanlab.harmonizome.API_HOST)
-  parser.add_argument("--api_base_path", default=maayanlab.harmonizome.API_BASE_PATH)
+  parser.add_argument("--skip", type=int, default=0)
+  parser.add_argument("--nmax", type=int, default=None)
+  parser.add_argument("--api_host", default=API_HOST)
+  parser.add_argument("--api_base_path", default=API_BASE_PATH)
   parser.add_argument("-v", "--verbose", default=0, action="count")
   args = parser.parse_args()
 
   logging.basicConfig(format='%(levelname)s:%(message)s', level=(logging.DEBUG if args.verbose>1 else logging.INFO))
 
   base_url = 'https://'+args.api_host+args.api_base_path
 
@@ -35,19 +39,25 @@
     while True:
       line = fin.readline()
       if not line: break
       if line.rstrip(): ids.append(line.rstrip())
     fin.close()
   elif args.ids:
     ids = re.split(r'[,\s]+', args.ids)
-  logging.info(f"Input queries: {len(ids)}")
+  logging.info('Input queries: %d'%(len(ids)))
 
-  if args.op == "get_gene":
-    maayanlab.harmonizome.Utils.GetGene(ids, base_url, fout)
+  if args.op == "list_projects":
+    tcga.ListProjects(base_url, args.skip, args.nmax, fout)
 
-  elif args.op == "get_gene_associations":
-    maayanlab.harmonizome.Utils.GetGeneAssociations(ids, base_url, fout)
+  elif args.op == "list_cases":
+    tcga.ListCases(base_url, args.skip, args.nmax, fout)
+
+  elif args.op == "list_files":
+    tcga.ListFiles(base_url, args.skip, args.nmax, fout)
+
+  elif args.op == "list_annotations":
+    tcga.ListAnnotations(base_url, args.skip, args.nmax, fout)
 
   else:
-    parser.error(f"Invalid operation: {args.op}")
+    parser.error("Invalid operation: %s"%args.op)
 
-  logging.info(f"elapsed time: {time.strftime('%Hh:%Mm:%Ss', time.gmtime(time.time()-t0))}")
+  logging.info(('elapsed time: %s'%(time.strftime('%Hh:%Mm:%Ss', time.gmtime(time.time()-t0)))))
```

### Comparing `BioClients-0.2.8/BioClients/maayanlab/harmonizome/Utils.py` & `BioClients-0.2.9/BioClients/maayanlab/harmonizome/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/medline/connect/Client.py` & `BioClients-0.2.9/BioClients/medline/connect/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/medline/connect/Utils.py` & `BioClients-0.2.9/BioClients/medline/connect/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/medline/genetics/Client.py` & `BioClients-0.2.9/BioClients/medline/genetics/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/medline/genetics/Utils.py` & `BioClients-0.2.9/BioClients/medline/genetics/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/mesh/Client.py` & `BioClients-0.2.9/BioClients/mesh/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/mesh/Utils.py` & `BioClients-0.2.9/BioClients/mesh/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/monarch/Biolink.py` & `BioClients-0.2.9/BioClients/monarch/Biolink.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/monarch/Client.py` & `BioClients-0.2.9/BioClients/monarch/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/monarch/Utils.py` & `BioClients-0.2.9/BioClients/monarch/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/mygene/Client.py` & `BioClients-0.2.9/BioClients/mygene/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/mygene/Utils.py` & `BioClients-0.2.9/BioClients/mygene/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/ncbo/Client.py` & `BioClients-0.2.9/BioClients/ncbo/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/ncbo/Utils.py` & `BioClients-0.2.9/BioClients/ncbo/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/omim/Client.py` & `BioClients-0.2.9/BioClients/omim/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/openphacts/Client.py` & `BioClients-0.2.9/BioClients/openphacts/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/openphacts/Utils.py` & `BioClients-0.2.9/BioClients/openphacts/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/opentargets/Client.py` & `BioClients-0.2.9/BioClients/opentargets/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/opentargets/Utils.py` & `BioClients-0.2.9/BioClients/opentargets/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/panther/Client.py` & `BioClients-0.2.9/BioClients/panther/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pdb/Client.py` & `BioClients-0.2.9/BioClients/pdb/Client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,64 @@
 #!/usr/bin/env python3
 """
 Utility for PDB REST API.
-See: http://www.rcsb.org/pdb/software/rest.do
+https://www.rcsb.org/docs/programmatic-access/web-services-overview
+https://data.rcsb.org/redoc/
 """
 ###
 import sys,os,re,json,argparse,time,logging
 #
-from .. import pdb
-#
-API_HOST='www.rcsb.org'
-API_BASE_PATH='/pdb/rest'
+from .. import pdb as pdb_utils
 #
 ##############################################################################
 if __name__=='__main__':
   epilog="""
-Example keywords: ACTIN, Example UniProts: P50225'.
-get_uniprots functionality may be discontinued by PDB.
+Example entry IDs: 3ERT, 3TTC
+Example chemical IDs: CFF
 """
   parser = argparse.ArgumentParser(description='PDB REST API client', epilog=epilog)
-  ops = ['show_counts',
-    'list_proteins', 'list_ligands',
-    'search',
-    'get_proteins', 'get_ligands', 'get_ligands_LID2SDF',
-    'get_uniprots']
-  parser.add_argument("op", choices=ops, help='operation')
-  parser.add_argument("--ids", dest="ids", help="PDB IDs, comma-separated")
-  parser.add_argument("--i", dest="ifile", help="input file, PDB IDs")
-  parser.add_argument("--druglike", action="store_true", help="druglike ligands only (organic; !polymer; !monoatomic)")
+  ops = ['list_entrys', 
+    'get_entrys', 'get_chemicals', 
+    ]
+  parser.add_argument("op", choices=ops, help='OPERATION')
+  parser.add_argument("--ids", dest="ids", help="PDB entry IDs, comma-separated")
+  parser.add_argument("--i", dest="ifile", help="input file, PDB entry IDs")
+  parser.add_argument("--druglike", action="store_true", help="druglike chemicals only (organic; !polymer; !monoatomic)")
   parser.add_argument("--o", dest="ofile", help="output file (TSV)")
-  parser.add_argument("--qstr", help="search query")
-  parser.add_argument("--api_host", default=API_HOST)
-  parser.add_argument("--api_base_path", default=API_BASE_PATH)
+  parser.add_argument("--api_host", default=pdb_utils.API_HOST)
+  parser.add_argument("--api_base_path", default=pdb_utils.API_BASE_PATH)
   parser.add_argument("-v", "--verbose", action="count", default=0)
-
   args = parser.parse_args()
 
   logging.basicConfig(format='%(levelname)s:%(message)s', level=(logging.DEBUG if args.verbose>1 else logging.INFO))
 
-  BASE_URL='https://'+args.api_host+args.api_base_path
+  base_url = f"https://{args.api_host}{args.api_base_path}"
 
   ids=[]
   if args.ifile:
     fin = open(args.ifile)
     while True:
       line = fin.readline()
       if not line: break
       ids.append(line.strip())
   elif args.ids:
     ids = re.split('[, ]+', args.ids.strip())
 
-  if args.ofile:
-    fout = open(args.ofile, "w+")
-  else:
-    fout = sys.stdout
+  fout = open(args.ofile, "w+") if args.ofile else sys.stdout
 
   t0=time.time()
 
-  if args.op == "get_proteins":
-    if not ids: parser.error('ID[s] required.')
-    pdb.GetProteins(BASE_URL, ids, fout)
-
-  elif args.op == "get_uniprots":
+  if args.op == "get_entrys":
     if not ids: parser.error('ID[s] required.')
-    pdb.GetUniprots(BASE_URL, ids, fout)
+    pdb_utils.GetEntrys(ids, base_url, fout)
 
-  elif args.op == "get_ligands":
+  elif args.op == "get_chemicals":
     if not ids: parser.error('ID[s] required.')
-    pdb.GetLigands(BASE_URL, ids, args.druglike, fout)
-
-  elif args.op == "get_ligands_LID2SDF":
-    if not ids: parser.error('ID[s] required.')
-    pdb.GetLigands_LID2SDF(BASE_URL, ids, fout)
-
-  elif args.op == "list_proteins":
-    pdb.ListProteins(BASE_URL, fout)
-
-  elif args.op == "list_ligands":
-    pdb.ListLigands(BASE_URL, args.druglike, fout)
-
-  elif args.op == "show_counts":
-    pdb.ShowCounts(BASE_URL)
+    pdb_utils.GetChemicals(ids, args.druglike, base_url, fout)
 
-  elif args.op == "search":
-    ids = pdb.SearchByKeywords(BASE_URL, args.qstr)
-    logging.info('protein count: %d'%(len(ids)))
-    pdb.GetProteins(BASE_URL, ids, fout)
+  elif args.op == "list_entrys":
+    pdb_utils.ListEntrys(base_url, fout)
 
   else:
-    parser.error('Invalid operation: %s'%args.op)
+    parser.error(f"Invalid operation: {args.op}")
 
-  logging.info(('elapsed time: %s'%(time.strftime('%Hh:%Mm:%Ss', time.gmtime(time.time()-t0)))))
+  logging.info(f"Elapsed time: {time.strftime('%Hh:%Mm:%Ss', time.gmtime(time.time()-t0))}")
```

### Comparing `BioClients-0.2.8/BioClients/pubchem/Client.py` & `BioClients-0.2.9/BioClients/pubchem/Client.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,24 +17,26 @@
         "get_cid2properties", "get_cid2inchi",
         "get_cid2descriptions",
         "get_cid2synonyms", "get_cid2sid", "get_cid2assaysummary",
         "get_cid2nicename",
         "get_sid2cid", "get_sid2sdf", "get_sid2assaysummary",
         "get_assayname", "get_assaydescriptions",
 	"get_assaysubstances",
-	"get_assaysubstanceresults",]
+	"get_assaysubstanceresults",
+        "get_compoundview", "get_substanceview", "get_assayview",]
   parser = argparse.ArgumentParser(description="PubChem PUG REST client")
   parser.add_argument("op", choices=OPS, help="OPERATION")
   parser.add_argument("--i", dest="ifile", help="input IDs file (CID|SID|SMILES|name)")
   parser.add_argument("--ids", help="input IDs (CID|SID|SMILES|name) (comma-separated)")
   parser.add_argument("--aids", help="input AIDs (comma-separated)")
   parser.add_argument("--iaid", dest="ifile_aid", help="input AIDs file")
   parser.add_argument("--o", dest="ofile", help="output (usually TSV)")
   parser.add_argument("--api_host", default=pubchem.API_HOST)
   parser.add_argument("--api_base_path", default=pubchem.API_BASE_PATH)
+  parser.add_argument("--api_base_path_view", default=pubchem.API_BASE_PATH_VIEW)
   parser.add_argument("--skip", type=int, default=0)
   parser.add_argument("--nmax", type=int, default=0)
   parser.add_argument("--nmax_per_cid", type=int, default=20)
   parser.add_argument("-q", "--quiet", action="store_true", help="Suppress progress notification.")
   parser.add_argument("-v", "--verbose", default=0, action="count")
   args = parser.parse_args()
 
@@ -99,23 +101,30 @@
 
   elif args.op == 'get_cid2sdf':
     pubchem.GetCID2SDF(ids, base_url, fout)
 
   elif args.op == 'get_cid2assaysummary':
     pubchem.GetCID2AssaySummary(ids, base_url, fout)
 
+  elif args.op == 'get_compoundview':
+    base_url = f"https://{args.api_host}{args.api_base_path_view}"
+    pubchem.GetCompoundView(ids, base_url, fout)
+
   elif args.op == 'get_sid2cid':
     pubchem.GetSID2CID(ids, base_url, fout)
 
   elif args.op == 'get_sid2assaysummary':
     pubchem.GetSID2AssaySummary(ids, base_url, fout)
 
   elif args.op == 'get_sid2sdf':
     pubchem.GetSID2SDF(ids, fout, args.skip, args.nmax, base_url)
 
+  elif args.op == 'get_substanceview':
+    pubchem.GetSubstanceView(ids, base_url, fout)
+
   elif args.op == 'get_smi2cid':
     pubchem.GetSmiles2CID(ids, base_url, fout)
 
   elif args.op == 'get_name2sid':
     pubchem.GetName2SID(ids, args.skip, args.nmax, base_url, fout)
 
   elif args.op == 'get_name2cid':
@@ -129,14 +138,17 @@
 
   elif args.op == 'get_assaydescriptions':
     pubchem.GetAssayDescriptions(aids, args.skip, args.nmax, base_url, fout)
 
   elif args.op == 'get_assaysubstances':
     pubchem.Utils.GetAssaySIDs(aids, args.skip, args.nmax, base_url, fout)
 
+  elif args.op == 'get_assayview':
+    pubchem.GetAssayView(aids, base_url, fout)
+
   elif args.op == 'get_assaysubstanceresults':
     if not (aids and ids): parser.error('Input AIDs and SIDs required.')
     pubchem.GetAssaySIDResults(aids, ids, args.skip, args.nmax, base_url, fout)
 
   else:
     parser.error(f"Invalid operation: {args.op}")
```

### Comparing `BioClients-0.2.8/BioClients/pubchem/Utils.py` & `BioClients-0.2.9/BioClients/pubchem/Utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         'active':2,
         'inconclusive':3,
         'unspecified':4,
         'probe':5}
 #
 API_HOST='pubchem.ncbi.nlm.nih.gov'
 API_BASE_PATH='/rest/pug'
+API_BASE_PATH_VIEW='/rest/pug_view'
 BASE_URL="https://"+API_HOST+API_BASE_PATH
 #
 NCHUNK=100
 #
 #############################################################################
 def OutcomeCode(txt):
   return OUTCOME_CODES[txt.lower()] if txt.lower() in OUTCOME_CODES else OUTCOME_CODES['unspecified']
@@ -824,7 +825,61 @@
 
     fout.write(f"{cid}\t{sid}\t{aid}\t{outcome_code}\t{actval:.3f}\n")
 
   logging.info(f"[CID={cid_query}] records: {n_in}; activities: {n_act}")
   return True
 
 #############################################################################
+def GetCompoundView(ids, base_url=BASE_URL, fout=None):
+  n_out=0; results=[];
+  for i_cid in tqdm.auto.trange(len(ids), desc="CIDs"):
+    id_this = ids[i_cid]
+    response = requests.get(base_url+f"/data/compound/{id_this}/JSON")
+    if response.status_code != 200:
+      logging.info(f"Not found (status_code={response.status_code}): {id_this}")
+      continue
+    result = response.json()
+    if fout is not None:
+      fout.write(json.dumps(result, indent=2))
+    else:
+      results.append(result)
+    n_out+=1
+  logging.info(f"CIDs: {len(ids)}; out: {n_out}")
+  return results
+
+#############################################################################
+def GetSubstanceView(ids, base_url=BASE_URL, fout=None):
+  n_out=0; results=[];
+  for i_sid in tqdm.auto.trange(len(ids), desc="CIDs"):
+    id_this = ids[i_sid]
+    response = requests.get(base_url+f"/data/substance/{id_this}/JSON")
+    if response.status_code != 200:
+      logging.info(f"Not found (status_code={response.status_code}): {id_this}")
+      continue
+    result = response.json()
+    if fout is not None:
+      fout.write(json.dumps(result, indent=2))
+    else:
+      results.append(result)
+    n_out+=1
+  logging.info(f"SIDs: {len(ids)}; out: {n_out}")
+  return results
+
+#############################################################################
+def GetAssayView(ids, base_url=BASE_URL, fout=None):
+  n_out=0; results=[];
+  for i_aid in tqdm.auto.trange(len(ids), desc="CIDs"):
+    id_this = ids[i_aid]
+    response = requests.get(base_url+f"/data/bioassay/{id_this}/JSON")
+    if response.status_code != 200:
+      logging.info(f"Not found (status_code={response.status_code}): {id_this}")
+      continue
+    result = response.json()
+    if fout is not None:
+      fout.write(json.dumps(result, indent=2))
+    else:
+      results.append(result)
+    n_out+=1
+  logging.info(f"AIDs: {len(ids)}; out: {n_out}")
+  return results
+
+#############################################################################
```

### Comparing `BioClients-0.2.8/BioClients/pubchem/ftp/Client.py` & `BioClients-0.2.9/BioClients/pubchem/ftp/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/ftp/Utils.py` & `BioClients-0.2.9/BioClients/pubchem/ftp/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_actives.py` & `BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_actives.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_assay_fetch.py` & `BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_assay_fetch.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_assay_results.py` & `BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_assay_results.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_assay_search.py` & `BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_assay_search.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_assaysim.py` & `BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_assaysim.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_compound_assaystats.py` & `BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_compound_assaystats.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/ftp/pubchem_ftp_gini_index.py` & `BioClients-0.2.9/BioClients/pubchem/ftp/pubchem_ftp_gini_index.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/rdf/Client.py` & `BioClients-0.2.9/BioClients/pubchem/rdf/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/soap/Client.py` & `BioClients-0.2.9/BioClients/pubchem/soap/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/soap/Utils.py` & `BioClients-0.2.9/BioClients/pubchem/soap/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/soap/pug_aids2assays.py` & `BioClients-0.2.9/BioClients/pubchem/soap/pug_aids2assays.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/soap/pug_ids2mols.py` & `BioClients-0.2.9/BioClients/pubchem/soap/pug_ids2mols.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubchem/soap/pug_substance_search.py` & `BioClients-0.2.9/BioClients/pubchem/soap/pug_substance_search.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubmed/Utils.py` & `BioClients-0.2.9/BioClients/pubmed/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubtator/Client.py` & `BioClients-0.2.9/BioClients/pubtator/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/pubtator/Utils.py` & `BioClients-0.2.9/BioClients/pubtator/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/reactome/Client.py` & `BioClients-0.2.9/BioClients/reactome/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/reactome/SMBL_utils.py` & `BioClients-0.2.9/BioClients/reactome/SMBL_utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/reactome/Utils.py` & `BioClients-0.2.9/BioClients/reactome/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/rxnorm/Client.py` & `BioClients-0.2.9/BioClients/rxnorm/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/rxnorm/Utils.py` & `BioClients-0.2.9/BioClients/rxnorm/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/stringdb/Client.py` & `BioClients-0.2.9/BioClients/stringdb/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/stringdb/Utils.py` & `BioClients-0.2.9/BioClients/stringdb/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/tcga/Client.py` & `BioClients-0.2.9/BioClients/ncats/gsrs/Client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,80 @@
 #!/usr/bin/env python3
 """
-See: https://docs.gdc.cancer.gov/API/Users_Guide/
+https://ncats.nih.gov/expertise/preclinical/gsrs
+https://gsrs.ncats.nih.gov/
+https://gsrs.ncats.nih.gov/#/api
 """
-###
-import sys,os,re,argparse,time,json,logging
-#
-from .. import tcga
-#
-API_HOST='api.gdc.cancer.gov'
-API_BASE_PATH=''
+### 
+import sys,os,re,json,argparse,time,logging
+
+from ... import ncats
 #
-##############################################################################
+#############################################################################
 if __name__=='__main__':
-  parser = argparse.ArgumentParser(description='TCGA REST API client')
-  ops = [ 'list_projects', 'list_cases', 'list_files', 'list_annotations' ]
-  parser.add_argument("op", choices=ops, help='operation')
-  parser.add_argument("--i", dest="ifile", help="input IDs")
-  parser.add_argument("--ids", help="input IDs (comma-separated)")
-  parser.add_argument("--o", dest="ofile", help="output (TSV)")
-  parser.add_argument("--skip", type=int, default=0)
-  parser.add_argument("--nmax", type=int, default=None)
-  parser.add_argument("--api_host", default=API_HOST)
-  parser.add_argument("--api_base_path", default=API_BASE_PATH)
+  epilog='''\
+Example search queries:
+IBUPRO
+ASPIRIN
+OXYTOCIN
+OXYTO*
+ASPIRIN AND ESTER
+COCN
+C=1CC=CC=C1C(=O)O
+'''
+  parser = argparse.ArgumentParser(description='NCATS Global Substance Registration System (GSRS) client', epilog=epilog)
+  ops = [
+	'list_vocabularies',
+	'list_substances',
+	'search',
+	'get_substance',
+	'get_substance_names',
+	]
+  parser.add_argument("op", choices=ops, help='OPERATION')
+  parser.add_argument("--i", dest="ifile", help="Input IDs")
+  parser.add_argument("--o", dest="ofile", help="Output (TSV)")
+  parser.add_argument("--ids", help="Input IDs (comma-separated)")
+  parser.add_argument("--query", help="Search query.")
+  parser.add_argument("--api_host", default=ncats.gsrs.API_HOST)
+  parser.add_argument("--api_base_path", default=ncats.gsrs.API_BASE_PATH)
   parser.add_argument("-v", "--verbose", default=0, action="count")
   args = parser.parse_args()
 
   logging.basicConfig(format='%(levelname)s:%(message)s', level=(logging.DEBUG if args.verbose>1 else logging.INFO))
 
-  base_url = 'https://'+args.api_host+args.api_base_path
+  api_base_url = 'https://'+args.api_host+args.api_base_path
 
-  fout = open(args.ofile,"w") if args.ofile else sys.stdout
+  fout = open(args.ofile, "w+") if args.ofile else sys.stdout
 
   t0=time.time()
 
-  ids=[];
+  ids=[]
   if args.ifile:
     fin = open(args.ifile)
     while True:
       line = fin.readline()
       if not line: break
-      if line.rstrip(): ids.append(line.rstrip())
+      ids.append(line.rstrip())
     fin.close()
+    logging.info(f"Input IDs: {len(ids)}")
   elif args.ids:
     ids = re.split(r'[,\s]+', args.ids)
-  logging.info('Input queries: %d'%(len(ids)))
 
-  if args.op == "list_projects":
-    tcga.ListProjects(base_url, args.skip, args.nmax, fout)
+  if args.op == "list_vocabularies":
+    ncats.gsrs.Utils.ListVocabularies(api_base_url, fout)
+
+  elif args.op == "list_substances":
+    ncats.gsrs.Utils.ListSubstances(api_base_url, fout)
 
-  elif args.op == "list_cases":
-    tcga.ListCases(base_url, args.skip, args.nmax, fout)
+  elif args.op == "search":
+    ncats.gsrs.Utils.Search(args.query, api_base_url, fout)
 
-  elif args.op == "list_files":
-    tcga.ListFiles(base_url, args.skip, args.nmax, fout)
+  elif args.op == "get_substance":
+    ncats.gsrs.Utils.GetSubstance(ids, api_base_url, fout)
 
-  elif args.op == "list_annotations":
-    tcga.ListAnnotations(base_url, args.skip, args.nmax, fout)
+  elif args.op == "get_substance_names":
+    ncats.gsrs.Utils.GetSubstanceNames(ids, api_base_url, fout)
 
   else:
-    parser.error("Invalid operation: %s"%args.op)
+    parser.error(f"Invalid operation: {args.op}")
 
-  logging.info(('elapsed time: %s'%(time.strftime('%Hh:%Mm:%Ss', time.gmtime(time.time()-t0)))))
+  logging.info(f"Elapsed time: {time.strftime('%Hh:%Mm:%Ss',time.gmtime(time.time()-t0))}")
```

### Comparing `BioClients-0.2.8/BioClients/tcga/Utils.py` & `BioClients-0.2.9/BioClients/tcga/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/umls/Client.py` & `BioClients-0.2.9/BioClients/umls/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/umls/Utils.py` & `BioClients-0.2.9/BioClients/umls/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/uniprot/Client.py` & `BioClients-0.2.9/BioClients/uniprot/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/uniprot/Utils.py` & `BioClients-0.2.9/BioClients/uniprot/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/db/Utils.py` & `BioClients-0.2.9/BioClients/util/db/Utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,37 +3,42 @@
 Commonly used functions for database client applications.
 '''
 import sys,os,logging,urllib.parse
 import sqlalchemy
 
 ##############################################################################
 def PostgreSqlConnect(dbhost, dbport, dbname, dbusr, dbpw):
-  import psycopg2
-  engine = sqlalchemy.create_engine(f"postgresql+psycopg2://{dbusr}:{urllib.parse.quote_plus(dbpw)}@{dbhost}:{dbport}/{dbname}")
+  try:
+    import psycopg2
+    engine = sqlalchemy.create_engine(f"postgresql+psycopg2://{dbusr}:{urllib.parse.quote_plus(dbpw)}@{dbhost}:{dbport}/{dbname}")
+  except Exception as e:
+    logging.info(f"{e}")
+    logging.error("Failed to connect.")
+    return None
   return engine.connect()
 
 ##############################################################################
 def MySqlConnect(dbhost, dbport, dbname, dbusr, dbpw):
   try:
-    # pip install MySQL-python
-    # import mysql-python #default
-    engine = sqlalchemy.create_engine(f"mysql://{dbusr}:{urllib.parse.quote_plus(dbpw)}@{dbhost}:{dbport}/{dbname}")
-  except:
+    # https://pypi.org/project/mysql-connector-python/
+    # pip install mysql-connector-python
+    import mysql.connector
+    engine = sqlalchemy.create_engine(f"mysql+mysqlconnector://{dbusr}:{urllib.parse.quote_plus(dbpw)}@{dbhost}:{dbport}/{dbname}")
+  except Exception as e:
+    logging.info(f"{e}")
     try:
-      # pip install mysql-connector-python
-      # import mysql-connector-python
-      engine = sqlalchemy.create_engine(f"mysql+mysqlconnector://{dbusr}:{urllib.parse.quote_plus(dbpw)}@{dbhost}:{dbport}/{dbname}")
-    except:
+      # https://pypi.org/project/PyMySQL/
+      # pip install PyMySQL
+      import pymysql
+      engine = sqlalchemy.create_engine(f"mysql+pymysql://{dbusr}:{urllib.parse.quote_plus(dbpw)}@{dbhost}:{dbport}/{dbname}")
+    except Exception as e:
+      logging.info(f"{e}")
       try:
-        # pip install PyMySQL
-        # import pymysql
-        engine = sqlalchemy.create_engine(f"mysql+pymysql://{dbusr}:{urllib.parse.quote_plus(dbpw)}@{dbhost}:{dbport}/{dbname}")
-      except:
-        try:
-          # pip install MySQLdb
-          # import MySQLdb
-          engine = sqlalchemy.create_engine(f"mysql+mysqldb://{dbusr}:{urllib.parse.quote_plus(dbpw)}@{dbhost}:{dbport}/{dbname}")
-        except:
-          logging.error("Failed to connect.")
-          return None
-
+        # https://mysqlclient.readthedocs.io/
+        # pip install mysqlclient
+        import MySQLdb
+        engine = sqlalchemy.create_engine(f"mysql+mysqldb://{dbusr}:{urllib.parse.quote_plus(dbpw)}@{dbhost}:{dbport}/{dbname}")
+      except Exception as e:
+        logging.info(f"{e}")
+        logging.error("Failed to connect.")
+        return None
   return engine.connect()
```

### Comparing `BioClients-0.2.8/BioClients/util/graphql/Utils.py` & `BioClients-0.2.9/BioClients/util/graphql/Utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 #!/usr/bin/env python3
 ###
+# https://gql.readthedocs.io/en/stable/
+# https://gql.readthedocs.io/en/stable/usage/basic_usage.html
+###
 import sys,os,json,logging
 
-import gql
-from gql.transport.requests import RequestsHTTPTransport
+from gql import Client, gql
+from gql.transport.aiohttp import AIOHTTPTransport
 
 #############################################################################
-def RunQuery(gql_url, graphql, fout):
+def RunQuery(graphql, base_url, fout):
   if graphql is None:
     logging.error("No query.")
     return
 
-  _transport = RequestsHTTPTransport(gql_url)
-  client = gql.Client(transport=_transport, fetch_schema_from_transport=False)
+  transport = AIOHTTPTransport(url=base_url)
+  client = Client(transport=transport, fetch_schema_from_transport=True)
   logging.debug(f"client.schema: '{client.schema}'")
 
   try:
-    query = gql.gql(graphql)
-    rval = client.execute(query)
-    fout.write(json.dumps(rval, indent=2)+"\n")
+    query = gql(graphql)
+    result = client.execute(query)
+    fout.write(json.dumps(result, indent=2)+"\n")
   except Exception as e:
     logging.error(e)
 
 #############################################################################
```

### Comparing `BioClients-0.2.8/BioClients/util/igraph/App.py` & `BioClients-0.2.9/BioClients/util/igraph/App.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/igraph/Utils.py` & `BioClients-0.2.9/BioClients/util/igraph/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/neo4j/App.py` & `BioClients-0.2.9/BioClients/util/neo4j/App.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/neo4j/Utils.py` & `BioClients-0.2.9/BioClients/util/neo4j/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/obo/App.py` & `BioClients-0.2.9/BioClients/util/obo/App.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/obo/Utils.py` & `BioClients-0.2.9/BioClients/util/obo/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/pandas/App.py` & `BioClients-0.2.9/BioClients/util/pandas/App.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,32 +8,36 @@
 
 from .. import pandas as util_pandas
 
 #############################################################################
 if __name__=='__main__':
   verstr = (f'Python: {sys.version.split()[0]}; pandas: {pd.__version__}')
   parser = argparse.ArgumentParser(prog="BioClients.util.pandas.Utils", description='Pandas utilities for simple datafile transformations.', epilog=verstr)
-  ops = ['csv2tsv', 'shape', 'summary', 'showcols', 'list_columns', 'to_html',
+  ops = ['csv2tsv', 'tsv2csv', 'shape', 'summary', 'showcols', 'list_columns', 'to_html',
 	'selectcols', 'selectcols_deduplicate', 'uvalcounts',
 	'colvalcounts', 'sortbycols', 'deduplicate', 'colstats', 'searchrows',
-	'pickle', 'sample', 'set_header', 'remove_header']
+	'pickle', 'sample', 'set_header', 'remove_header', 'merge']
   compressions=['gzip', 'zip', 'bz2']
   parser.add_argument("op", choices=ops, help='OPERATION')
   parser.add_argument("--i", dest="ifile", required=True, help="input (CSV|TSV)")
+  parser.add_argument("--iB", dest="ifileB", help="input (CSV|TSV) for merge operation")
   parser.add_argument("--o", dest="ofile", help="output (CSV|TSV)")
   parser.add_argument("--coltags", help="cols specified by tag (comma-separated)")
   parser.add_argument("--cols", help="cols specified by idx (1+) (comma-separated)")
   parser.add_argument("--noheader", action="store_true", help="default: line-one is header")
   parser.add_argument("--search_qrys", help="qrys (comma-separated, NA|NaN handled specially)")
   parser.add_argument("--search_rels", default="=", help="relationships (=|>|<) (comma-separated)")
   parser.add_argument("--search_typs", default="str", help="types (str|int|float) (comma-separated)")
   parser.add_argument("--compression", choices=compressions)
   parser.add_argument("--csv", action="store_true", help="delimiter is comma")
   parser.add_argument("--tsv", action="store_true", help="delimiter is tab")
+  parser.add_argument("--clean_coltags", action="store_true", help="trim and replace whitespace, punctuation")
   parser.add_argument("--on_bad_lines", choices=["error", "warn", "skip"], default="warn")
+  parser.add_argument("--merge_how", choices=["left", "right", "outer", "inner", "cross"], default="inner")
+  parser.add_argument("--merge_type", choices=[str, int, float], default=str)
   parser.add_argument("--nrows", type=int)
   parser.add_argument("--skiprows", type=int)
   parser.add_argument("--sample_frac", type=float, default=.01, help="sampling probability (0-1)")
   parser.add_argument("--sample_n", type=int, help="sampling N")
   parser.add_argument("--html_title", help="table title")
   parser.add_argument("--html_prettify", action="store_true", help="requires Pandas v1.4.0+")
   parser.add_argument("-v", "--verbose", action="count", default=0)
@@ -52,15 +56,15 @@
   if args.compression: compression=args.compression
   elif re.search('\.gz$', args.ifile, re.I): compression='gzip'
   elif re.search('\.bz2$', args.ifile, re.I): compression='bz2'
   elif re.search('\.zip$', args.ifile, re.I): compression='zip'
   else: compression=None
 
   if args.csv or args.op=='csv2tsv': delim=','
-  elif args.tsv: delim='\t'
+  elif args.tsv or args.op=='tsv2csv': delim='\t'
   elif re.search('\.csv', args.ifile, re.I): delim=','
   elif re.search('\.tsv', args.ifile, re.I) or re.search('\.tab', args.ifile, re.I): delim='\t'
   else: delim='\t'
 
   cols=None; coltags=None;
   if args.cols:
     cols = [(int(col.strip())-1) for col in re.split(r',', args.cols.strip())]
@@ -69,14 +73,16 @@
 
   search_qrys = [qry.strip() for qry in re.split(r',', args.search_qrys.strip())] if (args.search_qrys is not None) else None
   search_rels = [rel.strip() for rel in re.split(r',', args.search_rels.strip())] if (args.search_rels is not None) else None
   search_typs = [typ.strip() for typ in re.split(r',', args.search_typs.strip())] if (args.search_typs is not None) else None
 
   df = pd.read_csv(args.ifile, sep=delim, header=(None if args.noheader else 0), compression=compression, on_bad_lines=args.on_bad_lines, nrows=(1 if args.op in ('showcols', 'list_columns') else args.nrows), skiprows=args.skiprows)
 
+  if args.clean_coltags: util_pandas.CleanColtags(df)
+    
   if args.op == 'showcols':
     for j,tag in enumerate(df.columns):
       fout.write(f'{j+1}. "{tag}"\n')
 
   elif args.op == 'list_columns':
     fout.write("\n".join(df.columns)+"\n")
 
@@ -86,14 +92,17 @@
   elif args.op == 'summary':
     fout.write(f"rows: {df.shape[0]}; cols: {df.shape[1]}\n")
     fout.write("coltags: {}\n".format(', '.join([f'"{tag}"' for tag in df.columns])))
 
   elif args.op=='csv2tsv':
     df.to_csv(fout, '\t', index=False, header=(not args.noheader))
 
+  elif args.op=='tsv2csv':
+    df.to_csv(fout, ',', index=False, header=(not args.noheader))
+
   elif args.op=='to_html':
     util_pandas.ToHtml(df, args.html_title, args.html_prettify, fout)
 
   elif args.op == 'selectcols':
     logging.info(f"Input: rows: {df.shape[0]}; cols: {df.shape[1]}")
     df = df[coltags] if coltags else df.iloc[:, cols]
     logging.info(f"Output: rows: {df.shape[0]}; cols: {df.shape[1]}")
@@ -157,9 +166,17 @@
   elif args.op == 'pickle':
     if not args.ofile:
       parser.error(f'{args.op} requires --o.')
     fout.close()
     with open(args.ofile, 'wb') as fout:
       pickle.dump(df, fout, pickle.HIGHEST_PROTOCOL)
 
+  elif args.op == 'merge':
+    if not args.ifileB: parser.error(f'{args.op} requires --iB.')
+    if not args.coltags: parser.error(f'{args.op} requires --coltags.')
+    dfB = pd.read_csv(args.ifileB, sep=delim, header=(None if args.noheader else 0), compression=compression, on_bad_lines=args.on_bad_lines, nrows=args.nrows, skiprows=args.skiprows)
+    if args.clean_coltags: util_pandas.CleanColtags(dfB)
+    coltags = [coltag.strip() for coltag in re.split(r',', args.coltags.strip())]
+    util_pandas.Merge(df, dfB, args.merge_how, args.merge_type, coltags, delim, fout)
+
   else:
     parser.error(f'Unknown operation: {args.op}')
```

### Comparing `BioClients-0.2.8/BioClients/util/pandas/Csv2Html.py` & `BioClients-0.2.9/BioClients/util/pandas/Csv2Html.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/pandas/Csv2Markdown.py` & `BioClients-0.2.9/BioClients/util/pandas/Csv2Markdown.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/pandas/Utils.py` & `BioClients-0.2.9/BioClients/util/pandas/Utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 Pandas CSV/TSV utilities.
 """
 ###
 import sys,os,re,logging
 import pandas as pd
 
 #############################################################################
+def CleanColtags(df):
+  oldtags = list(df.columns)[:]
+  newtags=[];
+  for j,tag in enumerate(oldtags):
+    tag = re.sub(r'[\s,;|\\]+', '_', tag.strip())
+    if tag=="": tag = f"Column_{j:02d}"
+    newtags.append(tag)
+  for j in range(len(oldtags)):
+    logging.debug(f"""{j}. "{oldtags[j]}" -> "{newtags[j]}" """)
+  df.columns = newtags
+
+#############################################################################
 def SearchRows(df, cols, coltags, qrys, rels, typs, fout):
   n = df.shape[0]
   for j,tag in enumerate(df.columns):
     if cols:
       if j not in cols: continue
       else: jj = cols.index(j)
     elif coltags:
@@ -64,7 +76,19 @@
     df.round(precision).to_html(fout, index=True, header=True,
 	formatters=None, float_format=None, sparsify=None,
 	bold_rows=True, border=None, justify=None,
 	classes=None, render_links=True,
 	show_dimensions=False)
 
 #############################################################################
+def Merge(dfA, dfB, merge_how, merge_type, coltags, delim, fout):
+  for tag in coltags:
+    dfA[tag] = dfA[tag].astype(merge_type)
+    dfB[tag] = dfB[tag].astype(merge_type)
+  df = dfA.merge(dfB, how=merge_how, on=coltags)
+  df.drop_duplicates(inplace=True)
+  df.to_csv(fout, delim, index=False, header=True)
+  logging.info(f"Rows in A: {dfA.shape[0]}")
+  logging.info(f"Rows in B: {dfB.shape[0]}")
+  logging.info(f"Rows out: {df.shape[0]}")
+
+#############################################################################
```

### Comparing `BioClients-0.2.8/BioClients/util/rdf/App.py` & `BioClients-0.2.9/BioClients/util/rdf/App.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/rdf/Utils.py` & `BioClients-0.2.9/BioClients/util/rdf/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/rest/Utils.py` & `BioClients-0.2.9/BioClients/util/rest/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/sparql/Client.py` & `BioClients-0.2.9/BioClients/util/sparql/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/sparql/Utils.py` & `BioClients-0.2.9/BioClients/util/sparql/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/util/xml/Utils.py` & `BioClients-0.2.9/BioClients/util/xml/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/wikidata/Client.py` & `BioClients-0.2.9/BioClients/wikidata/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/wikidata/Utils.py` & `BioClients-0.2.9/BioClients/wikidata/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/wikipathways/Client.py` & `BioClients-0.2.9/BioClients/wikipathways/Client.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients/wikipathways/Utils.py` & `BioClients-0.2.9/BioClients/wikipathways/Utils.py`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/BioClients.egg-info/PKG-INFO` & `BioClients-0.2.9/BioClients.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: BioClients
-Version: 0.2.8
+Version: 0.2.9
 Summary: Clients to online biomedical resources, usually REST APIs.
 Home-page: https://github.com/jeremyjyang/BioClients
 Author: Jeremy Yang
 Author-email: jeremyjyang@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,42 +36,40 @@
 $ cd BioClients
 $ python3 setup.py install
 ```
 
 ## Dependencies
 
 * Python 3.7+
-* Python packages: `pandas`, `requests`, `urllib`, `json`, `xml`, `yaml`, `psycopg2`,  `tqdm`, etc.
+* Python packages: `pandas`, `requests`, `urllib`, `json`, `xml`, `yaml`, `psycopg2`, `tqdm`, etc.
 
 ## Modules
 
- [__Allen__](doc/allen.md) &#8226; [__AMP-T2D__](doc/amp__t2d.md) &#8226; [__BindingDb__](doc/bindingdb.md) &#8226; [__BioGrid__](doc/biogrid.md) &#8226; [__Bioregistry__](doc/bioregistry.md) &#8226; [__BRENDA__](doc/brenda.md) &#8226; [__CAS__](doc/cas.md) &#8226; [__CDC__](doc/cdc.md) &#8226; [__CFDE__](doc/cfde.md) &#8226; [__Chem2Bio2RDF__](doc/chem2bio2rdf.md) &#8226; [__ChEBI__](doc/chebi.md) &#8226; [__ChEMBL__](doc/chembl.md) &#8226; [__ChemIdPlus__](doc/chemidplus.md) &#8226; [__ClinicalTrials.gov__](doc/clinicaltrials.md) &#8226; [__Disease Ontology__](doc/diseaseontology.md) &#8226;  [__DisGeNet__](doc/disgenet.md) &#8226;  [__DNorm__](doc/dnorm.md) &#8226;  [__DrugCentral__](doc/drugcentral.md) &#8226; [__EMBL-EBI__](doc/emblebi.md) &#8226; [__EnsEMBL__](doc/ensembl.md) &#8226; [__FDA__](doc/fda.md) &#8226;  [__Gene Ontology__](doc/geneontology.md) &#8226;  [__GWAS Catalog__](doc/gwascatalog.md) &#8226;  [__HUGO__](doc/hugo.md) &#8226;  [__HumanBase__](doc/humanbase.md) &#8226;  [__iCite__](doc/icite.md) &#8226;  [__IDG__](doc/idg.md) &#8226; [__JensenLab__](doc/jensenlab.md) &#8226; [__LINCS__](doc/lincs.md) &#8226; [__MaayanLab__](doc/maayanlab.md) &#8226; [__Medline__](doc/medline.md) &#8226; [__MeSH__](doc/mesh.md) &#8226; [__MONARCH__](doc/monarch.md) &#8226; [__MyGene__](doc/mygene.md) &#8226; [__NCBO__](doc/ncbo.md) &#8226;  [__OMIM__](doc/omim.md) &#8226;  [__Open Targets__](doc/opentargets.md) &#8226;  [__Panther__](doc/panther.md) &#8226;  [__PDB__](doc/pdb.md) &#8226;  [__PubChem__](doc/pubchem.md) &#8226;  [__PubMed__](doc/pubmed.md) &#8226;  [__PubTator__](doc/pubtator.md) &#8226;  [__Reactome__](doc/reactome.md) &#8226;  [__RXNorm__](doc/rxnorm.md) &#8226;  [__STRINGDB__](doc/stringdb.md) &#8226; [__TCGA__](doc/tcga.md) &#8226; [__UMLS__](doc/umls.md) &#8226; [__UniProt__](doc/uniprot.md) &#8226; [__Wikidata__](doc/wikidata.md) &#8226; [__WikiPathways__](doc/wikipathways.md) 
+ [__Allen__](doc/allen.md) &#8226; [__AMP-T2D__](doc/amp__t2d.md) &#8226; [__BindingDb__](doc/bindingdb.md) &#8226; [__BioGrid__](doc/biogrid.md) &#8226; [__Bioregistry__](doc/bioregistry.md) &#8226; [__BRENDA__](doc/brenda.md) &#8226; [__CAS__](doc/cas.md) &#8226; [__CDC__](doc/cdc.md) &#8226; [__CFDE__](doc/cfde.md) &#8226; [__Chem2Bio2RDF__](doc/chem2bio2rdf.md) &#8226; [__ChEBI__](doc/chebi.md) &#8226; [__ChEMBL__](doc/chembl.md) &#8226; [__ChemIdPlus__](doc/chemidplus.md) &#8226; [__ClinicalTrials.gov__](doc/clinicaltrials.md) &#8226; [__Disease Ontology__](doc/diseaseontology.md) &#8226; [__DisGeNet__](doc/disgenet.md) &#8226; [__DNorm__](doc/dnorm.md) &#8226; [__DrugCentral__](doc/drugcentral.md) &#8226; [__EMBL-EBI__](doc/emblebi.md) &#8226; [__EnsEMBL__](doc/ensembl.md) &#8226; [__FDA__](doc/fda.md) &#8226; [__Gene Ontology__](doc/geneontology.md) &#8226; [__GWAS Catalog__](doc/gwascatalog.md) &#8226; [__HUGO__](doc/hugo.md) &#8226; [__HumanBase__](doc/humanbase.md) &#8226; [__iCite__](doc/icite.md) &#8226; [__IDG__](doc/idg.md) &#8226; [__JensenLab__](doc/jensenlab.md) &#8226; [__LINCS__](doc/lincs.md) &#8226; [__MaayanLab__](doc/maayanlab.md) &#8226; [__Medline__](doc/medline.md) &#8226; [__MeSH__](doc/mesh.md) &#8226; [__MONARCH__](doc/monarch.md) &#8226; [__MyGene__](doc/mygene.md) &#8226; [__NCBO__](doc/ncbo.md) &#8226; [__NCATS__](doc/ncats.md) &#8226; [__OMIM__](doc/omim.md) &#8226; [__Open Targets__](doc/opentargets.md) &#8226; [__Panther__](doc/panther.md) &#8226; [__PDB__](doc/pdb.md) &#8226; [__PubChem__](doc/pubchem.md) &#8226; [__PubMed__](doc/pubmed.md) &#8226; [__PubTator__](doc/pubtator.md) &#8226; [__Reactome__](doc/reactome.md) &#8226; [__RXNorm__](doc/rxnorm.md) &#8226; [__STRINGDB__](doc/stringdb.md) &#8226; [__TCGA__](doc/tcga.md) &#8226; [__UMLS__](doc/umls.md) &#8226; [__UniProt__](doc/uniprot.md) &#8226; [__Wikidata__](doc/wikidata.md) &#8226; [__WikiPathways__](doc/wikipathways.md) 
 
 Miscellaneous utilities: [__UTIL__](doc/util.md) 
 
 ## Usage Example
 
 ```
 $ python3 -m BioClients.pubchem.Client -h
 ```
 
 ## Design pattern
 
 Generally each module includes command-line app `Client.py` which calls 
 functions in a corresponding `Utils.py`, providing all capabilities
 by import of the module. Command-line apps not API clients are generally 
-named `App.py`.  Functions can write to an output file
+named `App.py`. Functions can write to an output file
 or return a Pandas dataframe (if output file unspecified).
 
 ## Data structures and formats, XML, JSON, and TSV
 
 BioClients is designed to be simple and practical, and XML, JSON
 and TSV are likewise simple in many respects, yet a great deal
 of conceptual and technological progress is reflected. XML and JSON
 can represent arbitrarily complex data objects, comprised of nested lists,
 dictionaries, and trees of primary types. TSV represents tables of
 rows and columns, related by common keys, reflecting the development
 of SQL and relational databases. Transforming JSON to TSV, as these
 clients generally do, projects data objects to tables useful for many
 applications (e.g. machine learning).
-
-
```

### Comparing `BioClients-0.2.8/BioClients.egg-info/SOURCES.txt` & `BioClients-0.2.9/BioClients.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,14 @@
 BioClients/icite/Client.py
 BioClients/icite/Utils.py
 BioClients/icite/__init__.py
 BioClients/idg/Client.py
 BioClients/idg/Utils.py
 BioClients/idg/__init__.py
 BioClients/idg/pharos/Client.py
-BioClients/idg/pharos/ClientGql.py
 BioClients/idg/pharos/Utils.py
 BioClients/idg/pharos/__init__.py
 BioClients/idg/rss/Client.py
 BioClients/idg/rss/Utils.py
 BioClients/idg/rss/__init__.py
 BioClients/idg/tcrd/Client.py
 BioClients/idg/tcrd/Utils.py
@@ -155,14 +154,18 @@
 BioClients/monarch/Biolink.py
 BioClients/monarch/Client.py
 BioClients/monarch/Utils.py
 BioClients/monarch/__init__.py
 BioClients/mygene/Client.py
 BioClients/mygene/Utils.py
 BioClients/mygene/__init__.py
+BioClients/ncats/__init__.py
+BioClients/ncats/gsrs/Client.py
+BioClients/ncats/gsrs/Utils.py
+BioClients/ncats/gsrs/__init__.py
 BioClients/ncbo/Client.py
 BioClients/ncbo/Utils.py
 BioClients/ncbo/__init__.py
 BioClients/omim/Client.py
 BioClients/omim/__init__.py
 BioClients/openphacts/Client.py
 BioClients/openphacts/Utils.py
@@ -235,14 +238,15 @@
 BioClients/util/neo4j/__init__.py
 BioClients/util/obo/App.py
 BioClients/util/obo/Utils.py
 BioClients/util/obo/__init__.py
 BioClients/util/pandas/App.py
 BioClients/util/pandas/Csv2Html.py
 BioClients/util/pandas/Csv2Markdown.py
+BioClients/util/pandas/Csv2Sql.py
 BioClients/util/pandas/Utils.py
 BioClients/util/pandas/__init__.py
 BioClients/util/rdf/App.py
 BioClients/util/rdf/Utils.py
 BioClients/util/rdf/__init__.py
 BioClients/util/rest/Utils.py
 BioClients/util/rest/__init__.py
@@ -259,22 +263,24 @@
 BioClients/wikipathways/Client.py
 BioClients/wikipathways/Utils.py
 BioClients/wikipathways/__init__.py
 doc/allen.md
 doc/amp_t2d.md
 doc/bindingdb.md
 doc/biogrid.md
+doc/bioregistry.md
 doc/brenda.md
 doc/cas.md
 doc/cdc.md
 doc/cfde.md
 doc/chebi.md
 doc/chem2bio2rdf.md
 doc/chembl.md
 doc/chemidplus.md
+doc/clinicaltrials.md
 doc/disgenet.md
 doc/dnorm.md
 doc/drugcentral.md
 doc/emblebi.md
 doc/ensembl.md
 doc/fda.md
 doc/geneontology.md
@@ -288,14 +294,15 @@
 doc/jensenlab.md
 doc/lincs.md
 doc/maayanlab.md
 doc/medline.md
 doc/mesh.md
 doc/monarch.md
 doc/mygene.md
+doc/ncats.md
 doc/ncbo.md
 doc/omim.md
 doc/opentargets.md
 doc/panther.md
 doc/pdb.md
 doc/pubchem.md
 doc/pubmed.md
```

### Comparing `BioClients-0.2.8/LICENSE` & `BioClients-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/PKG-INFO` & `BioClients-0.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: BioClients
-Version: 0.2.8
+Version: 0.2.9
 Summary: Clients to online biomedical resources, usually REST APIs.
 Home-page: https://github.com/jeremyjyang/BioClients
 Author: Jeremy Yang
 Author-email: jeremyjyang@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,42 +36,40 @@
 $ cd BioClients
 $ python3 setup.py install
 ```
 
 ## Dependencies
 
 * Python 3.7+
-* Python packages: `pandas`, `requests`, `urllib`, `json`, `xml`, `yaml`, `psycopg2`,  `tqdm`, etc.
+* Python packages: `pandas`, `requests`, `urllib`, `json`, `xml`, `yaml`, `psycopg2`, `tqdm`, etc.
 
 ## Modules
 
- [__Allen__](doc/allen.md) &#8226; [__AMP-T2D__](doc/amp__t2d.md) &#8226; [__BindingDb__](doc/bindingdb.md) &#8226; [__BioGrid__](doc/biogrid.md) &#8226; [__Bioregistry__](doc/bioregistry.md) &#8226; [__BRENDA__](doc/brenda.md) &#8226; [__CAS__](doc/cas.md) &#8226; [__CDC__](doc/cdc.md) &#8226; [__CFDE__](doc/cfde.md) &#8226; [__Chem2Bio2RDF__](doc/chem2bio2rdf.md) &#8226; [__ChEBI__](doc/chebi.md) &#8226; [__ChEMBL__](doc/chembl.md) &#8226; [__ChemIdPlus__](doc/chemidplus.md) &#8226; [__ClinicalTrials.gov__](doc/clinicaltrials.md) &#8226; [__Disease Ontology__](doc/diseaseontology.md) &#8226;  [__DisGeNet__](doc/disgenet.md) &#8226;  [__DNorm__](doc/dnorm.md) &#8226;  [__DrugCentral__](doc/drugcentral.md) &#8226; [__EMBL-EBI__](doc/emblebi.md) &#8226; [__EnsEMBL__](doc/ensembl.md) &#8226; [__FDA__](doc/fda.md) &#8226;  [__Gene Ontology__](doc/geneontology.md) &#8226;  [__GWAS Catalog__](doc/gwascatalog.md) &#8226;  [__HUGO__](doc/hugo.md) &#8226;  [__HumanBase__](doc/humanbase.md) &#8226;  [__iCite__](doc/icite.md) &#8226;  [__IDG__](doc/idg.md) &#8226; [__JensenLab__](doc/jensenlab.md) &#8226; [__LINCS__](doc/lincs.md) &#8226; [__MaayanLab__](doc/maayanlab.md) &#8226; [__Medline__](doc/medline.md) &#8226; [__MeSH__](doc/mesh.md) &#8226; [__MONARCH__](doc/monarch.md) &#8226; [__MyGene__](doc/mygene.md) &#8226; [__NCBO__](doc/ncbo.md) &#8226;  [__OMIM__](doc/omim.md) &#8226;  [__Open Targets__](doc/opentargets.md) &#8226;  [__Panther__](doc/panther.md) &#8226;  [__PDB__](doc/pdb.md) &#8226;  [__PubChem__](doc/pubchem.md) &#8226;  [__PubMed__](doc/pubmed.md) &#8226;  [__PubTator__](doc/pubtator.md) &#8226;  [__Reactome__](doc/reactome.md) &#8226;  [__RXNorm__](doc/rxnorm.md) &#8226;  [__STRINGDB__](doc/stringdb.md) &#8226; [__TCGA__](doc/tcga.md) &#8226; [__UMLS__](doc/umls.md) &#8226; [__UniProt__](doc/uniprot.md) &#8226; [__Wikidata__](doc/wikidata.md) &#8226; [__WikiPathways__](doc/wikipathways.md) 
+ [__Allen__](doc/allen.md) &#8226; [__AMP-T2D__](doc/amp__t2d.md) &#8226; [__BindingDb__](doc/bindingdb.md) &#8226; [__BioGrid__](doc/biogrid.md) &#8226; [__Bioregistry__](doc/bioregistry.md) &#8226; [__BRENDA__](doc/brenda.md) &#8226; [__CAS__](doc/cas.md) &#8226; [__CDC__](doc/cdc.md) &#8226; [__CFDE__](doc/cfde.md) &#8226; [__Chem2Bio2RDF__](doc/chem2bio2rdf.md) &#8226; [__ChEBI__](doc/chebi.md) &#8226; [__ChEMBL__](doc/chembl.md) &#8226; [__ChemIdPlus__](doc/chemidplus.md) &#8226; [__ClinicalTrials.gov__](doc/clinicaltrials.md) &#8226; [__Disease Ontology__](doc/diseaseontology.md) &#8226; [__DisGeNet__](doc/disgenet.md) &#8226; [__DNorm__](doc/dnorm.md) &#8226; [__DrugCentral__](doc/drugcentral.md) &#8226; [__EMBL-EBI__](doc/emblebi.md) &#8226; [__EnsEMBL__](doc/ensembl.md) &#8226; [__FDA__](doc/fda.md) &#8226; [__Gene Ontology__](doc/geneontology.md) &#8226; [__GWAS Catalog__](doc/gwascatalog.md) &#8226; [__HUGO__](doc/hugo.md) &#8226; [__HumanBase__](doc/humanbase.md) &#8226; [__iCite__](doc/icite.md) &#8226; [__IDG__](doc/idg.md) &#8226; [__JensenLab__](doc/jensenlab.md) &#8226; [__LINCS__](doc/lincs.md) &#8226; [__MaayanLab__](doc/maayanlab.md) &#8226; [__Medline__](doc/medline.md) &#8226; [__MeSH__](doc/mesh.md) &#8226; [__MONARCH__](doc/monarch.md) &#8226; [__MyGene__](doc/mygene.md) &#8226; [__NCBO__](doc/ncbo.md) &#8226; [__NCATS__](doc/ncats.md) &#8226; [__OMIM__](doc/omim.md) &#8226; [__Open Targets__](doc/opentargets.md) &#8226; [__Panther__](doc/panther.md) &#8226; [__PDB__](doc/pdb.md) &#8226; [__PubChem__](doc/pubchem.md) &#8226; [__PubMed__](doc/pubmed.md) &#8226; [__PubTator__](doc/pubtator.md) &#8226; [__Reactome__](doc/reactome.md) &#8226; [__RXNorm__](doc/rxnorm.md) &#8226; [__STRINGDB__](doc/stringdb.md) &#8226; [__TCGA__](doc/tcga.md) &#8226; [__UMLS__](doc/umls.md) &#8226; [__UniProt__](doc/uniprot.md) &#8226; [__Wikidata__](doc/wikidata.md) &#8226; [__WikiPathways__](doc/wikipathways.md) 
 
 Miscellaneous utilities: [__UTIL__](doc/util.md) 
 
 ## Usage Example
 
 ```
 $ python3 -m BioClients.pubchem.Client -h
 ```
 
 ## Design pattern
 
 Generally each module includes command-line app `Client.py` which calls 
 functions in a corresponding `Utils.py`, providing all capabilities
 by import of the module. Command-line apps not API clients are generally 
-named `App.py`.  Functions can write to an output file
+named `App.py`. Functions can write to an output file
 or return a Pandas dataframe (if output file unspecified).
 
 ## Data structures and formats, XML, JSON, and TSV
 
 BioClients is designed to be simple and practical, and XML, JSON
 and TSV are likewise simple in many respects, yet a great deal
 of conceptual and technological progress is reflected. XML and JSON
 can represent arbitrarily complex data objects, comprised of nested lists,
 dictionaries, and trees of primary types. TSV represents tables of
 rows and columns, related by common keys, reflecting the development
 of SQL and relational databases. Transforming JSON to TSV, as these
 clients generally do, projects data objects to tables useful for many
 applications (e.g. machine learning).
-
-
```

### Comparing `BioClients-0.2.8/README.md` & `BioClients-0.2.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -22,34 +22,34 @@
 $ cd BioClients
 $ python3 setup.py install
 ```
 
 ## Dependencies
 
 * Python 3.7+
-* Python packages: `pandas`, `requests`, `urllib`, `json`, `xml`, `yaml`, `psycopg2`,  `tqdm`, etc.
+* Python packages: `pandas`, `requests`, `urllib`, `json`, `xml`, `yaml`, `psycopg2`, `tqdm`, etc.
 
 ## Modules
 
- [__Allen__](doc/allen.md) &#8226; [__AMP-T2D__](doc/amp__t2d.md) &#8226; [__BindingDb__](doc/bindingdb.md) &#8226; [__BioGrid__](doc/biogrid.md) &#8226; [__Bioregistry__](doc/bioregistry.md) &#8226; [__BRENDA__](doc/brenda.md) &#8226; [__CAS__](doc/cas.md) &#8226; [__CDC__](doc/cdc.md) &#8226; [__CFDE__](doc/cfde.md) &#8226; [__Chem2Bio2RDF__](doc/chem2bio2rdf.md) &#8226; [__ChEBI__](doc/chebi.md) &#8226; [__ChEMBL__](doc/chembl.md) &#8226; [__ChemIdPlus__](doc/chemidplus.md) &#8226; [__ClinicalTrials.gov__](doc/clinicaltrials.md) &#8226; [__Disease Ontology__](doc/diseaseontology.md) &#8226;  [__DisGeNet__](doc/disgenet.md) &#8226;  [__DNorm__](doc/dnorm.md) &#8226;  [__DrugCentral__](doc/drugcentral.md) &#8226; [__EMBL-EBI__](doc/emblebi.md) &#8226; [__EnsEMBL__](doc/ensembl.md) &#8226; [__FDA__](doc/fda.md) &#8226;  [__Gene Ontology__](doc/geneontology.md) &#8226;  [__GWAS Catalog__](doc/gwascatalog.md) &#8226;  [__HUGO__](doc/hugo.md) &#8226;  [__HumanBase__](doc/humanbase.md) &#8226;  [__iCite__](doc/icite.md) &#8226;  [__IDG__](doc/idg.md) &#8226; [__JensenLab__](doc/jensenlab.md) &#8226; [__LINCS__](doc/lincs.md) &#8226; [__MaayanLab__](doc/maayanlab.md) &#8226; [__Medline__](doc/medline.md) &#8226; [__MeSH__](doc/mesh.md) &#8226; [__MONARCH__](doc/monarch.md) &#8226; [__MyGene__](doc/mygene.md) &#8226; [__NCBO__](doc/ncbo.md) &#8226;  [__OMIM__](doc/omim.md) &#8226;  [__Open Targets__](doc/opentargets.md) &#8226;  [__Panther__](doc/panther.md) &#8226;  [__PDB__](doc/pdb.md) &#8226;  [__PubChem__](doc/pubchem.md) &#8226;  [__PubMed__](doc/pubmed.md) &#8226;  [__PubTator__](doc/pubtator.md) &#8226;  [__Reactome__](doc/reactome.md) &#8226;  [__RXNorm__](doc/rxnorm.md) &#8226;  [__STRINGDB__](doc/stringdb.md) &#8226; [__TCGA__](doc/tcga.md) &#8226; [__UMLS__](doc/umls.md) &#8226; [__UniProt__](doc/uniprot.md) &#8226; [__Wikidata__](doc/wikidata.md) &#8226; [__WikiPathways__](doc/wikipathways.md) 
+ [__Allen__](doc/allen.md) &#8226; [__AMP-T2D__](doc/amp__t2d.md) &#8226; [__BindingDb__](doc/bindingdb.md) &#8226; [__BioGrid__](doc/biogrid.md) &#8226; [__Bioregistry__](doc/bioregistry.md) &#8226; [__BRENDA__](doc/brenda.md) &#8226; [__CAS__](doc/cas.md) &#8226; [__CDC__](doc/cdc.md) &#8226; [__CFDE__](doc/cfde.md) &#8226; [__Chem2Bio2RDF__](doc/chem2bio2rdf.md) &#8226; [__ChEBI__](doc/chebi.md) &#8226; [__ChEMBL__](doc/chembl.md) &#8226; [__ChemIdPlus__](doc/chemidplus.md) &#8226; [__ClinicalTrials.gov__](doc/clinicaltrials.md) &#8226; [__Disease Ontology__](doc/diseaseontology.md) &#8226; [__DisGeNet__](doc/disgenet.md) &#8226; [__DNorm__](doc/dnorm.md) &#8226; [__DrugCentral__](doc/drugcentral.md) &#8226; [__EMBL-EBI__](doc/emblebi.md) &#8226; [__EnsEMBL__](doc/ensembl.md) &#8226; [__FDA__](doc/fda.md) &#8226; [__Gene Ontology__](doc/geneontology.md) &#8226; [__GWAS Catalog__](doc/gwascatalog.md) &#8226; [__HUGO__](doc/hugo.md) &#8226; [__HumanBase__](doc/humanbase.md) &#8226; [__iCite__](doc/icite.md) &#8226; [__IDG__](doc/idg.md) &#8226; [__JensenLab__](doc/jensenlab.md) &#8226; [__LINCS__](doc/lincs.md) &#8226; [__MaayanLab__](doc/maayanlab.md) &#8226; [__Medline__](doc/medline.md) &#8226; [__MeSH__](doc/mesh.md) &#8226; [__MONARCH__](doc/monarch.md) &#8226; [__MyGene__](doc/mygene.md) &#8226; [__NCBO__](doc/ncbo.md) &#8226; [__NCATS__](doc/ncats.md) &#8226; [__OMIM__](doc/omim.md) &#8226; [__Open Targets__](doc/opentargets.md) &#8226; [__Panther__](doc/panther.md) &#8226; [__PDB__](doc/pdb.md) &#8226; [__PubChem__](doc/pubchem.md) &#8226; [__PubMed__](doc/pubmed.md) &#8226; [__PubTator__](doc/pubtator.md) &#8226; [__Reactome__](doc/reactome.md) &#8226; [__RXNorm__](doc/rxnorm.md) &#8226; [__STRINGDB__](doc/stringdb.md) &#8226; [__TCGA__](doc/tcga.md) &#8226; [__UMLS__](doc/umls.md) &#8226; [__UniProt__](doc/uniprot.md) &#8226; [__Wikidata__](doc/wikidata.md) &#8226; [__WikiPathways__](doc/wikipathways.md) 
 
 Miscellaneous utilities: [__UTIL__](doc/util.md) 
 
 ## Usage Example
 
 ```
 $ python3 -m BioClients.pubchem.Client -h
 ```
 
 ## Design pattern
 
 Generally each module includes command-line app `Client.py` which calls 
 functions in a corresponding `Utils.py`, providing all capabilities
 by import of the module. Command-line apps not API clients are generally 
-named `App.py`.  Functions can write to an output file
+named `App.py`. Functions can write to an output file
 or return a Pandas dataframe (if output file unspecified).
 
 ## Data structures and formats, XML, JSON, and TSV
 
 BioClients is designed to be simple and practical, and XML, JSON
 and TSV are likewise simple in many respects, yet a great deal
 of conceptual and technological progress is reflected. XML and JSON
```

### Comparing `BioClients-0.2.8/doc/cfde.md` & `BioClients-0.2.9/doc/cfde.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/drugcentral.md` & `BioClients-0.2.9/doc/drugcentral.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 
 ## DrugCentral (`drugcentral.org`)
 
 [DrugCentral](https://drugcentral.org) is a widely used research database of
 approved drugs, active pharmaceutical ingredients and clinical products,
 with indications, side effects, molecular mechanism of action targets,
 and much more.  Developed, curated, and maintained by Tudor Oprea, Oleg Ursu,
-Jayme Holmes and coworkers as a key resource for the NIH Illuminating the
+Jayme Holmes, Sorin Avram, and coworkers as a key resource for the NIH Illuminating the
 Druggable Genome (IDG) project.
 
 DrugCentral employs a backend PostgreSql db, freely available at
-<https://drugcentral.org/download>. The BioClients API provides
+<https://drugcentral.org/download>, and containerized via
+[DockerHub](https://hub.docker.com/repository/docker/unmtransinfo/drugcentral_db).
+The BioClients API provides
 programmatic access to an available db instance, which may be deployed
 locally, or may be available publicly with configuration details
-at <https://drugcentral.org> (this service in beta at time of writing, 
-available at: dbhost=unmtid-dbs.net, dbport=5433, dbname=drugcentral,
+at <https://drugcentral.org> (at time of writing:
+dbhost=unmtid-dbs.net, dbport=5433, dbname=drugcentral,
 dbuser=drugman, dbpw=dosage).
 
 Operations include:
 
 * __list_products__ - List all drug products.
 * __list_structures__ - List all drug structures.  
 * __list_structures2smiles__ - List all drug structures as SMILES file.
 * __list_structures2molfile__ - List all drug structures as MDL molfile.
 * __list_active_ingredients__ - List all active ingredients.
 * __list_indications__ - List all indications.
 * __list_xref_types__ - List all xref types.
 * __list_ddis__ - List all drug-drug interactions.
-* __get_structure__ - Get structure by struct_id.
+* __get_structure__ - Get structure by struct\_id.
 * __get_structure_by_synonym__ - Get structure by synonym.
 * __get_structure_by_xref__ - Get structure by xref ID.
 * __get_structure_xrefs__ - Get all xref IDs for structures.
 * __get_structure_products__ - Get all products for structures.
 * __get_structure_atcs__ - Get all ATC classes for structures.
-* __get_product__ - Get product by product_id.
+* __get_product__ - Get product by product\_id.
 * __get_product_structures__ - Get structures for product.
 * __get_indication_structures__ - Get all structures for indication (OMOP ID).
 * __get_drugpage__ - Get drug (structure), with products, xrefs, etc. as JSON.
 * __search_indications__ - Search indications by regular expression.
 * __search_products__ - Search products by regular expression.
 
 All results are TSV format except as noted.
```

### Comparing `BioClients-0.2.8/doc/emblebi.md` & `BioClients-0.2.9/doc/emblebi.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/gwascatalog.md` & `BioClients-0.2.9/doc/gwascatalog.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/idg.md` & `BioClients-0.2.9/doc/idg.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,41 +7,44 @@
 
 # `BioClients.idg.pharos`
 
 Access the Pharos GraphQL API.
 
 ## Dependencies
 
-  * Python package `python-graphql-client`
+  * Python packages `gql`, `python-graphql-client`
 
 ```
 python3 -m BioClients.idg.pharos.Client -h
-usage: Client.py [-h] [--i IFILE] [--ids IDS] [--o OFILE]
-                 [--idtype_target {tcrdid,uniprot,sym}]
-                 [--idtype_disease {cui,doid,name}] [--nmax NMAX]
-                 [--api_endpoint API_ENDPOINT] [-v]
-                 {get_targets,get_diseases,test}
+usage: Client.py [-h] [--i IFILE] [--i_gql IFILE_GQL] [--graphql GRAPHQL] [--ids IDS]
+                 [--o OFILE] [--idtype_target {tcrdid,uniprot,sym}]
+                 [--idtype_disease {cui,doid,name}] [--nmax NMAX] [--api_host API_HOST]
+                 [--api_base_path API_BASE_PATH] [-v]
+                 {get_targets,get_diseases,test,gql_query,gql_demo}
 
 Pharos GraphQL API client
 
 positional arguments:
-  {get_targets,get_diseases,test}
-                        operation
+  {get_targets,get_diseases,test,gql_query,gql_demo}
+                        OPERATION
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --i IFILE             input file, target IDs
+  --i_gql IFILE_GQL     input file, GraphQL
+  --graphql GRAPHQL     input GraphQL
   --ids IDS             IDs, target, comma-separated
   --o OFILE             output (TSV)
   --idtype_target {tcrdid,uniprot,sym}
                         target ID type
   --idtype_disease {cui,doid,name}
                         disease ID type
   --nmax NMAX           max to return
-  --api_endpoint API_ENDPOINT
+  --api_host API_HOST
+  --api_base_path API_BASE_PATH
   -v, --verbose
 ```
 
 # `BioClients.idg.tcrd`
 
 Provides access to the TCRD MySql db.
```

### Comparing `BioClients-0.2.8/doc/images/BioClients_logo.png` & `BioClients-0.2.9/doc/images/BioClients_logo.png`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/medline.md` & `BioClients-0.2.9/doc/medline.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/mesh.md` & `BioClients-0.2.9/doc/mesh.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/opentargets.md` & `BioClients-0.2.9/doc/opentargets.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/pubchem.md` & `BioClients-0.2.9/doc/pubchem.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/pubtator.md` & `BioClients-0.2.9/doc/pubtator.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/reactome.md` & `BioClients-0.2.9/doc/reactome.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/rxnorm.md` & `BioClients-0.2.9/doc/rxnorm.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/stringdb.md` & `BioClients-0.2.9/doc/stringdb.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/umls.md` & `BioClients-0.2.9/doc/umls.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/util.md` & `BioClients-0.2.9/doc/util.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/doc/wikidata.md` & `BioClients-0.2.9/doc/wikidata.md`

 * *Files identical despite different names*

### Comparing `BioClients-0.2.8/setup.py` & `BioClients-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="BioClients",
-    version="0.2.8",
+    version="0.2.9",
     author="Jeremy Yang",
     author_email="jeremyjyang@gmail.com",
     description="Clients to online biomedical resources, usually REST APIs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeremyjyang/BioClients",
     packages=setuptools.find_packages(),
```

