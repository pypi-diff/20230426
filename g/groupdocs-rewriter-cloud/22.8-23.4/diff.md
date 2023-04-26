# Comparing `tmp/groupdocs-rewriter-cloud-22.8.tar.gz` & `tmp/groupdocs-rewriter-cloud-23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\groupdocs-rewriter-cloud-22.8.tar", last modified: Sun Jul 31 22:38:20 2022, max compression
+gzip compressed data, was "dist\groupdocs-rewriter-cloud-23.4.tar", last modified: Wed Apr 26 08:46:24 2023, max compression
```

## Comparing `groupdocs-rewriter-cloud-22.8.tar` & `groupdocs-rewriter-cloud-23.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2022-07-31 22:38:20.081844 groupdocs-rewriter-cloud-22.8/
--rw-rw-rw-   0        0        0    12877 2022-07-31 22:38:20.080848 groupdocs-rewriter-cloud-22.8/PKG-INFO
--rw-rw-rw-   0        0        0    10274 2022-07-31 21:50:04.000000 groupdocs-rewriter-cloud-22.8/README.md
-drwxrwxrwx   0        0        0        0 2022-07-31 22:38:20.052922 groupdocs-rewriter-cloud-22.8/groupdocs_rewriter_cloud.egg-info/
--rw-rw-rw-   0        0        0    12877 2022-07-31 22:38:19.000000 groupdocs-rewriter-cloud-22.8/groupdocs_rewriter_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1351 2022-07-31 22:38:19.000000 groupdocs-rewriter-cloud-22.8/groupdocs_rewriter_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-31 22:38:19.000000 groupdocs-rewriter-cloud-22.8/groupdocs_rewriter_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2022-07-31 22:38:19.000000 groupdocs-rewriter-cloud-22.8/groupdocs_rewriter_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2022-07-31 22:38:19.000000 groupdocs-rewriter-cloud-22.8/groupdocs_rewriter_cloud.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-07-31 22:38:20.056945 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/
--rw-rw-rw-   0        0        0     1665 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-31 22:38:20.059904 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/api/
--rw-rw-rw-   0        0        0     1482 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/api/__init__.py
--rw-rw-rw-   0        0        0    10682 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/api/rewriter_api.py
--rw-rw-rw-   0        0        0    56910 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/api/storage_api.py
--rw-rw-rw-   0        0        0    25431 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/api_client.py
--rw-rw-rw-   0        0        0    10057 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/configuration.py
-drwxrwxrwx   0        0        0        0 2022-07-31 22:38:20.074863 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/
--rw-rw-rw-   0        0        0     2094 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/__init__.py
--rw-rw-rw-   0        0        0     2972 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/base_model.py
--rw-rw-rw-   0        0        0     3556 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     3199 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/document_response.py
--rw-rw-rw-   0        0        0     4586 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/error.py
--rw-rw-rw-   0        0        0     3377 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/error_details.py
--rw-rw-rw-   0        0        0     7202 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/file_version.py
--rw-rw-rw-   0        0        0     2650 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/file_versions.py
--rw-rw-rw-   0        0        0     2682 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/files_list.py
--rw-rw-rw-   0        0        0     3416 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     3575 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/object_exist.py
--rw-rw-rw-   0        0        0     3636 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/rewrite_document.py
--rw-rw-rw-   0        0        0     2632 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/rewrite_text.py
--rw-rw-rw-   0        0        0     2711 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     5521 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/storage_file.py
--rw-rw-rw-   0        0        0     4128 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/text_response.py
--rw-rw-rw-   0        0        0    14697 2022-07-31 21:49:03.000000 groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/rest.py
--rw-rw-rw-   0        0        0       42 2022-07-31 22:38:20.081844 groupdocs-rewriter-cloud-22.8/setup.cfg
--rw-rw-rw-   0        0        0     3178 2022-07-31 21:53:18.000000 groupdocs-rewriter-cloud-22.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-31 22:38:20.079849 groupdocs-rewriter-cloud-22.8/test/
--rw-rw-rw-   0        0        0     1441 2022-07-31 21:49:21.000000 groupdocs-rewriter-cloud-22.8/test/__init__.py
--rw-rw-rw-   0        0        0     3534 2022-07-31 21:49:21.000000 groupdocs-rewriter-cloud-22.8/test/test_helper.py
--rw-rw-rw-   0        0        0     3483 2022-07-31 21:49:21.000000 groupdocs-rewriter-cloud-22.8/test/test_rewriter_api.py
--rw-rw-rw-   0        0        0    13208 2022-07-31 21:49:21.000000 groupdocs-rewriter-cloud-22.8/test/test_storage_api.py
+drwxrwxrwx   0        0        0        0 2023-04-26 08:46:24.546115 groupdocs-rewriter-cloud-23.4/
+-rw-rw-rw-   0        0        0    13635 2023-04-26 08:46:24.546115 groupdocs-rewriter-cloud-23.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10944 2023-04-26 08:37:48.000000 groupdocs-rewriter-cloud-23.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 08:46:24.347335 groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/
+-rw-rw-rw-   0        0        0    13635 2023-04-26 08:46:24.000000 groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1351 2023-04-26 08:46:24.000000 groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 08:46:24.000000 groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-26 08:46:24.000000 groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-26 08:46:24.000000 groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 08:46:24.378398 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/
+-rw-rw-rw-   0        0        0     1665 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 08:46:24.403856 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/
+-rw-rw-rw-   0        0        0     1482 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/__init__.py
+-rw-rw-rw-   0        0        0    10682 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/rewriter_api.py
+-rw-rw-rw-   0        0        0    56910 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/storage_api.py
+-rw-rw-rw-   0        0        0    25431 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api_client.py
+-rw-rw-rw-   0        0        0    10057 2022-12-30 11:43:49.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/configuration.py
+drwxrwxrwx   0        0        0        0 2023-04-26 08:46:24.517444 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/
+-rw-rw-rw-   0        0        0     2094 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/__init__.py
+-rw-rw-rw-   0        0        0     2972 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/base_model.py
+-rw-rw-rw-   0        0        0     3556 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0     3718 2022-12-30 11:20:06.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/document_response.py
+-rw-rw-rw-   0        0        0     4586 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/error.py
+-rw-rw-rw-   0        0        0     3377 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/error_details.py
+-rw-rw-rw-   0        0        0     7202 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/file_version.py
+-rw-rw-rw-   0        0        0     2650 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     2682 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/files_list.py
+-rw-rw-rw-   0        0        0     3416 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     3575 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     3803 2022-12-30 09:03:16.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/rewrite_document.py
+-rw-rw-rw-   0        0        0     3249 2022-12-30 09:06:12.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/rewrite_text.py
+-rw-rw-rw-   0        0        0     2711 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     5521 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/storage_file.py
+-rw-rw-rw-   0        0        0     4348 2022-12-30 09:07:44.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/text_response.py
+-rw-rw-rw-   0        0        0    14697 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/rest.py
+-rw-rw-rw-   0        0        0       42 2023-04-26 08:46:24.547112 groupdocs-rewriter-cloud-23.4/setup.cfg
+-rw-rw-rw-   0        0        0     3255 2023-04-26 08:39:17.000000 groupdocs-rewriter-cloud-23.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 08:46:24.545115 groupdocs-rewriter-cloud-23.4/test/
+-rw-rw-rw-   0        0        0     1441 2022-12-30 22:38:33.000000 groupdocs-rewriter-cloud-23.4/test/__init__.py
+-rw-rw-rw-   0        0        0     3534 2022-12-30 22:38:33.000000 groupdocs-rewriter-cloud-23.4/test/test_helper.py
+-rw-rw-rw-   0        0        0     3483 2022-12-30 22:38:33.000000 groupdocs-rewriter-cloud-23.4/test/test_rewriter_api.py
+-rw-rw-rw-   0        0        0    13208 2022-12-30 22:38:33.000000 groupdocs-rewriter-cloud-23.4/test/test_storage_api.py
```

### Comparing `groupdocs-rewriter-cloud-22.8/PKG-INFO` & `groupdocs-rewriter-cloud-23.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: groupdocs-rewriter-cloud
-Version: 22.8
+Version: 23.4
 Summary: GroupDocs.Rewriter Cloud SDK
 Home-page: https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python
 Author: Aspose
 Author-email: ekaterina.tretiak@aspose.com
 License: MIT
 Description: # Python SDK for GroupDocs.Rewriter Cloud
         
         ![](https://img.shields.io/badge/api-v1.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/groupdocs-rewriter-cloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/groupdocs-rewriter-cloud) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/groupdocs-rewriter-cloud) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/groupdocs-rewriter-cloud) [![GitHub license](https://img.shields.io/github/license/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python)](https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python/blob/master/LICENSE)
         
         [Product Page](https://products.groupdocs.cloud/rewriter/python/) | [Documentation](https://docs.groupdocs.cloud/rewriter/) | [Demos](https://products.groupdocs.app/rewriter/family) | [Swagger UI](https://apireference.groupdocs.cloud/rewriter/) | [Examples](https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python) | [Blog](https://blog.groupdocs.cloud/category/rewriter/) | [Search](https://search.groupdocs.cloud/) | [Free Support](https://forum.groupdocs.cloud/c/rewriter) | [Free Trial](https://purchase.groupdocs.cloud/trial)
         
-        [GroupDocs.Rewriter Cloud](https://products.groupdocs.cloud/rewriter/) is an easy-to-use and versatile online service for rephrasing the content of Microsoft Word, Open Office, PDF, and plain text documents with full preservation of their meaning. A powerful neural network reads and understands the text and then paraphrases it with different wording, producing a plagiarism-free result. While the background process is very complex and resource-intensive, you do not have to worry about formulas, machine learning, and load - our cloud services do all the work by providing you with a REST API to interact with them.
+        [GroupDocs.Rewriter Cloud](https://products.groupdocs.cloud/rewriter/) is an easy-to-use and versatile online service for rephrasing the content of Microsoft Word®, OpenOffice, Adobe Acrobat® PDF documents, Markdown and HTML files as well as a plain text with full preservation of their meaning. A powerful neural network reads and understands the text and then paraphrases it with different wording, producing a plagiarism-free result. While the background process is very complex and resource-intensive, you do not have to worry about formulas, machine learning, and load - our cloud services do all the work by providing you with a REST API to interact with them.
         
         This software development kit (SDK) simplifies the interaction with GroupDocs.Rewriter Cloud API from Python code, allowing you to focus on the task at hand rather than the technical details. It handles all the routine operations such as establishing connection, sending API requests, and parsing responses, wrapping all these tasks into a few lines of code that are very easy to read and maintain even for inexperienced developers.
         
         ## Before you begin
         
         GroupDocs.Rewriter Cloud is an on-demand service. As such, it has no specific hardware or operating system requirements. In order to use the service, you must create an account at GroupDocs Cloud API:
         
@@ -36,30 +36,39 @@
         GroupDocs.Rewriter Cloud can rephrase documents in the most popular formats.
         
         Document | Extensions | Description
         -------- | ---------- | -----------
         Microsoft Word | .DOCX<br />.DOCM<br />.DOC<br />.RTF | Microsoft Word 97-2021 and Microsoft 365 Word documents, including macro-enabled documents.
         Portable Document Format | .PDF | An open standard cross-platform format for documents that include formatted text, images, multimedia elements, and more.
         OpenDocument Text | .ODT | Documents created with a number of open source word processing applications, such as Writer from Apache OpenOffice and LibreOffice.
+        Markdown | .MD | Files created using one of dialects of the Markdown language.
+        HTML | .HTML | Files containing Hypertext Markup Language (HTML) that formats the structure of a webpage. 
         Plain text | .TXT | Plain text files or text in the form of lines.
         
         In addition to rephrasing, GroupDocs.Rewriter Cloud can save the resulting document in various file formats other than the original, with formatting preserved (where applicable).
         
         Source file format | Paraphrased file format
         ------------------ | ----------------------
         .DOCX              | .DOCX<br />.RTF<br />.HTML<br />.ODT<br />.TXT<br />.MD<br />.PDF<br />.TIFF<br />.SVG<br />.XPS
         .DOC               | .DOC<br />.DOCX<br />.RTF<br />.HTML<br />.ODT<br />.TXT<br />.MD<br />.PDF<br />.TIFF<br />.SVG<br />.XPS
         .ODT               | .DOCX<br />.RTF<br />.HTML<br />.ODT<br />.TXT<br />.MD<br />.PDF<br />.TIFF<br />.SVG<br />.XPS
         .RTF               | .DOCX<br />.RTF<br />.HTML<br />.ODT<br />.TXT<br />.MD<br />.PDF<br />.TIFF<br />.SVG<br />.XPS
-        .PDF               | .DOCX<br />.PPTX<br />.HTML<br />.XPS<br />.SVG
+        .PDF               | .PDF<br />.DOCX<br />.PPTX<br />.HTML<br />.XPS<br />.SVG
+        .MD                | .MD<br />
+        .HTML              | .HTML<br />.PDF<br />.DOCX<br />.TIFF<br />.XPS<br />
         
         ## Supported languages
         
+        - **ar** — to paraphrase Arabic text or document
+        — **de** — to paraphrase German text or document
         - **en** — to paraphrase English text or document
+        — **fr** — to paraphrase French text or document
+        — **id** — to paraphrase Indonesian text or document
         - **ru** — to paraphrase Russian text or document
+        - **uk** — to paraphrase Ukrainian text or document
         
         ## Quick start
         
         To start using GroupDocs.Rewriter Cloud in your Python applications, follow a few simple steps:
         
         ## System requirements
         
@@ -142,26 +151,27 @@
         The following code snippets demonstrate how to use the GroupDocs.Rewriter Python SDK to accomplish various tasks.
         
         ### Rewrite a text
         
         ```python
         # Load the gem
         import groupdocs_rewriter_cloud
+        
         # Get Client Id and Client Secret from https://dashboard.groupdocs.cloud
         my_client_id = ""
         my_client_secret = ""
         
         # Create instance of the API
         configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
         api = RewriterApi(configuration)
         
         language = "en"
         text = "GroupDocs Cloud customers come from a wide variety of industries and can be found all over the globe."
         
-        rewriter = RewriteText(language, text)
+        rewriter = RewriteText(language, text, diversity = "medium", suggestions=2)
         request = rewriter.to_string()
         res_text = api.post_rewrite_text(request)
         print(res_text.message)
         ```
         
         ### Rewrite a Word document
         
@@ -175,22 +185,23 @@
         # Create instance of the API
         configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
         api = RewriterApi(configuration)
         
         # Document paraphrasing
         language = "en"
         _format = "docx"
+        outformat = "docx"
         storage = "internal"
         name = "test_python.docx"
         folder = ""
         savepath = ""
-        savefile = "test_python.docx"  
-        masters = False
-        elements = []
-        rewriter = RewriteDocument(language, _format, storage, name, folder, savepath, savefile, masters, elements)
+        savefile = "paraphrased.docx"
+        
+        rewriter = RewriteDocument(language, _format, outformat, storage, name, folder, savepath, savefile, diversity="medium")
+        
         request = rewriter.to_string()
         res_doc = api.post_rewrite_document(request)
         print(res_doc.message)
         ```
         
         ## Other SDKs for GroupDocs.Rewriter Cloud
```

### Comparing `groupdocs-rewriter-cloud-22.8/README.md` & `groupdocs-rewriter-cloud-23.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Python SDK for GroupDocs.Rewriter Cloud
 
 ![](https://img.shields.io/badge/api-v1.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/groupdocs-rewriter-cloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/groupdocs-rewriter-cloud) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/groupdocs-rewriter-cloud) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/groupdocs-rewriter-cloud) [![GitHub license](https://img.shields.io/github/license/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python)](https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python/blob/master/LICENSE)
 
 [Product Page](https://products.groupdocs.cloud/rewriter/python/) | [Documentation](https://docs.groupdocs.cloud/rewriter/) | [Demos](https://products.groupdocs.app/rewriter/family) | [Swagger UI](https://apireference.groupdocs.cloud/rewriter/) | [Examples](https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python) | [Blog](https://blog.groupdocs.cloud/category/rewriter/) | [Search](https://search.groupdocs.cloud/) | [Free Support](https://forum.groupdocs.cloud/c/rewriter) | [Free Trial](https://purchase.groupdocs.cloud/trial)
 
-[GroupDocs.Rewriter Cloud](https://products.groupdocs.cloud/rewriter/) is an easy-to-use and versatile online service for rephrasing the content of Microsoft Word, Open Office, PDF, and plain text documents with full preservation of their meaning. A powerful neural network reads and understands the text and then paraphrases it with different wording, producing a plagiarism-free result. While the background process is very complex and resource-intensive, you do not have to worry about formulas, machine learning, and load - our cloud services do all the work by providing you with a REST API to interact with them.
+[GroupDocs.Rewriter Cloud](https://products.groupdocs.cloud/rewriter/) is an easy-to-use and versatile online service for rephrasing the content of Microsoft Word®, OpenOffice, Adobe Acrobat® PDF documents, Markdown and HTML files as well as a plain text with full preservation of their meaning. A powerful neural network reads and understands the text and then paraphrases it with different wording, producing a plagiarism-free result. While the background process is very complex and resource-intensive, you do not have to worry about formulas, machine learning, and load - our cloud services do all the work by providing you with a REST API to interact with them.
 
 This software development kit (SDK) simplifies the interaction with GroupDocs.Rewriter Cloud API from Python code, allowing you to focus on the task at hand rather than the technical details. It handles all the routine operations such as establishing connection, sending API requests, and parsing responses, wrapping all these tasks into a few lines of code that are very easy to read and maintain even for inexperienced developers.
 
 ## Before you begin
 
 GroupDocs.Rewriter Cloud is an on-demand service. As such, it has no specific hardware or operating system requirements. In order to use the service, you must create an account at GroupDocs Cloud API:
 
@@ -28,30 +28,39 @@
 GroupDocs.Rewriter Cloud can rephrase documents in the most popular formats.
 
 Document | Extensions | Description
 -------- | ---------- | -----------
 Microsoft Word | .DOCX<br />.DOCM<br />.DOC<br />.RTF | Microsoft Word 97-2021 and Microsoft 365 Word documents, including macro-enabled documents.
 Portable Document Format | .PDF | An open standard cross-platform format for documents that include formatted text, images, multimedia elements, and more.
 OpenDocument Text | .ODT | Documents created with a number of open source word processing applications, such as Writer from Apache OpenOffice and LibreOffice.
+Markdown | .MD | Files created using one of dialects of the Markdown language.
+HTML | .HTML | Files containing Hypertext Markup Language (HTML) that formats the structure of a webpage. 
 Plain text | .TXT | Plain text files or text in the form of lines.
 
 In addition to rephrasing, GroupDocs.Rewriter Cloud can save the resulting document in various file formats other than the original, with formatting preserved (where applicable).
 
 Source file format | Paraphrased file format
 ------------------ | ----------------------
 .DOCX              | .DOCX<br />.RTF<br />.HTML<br />.ODT<br />.TXT<br />.MD<br />.PDF<br />.TIFF<br />.SVG<br />.XPS
 .DOC               | .DOC<br />.DOCX<br />.RTF<br />.HTML<br />.ODT<br />.TXT<br />.MD<br />.PDF<br />.TIFF<br />.SVG<br />.XPS
 .ODT               | .DOCX<br />.RTF<br />.HTML<br />.ODT<br />.TXT<br />.MD<br />.PDF<br />.TIFF<br />.SVG<br />.XPS
 .RTF               | .DOCX<br />.RTF<br />.HTML<br />.ODT<br />.TXT<br />.MD<br />.PDF<br />.TIFF<br />.SVG<br />.XPS
-.PDF               | .DOCX<br />.PPTX<br />.HTML<br />.XPS<br />.SVG
+.PDF               | .PDF<br />.DOCX<br />.PPTX<br />.HTML<br />.XPS<br />.SVG
+.MD                | .MD<br />
+.HTML              | .HTML<br />.PDF<br />.DOCX<br />.TIFF<br />.XPS<br />
 
 ## Supported languages
 
+- **ar** — to paraphrase Arabic text or document
+— **de** — to paraphrase German text or document
 - **en** — to paraphrase English text or document
+— **fr** — to paraphrase French text or document
+— **id** — to paraphrase Indonesian text or document
 - **ru** — to paraphrase Russian text or document
+- **uk** — to paraphrase Ukrainian text or document
 
 ## Quick start
 
 To start using GroupDocs.Rewriter Cloud in your Python applications, follow a few simple steps:
 
 ## System requirements
 
@@ -134,26 +143,27 @@
 The following code snippets demonstrate how to use the GroupDocs.Rewriter Python SDK to accomplish various tasks.
 
 ### Rewrite a text
 
 ```python
 # Load the gem
 import groupdocs_rewriter_cloud
+
 # Get Client Id and Client Secret from https://dashboard.groupdocs.cloud
 my_client_id = ""
 my_client_secret = ""
 
 # Create instance of the API
 configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
 api = RewriterApi(configuration)
 
 language = "en"
 text = "GroupDocs Cloud customers come from a wide variety of industries and can be found all over the globe."
 
-rewriter = RewriteText(language, text)
+rewriter = RewriteText(language, text, diversity = "medium", suggestions=2)
 request = rewriter.to_string()
 res_text = api.post_rewrite_text(request)
 print(res_text.message)
 ```
 
 ### Rewrite a Word document
 
@@ -167,22 +177,23 @@
 # Create instance of the API
 configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
 api = RewriterApi(configuration)
 
 # Document paraphrasing
 language = "en"
 _format = "docx"
+outformat = "docx"
 storage = "internal"
 name = "test_python.docx"
 folder = ""
 savepath = ""
-savefile = "test_python.docx"  
-masters = False
-elements = []
-rewriter = RewriteDocument(language, _format, storage, name, folder, savepath, savefile, masters, elements)
+savefile = "paraphrased.docx"
+
+rewriter = RewriteDocument(language, _format, outformat, storage, name, folder, savepath, savefile, diversity="medium")
+
 request = rewriter.to_string()
 res_doc = api.post_rewrite_document(request)
 print(res_doc.message)
 ```
 
 ## Other SDKs for GroupDocs.Rewriter Cloud
```

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocs_rewriter_cloud.egg-info/PKG-INFO` & `groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: groupdocs-rewriter-cloud
-Version: 22.8
+Version: 23.4
 Summary: GroupDocs.Rewriter Cloud SDK
 Home-page: https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python
 Author: Aspose
 Author-email: ekaterina.tretiak@aspose.com
 License: MIT
 Description: # Python SDK for GroupDocs.Rewriter Cloud
         
         ![](https://img.shields.io/badge/api-v1.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/groupdocs-rewriter-cloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/groupdocs-rewriter-cloud) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/groupdocs-rewriter-cloud) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/groupdocs-rewriter-cloud) [![GitHub license](https://img.shields.io/github/license/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python)](https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python/blob/master/LICENSE)
         
         [Product Page](https://products.groupdocs.cloud/rewriter/python/) | [Documentation](https://docs.groupdocs.cloud/rewriter/) | [Demos](https://products.groupdocs.app/rewriter/family) | [Swagger UI](https://apireference.groupdocs.cloud/rewriter/) | [Examples](https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python) | [Blog](https://blog.groupdocs.cloud/category/rewriter/) | [Search](https://search.groupdocs.cloud/) | [Free Support](https://forum.groupdocs.cloud/c/rewriter) | [Free Trial](https://purchase.groupdocs.cloud/trial)
         
-        [GroupDocs.Rewriter Cloud](https://products.groupdocs.cloud/rewriter/) is an easy-to-use and versatile online service for rephrasing the content of Microsoft Word, Open Office, PDF, and plain text documents with full preservation of their meaning. A powerful neural network reads and understands the text and then paraphrases it with different wording, producing a plagiarism-free result. While the background process is very complex and resource-intensive, you do not have to worry about formulas, machine learning, and load - our cloud services do all the work by providing you with a REST API to interact with them.
+        [GroupDocs.Rewriter Cloud](https://products.groupdocs.cloud/rewriter/) is an easy-to-use and versatile online service for rephrasing the content of Microsoft Word®, OpenOffice, Adobe Acrobat® PDF documents, Markdown and HTML files as well as a plain text with full preservation of their meaning. A powerful neural network reads and understands the text and then paraphrases it with different wording, producing a plagiarism-free result. While the background process is very complex and resource-intensive, you do not have to worry about formulas, machine learning, and load - our cloud services do all the work by providing you with a REST API to interact with them.
         
         This software development kit (SDK) simplifies the interaction with GroupDocs.Rewriter Cloud API from Python code, allowing you to focus on the task at hand rather than the technical details. It handles all the routine operations such as establishing connection, sending API requests, and parsing responses, wrapping all these tasks into a few lines of code that are very easy to read and maintain even for inexperienced developers.
         
         ## Before you begin
         
         GroupDocs.Rewriter Cloud is an on-demand service. As such, it has no specific hardware or operating system requirements. In order to use the service, you must create an account at GroupDocs Cloud API:
         
@@ -36,30 +36,39 @@
         GroupDocs.Rewriter Cloud can rephrase documents in the most popular formats.
         
         Document | Extensions | Description
         -------- | ---------- | -----------
         Microsoft Word | .DOCX<br />.DOCM<br />.DOC<br />.RTF | Microsoft Word 97-2021 and Microsoft 365 Word documents, including macro-enabled documents.
         Portable Document Format | .PDF | An open standard cross-platform format for documents that include formatted text, images, multimedia elements, and more.
         OpenDocument Text | .ODT | Documents created with a number of open source word processing applications, such as Writer from Apache OpenOffice and LibreOffice.
+        Markdown | .MD | Files created using one of dialects of the Markdown language.
+        HTML | .HTML | Files containing Hypertext Markup Language (HTML) that formats the structure of a webpage. 
         Plain text | .TXT | Plain text files or text in the form of lines.
         
         In addition to rephrasing, GroupDocs.Rewriter Cloud can save the resulting document in various file formats other than the original, with formatting preserved (where applicable).
         
         Source file format | Paraphrased file format
         ------------------ | ----------------------
         .DOCX              | .DOCX<br />.RTF<br />.HTML<br />.ODT<br />.TXT<br />.MD<br />.PDF<br />.TIFF<br />.SVG<br />.XPS
         .DOC               | .DOC<br />.DOCX<br />.RTF<br />.HTML<br />.ODT<br />.TXT<br />.MD<br />.PDF<br />.TIFF<br />.SVG<br />.XPS
         .ODT               | .DOCX<br />.RTF<br />.HTML<br />.ODT<br />.TXT<br />.MD<br />.PDF<br />.TIFF<br />.SVG<br />.XPS
         .RTF               | .DOCX<br />.RTF<br />.HTML<br />.ODT<br />.TXT<br />.MD<br />.PDF<br />.TIFF<br />.SVG<br />.XPS
-        .PDF               | .DOCX<br />.PPTX<br />.HTML<br />.XPS<br />.SVG
+        .PDF               | .PDF<br />.DOCX<br />.PPTX<br />.HTML<br />.XPS<br />.SVG
+        .MD                | .MD<br />
+        .HTML              | .HTML<br />.PDF<br />.DOCX<br />.TIFF<br />.XPS<br />
         
         ## Supported languages
         
+        - **ar** — to paraphrase Arabic text or document
+        — **de** — to paraphrase German text or document
         - **en** — to paraphrase English text or document
+        — **fr** — to paraphrase French text or document
+        — **id** — to paraphrase Indonesian text or document
         - **ru** — to paraphrase Russian text or document
+        - **uk** — to paraphrase Ukrainian text or document
         
         ## Quick start
         
         To start using GroupDocs.Rewriter Cloud in your Python applications, follow a few simple steps:
         
         ## System requirements
         
@@ -142,26 +151,27 @@
         The following code snippets demonstrate how to use the GroupDocs.Rewriter Python SDK to accomplish various tasks.
         
         ### Rewrite a text
         
         ```python
         # Load the gem
         import groupdocs_rewriter_cloud
+        
         # Get Client Id and Client Secret from https://dashboard.groupdocs.cloud
         my_client_id = ""
         my_client_secret = ""
         
         # Create instance of the API
         configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
         api = RewriterApi(configuration)
         
         language = "en"
         text = "GroupDocs Cloud customers come from a wide variety of industries and can be found all over the globe."
         
-        rewriter = RewriteText(language, text)
+        rewriter = RewriteText(language, text, diversity = "medium", suggestions=2)
         request = rewriter.to_string()
         res_text = api.post_rewrite_text(request)
         print(res_text.message)
         ```
         
         ### Rewrite a Word document
         
@@ -175,22 +185,23 @@
         # Create instance of the API
         configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
         api = RewriterApi(configuration)
         
         # Document paraphrasing
         language = "en"
         _format = "docx"
+        outformat = "docx"
         storage = "internal"
         name = "test_python.docx"
         folder = ""
         savepath = ""
-        savefile = "test_python.docx"  
-        masters = False
-        elements = []
-        rewriter = RewriteDocument(language, _format, storage, name, folder, savepath, savefile, masters, elements)
+        savefile = "paraphrased.docx"
+        
+        rewriter = RewriteDocument(language, _format, outformat, storage, name, folder, savepath, savefile, diversity="medium")
+        
         request = rewriter.to_string()
         res_doc = api.post_rewrite_document(request)
         print(res_doc.message)
         ```
         
         ## Other SDKs for GroupDocs.Rewriter Cloud
```

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocs_rewriter_cloud.egg-info/SOURCES.txt` & `groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/__init__.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/api/__init__.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/api/rewriter_api.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/rewriter_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/api/storage_api.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/storage_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/api_client.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api_client.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/configuration.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/configuration.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/__init__.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/base_model.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/base_model.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/disc_usage.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/document_response.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/document_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,22 +43,24 @@
     }
 
     attribute_map = {
         'status': 'status',
         'message': 'message'
     }
 
-    def __init__(self, status="", message="", paraphrase=""):
+    def __init__(self, status="", message="", result=""):
         """
 
         :type status: str
         :type message: str
+        :type result: str
         """
         self._status = status  # type: str
         self._message = message  # type: str
+        self._result = result # type: str
 
     @property
     def status(self):
         """Operation status
         :return: status.
         :type: str
         """
@@ -81,15 +83,34 @@
         :return: message.
         :type: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets rersponse message.
+        """Sets response message.
         :param message: message.
         :type: str
         """
         if message is None:
             raise ValueError("Invalid value for `message`, must not be `None`")
 
         self._message = message
+
+    @property
+    def result(self):
+        """Gets response result
+        :return: result.
+        :type: str
+        """
+        return self._result
+
+    @result.setter
+    def result(self, result):
+        """Sets response result.
+        :param result: result.
+        :type: str
+        """
+        if result is None:
+            raise ValueError("Invalid value for `result`, must not be `None`")
+
+        self._result = result
```

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/error.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/error.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/error_details.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/file_version.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/file_versions.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/files_list.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/files_upload_result.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/object_exist.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/rewrite_document.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/rewrite_document.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,29 +44,31 @@
         'Language': 'str',
         'Format': 'str',
         'Outformat': 'str',
         'Storage': 'str',
         'Name': 'str',
         'Folder': 'str',
         'Savepath': 'str',
-        'Savefile': 'str'
+        'Savefile': 'str',
+        'Diversity': 'str'
     }
 
     attribute_map = {
         'Language': 'language',
         'Format': 'format',
         'Outformat': 'outformat',
         'Storage': 'storage',
         'Name': 'name',
         'Folder': 'folder',
         'Savepath': 'savepath',
-        'Savefile': 'savefile'
+        'Savefile': 'savefile',
+        'Diversity': 'diversity'
     }
 
-    def __init__(self, language, _format, outformat, storage, name, folder, savepath, savefile):
+    def __init__(self, language, _format, outformat, storage, name, folder, savepath, savefile, diversity="off"):
         """
         :param str Language: language of document
         :param str Format: format of file for rewriting, put file extension here
         :param str Outformat: format of paraphrased file, put file extension of desired format here
         :param str Storage: name of storage
         :param str Name: name of file to rewrite
         :param str Folder: folder(s) where file is saved
@@ -77,12 +79,14 @@
         self.Format = _format
         self.Outformat = outformat
         self.Storage = storage
         self.Name = name
         self.Folder = folder
         self.Savepath = savepath
         self.Savefile = savefile
+        self.Diversity = diversity
 
     def to_string(self):
-        request = [{"language": self.Language, "format": self.Format, "outformat": self.Outformat, "storage": self.Storage,
-                    "name": self.Name, "folder": self.Folder, "savepath": self.Savepath, "savefile": self.Savefile}]
+        request = [{"language": self.Language, "format": self.Format, "outformat": self.Outformat,
+                    "storage": self.Storage, "name": self.Name, "folder": self.Folder, "savepath": self.Savepath,
+                    "savefile": self.Savefile, "diversity": self.Diversity}]
         return  json.dumps(request)
```

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/rewrite_text.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/rewrite_text.py`

 * *Files 20% similar despite different names*

```diff
@@ -39,28 +39,38 @@
                                 and the value is attribute type.
           attribute_map (dict): The key is attribute name
                                 and the value is json key in definition.
         """
     model_types = {
         'Language': 'str',
         'Text': 'str',
-        'Tokenize': bool
+        'Tokenize': bool,
+        'Diversity': 'str',
+        'Suggestions': int
     }
 
     attribute_map = {
         'Language': 'language',
         'Text': 'text',
-        'Tokenize': 'tokenize'
+        'Tokenize': 'tokenize',
+        'Diversity': 'diversity',
+        'Suggestions': 'suggestions'
     }
 
-    def __init__(self, language, text, tokenize=False):
+    def __init__(self, language, text, tokenize=False, diversity="off", suggestions=1):
         """
         :param str language: language of text
         :param str text: text to paraphrase
+        :param bool tokenize: to tokenize input and output texts
+        :param str diversity: diversity level of output text
+        :param int suggestions: number of paraphrasing variants returned
         """
-        self.Language = language        # language of text
-        self.Text = text            # text to paraphrase
-        self.Tokenize = tokenize    # tokenization mode
+        self.Language = language  # language of text
+        self.Text = text  # text to paraphrase
+        self.Tokenize = tokenize  # tokenization mode
+        self.Diversity = diversity  # diversity of paraphrasing, "medium" or "high", default is "off"
+        self.Suggestions = suggestions  # number of suggested variants, 3 maximum
 
     def to_string(self):
-        request = [{"language": self.Language, "text": self.Text, "tokenize": self.Tokenize}]
+        request = [{"language": self.Language, "text": self.Text, "tokenize": self.Tokenize,
+                    "diversity": self.Diversity, "suggestions": self.Suggestions}]
         return json.dumps(request)
```

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/storage_exist.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/storage_file.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/models/text_response.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/text_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,36 +37,41 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     model_types = {
         'status': 'str',
         'message': 'str',
         'result': 'str',
+        'results': 'list[str]',
         'sourcelist': 'list[str]',
         'targetlist': 'list[str]'
     }
 
     attribute_map = {
         'status': 'status',
         'message': 'message',
         'result': 'result',
+        'results': 'results',
         'sourcelist': 'sourcelist',
         'targetlist': 'targetlist'
     }
 
-    def __init__(self, status="", message="", result="", sourcelist=[], targetlist=[]):
+    def __init__(self, status="", message="", result="", results=[], sourcelist=[], targetlist=[]):
         """
-
         :type status: str
         :type message: str
         :type result: str
+        :type results: list
+        :type sourcelist: list
+        :type targetlist: list
         """
         self._status = status  # type: str
         self._message = message  # type: str
         self._result = result # type: str
+        self._results = results # type: list
         self._sourcelist = sourcelist # type: list
         self._targetlist = targetlist # type: list
 
     @property
     def status(self):
         """Operation status
         :return: status.
@@ -107,20 +112,20 @@
     @property
     def result(self):
         """
         Gets paraphrased text
         :return: paraphrased text
         :type: str
         """
-        return self._result, self._sourcelist, self._targetlist
+        return self._result, self._results, self._sourcelist, self._targetlist
 
     @result.setter
     def result(self, result):
         """
         Sets paraphrased text
-        :param paraphrase: paraphrased text
+        :param result: paraphrased text
         :type: str
         """
         if result is None:
-            raise ValueError("Invalid value for `paraphrase`, must not be `None`")
+            raise ValueError("Invalid value for `result`, must not be `None`")
         self._result = result
```

### Comparing `groupdocs-rewriter-cloud-22.8/groupdocsrewritercloud/rest.py` & `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/rest.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/setup.py` & `groupdocs-rewriter-cloud-23.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages
 from os import path
 
 NAME = "groupdocs-rewriter-cloud"
-VERSION = "22.8"
+VERSION = "23.4"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -58,12 +58,12 @@
     packages=find_packages(),
     include_package_data=True
     # long_description="""
     # GroupDocs.Rewriter Cloud API Reference
     # This package contains GroupDocs.Rewriter Cloud SDK for Python.
     # This SDK allows you to work with GroupDocs.Rewriter Cloud REST APIs in your Python applications, and integrate Rewriter functionality in few steps.
     #
-    # In detail, it's a set of SDKs for plain text and document rewriting in our Cloud. It supports paraphrasing of Word and PDF documents. Just pass text or parameteres of document uploaded to our Cloud Storage, to the GroupDocs.Rewriter Cloud API, and it will return paraphrased text or will save paraphrased file in Cloud Storage usinng specified path and name.
+    # In detail, it's a set of SDKs for plain text and document rewriting in our Cloud. It supports paraphrasing of Microsoft Word or Open Office documents, Adobe PDF documents, Markdown files, HTML files and plain text. Just pass text or parameteres of document uploaded to our Cloud Storage, to the GroupDocs.Rewriter Cloud API, and it will return paraphrased text or will save paraphrased file in Cloud Storage using specified path and name.
     #
-    # It is easy to get started with GroupDocs.Rewriter Cloud, and there is nothing to install locally or configure servers. Create an account at GrroupDocs Cloud and get your application KEY, import this python, module, initialize "Configuration. class with this keys, and then you are ready to use the API.
+    # It is easy to get started with GroupDocs.Rewriter Cloud, and there is nothing to install locally or configure servers. Create an account at GroupDocs Cloud and get your application KEY, import this python, module, initialize "Configuration. class with this keys, and then you are ready to use the API.
     # """
-)
+)
```

### Comparing `groupdocs-rewriter-cloud-22.8/test/__init__.py` & `groupdocs-rewriter-cloud-23.4/test/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/test/test_helper.py` & `groupdocs-rewriter-cloud-23.4/test/test_helper.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/test/test_rewriter_api.py` & `groupdocs-rewriter-cloud-23.4/test/test_rewriter_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-rewriter-cloud-22.8/test/test_storage_api.py` & `groupdocs-rewriter-cloud-23.4/test/test_storage_api.py`

 * *Files identical despite different names*

