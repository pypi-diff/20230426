# Comparing `tmp/rcsb.db-1.708.tar.gz` & `tmp/rcsb.db-1.709.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.db-1.708.tar", last modified: Thu Apr  6 16:01:12 2023, max compression
+gzip compressed data, was "rcsb.db-1.709.tar", last modified: Wed Apr 26 21:10:27 2023, max compression
```

## Comparing `rcsb.db-1.708.tar` & `rcsb.db-1.709.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.600047 rcsb.db-1.708/
--rw-r--r--   0 vsts      (1001) docker     (122)    29564 2023-04-06 15:42:21.000000 rcsb.db-1.708/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-04-06 15:42:21.000000 rcsb.db-1.708/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-04-06 15:42:21.000000 rcsb.db-1.708/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    27551 2023-04-06 16:01:12.600047 rcsb.db-1.708/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    26823 2023-04-06 15:42:21.000000 rcsb.db-1.708/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.576047 rcsb.db-1.708/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.580047 rcsb.db-1.708/rcsb/db/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.584047 rcsb.db-1.708/rcsb/db/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)     9528 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/cli/ETLExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7657 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/cli/RepoHoldingsEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22767 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/cli/RepoLoadExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10064 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/cli/RepoScanExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11316 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/cli/SchemaUpdateExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8774 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/cli/SequenceClustersEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)      155 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.584047 rcsb.db-1.708/rcsb/db/cockroach/
--rw-r--r--   0 vsts      (1001) docker     (122)     9848 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/cockroach/CockroachDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9605 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/cockroach/CockroachDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5467 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/cockroach/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/cockroach/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.588047 rcsb.db-1.708/rcsb/db/crate/
--rw-r--r--   0 vsts      (1001) docker     (122)     5142 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/crate/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7987 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/crate/CrateDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9990 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/crate/CrateDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/crate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.592047 rcsb.db-1.708/rcsb/db/define/
--rw-r--r--   0 vsts      (1001) docker     (122)    33223 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/define/ContentDefinition.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4169 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/define/DataTypeApiProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15211 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/define/DataTypeApplicationInfo.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4188 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/define/DataTypeInstanceInfo.py
--rw-r--r--   0 vsts      (1001) docker     (122)    34868 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/define/SchemaDefAccess.py
--rw-r--r--   0 vsts      (1001) docker     (122)    60184 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/define/SchemaDefBuild.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/define/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.592047 rcsb.db-1.708/rcsb/db/helpers/
--rw-r--r--   0 vsts      (1001) docker     (122)    16974 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/helpers/ContentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    34236 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/helpers/DocumentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/helpers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1611 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/helpers/r.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.596047 rcsb.db-1.708/rcsb/db/mongo/
--rw-r--r--   0 vsts      (1001) docker     (122)     5655 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mongo/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4938 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mongo/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15040 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mongo/DocumentLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23696 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mongo/MongoDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)    67004 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mongo/PdbxLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mongo/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.596047 rcsb.db-1.708/rcsb/db/mysql/
--rw-r--r--   0 vsts      (1001) docker     (122)     2832 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mysql/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4258 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mysql/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18626 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mysql/MyDbAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12211 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mysql/MyDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5169 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mysql/MysqlSchemaImporter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19129 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mysql/SchemaDefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/mysql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.600047 rcsb.db-1.708/rcsb/db/processors/
--rw-r--r--   0 vsts      (1001) docker     (122)     7467 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/processors/ClusterDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5081 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/processors/DataExchangeStatus.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19485 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/processors/DataTransformFactory.py
--rw-r--r--   0 vsts      (1001) docker     (122)    31322 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/processors/RepoHoldingsDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (122)    40786 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/processors/SchemaDefDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26654 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/processors/SchemaDefReShape.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/processors/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.600047 rcsb.db-1.708/rcsb/db/sql/
--rw-r--r--   0 vsts      (1001) docker     (122)    23627 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/sql/QueryDirectives.py
--rw-r--r--   0 vsts      (1001) docker     (122)    40731 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/sql/SqlGen.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 15:42:21.000000 rcsb.db-1.708/rcsb/db/sql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.600047 rcsb.db-1.708/rcsb/db/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)     2696 2023-04-06 15:42:22.000000 rcsb.db-1.708/rcsb/db/utils/CaseNormalizedDict.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12446 2023-04-06 15:42:22.000000 rcsb.db-1.708/rcsb/db/utils/PdbxSchemaMapReader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3683 2023-04-06 15:42:22.000000 rcsb.db-1.708/rcsb/db/utils/ProvenanceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22110 2023-04-06 15:42:22.000000 rcsb.db-1.708/rcsb/db/utils/SchemaProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1353 2023-04-06 15:42:22.000000 rcsb.db-1.708/rcsb/db/utils/TextUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2172 2023-04-06 15:42:22.000000 rcsb.db-1.708/rcsb/db/utils/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 15:42:22.000000 rcsb.db-1.708/rcsb/db/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1614 2023-04-06 15:42:22.000000 rcsb.db-1.708/rcsb/db/utils/makePathList.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1055 2023-04-06 15:42:22.000000 rcsb.db-1.708/rcsb/db/utils/unescape.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.600047 rcsb.db-1.708/rcsb/db/wf/
--rw-r--r--   0 vsts      (1001) docker     (122)    11213 2023-04-06 15:42:22.000000 rcsb.db-1.708/rcsb/db/wf/RepoLoadWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 15:42:22.000000 rcsb.db-1.708/rcsb/db/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 16:01:12.580047 rcsb.db-1.708/rcsb.db.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    27551 2023-04-06 16:01:12.000000 rcsb.db-1.708/rcsb.db.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     2298 2023-04-06 16:01:12.000000 rcsb.db-1.708/rcsb.db.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-06 16:01:12.000000 rcsb.db-1.708/rcsb.db.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      209 2023-04-06 16:01:12.000000 rcsb.db-1.708/rcsb.db.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-06 15:45:55.000000 rcsb.db-1.708/rcsb.db.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      437 2023-04-06 16:01:12.000000 rcsb.db-1.708/rcsb.db.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-06 16:01:12.000000 rcsb.db-1.708/rcsb.db.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      513 2023-04-06 15:42:22.000000 rcsb.db-1.708/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-04-06 16:01:12.604047 rcsb.db-1.708/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2876 2023-04-06 15:42:22.000000 rcsb.db-1.708/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.259347 rcsb.db-1.709/
+-rw-r--r--   0 vsts      (1001) docker     (122)    29680 2023-04-26 20:49:04.000000 rcsb.db-1.709/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-04-26 20:49:04.000000 rcsb.db-1.709/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-04-26 20:49:04.000000 rcsb.db-1.709/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    27551 2023-04-26 21:10:27.259347 rcsb.db-1.709/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    26823 2023-04-26 20:49:04.000000 rcsb.db-1.709/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.235347 rcsb.db-1.709/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.239347 rcsb.db-1.709/rcsb/db/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.239347 rcsb.db-1.709/rcsb/db/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9528 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/ETLExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7657 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/RepoHoldingsEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22767 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/RepoLoadExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10064 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/RepoScanExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11316 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/SchemaUpdateExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8774 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/SequenceClustersEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      155 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.243347 rcsb.db-1.709/rcsb/db/cockroach/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9848 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cockroach/CockroachDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9605 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cockroach/CockroachDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5467 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cockroach/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cockroach/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.243347 rcsb.db-1.709/rcsb/db/crate/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5142 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/crate/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7987 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/crate/CrateDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9990 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/crate/CrateDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/crate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.247347 rcsb.db-1.709/rcsb/db/define/
+-rw-r--r--   0 vsts      (1001) docker     (122)    33223 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/ContentDefinition.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4169 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/DataTypeApiProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15211 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/DataTypeApplicationInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4188 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/DataTypeInstanceInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    34868 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/SchemaDefAccess.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    60184 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/SchemaDefBuild.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.247347 rcsb.db-1.709/rcsb/db/helpers/
+-rw-r--r--   0 vsts      (1001) docker     (122)    16974 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/helpers/ContentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    34236 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/helpers/DocumentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/helpers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1611 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/helpers/r.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.251347 rcsb.db-1.709/rcsb/db/mongo/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5655 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mongo/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4938 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mongo/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15040 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mongo/DocumentLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23696 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mongo/MongoDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    69158 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mongo/PdbxLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mongo/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.251347 rcsb.db-1.709/rcsb/db/mysql/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2832 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4258 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18626 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/MyDbAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12211 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/MyDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5169 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/MysqlSchemaImporter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19129 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/SchemaDefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.255347 rcsb.db-1.709/rcsb/db/processors/
+-rw-r--r--   0 vsts      (1001) docker     (122)     7467 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/ClusterDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5081 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/DataExchangeStatus.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19485 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/DataTransformFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    31322 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/RepoHoldingsDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    40786 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/SchemaDefDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26654 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/SchemaDefReShape.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.255347 rcsb.db-1.709/rcsb/db/sql/
+-rw-r--r--   0 vsts      (1001) docker     (122)    23627 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/sql/QueryDirectives.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    40731 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/sql/SqlGen.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/sql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.259347 rcsb.db-1.709/rcsb/db/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2696 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/CaseNormalizedDict.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12446 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/PdbxSchemaMapReader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3683 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/ProvenanceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22110 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/SchemaProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1353 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/TextUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2172 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1614 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/makePathList.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1055 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/unescape.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.259347 rcsb.db-1.709/rcsb/db/wf/
+-rw-r--r--   0 vsts      (1001) docker     (122)    11438 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/wf/RepoLoadWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.239347 rcsb.db-1.709/rcsb.db.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    27551 2023-04-26 21:10:27.000000 rcsb.db-1.709/rcsb.db.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2298 2023-04-26 21:10:27.000000 rcsb.db-1.709/rcsb.db.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-26 21:10:27.000000 rcsb.db-1.709/rcsb.db.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      209 2023-04-26 21:10:27.000000 rcsb.db-1.709/rcsb.db.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-26 20:54:12.000000 rcsb.db-1.709/rcsb.db.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      437 2023-04-26 21:10:27.000000 rcsb.db-1.709/rcsb.db.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-26 21:10:27.000000 rcsb.db-1.709/rcsb.db.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      513 2023-04-26 20:49:04.000000 rcsb.db-1.709/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-04-26 21:10:27.259347 rcsb.db-1.709/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2876 2023-04-26 20:49:04.000000 rcsb.db-1.709/setup.py
```

### Comparing `rcsb.db-1.708/HISTORY.txt` & `rcsb.db-1.709/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -339,7 +339,8 @@
  29-Jun-2022  V1.702 Remove unnecessary custom handling of computed-model identifiers (will now use the internally-modified entry.id)
  23-Dec-2022  V1.703 Configuration changes to support tox 4
  26-Jan-2023  V1.704 Update MA_DICT_LOCATOR path in exdb-config-example.yml and add uchar5 to DataTypeApplicationInfo.py
  30-Jan-2023  V1.705 Update requirements (pin SQLAlchemy)
  14-Feb-2023  V1.706 Updates to PdbxLoader and RepoLoadWorkflow to support resumability of core data loading tasks
  22-Feb-2023  V1.707 Updates to PdbxLoader to use case-sensitivity for brute force document purge
  06-Apr-2023  V1.708 Add support for entity_id_list cifType in DataTypeApplicationInfo
+ 26-Apr-2023  V1.709 Fix document pre-purge regex during load, and add regexPurge flag to control running that step
```

### Comparing `rcsb.db-1.708/LICENSE` & `rcsb.db-1.709/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/PKG-INFO` & `rcsb.db-1.709/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.708
+Version: 1.709
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.db-1.708/README.md` & `rcsb.db-1.709/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/cli/ETLExec.py` & `rcsb.db-1.709/rcsb/db/cli/ETLExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/cli/RepoHoldingsEtlWorker.py` & `rcsb.db-1.709/rcsb/db/cli/RepoHoldingsEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/cli/RepoLoadExec.py` & `rcsb.db-1.709/rcsb/db/cli/RepoLoadExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/cli/RepoScanExec.py` & `rcsb.db-1.709/rcsb/db/cli/RepoScanExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/cli/SchemaUpdateExec.py` & `rcsb.db-1.709/rcsb/db/cli/SchemaUpdateExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/cli/SequenceClustersEtlWorker.py` & `rcsb.db-1.709/rcsb/db/cli/SequenceClustersEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/cockroach/CockroachDbLoader.py` & `rcsb.db-1.709/rcsb/db/cockroach/CockroachDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/cockroach/CockroachDbUtil.py` & `rcsb.db-1.709/rcsb/db/cockroach/CockroachDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/cockroach/Connection.py` & `rcsb.db-1.709/rcsb/db/cockroach/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/crate/Connection.py` & `rcsb.db-1.709/rcsb/db/crate/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/crate/CrateDbLoader.py` & `rcsb.db-1.709/rcsb/db/crate/CrateDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/crate/CrateDbUtil.py` & `rcsb.db-1.709/rcsb/db/crate/CrateDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/define/ContentDefinition.py` & `rcsb.db-1.709/rcsb/db/define/ContentDefinition.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/define/DataTypeApiProvider.py` & `rcsb.db-1.709/rcsb/db/define/DataTypeApiProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/define/DataTypeApplicationInfo.py` & `rcsb.db-1.709/rcsb/db/define/DataTypeApplicationInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/define/DataTypeInstanceInfo.py` & `rcsb.db-1.709/rcsb/db/define/DataTypeInstanceInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/define/SchemaDefAccess.py` & `rcsb.db-1.709/rcsb/db/define/SchemaDefAccess.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/define/SchemaDefBuild.py` & `rcsb.db-1.709/rcsb/db/define/SchemaDefBuild.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/helpers/ContentDefinitionHelper.py` & `rcsb.db-1.709/rcsb/db/helpers/ContentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/helpers/DocumentDefinitionHelper.py` & `rcsb.db-1.709/rcsb/db/helpers/DocumentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/helpers/r.py` & `rcsb.db-1.709/rcsb/db/helpers/r.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/mongo/Connection.py` & `rcsb.db-1.709/rcsb/db/mongo/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/mongo/ConnectionBase.py` & `rcsb.db-1.709/rcsb/db/mongo/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/mongo/DocumentLoader.py` & `rcsb.db-1.709/rcsb/db/mongo/DocumentLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/mongo/MongoDbUtil.py` & `rcsb.db-1.709/rcsb/db/mongo/MongoDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/mongo/PdbxLoader.py` & `rcsb.db-1.709/rcsb/db/mongo/PdbxLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 #      6-Aug-2019 jdw  Add schema generation option and move dictionary API instantiation into load() method.
 #     18-May-2020 jdw  Add brute force document purging for loadType=replace
 #     10-Jan-2022 dwp  Add support for loading id code lists for mongo PdbxLoader() (preliminary)
 #     29-Apr-2022 dwp  Add support for handling and making use of internal computed-model identifiers
 #     29-Jun-2022 dwp  Remove uneeded custom-support for computed-model identifiers (will now use the internally-modified entry.id)
 #      2-Feb-2023 dwp  Add removeAndRecreateDbCollections method for wiping a database without involving any data loading
 #     22-Feb-2023 dwp  Use case-sensitivity for brute force document purge
+#     26-Apr-2023 dwp  Fix regex document purge, and add regexPurge flag to control running that step (with default set to skip it)
 #
 ##
 """
 Worker methods for loading primary data content following mapping conventions in external schema definitions.
 
 """
 
@@ -95,14 +96,15 @@
             filterType = optionsD["filterType"]
             readBackCheck = optionsD["readBackCheck"]
             logSize = "logSize" in optionsD and optionsD["logSize"]
             dataSelectors = optionsD["dataSelectors"]
             loadType = optionsD["loadType"]
             databaseName = optionsD["databaseName"]
             pruneDocumentSize = optionsD["pruneDocumentSize"]
+            regexPurge = optionsD["regexPurge"]
             sd = optionsD["schemaDefAccess"]
             dtf = optionsD["dataTransformFactory"]
             collectionNameList = optionsD["collectionNameList"]
             useNameFlag = optionsD["useNameFlag"]
             sdp = SchemaDefDataPrep(schemaDefAccessObj=sd, dtObj=dtf, workPath=workingDir, verbose=self.__verbose)
             # -------------------------------------------
             # -- Create map of  cIdD{ container identifier} =  locatorObj
@@ -122,15 +124,18 @@
             # -- Apply methods to each container -
             for container in containerList:
                 if self.__dmh:
                     self.__dmh.apply(container)
                 else:
                     logger.debug("%s No dynamic method handler for ", procName)
             # -----
-            if loadType != "full":
+            # Perform force purge of existing documents based on regex. Also note that another deletion is performed by deleteList() below (via __loadDocuments)
+            # This is skipped if regexPurge == False (default), since other deletion step is more efficient (based on container identifiers)
+            # Note: might be able to even comment this entire block out, but leaving here temporariliy in case we discover a reason to keep it (DWP 04/2023)
+            if loadType != "full" and regexPurge:
                 for collectionName in collectionNameList:
                     ok = self.__purgeDocuments(databaseName, collectionName, cNameL)
                     logger.debug("%s %s - loadType %r cNameL %r (%r)", databaseName, collectionName, loadType, cNameL, ok)
             # --
             failContainerIdS = set()
             rejectContainerIdS = set()
             # -----
@@ -252,19 +257,24 @@
                 #
         logger.info("%s maximum document size loaded %.4f MB", procName, maxDocumentMegaBytes)
         return True
 
     def __purgeDocuments(self, databaseName, collectionName, cardinalIdL):
         """Purge documents from collection within database with cardinal identifiers in cardinalIdL."""
         try:
+            # Prepare terminating regex pattern based on database and collection for most efficient searching
+            regexEnd = "$"  # ensures pattern won't overmatch other entries (e.g., bird_chem_comp "PRD" won't match "PRD_000306")
+            if databaseName in ["pdbx_core", "pdbx_comp_model_core"] and "core_entry" not in collectionName:
+                regexEnd = "[_.-]"  # captures entities, instances, and assemblies
+            #
             with Connection(cfgOb=self.__cfgOb, resourceName=self.__resourceName) as client:
                 mg = MongoDbUtil(client)
                 for cardId in cardinalIdL:
                     # selectD = {"rcsb_id": "/%s/" % cardId} # this filter did not work
-                    selectD = {"rcsb_id": {"$regex": "^%s" % cardId.upper()}}  # case-sensitive (avoid case-insensitive -- very slow performance)
+                    selectD = {"rcsb_id": {"$regex": f"^{cardId.upper()}{regexEnd}"}}  # case-sensitive (avoid case-insensitive -- very slow performance)
                     dCount = mg.delete(databaseName, collectionName, selectD)
                     logger.debug("Remove %d objects in database %s collection %s selection %r", dCount, databaseName, collectionName, selectD)
             return True
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return False
 
@@ -542,14 +552,15 @@
         inputPathList=None,
         inputIdCodeList=None,
         styleType="rowwise_by_name",
         dataSelectors=None,
         failedFilePath=None,
         saveInputFileListPath=None,
         pruneDocumentSize=None,
+        regexPurge=False,
         logSize=False,
         validationLevel="min",
         mergeContentTypes=None,
         useNameFlag=True,
         updateSchemaOnReplace=True,
         validateFailures=True,
         reloadPartial=True,
@@ -566,14 +577,15 @@
             inputPathList (list, optional): Data file path list (if not provided the full repository will be scanned)
             inputIdCodeList (list, optional): ID Code list (remote discovery mode) (if not provided the full repository will be scanned)
             styleType (str, optional): one of 'rowwise_by_name', 'columnwise_by_name', 'rowwise_no_name', 'rowwise_by_name_with_cardinality'
             dataSelectors (list, optional): selector names defined for this schema (e.g. PUBLIC_RELEASE)
             failedFilePath (str, optional): Path to hold file paths for load failures
             saveInputFileListPath (list, optional): List of files
             pruneDocumentSize (float, optional): iteratively remove large elements from a collection to satisfy size limits
+            regexPurge (bool, optional): perform an additional regex-based round of purging of all pre-existing documents for loadType != "full" (default False)
             logSize (bool, optional): Compute and log bson serialized object size
             validationLevel (str, optional): Completeness of json/bson metadata schema bound to each collection (e.g. 'min', 'full' or None)
             useNameFlag (bool, optional): Use container name as unique identifier otherwise use UID property.
             updateSchemaOnReplace (bool, optional): Update validation schema for loadType == 'replace'
             validateFailures (bool, optional): output validation report on load failures
             reloadPartial (bool, optional): on load failures attempt reload of partial objects.
             providerTypeExclude (str, optional): exclude dictionary method provider by type name. Defaults to None.
@@ -622,14 +634,15 @@
             optD["styleType"] = styleType
             optD["filterType"] = filterType
             optD["readBackCheck"] = self.__readBackCheck
             optD["dataSelectors"] = dataSelectors
             optD["loadType"] = loadType
             optD["logSize"] = logSize
             optD["pruneDocumentSize"] = pruneDocumentSize
+            optD["regexPurge"] = regexPurge
             optD["useNameFlag"] = useNameFlag
             optD["validationLevel"] = validationLevel
             optD["validateFailures"] = validateFailures
             optD["reloadPartial"] = reloadPartial
             # ---------------- - ---------------- - ---------------- - ---------------- - ---------------- -
             #
 
@@ -768,14 +781,15 @@
             filterType = optionsD["filterType"]
             readBackCheck = optionsD["readBackCheck"]
             logSize = "logSize" in optionsD and optionsD["logSize"]
             dataSelectors = optionsD["dataSelectors"]
             loadType = optionsD["loadType"]
             databaseName = optionsD["databaseName"]
             pruneDocumentSize = optionsD["pruneDocumentSize"]
+            regexPurge = optionsD["regexPurge"]
             sd = optionsD["schemaDefAccess"]
             dtf = optionsD["dataTransformFactory"]
             collectionNameList = optionsD["collectionNameList"]
             useNameFlag = optionsD["useNameFlag"]
             validationLevel = optionsD["validationLevel"]
             validateFailures = optionsD["validateFailures"]
             reloadPartial = optionsD["reloadPartial"]
@@ -801,15 +815,17 @@
             for container in containerList:
                 if self.__dmh:
                     self.__dmh.apply(container)
                 else:
                     logger.debug("%s No dynamic method handler for ", procName)
             # -----
             # Perform force purge of existing documents based on regex. Also note that another deletion is performed by deleteList() below (via __loadDocuments)
-            if loadType != "full":
+            # This is skipped if regexPurge == False (default), since other deletion step is more efficient (based on container identifiers)
+            # Note: might be able to even comment this entire block out, but leaving here temporariliy in case we discover a reason to keep it (DWP 04/2023)
+            if loadType != "full" and regexPurge:
                 for collectionName in collectionNameList:
                     logger.debug("Purging objects from %s for %d containers", collectionName, len(cNameL))
                     ok = self.__purgeDocuments(databaseName, collectionName, cNameL)
                     logger.debug("%s %s - loadType %r cNameL %r (%r)", databaseName, collectionName, loadType, cNameL, ok)
                     # --
             # -----
             failContainerIdS = set()
@@ -1147,18 +1163,23 @@
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return False
 
     def __purgeDocuments(self, databaseName, collectionName, cardinalIdL):
         """Purge documents from collection within database with cardinal identifiers in cardinalIdL."""
         try:
+            # Prepare terminating regex pattern based on database and collection for most efficient searching
+            regexEnd = "$"  # ensures pattern won't overmatch other entries (e.g., bird_chem_comp "PRD" won't match "PRD_000306")
+            if databaseName in ["pdbx_core", "pdbx_comp_model_core"] and "core_entry" not in collectionName:
+                regexEnd = "[_.-]"  # captures entities, instances, and assemblies
+            #
             with Connection(cfgOb=self.__cfgOb, resourceName=self.__resourceName) as client:
                 mg = MongoDbUtil(client)
                 for cardId in cardinalIdL:
-                    selectD = {"rcsb_id": {"$regex": "^%s" % cardId.upper()}}  # case-sensitive (avoid case-insensitive -- very slow performance)
+                    selectD = {"rcsb_id": {"$regex": f"^{cardId.upper()}{regexEnd}"}}  # case-sensitive (avoid case-insensitive -- very slow performance)
                     dCount = mg.delete(databaseName, collectionName, selectD)
                     logger.debug("Remove %d objects in database %s collection %s selection %r", dCount, databaseName, collectionName, selectD)
             return True
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return False
```

### Comparing `rcsb.db-1.708/rcsb/db/mysql/Connection.py` & `rcsb.db-1.709/rcsb/db/mysql/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/mysql/ConnectionBase.py` & `rcsb.db-1.709/rcsb/db/mysql/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/mysql/MyDbAdapter.py` & `rcsb.db-1.709/rcsb/db/mysql/MyDbAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/mysql/MyDbUtil.py` & `rcsb.db-1.709/rcsb/db/mysql/MyDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/mysql/MysqlSchemaImporter.py` & `rcsb.db-1.709/rcsb/db/mysql/MysqlSchemaImporter.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/mysql/SchemaDefLoader.py` & `rcsb.db-1.709/rcsb/db/mysql/SchemaDefLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/processors/ClusterDataPrep.py` & `rcsb.db-1.709/rcsb/db/processors/ClusterDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/processors/DataExchangeStatus.py` & `rcsb.db-1.709/rcsb/db/processors/DataExchangeStatus.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/processors/DataTransformFactory.py` & `rcsb.db-1.709/rcsb/db/processors/DataTransformFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/processors/RepoHoldingsDataPrep.py` & `rcsb.db-1.709/rcsb/db/processors/RepoHoldingsDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py` & `rcsb.db-1.709/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/processors/SchemaDefDataPrep.py` & `rcsb.db-1.709/rcsb/db/processors/SchemaDefDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/processors/SchemaDefReShape.py` & `rcsb.db-1.709/rcsb/db/processors/SchemaDefReShape.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/sql/QueryDirectives.py` & `rcsb.db-1.709/rcsb/db/sql/QueryDirectives.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/sql/SqlGen.py` & `rcsb.db-1.709/rcsb/db/sql/SqlGen.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/utils/CaseNormalizedDict.py` & `rcsb.db-1.709/rcsb/db/utils/CaseNormalizedDict.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/utils/PdbxSchemaMapReader.py` & `rcsb.db-1.709/rcsb/db/utils/PdbxSchemaMapReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/utils/ProvenanceProvider.py` & `rcsb.db-1.709/rcsb/db/utils/ProvenanceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/utils/SchemaProvider.py` & `rcsb.db-1.709/rcsb/db/utils/SchemaProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/utils/TextUtil.py` & `rcsb.db-1.709/rcsb/db/utils/TextUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/utils/TimeUtil.py` & `rcsb.db-1.709/rcsb/db/utils/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/utils/makePathList.py` & `rcsb.db-1.709/rcsb/db/utils/makePathList.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/utils/unescape.py` & `rcsb.db-1.709/rcsb/db/utils/unescape.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/rcsb/db/wf/RepoLoadWorkflow.py` & `rcsb.db-1.709/rcsb/db/wf/RepoLoadWorkflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 #  Workflow wrapper  --  repository database loading utilities --
 #
 #  Updates:
 #   1-Jun-2022 dwp Add clusterFileNameTemplate to load method kwargs
 #   2-Feb-2023 dwp Add removeAndRecreateDbCollections method for wiping a database without involving any data loading;
 #                  Add support for inputIdCodeList
+#  26-Apr-2023 dwp Add regexPurge flag to control running regexp purge step during document load (with default set to False)
 #
 ##
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
 
@@ -68,14 +69,15 @@
             loadFileListPath = kwargs.get("loadFileListPath", None)
             inputIdCodeList = kwargs.get("inputIdCodeList", None)
             saveInputFileListPath = kwargs.get("saveFileListPath", None)
             schemaLevel = kwargs.get("schemaLevel", "min") if kwargs.get("schemaLevel") in ["min", "full"] else "min"
             loadType = kwargs.get("loadType", "full")  # or replace
             updateSchemaOnReplace = kwargs.get("updateSchemaOnReplace", True)
             pruneDocumentSize = float(kwargs.get("pruneDocumentSize")) if "pruneDocumentSize" in kwargs else None
+            regexPurge = kwargs.get("regexPurge", False)
             clusterFileNameTemplate = kwargs.get("clusterFileNameTemplate", None)
 
             # "Document organization (rowwise_by_name_with_cardinality|rowwise_by_name|columnwise_by_name|rowwise_by_id|rowwise_no_name",
             documentStyle = kwargs.get("documentStyle", "rowwise_by_name_with_cardinality")
             dbType = kwargs.get("dbType", "mongo")
             #
             databaseName = kwargs.get("databaseName", None)
@@ -125,14 +127,15 @@
                     inputPathList=inputPathList,
                     inputIdCodeList=inputIdCodeList,
                     styleType=documentStyle,
                     dataSelectors=["PUBLIC_RELEASE"],
                     failedFilePath=failedFilePath,
                     saveInputFileListPath=saveInputFileListPath,
                     pruneDocumentSize=pruneDocumentSize,
+                    regexPurge=regexPurge,
                     validationLevel=schemaLevel,
                     mergeContentTypes=["vrpt"] if mergeValidationReports else None,
                     updateSchemaOnReplace=updateSchemaOnReplace,
                 )
                 okS = self.loadStatus(mw.getLoadStatus(), readBackCheck=readBackCheck)
             except Exception as e:
                 logger.exception("Operation %r database %r failing with %s", op, databaseName, str(e))
```

### Comparing `rcsb.db-1.708/rcsb.db.egg-info/PKG-INFO` & `rcsb.db-1.709/rcsb.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.708
+Version: 1.709
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.db-1.708/rcsb.db.egg-info/SOURCES.txt` & `rcsb.db-1.709/rcsb.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/requirements.txt` & `rcsb.db-1.709/requirements.txt`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.708/setup.py` & `rcsb.db-1.709/setup.py`

 * *Files identical despite different names*

