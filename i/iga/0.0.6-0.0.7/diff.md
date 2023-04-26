# Comparing `tmp/iga-0.0.6.tar.gz` & `tmp/iga-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iga-0.0.6.tar", last modified: Thu Apr 20 01:00:51 2023, max compression
+gzip compressed data, was "iga-0.0.7.tar", last modified: Tue Apr 25 22:37:13 2023, max compression
```

## Comparing `iga-0.0.6.tar` & `iga-0.0.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-20 01:00:51.687296 iga-0.0.6/
--rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-0.0.6/LICENSE
--rw-r--r--   0 mhucka     (503) staff       (20)    25734 2023-04-20 01:00:51.687407 iga-0.0.6/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)    24828 2023-04-20 00:49:26.000000 iga-0.0.6/README.md
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-20 01:00:51.656158 iga-0.0.6/iga/
--rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-04-20 01:00:03.000000 iga-0.0.6/iga/__init__.py
--rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-0.0.6/iga/__main__.py
--rw-r--r--   0 mhucka     (503) staff       (20)    31130 2023-04-10 21:10:55.000000 iga-0.0.6/iga/cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-0.0.6/iga/data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-04-10 21:11:51.000000 iga-0.0.6/iga/doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1069 2023-04-07 18:13:39.000000 iga-0.0.6/iga/exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1447 2023-03-28 00:40:16.000000 iga-0.0.6/iga/exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)    15031 2023-04-20 00:58:38.000000 iga-0.0.6/iga/github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3192 2023-03-28 22:54:00.000000 iga-0.0.6/iga/id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)    14934 2023-04-10 21:13:20.000000 iga-0.0.6/iga/invenio.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2058 2023-04-20 00:58:38.000000 iga-0.0.6/iga/json_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-0.0.6/iga/licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    69392 2023-04-20 00:58:38.000000 iga-0.0.6/iga/metadata.py
--rw-r--r--   0 mhucka     (503) staff       (20)    14559 2023-04-20 00:58:38.000000 iga-0.0.6/iga/name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-0.0.6/iga/orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-0.0.6/iga/reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-0.0.6/iga/ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-0.0.6/iga/text_utils.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-20 01:00:51.670452 iga-0.0.6/iga.egg-info/
--rw-r--r--   0 mhucka     (503) staff       (20)    25734 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/requires.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-04-20 01:00:51.000000 iga-0.0.6/iga.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-04-20 01:00:51.687837 iga-0.0.6/setup.cfg
--rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-0.0.6/setup.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-20 01:00:51.687134 iga-0.0.6/tests/
--rw-r--r--   0 mhucka     (503) staff       (20)     5732 2023-04-20 00:58:38.000000 iga-0.0.6/tests/test_cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-0.0.6/tests/test_data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-0.0.6/tests/test_doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-0.0.6/tests/test_exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-0.0.6/tests/test_exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-0.0.6/tests/test_github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-0.0.6/tests/test_github_mocks.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2149 2023-03-02 15:19:42.000000 iga-0.0.6/tests/test_id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-0.0.6/tests/test_init.py
--rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-04-20 00:58:38.000000 iga-0.0.6/tests/test_is_person.py
--rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-0.0.6/tests/test_licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-04-20 00:58:38.000000 iga-0.0.6/tests/test_name_splitting.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-04-20 00:58:38.000000 iga-0.0.6/tests/test_name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-0.0.6/tests/test_orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1935 2023-04-08 01:31:14.000000 iga-0.0.6/tests/test_record_from_codemeta.py
--rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-0.0.6/tests/test_reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-0.0.6/tests/test_ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-0.0.6/tests/test_text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-25 22:37:13.961297 iga-0.0.7/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-0.0.7/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    27009 2023-04-25 22:37:13.961392 iga-0.0.7/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    26103 2023-04-25 22:30:46.000000 iga-0.0.7/README.md
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-25 22:37:13.957922 iga-0.0.7/iga/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-04-25 22:35:25.000000 iga-0.0.7/iga/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-0.0.7/iga/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    32559 2023-04-25 22:30:46.000000 iga-0.0.7/iga/cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-0.0.7/iga/data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-04-10 21:11:51.000000 iga-0.0.7/iga/doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1179 2023-04-25 22:30:46.000000 iga-0.0.7/iga/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1447 2023-03-28 00:40:16.000000 iga-0.0.7/iga/exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15031 2023-04-20 00:58:38.000000 iga-0.0.7/iga/github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4887 2023-04-25 22:30:46.000000 iga-0.0.7/iga/id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    16908 2023-04-25 22:30:46.000000 iga-0.0.7/iga/invenio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2058 2023-04-20 00:58:38.000000 iga-0.0.7/iga/json_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-0.0.7/iga/licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    69392 2023-04-20 00:58:38.000000 iga-0.0.7/iga/metadata.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14559 2023-04-20 00:58:38.000000 iga-0.0.7/iga/name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-0.0.7/iga/orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-0.0.7/iga/reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-0.0.7/iga/ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-0.0.7/iga/text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-25 22:37:13.958894 iga-0.0.7/iga.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    27009 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-04-25 22:37:13.961714 iga-0.0.7/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-0.0.7/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-25 22:37:13.961186 iga-0.0.7/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     5734 2023-04-25 22:30:46.000000 iga-0.0.7/tests/test_cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-0.0.7/tests/test_data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-0.0.7/tests/test_doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-0.0.7/tests/test_exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-0.0.7/tests/test_exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-0.0.7/tests/test_github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-0.0.7/tests/test_github_mocks.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2551 2023-04-25 22:30:46.000000 iga-0.0.7/tests/test_id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-0.0.7/tests/test_init.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-04-20 00:58:38.000000 iga-0.0.7/tests/test_is_person.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-0.0.7/tests/test_licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-04-20 00:58:38.000000 iga-0.0.7/tests/test_name_splitting.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-04-20 00:58:38.000000 iga-0.0.7/tests/test_name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-0.0.7/tests/test_orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1935 2023-04-08 01:31:14.000000 iga-0.0.7/tests/test_record_from_codemeta.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-0.0.7/tests/test_reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-0.0.7/tests/test_ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-0.0.7/tests/test_text_utils.py
```

### Comparing `iga-0.0.6/LICENSE` & `iga-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/PKG-INFO` & `iga-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 0.0.6
+Version: 0.0.7
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -141,15 +141,15 @@
 ```
 Note that when using this form of the command, the release tag (`v1.2.0` above) must be the last item given on the command line.
 
 ### Use of a GitHub access token
 
 It is possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for many repositories, IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
 
-### Construction of an InvenioRDM record
+### Gathering metadata for an InvenioRDM record
 
 The record created in InvenioRDM is constructed using information obtained using GitHub's API as well as several other APIs as needed. The information includes the following:
  * (if one exists) a `codemeta.json` file in the GitHub repository
  * (if one exists) a `CITATION.cff` file in the GitHub repository
  * data available from GitHub for the release
  * data available from GitHub for the repository
  * data available from GitHub for the account of the owner
@@ -158,35 +158,42 @@
  * data available from ORCID.org for ORCID identifiers
  * data available from ROR.org for Research Organization Registry identifiers
  * data available from DOI.org, NCBI, Google Books, & others for publications
  * data available from spdx.org for software licenses
 
 IGA tries to use `CodeMeta.json` first and `CITATION.cff` second to fill out the fields of the InvenioRDM record. If neither of those files are present, IGA uses values from the GitHub repository instead. You can make it always use all sources of info with the option `--all-metadata`. Depending on how complete and up-to-date your `CodeMeta.json` and `CITATION.cff` are, this may or may not make the record more comprehensive and may or may not introduce redundancies or unwanted values.
 
-To override the auto-created record, use the option `--read-record` followed by the path to a JSON file structured according to the InvenioRDM schema used by the destination server. When `--read-record` is provided, IGA does _not_ extract the data above, but still obtains the file assets from GitHub.
+To override the auto-created metadata, use the option `--read-metadata` followed by the path to a JSON file structured according to the InvenioRDM schema used by the destination server. When `--read-metadata` is provided, IGA does _not_ extract the data above, but still obtains the file assets from GitHub.
 
 ### Specification of GitHub file assets
 
 By default, IGA attaches to the InvenioRDM record _only_ the ZIP file asset created by GitHub for the release. To make IGA attach all assets associated with the GitHub release, use the option `--all-assets`.
 
 To upload specific file assets and override the default selections made by IGA, you can use the option `--file` followed by a path to a file to be uploaded.  You can repeat the option `--file` to upload multiple file assets. Note that if `--file` is provided, then IGA _does not use any file assets from GitHub_; it is the user's responsibility to supply all the files that should be uploaded.
 
-If both `--read-record` and `--file` are used, then IGA does not actually contact GitHub for any information.
+If both `--read-metadata` and `--file` are used, then IGA does not actually contact GitHub for any information.
 
 ### Handling communities
 
 To submit your record to a community, use the `--community` option together with a community name. The option `--list-communities` can be used to get a list of communities supported by the InvenioRDM server. Note that submitting a record to a community means that the record will not be finalized and will not be publicly visible when IGA finishes; instead, the record URL that you receive will be for a draft version, pending review by the community moderators.
 
 ### Draft versus published records
 
 If the `--community` option is not used, then by default, IGA will finalize and publish the record. To make it stop short and leave the record as a draft instead, use the option `--draft`. The draft option also takes precedence over the community option: if you use both `--draft` and `--community`, IGA will stop after creating the draft record and will _not_ submit it to the community.  (You can nevertheless submit the record to a community manually once the draft is created, by visiting the record's web page and using the InvenioRDM interface there.)
 
+### Versioning of records
+
+The option `--parent-record` can be used to indicate that the record being constructed is a new version of an existing record. This will make IGA use the InvenioRDM API for [record versioning](https://inveniordm.docs.cern.ch/releases/versions/version-v2.0.0/#versioning-support). The newly-created record will be linked to a parent record identified by the value passed to `--parent-record`. The value must be either an InvenioRDM record identifier (which is a sequence of alphanumeric characters of the form _XXXXX-XXXXX_, such as `bknz4-bch35`, generated by the InvenioRDM server), or a URL to the landing page of the record in the InvenioRDM server. (Note that such URLs end in the record identifier.) Here is an example of using this option:
+```
+iga --parent-record xbcd4-efgh5 https://github.com/mhucka/taupe/releases/tag/v1.2.0
+```
+
 ### Other options recognized by IGA
 
-Running IGA with the option `--save-record` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-record` to save a record to a file, edit the result, then finally run IGA with the `--read-record` option to use the modified record to create a release in the InvenioRDM server.
+Running IGA with the option `--save-metadata` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-metadata` to save a record to a file, edit the result, then finally run IGA with the `--read-metadata` option to use the modified record to create a release in the InvenioRDM server.
 
 The `--mode` option can be used to change the run mode. Four run modes are available: `quiet`, `normal`, `verbose`, and `debug`. The default mode is `normal`, in which IGA prints a few messages while it's working. The mode `quiet` will make it avoid printing anything unless an error occurs, the mode `verbose` will make it print a detailed trace of what it is doing, and the mode `debug` will make IGA even more verbose. In addition, in `debug` mode, IGA will drop into the `pdb` debugger if it encounters an exception during execution. On Linux and macOS, debug mode also installs a signal handler on signal USR1 that causes IGA to drop into the `pdb` debugger if the signal USR1 is received. (Use `kill -USR1 NNN`, where NNN is the IGA process id.)
 
 Networks latencies are unpredicatable. Reading and writing large files may take a long time; on the other hand, IGA should not wait forever before reporting an error if a server or network becomes unresponsive. To balance these conflicting needs, IGA automatically scales its network timeout based on file sizes. To override its adaptive algorithm and set an explicit timeout value, use the option `--timeout` with a value in seconds.
 
 By default, the output of the `verbose` and `debug` run modes is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` to indicate console output, or a file path to send the output to the file.
 
@@ -211,23 +218,25 @@
 | `--github-token` _T_   | `-t` _T_ | Use GitHub acccess token _T_| Use value in env. var. `GITHUB_TOKEN` | |
 | `--help`               | `-h`     | Print help info and exit | | |
 | `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
 | `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
-| `--open`               | `-O`     | Open record's RDM web page in a browser when done | Do nothing when done | |
-| `--read-record` _R_    | `-R` _R_ | Read metadata record from _R_; don\'t build one | Build metadata record | |
-| `--save-record` _D_    | `-S` _D_ | Save metadata record to _D_; don\'t upload it | Upload to InvenioRDM server | |
+| `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
+| `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
+| `--read-metadata` _R_  | `-R` _R_ | Read metadata record from file _R_; don\'t build one | Build metadata record | |
+| `--save-metadata` _D_  | `-S` _D_ | Save metadata record to file _D_; don\'t upload it | Upload to InvenioRDM server | |
 | `--timeout` _X_        | `-T` _X_ | Wait on network operations a max of _X_ seconds | Auto-adjusted based on file size | |
 | `--version`            | `-V`     | Print program version info and exit | | |
 
-⚑ &nbsp; Can repeat for multiple files.<br>
+⚑ &nbsp; Can repeat the option to specify multiple files.<br>
 ⚐ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.<br>
-✯ &nbsp; When using `--github-account` and `--github-repo`, the last argument on the command line must be a release tag name.
+✯ &nbsp; When using `--github-account` and `--github-repo`, the last argument on the command line must be a release tag name.<br>
+❖ &nbsp; The record identifier must be given either as a sequence of alphanumeric characters of the form _XXXXX-XXXXX_ (e.g., `bknz4-bch35`), or as a URL to the landing page of an existing record in the InvenioRDM server.
 
 ### Return values
 
 This program exits with a return status code of 0 if no problem is encountered.  Otherwise, it returns a nonzero status code. The following table lists the possible values:
 
 | Code | Meaning                                                  |
 |:----:|----------------------------------------------------------|
```

### Comparing `iga-0.0.6/README.md` & `iga-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 ```
 Note that when using this form of the command, the release tag (`v1.2.0` above) must be the last item given on the command line.
 
 ### Use of a GitHub access token
 
 It is possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for many repositories, IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
 
-### Construction of an InvenioRDM record
+### Gathering metadata for an InvenioRDM record
 
 The record created in InvenioRDM is constructed using information obtained using GitHub's API as well as several other APIs as needed. The information includes the following:
  * (if one exists) a `codemeta.json` file in the GitHub repository
  * (if one exists) a `CITATION.cff` file in the GitHub repository
  * data available from GitHub for the release
  * data available from GitHub for the repository
  * data available from GitHub for the account of the owner
@@ -134,35 +134,42 @@
  * data available from ORCID.org for ORCID identifiers
  * data available from ROR.org for Research Organization Registry identifiers
  * data available from DOI.org, NCBI, Google Books, & others for publications
  * data available from spdx.org for software licenses
 
 IGA tries to use `CodeMeta.json` first and `CITATION.cff` second to fill out the fields of the InvenioRDM record. If neither of those files are present, IGA uses values from the GitHub repository instead. You can make it always use all sources of info with the option `--all-metadata`. Depending on how complete and up-to-date your `CodeMeta.json` and `CITATION.cff` are, this may or may not make the record more comprehensive and may or may not introduce redundancies or unwanted values.
 
-To override the auto-created record, use the option `--read-record` followed by the path to a JSON file structured according to the InvenioRDM schema used by the destination server. When `--read-record` is provided, IGA does _not_ extract the data above, but still obtains the file assets from GitHub.
+To override the auto-created metadata, use the option `--read-metadata` followed by the path to a JSON file structured according to the InvenioRDM schema used by the destination server. When `--read-metadata` is provided, IGA does _not_ extract the data above, but still obtains the file assets from GitHub.
 
 ### Specification of GitHub file assets
 
 By default, IGA attaches to the InvenioRDM record _only_ the ZIP file asset created by GitHub for the release. To make IGA attach all assets associated with the GitHub release, use the option `--all-assets`.
 
 To upload specific file assets and override the default selections made by IGA, you can use the option `--file` followed by a path to a file to be uploaded.  You can repeat the option `--file` to upload multiple file assets. Note that if `--file` is provided, then IGA _does not use any file assets from GitHub_; it is the user's responsibility to supply all the files that should be uploaded.
 
-If both `--read-record` and `--file` are used, then IGA does not actually contact GitHub for any information.
+If both `--read-metadata` and `--file` are used, then IGA does not actually contact GitHub for any information.
 
 ### Handling communities
 
 To submit your record to a community, use the `--community` option together with a community name. The option `--list-communities` can be used to get a list of communities supported by the InvenioRDM server. Note that submitting a record to a community means that the record will not be finalized and will not be publicly visible when IGA finishes; instead, the record URL that you receive will be for a draft version, pending review by the community moderators.
 
 ### Draft versus published records
 
 If the `--community` option is not used, then by default, IGA will finalize and publish the record. To make it stop short and leave the record as a draft instead, use the option `--draft`. The draft option also takes precedence over the community option: if you use both `--draft` and `--community`, IGA will stop after creating the draft record and will _not_ submit it to the community.  (You can nevertheless submit the record to a community manually once the draft is created, by visiting the record's web page and using the InvenioRDM interface there.)
 
+### Versioning of records
+
+The option `--parent-record` can be used to indicate that the record being constructed is a new version of an existing record. This will make IGA use the InvenioRDM API for [record versioning](https://inveniordm.docs.cern.ch/releases/versions/version-v2.0.0/#versioning-support). The newly-created record will be linked to a parent record identified by the value passed to `--parent-record`. The value must be either an InvenioRDM record identifier (which is a sequence of alphanumeric characters of the form _XXXXX-XXXXX_, such as `bknz4-bch35`, generated by the InvenioRDM server), or a URL to the landing page of the record in the InvenioRDM server. (Note that such URLs end in the record identifier.) Here is an example of using this option:
+```
+iga --parent-record xbcd4-efgh5 https://github.com/mhucka/taupe/releases/tag/v1.2.0
+```
+
 ### Other options recognized by IGA
 
-Running IGA with the option `--save-record` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-record` to save a record to a file, edit the result, then finally run IGA with the `--read-record` option to use the modified record to create a release in the InvenioRDM server.
+Running IGA with the option `--save-metadata` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-metadata` to save a record to a file, edit the result, then finally run IGA with the `--read-metadata` option to use the modified record to create a release in the InvenioRDM server.
 
 The `--mode` option can be used to change the run mode. Four run modes are available: `quiet`, `normal`, `verbose`, and `debug`. The default mode is `normal`, in which IGA prints a few messages while it's working. The mode `quiet` will make it avoid printing anything unless an error occurs, the mode `verbose` will make it print a detailed trace of what it is doing, and the mode `debug` will make IGA even more verbose. In addition, in `debug` mode, IGA will drop into the `pdb` debugger if it encounters an exception during execution. On Linux and macOS, debug mode also installs a signal handler on signal USR1 that causes IGA to drop into the `pdb` debugger if the signal USR1 is received. (Use `kill -USR1 NNN`, where NNN is the IGA process id.)
 
 Networks latencies are unpredicatable. Reading and writing large files may take a long time; on the other hand, IGA should not wait forever before reporting an error if a server or network becomes unresponsive. To balance these conflicting needs, IGA automatically scales its network timeout based on file sizes. To override its adaptive algorithm and set an explicit timeout value, use the option `--timeout` with a value in seconds.
 
 By default, the output of the `verbose` and `debug` run modes is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` to indicate console output, or a file path to send the output to the file.
 
@@ -187,23 +194,25 @@
 | `--github-token` _T_   | `-t` _T_ | Use GitHub acccess token _T_| Use value in env. var. `GITHUB_TOKEN` | |
 | `--help`               | `-h`     | Print help info and exit | | |
 | `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
 | `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
-| `--open`               | `-O`     | Open record's RDM web page in a browser when done | Do nothing when done | |
-| `--read-record` _R_    | `-R` _R_ | Read metadata record from _R_; don\'t build one | Build metadata record | |
-| `--save-record` _D_    | `-S` _D_ | Save metadata record to _D_; don\'t upload it | Upload to InvenioRDM server | |
+| `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
+| `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
+| `--read-metadata` _R_  | `-R` _R_ | Read metadata record from file _R_; don\'t build one | Build metadata record | |
+| `--save-metadata` _D_  | `-S` _D_ | Save metadata record to file _D_; don\'t upload it | Upload to InvenioRDM server | |
 | `--timeout` _X_        | `-T` _X_ | Wait on network operations a max of _X_ seconds | Auto-adjusted based on file size | |
 | `--version`            | `-V`     | Print program version info and exit | | |
 
-⚑ &nbsp; Can repeat for multiple files.<br>
+⚑ &nbsp; Can repeat the option to specify multiple files.<br>
 ⚐ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.<br>
-✯ &nbsp; When using `--github-account` and `--github-repo`, the last argument on the command line must be a release tag name.
+✯ &nbsp; When using `--github-account` and `--github-repo`, the last argument on the command line must be a release tag name.<br>
+❖ &nbsp; The record identifier must be given either as a sequence of alphanumeric characters of the form _XXXXX-XXXXX_ (e.g., `bknz4-bch35`), or as a URL to the landing page of an existing record in the InvenioRDM server.
 
 ### Return values
 
 This program exits with a return status code of 0 if no problem is encountered.  Otherwise, it returns a nonzero status code. The following table lists the possible values:
 
 | Code | Meaning                                                  |
 |:----:|----------------------------------------------------------|
```

### Comparing `iga-0.0.6/iga/__init__.py` & `iga-0.0.7/iga/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # .............................................................................
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '0.0.6'
+__version__     = '0.0.7'
 __description__ = 'InvenioRDM GitHub Archiver'
 __url__         = 'https://github.com/caltechlibrary/iga'
 __author__      = 'Michael Hucka'
 __email__       = 'helpdesk@library.caltech.edu'
 __license__     = 'https://github.com/caltechlibrary/iga/blob/main/LICENSE'
```

### Comparing `iga-0.0.6/iga/__main__.py` & `iga-0.0.7/iga/__main__.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga/cli.py` & `iga-0.0.7/iga/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 from   rich.style import Style
 import rich_click as click
 from   rich_click import File, Path, INT, Choice
 import sys
 from   sidetrack import set_debug, log
 
 from iga.exit_codes import ExitCode
-from iga.exceptions import GitHubError, InvenioRDMError
+from iga.exceptions import GitHubError, InvenioRDMError, RecordNotFound
 from iga.github import (
     github_account_repo_tag,
     github_release_assets,
     valid_github_release_url,
 )
+from iga.id_utils import is_invenio_rdm
 from iga.invenio import (
     invenio_api_available,
     invenio_communities,
     invenio_community_send,
     invenio_create,
     invenio_publish,
     invenio_upload,
@@ -295,15 +296,15 @@
             table.add_row(community.name, community.title,
                           f'[link={community.url}]{community.url}[/]')
         Console().print()
         Console().print(table)
     except KeyboardInterrupt:
         log('keyboard interrupt received')
         sys.exit(int(ExitCode.interrupt))
-    except Exception as ex:
+    except Exception as ex:             # noqa PIE786
         log('exception trying to list communities: ' + str(ex))
         _alert(ctx, 'Unable to get a list of communitities from the InvenioRDM'
                f' server at {server}. Please check the server address and the'
                ' condition of the network.')
         sys.exit(int(ExitCode.exception))
     sys.exit(int(ExitCode.success))
 
@@ -349,42 +350,46 @@
               help="InvenioRDM access token (**avoid – use variable**)")
 #
 @click.option('--list-communities', '-L', is_flag=True, callback=_list_communities,
               help='List communities available for `--community`')
 #
 @click.option('--log-dest', '-l', metavar='FILE', callback=_config_log,
               type=File('w', lazy=False), expose_value=False, is_eager=True,
-              help='Send log output to _FILE_ (use `-` for stdout)')
+              help='Send log output to _FILE_ (use "`-`" for stdout)')
 #
 @click.option('--mode', '-m', metavar='STR', callback=_config_mode, is_eager=True,
               type=Choice(['normal', 'quiet', 'verbose', 'debug'], case_sensitive=False),
               help='Run mode: `quiet`, **`normal`**, `verbose`, `debug`')
 #
-@click.option('--open', '-O', is_flag=True,
-              help='Open the finished record in the default web browser')
+@click.option('--open', '-o', 'open_in_browser', is_flag=True,
+              help='Open the finished record in your web browser')
 #
-@click.option('--read-record', '-R', 'source', metavar='FILE', type=File('r'),
+@click.option('--parent-record', '-p', 'parent_id', metavar='STR',
+              help='Make this a new version of an existing record')
+#
+@click.option('--read-metadata', '-R', 'source', metavar='FILE', type=File('r'),
               help='Read metadata record from _FILE_; don\'t build one')
 #
-@click.option('--save-record', '-S', 'dest', metavar='FILE', type=File('w', lazy=False),
+@click.option('--save-metadata', '-S', 'dest', metavar='FILE', type=File('w', lazy=False),
               help='Save metadata record to _FILE_; don\'t upload it')
 #
 @click.option('--timeout', '-T', metavar='NUM', type=INT, callback=_read_timeout,
               help='Wait on network operations a max of _NUM_ seconds')
 #
 @click.option('--version', '-V', callback=_print_version_and_exit, is_flag=True,
               help='Print IGA version and exit', expose_value=False, is_eager=True)
 #
 @click.argument('url_or_tag', required=True)
 @click.pass_context
 def cli(ctx, url_or_tag, all_assets=False, community=None, draft=False,
         files_to_upload=None, account=None, repo=None, github_token=None,
-        server=None, invenio_token=None, list_communities=False, open=False,
-        log_dest=None, mode='normal', all_metadata=False, source=None,
-        dest=None, timeout=None, help=False, version=False):  # noqa A002
+        server=None, invenio_token=None, list_communities=False,
+        open_in_browser=False, log_dest=None, mode='normal', parent_id=None,
+        all_metadata=False, source=None, dest=None, timeout=None,
+        help=False, version=False):  # noqa A002
     '''InvenioRDM GitHub Archiver (IGA) command-line interface.
 \r
 IGA creates a metadata record in an InvenioRDM server and attaches a GitHub
 release archive to the record. The GitHub release can be specified using
 _either_ a full release URL, _or_ a combination of GitHub account + repository
 \+ tag. Different command-line options can be used to adjust this behavior.
 \r
@@ -413,19 +418,19 @@
  2. A combination of _account name_, _repository name_, and _tag_. In this
     case, the final argument on the command line must be the _tag_, and in
     addition, values for the options `--account` and `--repo` must be provided.
 \r
 Here's an example using approach #1 (assuming environment variables
 INVENIO_SERVER, INVENIO_TOKEN, and GITHUB_TOKEN have all been set):
 ```shell
-    iga https://github.com/mhucka/taupe/releases/tag/v1.2.0
+  iga https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 and here's the equivalent using approach #2:
 ```shell
-    iga --github-account mhucka --github-repo taupe v1.2.0
+  iga --github-account mhucka --github-repo taupe v1.2.0
 ```
 Note that when using this form of the command, the release tag ("v1.2.0" above)
 must be the last item given on the command line.
 \r
 _**Use of a GitHub access token**_
 \r
 It is possible to run IGA without providing a GitHub access token. GitHub
@@ -501,14 +506,29 @@
 instead, use the option `--draft`. The draft option also takes precedence over
 the community option: if you use both `--draft` and `--community`, IGA will
 stop after creating the draft record and will _not_ submit it to the community.
 (You can nevertheless submit the record to a community manually once the draft
 is created, by visiting the record's web page and using the InvenioRDM
 interface there.)
 \r
+_**Versioning of records**_
+\r
+The option `--parent-record` can be used to indicate that the record being
+constructed is a new version of an existing record. This will make IGA use the
+InvenioRDM API for record versioning. The newly-created record will be linked
+to a parent record identified by the value passed to `--parent-record`. The
+value must be either an InvenioRDM record identifier (which is a sequence of
+alphanumeric characters of the form _XXXXX-XXXXX_, such as `bknz4-bch35`,
+generated by the InvenioRDM server), or a URL to the landing page of the record
+in the InvenioRDM server. (Such URLs contain an embedded record identifier.)
+Here is an example of using this option:
+```
+  iga --parent-record xbcd4-efgh5 https://github.com/foo/bar/releases/tag/v1
+```
+\r
 _**Other options recognized by IGA**_
 \r
 Running IGA with the option `--save-record` will make it create a metadata
 record, but instead of uploading the record (and any assets) to the InvenioRDM
 server, IGA will write the result to the given destination. This can be useful
 not only for debugging but also for creating a starting point for a custom
 metadata record: first run IGA with `--save-record` to save a record to a file,
@@ -585,14 +605,20 @@
 
     if community and community not in invenio_communities():
         _alert(ctx, f'"{community}" is not the name of a known community in'
                ' the InvenioRDM server. The known communities can be obtained'
                ' by using the option `--list-communities`.')
         sys.exit(int(ExitCode.file_error))
 
+    if parent_id and not is_invenio_rdm(parent_id):
+        _alert(ctx, f'"{parent_id}" does not appear to be an InvenioRDM'
+               ' record identifier.')
+        sys.exit(int(ExitCode.file_error))
+
+
     # Do the main work ........................................................
 
     from iga.metadata import metadata_for_release, metadata_from_file
 
     log(f'invoked with command line: {sys.argv}')
     exit_code = ExitCode.success
     try:
@@ -613,15 +639,15 @@
         if dest:
             import json
             dest.write(json.dumps(metadata, indent=2))
             dest.write('\n')
             _inform(f'Wrote metadata to {dest.name}.')
         else:
             _inform('Sending metadata to InvenioRDM server', end='...')
-            record = invenio_create(metadata)
+            record = invenio_create(metadata, parent_id)
             _inform(' done.')
 
             _inform('Attaching assets:')
             for item in files_to_upload or github_assets:
                 invenio_upload(record, item, _print_text)
             _inform('Done.')
 
@@ -633,16 +659,16 @@
                         f' and the draft is available at {record.draft_url}')
             else:
                 invenio_publish(record)
                 _inform(f'The published record is available at {record.record_url}')
         if os.environ.get('IGA_RUN_MODE') == 'quiet':
             # In quiet mode nothing else will be printed, so we finish with this
             click.echo(record.record_url or record.draft_url)
-        if open:
-            log('opening {record.record_url or record.draft_url}')
+        if open_in_browser:
+            log(f'opening {record.record_url or record.draft_url}')
             click.launch(record.record_url or record.draft_url)
     except KeyboardInterrupt:
         log('keyboard interrupt received')
         exit_code = ExitCode.user_interrupt
     except bdb.BdbQuit:
         # Exiting the debugger. Not a real exception.
         pass
@@ -656,14 +682,17 @@
                 text += (' The partially-completed record can be found at'
                          f' [{record.draft_url}]({record.draft_url}). You'
                          ' may complete it manually, or delete it and try again.')
             if os.environ.get('IGA_RUN_MODE') in ['verbose', 'debug']:
                 text += f'\n\nThe error is as follows: **{ex}**'
             _alert(ctx, text)
             exit_code = ExitCode.inveniordm_error
+        elif isinstance(ex, RecordNotFound):
+            _alert(ctx, f'Unable to continue. {str(ex)}.')
+            exit_code = ExitCode.inveniordm_error
         else:
             import iga
             error_type = ex.__class__.__name__
             log(f'exiting due to {error_type}: {str(ex)}')
             _alert(ctx, 'IGA experienced an error. Please report this to the'
                    f' developers. Your version of IGA is {iga.__version__}.'
                    f' For information about how to report errors, please see'
```

### Comparing `iga-0.0.6/iga/data_utils.py` & `iga-0.0.7/iga/data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga/doi.py` & `iga-0.0.7/iga/doi.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga/exceptions.py` & `iga-0.0.7/iga/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,9 +29,13 @@
     '''InvenioRDM returned an error.'''
 
 
 class MissingData(IGAException):
     '''Could not obtain all the required data to create an InvenioRDM record.'''
 
 
+class RecordNotFound(IGAException):
+    '''Could not find the requested record in the InvenioRDM server.'''
+
+
 class InternalError(IGAException):
     '''An internal error occurred in IGA.'''
```

### Comparing `iga-0.0.6/iga/exit_codes.py` & `iga-0.0.7/iga/exit_codes.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga/github.py` & `iga-0.0.7/iga/github.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga/invenio.py` & `iga-0.0.7/iga/invenio.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 import os
 from   os import path
 
 import iga
 from   iga.exceptions import (
     InternalError,
     InvenioRDMError,
+    RecordNotFound,
 )
+from   iga.id_utils import normalize_invenio_rdm
 
 
 # Exported data structures.
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 @dataclass
 class InvenioRecord():
@@ -84,29 +86,67 @@
         return False
     except Exception:
         raise
     log(f'failed to reach server {server_url}')
     return False
 
 
-def invenio_create(metadata):
-    '''Create a record in the InvenioRDM server using the given metadata.
-
-    This only creates a record, and returns an InvenioRecord data class; it
-    does not upload file attachments, which is something handled by a separate
-    function, invenio_upload(...).
+def invenio_get(record_id):
+    '''Get the InvenioRDM record with the given identifier.'''
+    log(f'asking InvenioRDM server for record {record_id}')
+    record_id = normalize_invenio_rdm(record_id)
+    result = _invenio('get', endpoint=f'/api/records/{record_id}',
+                      msg='get record {record_id}')
+    if result is None:
+        # Maybe it's a draft record -- try one more time with /draft appended.
+        result = _invenio('get', endpoint=f'/api/records/{record_id}/draft',
+                          msg='get record {record_id}')
+    if result is None:
+        raise RecordNotFound(f'Could not find record with id {record_id}')
+    return result
+
+
+def invenio_create(metadata, parent_id=None):
+    '''Create a record in the InvenioRDM server using the given metadataa.
+
+    This only creates a draft record, and returns an InvenioRecord data class;
+    it does not upload file attachments, which is something handled by a
+    separate function, invenio_upload(...), or publish the record, which is
+    handled by invenio_publish(...).
     '''
-    log('creating record in InvenioRDM')
-    result = _invenio('post', endpoint='/api/records', data=metadata,
-                      msg='create new record using metadata')
+    # Relevant InvenioRDM documentation:
+    # https://inveniordm.docs.cern.ch/reference/rest_api_drafts_records/#drafts
+    # https://inveniordm.docs.cern.ch/reference/rest_api_drafts_records/#versions
+    if parent_id:
+        # Make sure parent actually exists. The resulting record is not needed.
+        invenio_get(parent_id)
+
+        log(f'creating a new version of record {parent_id} in InvenioRDM')
+        result = _invenio('post', endpoint=f'/api/records/{parent_id}/versions',
+                          msg='create new record using metadata')
+        if not result:
+            raise InvenioRDMError(f'Unable to create new version of {parent_id}')
+        record_id = result['id']
+
+        log(f'updating metadata in new record {record_id} in InvenioRDM')
+        metadata['files'] = {'enabled': True}
+        result = _invenio('put', endpoint=f'/api/records/{record_id}/draft',
+                          data=metadata, msg='create new record using metadata')
+        # The server will make some changes to the metadata we send.
+        result['metadata'] = metadata
+    else:
+        log('creating record in InvenioRDM')
+        result = _invenio('post', endpoint='/api/records', data=metadata,
+                          msg='create new record using metadata')
+
     if validation_errors := result.get('errors', []):
         log(f'the server reported {pluralized("error", validation_errors, True)}:')
         for error in validation_errors:
             log(f' * in field "{error["field"]}": {error["messages"]}')
-        # FIXME need to report to user
+        # FIXME some should be reported to the user, but others are harmless.
     else:
         log('record created successfully with no errors')
 
     record = InvenioRecord(data=result,
                            draft_url=result['links']['self_html'],
                            review_url=result['links']['review'],
                            publish_url=result['links']['publish'],
@@ -282,15 +322,15 @@
     data_type = 'json' if isinstance(data, (dict, list)) else 'octet-stream'
     headers = {'Content-type': 'application/' + data_type}
     if token := os.environ.get('INVENIO_TOKEN'):
         headers['Authorization'] = 'Bearer ' + token
 
     if os.environ.get('IGA_RUN_MODE') == 'debug':
         d = json.dumps(data, indent=2) if data_type == 'json' else ''
-        log(f'doing {action} on {url} with payload' + (f':\n{d}' if d else ''))
+        log(f'doing {action} on {url}' + (f' with payload:\n{d}' if d else ''))
 
     # Construct a Python partial to gather some args for calling network().
     client = None
     if action == 'put':
         # 'put' => data is being uploaded, so we need to set longer timeouts.
         import httpx
         tmout = _network_timeout(data)
```

### Comparing `iga-0.0.6/iga/json_utils.py` & `iga-0.0.7/iga/json_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga/licenses.py` & `iga-0.0.7/iga/licenses.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga/metadata.py` & `iga-0.0.7/iga/metadata.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga/name_utils.py` & `iga-0.0.7/iga/name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga/orcid.py` & `iga-0.0.7/iga/orcid.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga/reference.py` & `iga-0.0.7/iga/reference.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga/ror.py` & `iga-0.0.7/iga/ror.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga/text_utils.py` & `iga-0.0.7/iga/text_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga.egg-info/PKG-INFO` & `iga-0.0.7/iga.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 0.0.6
+Version: 0.0.7
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -141,15 +141,15 @@
 ```
 Note that when using this form of the command, the release tag (`v1.2.0` above) must be the last item given on the command line.
 
 ### Use of a GitHub access token
 
 It is possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for many repositories, IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
 
-### Construction of an InvenioRDM record
+### Gathering metadata for an InvenioRDM record
 
 The record created in InvenioRDM is constructed using information obtained using GitHub's API as well as several other APIs as needed. The information includes the following:
  * (if one exists) a `codemeta.json` file in the GitHub repository
  * (if one exists) a `CITATION.cff` file in the GitHub repository
  * data available from GitHub for the release
  * data available from GitHub for the repository
  * data available from GitHub for the account of the owner
@@ -158,35 +158,42 @@
  * data available from ORCID.org for ORCID identifiers
  * data available from ROR.org for Research Organization Registry identifiers
  * data available from DOI.org, NCBI, Google Books, & others for publications
  * data available from spdx.org for software licenses
 
 IGA tries to use `CodeMeta.json` first and `CITATION.cff` second to fill out the fields of the InvenioRDM record. If neither of those files are present, IGA uses values from the GitHub repository instead. You can make it always use all sources of info with the option `--all-metadata`. Depending on how complete and up-to-date your `CodeMeta.json` and `CITATION.cff` are, this may or may not make the record more comprehensive and may or may not introduce redundancies or unwanted values.
 
-To override the auto-created record, use the option `--read-record` followed by the path to a JSON file structured according to the InvenioRDM schema used by the destination server. When `--read-record` is provided, IGA does _not_ extract the data above, but still obtains the file assets from GitHub.
+To override the auto-created metadata, use the option `--read-metadata` followed by the path to a JSON file structured according to the InvenioRDM schema used by the destination server. When `--read-metadata` is provided, IGA does _not_ extract the data above, but still obtains the file assets from GitHub.
 
 ### Specification of GitHub file assets
 
 By default, IGA attaches to the InvenioRDM record _only_ the ZIP file asset created by GitHub for the release. To make IGA attach all assets associated with the GitHub release, use the option `--all-assets`.
 
 To upload specific file assets and override the default selections made by IGA, you can use the option `--file` followed by a path to a file to be uploaded.  You can repeat the option `--file` to upload multiple file assets. Note that if `--file` is provided, then IGA _does not use any file assets from GitHub_; it is the user's responsibility to supply all the files that should be uploaded.
 
-If both `--read-record` and `--file` are used, then IGA does not actually contact GitHub for any information.
+If both `--read-metadata` and `--file` are used, then IGA does not actually contact GitHub for any information.
 
 ### Handling communities
 
 To submit your record to a community, use the `--community` option together with a community name. The option `--list-communities` can be used to get a list of communities supported by the InvenioRDM server. Note that submitting a record to a community means that the record will not be finalized and will not be publicly visible when IGA finishes; instead, the record URL that you receive will be for a draft version, pending review by the community moderators.
 
 ### Draft versus published records
 
 If the `--community` option is not used, then by default, IGA will finalize and publish the record. To make it stop short and leave the record as a draft instead, use the option `--draft`. The draft option also takes precedence over the community option: if you use both `--draft` and `--community`, IGA will stop after creating the draft record and will _not_ submit it to the community.  (You can nevertheless submit the record to a community manually once the draft is created, by visiting the record's web page and using the InvenioRDM interface there.)
 
+### Versioning of records
+
+The option `--parent-record` can be used to indicate that the record being constructed is a new version of an existing record. This will make IGA use the InvenioRDM API for [record versioning](https://inveniordm.docs.cern.ch/releases/versions/version-v2.0.0/#versioning-support). The newly-created record will be linked to a parent record identified by the value passed to `--parent-record`. The value must be either an InvenioRDM record identifier (which is a sequence of alphanumeric characters of the form _XXXXX-XXXXX_, such as `bknz4-bch35`, generated by the InvenioRDM server), or a URL to the landing page of the record in the InvenioRDM server. (Note that such URLs end in the record identifier.) Here is an example of using this option:
+```
+iga --parent-record xbcd4-efgh5 https://github.com/mhucka/taupe/releases/tag/v1.2.0
+```
+
 ### Other options recognized by IGA
 
-Running IGA with the option `--save-record` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-record` to save a record to a file, edit the result, then finally run IGA with the `--read-record` option to use the modified record to create a release in the InvenioRDM server.
+Running IGA with the option `--save-metadata` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-metadata` to save a record to a file, edit the result, then finally run IGA with the `--read-metadata` option to use the modified record to create a release in the InvenioRDM server.
 
 The `--mode` option can be used to change the run mode. Four run modes are available: `quiet`, `normal`, `verbose`, and `debug`. The default mode is `normal`, in which IGA prints a few messages while it's working. The mode `quiet` will make it avoid printing anything unless an error occurs, the mode `verbose` will make it print a detailed trace of what it is doing, and the mode `debug` will make IGA even more verbose. In addition, in `debug` mode, IGA will drop into the `pdb` debugger if it encounters an exception during execution. On Linux and macOS, debug mode also installs a signal handler on signal USR1 that causes IGA to drop into the `pdb` debugger if the signal USR1 is received. (Use `kill -USR1 NNN`, where NNN is the IGA process id.)
 
 Networks latencies are unpredicatable. Reading and writing large files may take a long time; on the other hand, IGA should not wait forever before reporting an error if a server or network becomes unresponsive. To balance these conflicting needs, IGA automatically scales its network timeout based on file sizes. To override its adaptive algorithm and set an explicit timeout value, use the option `--timeout` with a value in seconds.
 
 By default, the output of the `verbose` and `debug` run modes is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` to indicate console output, or a file path to send the output to the file.
 
@@ -211,23 +218,25 @@
 | `--github-token` _T_   | `-t` _T_ | Use GitHub acccess token _T_| Use value in env. var. `GITHUB_TOKEN` | |
 | `--help`               | `-h`     | Print help info and exit | | |
 | `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
 | `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
-| `--open`               | `-O`     | Open record's RDM web page in a browser when done | Do nothing when done | |
-| `--read-record` _R_    | `-R` _R_ | Read metadata record from _R_; don\'t build one | Build metadata record | |
-| `--save-record` _D_    | `-S` _D_ | Save metadata record to _D_; don\'t upload it | Upload to InvenioRDM server | |
+| `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
+| `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
+| `--read-metadata` _R_  | `-R` _R_ | Read metadata record from file _R_; don\'t build one | Build metadata record | |
+| `--save-metadata` _D_  | `-S` _D_ | Save metadata record to file _D_; don\'t upload it | Upload to InvenioRDM server | |
 | `--timeout` _X_        | `-T` _X_ | Wait on network operations a max of _X_ seconds | Auto-adjusted based on file size | |
 | `--version`            | `-V`     | Print program version info and exit | | |
 
-⚑ &nbsp; Can repeat for multiple files.<br>
+⚑ &nbsp; Can repeat the option to specify multiple files.<br>
 ⚐ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.<br>
-✯ &nbsp; When using `--github-account` and `--github-repo`, the last argument on the command line must be a release tag name.
+✯ &nbsp; When using `--github-account` and `--github-repo`, the last argument on the command line must be a release tag name.<br>
+❖ &nbsp; The record identifier must be given either as a sequence of alphanumeric characters of the form _XXXXX-XXXXX_ (e.g., `bknz4-bch35`), or as a URL to the landing page of an existing record in the InvenioRDM server.
 
 ### Return values
 
 This program exits with a return status code of 0 if no problem is encountered.  Otherwise, it returns a nonzero status code. The following table lists the possible values:
 
 | Code | Meaning                                                  |
 |:----:|----------------------------------------------------------|
```

### Comparing `iga-0.0.6/iga.egg-info/SOURCES.txt` & `iga-0.0.7/iga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/iga.egg-info/requires.txt` & `iga-0.0.7/iga.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aenum==3.1.11
 arrow==1.2.3
 boltons==21.0.0
 caltechdata-api==1.3.0
-commonpy==1.12.2
+commonpy==1.12.4
 demoji==1.1.0
 dirtyjson==1.0.8
 httpx==0.23.1
 humanize==4.4.0
 idutils==1.2.0
 iptools==0.7.0
 isbnlib==3.10.12
```

### Comparing `iga-0.0.6/setup.cfg` & `iga-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iga
-version = 0.0.6
+version = 0.0.7
 description = InvenioRDM GitHub Archiver
 author = Michael Hucka
 author_email = helpdesk@library.caltech.edu
 license = https://github.com/caltechlibrary/iga/blob/main/LICENSE
 license_files = LICENSE
 url = https://github.com/caltechlibrary/iga
 project_urls =
```

### Comparing `iga-0.0.6/setup.py` & `iga-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_cli.py` & `iga-0.0.7/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 @mock.patch('iga.orcid.orcid_data', new=mocked_orcid_data)
 def test_environment_vars_from_options(capsys):
     from iga.cli import cli
     runner = click.testing.CliRunner()
     args = ['--invenio-server', 'https://data.caltechlibrary.dev',
             '--invenio-token', 'itoken',
             '--github-token', 'gtoken',
-            '--save-record', '/tmp/fake.json',
+            '--save-metadata', '/tmp/fake.json',
             'https://github.com/fakeaccount/fakerepo/releases/tag/fakerelease']
     result = runner.invoke(cli, args)
     assert result.exit_code == int(ExitCode.success)
     assert 'INVENIO_SERVER' in os.environ
     assert os.environ['INVENIO_SERVER'] == 'https://data.caltechlibrary.dev'
     assert 'INVENIO_TOKEN' in os.environ
     assert os.environ['INVENIO_TOKEN'] == 'itoken'
```

### Comparing `iga-0.0.6/tests/test_data_utils.py` & `iga-0.0.7/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_doi.py` & `iga-0.0.7/tests/test_doi.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_exceptions.py` & `iga-0.0.7/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_github.py` & `iga-0.0.7/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_github_mocks.py` & `iga-0.0.7/tests/test_github_mocks.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_init.py` & `iga-0.0.7/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_is_person.py` & `iga-0.0.7/tests/test_is_person.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_licenses.py` & `iga-0.0.7/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_name_splitting.py` & `iga-0.0.7/tests/test_name_splitting.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_name_utils.py` & `iga-0.0.7/tests/test_name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_orcid.py` & `iga-0.0.7/tests/test_orcid.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_record_from_codemeta.py` & `iga-0.0.7/tests/test_record_from_codemeta.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_reference.py` & `iga-0.0.7/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_ror.py` & `iga-0.0.7/tests/test_ror.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.6/tests/test_text_utils.py` & `iga-0.0.7/tests/test_text_utils.py`

 * *Files identical despite different names*

