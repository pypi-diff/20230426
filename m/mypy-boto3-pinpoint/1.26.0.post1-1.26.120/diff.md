# Comparing `tmp/mypy-boto3-pinpoint-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-pinpoint-1.26.120.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:50 2022, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-1.26.120.tar", last modified: Tue Apr 25 21:20:46 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-1.26.0.post1.tar` & `mypy-boto3-pinpoint-1.26.120.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:50.348841 mypy-boto3-pinpoint-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:39:08.000000 mypy-boto3-pinpoint-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    28486 2022-11-01 21:43:50.348841 mypy-boto3-pinpoint-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    27041 2022-11-01 21:39:08.000000 mypy-boto3-pinpoint-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:50.348841 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-11-01 21:39:08.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-11-01 21:39:08.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-01 21:39:08.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    77565 2022-11-01 21:39:08.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    77440 2022-11-01 21:39:08.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9882 2022-11-01 21:39:08.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9880 2022-11-01 21:39:08.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:39:08.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)   154277 2022-11-01 21:39:13.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)   154068 2022-11-01 21:39:10.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:39:08.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:50.348841 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    28486 2022-11-01 21:43:50.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-01 21:43:50.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:50.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:50.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:50.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-01 21:43:50.000000 mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:50.348841 mypy-boto3-pinpoint-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2022-11-01 21:39:08.000000 mypy-boto3-pinpoint-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:20:46.074512 mypy-boto3-pinpoint-1.26.120/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-04-25 21:20:46.074512 mypy-boto3-pinpoint-1.26.120/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:20:46.074512 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79752 2023-04-25 21:20:32.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79624 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-04-25 21:20:32.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-04-25 21:20:32.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   159068 2023-04-25 21:20:36.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158851 2023-04-25 21:20:34.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:20:46.074512 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29010 2023-04-25 21:20:45.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-25 21:20:45.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:20:45.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:20:45.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 21:20:45.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 21:20:45.000000 mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 21:20:46.074512 mypy-boto3-pinpoint-1.26.120/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-25 21:20:31.000000 mypy-boto3-pinpoint-1.26.120/setup.py
```

### Comparing `mypy-boto3-pinpoint-1.26.0.post1/LICENSE` & `mypy-boto3-pinpoint-1.26.120/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-pinpoint-1.26.0.post1/PKG-INFO` & `mypy-boto3-pinpoint-1.26.120/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Pinpoint 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.120
+Summary: Type annotations for boto3.Pinpoint 1.26.120 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-pinpoint"></a>
 
 # mypy-boto3-pinpoint
 
 [![PyPI - mypy-boto3-pinpoint](https://img.shields.io/pypi/v/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.26.120](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,14 +291,15 @@
     DurationType,
     EndpointTypesElementType,
     FilterTypeType,
     FormatType,
     FrequencyType,
     IncludeType,
     JobStatusType,
+    JourneyRunStatusType,
     LayoutType,
     MessageTypeType,
     ModeType,
     OperatorType,
     RecencyTypeType,
     SegmentTypeType,
     SourceTypeType,
@@ -356,15 +358,14 @@
     CampaignStateTypeDef,
     CustomDeliveryConfigurationTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
     ClosedDaysRuleTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
-    ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
@@ -407,14 +408,15 @@
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
     EndpointItemResponseTypeDef,
     EndpointMessageResultTypeDef,
     EndpointSendConfigurationTypeDef,
     MetricDimensionTypeDef,
@@ -454,14 +456,19 @@
     GetInAppTemplateRequestRequestTypeDef,
     GetJourneyDateRangeKpiRequestRequestTypeDef,
     GetJourneyExecutionActivityMetricsRequestRequestTypeDef,
     JourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsRequestRequestTypeDef,
     JourneyExecutionMetricsResponseTypeDef,
     GetJourneyRequestRequestTypeDef,
+    GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
+    JourneyRunExecutionActivityMetricsResponseTypeDef,
+    GetJourneyRunExecutionMetricsRequestRequestTypeDef,
+    JourneyRunExecutionMetricsResponseTypeDef,
+    GetJourneyRunsRequestRequestTypeDef,
     GetPushTemplateRequestRequestTypeDef,
     GetRecommenderConfigurationRequestRequestTypeDef,
     GetRecommenderConfigurationsRequestRequestTypeDef,
     GetSegmentExportJobsRequestRequestTypeDef,
     GetSegmentImportJobsRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     GetSegmentVersionRequestRequestTypeDef,
@@ -478,14 +485,15 @@
     InAppMessageBodyConfigTypeDef,
     OverrideButtonConfigurationTypeDef,
     InAppMessageHeaderConfigTypeDef,
     JourneyChannelSettingsTypeDef,
     JourneyLimitsTypeDef,
     JourneyPushMessageTypeDef,
     JourneyScheduleTypeDef,
+    JourneyRunResponseTypeDef,
     JourneySMSMessageTypeDef,
     JourneyStateRequestTypeDef,
     ListJourneysRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagsModelTypeDef,
     ListTemplateVersionsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
@@ -494,14 +502,15 @@
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
     RandomSplitEntryTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
+    ResponseMetadataTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
     SegmentConditionTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
@@ -511,50 +520,49 @@
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
     VerifyOTPMessageRequestParametersTypeDef,
     UpdateAdmChannelRequestRequestTypeDef,
+    DeleteAdmChannelResponseTypeDef,
+    GetAdmChannelResponseTypeDef,
+    UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
+    DeleteApnsChannelResponseTypeDef,
+    GetApnsChannelResponseTypeDef,
+    UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
+    DeleteApnsSandboxChannelResponseTypeDef,
+    GetApnsSandboxChannelResponseTypeDef,
+    UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
+    DeleteApnsVoipChannelResponseTypeDef,
+    GetApnsVoipChannelResponseTypeDef,
+    UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
+    DeleteApnsVoipSandboxChannelResponseTypeDef,
+    GetApnsVoipSandboxChannelResponseTypeDef,
+    UpdateApnsVoipSandboxChannelResponseTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
+    CreateAppResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    GetAppResponseTypeDef,
     ApplicationSettingsResourceTypeDef,
     WriteApplicationSettingsRequestTypeDef,
+    RemoveAttributesResponseTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
+    DeleteBaiduChannelResponseTypeDef,
+    GetBaiduChannelResponseTypeDef,
+    UpdateBaiduChannelResponseTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
-    CreateAppResponseTypeDef,
-    DeleteAdmChannelResponseTypeDef,
-    DeleteApnsChannelResponseTypeDef,
-    DeleteApnsSandboxChannelResponseTypeDef,
-    DeleteApnsVoipChannelResponseTypeDef,
-    DeleteApnsVoipSandboxChannelResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    DeleteBaiduChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAdmChannelResponseTypeDef,
-    GetApnsChannelResponseTypeDef,
-    GetApnsSandboxChannelResponseTypeDef,
-    GetApnsVoipChannelResponseTypeDef,
-    GetApnsVoipSandboxChannelResponseTypeDef,
-    GetAppResponseTypeDef,
-    GetBaiduChannelResponseTypeDef,
-    RemoveAttributesResponseTypeDef,
-    UpdateAdmChannelResponseTypeDef,
-    UpdateApnsChannelResponseTypeDef,
-    UpdateApnsSandboxChannelResponseTypeDef,
-    UpdateApnsVoipChannelResponseTypeDef,
-    UpdateApnsVoipSandboxChannelResponseTypeDef,
-    UpdateBaiduChannelResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     CreateEmailTemplateResponseTypeDef,
     CreatePushTemplateResponseTypeDef,
     CreateSmsTemplateResponseTypeDef,
     CreateVoiceTemplateResponseTypeDef,
     CreateExportJobRequestRequestTypeDef,
@@ -614,19 +622,22 @@
     ItemResponseTypeDef,
     EventTypeDef,
     ExportJobResponseTypeDef,
     UpdateGcmChannelRequestRequestTypeDef,
     GPSPointDimensionTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
+    GetJourneyRunExecutionActivityMetricsResponseTypeDef,
+    GetJourneyRunExecutionMetricsResponseTypeDef,
     GetSmsTemplateResponseTypeDef,
     GetVoiceTemplateResponseTypeDef,
     ImportJobResponseTypeDef,
     InAppMessageButtonTypeDef,
     PushMessageActivityTypeDef,
+    JourneyRunsResponseTypeDef,
     SMSMessageActivityTypeDef,
     UpdateJourneyStateRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     MessageResponseTypeDef,
     PhoneNumberValidateRequestRequestTypeDef,
     PhoneNumberValidateResponseTypeDef,
@@ -672,14 +683,15 @@
     ExportJobsResponseTypeDef,
     GetExportJobResponseTypeDef,
     SegmentLocationTypeDef,
     CreateImportJobResponseTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobsResponseTypeDef,
     InAppMessageContentTypeDef,
+    GetJourneyRunsResponseTypeDef,
     SendMessagesResponseTypeDef,
     SendOTPMessageResponseTypeDef,
     BaseKpiResultTypeDef,
     EmailMessageTypeDef,
     ListTemplatesResponseTypeDef,
     ListTemplateVersionsResponseTypeDef,
     UpdateEndpointsBatchRequestRequestTypeDef,
@@ -774,42 +786,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-pinpoint-1.26.0.post1/README.md` & `mypy-boto3-pinpoint-1.26.120/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-pinpoint"></a>
 
 # mypy-boto3-pinpoint
 
 [![PyPI - mypy-boto3-pinpoint](https://img.shields.io/pypi/v/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.26.120](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
 
@@ -259,14 +259,15 @@
     DurationType,
     EndpointTypesElementType,
     FilterTypeType,
     FormatType,
     FrequencyType,
     IncludeType,
     JobStatusType,
+    JourneyRunStatusType,
     LayoutType,
     MessageTypeType,
     ModeType,
     OperatorType,
     RecencyTypeType,
     SegmentTypeType,
     SourceTypeType,
@@ -325,15 +326,14 @@
     CampaignStateTypeDef,
     CustomDeliveryConfigurationTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
     ClosedDaysRuleTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
-    ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
@@ -376,14 +376,15 @@
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
     EndpointItemResponseTypeDef,
     EndpointMessageResultTypeDef,
     EndpointSendConfigurationTypeDef,
     MetricDimensionTypeDef,
@@ -423,14 +424,19 @@
     GetInAppTemplateRequestRequestTypeDef,
     GetJourneyDateRangeKpiRequestRequestTypeDef,
     GetJourneyExecutionActivityMetricsRequestRequestTypeDef,
     JourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsRequestRequestTypeDef,
     JourneyExecutionMetricsResponseTypeDef,
     GetJourneyRequestRequestTypeDef,
+    GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
+    JourneyRunExecutionActivityMetricsResponseTypeDef,
+    GetJourneyRunExecutionMetricsRequestRequestTypeDef,
+    JourneyRunExecutionMetricsResponseTypeDef,
+    GetJourneyRunsRequestRequestTypeDef,
     GetPushTemplateRequestRequestTypeDef,
     GetRecommenderConfigurationRequestRequestTypeDef,
     GetRecommenderConfigurationsRequestRequestTypeDef,
     GetSegmentExportJobsRequestRequestTypeDef,
     GetSegmentImportJobsRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     GetSegmentVersionRequestRequestTypeDef,
@@ -447,14 +453,15 @@
     InAppMessageBodyConfigTypeDef,
     OverrideButtonConfigurationTypeDef,
     InAppMessageHeaderConfigTypeDef,
     JourneyChannelSettingsTypeDef,
     JourneyLimitsTypeDef,
     JourneyPushMessageTypeDef,
     JourneyScheduleTypeDef,
+    JourneyRunResponseTypeDef,
     JourneySMSMessageTypeDef,
     JourneyStateRequestTypeDef,
     ListJourneysRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagsModelTypeDef,
     ListTemplateVersionsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
@@ -463,14 +470,15 @@
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
     RandomSplitEntryTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
+    ResponseMetadataTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
     SegmentConditionTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
@@ -480,50 +488,49 @@
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
     VerifyOTPMessageRequestParametersTypeDef,
     UpdateAdmChannelRequestRequestTypeDef,
+    DeleteAdmChannelResponseTypeDef,
+    GetAdmChannelResponseTypeDef,
+    UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
+    DeleteApnsChannelResponseTypeDef,
+    GetApnsChannelResponseTypeDef,
+    UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
+    DeleteApnsSandboxChannelResponseTypeDef,
+    GetApnsSandboxChannelResponseTypeDef,
+    UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
+    DeleteApnsVoipChannelResponseTypeDef,
+    GetApnsVoipChannelResponseTypeDef,
+    UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
+    DeleteApnsVoipSandboxChannelResponseTypeDef,
+    GetApnsVoipSandboxChannelResponseTypeDef,
+    UpdateApnsVoipSandboxChannelResponseTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
+    CreateAppResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    GetAppResponseTypeDef,
     ApplicationSettingsResourceTypeDef,
     WriteApplicationSettingsRequestTypeDef,
+    RemoveAttributesResponseTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
+    DeleteBaiduChannelResponseTypeDef,
+    GetBaiduChannelResponseTypeDef,
+    UpdateBaiduChannelResponseTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
-    CreateAppResponseTypeDef,
-    DeleteAdmChannelResponseTypeDef,
-    DeleteApnsChannelResponseTypeDef,
-    DeleteApnsSandboxChannelResponseTypeDef,
-    DeleteApnsVoipChannelResponseTypeDef,
-    DeleteApnsVoipSandboxChannelResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    DeleteBaiduChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAdmChannelResponseTypeDef,
-    GetApnsChannelResponseTypeDef,
-    GetApnsSandboxChannelResponseTypeDef,
-    GetApnsVoipChannelResponseTypeDef,
-    GetApnsVoipSandboxChannelResponseTypeDef,
-    GetAppResponseTypeDef,
-    GetBaiduChannelResponseTypeDef,
-    RemoveAttributesResponseTypeDef,
-    UpdateAdmChannelResponseTypeDef,
-    UpdateApnsChannelResponseTypeDef,
-    UpdateApnsSandboxChannelResponseTypeDef,
-    UpdateApnsVoipChannelResponseTypeDef,
-    UpdateApnsVoipSandboxChannelResponseTypeDef,
-    UpdateBaiduChannelResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     CreateEmailTemplateResponseTypeDef,
     CreatePushTemplateResponseTypeDef,
     CreateSmsTemplateResponseTypeDef,
     CreateVoiceTemplateResponseTypeDef,
     CreateExportJobRequestRequestTypeDef,
@@ -583,19 +590,22 @@
     ItemResponseTypeDef,
     EventTypeDef,
     ExportJobResponseTypeDef,
     UpdateGcmChannelRequestRequestTypeDef,
     GPSPointDimensionTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
+    GetJourneyRunExecutionActivityMetricsResponseTypeDef,
+    GetJourneyRunExecutionMetricsResponseTypeDef,
     GetSmsTemplateResponseTypeDef,
     GetVoiceTemplateResponseTypeDef,
     ImportJobResponseTypeDef,
     InAppMessageButtonTypeDef,
     PushMessageActivityTypeDef,
+    JourneyRunsResponseTypeDef,
     SMSMessageActivityTypeDef,
     UpdateJourneyStateRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     MessageResponseTypeDef,
     PhoneNumberValidateRequestRequestTypeDef,
     PhoneNumberValidateResponseTypeDef,
@@ -641,14 +651,15 @@
     ExportJobsResponseTypeDef,
     GetExportJobResponseTypeDef,
     SegmentLocationTypeDef,
     CreateImportJobResponseTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobsResponseTypeDef,
     InAppMessageContentTypeDef,
+    GetJourneyRunsResponseTypeDef,
     SendMessagesResponseTypeDef,
     SendOTPMessageResponseTypeDef,
     BaseKpiResultTypeDef,
     EmailMessageTypeDef,
     ListTemplatesResponseTypeDef,
     ListTemplateVersionsResponseTypeDef,
     UpdateEndpointsBatchRequestRequestTypeDef,
@@ -743,42 +754,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/client.py` & `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,17 @@
     GetImportJobsResponseTypeDef,
     GetInAppMessagesResponseTypeDef,
     GetInAppTemplateResponseTypeDef,
     GetJourneyDateRangeKpiResponseTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
     GetJourneyResponseTypeDef,
+    GetJourneyRunExecutionActivityMetricsResponseTypeDef,
+    GetJourneyRunExecutionMetricsResponseTypeDef,
+    GetJourneyRunsResponseTypeDef,
     GetPushTemplateResponseTypeDef,
     GetRecommenderConfigurationResponseTypeDef,
     GetRecommenderConfigurationsResponseTypeDef,
     GetSegmentExportJobsResponseTypeDef,
     GetSegmentImportJobsResponseTypeDef,
     GetSegmentResponseTypeDef,
     GetSegmentsResponseTypeDef,
@@ -936,14 +939,59 @@
         Retrieves (queries) pre-aggregated data for a standard execution metric that
         applies to a journey.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_execution_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_journey_execution_metrics)
         """
 
+    def get_journey_run_execution_activity_metrics(
+        self,
+        *,
+        ApplicationId: str,
+        JourneyActivityId: str,
+        JourneyId: str,
+        RunId: str,
+        NextToken: str = ...,
+        PageSize: str = ...
+    ) -> GetJourneyRunExecutionActivityMetricsResponseTypeDef:
+        """
+        Retrieves (queries) pre-aggregated data for a standard run execution metric that
+        applies to a journey activity.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_run_execution_activity_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_journey_run_execution_activity_metrics)
+        """
+
+    def get_journey_run_execution_metrics(
+        self,
+        *,
+        ApplicationId: str,
+        JourneyId: str,
+        RunId: str,
+        NextToken: str = ...,
+        PageSize: str = ...
+    ) -> GetJourneyRunExecutionMetricsResponseTypeDef:
+        """
+        Retrieves (queries) pre-aggregated data for a standard run execution metric that
+        applies to a journey.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_run_execution_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_journey_run_execution_metrics)
+        """
+
+    def get_journey_runs(
+        self, *, ApplicationId: str, JourneyId: str, PageSize: str = ..., Token: str = ...
+    ) -> GetJourneyRunsResponseTypeDef:
+        """
+        Provides information about the runs of a journey.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_runs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_journey_runs)
+        """
+
     def get_push_template(
         self, *, TemplateName: str, Version: str = ...
     ) -> GetPushTemplateResponseTypeDef:
         """
         Retrieves the content and settings of a message template for messages that are
         sent through a push notification channel.
 
@@ -1501,15 +1549,15 @@
         self,
         *,
         TemplateActiveVersionRequest: TemplateActiveVersionRequestTypeDef,
         TemplateName: str,
         TemplateType: str
     ) -> UpdateTemplateActiveVersionResponseTypeDef:
         """
-        Changes the status of a specific version of a message template to *active* .
+        Changes the status of a specific version of a message template to *active*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_template_active_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_template_active_version)
         """
 
     def update_voice_channel(
         self, *, ApplicationId: str, VoiceChannelRequest: VoiceChannelRequestTypeDef
```

### Comparing `mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/client.pyi` & `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,17 @@
     GetImportJobsResponseTypeDef,
     GetInAppMessagesResponseTypeDef,
     GetInAppTemplateResponseTypeDef,
     GetJourneyDateRangeKpiResponseTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
     GetJourneyResponseTypeDef,
+    GetJourneyRunExecutionActivityMetricsResponseTypeDef,
+    GetJourneyRunExecutionMetricsResponseTypeDef,
+    GetJourneyRunsResponseTypeDef,
     GetPushTemplateResponseTypeDef,
     GetRecommenderConfigurationResponseTypeDef,
     GetRecommenderConfigurationsResponseTypeDef,
     GetSegmentExportJobsResponseTypeDef,
     GetSegmentImportJobsResponseTypeDef,
     GetSegmentResponseTypeDef,
     GetSegmentsResponseTypeDef,
@@ -862,14 +865,56 @@
         """
         Retrieves (queries) pre-aggregated data for a standard execution metric that
         applies to a journey.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_execution_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_journey_execution_metrics)
         """
+    def get_journey_run_execution_activity_metrics(
+        self,
+        *,
+        ApplicationId: str,
+        JourneyActivityId: str,
+        JourneyId: str,
+        RunId: str,
+        NextToken: str = ...,
+        PageSize: str = ...
+    ) -> GetJourneyRunExecutionActivityMetricsResponseTypeDef:
+        """
+        Retrieves (queries) pre-aggregated data for a standard run execution metric that
+        applies to a journey activity.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_run_execution_activity_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_journey_run_execution_activity_metrics)
+        """
+    def get_journey_run_execution_metrics(
+        self,
+        *,
+        ApplicationId: str,
+        JourneyId: str,
+        RunId: str,
+        NextToken: str = ...,
+        PageSize: str = ...
+    ) -> GetJourneyRunExecutionMetricsResponseTypeDef:
+        """
+        Retrieves (queries) pre-aggregated data for a standard run execution metric that
+        applies to a journey.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_run_execution_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_journey_run_execution_metrics)
+        """
+    def get_journey_runs(
+        self, *, ApplicationId: str, JourneyId: str, PageSize: str = ..., Token: str = ...
+    ) -> GetJourneyRunsResponseTypeDef:
+        """
+        Provides information about the runs of a journey.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_runs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_journey_runs)
+        """
     def get_push_template(
         self, *, TemplateName: str, Version: str = ...
     ) -> GetPushTemplateResponseTypeDef:
         """
         Retrieves the content and settings of a message template for messages that are
         sent through a push notification channel.
 
@@ -1379,15 +1424,15 @@
         self,
         *,
         TemplateActiveVersionRequest: TemplateActiveVersionRequestTypeDef,
         TemplateName: str,
         TemplateType: str
     ) -> UpdateTemplateActiveVersionResponseTypeDef:
         """
-        Changes the status of a specific version of a message template to *active* .
+        Changes the status of a specific version of a message template to *active*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_template_active_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_template_active_version)
         """
     def update_voice_channel(
         self, *, ApplicationId: str, VoiceChannelRequest: VoiceChannelRequestTypeDef
     ) -> UpdateVoiceChannelResponseTypeDef:
```

### Comparing `mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/literals.py` & `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     "DurationType",
     "EndpointTypesElementType",
     "FilterTypeType",
     "FormatType",
     "FrequencyType",
     "IncludeType",
     "JobStatusType",
+    "JourneyRunStatusType",
     "LayoutType",
     "MessageTypeType",
     "ModeType",
     "OperatorType",
     "RecencyTypeType",
     "SegmentTypeType",
     "SourceTypeType",
@@ -117,14 +118,15 @@
     "FAILED",
     "FAILING",
     "INITIALIZING",
     "PENDING_JOB",
     "PREPARING_FOR_INITIALIZATION",
     "PROCESSING",
 ]
+JourneyRunStatusType = Literal["CANCELLED", "COMPLETED", "RUNNING", "SCHEDULED"]
 LayoutType = Literal[
     "BOTTOM_BANNER", "CAROUSEL", "MIDDLE_BANNER", "MOBILE_FEED", "OVERLAYS", "TOP_BANNER"
 ]
 MessageTypeType = Literal["PROMOTIONAL", "TRANSACTIONAL"]
 ModeType = Literal["DELIVERY", "FILTER"]
 OperatorType = Literal["ALL", "ANY"]
 RecencyTypeType = Literal["ACTIVE", "INACTIVE"]
@@ -154,14 +156,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -171,27 +174,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -220,14 +227,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -272,51 +280,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -348,28 +362,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -378,14 +396,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -396,55 +415,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/literals.pyi` & `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "DurationType",
     "EndpointTypesElementType",
     "FilterTypeType",
     "FormatType",
     "FrequencyType",
     "IncludeType",
     "JobStatusType",
+    "JourneyRunStatusType",
     "LayoutType",
     "MessageTypeType",
     "ModeType",
     "OperatorType",
     "RecencyTypeType",
     "SegmentTypeType",
     "SourceTypeType",
@@ -115,14 +116,15 @@
     "FAILED",
     "FAILING",
     "INITIALIZING",
     "PENDING_JOB",
     "PREPARING_FOR_INITIALIZATION",
     "PROCESSING",
 ]
+JourneyRunStatusType = Literal["CANCELLED", "COMPLETED", "RUNNING", "SCHEDULED"]
 LayoutType = Literal[
     "BOTTOM_BANNER", "CAROUSEL", "MIDDLE_BANNER", "MOBILE_FEED", "OVERLAYS", "TOP_BANNER"
 ]
 MessageTypeType = Literal["PROMOTIONAL", "TRANSACTIONAL"]
 ModeType = Literal["DELIVERY", "FILTER"]
 OperatorType = Literal["ALL", "ANY"]
 RecencyTypeType = Literal["ACTIVE", "INACTIVE"]
@@ -152,14 +154,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -169,27 +172,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -218,14 +225,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -270,51 +278,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -346,28 +360,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -376,14 +394,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -394,55 +413,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/type_defs.py` & `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     DurationType,
     EndpointTypesElementType,
     FilterTypeType,
     FormatType,
     FrequencyType,
     IncludeType,
     JobStatusType,
+    JourneyRunStatusType,
     LayoutType,
     MessageTypeType,
     ModeType,
     OperatorType,
     RecencyTypeType,
     SegmentTypeType,
     SourceTypeType,
@@ -85,15 +86,14 @@
     "CampaignStateTypeDef",
     "CustomDeliveryConfigurationTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
     "ClosedDaysRuleTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "EmailTemplateRequestTypeDef",
     "CreateTemplateMessageBodyTypeDef",
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
@@ -136,14 +136,15 @@
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
     "JourneyEmailMessageTypeDef",
     "RawEmailTypeDef",
     "EmailTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
     "EndpointItemResponseTypeDef",
     "EndpointMessageResultTypeDef",
     "EndpointSendConfigurationTypeDef",
     "MetricDimensionTypeDef",
@@ -183,14 +184,19 @@
     "GetInAppTemplateRequestRequestTypeDef",
     "GetJourneyDateRangeKpiRequestRequestTypeDef",
     "GetJourneyExecutionActivityMetricsRequestRequestTypeDef",
     "JourneyExecutionActivityMetricsResponseTypeDef",
     "GetJourneyExecutionMetricsRequestRequestTypeDef",
     "JourneyExecutionMetricsResponseTypeDef",
     "GetJourneyRequestRequestTypeDef",
+    "GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef",
+    "JourneyRunExecutionActivityMetricsResponseTypeDef",
+    "GetJourneyRunExecutionMetricsRequestRequestTypeDef",
+    "JourneyRunExecutionMetricsResponseTypeDef",
+    "GetJourneyRunsRequestRequestTypeDef",
     "GetPushTemplateRequestRequestTypeDef",
     "GetRecommenderConfigurationRequestRequestTypeDef",
     "GetRecommenderConfigurationsRequestRequestTypeDef",
     "GetSegmentExportJobsRequestRequestTypeDef",
     "GetSegmentImportJobsRequestRequestTypeDef",
     "GetSegmentRequestRequestTypeDef",
     "GetSegmentVersionRequestRequestTypeDef",
@@ -207,14 +213,15 @@
     "InAppMessageBodyConfigTypeDef",
     "OverrideButtonConfigurationTypeDef",
     "InAppMessageHeaderConfigTypeDef",
     "JourneyChannelSettingsTypeDef",
     "JourneyLimitsTypeDef",
     "JourneyPushMessageTypeDef",
     "JourneyScheduleTypeDef",
+    "JourneyRunResponseTypeDef",
     "JourneySMSMessageTypeDef",
     "JourneyStateRequestTypeDef",
     "ListJourneysRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagsModelTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
@@ -223,14 +230,15 @@
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
     "OpenHoursRuleTypeDef",
     "WriteEventStreamTypeDef",
     "RandomSplitEntryTypeDef",
     "RecencyDimensionTypeDef",
     "UpdateAttributesRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
     "SegmentConditionTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
@@ -240,50 +248,49 @@
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
     "VerificationResponseTypeDef",
     "VerifyOTPMessageRequestParametersTypeDef",
     "UpdateAdmChannelRequestRequestTypeDef",
+    "DeleteAdmChannelResponseTypeDef",
+    "GetAdmChannelResponseTypeDef",
+    "UpdateAdmChannelResponseTypeDef",
     "UpdateApnsChannelRequestRequestTypeDef",
+    "DeleteApnsChannelResponseTypeDef",
+    "GetApnsChannelResponseTypeDef",
+    "UpdateApnsChannelResponseTypeDef",
     "UpdateApnsSandboxChannelRequestRequestTypeDef",
+    "DeleteApnsSandboxChannelResponseTypeDef",
+    "GetApnsSandboxChannelResponseTypeDef",
+    "UpdateApnsSandboxChannelResponseTypeDef",
     "UpdateApnsVoipChannelRequestRequestTypeDef",
+    "DeleteApnsVoipChannelResponseTypeDef",
+    "GetApnsVoipChannelResponseTypeDef",
+    "UpdateApnsVoipChannelResponseTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+    "GetApnsVoipSandboxChannelResponseTypeDef",
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
+    "CreateAppResponseTypeDef",
+    "DeleteAppResponseTypeDef",
+    "GetAppResponseTypeDef",
     "ApplicationSettingsResourceTypeDef",
     "WriteApplicationSettingsRequestTypeDef",
+    "RemoveAttributesResponseTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
+    "DeleteBaiduChannelResponseTypeDef",
+    "GetBaiduChannelResponseTypeDef",
+    "UpdateBaiduChannelResponseTypeDef",
     "ChannelsResponseTypeDef",
     "ClosedDaysTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
-    "CreateAppResponseTypeDef",
-    "DeleteAdmChannelResponseTypeDef",
-    "DeleteApnsChannelResponseTypeDef",
-    "DeleteApnsSandboxChannelResponseTypeDef",
-    "DeleteApnsVoipChannelResponseTypeDef",
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
-    "DeleteAppResponseTypeDef",
-    "DeleteBaiduChannelResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAdmChannelResponseTypeDef",
-    "GetApnsChannelResponseTypeDef",
-    "GetApnsSandboxChannelResponseTypeDef",
-    "GetApnsVoipChannelResponseTypeDef",
-    "GetApnsVoipSandboxChannelResponseTypeDef",
-    "GetAppResponseTypeDef",
-    "GetBaiduChannelResponseTypeDef",
-    "RemoveAttributesResponseTypeDef",
-    "UpdateAdmChannelResponseTypeDef",
-    "UpdateApnsChannelResponseTypeDef",
-    "UpdateApnsSandboxChannelResponseTypeDef",
-    "UpdateApnsVoipChannelResponseTypeDef",
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
-    "UpdateBaiduChannelResponseTypeDef",
     "CreateEmailTemplateRequestRequestTypeDef",
     "UpdateEmailTemplateRequestRequestTypeDef",
     "CreateEmailTemplateResponseTypeDef",
     "CreatePushTemplateResponseTypeDef",
     "CreateSmsTemplateResponseTypeDef",
     "CreateVoiceTemplateResponseTypeDef",
     "CreateExportJobRequestRequestTypeDef",
@@ -343,19 +350,22 @@
     "ItemResponseTypeDef",
     "EventTypeDef",
     "ExportJobResponseTypeDef",
     "UpdateGcmChannelRequestRequestTypeDef",
     "GPSPointDimensionTypeDef",
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     "GetJourneyExecutionMetricsResponseTypeDef",
+    "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
+    "GetJourneyRunExecutionMetricsResponseTypeDef",
     "GetSmsTemplateResponseTypeDef",
     "GetVoiceTemplateResponseTypeDef",
     "ImportJobResponseTypeDef",
     "InAppMessageButtonTypeDef",
     "PushMessageActivityTypeDef",
+    "JourneyRunsResponseTypeDef",
     "SMSMessageActivityTypeDef",
     "UpdateJourneyStateRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "MessageResponseTypeDef",
     "PhoneNumberValidateRequestRequestTypeDef",
     "PhoneNumberValidateResponseTypeDef",
@@ -401,14 +411,15 @@
     "ExportJobsResponseTypeDef",
     "GetExportJobResponseTypeDef",
     "SegmentLocationTypeDef",
     "CreateImportJobResponseTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobsResponseTypeDef",
     "InAppMessageContentTypeDef",
+    "GetJourneyRunsResponseTypeDef",
     "SendMessagesResponseTypeDef",
     "SendOTPMessageResponseTypeDef",
     "BaseKpiResultTypeDef",
     "EmailMessageTypeDef",
     "ListTemplatesResponseTypeDef",
     "ListTemplateVersionsResponseTypeDef",
     "UpdateEndpointsBatchRequestRequestTypeDef",
@@ -809,14 +820,15 @@
         "Start": str,
         "State": str,
         "SuccessfulEndpointCount": int,
         "TimezonesCompletedCount": int,
         "TimezonesTotalCount": int,
         "TotalEndpointCount": int,
         "TreatmentId": str,
+        "ExecutionMetrics": Dict[str, str],
     },
     total=False,
 )
 
 
 class ActivityResponseTypeDef(_RequiredActivityResponseTypeDef, _OptionalActivityResponseTypeDef):
     pass
@@ -1162,25 +1174,14 @@
 
 class CreateApplicationRequestTypeDef(
     _RequiredCreateApplicationRequestTypeDef, _OptionalCreateApplicationRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 EmailTemplateRequestTypeDef = TypedDict(
     "EmailTemplateRequestTypeDef",
     {
         "DefaultSubstitutions": str,
         "HtmlPart": str,
         "RecommenderId": str,
         "Subject": str,
@@ -1928,14 +1929,21 @@
 
 class EmailTemplateResponseTypeDef(
     _RequiredEmailTemplateResponseTypeDef, _OptionalEmailTemplateResponseTypeDef
 ):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EndpointDemographicTypeDef = TypedDict(
     "EndpointDemographicTypeDef",
     {
         "AppVersion": str,
         "Locale": str,
         "Make": str,
         "Model": str,
@@ -2577,14 +2585,112 @@
     "GetJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
     },
 )
 
+_RequiredGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "JourneyActivityId": str,
+        "JourneyId": str,
+        "RunId": str,
+    },
+)
+_OptionalGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "PageSize": str,
+    },
+    total=False,
+)
+
+
+class GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef(
+    _RequiredGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
+    _OptionalGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
+):
+    pass
+
+
+JourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
+    "JourneyRunExecutionActivityMetricsResponseTypeDef",
+    {
+        "ActivityType": str,
+        "ApplicationId": str,
+        "JourneyActivityId": str,
+        "JourneyId": str,
+        "LastEvaluatedTime": str,
+        "Metrics": Dict[str, str],
+        "RunId": str,
+    },
+)
+
+_RequiredGetJourneyRunExecutionMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetJourneyRunExecutionMetricsRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "JourneyId": str,
+        "RunId": str,
+    },
+)
+_OptionalGetJourneyRunExecutionMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetJourneyRunExecutionMetricsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "PageSize": str,
+    },
+    total=False,
+)
+
+
+class GetJourneyRunExecutionMetricsRequestRequestTypeDef(
+    _RequiredGetJourneyRunExecutionMetricsRequestRequestTypeDef,
+    _OptionalGetJourneyRunExecutionMetricsRequestRequestTypeDef,
+):
+    pass
+
+
+JourneyRunExecutionMetricsResponseTypeDef = TypedDict(
+    "JourneyRunExecutionMetricsResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "JourneyId": str,
+        "LastEvaluatedTime": str,
+        "Metrics": Dict[str, str],
+        "RunId": str,
+    },
+)
+
+_RequiredGetJourneyRunsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetJourneyRunsRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "JourneyId": str,
+    },
+)
+_OptionalGetJourneyRunsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetJourneyRunsRequestRequestTypeDef",
+    {
+        "PageSize": str,
+        "Token": str,
+    },
+    total=False,
+)
+
+
+class GetJourneyRunsRequestRequestTypeDef(
+    _RequiredGetJourneyRunsRequestRequestTypeDef, _OptionalGetJourneyRunsRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetPushTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalGetPushTemplateRequestRequestTypeDef = TypedDict(
@@ -2954,14 +3060,24 @@
         "EndTime": Union[datetime, str],
         "StartTime": Union[datetime, str],
         "Timezone": str,
     },
     total=False,
 )
 
+JourneyRunResponseTypeDef = TypedDict(
+    "JourneyRunResponseTypeDef",
+    {
+        "CreationTime": str,
+        "LastUpdateTime": str,
+        "RunId": str,
+        "Status": JourneyRunStatusType,
+    },
+)
+
 JourneySMSMessageTypeDef = TypedDict(
     "JourneySMSMessageTypeDef",
     {
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
         "EntityId": str,
@@ -3158,14 +3274,25 @@
     "UpdateAttributesRequestTypeDef",
     {
         "Blacklist": Sequence[str],
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 ResultRowValueTypeDef = TypedDict(
     "ResultRowValueTypeDef",
     {
         "Key": str,
         "Type": str,
         "Value": str,
     },
@@ -3405,335 +3532,328 @@
     "UpdateAdmChannelRequestRequestTypeDef",
     {
         "ADMChannelRequest": ADMChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-UpdateApnsChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsChannelRequestRequestTypeDef",
+DeleteAdmChannelResponseTypeDef = TypedDict(
+    "DeleteAdmChannelResponseTypeDef",
     {
-        "APNSChannelRequest": APNSChannelRequestTypeDef,
-        "ApplicationId": str,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelRequestRequestTypeDef",
+GetAdmChannelResponseTypeDef = TypedDict(
+    "GetAdmChannelResponseTypeDef",
     {
-        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
-        "ApplicationId": str,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipChannelRequestRequestTypeDef",
+UpdateAdmChannelResponseTypeDef = TypedDict(
+    "UpdateAdmChannelResponseTypeDef",
     {
-        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
-        "ApplicationId": str,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
+UpdateApnsChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsChannelRequestRequestTypeDef",
     {
-        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
+        "APNSChannelRequest": APNSChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-_RequiredActivitiesResponseTypeDef = TypedDict(
-    "_RequiredActivitiesResponseTypeDef",
+DeleteApnsChannelResponseTypeDef = TypedDict(
+    "DeleteApnsChannelResponseTypeDef",
     {
-        "Item": List[ActivityResponseTypeDef],
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalActivitiesResponseTypeDef = TypedDict(
-    "_OptionalActivitiesResponseTypeDef",
+
+GetApnsChannelResponseTypeDef = TypedDict(
+    "GetApnsChannelResponseTypeDef",
     {
-        "NextToken": str,
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ActivitiesResponseTypeDef(
-    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
-):
-    pass
-
-
-ApplicationsResponseTypeDef = TypedDict(
-    "ApplicationsResponseTypeDef",
+UpdateApnsChannelResponseTypeDef = TypedDict(
+    "UpdateApnsChannelResponseTypeDef",
     {
-        "Item": List[ApplicationResponseTypeDef],
-        "NextToken": str,
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredApplicationSettingsResourceTypeDef = TypedDict(
-    "_RequiredApplicationSettingsResourceTypeDef",
+UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelRequestRequestTypeDef",
     {
+        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
-_OptionalApplicationSettingsResourceTypeDef = TypedDict(
-    "_OptionalApplicationSettingsResourceTypeDef",
+
+DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsSandboxChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "LastModifiedDate": str,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
+GetApnsSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsSandboxChannelResponseTypeDef",
+    {
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-class ApplicationSettingsResourceTypeDef(
-    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
-):
-    pass
-
-
-WriteApplicationSettingsRequestTypeDef = TypedDict(
-    "WriteApplicationSettingsRequestTypeDef",
+UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "CloudWatchMetricsEnabled": bool,
-        "EventTaggingEnabled": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
-    "UpdateBaiduChannelRequestRequestTypeDef",
+UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipChannelRequestRequestTypeDef",
     {
+        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
         "ApplicationId": str,
-        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
-ChannelsResponseTypeDef = TypedDict(
-    "ChannelsResponseTypeDef",
+DeleteApnsVoipChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipChannelResponseTypeDef",
     {
-        "Channels": Dict[str, ChannelResponseTypeDef],
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ClosedDaysTypeDef = TypedDict(
-    "ClosedDaysTypeDef",
+GetApnsVoipChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipChannelResponseTypeDef",
     {
-        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
-        "SMS": Sequence[ClosedDaysRuleTypeDef],
-        "PUSH": Sequence[ClosedDaysRuleTypeDef],
-        "VOICE": Sequence[ClosedDaysRuleTypeDef],
-        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-WaitActivityTypeDef = TypedDict(
-    "WaitActivityTypeDef",
+UpdateApnsVoipChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipChannelResponseTypeDef",
     {
-        "NextActivity": str,
-        "WaitTime": WaitTimeTypeDef,
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
+UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     {
-        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
+        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteAdmChannelResponseTypeDef = TypedDict(
-    "DeleteAdmChannelResponseTypeDef",
+GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteApnsChannelResponseTypeDef = TypedDict(
-    "DeleteApnsChannelResponseTypeDef",
+UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsSandboxChannelResponseTypeDef",
+_RequiredActivitiesResponseTypeDef = TypedDict(
+    "_RequiredActivitiesResponseTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Item": List[ActivityResponseTypeDef],
     },
 )
-
-DeleteApnsVoipChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipChannelResponseTypeDef",
+_OptionalActivitiesResponseTypeDef = TypedDict(
+    "_OptionalActivitiesResponseTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": str,
     },
+    total=False,
 )
 
-DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+
+class ActivitiesResponseTypeDef(
+    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
+):
+    pass
+
+
+ApplicationsResponseTypeDef = TypedDict(
+    "ApplicationsResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Item": List[ApplicationResponseTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-DeleteAppResponseTypeDef = TypedDict(
-    "DeleteAppResponseTypeDef",
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
     {
         "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteBaiduChannelResponseTypeDef = TypedDict(
-    "DeleteBaiduChannelResponseTypeDef",
+DeleteAppResponseTypeDef = TypedDict(
+    "DeleteAppResponseTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+GetAppResponseTypeDef = TypedDict(
+    "GetAppResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAdmChannelResponseTypeDef = TypedDict(
-    "GetAdmChannelResponseTypeDef",
+_RequiredApplicationSettingsResourceTypeDef = TypedDict(
+    "_RequiredApplicationSettingsResourceTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
     },
 )
-
-GetApnsChannelResponseTypeDef = TypedDict(
-    "GetApnsChannelResponseTypeDef",
+_OptionalApplicationSettingsResourceTypeDef = TypedDict(
+    "_OptionalApplicationSettingsResourceTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "LastModifiedDate": str,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
+    total=False,
 )
 
-GetApnsSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsSandboxChannelResponseTypeDef",
+
+class ApplicationSettingsResourceTypeDef(
+    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
+):
+    pass
+
+
+WriteApplicationSettingsRequestTypeDef = TypedDict(
+    "WriteApplicationSettingsRequestTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "CloudWatchMetricsEnabled": bool,
+        "EventTaggingEnabled": bool,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
+    total=False,
 )
 
-GetApnsVoipChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipChannelResponseTypeDef",
+RemoveAttributesResponseTypeDef = TypedDict(
+    "RemoveAttributesResponseTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AttributesResource": AttributesResourceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipSandboxChannelResponseTypeDef",
+UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
+    "UpdateBaiduChannelRequestRequestTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
+        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
-GetAppResponseTypeDef = TypedDict(
-    "GetAppResponseTypeDef",
+DeleteBaiduChannelResponseTypeDef = TypedDict(
+    "DeleteBaiduChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBaiduChannelResponseTypeDef = TypedDict(
     "GetBaiduChannelResponseTypeDef",
     {
         "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveAttributesResponseTypeDef = TypedDict(
-    "RemoveAttributesResponseTypeDef",
-    {
-        "AttributesResource": AttributesResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAdmChannelResponseTypeDef = TypedDict(
-    "UpdateAdmChannelResponseTypeDef",
-    {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApnsChannelResponseTypeDef = TypedDict(
-    "UpdateApnsChannelResponseTypeDef",
+UpdateBaiduChannelResponseTypeDef = TypedDict(
+    "UpdateBaiduChannelResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelResponseTypeDef",
+ChannelsResponseTypeDef = TypedDict(
+    "ChannelsResponseTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
-UpdateApnsVoipChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipChannelResponseTypeDef",
+ClosedDaysTypeDef = TypedDict(
+    "ClosedDaysTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
+        "SMS": Sequence[ClosedDaysRuleTypeDef],
+        "PUSH": Sequence[ClosedDaysRuleTypeDef],
+        "VOICE": Sequence[ClosedDaysRuleTypeDef],
+        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
     },
+    total=False,
 )
 
-UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+WaitActivityTypeDef = TypedDict(
+    "WaitActivityTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextActivity": str,
+        "WaitTime": WaitTimeTypeDef,
     },
+    total=False,
 )
 
-UpdateBaiduChannelResponseTypeDef = TypedDict(
-    "UpdateBaiduChannelResponseTypeDef",
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
     },
 )
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "EmailTemplateRequest": EmailTemplateRequestTypeDef,
@@ -3765,39 +3885,39 @@
     pass
 
 
 CreateEmailTemplateResponseTypeDef = TypedDict(
     "CreateEmailTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePushTemplateResponseTypeDef = TypedDict(
     "CreatePushTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSmsTemplateResponseTypeDef = TypedDict(
     "CreateSmsTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVoiceTemplateResponseTypeDef = TypedDict(
     "CreateVoiceTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateExportJobRequestRequestTypeDef = TypedDict(
     "CreateExportJobRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -3813,46 +3933,46 @@
     },
 )
 
 CreateInAppTemplateResponseTypeDef = TypedDict(
     "CreateInAppTemplateResponseTypeDef",
     {
         "TemplateCreateMessageBody": TemplateCreateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "CreateRecommenderConfigurationRequestRequestTypeDef",
     {
         "CreateRecommenderConfiguration": CreateRecommenderConfigurationTypeDef,
     },
 )
 
 CreateRecommenderConfigurationResponseTypeDef = TypedDict(
     "CreateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRecommenderConfigurationResponseTypeDef = TypedDict(
     "DeleteRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommenderConfigurationResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRecommenderConfigurationsResponseTypeDef = TypedDict(
     "_RequiredListRecommenderConfigurationsResponseTypeDef",
     {
         "Item": List[RecommenderConfigurationResponseTypeDef],
@@ -3874,15 +3994,15 @@
     pass
 
 
 UpdateRecommenderConfigurationResponseTypeDef = TypedDict(
     "UpdateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSmsTemplateRequestRequestTypeDef = TypedDict(
     "CreateSmsTemplateRequestRequestTypeDef",
     {
         "SMSTemplateRequest": SMSTemplateRequestTypeDef,
@@ -4009,231 +4129,231 @@
     pass
 
 
 DeleteEmailChannelResponseTypeDef = TypedDict(
     "DeleteEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEmailChannelResponseTypeDef = TypedDict(
     "GetEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailChannelResponseTypeDef = TypedDict(
     "UpdateEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEmailTemplateResponseTypeDef = TypedDict(
     "DeleteEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInAppTemplateResponseTypeDef = TypedDict(
     "DeleteInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePushTemplateResponseTypeDef = TypedDict(
     "DeletePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSmsTemplateResponseTypeDef = TypedDict(
     "DeleteSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVoiceTemplateResponseTypeDef = TypedDict(
     "DeleteVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailTemplateResponseTypeDef = TypedDict(
     "UpdateEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointResponseTypeDef = TypedDict(
     "UpdateEndpointResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointsBatchResponseTypeDef = TypedDict(
     "UpdateEndpointsBatchResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInAppTemplateResponseTypeDef = TypedDict(
     "UpdateInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePushTemplateResponseTypeDef = TypedDict(
     "UpdatePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSmsTemplateResponseTypeDef = TypedDict(
     "UpdateSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTemplateActiveVersionResponseTypeDef = TypedDict(
     "UpdateTemplateActiveVersionResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceTemplateResponseTypeDef = TypedDict(
     "UpdateVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEventStreamResponseTypeDef = TypedDict(
     "DeleteEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEventStreamResponseTypeDef = TypedDict(
     "GetEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutEventStreamResponseTypeDef = TypedDict(
     "PutEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteGcmChannelResponseTypeDef = TypedDict(
     "DeleteGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGcmChannelResponseTypeDef = TypedDict(
     "GetGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGcmChannelResponseTypeDef = TypedDict(
     "UpdateGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSmsChannelResponseTypeDef = TypedDict(
     "DeleteSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSmsChannelResponseTypeDef = TypedDict(
     "GetSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSmsChannelResponseTypeDef = TypedDict(
     "UpdateSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVoiceChannelResponseTypeDef = TypedDict(
     "DeleteVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceChannelResponseTypeDef = TypedDict(
     "GetVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceChannelResponseTypeDef = TypedDict(
     "UpdateVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailChannelRequestRequestTypeDef = TypedDict(
     "UpdateEmailChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4252,15 +4372,15 @@
     total=False,
 )
 
 GetEmailTemplateResponseTypeDef = TypedDict(
     "GetEmailTemplateResponseTypeDef",
     {
         "EmailTemplateResponse": EmailTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointBatchItemTypeDef = TypedDict(
     "EndpointBatchItemTypeDef",
     {
         "Address": str,
@@ -4479,39 +4599,57 @@
     pass
 
 
 GetJourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyExecutionActivityMetricsResponse": JourneyExecutionActivityMetricsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionMetricsResponseTypeDef",
     {
         "JourneyExecutionMetricsResponse": JourneyExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetJourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
+    "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
+    {
+        "JourneyRunExecutionActivityMetricsResponse": (
+            JourneyRunExecutionActivityMetricsResponseTypeDef
+        ),
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetJourneyRunExecutionMetricsResponseTypeDef = TypedDict(
+    "GetJourneyRunExecutionMetricsResponseTypeDef",
+    {
+        "JourneyRunExecutionMetricsResponse": JourneyRunExecutionMetricsResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSmsTemplateResponseTypeDef = TypedDict(
     "GetSmsTemplateResponseTypeDef",
     {
         "SMSTemplateResponse": SMSTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceTemplateResponseTypeDef = TypedDict(
     "GetVoiceTemplateResponseTypeDef",
     {
         "VoiceTemplateResponse": VoiceTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportJobResponseTypeDef = TypedDict(
     "_RequiredImportJobResponseTypeDef",
     {
         "ApplicationId": str,
@@ -4561,14 +4699,35 @@
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
     },
     total=False,
 )
 
+_RequiredJourneyRunsResponseTypeDef = TypedDict(
+    "_RequiredJourneyRunsResponseTypeDef",
+    {
+        "Item": List[JourneyRunResponseTypeDef],
+    },
+)
+_OptionalJourneyRunsResponseTypeDef = TypedDict(
+    "_OptionalJourneyRunsResponseTypeDef",
+    {
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class JourneyRunsResponseTypeDef(
+    _RequiredJourneyRunsResponseTypeDef, _OptionalJourneyRunsResponseTypeDef
+):
+    pass
+
+
 SMSMessageActivityTypeDef = TypedDict(
     "SMSMessageActivityTypeDef",
     {
         "MessageConfig": JourneySMSMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -4585,15 +4744,15 @@
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagsModel": TagsModelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -4629,15 +4788,15 @@
     },
 )
 
 PhoneNumberValidateResponseTypeDef = TypedDict(
     "PhoneNumberValidateResponseTypeDef",
     {
         "NumberValidateResponse": NumberValidateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
         "EMAIL": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
@@ -4796,15 +4955,15 @@
     },
 )
 
 VerifyOTPMessageResponseTypeDef = TypedDict(
     "VerifyOTPMessageResponseTypeDef",
     {
         "VerificationResponse": VerificationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VerifyOTPMessageRequestRequestTypeDef = TypedDict(
     "VerifyOTPMessageRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4812,39 +4971,39 @@
     },
 )
 
 GetCampaignActivitiesResponseTypeDef = TypedDict(
     "GetCampaignActivitiesResponseTypeDef",
     {
         "ActivitiesResponse": ActivitiesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppsResponseTypeDef = TypedDict(
     "GetAppsResponseTypeDef",
     {
         "ApplicationsResponse": ApplicationsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationSettingsResponseTypeDef = TypedDict(
     "GetApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationSettingsResponseTypeDef = TypedDict(
     "UpdateApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
     "UpdateApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4852,23 +5011,23 @@
     },
 )
 
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommenderConfigurationsResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationsResponseTypeDef",
     {
         "ListRecommenderConfigurationsResponse": ListRecommenderConfigurationsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePushTemplateRequestRequestTypeDef = TypedDict(
     "CreatePushTemplateRequestRequestTypeDef",
     {
         "PushNotificationTemplateRequest": PushNotificationTemplateRequestTypeDef,
@@ -4900,15 +5059,15 @@
     pass
 
 
 GetPushTemplateResponseTypeDef = TypedDict(
     "GetPushTemplateResponseTypeDef",
     {
         "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointBatchRequestTypeDef = TypedDict(
     "EndpointBatchRequestTypeDef",
     {
         "Item": Sequence[EndpointBatchItemTypeDef],
@@ -4924,38 +5083,38 @@
     },
 )
 
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointsResponseTypeDef = TypedDict(
     "EndpointsResponseTypeDef",
     {
         "Item": List[EndpointResponseTypeDef],
     },
 )
 
 GetEndpointResponseTypeDef = TypedDict(
     "GetEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendUsersMessagesResponseTypeDef = TypedDict(
     "SendUsersMessagesResponseTypeDef",
     {
         "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CampaignEventFilterTypeDef = TypedDict(
     "CampaignEventFilterTypeDef",
     {
         "Dimensions": EventDimensionsTypeDef,
@@ -4996,15 +5155,15 @@
     },
 )
 
 CreateExportJobResponseTypeDef = TypedDict(
     "CreateExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredExportJobsResponseTypeDef = TypedDict(
     "_RequiredExportJobsResponseTypeDef",
     {
         "Item": List[ExportJobResponseTypeDef],
@@ -5025,15 +5184,15 @@
     pass
 
 
 GetExportJobResponseTypeDef = TypedDict(
     "GetExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
         "Country": SetDimensionTypeDef,
@@ -5042,23 +5201,23 @@
     total=False,
 )
 
 CreateImportJobResponseTypeDef = TypedDict(
     "CreateImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetImportJobResponseTypeDef = TypedDict(
     "GetImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportJobsResponseTypeDef = TypedDict(
     "_RequiredImportJobsResponseTypeDef",
     {
         "Item": List[ImportJobResponseTypeDef],
@@ -5088,27 +5247,35 @@
         "ImageUrl": str,
         "PrimaryBtn": InAppMessageButtonTypeDef,
         "SecondaryBtn": InAppMessageButtonTypeDef,
     },
     total=False,
 )
 
+GetJourneyRunsResponseTypeDef = TypedDict(
+    "GetJourneyRunsResponseTypeDef",
+    {
+        "JourneyRunsResponse": JourneyRunsResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SendMessagesResponseTypeDef = TypedDict(
     "SendMessagesResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendOTPMessageResponseTypeDef = TypedDict(
     "SendOTPMessageResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BaseKpiResultTypeDef = TypedDict(
     "BaseKpiResultTypeDef",
     {
         "Rows": List[ResultRowTypeDef],
@@ -5129,23 +5296,23 @@
     total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesResponse": TemplatesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTemplateVersionsResponseTypeDef = TypedDict(
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionsResponse": TemplateVersionsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointsBatchRequestRequestTypeDef = TypedDict(
     "UpdateEndpointsBatchRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5153,23 +5320,23 @@
     },
 )
 
 DeleteUserEndpointsResponseTypeDef = TypedDict(
     "DeleteUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserEndpointsResponseTypeDef = TypedDict(
     "GetUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": str,
@@ -5212,38 +5379,38 @@
     total=False,
 )
 
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "EventsResponse": EventsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventsRequestTypeDef = TypedDict(
     "EventsRequestTypeDef",
     {
         "BatchItem": Mapping[str, EventsBatchTypeDef],
     },
 )
 
 GetExportJobsResponseTypeDef = TypedDict(
     "GetExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentExportJobsResponseTypeDef = TypedDict(
     "GetSegmentExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
@@ -5256,23 +5423,23 @@
     total=False,
 )
 
 GetImportJobsResponseTypeDef = TypedDict(
     "GetImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentImportJobsResponseTypeDef = TypedDict(
     "GetSegmentImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CampaignInAppMessageTypeDef = TypedDict(
     "CampaignInAppMessageTypeDef",
     {
         "Body": str,
@@ -5530,39 +5697,39 @@
     pass
 
 
 GetInAppTemplateResponseTypeDef = TypedDict(
     "GetInAppTemplateResponseTypeDef",
     {
         "InAppTemplateResponse": InAppTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "GetApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationDateRangeKpiResponse": ApplicationDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "GetCampaignDateRangeKpiResponseTypeDef",
     {
         "CampaignDateRangeKpiResponse": CampaignDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "GetJourneyDateRangeKpiResponseTypeDef",
     {
         "JourneyDateRangeKpiResponse": JourneyDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMessageRequestTypeDef = TypedDict(
     "_RequiredMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
@@ -5841,47 +6008,47 @@
     total=False,
 )
 
 GetInAppMessagesResponseTypeDef = TypedDict(
     "GetInAppMessagesResponseTypeDef",
     {
         "InAppMessagesResponse": InAppMessagesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSegmentResponseTypeDef = TypedDict(
     "DeleteSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentVersionResponseTypeDef = TypedDict(
     "GetSegmentVersionResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSegmentsResponseTypeDef = TypedDict(
     "_RequiredSegmentsResponseTypeDef",
     {
         "Item": List[SegmentResponseTypeDef],
@@ -5900,15 +6067,15 @@
     pass
 
 
 UpdateSegmentResponseTypeDef = TypedDict(
     "UpdateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5964,47 +6131,47 @@
     pass
 
 
 CreateCampaignResponseTypeDef = TypedDict(
     "CreateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCampaignResponseTypeDef = TypedDict(
     "DeleteCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignResponseTypeDef = TypedDict(
     "GetCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignVersionResponseTypeDef = TypedDict(
     "GetCampaignVersionResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCampaignResponseTypeDef = TypedDict(
     "UpdateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCampaignRequestRequestTypeDef = TypedDict(
     "CreateCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6021,23 +6188,23 @@
     },
 )
 
 GetSegmentVersionsResponseTypeDef = TypedDict(
     "GetSegmentVersionsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentsResponseTypeDef = TypedDict(
     "GetSegmentsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJourneyResponseTypeDef = TypedDict(
     "_RequiredJourneyResponseTypeDef",
     {
         "ApplicationId": str,
@@ -6112,47 +6279,47 @@
     pass
 
 
 GetCampaignVersionsResponseTypeDef = TypedDict(
     "GetCampaignVersionsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignsResponseTypeDef = TypedDict(
     "GetCampaignsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateJourneyResponseTypeDef = TypedDict(
     "CreateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteJourneyResponseTypeDef = TypedDict(
     "DeleteJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyResponseTypeDef = TypedDict(
     "GetJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJourneysResponseTypeDef = TypedDict(
     "_RequiredJourneysResponseTypeDef",
     {
         "Item": List[JourneyResponseTypeDef],
@@ -6171,23 +6338,23 @@
     pass
 
 
 UpdateJourneyResponseTypeDef = TypedDict(
     "UpdateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateJourneyStateResponseTypeDef = TypedDict(
     "UpdateJourneyStateResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateJourneyRequestRequestTypeDef = TypedDict(
     "CreateJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -6204,10 +6371,10 @@
     },
 )
 
 ListJourneysResponseTypeDef = TypedDict(
     "ListJourneysResponseTypeDef",
     {
         "JourneysResponse": JourneysResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint/type_defs.pyi` & `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     DurationType,
     EndpointTypesElementType,
     FilterTypeType,
     FormatType,
     FrequencyType,
     IncludeType,
     JobStatusType,
+    JourneyRunStatusType,
     LayoutType,
     MessageTypeType,
     ModeType,
     OperatorType,
     RecencyTypeType,
     SegmentTypeType,
     SourceTypeType,
@@ -84,15 +85,14 @@
     "CampaignStateTypeDef",
     "CustomDeliveryConfigurationTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
     "ClosedDaysRuleTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "EmailTemplateRequestTypeDef",
     "CreateTemplateMessageBodyTypeDef",
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
@@ -135,14 +135,15 @@
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
     "JourneyEmailMessageTypeDef",
     "RawEmailTypeDef",
     "EmailTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
     "EndpointItemResponseTypeDef",
     "EndpointMessageResultTypeDef",
     "EndpointSendConfigurationTypeDef",
     "MetricDimensionTypeDef",
@@ -182,14 +183,19 @@
     "GetInAppTemplateRequestRequestTypeDef",
     "GetJourneyDateRangeKpiRequestRequestTypeDef",
     "GetJourneyExecutionActivityMetricsRequestRequestTypeDef",
     "JourneyExecutionActivityMetricsResponseTypeDef",
     "GetJourneyExecutionMetricsRequestRequestTypeDef",
     "JourneyExecutionMetricsResponseTypeDef",
     "GetJourneyRequestRequestTypeDef",
+    "GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef",
+    "JourneyRunExecutionActivityMetricsResponseTypeDef",
+    "GetJourneyRunExecutionMetricsRequestRequestTypeDef",
+    "JourneyRunExecutionMetricsResponseTypeDef",
+    "GetJourneyRunsRequestRequestTypeDef",
     "GetPushTemplateRequestRequestTypeDef",
     "GetRecommenderConfigurationRequestRequestTypeDef",
     "GetRecommenderConfigurationsRequestRequestTypeDef",
     "GetSegmentExportJobsRequestRequestTypeDef",
     "GetSegmentImportJobsRequestRequestTypeDef",
     "GetSegmentRequestRequestTypeDef",
     "GetSegmentVersionRequestRequestTypeDef",
@@ -206,14 +212,15 @@
     "InAppMessageBodyConfigTypeDef",
     "OverrideButtonConfigurationTypeDef",
     "InAppMessageHeaderConfigTypeDef",
     "JourneyChannelSettingsTypeDef",
     "JourneyLimitsTypeDef",
     "JourneyPushMessageTypeDef",
     "JourneyScheduleTypeDef",
+    "JourneyRunResponseTypeDef",
     "JourneySMSMessageTypeDef",
     "JourneyStateRequestTypeDef",
     "ListJourneysRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagsModelTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
@@ -222,14 +229,15 @@
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
     "OpenHoursRuleTypeDef",
     "WriteEventStreamTypeDef",
     "RandomSplitEntryTypeDef",
     "RecencyDimensionTypeDef",
     "UpdateAttributesRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
     "SegmentConditionTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
@@ -239,50 +247,49 @@
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
     "VerificationResponseTypeDef",
     "VerifyOTPMessageRequestParametersTypeDef",
     "UpdateAdmChannelRequestRequestTypeDef",
+    "DeleteAdmChannelResponseTypeDef",
+    "GetAdmChannelResponseTypeDef",
+    "UpdateAdmChannelResponseTypeDef",
     "UpdateApnsChannelRequestRequestTypeDef",
+    "DeleteApnsChannelResponseTypeDef",
+    "GetApnsChannelResponseTypeDef",
+    "UpdateApnsChannelResponseTypeDef",
     "UpdateApnsSandboxChannelRequestRequestTypeDef",
+    "DeleteApnsSandboxChannelResponseTypeDef",
+    "GetApnsSandboxChannelResponseTypeDef",
+    "UpdateApnsSandboxChannelResponseTypeDef",
     "UpdateApnsVoipChannelRequestRequestTypeDef",
+    "DeleteApnsVoipChannelResponseTypeDef",
+    "GetApnsVoipChannelResponseTypeDef",
+    "UpdateApnsVoipChannelResponseTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+    "GetApnsVoipSandboxChannelResponseTypeDef",
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
+    "CreateAppResponseTypeDef",
+    "DeleteAppResponseTypeDef",
+    "GetAppResponseTypeDef",
     "ApplicationSettingsResourceTypeDef",
     "WriteApplicationSettingsRequestTypeDef",
+    "RemoveAttributesResponseTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
+    "DeleteBaiduChannelResponseTypeDef",
+    "GetBaiduChannelResponseTypeDef",
+    "UpdateBaiduChannelResponseTypeDef",
     "ChannelsResponseTypeDef",
     "ClosedDaysTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
-    "CreateAppResponseTypeDef",
-    "DeleteAdmChannelResponseTypeDef",
-    "DeleteApnsChannelResponseTypeDef",
-    "DeleteApnsSandboxChannelResponseTypeDef",
-    "DeleteApnsVoipChannelResponseTypeDef",
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
-    "DeleteAppResponseTypeDef",
-    "DeleteBaiduChannelResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAdmChannelResponseTypeDef",
-    "GetApnsChannelResponseTypeDef",
-    "GetApnsSandboxChannelResponseTypeDef",
-    "GetApnsVoipChannelResponseTypeDef",
-    "GetApnsVoipSandboxChannelResponseTypeDef",
-    "GetAppResponseTypeDef",
-    "GetBaiduChannelResponseTypeDef",
-    "RemoveAttributesResponseTypeDef",
-    "UpdateAdmChannelResponseTypeDef",
-    "UpdateApnsChannelResponseTypeDef",
-    "UpdateApnsSandboxChannelResponseTypeDef",
-    "UpdateApnsVoipChannelResponseTypeDef",
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
-    "UpdateBaiduChannelResponseTypeDef",
     "CreateEmailTemplateRequestRequestTypeDef",
     "UpdateEmailTemplateRequestRequestTypeDef",
     "CreateEmailTemplateResponseTypeDef",
     "CreatePushTemplateResponseTypeDef",
     "CreateSmsTemplateResponseTypeDef",
     "CreateVoiceTemplateResponseTypeDef",
     "CreateExportJobRequestRequestTypeDef",
@@ -342,19 +349,22 @@
     "ItemResponseTypeDef",
     "EventTypeDef",
     "ExportJobResponseTypeDef",
     "UpdateGcmChannelRequestRequestTypeDef",
     "GPSPointDimensionTypeDef",
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     "GetJourneyExecutionMetricsResponseTypeDef",
+    "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
+    "GetJourneyRunExecutionMetricsResponseTypeDef",
     "GetSmsTemplateResponseTypeDef",
     "GetVoiceTemplateResponseTypeDef",
     "ImportJobResponseTypeDef",
     "InAppMessageButtonTypeDef",
     "PushMessageActivityTypeDef",
+    "JourneyRunsResponseTypeDef",
     "SMSMessageActivityTypeDef",
     "UpdateJourneyStateRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "MessageResponseTypeDef",
     "PhoneNumberValidateRequestRequestTypeDef",
     "PhoneNumberValidateResponseTypeDef",
@@ -400,14 +410,15 @@
     "ExportJobsResponseTypeDef",
     "GetExportJobResponseTypeDef",
     "SegmentLocationTypeDef",
     "CreateImportJobResponseTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobsResponseTypeDef",
     "InAppMessageContentTypeDef",
+    "GetJourneyRunsResponseTypeDef",
     "SendMessagesResponseTypeDef",
     "SendOTPMessageResponseTypeDef",
     "BaseKpiResultTypeDef",
     "EmailMessageTypeDef",
     "ListTemplatesResponseTypeDef",
     "ListTemplateVersionsResponseTypeDef",
     "UpdateEndpointsBatchRequestRequestTypeDef",
@@ -796,14 +807,15 @@
         "Start": str,
         "State": str,
         "SuccessfulEndpointCount": int,
         "TimezonesCompletedCount": int,
         "TimezonesTotalCount": int,
         "TotalEndpointCount": int,
         "TreatmentId": str,
+        "ExecutionMetrics": Dict[str, str],
     },
     total=False,
 )
 
 class ActivityResponseTypeDef(_RequiredActivityResponseTypeDef, _OptionalActivityResponseTypeDef):
     pass
 
@@ -1131,25 +1143,14 @@
 )
 
 class CreateApplicationRequestTypeDef(
     _RequiredCreateApplicationRequestTypeDef, _OptionalCreateApplicationRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 EmailTemplateRequestTypeDef = TypedDict(
     "EmailTemplateRequestTypeDef",
     {
         "DefaultSubstitutions": str,
         "HtmlPart": str,
         "RecommenderId": str,
         "Subject": str,
@@ -1863,14 +1864,21 @@
 )
 
 class EmailTemplateResponseTypeDef(
     _RequiredEmailTemplateResponseTypeDef, _OptionalEmailTemplateResponseTypeDef
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EndpointDemographicTypeDef = TypedDict(
     "EndpointDemographicTypeDef",
     {
         "AppVersion": str,
         "Locale": str,
         "Make": str,
         "Model": str,
@@ -2478,14 +2486,106 @@
     "GetJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "JourneyId": str,
     },
 )
 
+_RequiredGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "JourneyActivityId": str,
+        "JourneyId": str,
+        "RunId": str,
+    },
+)
+_OptionalGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "PageSize": str,
+    },
+    total=False,
+)
+
+class GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef(
+    _RequiredGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
+    _OptionalGetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
+):
+    pass
+
+JourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
+    "JourneyRunExecutionActivityMetricsResponseTypeDef",
+    {
+        "ActivityType": str,
+        "ApplicationId": str,
+        "JourneyActivityId": str,
+        "JourneyId": str,
+        "LastEvaluatedTime": str,
+        "Metrics": Dict[str, str],
+        "RunId": str,
+    },
+)
+
+_RequiredGetJourneyRunExecutionMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetJourneyRunExecutionMetricsRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "JourneyId": str,
+        "RunId": str,
+    },
+)
+_OptionalGetJourneyRunExecutionMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetJourneyRunExecutionMetricsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "PageSize": str,
+    },
+    total=False,
+)
+
+class GetJourneyRunExecutionMetricsRequestRequestTypeDef(
+    _RequiredGetJourneyRunExecutionMetricsRequestRequestTypeDef,
+    _OptionalGetJourneyRunExecutionMetricsRequestRequestTypeDef,
+):
+    pass
+
+JourneyRunExecutionMetricsResponseTypeDef = TypedDict(
+    "JourneyRunExecutionMetricsResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "JourneyId": str,
+        "LastEvaluatedTime": str,
+        "Metrics": Dict[str, str],
+        "RunId": str,
+    },
+)
+
+_RequiredGetJourneyRunsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetJourneyRunsRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "JourneyId": str,
+    },
+)
+_OptionalGetJourneyRunsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetJourneyRunsRequestRequestTypeDef",
+    {
+        "PageSize": str,
+        "Token": str,
+    },
+    total=False,
+)
+
+class GetJourneyRunsRequestRequestTypeDef(
+    _RequiredGetJourneyRunsRequestRequestTypeDef, _OptionalGetJourneyRunsRequestRequestTypeDef
+):
+    pass
+
 _RequiredGetPushTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetPushTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 _OptionalGetPushTemplateRequestRequestTypeDef = TypedDict(
@@ -2833,14 +2933,24 @@
         "EndTime": Union[datetime, str],
         "StartTime": Union[datetime, str],
         "Timezone": str,
     },
     total=False,
 )
 
+JourneyRunResponseTypeDef = TypedDict(
+    "JourneyRunResponseTypeDef",
+    {
+        "CreationTime": str,
+        "LastUpdateTime": str,
+        "RunId": str,
+        "Status": JourneyRunStatusType,
+    },
+)
+
 JourneySMSMessageTypeDef = TypedDict(
     "JourneySMSMessageTypeDef",
     {
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
         "EntityId": str,
@@ -3031,14 +3141,25 @@
     "UpdateAttributesRequestTypeDef",
     {
         "Blacklist": Sequence[str],
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 ResultRowValueTypeDef = TypedDict(
     "ResultRowValueTypeDef",
     {
         "Key": str,
         "Type": str,
         "Value": str,
     },
@@ -3266,331 +3387,324 @@
     "UpdateAdmChannelRequestRequestTypeDef",
     {
         "ADMChannelRequest": ADMChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-UpdateApnsChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsChannelRequestRequestTypeDef",
+DeleteAdmChannelResponseTypeDef = TypedDict(
+    "DeleteAdmChannelResponseTypeDef",
     {
-        "APNSChannelRequest": APNSChannelRequestTypeDef,
-        "ApplicationId": str,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelRequestRequestTypeDef",
+GetAdmChannelResponseTypeDef = TypedDict(
+    "GetAdmChannelResponseTypeDef",
     {
-        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
-        "ApplicationId": str,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipChannelRequestRequestTypeDef",
+UpdateAdmChannelResponseTypeDef = TypedDict(
+    "UpdateAdmChannelResponseTypeDef",
     {
-        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
-        "ApplicationId": str,
+        "ADMChannelResponse": ADMChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
+UpdateApnsChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsChannelRequestRequestTypeDef",
     {
-        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
+        "APNSChannelRequest": APNSChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
 
-_RequiredActivitiesResponseTypeDef = TypedDict(
-    "_RequiredActivitiesResponseTypeDef",
+DeleteApnsChannelResponseTypeDef = TypedDict(
+    "DeleteApnsChannelResponseTypeDef",
     {
-        "Item": List[ActivityResponseTypeDef],
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalActivitiesResponseTypeDef = TypedDict(
-    "_OptionalActivitiesResponseTypeDef",
+
+GetApnsChannelResponseTypeDef = TypedDict(
+    "GetApnsChannelResponseTypeDef",
     {
-        "NextToken": str,
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ActivitiesResponseTypeDef(
-    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
-):
-    pass
-
-ApplicationsResponseTypeDef = TypedDict(
-    "ApplicationsResponseTypeDef",
+UpdateApnsChannelResponseTypeDef = TypedDict(
+    "UpdateApnsChannelResponseTypeDef",
     {
-        "Item": List[ApplicationResponseTypeDef],
-        "NextToken": str,
+        "APNSChannelResponse": APNSChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredApplicationSettingsResourceTypeDef = TypedDict(
-    "_RequiredApplicationSettingsResourceTypeDef",
+UpdateApnsSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelRequestRequestTypeDef",
     {
+        "APNSSandboxChannelRequest": APNSSandboxChannelRequestTypeDef,
         "ApplicationId": str,
     },
 )
-_OptionalApplicationSettingsResourceTypeDef = TypedDict(
-    "_OptionalApplicationSettingsResourceTypeDef",
+
+DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsSandboxChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "LastModifiedDate": str,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ApplicationSettingsResourceTypeDef(
-    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
-):
-    pass
+GetApnsSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsSandboxChannelResponseTypeDef",
+    {
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-WriteApplicationSettingsRequestTypeDef = TypedDict(
-    "WriteApplicationSettingsRequestTypeDef",
+UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsSandboxChannelResponseTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "CloudWatchMetricsEnabled": bool,
-        "EventTaggingEnabled": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
-    "UpdateBaiduChannelRequestRequestTypeDef",
+UpdateApnsVoipChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipChannelRequestRequestTypeDef",
     {
+        "APNSVoipChannelRequest": APNSVoipChannelRequestTypeDef,
         "ApplicationId": str,
-        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
-ChannelsResponseTypeDef = TypedDict(
-    "ChannelsResponseTypeDef",
+DeleteApnsVoipChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipChannelResponseTypeDef",
     {
-        "Channels": Dict[str, ChannelResponseTypeDef],
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ClosedDaysTypeDef = TypedDict(
-    "ClosedDaysTypeDef",
+GetApnsVoipChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipChannelResponseTypeDef",
     {
-        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
-        "SMS": Sequence[ClosedDaysRuleTypeDef],
-        "PUSH": Sequence[ClosedDaysRuleTypeDef],
-        "VOICE": Sequence[ClosedDaysRuleTypeDef],
-        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-WaitActivityTypeDef = TypedDict(
-    "WaitActivityTypeDef",
+UpdateApnsVoipChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipChannelResponseTypeDef",
     {
-        "NextActivity": str,
-        "WaitTime": WaitTimeTypeDef,
+        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
+UpdateApnsVoipSandboxChannelRequestRequestTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     {
-        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
+        "APNSVoipSandboxChannelRequest": APNSVoipSandboxChannelRequestTypeDef,
+        "ApplicationId": str,
     },
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "DeleteApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteAdmChannelResponseTypeDef = TypedDict(
-    "DeleteAdmChannelResponseTypeDef",
+GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "GetApnsVoipSandboxChannelResponseTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteApnsChannelResponseTypeDef = TypedDict(
-    "DeleteApnsChannelResponseTypeDef",
+UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
+    "UpdateApnsVoipSandboxChannelResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteApnsSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsSandboxChannelResponseTypeDef",
+_RequiredActivitiesResponseTypeDef = TypedDict(
+    "_RequiredActivitiesResponseTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Item": List[ActivityResponseTypeDef],
     },
 )
-
-DeleteApnsVoipChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipChannelResponseTypeDef",
+_OptionalActivitiesResponseTypeDef = TypedDict(
+    "_OptionalActivitiesResponseTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": str,
     },
+    total=False,
 )
 
-DeleteApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "DeleteApnsVoipSandboxChannelResponseTypeDef",
+class ActivitiesResponseTypeDef(
+    _RequiredActivitiesResponseTypeDef, _OptionalActivitiesResponseTypeDef
+):
+    pass
+
+ApplicationsResponseTypeDef = TypedDict(
+    "ApplicationsResponseTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Item": List[ApplicationResponseTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-DeleteAppResponseTypeDef = TypedDict(
-    "DeleteAppResponseTypeDef",
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
     {
         "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteBaiduChannelResponseTypeDef = TypedDict(
-    "DeleteBaiduChannelResponseTypeDef",
+DeleteAppResponseTypeDef = TypedDict(
+    "DeleteAppResponseTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+GetAppResponseTypeDef = TypedDict(
+    "GetAppResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationResponse": ApplicationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAdmChannelResponseTypeDef = TypedDict(
-    "GetAdmChannelResponseTypeDef",
+_RequiredApplicationSettingsResourceTypeDef = TypedDict(
+    "_RequiredApplicationSettingsResourceTypeDef",
     {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
     },
 )
-
-GetApnsChannelResponseTypeDef = TypedDict(
-    "GetApnsChannelResponseTypeDef",
+_OptionalApplicationSettingsResourceTypeDef = TypedDict(
+    "_OptionalApplicationSettingsResourceTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "LastModifiedDate": str,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
+    total=False,
 )
 
-GetApnsSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsSandboxChannelResponseTypeDef",
+class ApplicationSettingsResourceTypeDef(
+    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
+):
+    pass
+
+WriteApplicationSettingsRequestTypeDef = TypedDict(
+    "WriteApplicationSettingsRequestTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "CloudWatchMetricsEnabled": bool,
+        "EventTaggingEnabled": bool,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
+    total=False,
 )
 
-GetApnsVoipChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipChannelResponseTypeDef",
+RemoveAttributesResponseTypeDef = TypedDict(
+    "RemoveAttributesResponseTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AttributesResource": AttributesResourceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "GetApnsVoipSandboxChannelResponseTypeDef",
+UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
+    "UpdateBaiduChannelRequestRequestTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
+        "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
 
-GetAppResponseTypeDef = TypedDict(
-    "GetAppResponseTypeDef",
+DeleteBaiduChannelResponseTypeDef = TypedDict(
+    "DeleteBaiduChannelResponseTypeDef",
     {
-        "ApplicationResponse": ApplicationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBaiduChannelResponseTypeDef = TypedDict(
     "GetBaiduChannelResponseTypeDef",
     {
         "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RemoveAttributesResponseTypeDef = TypedDict(
-    "RemoveAttributesResponseTypeDef",
-    {
-        "AttributesResource": AttributesResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAdmChannelResponseTypeDef = TypedDict(
-    "UpdateAdmChannelResponseTypeDef",
-    {
-        "ADMChannelResponse": ADMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApnsChannelResponseTypeDef = TypedDict(
-    "UpdateApnsChannelResponseTypeDef",
+UpdateBaiduChannelResponseTypeDef = TypedDict(
+    "UpdateBaiduChannelResponseTypeDef",
     {
-        "APNSChannelResponse": APNSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApnsSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsSandboxChannelResponseTypeDef",
+ChannelsResponseTypeDef = TypedDict(
+    "ChannelsResponseTypeDef",
     {
-        "APNSSandboxChannelResponse": APNSSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
-UpdateApnsVoipChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipChannelResponseTypeDef",
+ClosedDaysTypeDef = TypedDict(
+    "ClosedDaysTypeDef",
     {
-        "APNSVoipChannelResponse": APNSVoipChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "EMAIL": Sequence[ClosedDaysRuleTypeDef],
+        "SMS": Sequence[ClosedDaysRuleTypeDef],
+        "PUSH": Sequence[ClosedDaysRuleTypeDef],
+        "VOICE": Sequence[ClosedDaysRuleTypeDef],
+        "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
     },
+    total=False,
 )
 
-UpdateApnsVoipSandboxChannelResponseTypeDef = TypedDict(
-    "UpdateApnsVoipSandboxChannelResponseTypeDef",
+WaitActivityTypeDef = TypedDict(
+    "WaitActivityTypeDef",
     {
-        "APNSVoipSandboxChannelResponse": APNSVoipSandboxChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextActivity": str,
+        "WaitTime": WaitTimeTypeDef,
     },
+    total=False,
 )
 
-UpdateBaiduChannelResponseTypeDef = TypedDict(
-    "UpdateBaiduChannelResponseTypeDef",
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
     {
-        "BaiduChannelResponse": BaiduChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CreateApplicationRequest": CreateApplicationRequestTypeDef,
     },
 )
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "EmailTemplateRequest": EmailTemplateRequestTypeDef,
@@ -3620,39 +3734,39 @@
 ):
     pass
 
 CreateEmailTemplateResponseTypeDef = TypedDict(
     "CreateEmailTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePushTemplateResponseTypeDef = TypedDict(
     "CreatePushTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSmsTemplateResponseTypeDef = TypedDict(
     "CreateSmsTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVoiceTemplateResponseTypeDef = TypedDict(
     "CreateVoiceTemplateResponseTypeDef",
     {
         "CreateTemplateMessageBody": CreateTemplateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateExportJobRequestRequestTypeDef = TypedDict(
     "CreateExportJobRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -3668,46 +3782,46 @@
     },
 )
 
 CreateInAppTemplateResponseTypeDef = TypedDict(
     "CreateInAppTemplateResponseTypeDef",
     {
         "TemplateCreateMessageBody": TemplateCreateMessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRecommenderConfigurationRequestRequestTypeDef = TypedDict(
     "CreateRecommenderConfigurationRequestRequestTypeDef",
     {
         "CreateRecommenderConfiguration": CreateRecommenderConfigurationTypeDef,
     },
 )
 
 CreateRecommenderConfigurationResponseTypeDef = TypedDict(
     "CreateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRecommenderConfigurationResponseTypeDef = TypedDict(
     "DeleteRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommenderConfigurationResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListRecommenderConfigurationsResponseTypeDef = TypedDict(
     "_RequiredListRecommenderConfigurationsResponseTypeDef",
     {
         "Item": List[RecommenderConfigurationResponseTypeDef],
@@ -3727,15 +3841,15 @@
 ):
     pass
 
 UpdateRecommenderConfigurationResponseTypeDef = TypedDict(
     "UpdateRecommenderConfigurationResponseTypeDef",
     {
         "RecommenderConfigurationResponse": RecommenderConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSmsTemplateRequestRequestTypeDef = TypedDict(
     "CreateSmsTemplateRequestRequestTypeDef",
     {
         "SMSTemplateRequest": SMSTemplateRequestTypeDef,
@@ -3856,231 +3970,231 @@
 ):
     pass
 
 DeleteEmailChannelResponseTypeDef = TypedDict(
     "DeleteEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEmailChannelResponseTypeDef = TypedDict(
     "GetEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailChannelResponseTypeDef = TypedDict(
     "UpdateEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEmailTemplateResponseTypeDef = TypedDict(
     "DeleteEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteInAppTemplateResponseTypeDef = TypedDict(
     "DeleteInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePushTemplateResponseTypeDef = TypedDict(
     "DeletePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSmsTemplateResponseTypeDef = TypedDict(
     "DeleteSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVoiceTemplateResponseTypeDef = TypedDict(
     "DeleteVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailTemplateResponseTypeDef = TypedDict(
     "UpdateEmailTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointResponseTypeDef = TypedDict(
     "UpdateEndpointResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointsBatchResponseTypeDef = TypedDict(
     "UpdateEndpointsBatchResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInAppTemplateResponseTypeDef = TypedDict(
     "UpdateInAppTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePushTemplateResponseTypeDef = TypedDict(
     "UpdatePushTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSmsTemplateResponseTypeDef = TypedDict(
     "UpdateSmsTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTemplateActiveVersionResponseTypeDef = TypedDict(
     "UpdateTemplateActiveVersionResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceTemplateResponseTypeDef = TypedDict(
     "UpdateVoiceTemplateResponseTypeDef",
     {
         "MessageBody": MessageBodyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEventStreamResponseTypeDef = TypedDict(
     "DeleteEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEventStreamResponseTypeDef = TypedDict(
     "GetEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutEventStreamResponseTypeDef = TypedDict(
     "PutEventStreamResponseTypeDef",
     {
         "EventStream": EventStreamTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteGcmChannelResponseTypeDef = TypedDict(
     "DeleteGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGcmChannelResponseTypeDef = TypedDict(
     "GetGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGcmChannelResponseTypeDef = TypedDict(
     "UpdateGcmChannelResponseTypeDef",
     {
         "GCMChannelResponse": GCMChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSmsChannelResponseTypeDef = TypedDict(
     "DeleteSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSmsChannelResponseTypeDef = TypedDict(
     "GetSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSmsChannelResponseTypeDef = TypedDict(
     "UpdateSmsChannelResponseTypeDef",
     {
         "SMSChannelResponse": SMSChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVoiceChannelResponseTypeDef = TypedDict(
     "DeleteVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceChannelResponseTypeDef = TypedDict(
     "GetVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceChannelResponseTypeDef = TypedDict(
     "UpdateVoiceChannelResponseTypeDef",
     {
         "VoiceChannelResponse": VoiceChannelResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEmailChannelRequestRequestTypeDef = TypedDict(
     "UpdateEmailChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4099,15 +4213,15 @@
     total=False,
 )
 
 GetEmailTemplateResponseTypeDef = TypedDict(
     "GetEmailTemplateResponseTypeDef",
     {
         "EmailTemplateResponse": EmailTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointBatchItemTypeDef = TypedDict(
     "EndpointBatchItemTypeDef",
     {
         "Address": str,
@@ -4318,39 +4432,57 @@
 ):
     pass
 
 GetJourneyExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     {
         "JourneyExecutionActivityMetricsResponse": JourneyExecutionActivityMetricsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyExecutionMetricsResponseTypeDef",
     {
         "JourneyExecutionMetricsResponse": JourneyExecutionMetricsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetJourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
+    "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
+    {
+        "JourneyRunExecutionActivityMetricsResponse": (
+            JourneyRunExecutionActivityMetricsResponseTypeDef
+        ),
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetJourneyRunExecutionMetricsResponseTypeDef = TypedDict(
+    "GetJourneyRunExecutionMetricsResponseTypeDef",
+    {
+        "JourneyRunExecutionMetricsResponse": JourneyRunExecutionMetricsResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSmsTemplateResponseTypeDef = TypedDict(
     "GetSmsTemplateResponseTypeDef",
     {
         "SMSTemplateResponse": SMSTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceTemplateResponseTypeDef = TypedDict(
     "GetVoiceTemplateResponseTypeDef",
     {
         "VoiceTemplateResponse": VoiceTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportJobResponseTypeDef = TypedDict(
     "_RequiredImportJobResponseTypeDef",
     {
         "ApplicationId": str,
@@ -4398,14 +4530,33 @@
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
     },
     total=False,
 )
 
+_RequiredJourneyRunsResponseTypeDef = TypedDict(
+    "_RequiredJourneyRunsResponseTypeDef",
+    {
+        "Item": List[JourneyRunResponseTypeDef],
+    },
+)
+_OptionalJourneyRunsResponseTypeDef = TypedDict(
+    "_OptionalJourneyRunsResponseTypeDef",
+    {
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class JourneyRunsResponseTypeDef(
+    _RequiredJourneyRunsResponseTypeDef, _OptionalJourneyRunsResponseTypeDef
+):
+    pass
+
 SMSMessageActivityTypeDef = TypedDict(
     "SMSMessageActivityTypeDef",
     {
         "MessageConfig": JourneySMSMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -4422,15 +4573,15 @@
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagsModel": TagsModelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -4464,15 +4615,15 @@
     },
 )
 
 PhoneNumberValidateResponseTypeDef = TypedDict(
     "PhoneNumberValidateResponseTypeDef",
     {
         "NumberValidateResponse": NumberValidateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
         "EMAIL": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
@@ -4627,15 +4778,15 @@
     },
 )
 
 VerifyOTPMessageResponseTypeDef = TypedDict(
     "VerifyOTPMessageResponseTypeDef",
     {
         "VerificationResponse": VerificationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VerifyOTPMessageRequestRequestTypeDef = TypedDict(
     "VerifyOTPMessageRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4643,39 +4794,39 @@
     },
 )
 
 GetCampaignActivitiesResponseTypeDef = TypedDict(
     "GetCampaignActivitiesResponseTypeDef",
     {
         "ActivitiesResponse": ActivitiesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppsResponseTypeDef = TypedDict(
     "GetAppsResponseTypeDef",
     {
         "ApplicationsResponse": ApplicationsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationSettingsResponseTypeDef = TypedDict(
     "GetApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationSettingsResponseTypeDef = TypedDict(
     "UpdateApplicationSettingsResponseTypeDef",
     {
         "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
     "UpdateApplicationSettingsRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4683,23 +4834,23 @@
     },
 )
 
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRecommenderConfigurationsResponseTypeDef = TypedDict(
     "GetRecommenderConfigurationsResponseTypeDef",
     {
         "ListRecommenderConfigurationsResponse": ListRecommenderConfigurationsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePushTemplateRequestRequestTypeDef = TypedDict(
     "CreatePushTemplateRequestRequestTypeDef",
     {
         "PushNotificationTemplateRequest": PushNotificationTemplateRequestTypeDef,
@@ -4729,15 +4880,15 @@
 ):
     pass
 
 GetPushTemplateResponseTypeDef = TypedDict(
     "GetPushTemplateResponseTypeDef",
     {
         "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointBatchRequestTypeDef = TypedDict(
     "EndpointBatchRequestTypeDef",
     {
         "Item": Sequence[EndpointBatchItemTypeDef],
@@ -4753,38 +4904,38 @@
     },
 )
 
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointsResponseTypeDef = TypedDict(
     "EndpointsResponseTypeDef",
     {
         "Item": List[EndpointResponseTypeDef],
     },
 )
 
 GetEndpointResponseTypeDef = TypedDict(
     "GetEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendUsersMessagesResponseTypeDef = TypedDict(
     "SendUsersMessagesResponseTypeDef",
     {
         "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CampaignEventFilterTypeDef = TypedDict(
     "CampaignEventFilterTypeDef",
     {
         "Dimensions": EventDimensionsTypeDef,
@@ -4825,15 +4976,15 @@
     },
 )
 
 CreateExportJobResponseTypeDef = TypedDict(
     "CreateExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredExportJobsResponseTypeDef = TypedDict(
     "_RequiredExportJobsResponseTypeDef",
     {
         "Item": List[ExportJobResponseTypeDef],
@@ -4852,15 +5003,15 @@
 ):
     pass
 
 GetExportJobResponseTypeDef = TypedDict(
     "GetExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
         "Country": SetDimensionTypeDef,
@@ -4869,23 +5020,23 @@
     total=False,
 )
 
 CreateImportJobResponseTypeDef = TypedDict(
     "CreateImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetImportJobResponseTypeDef = TypedDict(
     "GetImportJobResponseTypeDef",
     {
         "ImportJobResponse": ImportJobResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportJobsResponseTypeDef = TypedDict(
     "_RequiredImportJobsResponseTypeDef",
     {
         "Item": List[ImportJobResponseTypeDef],
@@ -4913,27 +5064,35 @@
         "ImageUrl": str,
         "PrimaryBtn": InAppMessageButtonTypeDef,
         "SecondaryBtn": InAppMessageButtonTypeDef,
     },
     total=False,
 )
 
+GetJourneyRunsResponseTypeDef = TypedDict(
+    "GetJourneyRunsResponseTypeDef",
+    {
+        "JourneyRunsResponse": JourneyRunsResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SendMessagesResponseTypeDef = TypedDict(
     "SendMessagesResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendOTPMessageResponseTypeDef = TypedDict(
     "SendOTPMessageResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BaseKpiResultTypeDef = TypedDict(
     "BaseKpiResultTypeDef",
     {
         "Rows": List[ResultRowTypeDef],
@@ -4954,23 +5113,23 @@
     total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesResponse": TemplatesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTemplateVersionsResponseTypeDef = TypedDict(
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionsResponse": TemplateVersionsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEndpointsBatchRequestRequestTypeDef = TypedDict(
     "UpdateEndpointsBatchRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -4978,23 +5137,23 @@
     },
 )
 
 DeleteUserEndpointsResponseTypeDef = TypedDict(
     "DeleteUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserEndpointsResponseTypeDef = TypedDict(
     "GetUserEndpointsResponseTypeDef",
     {
         "EndpointsResponse": EndpointsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": str,
@@ -5035,38 +5194,38 @@
     total=False,
 )
 
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "EventsResponse": EventsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventsRequestTypeDef = TypedDict(
     "EventsRequestTypeDef",
     {
         "BatchItem": Mapping[str, EventsBatchTypeDef],
     },
 )
 
 GetExportJobsResponseTypeDef = TypedDict(
     "GetExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentExportJobsResponseTypeDef = TypedDict(
     "GetSegmentExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
@@ -5079,23 +5238,23 @@
     total=False,
 )
 
 GetImportJobsResponseTypeDef = TypedDict(
     "GetImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentImportJobsResponseTypeDef = TypedDict(
     "GetSegmentImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CampaignInAppMessageTypeDef = TypedDict(
     "CampaignInAppMessageTypeDef",
     {
         "Body": str,
@@ -5343,39 +5502,39 @@
 ):
     pass
 
 GetInAppTemplateResponseTypeDef = TypedDict(
     "GetInAppTemplateResponseTypeDef",
     {
         "InAppTemplateResponse": InAppTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "GetApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationDateRangeKpiResponse": ApplicationDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignDateRangeKpiResponseTypeDef = TypedDict(
     "GetCampaignDateRangeKpiResponseTypeDef",
     {
         "CampaignDateRangeKpiResponse": CampaignDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyDateRangeKpiResponseTypeDef = TypedDict(
     "GetJourneyDateRangeKpiResponseTypeDef",
     {
         "JourneyDateRangeKpiResponse": JourneyDateRangeKpiResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMessageRequestTypeDef = TypedDict(
     "_RequiredMessageRequestTypeDef",
     {
         "MessageConfiguration": DirectMessageConfigurationTypeDef,
@@ -5642,47 +5801,47 @@
     total=False,
 )
 
 GetInAppMessagesResponseTypeDef = TypedDict(
     "GetInAppMessagesResponseTypeDef",
     {
         "InAppMessagesResponse": InAppMessagesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteSegmentResponseTypeDef = TypedDict(
     "DeleteSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentVersionResponseTypeDef = TypedDict(
     "GetSegmentVersionResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSegmentsResponseTypeDef = TypedDict(
     "_RequiredSegmentsResponseTypeDef",
     {
         "Item": List[SegmentResponseTypeDef],
@@ -5699,15 +5858,15 @@
 class SegmentsResponseTypeDef(_RequiredSegmentsResponseTypeDef, _OptionalSegmentsResponseTypeDef):
     pass
 
 UpdateSegmentResponseTypeDef = TypedDict(
     "UpdateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5761,47 +5920,47 @@
 ):
     pass
 
 CreateCampaignResponseTypeDef = TypedDict(
     "CreateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCampaignResponseTypeDef = TypedDict(
     "DeleteCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignResponseTypeDef = TypedDict(
     "GetCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignVersionResponseTypeDef = TypedDict(
     "GetCampaignVersionResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCampaignResponseTypeDef = TypedDict(
     "UpdateCampaignResponseTypeDef",
     {
         "CampaignResponse": CampaignResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCampaignRequestRequestTypeDef = TypedDict(
     "CreateCampaignRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5818,23 +5977,23 @@
     },
 )
 
 GetSegmentVersionsResponseTypeDef = TypedDict(
     "GetSegmentVersionsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSegmentsResponseTypeDef = TypedDict(
     "GetSegmentsResponseTypeDef",
     {
         "SegmentsResponse": SegmentsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJourneyResponseTypeDef = TypedDict(
     "_RequiredJourneyResponseTypeDef",
     {
         "ApplicationId": str,
@@ -5905,47 +6064,47 @@
 ):
     pass
 
 GetCampaignVersionsResponseTypeDef = TypedDict(
     "GetCampaignVersionsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCampaignsResponseTypeDef = TypedDict(
     "GetCampaignsResponseTypeDef",
     {
         "CampaignsResponse": CampaignsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateJourneyResponseTypeDef = TypedDict(
     "CreateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteJourneyResponseTypeDef = TypedDict(
     "DeleteJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJourneyResponseTypeDef = TypedDict(
     "GetJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJourneysResponseTypeDef = TypedDict(
     "_RequiredJourneysResponseTypeDef",
     {
         "Item": List[JourneyResponseTypeDef],
@@ -5962,23 +6121,23 @@
 class JourneysResponseTypeDef(_RequiredJourneysResponseTypeDef, _OptionalJourneysResponseTypeDef):
     pass
 
 UpdateJourneyResponseTypeDef = TypedDict(
     "UpdateJourneyResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateJourneyStateResponseTypeDef = TypedDict(
     "UpdateJourneyStateResponseTypeDef",
     {
         "JourneyResponse": JourneyResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateJourneyRequestRequestTypeDef = TypedDict(
     "CreateJourneyRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -5995,10 +6154,10 @@
     },
 )
 
 ListJourneysResponseTypeDef = TypedDict(
     "ListJourneysResponseTypeDef",
     {
         "JourneysResponse": JourneysResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Pinpoint 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.120
+Summary: Type annotations for boto3.Pinpoint 1.26.120 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-pinpoint"></a>
 
 # mypy-boto3-pinpoint
 
 [![PyPI - mypy-boto3-pinpoint](https://img.shields.io/pypi/v/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.26.120](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,14 +291,15 @@
     DurationType,
     EndpointTypesElementType,
     FilterTypeType,
     FormatType,
     FrequencyType,
     IncludeType,
     JobStatusType,
+    JourneyRunStatusType,
     LayoutType,
     MessageTypeType,
     ModeType,
     OperatorType,
     RecencyTypeType,
     SegmentTypeType,
     SourceTypeType,
@@ -356,15 +358,14 @@
     CampaignStateTypeDef,
     CustomDeliveryConfigurationTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
     ClosedDaysRuleTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
-    ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
@@ -407,14 +408,15 @@
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
     EndpointItemResponseTypeDef,
     EndpointMessageResultTypeDef,
     EndpointSendConfigurationTypeDef,
     MetricDimensionTypeDef,
@@ -454,14 +456,19 @@
     GetInAppTemplateRequestRequestTypeDef,
     GetJourneyDateRangeKpiRequestRequestTypeDef,
     GetJourneyExecutionActivityMetricsRequestRequestTypeDef,
     JourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsRequestRequestTypeDef,
     JourneyExecutionMetricsResponseTypeDef,
     GetJourneyRequestRequestTypeDef,
+    GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef,
+    JourneyRunExecutionActivityMetricsResponseTypeDef,
+    GetJourneyRunExecutionMetricsRequestRequestTypeDef,
+    JourneyRunExecutionMetricsResponseTypeDef,
+    GetJourneyRunsRequestRequestTypeDef,
     GetPushTemplateRequestRequestTypeDef,
     GetRecommenderConfigurationRequestRequestTypeDef,
     GetRecommenderConfigurationsRequestRequestTypeDef,
     GetSegmentExportJobsRequestRequestTypeDef,
     GetSegmentImportJobsRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     GetSegmentVersionRequestRequestTypeDef,
@@ -478,14 +485,15 @@
     InAppMessageBodyConfigTypeDef,
     OverrideButtonConfigurationTypeDef,
     InAppMessageHeaderConfigTypeDef,
     JourneyChannelSettingsTypeDef,
     JourneyLimitsTypeDef,
     JourneyPushMessageTypeDef,
     JourneyScheduleTypeDef,
+    JourneyRunResponseTypeDef,
     JourneySMSMessageTypeDef,
     JourneyStateRequestTypeDef,
     ListJourneysRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagsModelTypeDef,
     ListTemplateVersionsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
@@ -494,14 +502,15 @@
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
     RandomSplitEntryTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
+    ResponseMetadataTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
     SegmentConditionTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
@@ -511,50 +520,49 @@
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
     VerifyOTPMessageRequestParametersTypeDef,
     UpdateAdmChannelRequestRequestTypeDef,
+    DeleteAdmChannelResponseTypeDef,
+    GetAdmChannelResponseTypeDef,
+    UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
+    DeleteApnsChannelResponseTypeDef,
+    GetApnsChannelResponseTypeDef,
+    UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
+    DeleteApnsSandboxChannelResponseTypeDef,
+    GetApnsSandboxChannelResponseTypeDef,
+    UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
+    DeleteApnsVoipChannelResponseTypeDef,
+    GetApnsVoipChannelResponseTypeDef,
+    UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
+    DeleteApnsVoipSandboxChannelResponseTypeDef,
+    GetApnsVoipSandboxChannelResponseTypeDef,
+    UpdateApnsVoipSandboxChannelResponseTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
+    CreateAppResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    GetAppResponseTypeDef,
     ApplicationSettingsResourceTypeDef,
     WriteApplicationSettingsRequestTypeDef,
+    RemoveAttributesResponseTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
+    DeleteBaiduChannelResponseTypeDef,
+    GetBaiduChannelResponseTypeDef,
+    UpdateBaiduChannelResponseTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
-    CreateAppResponseTypeDef,
-    DeleteAdmChannelResponseTypeDef,
-    DeleteApnsChannelResponseTypeDef,
-    DeleteApnsSandboxChannelResponseTypeDef,
-    DeleteApnsVoipChannelResponseTypeDef,
-    DeleteApnsVoipSandboxChannelResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    DeleteBaiduChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAdmChannelResponseTypeDef,
-    GetApnsChannelResponseTypeDef,
-    GetApnsSandboxChannelResponseTypeDef,
-    GetApnsVoipChannelResponseTypeDef,
-    GetApnsVoipSandboxChannelResponseTypeDef,
-    GetAppResponseTypeDef,
-    GetBaiduChannelResponseTypeDef,
-    RemoveAttributesResponseTypeDef,
-    UpdateAdmChannelResponseTypeDef,
-    UpdateApnsChannelResponseTypeDef,
-    UpdateApnsSandboxChannelResponseTypeDef,
-    UpdateApnsVoipChannelResponseTypeDef,
-    UpdateApnsVoipSandboxChannelResponseTypeDef,
-    UpdateBaiduChannelResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     CreateEmailTemplateResponseTypeDef,
     CreatePushTemplateResponseTypeDef,
     CreateSmsTemplateResponseTypeDef,
     CreateVoiceTemplateResponseTypeDef,
     CreateExportJobRequestRequestTypeDef,
@@ -614,19 +622,22 @@
     ItemResponseTypeDef,
     EventTypeDef,
     ExportJobResponseTypeDef,
     UpdateGcmChannelRequestRequestTypeDef,
     GPSPointDimensionTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
+    GetJourneyRunExecutionActivityMetricsResponseTypeDef,
+    GetJourneyRunExecutionMetricsResponseTypeDef,
     GetSmsTemplateResponseTypeDef,
     GetVoiceTemplateResponseTypeDef,
     ImportJobResponseTypeDef,
     InAppMessageButtonTypeDef,
     PushMessageActivityTypeDef,
+    JourneyRunsResponseTypeDef,
     SMSMessageActivityTypeDef,
     UpdateJourneyStateRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     MessageResponseTypeDef,
     PhoneNumberValidateRequestRequestTypeDef,
     PhoneNumberValidateResponseTypeDef,
@@ -672,14 +683,15 @@
     ExportJobsResponseTypeDef,
     GetExportJobResponseTypeDef,
     SegmentLocationTypeDef,
     CreateImportJobResponseTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobsResponseTypeDef,
     InAppMessageContentTypeDef,
+    GetJourneyRunsResponseTypeDef,
     SendMessagesResponseTypeDef,
     SendOTPMessageResponseTypeDef,
     BaseKpiResultTypeDef,
     EmailMessageTypeDef,
     ListTemplatesResponseTypeDef,
     ListTemplateVersionsResponseTypeDef,
     UpdateEndpointsBatchRequestRequestTypeDef,
@@ -774,42 +786,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-pinpoint-1.26.0.post1/mypy_boto3_pinpoint.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-1.26.120/mypy_boto3_pinpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.26.0.post1/setup.py` & `mypy-boto3-pinpoint-1.26.120/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-pinpoint.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint",
-    version="1.26.0.post1",
+    version="1.26.120",
     packages=["mypy_boto3_pinpoint"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Pinpoint 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.Pinpoint 1.26.120 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 pinpoint type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_pinpoint": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_pinpoint": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

