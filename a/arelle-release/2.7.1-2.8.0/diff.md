# Comparing `tmp/arelle-release-2.7.1.tar.gz` & `tmp/arelle-release-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arelle-release-2.7.1.tar", last modified: Tue Apr 18 22:25:38 2023, max compression
+gzip compressed data, was "arelle-release-2.8.0.tar", last modified: Tue Apr 25 16:38:16 2023, max compression
```

## Comparing `arelle-release-2.7.1.tar` & `arelle-release-2.8.0.tar`

### file list

```diff
@@ -1,747 +1,747 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.026026 arelle-release-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.906024 arelle-release-2.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.906024 arelle-release-2.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/ISSUE_TEMPLATE/change.yml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.910024 arelle-release-2.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/workflows/build-and-release-linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/workflows/build-and-release-mac.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/workflows/build-and-release-windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/workflows/build-windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/workflows/conformance-suites.yml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/workflows/project.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/workflows/test-ui.yml
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-18 22:25:21.000000 arelle-release-2.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-18 22:25:21.000000 arelle-release-2.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 22:25:21.000000 arelle-release-2.7.1/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-18 22:25:21.000000 arelle-release-2.7.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-18 22:25:21.000000 arelle-release-2.7.1/EFM-only-test.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-18 22:25:21.000000 arelle-release-2.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-18 22:25:38.030026 arelle-release-2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-18 22:25:21.000000 arelle-release-2.7.1/QuickBooks.qwc
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-18 22:25:21.000000 arelle-release-2.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.910024 arelle-release-2.7.1/apidocs/
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-18 22:25:21.000000 arelle-release-2.7.1/apidocs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-18 22:25:21.000000 arelle-release-2.7.1/apidocs/arelle.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-18 22:25:21.000000 arelle-release-2.7.1/apidocs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-18 22:25:21.000000 arelle-release-2.7.1/apidocs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-18 22:25:21.000000 arelle-release-2.7.1/apidocs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 22:25:21.000000 arelle-release-2.7.1/apidocs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.926024 arelle-release-2.7.1/arelle/
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/Aspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    39928 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/Cntlr.py
--rw-r--r--   0 runner    (1001) docker     (123)    76322 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/CntlrCmdLine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/CntlrComServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/CntlrProfiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31445 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/CntlrQuickBooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    48719 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/CntlrWebMain.py
--rw-r--r--   0 runner    (1001) docker     (123)    88038 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/CntlrWinMain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/CntlrWinTooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogAbout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogArcroleGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19419 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogFind.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogFormulaParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogLanguage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogNewFactItem.py
--rw-r--r--   0 runner    (1001) docker     (123)    24340 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogOpenArchive.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogOpenTaxonomyPackage.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogPackageManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    32913 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogPluginManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogRssWatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogURL.py
--rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DialogUserPassword.py
--rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/DisclosureSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    43688 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/FileSource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/FunctionCustom.py
--rw-r--r--   0 runner    (1001) docker     (123)    36519 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/FunctionFn.py
--rw-r--r--   0 runner    (1001) docker     (123)    80279 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/FunctionIxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/FunctionUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)    71334 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/FunctionXfi.py
--rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/FunctionXs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/HashUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/HtmlUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/InstanceAspectsEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/LeiUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/LocalViewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28242 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/Locale.py
--rw-r--r--   0 runner    (1001) docker     (123)   119586 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelDocument.py
--rw-r--r--   0 runner    (1001) docker     (123)    88883 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelDtsObject.py
--rw-r--r--   0 runner    (1001) docker     (123)   122124 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelFormulaObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    72084 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelInstanceObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18455 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelObjectFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21424 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelRelationshipSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    70336 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelRenderingObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelRssItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelRssObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelTestcaseObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    38714 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelValue.py
--rw-r--r--   0 runner    (1001) docker     (123)    26062 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelVersObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    73327 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelVersReport.py
--rw-r--r--   0 runner    (1001) docker     (123)    69922 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ModelXbrl.py
--rw-r--r--   0 runner    (1001) docker     (123)    31672 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/PackageManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    29001 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/PluginManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/PrototypeDtsObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/PrototypeInstanceObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/PythonUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/RenderingEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43733 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/RenderingResolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/SystemInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    29404 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/TableStructure.py
--rw-r--r--   0 runner    (1001) docker     (123)    32276 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/TkTableWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    39250 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/UITkTable.py
--rw-r--r--   0 runner    (1001) docker     (123)    34218 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/UiUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/Updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    32121 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/UrlUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)    49309 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/Validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    51377 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ValidateFilingText.py
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ValidateInfoset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ValidateUtr.py
--rw-r--r--   0 runner    (1001) docker     (123)    43196 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ValidateVersReport.py
--rw-r--r--   0 runner    (1001) docker     (123)    75131 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ValidateXbrl.py
--rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ValidateXbrlCalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)   100180 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ValidateXbrlDTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    38118 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ValidateXbrlDimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/Version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewFileConcepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewFileDTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewFileFactList.py
--rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewFileFactTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewFileFormulae.py
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewFileRelationshipSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewFileRenderedGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewFileRoleTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewFileRssFeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewFileTests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewUtilFormulae.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinConcepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinDTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinDiffs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinFactGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinFactList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinFactTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinFormulae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinList.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinPane.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinRelationshipSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    78864 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinRenderedGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinRoleTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinRssFeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinTests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinTkTable.py
--rw-r--r--   0 runner    (1001) docker     (123)    19434 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinTree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinTupleGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinVersReport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/ViewWinXml.py
--rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/WatchRss.py
--rw-r--r--   0 runner    (1001) docker     (123)    36553 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/WebCache.py
--rw-r--r--   0 runner    (1001) docker     (123)    62211 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/XbrlConst.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/XbrlUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/XhtmlValidate.py
--rw-r--r--   0 runner    (1001) docker     (123)    56964 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/XmlUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)    44546 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/XmlValidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/XmlValidateParticles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/XmlValidateSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 22:25:37.000000 arelle-release-2.7.1/arelle/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.930024 arelle-release-2.7.1/arelle/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/arelle_test.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/creationSoftwareNames.json
--rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/disclosuresystems.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/disclosuresystems.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/edbody.dtd
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/empty-instance.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/erxl.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/mappings.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/mappings.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/xbrlschemafiles.xml
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/xhtml-lat1.ent
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/xhtml-special.ent
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/xhtml-symbol.ent
--rw-r--r--   0 runner    (1001) docker     (123)    26880 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/xhtml1-strict-ix.dtd
--rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/config/xhtml1_1-strict-ix.dtd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.930024 arelle-release-2.7.1/arelle/doc/
--rw-r--r--   0 runner    (1001) docker     (123)   458032 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/doc/messagesCatalog.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/doc/messagesCatalog.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.930024 arelle-release-2.7.1/arelle/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/.pydevproject
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/CustomLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/LoadEFMvalidate.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/LoadSavePreLbCsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/LoadValidate.cs
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/LoadValidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/LoadValidateCmdLine.java
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/LoadValidatePostedZip.java
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/LoadValidateWebService.java
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/SaveTableToExelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/TR3toTR4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.934024 arelle-release-2.7.1/arelle/examples/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/bigInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/cmdWebServerExtension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/crashTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/formulaSuiteConverter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/functionsCustom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/hello_dolly.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/hello_i18n.pot
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/hello_i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/importTestChild1.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/importTestChild2.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/importTestGrandchild1.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/importTestGrandchild2.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/importTestImported1.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/importTestImported11.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/importTestParent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.894024 arelle-release-2.7.1/arelle/examples/plugin/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.894024 arelle-release-2.7.1/arelle/examples/plugin/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.934024 arelle-release-2.7.1/arelle/examples/plugin/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/locale/fr/LC_MESSAGES/hello_i18n.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.934024 arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/importTestChild1.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/importTestChild2.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/importTestGrandchild1.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/importTestGrandchild2.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/importTestImported1.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/importTestImported11.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.934024 arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/subdir/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/subdir/importTestImported111.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.934024 arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/importTestImported1111.py
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/sakaCalendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/saveInstanceInfoset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/streamingExtensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/testcaseIxExpectedHtmlFixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/updateTableLB.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/validateSchemaLxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/plugin/validateTableInfoset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/us-gaap-dei-docType-extraction-frm.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/examples/us-gaap-dei-ratio-cash-frm.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.938024 arelle-release-2.7.1/arelle/formula/
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/formula/FactAspectsCache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/formula/FormulaConsisAsser.py
--rw-r--r--   0 runner    (1001) docker     (123)    83178 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/formula/FormulaEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    98324 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/formula/ValidateFormula.py
--rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/formula/XPathContext.py
--rw-r--r--   0 runner    (1001) docker     (123)    49913 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/formula/XPathParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/formula/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.942025 arelle-release-2.7.1/arelle/images/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/arelle-full-word.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/arelle-mac-icon-4.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/arelle-word-only.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/arelle.gif
--rw-r--r--   0 runner    (1001) docker     (123)   212911 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/arelle.icns
--rw-r--r--   0 runner    (1001) docker     (123)   392859 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/arelle.icns.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/arelle.ico
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/arelle.xbm
--rw-r--r--   0 runner    (1001) docker     (123)   269858 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/arelle128.psd
--rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/arelle16.psd
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/arelle16x16and32x32.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/arelle32.gif
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/columnSortDown.gif
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/columnSortUp.gif
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/dmg_background.png
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/octocat.png
--rw-r--r--   0 runner    (1001) docker     (123)    23863 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/python-clear.png
--rw-r--r--   0 runner    (1001) docker     (123)   696358 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/python-icon-pack-crystalxp.net-842.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarClose.gif
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarCompare.gif
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarDelete.gif
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarFindMenu.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarLogClear - 1-piece-top.gif
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarLogClear-orig.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarLogClear.gif
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarNewFile.gif
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarOpenDatabase.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarOpenFile.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarOpenWeb.gif
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarProperties.gif
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarQuit.gif
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarReopen.gif
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarSaveFile.gif
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/toolbarValidate.gif
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/xbrl.gif
--rw-r--r--   0 runner    (1001) docker     (123)   201686 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/xbrl.psd
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/xbrl128-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/xbrl128.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/xbrl16.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/images/xbrl32.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.942025 arelle-release-2.7.1/arelle/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.894024 arelle-release-2.7.1/arelle/locale/ar_EG/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.942025 arelle-release-2.7.1/arelle/locale/ar_EG/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   341883 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/locale/ar_EG/LC_MESSAGES/ar_EG.po
--rw-r--r--   0 runner    (1001) docker     (123)   185904 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/locale/ar_EG/LC_MESSAGES/arelle.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.898024 arelle-release-2.7.1/arelle/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.946025 arelle-release-2.7.1/arelle/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   149331 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/locale/es/LC_MESSAGES/arelle.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.898024 arelle-release-2.7.1/arelle/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.946025 arelle-release-2.7.1/arelle/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   118897 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/locale/fr/LC_MESSAGES/arelle.mo
--rw-r--r--   0 runner    (1001) docker     (123)   168077 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/locale/fr/LC_MESSAGES/fr.po
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/locale/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)   249762 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/locale/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.898024 arelle-release-2.7.1/arelle/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.946025 arelle-release-2.7.1/arelle/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   375378 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/locale/ru/LC_MESSAGES/arelle.mo
--rw-r--r--   0 runner    (1001) docker     (123)   449579 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/locale/ru/LC_MESSAGES/ru.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.950025 arelle-release-2.7.1/arelle/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/EdgarRendererAllReports.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/SECCorrespondenceLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/TDnetLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/UKCompaniesHouseLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)   101637 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/formulaLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)    31396 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/formulaSaver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/formulaXPathChecker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/functionsMath.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/functionsXmlCreation.py
--rw-r--r--   0 runner    (1001) docker     (123)    37223 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/inlineXbrlDocumentSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/instanceInfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.898024 arelle-release-2.7.1/arelle/plugin/internet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.950025 arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/HTTPNtlmAuthHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/U32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/des.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/des_c.py
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/des_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/lgpl-3.0-standalone.html
--rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/ntlm.py
--rw-r--r--   0 runner    (1001) docker     (123)   124382 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/loadFromExcel.py
--rw-r--r--   0 runner    (1001) docker     (123)    76473 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/loadFromOIM-2018.py
--rw-r--r--   0 runner    (1001) docker     (123)   195836 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/loadFromOIM.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.954025 arelle-release-2.7.1/arelle/plugin/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/logging/dpmSignature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/logging/dqcParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/logging/saveMessages.py
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/objectmaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/profileCmdLine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/profileFormula.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/saveCHComponentFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/saveDTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/saveHtmlEBAtables.py
--rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/saveLoadableExcel.py
--rw-r--r--   0 runner    (1001) docker     (123)    32261 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/saveLoadableOIM.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/saveSKOS.py
--rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/saveSampleInstance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.954025 arelle-release-2.7.1/arelle/plugin/security/
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/security/cryptAES_CBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/security/cryptAES_EAX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.954025 arelle-release-2.7.1/arelle/plugin/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/sphinx/FormulaGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19516 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/sphinx/SphinxContext.py
--rw-r--r--   0 runner    (1001) docker     (123)    35742 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/sphinx/SphinxEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    49810 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/sphinx/SphinxMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    48614 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/sphinx/SphinxParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/sphinx/SphinxValidator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/sphinx/US-GAAP Ratios Example.xsr
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47646 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/streamingExtensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.954025 arelle-release-2.7.1/arelle/plugin/transforms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.954025 arelle-release-2.7.1/arelle/plugin/transforms/SEC/
--rw-r--r--   0 runner    (1001) docker     (123)    41892 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.962025 arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/extractTestcase.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/extractTestcase.xsl
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/runIxtSecTests.sh
--rw-r--r--   0 runner    (1001) docker     (123)  4737705 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/saxon9.jar
--rw-r--r--   0 runner    (1001) docker     (123)   225611 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/testcase.xml
--rw-r--r--   0 runner    (1001) docker     (123)    59680 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/tests.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/text2num.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.898024 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.962025 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-boolballotbox.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-countrynameen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-datequarterend.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durday.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durhour.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durmonth.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durweek.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durwordsen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-duryear.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-edgarprovcountryen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-entityfilercategoryen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-exchnameen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-numwordsen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-stateprovnameen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-yesnoballotbox.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/transform-registry.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.962025 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    55540 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/schema/inlinexbrl-sec-transformation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/transforms/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/unpackSecEisFile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.966025 arelle-release-2.7.1/arelle/plugin/validate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.966025 arelle-release-2.7.1/arelle/plugin/validate/CIPC/
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/CIPC/Const.py
--rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/CIPC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/CIPC/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.966025 arelle-release-2.7.1/arelle/plugin/validate/EBA/
--rw-r--r--   0 runner    (1001) docker     (123)    45950 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EBA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EBA/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.966025 arelle-release-2.7.1/arelle/plugin/validate/EFM/
--rw-r--r--   0 runner    (1001) docker     (123)    16365 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/Consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    40582 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/DTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/Dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/Document.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   253045 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/Filing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/PreCalAlignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    37995 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    42471 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.978025 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/axiswarnings.json
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/cef-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/country-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/currency-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/dei-deprecated-concepts.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   113832 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/dei-validations.json
--rw-r--r--   0 runner    (1001) docker     (123)    76859 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/dqc-us-rules.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/ecd-deprecated-concepts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.990025 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/
--rw-r--r--   0 runner    (1001) docker     (123)    31435 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-16-4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    76545 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-0-4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    76785 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    73012 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    80115 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-3-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   150333 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   138364 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.2.xml
--rw-r--r--   0 runner    (1001) docker     (123)   135467 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.3.xml
--rw-r--r--   0 runner    (1001) docker     (123)   180977 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   125792 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)   119973 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-3.xml
--rw-r--r--   0 runner    (1001) docker     (123)   134456 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   109498 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    99358 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-3.xml
--rw-r--r--   0 runner    (1001) docker     (123)    28394 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2012.xml
--rw-r--r--   0 runner    (1001) docker     (123)    29132 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2013.xml
--rw-r--r--   0 runner    (1001) docker     (123)    29744 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2014.xml
--rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2015.xml
--rw-r--r--   0 runner    (1001) docker     (123)    31676 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2016.xml
--rw-r--r--   0 runner    (1001) docker     (123)   109944 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    39675 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    35860 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-3.xml
--rw-r--r--   0 runner    (1001) docker     (123)    42433 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    58455 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1-preview.xml
--rw-r--r--   0 runner    (1001) docker     (123)    62455 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    49163 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    48412 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    57294 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    69072 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    69638 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   368244 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-all-years.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/erxl.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/extendedtaxonomies-all-years.xml
--rw-r--r--   0 runner    (1001) docker     (123)    93735 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrs-taxonomies.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrstaxonomies-all-years.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/exch-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/ifrs-full-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/invest-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/ixbrl-transform-registries.json
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/naics-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/other-standard-taxonomies.json
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/rr-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/sic-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/signwarnings.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/srt-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/stpr-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/taxonomy-compatibility.json
--rw-r--r--   0 runner    (1001) docker     (123)   205448 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/us-gaap-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)  1583747 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2020.json
--rw-r--r--   0 runner    (1001) docker     (123)  1624986 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2021.json
--rw-r--r--   0 runner    (1001) docker     (123)  1593440 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2022.json
--rw-r--r--   0 runner    (1001) docker     (123)  1613560 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2023.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/vip-deprecated-concepts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.990025 arelle-release-2.7.1/arelle/plugin/validate/EFM/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM/tools/CheckTxmyRefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.966025 arelle-release-2.7.1/arelle/plugin/validate/EFM-htm/
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM-htm/Const.py
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM-htm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM-htm/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.966025 arelle-release-2.7.1/arelle/plugin/validate/EFM-htm/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/EFM-htm/resources/efm-htm.dtd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.990025 arelle-release-2.7.1/arelle/plugin/validate/ESEF/
--rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF/Const.py
--rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF/DTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF/Dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF/Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    75653 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.990025 arelle-release-2.7.1/arelle/plugin/validate/ESEF/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF/resources/authority-validations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.990025 arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/
--rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/Const.py
--rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/DTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/Dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    81822 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.990025 arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/resources/authority-validations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.990025 arelle-release-2.7.1/arelle/plugin/validate/FERC/
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/FERC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/FERC/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.990025 arelle-release-2.7.1/arelle/plugin/validate/FERC/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/FERC/resources/ferc-utr.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.994025 arelle-release-2.7.1/arelle/plugin/validate/GFM/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/GFM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/GFM/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.994025 arelle-release-2.7.1/arelle/plugin/validate/HMRC/
--rw-r--r--   0 runner    (1001) docker     (123)    29346 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/HMRC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/HMRC/config.xml
--rw-r--r--   0 runner    (1001) docker     (123)    25247 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/HMRC/consistencyChecksByName.json
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/HMRC/hmrc-taxonomies.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.994025 arelle-release-2.7.1/arelle/plugin/validate/ROS/
--rw-r--r--   0 runner    (1001) docker     (123)    19281 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ROS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/ROS/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.994025 arelle-release-2.7.1/arelle/plugin/validate/SBRnl/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/SBRnl/CustomLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/SBRnl/DTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/SBRnl/Dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    59358 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/SBRnl/Document.py
--rw-r--r--   0 runner    (1001) docker     (123)    29571 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/SBRnl/Filing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/SBRnl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/SBRnl/config.xml
--rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/SBRnl/sbr-nl-taxonomies.xml
--rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/USBestPractices.py
--rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/USCorpAction.py
--rw-r--r--   0 runner    (1001) docker     (123)    18558 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/USSecTagging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.994025 arelle-release-2.7.1/arelle/plugin/validate/XDC/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/XDC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/XDC/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.994025 arelle-release-2.7.1/arelle/plugin/validate/XFsyntax/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/XFsyntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66728 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/XFsyntax/xf.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31565 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validate/calc2.py
--rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/validateSBRnl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.998025 arelle-release-2.7.1/arelle/plugin/xbrlDB/
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/DialogRssWatchExtender.py
--rw-r--r--   0 runner    (1001) docker     (123)    56450 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/SqlDb.py
--rw-r--r--   0 runner    (1001) docker     (123)    78257 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlDpmSqlDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    78348 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlOpenSqlDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    36203 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlPublicPostgresDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    64539 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlSemanticGraphDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    48567 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlSemanticJsonDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    55073 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlSemanticRdfDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    67782 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlSemanticSqlDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/entityInformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.998025 arelle-release-2.7.1/arelle/plugin/xbrlDB/ext/
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/ext/china.py
--rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/ext/edgar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/ext/xdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/primaryDocumentFacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.902024 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.998025 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.002025 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open/ext/chinaPostgresDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)   714004 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open/ext/edgarPostgresDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open/ext/xdcPostgresDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open/xbrlOpenPostgresDB.ddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.002025 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open2/
--rw-r--r--   0 runner    (1001) docker     (123)   728541 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open2/xbrlOpen2PostgresDB.ddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.002025 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/public/
--rw-r--r--   0 runner    (1001) docker     (123)   963416 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/public/xbrlPublicPostgresDB.ddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.010026 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/secDatabaseModelViews.sql
--rw-r--r--   0 runner    (1001) docker     (123)    21988 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticColumnComments.ddl
--rw-r--r--   0 runner    (1001) docker     (123)   728214 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMSSqlDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)   729124 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMySqlDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)  1056221 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticOracleDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)   727913 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticPostgresDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)   726301 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticSQLiteDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xbrlDB/tableFacts.py
--rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/plugin/xuleSaver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.010026 arelle-release-2.7.1/arelle/scripts-macOS/
--rwxr-xr-x   0 runner    (1001) docker     (123)       91 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/scripts-macOS/startWebServer.command
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.010026 arelle-release-2.7.1/arelle/scripts-unix/
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/scripts-unix/startWebServer.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.010026 arelle-release-2.7.1/arelle/scripts-windows/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/scripts-windows/exportCsvFromXbrlInstance.bat
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/scripts-windows/runEFMTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/scripts-windows/runFormulaTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/scripts-windows/runFunctionTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/scripts-windows/runXBRL21Tests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/scripts-windows/runXDTTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/scripts-windows/startWebServer.bat
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/scripts-windows/validateAndRunFormulas.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.010026 arelle-release-2.7.1/arelle/webserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   116069 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/webserver/bottle-no2to3.py
--rw-r--r--   0 runner    (1001) docker     (123)   171083 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle/webserver/bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle.pyw
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelleCmdLine.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelleGUI.pyw
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.014026 arelle-release-2.7.1/arelle_release.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-18 22:25:37.000000 arelle-release-2.7.1/arelle_release.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26653 2023-04-18 22:25:37.000000 arelle-release-2.7.1/arelle_release.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:25:37.000000 arelle-release-2.7.1/arelle_release.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 22:25:37.000000 arelle-release-2.7.1/arelle_release.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-18 22:25:37.000000 arelle-release-2.7.1/arelle_release.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 22:25:37.000000 arelle-release-2.7.1/arelle_release.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-18 22:25:21.000000 arelle-release-2.7.1/arelle_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.014026 arelle-release-2.7.1/attic/
--rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-04-18 22:25:21.000000 arelle-release-2.7.1/attic/CntlrGenVersReports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-18 22:25:21.000000 arelle-release-2.7.1/buildVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-18 22:25:21.000000 arelle-release-2.7.1/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 22:25:21.000000 arelle-release-2.7.1/debugCmdLineEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-18 22:25:21.000000 arelle-release-2.7.1/distro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.014026 arelle-release-2.7.1/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-18 22:25:21.000000 arelle-release-2.7.1/docker/ubuntu.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 22:25:21.000000 arelle-release-2.7.1/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-18 22:25:21.000000 arelle-release-2.7.1/encodeUtf8PySource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-04-18 22:25:21.000000 arelle-release-2.7.1/generateMessagesCatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-18 22:25:21.000000 arelle-release-2.7.1/installWin64.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-18 22:25:21.000000 arelle-release-2.7.1/installWin86.nsi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.902024 arelle-release-2.7.1/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.902024 arelle-release-2.7.1/libs/linux/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.014026 arelle-release-2.7.1/libs/linux/Tktable2.11/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/linux/Tktable2.11/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.014026 arelle-release-2.7.1/libs/linux/Tktable2.11/html/
--rw-r--r--   0 runner    (1001) docker     (123)    66891 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/linux/Tktable2.11/html/tkTable.html
--rwxr-xr-x   0 runner    (1001) docker     (123)   161976 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/linux/Tktable2.11/libTktable2.11.so
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/linux/Tktable2.11/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/linux/Tktable2.11/pkgIndex.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/linux/Tktable2.11/tkTable.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/linux/Tktable2.11/tktable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.902024 arelle-release-2.7.1/libs/macos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.014026 arelle-release-2.7.1/libs/macos/Tktable2.11/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/macos/Tktable2.11/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.018026 arelle-release-2.7.1/libs/macos/Tktable2.11/html/
--rw-r--r--   0 runner    (1001) docker     (123)    66891 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/macos/Tktable2.11/html/tkTable.html
--rw-r--r--   0 runner    (1001) docker     (123)   130952 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/macos/Tktable2.11/libTktable2.11.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/macos/Tktable2.11/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/macos/Tktable2.11/pkgIndex.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/macos/Tktable2.11/tkTable.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/macos/Tktable2.11/tktable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.902024 arelle-release-2.7.1/libs/win64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.018026 arelle-release-2.7.1/libs/win64/Tktable2.11/
--rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/win64/Tktable2.11/Tktable.dll
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/win64/Tktable2.11/pkgIndex.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-18 22:25:21.000000 arelle-release-2.7.1/libs/win64/Tktable2.11/tkTable.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-18 22:25:21.000000 arelle-release-2.7.1/messages.pot
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-18 22:25:21.000000 arelle-release-2.7.1/msgfmt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.902024 arelle-release-2.7.1/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.018026 arelle-release-2.7.1/plugins/xbrl-us/
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-18 22:25:21.000000 arelle-release-2.7.1/plugins/xbrl-us/us-gaap-consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-04-18 22:25:21.000000 arelle-release-2.7.1/pygettext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-18 22:25:21.000000 arelle-release-2.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-18 22:25:21.000000 arelle-release-2.7.1/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-18 22:25:21.000000 arelle-release-2.7.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-18 22:25:21.000000 arelle-release-2.7.1/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      276 2023-04-18 22:25:21.000000 arelle-release-2.7.1/runMacGUI.sh
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-18 22:25:21.000000 arelle-release-2.7.1/runtime.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.022026 arelle-release-2.7.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1517 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/buildLinuxDist.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      620 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/buildMacDist.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/buildWinDist.bat
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/charlieTest.bat
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/exportCsvFormulae.bat
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/exportCsvFromXbrlInstance.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/generateTestcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/reportAllTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runAllTests.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)     2138 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runESMAtests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runGUI.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      266 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runGUI.sh
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runGenerateVersioningTestcases.bat
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runGeneratedTestcase.bat
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runLocaleGettext.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runPackageTests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runProfilerXDTTest.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runPyTest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runTR2Tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runTR3Tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runTR4Tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runTR5Tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runTRSECTests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runUS-GFMTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/runVersioningConsumptionTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/startWebServer-27.bat
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 22:25:21.000000 arelle-release-2.7.1/scripts/startWebServer.bat
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-18 22:25:38.030026 arelle-release-2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-18 22:25:21.000000 arelle-release-2.7.1/testParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-18 22:25:21.000000 arelle-release-2.7.1/testParser2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.022026 arelle-release-2.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.902024 arelle-release-2.7.1/tests/integration_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.902024 arelle-release-2.7.1/tests/integration_tests/ui_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.022026 arelle-release-2.7.1/tests/integration_tests/ui_tests/ArelleGUITest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.022026 arelle-release-2.7.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/ArelleGUITest.csproj
--rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Tests.cs
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Usings.cs
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest.sln
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.022026 arelle-release-2.7.1/tests/integration_tests/ui_tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   223544 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/ui_tests/resources/workiva.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.022026 arelle-release-2.7.1/tests/integration_tests/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.026026 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/efm_current.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2021.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2022.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2021.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2022.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_dimensions_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_assertion_severity_2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_function_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_ixbrl_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_link_role_registry_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_oim_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)    29081 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_table_linkbase_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_taxonomy_packages_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_3.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_4.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_malformed_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_registry_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_structure_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/download_conformance_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/run_conformance_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/test_conformance_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/integration_tests/validation/validation_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.902024 arelle-release-2.7.1/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.026026 arelle-release-2.7.1/tests/unit_tests/arelle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.026026 arelle-release-2.7.1/tests/unit_tests/arelle/formula/
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/formula/test_fact_aspects_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.026026 arelle-release-2.7.1/tests/unit_tests/arelle/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/plugin/test_loadfromoim.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/test_cntlr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/test_modelmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/test_packagemanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/test_pluginmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/test_qname.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/test_system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/test_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/test_urlutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tests/unit_tests/arelle/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-18 22:25:21.000000 arelle-release-2.7.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:37.902024 arelle-release-2.7.1/vms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:25:38.026026 arelle-release-2.7.1/vms/mac/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-18 22:25:21.000000 arelle-release-2.7.1/vms/mac/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1478 2023-04-18 22:25:21.000000 arelle-release-2.7.1/vms/mac/create-macos-bootable-for-virtualbox.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.150523 arelle-release-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.054522 arelle-release-2.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.054522 arelle-release-2.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/ISSUE_TEMPLATE/change.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.054522 arelle-release-2.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/workflows/build-and-release-linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/workflows/build-and-release-mac.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/workflows/build-and-release-windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/workflows/build-windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/workflows/conformance-suites.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/workflows/project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/workflows/test-ui.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-25 16:38:01.000000 arelle-release-2.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-25 16:38:01.000000 arelle-release-2.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-25 16:38:01.000000 arelle-release-2.8.0/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-25 16:38:01.000000 arelle-release-2.8.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-25 16:38:01.000000 arelle-release-2.8.0/EFM-only-test.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-25 16:38:01.000000 arelle-release-2.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-25 16:38:16.150523 arelle-release-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-25 16:38:01.000000 arelle-release-2.8.0/QuickBooks.qwc
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-25 16:38:01.000000 arelle-release-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.054522 arelle-release-2.8.0/apidocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-25 16:38:01.000000 arelle-release-2.8.0/apidocs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-25 16:38:01.000000 arelle-release-2.8.0/apidocs/arelle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-25 16:38:01.000000 arelle-release-2.8.0/apidocs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-25 16:38:01.000000 arelle-release-2.8.0/apidocs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-25 16:38:01.000000 arelle-release-2.8.0/apidocs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 16:38:01.000000 arelle-release-2.8.0/apidocs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.070522 arelle-release-2.8.0/arelle/
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/Aspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39944 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/Cntlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76322 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/CntlrCmdLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/CntlrComServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/CntlrProfiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31445 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/CntlrQuickBooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48719 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/CntlrWebMain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88802 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/CntlrWinMain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/CntlrWinTooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogAbout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogArcroleGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19419 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogFind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogFormulaParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogLanguage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogNewFactItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24340 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogOpenArchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogOpenTaxonomyPackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogPackageManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32913 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogPluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogRssWatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogURL.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DialogUserPassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/DisclosureSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43656 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/FileSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/FunctionCustom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36519 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/FunctionFn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80279 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/FunctionIxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/FunctionUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71334 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/FunctionXfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/FunctionXs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/HashUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/HtmlUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/InstanceAspectsEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/LeiUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/LocalViewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28242 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/Locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120056 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelDocument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88883 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelDtsObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122124 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelFormulaObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72084 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelInstanceObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelObjectFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21424 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelRelationshipSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70336 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelRenderingObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelRssItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelRssObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelTestcaseObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38714 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26062 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelVersObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73327 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelVersReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69922 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ModelXbrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31672 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/PackageManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29039 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/PluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/PrototypeDtsObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/PrototypeInstanceObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/PythonUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/RenderingEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43733 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/RenderingResolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/SystemInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29404 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/TableStructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32276 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/TkTableWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39250 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/UITkTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34218 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/UiUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/Updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32121 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/UrlUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49309 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/Validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51377 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ValidateFilingText.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ValidateInfoset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ValidateUtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43196 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ValidateVersReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75131 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ValidateXbrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ValidateXbrlCalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100180 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ValidateXbrlDTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38118 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ValidateXbrlDimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/Version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewFileConcepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewFileDTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewFileFactList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewFileFactTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewFileFormulae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewFileRelationshipSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewFileRenderedGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewFileRoleTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewFileRssFeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewFileTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewUtilFormulae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinConcepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinDTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinDiffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinFactGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinFactList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinFactTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinFormulae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinPane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinRelationshipSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78864 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinRenderedGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinRoleTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinRssFeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinTkTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19434 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinTupleGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinVersReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/ViewWinXml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/WatchRss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36652 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/WebCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62211 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/XbrlConst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/XbrlUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/XhtmlValidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56964 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/XmlUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44568 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/XmlValidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/XmlValidateParticles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/XmlValidateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 16:38:15.000000 arelle-release-2.8.0/arelle/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.074523 arelle-release-2.8.0/arelle/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/arelle_test.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/creationSoftwareNames.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/disclosuresystems.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/disclosuresystems.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/edbody.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/empty-instance.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/erxl.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/mappings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/mappings.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/xbrlschemafiles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/xhtml-lat1.ent
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/xhtml-special.ent
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/xhtml-symbol.ent
+-rw-r--r--   0 runner    (1001) docker     (123)    26880 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/xhtml1-strict-ix.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/config/xhtml1_1-strict-ix.dtd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.074523 arelle-release-2.8.0/arelle/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)   458032 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/doc/messagesCatalog.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/doc/messagesCatalog.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.074523 arelle-release-2.8.0/arelle/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/.pydevproject
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/CustomLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/LoadEFMvalidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/LoadSavePreLbCsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/LoadValidate.cs
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/LoadValidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/LoadValidateCmdLine.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/LoadValidatePostedZip.java
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/LoadValidateWebService.java
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/SaveTableToExelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/TR3toTR4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.078523 arelle-release-2.8.0/arelle/examples/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/bigInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/cmdWebServerExtension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/crashTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/formulaSuiteConverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/functionsCustom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/hello_dolly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/hello_i18n.pot
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/hello_i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/importTestChild1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/importTestChild2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/importTestGrandchild1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/importTestGrandchild2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/importTestImported1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/importTestImported11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/importTestParent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.042522 arelle-release-2.8.0/arelle/examples/plugin/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.042522 arelle-release-2.8.0/arelle/examples/plugin/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.078523 arelle-release-2.8.0/arelle/examples/plugin/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/locale/fr/LC_MESSAGES/hello_i18n.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.078523 arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/importTestChild1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/importTestChild2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/importTestGrandchild1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/importTestGrandchild2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/importTestImported1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/importTestImported11.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.078523 arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/subdir/importTestImported111.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.078523 arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/importTestImported1111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/sakaCalendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/saveInstanceInfoset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/streamingExtensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/testcaseIxExpectedHtmlFixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/updateTableLB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/validateSchemaLxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/plugin/validateTableInfoset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/us-gaap-dei-docType-extraction-frm.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/examples/us-gaap-dei-ratio-cash-frm.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.078523 arelle-release-2.8.0/arelle/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/formula/FactAspectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/formula/FormulaConsisAsser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83178 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/formula/FormulaEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98324 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/formula/ValidateFormula.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/formula/XPathContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49913 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/formula/XPathParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/formula/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.086522 arelle-release-2.8.0/arelle/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/arelle-full-word.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/arelle-mac-icon-4.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/arelle-word-only.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/arelle.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   212911 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/arelle.icns
+-rw-r--r--   0 runner    (1001) docker     (123)   392859 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/arelle.icns.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/arelle.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/arelle.xbm
+-rw-r--r--   0 runner    (1001) docker     (123)   269858 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/arelle128.psd
+-rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/arelle16.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/arelle16x16and32x32.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/arelle32.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/columnSortDown.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/columnSortUp.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/dmg_background.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/octocat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23863 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/python-clear.png
+-rw-r--r--   0 runner    (1001) docker     (123)   696358 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/python-icon-pack-crystalxp.net-842.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarClose.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarCompare.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarDelete.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarFindMenu.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarLogClear - 1-piece-top.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarLogClear-orig.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarLogClear.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarNewFile.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarOpenDatabase.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarOpenFile.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarOpenWeb.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarProperties.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarQuit.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarReopen.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarSaveFile.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/toolbarValidate.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/xbrl.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   201686 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/xbrl.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/xbrl128-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/xbrl128.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/xbrl16.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/images/xbrl32.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.086522 arelle-release-2.8.0/arelle/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.046522 arelle-release-2.8.0/arelle/locale/ar_EG/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.086522 arelle-release-2.8.0/arelle/locale/ar_EG/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   341883 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/locale/ar_EG/LC_MESSAGES/ar_EG.po
+-rw-r--r--   0 runner    (1001) docker     (123)   185904 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/locale/ar_EG/LC_MESSAGES/arelle.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.046522 arelle-release-2.8.0/arelle/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.086522 arelle-release-2.8.0/arelle/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   149331 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/locale/es/LC_MESSAGES/arelle.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.046522 arelle-release-2.8.0/arelle/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.086522 arelle-release-2.8.0/arelle/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   118897 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/locale/fr/LC_MESSAGES/arelle.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   168077 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/locale/fr/LC_MESSAGES/fr.po
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/locale/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   249762 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/locale/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.046522 arelle-release-2.8.0/arelle/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.086522 arelle-release-2.8.0/arelle/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   375378 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/locale/ru/LC_MESSAGES/arelle.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   449579 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/locale/ru/LC_MESSAGES/ru.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.090523 arelle-release-2.8.0/arelle/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/EdgarRendererAllReports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/SECCorrespondenceLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/TDnetLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/UKCompaniesHouseLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101637 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/formulaLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31396 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/formulaSaver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/formulaXPathChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/functionsMath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/functionsXmlCreation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42075 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/inlineXbrlDocumentSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/instanceInfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.046522 arelle-release-2.8.0/arelle/plugin/internet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.094523 arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/HTTPNtlmAuthHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/U32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/des_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/des_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/lgpl-3.0-standalone.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/ntlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124382 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/loadFromExcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76473 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/loadFromOIM-2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)   195836 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/loadFromOIM.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.094523 arelle-release-2.8.0/arelle/plugin/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/logging/dpmSignature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/logging/dqcParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/logging/saveMessages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/objectmaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/profileCmdLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/profileFormula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/saveCHComponentFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/saveDTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/saveHtmlEBAtables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/saveLoadableExcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32261 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/saveLoadableOIM.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/saveSKOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/saveSampleInstance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.094523 arelle-release-2.8.0/arelle/plugin/security/
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/security/cryptAES_CBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/security/cryptAES_EAX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.094523 arelle-release-2.8.0/arelle/plugin/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/sphinx/FormulaGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19516 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/sphinx/SphinxContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35742 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/sphinx/SphinxEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49810 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/sphinx/SphinxMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48614 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/sphinx/SphinxParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/sphinx/SphinxValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/sphinx/US-GAAP Ratios Example.xsr
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47646 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/streamingExtensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.094523 arelle-release-2.8.0/arelle/plugin/transforms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.094523 arelle-release-2.8.0/arelle/plugin/transforms/SEC/
+-rw-r--r--   0 runner    (1001) docker     (123)    41892 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.098523 arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/extractTestcase.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/extractTestcase.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/runIxtSecTests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  4737705 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/saxon9.jar
+-rw-r--r--   0 runner    (1001) docker     (123)   225611 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/testcase.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    59680 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/tests.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/text2num.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.046522 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.102523 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-boolballotbox.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-countrynameen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-datequarterend.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durday.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durhour.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durmonth.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durweek.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durwordsen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-duryear.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-edgarprovcountryen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-entityfilercategoryen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-exchnameen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-numwordsen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-stateprovnameen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-yesnoballotbox.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/transform-registry.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.102523 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    55540 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/schema/inlinexbrl-sec-transformation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/transforms/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/unpackSecEisFile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.102523 arelle-release-2.8.0/arelle/plugin/validate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.102523 arelle-release-2.8.0/arelle/plugin/validate/CIPC/
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/CIPC/Const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/CIPC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/CIPC/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.102523 arelle-release-2.8.0/arelle/plugin/validate/EBA/
+-rw-r--r--   0 runner    (1001) docker     (123)    45950 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EBA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EBA/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.102523 arelle-release-2.8.0/arelle/plugin/validate/EFM/
+-rw-r--r--   0 runner    (1001) docker     (123)    16365 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/Consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40582 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/DTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/Dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/Document.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   253045 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/Filing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/PreCalAlignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37995 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42471 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.114523 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/axiswarnings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/cef-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/country-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/currency-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/dei-deprecated-concepts.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113832 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/dei-validations.json
+-rw-r--r--   0 runner    (1001) docker     (123)    76859 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/dqc-us-rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/ecd-deprecated-concepts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.122523 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/
+-rw-r--r--   0 runner    (1001) docker     (123)    31435 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-16-4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    76545 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-0-4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    76785 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    73012 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    80115 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-3-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   150333 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   138364 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   135467 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   180977 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   125792 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   119973 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   134456 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   109498 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    99358 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    28394 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2012.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    29132 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2013.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    29744 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2014.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2015.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    31676 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2016.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   109944 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    39675 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    35860 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    42433 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    58455 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1-preview.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    62455 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    49163 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    48412 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    57294 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    69072 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    69638 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   368244 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-all-years.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/erxl.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/extendedtaxonomies-all-years.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    93735 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrs-taxonomies.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrstaxonomies-all-years.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/exch-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/ifrs-full-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/invest-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/ixbrl-transform-registries.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/naics-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/other-standard-taxonomies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/rr-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/sic-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/signwarnings.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/srt-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/stpr-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/taxonomy-compatibility.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205448 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/us-gaap-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1583747 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2020.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1624986 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2021.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1593440 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2022.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1613560 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2023.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/vip-deprecated-concepts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.122523 arelle-release-2.8.0/arelle/plugin/validate/EFM/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM/tools/CheckTxmyRefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.106523 arelle-release-2.8.0/arelle/plugin/validate/EFM-htm/
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM-htm/Const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM-htm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM-htm/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.106523 arelle-release-2.8.0/arelle/plugin/validate/EFM-htm/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/EFM-htm/resources/efm-htm.dtd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.122523 arelle-release-2.8.0/arelle/plugin/validate/ESEF/
+-rw-r--r--   0 runner    (1001) docker     (123)    21793 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF/Const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF/DTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF/Dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF/Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76372 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.122523 arelle-release-2.8.0/arelle/plugin/validate/ESEF/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF/resources/authority-validations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.122523 arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/
+-rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/Const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/DTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/Dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85329 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.122523 arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/resources/authority-validations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.122523 arelle-release-2.8.0/arelle/plugin/validate/FERC/
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/FERC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/FERC/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.122523 arelle-release-2.8.0/arelle/plugin/validate/FERC/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/FERC/resources/ferc-utr.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.122523 arelle-release-2.8.0/arelle/plugin/validate/GFM/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/GFM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/GFM/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.122523 arelle-release-2.8.0/arelle/plugin/validate/HMRC/
+-rw-r--r--   0 runner    (1001) docker     (123)    29346 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/HMRC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/HMRC/config.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    25247 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/HMRC/consistencyChecksByName.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/HMRC/hmrc-taxonomies.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.122523 arelle-release-2.8.0/arelle/plugin/validate/ROS/
+-rw-r--r--   0 runner    (1001) docker     (123)    19281 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ROS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/ROS/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.126523 arelle-release-2.8.0/arelle/plugin/validate/SBRnl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/SBRnl/CustomLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/SBRnl/DTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/SBRnl/Dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59358 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/SBRnl/Document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29571 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/SBRnl/Filing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/SBRnl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/SBRnl/config.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/SBRnl/sbr-nl-taxonomies.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/USBestPractices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/USCorpAction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18558 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/USSecTagging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.126523 arelle-release-2.8.0/arelle/plugin/validate/XDC/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/XDC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/XDC/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.126523 arelle-release-2.8.0/arelle/plugin/validate/XFsyntax/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/XFsyntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66728 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/XFsyntax/xf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31565 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validate/calc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/validateSBRnl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.126523 arelle-release-2.8.0/arelle/plugin/xbrlDB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/DialogRssWatchExtender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56450 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/SqlDb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78257 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlDpmSqlDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78348 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlOpenSqlDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36203 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlPublicPostgresDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64539 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlSemanticGraphDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48567 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlSemanticJsonDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55073 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlSemanticRdfDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67782 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlSemanticSqlDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/entityInformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.126523 arelle-release-2.8.0/arelle/plugin/xbrlDB/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/ext/china.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/ext/edgar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/ext/xdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/primaryDocumentFacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.046522 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.126523 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.130523 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open/ext/chinaPostgresDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)   714004 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open/ext/edgarPostgresDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open/ext/xdcPostgresDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open/xbrlOpenPostgresDB.ddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.130523 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open2/
+-rw-r--r--   0 runner    (1001) docker     (123)   728541 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open2/xbrlOpen2PostgresDB.ddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.130523 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/public/
+-rw-r--r--   0 runner    (1001) docker     (123)   963416 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/public/xbrlPublicPostgresDB.ddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.134523 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/secDatabaseModelViews.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    21988 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticColumnComments.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)   728214 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMSSqlDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)   729124 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMySqlDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)  1056221 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticOracleDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)   727913 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticPostgresDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)   726301 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticSQLiteDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xbrlDB/tableFacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/plugin/xuleSaver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.134523 arelle-release-2.8.0/arelle/scripts-macOS/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       91 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/scripts-macOS/startWebServer.command
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.134523 arelle-release-2.8.0/arelle/scripts-unix/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/scripts-unix/startWebServer.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.134523 arelle-release-2.8.0/arelle/scripts-windows/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/scripts-windows/exportCsvFromXbrlInstance.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/scripts-windows/runEFMTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/scripts-windows/runFormulaTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/scripts-windows/runFunctionTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/scripts-windows/runXBRL21Tests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/scripts-windows/runXDTTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/scripts-windows/startWebServer.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/scripts-windows/validateAndRunFormulas.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.138523 arelle-release-2.8.0/arelle/webserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116069 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/webserver/bottle-no2to3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171083 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle/webserver/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle.pyw
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelleCmdLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelleGUI.pyw
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.138523 arelle-release-2.8.0/arelle_release.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-25 16:38:15.000000 arelle-release-2.8.0/arelle_release.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26653 2023-04-25 16:38:16.000000 arelle-release-2.8.0/arelle_release.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:38:15.000000 arelle-release-2.8.0/arelle_release.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-25 16:38:15.000000 arelle-release-2.8.0/arelle_release.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-25 16:38:15.000000 arelle-release-2.8.0/arelle_release.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 16:38:15.000000 arelle-release-2.8.0/arelle_release.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-25 16:38:01.000000 arelle-release-2.8.0/arelle_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.138523 arelle-release-2.8.0/attic/
+-rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-04-25 16:38:01.000000 arelle-release-2.8.0/attic/CntlrGenVersReports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-25 16:38:01.000000 arelle-release-2.8.0/buildVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-25 16:38:01.000000 arelle-release-2.8.0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 16:38:01.000000 arelle-release-2.8.0/debugCmdLineEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-25 16:38:01.000000 arelle-release-2.8.0/distro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.138523 arelle-release-2.8.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-25 16:38:01.000000 arelle-release-2.8.0/docker/ubuntu.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-25 16:38:01.000000 arelle-release-2.8.0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-25 16:38:01.000000 arelle-release-2.8.0/encodeUtf8PySource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-04-25 16:38:01.000000 arelle-release-2.8.0/generateMessagesCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-25 16:38:01.000000 arelle-release-2.8.0/installWin64.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-25 16:38:01.000000 arelle-release-2.8.0/installWin86.nsi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.046522 arelle-release-2.8.0/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.046522 arelle-release-2.8.0/libs/linux/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.138523 arelle-release-2.8.0/libs/linux/Tktable2.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/linux/Tktable2.11/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.138523 arelle-release-2.8.0/libs/linux/Tktable2.11/html/
+-rw-r--r--   0 runner    (1001) docker     (123)    66891 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/linux/Tktable2.11/html/tkTable.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)   161976 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/linux/Tktable2.11/libTktable2.11.so
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/linux/Tktable2.11/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/linux/Tktable2.11/pkgIndex.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/linux/Tktable2.11/tkTable.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/linux/Tktable2.11/tktable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.046522 arelle-release-2.8.0/libs/macos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.138523 arelle-release-2.8.0/libs/macos/Tktable2.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/macos/Tktable2.11/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.138523 arelle-release-2.8.0/libs/macos/Tktable2.11/html/
+-rw-r--r--   0 runner    (1001) docker     (123)    66891 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/macos/Tktable2.11/html/tkTable.html
+-rw-r--r--   0 runner    (1001) docker     (123)   130952 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/macos/Tktable2.11/libTktable2.11.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/macos/Tktable2.11/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/macos/Tktable2.11/pkgIndex.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/macos/Tktable2.11/tkTable.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/macos/Tktable2.11/tktable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.046522 arelle-release-2.8.0/libs/win64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.138523 arelle-release-2.8.0/libs/win64/Tktable2.11/
+-rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/win64/Tktable2.11/Tktable.dll
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/win64/Tktable2.11/pkgIndex.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-25 16:38:01.000000 arelle-release-2.8.0/libs/win64/Tktable2.11/tkTable.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-25 16:38:01.000000 arelle-release-2.8.0/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-25 16:38:01.000000 arelle-release-2.8.0/msgfmt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.050522 arelle-release-2.8.0/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.138523 arelle-release-2.8.0/plugins/xbrl-us/
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-25 16:38:01.000000 arelle-release-2.8.0/plugins/xbrl-us/us-gaap-consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-04-25 16:38:01.000000 arelle-release-2.8.0/pygettext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-25 16:38:01.000000 arelle-release-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-25 16:38:01.000000 arelle-release-2.8.0/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-25 16:38:01.000000 arelle-release-2.8.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-25 16:38:01.000000 arelle-release-2.8.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      276 2023-04-25 16:38:01.000000 arelle-release-2.8.0/runMacGUI.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 16:38:01.000000 arelle-release-2.8.0/runtime.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.142523 arelle-release-2.8.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1517 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/buildLinuxDist.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      620 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/buildMacDist.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/buildWinDist.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/charlieTest.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/exportCsvFormulae.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/exportCsvFromXbrlInstance.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/generateTestcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/reportAllTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runAllTests.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2138 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runESMAtests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runGUI.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      266 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runGUI.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runGenerateVersioningTestcases.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runGeneratedTestcase.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runLocaleGettext.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runPackageTests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runProfilerXDTTest.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runPyTest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runTR2Tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runTR3Tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runTR4Tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runTR5Tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runTRSECTests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runUS-GFMTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/runVersioningConsumptionTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/startWebServer-27.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-25 16:38:01.000000 arelle-release-2.8.0/scripts/startWebServer.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-25 16:38:16.150523 arelle-release-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-25 16:38:01.000000 arelle-release-2.8.0/testParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-25 16:38:01.000000 arelle-release-2.8.0/testParser2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.142523 arelle-release-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.050522 arelle-release-2.8.0/tests/integration_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.050522 arelle-release-2.8.0/tests/integration_tests/ui_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.142523 arelle-release-2.8.0/tests/integration_tests/ui_tests/ArelleGUITest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.142523 arelle-release-2.8.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/ArelleGUITest.csproj
+-rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Tests.cs
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Usings.cs
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest.sln
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.142523 arelle-release-2.8.0/tests/integration_tests/ui_tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   223544 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/ui_tests/resources/workiva.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.146523 arelle-release-2.8.0/tests/integration_tests/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.146523 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/efm_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2021.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2021.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_dimensions_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_assertion_severity_2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_function_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_ixbrl_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_link_role_registry_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_oim_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29081 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_table_linkbase_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_taxonomy_packages_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_malformed_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_registry_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_structure_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/download_conformance_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/run_conformance_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/test_conformance_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/integration_tests/validation/validation_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.050522 arelle-release-2.8.0/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.146523 arelle-release-2.8.0/tests/unit_tests/arelle/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.150523 arelle-release-2.8.0/tests/unit_tests/arelle/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/formula/test_fact_aspects_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.150523 arelle-release-2.8.0/tests/unit_tests/arelle/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/plugin/test_loadfromoim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/test_cntlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/test_modelmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/test_packagemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/test_pluginmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/test_qname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/test_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/test_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/test_urlutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tests/unit_tests/arelle/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-25 16:38:01.000000 arelle-release-2.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.050522 arelle-release-2.8.0/vms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:38:16.150523 arelle-release-2.8.0/vms/mac/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-25 16:38:01.000000 arelle-release-2.8.0/vms/mac/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1478 2023-04-25 16:38:01.000000 arelle-release-2.8.0/vms/mac/create-macos-bootable-for-virtualbox.sh
```

### Comparing `arelle-release-2.7.1/.github/ISSUE_TEMPLATE/bug.yml` & `arelle-release-2.8.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/.github/workflows/build-and-release-linux.yml` & `arelle-release-2.8.0/.github/workflows/build-and-release-linux.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/.github/workflows/build-and-release-mac.yml` & `arelle-release-2.8.0/.github/workflows/build-and-release-mac.yml`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     steps:
       - name: Checkout arelle
         uses: actions/checkout@v3.5.2
         with:
           fetch-depth: 0
       - name: Install Python
-        uses: actions/setup-python@v4.5.0
+        uses: actions/setup-python@v4.6.0
         with:
           cache: 'pip'
           check-latest: true
           python-version: ${{ inputs.python_version }}
       - run: |
           python -m pip install --upgrade pip setuptools wheel
           pip install -r requirements-build.txt
```

### Comparing `arelle-release-2.7.1/.github/workflows/build-and-release-windows.yml` & `arelle-release-2.8.0/.github/workflows/build-and-release-windows.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/.github/workflows/build-windows.yml` & `arelle-release-2.8.0/.github/workflows/build-windows.yml`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
       working-directory: ixbrl-viewer
       run: |
         npm install
         npm run prod
     - shell: cmd
       run: move ixbrl-viewer\iXBRLViewerPlugin arelle\plugin\iXBRLViewerPlugin && rmdir /s /q ixbrl-viewer
     - name: Set up Python ${{ inputs.python_version }}
-      uses: actions/setup-python@v4.5.0
+      uses: actions/setup-python@v4.6.0
       with:
         cache: 'pip'
         check-latest: true
         python-version: ${{ inputs.python_version }}
     - name: Install NSIS
       run: choco install nsis
     - name: Install requirements
```

### Comparing `arelle-release-2.7.1/.github/workflows/conformance-suites.yml` & `arelle-release-2.8.0/.github/workflows/conformance-suites.yml`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
       - name: Checkout EdgarRenderer
         if: ${{ matrix.test == 'efm_current' }}
         uses: actions/checkout@v3.5.2
         with:
           repository: Arelle/EdgarRenderer
           path: arelle/plugin/EdgarRenderer
       - name: Install Python 3
-        uses: actions/setup-python@v4.5.0
+        uses: actions/setup-python@v4.6.0
         with:
           cache: 'pip'
           check-latest: true
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip setuptools wheel
```

### Comparing `arelle-release-2.7.1/.github/workflows/python-package.yml` & `arelle-release-2.8.0/.github/workflows/python-package.yml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     runs-on: ubuntu-22.04
     steps:
       - name: Checkout arelle
         uses: actions/checkout@v3.5.2
         with:
           fetch-depth: 0
       - name: Install Python
-        uses: actions/setup-python@v4.5.0
+        uses: actions/setup-python@v4.6.0
         with:
           cache: 'pip'
           check-latest: true
           python-version: ${{ inputs.python_version }}
       - name: Build python package
         run: |
           python -m pip install --upgrade pip setuptools wheel
```

### Comparing `arelle-release-2.7.1/.github/workflows/release.yml` & `arelle-release-2.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/.github/workflows/test-ui.yml` & `arelle-release-2.8.0/.github/workflows/test-ui.yml`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
       - name: Extract artifact
         if: matrix.build-type == 'zip'
         run: expand-archive ${{ env.zip_artifact_versioned_name }} build
 
       - name: Install Python
         if: matrix.build-type == 'source'
-        uses: actions/setup-python@v4.5.0
+        uses: actions/setup-python@v4.6.0
         with:
           cache: 'pip'
           check-latest: true
           python-version: ${{ github.event_name == 'workflow_dispatch' && inputs.python_version || '3.11' }}
       - name: Install Python dependencies
         if: matrix.build-type == 'source'
         run: |
```

### Comparing `arelle-release-2.7.1/.github/workflows/tests.yml` & `arelle-release-2.8.0/.github/workflows/tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
           - '3.9'
           - '3.10'
           - '3.11'
     runs-on: ${{ matrix.os }}
     steps:
       - uses: actions/checkout@v3.5.2
       - name: Install Python 3
-        uses: actions/setup-python@v4.5.0
+        uses: actions/setup-python@v4.6.0
         with:
           cache: 'pip'
           check-latest: true
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip setuptools wheel
```

### Comparing `arelle-release-2.7.1/.gitignore` & `arelle-release-2.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/CONTRIBUTING.md` & `arelle-release-2.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/EFM-only-test.ini` & `arelle-release-2.8.0/EFM-only-test.ini`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/LICENSE.md` & `arelle-release-2.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/PKG-INFO` & `arelle-release-2.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arelle-release
-Version: 2.7.1
+Version: 2.8.0
 Summary: An open source XBRL platform.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
@@ -27,14 +27,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: Crypto
 Provides-Extra: DB
 Provides-Extra: EFM
+Provides-Extra: ESEF
 Provides-Extra: ObjectMaker
 Provides-Extra: WebServer
 License-File: LICENSE.md
 
 # Arelle
 
 [![pypi-version](https://img.shields.io/pypi/v/arelle-release.svg)](https://pypi.org/project/arelle-release/)
```

### Comparing `arelle-release-2.7.1/QuickBooks.qwc` & `arelle-release-2.8.0/QuickBooks.qwc`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/README.md` & `arelle-release-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/apidocs/Makefile` & `arelle-release-2.8.0/apidocs/Makefile`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/apidocs/arelle.rst` & `arelle-release-2.8.0/apidocs/arelle.rst`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/apidocs/conf.py` & `arelle-release-2.8.0/apidocs/conf.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/apidocs/make.bat` & `arelle-release-2.8.0/apidocs/make.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/Aspect.py` & `arelle-release-2.8.0/arelle/Aspect.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/Cntlr.py` & `arelle-release-2.8.0/arelle/Cntlr.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,15 +464,15 @@
                 pass
 
     def saveConfig(self) -> None:
         """Save user preferences configuration (in json configuration file)."""
         if self.hasFileSystem and not self.disablePersistentConfig:
             with io.open(self.configJsonFile, 'wt', encoding='utf-8') as f:
                 # might not be unicode in 2.7
-                jsonStr = str(json.dumps(self.config, ensure_ascii=False, indent=2))
+                jsonStr = str(json.dumps(self.config, ensure_ascii=False, indent=2, sort_keys=True))
                 f.write(jsonStr)  # 2.7 getss unicode this way
 
     # default non-threaded viewModelObject
     def viewModelObject(self, modelXbrl: ModelXbrl, objectId: str) -> None:
         """Notify any watching views to show and highlight selected object.  Generally used
         to scroll list control to object and highlight it, or if tree control, to find the object
         and open tree branches as needed for visibility, scroll to and highlight the object.
```

### Comparing `arelle-release-2.7.1/arelle/CntlrCmdLine.py` & `arelle-release-2.8.0/arelle/CntlrCmdLine.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/CntlrComServer.py` & `arelle-release-2.8.0/arelle/CntlrComServer.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/CntlrProfiler.py` & `arelle-release-2.8.0/arelle/CntlrProfiler.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/CntlrQuickBooks.py` & `arelle-release-2.8.0/arelle/CntlrQuickBooks.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/CntlrWebMain.py` & `arelle-release-2.8.0/arelle/CntlrWebMain.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/CntlrWinMain.py` & `arelle-release-2.8.0/arelle/CntlrWinMain.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,18 +219,20 @@
         for (_opt_label, _opt_val) in _internetRecheckEntries:
             internetCacheRecheckMenu.add_checkbutton(
                     label=_opt_label,
                     variable=self.internetRecheckVar,
                     underline=0,
                     onvalue=_opt_val
              )
+        self.webCache.timeout = self.config.setdefault("internetConnectionTimeout", None)
 
         cacheMenu.add_command(label=_("Clear cache"), underline=0, command=self.confirmClearWebCache)
         cacheMenu.add_command(label=_("Manage cache"), underline=0, command=self.manageWebCache)
         cacheMenu.add_cascade(label=self._internetRecheckLabel, menu=internetCacheRecheckMenu, underline=0, state=_recheck_initial)
+        cacheMenu.add_command(label=_("Internet connection timeout"), underline=0, command=self.internetConnectionTimeout)
         cacheMenu.add_command(label=_("Proxy Server"), underline=0, command=self.setupProxy)
         cacheMenu.add_command(label=_("HTTP User Agent"), underline=0, command=self.setupUserAgent)
         self.webCache.httpUserAgent = self.config.get("httpUserAgent")
         self._cacheMenu = cacheMenu
 
         logmsgMenu = Menu(self.menubar, tearoff=0)
         toolsMenu.add_cascade(label=_("Messages log"), menu=logmsgMenu, underline=0)
@@ -1127,14 +1129,24 @@
         self.saveConfig()
 
     def setNoCertificateCheck(self, *args):
         self.webCache.noCertificateCheck = self.noCertificateCheck.get() # resets proxy handlers
         self.config["noCertificateCheck"] = self.webCache.noCertificateCheck
         self.saveConfig()
 
+    def internetConnectionTimeout(self):
+        response = tkinter.simpledialog.askinteger(
+                    _("arelle - Internet Connection Timeout"),
+                    _("Enter timeout in seconds or 0 for no timeout"),
+                    initialvalue=str(self.webCache.timeout or 0),
+                    parent=self.parent)
+        if response is not None and response >= 0:
+            self.webCache.timeout = response or None # set to None if zero - no timenout
+            self.config["internetConnectionTimeout"] = self.webCache.timeout
+
     def confirmClearWebCache(self):
         if tkinter.messagebox.askyesno(
                     _("arelle - Clear Internet Cache"),
                     _("Are you sure you want to clear the internet cache?"),
                     parent=self.parent):
             def backgroundClearCache():
                 self.showStatus(_("Clearing internet cache"))
```

### Comparing `arelle-release-2.7.1/arelle/CntlrWinTooltip.py` & `arelle-release-2.8.0/arelle/CntlrWinTooltip.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DialogAbout.py` & `arelle-release-2.8.0/arelle/DialogAbout.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DialogArcroleGroup.py` & `arelle-release-2.8.0/arelle/DialogArcroleGroup.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DialogFind.py` & `arelle-release-2.8.0/arelle/DialogFind.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DialogFormulaParameters.py` & `arelle-release-2.8.0/arelle/DialogFormulaParameters.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DialogLanguage.py` & `arelle-release-2.8.0/arelle/DialogLanguage.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DialogNewFactItem.py` & `arelle-release-2.8.0/arelle/DialogNewFactItem.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DialogOpenArchive.py` & `arelle-release-2.8.0/arelle/DialogOpenArchive.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DialogPackageManager.py` & `arelle-release-2.8.0/arelle/DialogPackageManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DialogPluginManager.py` & `arelle-release-2.8.0/arelle/DialogPluginManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DialogRssWatch.py` & `arelle-release-2.8.0/arelle/DialogRssWatch.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DialogURL.py` & `arelle-release-2.8.0/arelle/DialogURL.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DialogUserPassword.py` & `arelle-release-2.8.0/arelle/DialogUserPassword.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/DisclosureSystem.py` & `arelle-release-2.8.0/arelle/DisclosureSystem.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/FileSource.py` & `arelle-release-2.8.0/arelle/FileSource.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         filesource = FileSource(POST_UPLOADED_ZIP, cntlr)
         filesource.openZipStream(sourceZipStream)
         if filename:
             filesource.select(filename)
         return filesource
     else:
         if cntlr and base:
-            filename = cntlr.webCache.normalizeUrl(filename, base=base) # type: ignore[no-untyped-call]
+            filename = cntlr.webCache.normalizeUrl(filename, base=base)
 
         assert filename is not None
         archivepathSelection = archiveFilenameParts(filename, checkIfXmlIsEis)
         if archivepathSelection is not None:
             archivepath = archivepathSelection[0]
             selection: str | None = archivepathSelection[1]
```

### Comparing `arelle-release-2.7.1/arelle/FunctionCustom.py` & `arelle-release-2.8.0/arelle/FunctionCustom.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/FunctionFn.py` & `arelle-release-2.8.0/arelle/FunctionFn.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/FunctionIxt.py` & `arelle-release-2.8.0/arelle/FunctionIxt.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/FunctionUtil.py` & `arelle-release-2.8.0/arelle/FunctionUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/FunctionXfi.py` & `arelle-release-2.8.0/arelle/FunctionXfi.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/FunctionXs.py` & `arelle-release-2.8.0/arelle/FunctionXs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/HashUtil.py` & `arelle-release-2.8.0/arelle/HashUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/HtmlUtil.py` & `arelle-release-2.8.0/arelle/HtmlUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/InstanceAspectsEvaluator.py` & `arelle-release-2.8.0/arelle/InstanceAspectsEvaluator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/LeiUtil.py` & `arelle-release-2.8.0/arelle/LeiUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/LocalViewer.py` & `arelle-release-2.8.0/arelle/LocalViewer.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/Locale.py` & `arelle-release-2.8.0/arelle/Locale.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelDocument.py` & `arelle-release-2.8.0/arelle/ModelDocument.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     elif not normalizedUri:
         modelXbrl.error("FileNotLoadable",
                 _("File name absent, document can not be loaded."),
                 modelObject=referringElement, fileName=normalizedUri)
         return None
 
     if isEntry:
-        modelXbrl.entryLoadingUrl = normalizedUri   # for error loggiong during loading
+        modelXbrl.entryLoadingUrl = normalizedUri   # for error logging during loading
         modelXbrl.uri = normalizedUri
         modelXbrl.uriDir = os.path.dirname(normalizedUri)
         for i in range(modelXbrl.modelManager.disclosureSystem.maxSubmissionSubdirectoryEntryNesting):
             modelXbrl.uriDir = os.path.dirname(modelXbrl.uriDir)
     if modelXbrl.modelManager.validateDisclosureSystem and \
        not normalizedUri.startswith(modelXbrl.uriDir) and \
        not modelXbrl.modelManager.disclosureSystem.hrefValid(normalizedUri):
@@ -1317,24 +1317,28 @@
             self.modelXbrl.error("ix:multipleIxNamespaces",
                     _("Multiple ix namespaces were found"),
                     modelObject=conflictingNSelts)
         self.ixNS = ixNS
         self.ixNStag = ixNStag = "{" + ixNS + "}" if ixNS else ""
         self.htmlBase = htmlBase
         ixdsTarget = getattr(self.modelXbrl, "ixdsTarget", None)
-        # load referenced schemas and linkbases (before validating inline HTML
-        for inlineElement in htmlElement.iterdescendants(tag=ixNStag + "references"):
-            if inlineElement.get("target") == ixdsTarget:
-                self.schemaLinkbaseRefsDiscover(inlineElement)
+        if all(pluginMethod(self.modelXbrl)
+               for pluginMethod in pluginClassMethods("ModelDocument.DiscoverIxdsDts")):
+            # load referenced schemas and linkbases (before validating inline HTML
+            for inlineElement in htmlElement.iterdescendants(tag=ixNStag + "references"):
+                if inlineElement.get("target") == ixdsTarget:
+                    self.schemaLinkbaseRefsDiscover(inlineElement)
+                    xmlValidate(self.modelXbrl, inlineElement) # validate instance elements
+        # validate resources only if no possibility of multi-document ixds for which ix:references not encountered yet
+        if len(list(pluginClassMethods("ModelDocument.SelectIxdsTarget"))) == 0:
+            for inlineElement in htmlElement.iterdescendants(tag=ixNStag + "resources"):
                 xmlValidate(self.modelXbrl, inlineElement) # validate instance elements
         # with DTS loaded, now validate inline HTML (so schema definition of facts is available)
         if htmlElement.namespaceURI == XbrlConst.xhtml:  # must validate xhtml
             XhtmlValidate.xhtmlValidate(self.modelXbrl, htmlElement)  # fails on prefixed content
-        for inlineElement in htmlElement.iterdescendants(tag=ixNStag + "resources"):
-            xmlValidate(self.modelXbrl, inlineElement) # validate instance elements
 
         # subsequent inline elements have to be processed after all of the document set is loaded
         if not hasattr(self.modelXbrl, "ixdsHtmlElements"):
             self.modelXbrl.ixdsHtmlElements = []
         self.modelXbrl.ixdsHtmlElements.append(htmlElement)
 
 
@@ -1432,14 +1436,16 @@
                 if r.referringModelObject is None and referringModelObject is not None:
                     r.referringModelObject = referringModelObject
 
 
 # inline document set level compilation
 # modelIxdsDocument is an inlineDocumentSet or entry inline document (if not a document set)
 def inlineIxdsDiscover(modelXbrl, modelIxdsDocument):
+    for pluginMethod in pluginClassMethods("ModelDocument.SelectIxdsTarget"):
+        pluginMethod(modelXbrl)
     # extract for a single target document
     ixdsTarget = getattr(modelXbrl, "ixdsTarget", None)
     # compile inline result set
     ixdsEltById = defaultdict(list)
     for htmlElement in modelXbrl.ixdsHtmlElements:
         for elt in htmlElement.iterfind(".//*[@id]"):
             if isinstance(elt,ModelObject) and elt.id:
```

### Comparing `arelle-release-2.7.1/arelle/ModelDtsObject.py` & `arelle-release-2.8.0/arelle/ModelDtsObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelFormulaObject.py` & `arelle-release-2.8.0/arelle/ModelFormulaObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelInstanceObject.py` & `arelle-release-2.8.0/arelle/ModelInstanceObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelManager.py` & `arelle-release-2.8.0/arelle/ModelManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelObject.py` & `arelle-release-2.8.0/arelle/ModelObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 See COPYRIGHT.md for copyright information.
 '''
 from __future__ import annotations
-from typing import TYPE_CHECKING, Any, Generator, cast
+from typing import TYPE_CHECKING, Any, Generator, cast, Union
 from lxml import etree
 from arelle import Locale
 from arelle.ModelValue import qname, qnameEltPfxName, QName
 
 if TYPE_CHECKING:
     from arelle.ModelDocument import ModelDocument
     from arelle.ModelXbrl import ModelXbrl
@@ -136,15 +136,15 @@
 
     def objectId(self, refId: str = "") -> str:
         """Returns a string surrogate representing the object index of the model document,
         prepended by the refId string.
         :param refId: A string to prefix the refId for uniqueless (such as to use in tags for tkinter)
         :type refId: str
         """
-        return "_{0}_{1}".format(refId, self.objectIndex)
+        return f"_{refId}_{getattr(self, 'objectIndex', 'None')}"
 
     @property
     def modelXbrl(self) -> ModelXbrl | None:
         modelDocument = getattr(self, "modelDocument", None)
         return modelDocument.modelXbrl if modelDocument is not None else None
 
     def attr(self, attrname: str) -> str | None:
```

### Comparing `arelle-release-2.7.1/arelle/ModelObjectFactory.py` & `arelle-release-2.8.0/arelle/ModelObjectFactory.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,19 @@
 ModelDocument: Any = None
 ModelFact: Any = None
 
 
 def parser(
         modelXbrl: ModelXbrl,
         baseUrl: str | None,
-        target: None = None,
+        target: None = None
 ) -> tuple[etree.XMLParser, KnownNamespacesModelObjectClassLookup, DiscoveringClassLookup]:
     moduleObject_init()  # init ModelObject globals
-    _parser = etree.XMLParser(recover=True, huge_tree=True, target=target, resolve_entities=False)
+    _parser = etree.XMLParser(recover=True, huge_tree=True, target=target,
+                              resolve_entities=False)
     return setParserElementClassLookup(_parser, modelXbrl, baseUrl)
 
 
 def setParserElementClassLookup(
         _parser: etree.XMLParser,
         modelXbrl: ModelXbrl,
         baseUrl: str | None = None,
```

### Comparing `arelle-release-2.7.1/arelle/ModelRelationshipSet.py` & `arelle-release-2.8.0/arelle/ModelRelationshipSet.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelRenderingObject.py` & `arelle-release-2.8.0/arelle/ModelRenderingObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelRssItem.py` & `arelle-release-2.8.0/arelle/ModelRssItem.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelRssObject.py` & `arelle-release-2.8.0/arelle/ModelRssObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelTestcaseObject.py` & `arelle-release-2.8.0/arelle/ModelTestcaseObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelValue.py` & `arelle-release-2.8.0/arelle/ModelValue.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelVersObject.py` & `arelle-release-2.8.0/arelle/ModelVersObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelVersReport.py` & `arelle-release-2.8.0/arelle/ModelVersReport.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ModelXbrl.py` & `arelle-release-2.8.0/arelle/ModelXbrl.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/PackageManager.py` & `arelle-release-2.8.0/arelle/PackageManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/PluginManager.py` & `arelle-release-2.8.0/arelle/PluginManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                                                                    'copyright': '11',
                                                                    'classMethods': '12'}.get(k[0],k[0]))))
                                 for moduleName, moduleInfo in sorted(pluginConfig['modules'].items()))),
          ('classes',OrderedDict(sorted(pluginConfig['classes'].items())))))
 
 def save(cntlr: Cntlr) -> None:
     global pluginConfigChanged
-    if pluginConfigChanged and cntlr.hasFileSystem:
+    if pluginConfigChanged and cntlr.hasFileSystem and not cntlr.disablePersistentConfig:
         pluginJsonFile = cntlr.userAppDir + os.sep + "plugins.json"
         with io.open(pluginJsonFile, 'wt', encoding='utf-8') as f:
             jsonStr = str(json.dumps(orderedPluginConfig(), ensure_ascii=False, indent=2)) # might not be unicode in 2.7
             f.write(jsonStr)
         pluginConfigChanged = False
 
 def close():  # close all loaded methods
```

### Comparing `arelle-release-2.7.1/arelle/PrototypeDtsObject.py` & `arelle-release-2.8.0/arelle/PrototypeDtsObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/PrototypeInstanceObject.py` & `arelle-release-2.8.0/arelle/PrototypeInstanceObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/PythonUtil.py` & `arelle-release-2.8.0/arelle/PythonUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/RenderingEvaluator.py` & `arelle-release-2.8.0/arelle/RenderingEvaluator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/RenderingResolver.py` & `arelle-release-2.8.0/arelle/RenderingResolver.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/SystemInfo.py` & `arelle-release-2.8.0/arelle/SystemInfo.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/TableStructure.py` & `arelle-release-2.8.0/arelle/TableStructure.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/TkTableWrapper.py` & `arelle-release-2.8.0/arelle/TkTableWrapper.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/UITkTable.py` & `arelle-release-2.8.0/arelle/UITkTable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/UiUtil.py` & `arelle-release-2.8.0/arelle/UiUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/Updater.py` & `arelle-release-2.8.0/arelle/Updater.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/UrlUtil.py` & `arelle-release-2.8.0/arelle/UrlUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/Validate.py` & `arelle-release-2.8.0/arelle/Validate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ValidateFilingText.py` & `arelle-release-2.8.0/arelle/ValidateFilingText.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ValidateInfoset.py` & `arelle-release-2.8.0/arelle/ValidateInfoset.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ValidateUtr.py` & `arelle-release-2.8.0/arelle/ValidateUtr.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ValidateVersReport.py` & `arelle-release-2.8.0/arelle/ValidateVersReport.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ValidateXbrl.py` & `arelle-release-2.8.0/arelle/ValidateXbrl.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ValidateXbrlCalcs.py` & `arelle-release-2.8.0/arelle/ValidateXbrlCalcs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ValidateXbrlDTS.py` & `arelle-release-2.8.0/arelle/ValidateXbrlDTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ValidateXbrlDimensions.py` & `arelle-release-2.8.0/arelle/ValidateXbrlDimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/Version.py` & `arelle-release-2.8.0/arelle/Version.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewFile.py` & `arelle-release-2.8.0/arelle/ViewFile.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewFileConcepts.py` & `arelle-release-2.8.0/arelle/ViewFileConcepts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewFileDTS.py` & `arelle-release-2.8.0/arelle/ViewFileDTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewFileFactList.py` & `arelle-release-2.8.0/arelle/ViewFileFactList.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewFileFactTable.py` & `arelle-release-2.8.0/arelle/ViewFileFactTable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewFileFormulae.py` & `arelle-release-2.8.0/arelle/ViewFileFormulae.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewFileRelationshipSet.py` & `arelle-release-2.8.0/arelle/ViewFileRelationshipSet.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewFileRenderedGrid.py` & `arelle-release-2.8.0/arelle/ViewFileRenderedGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewFileRoleTypes.py` & `arelle-release-2.8.0/arelle/ViewFileRoleTypes.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewFileRssFeed.py` & `arelle-release-2.8.0/arelle/ViewFileRssFeed.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewFileTests.py` & `arelle-release-2.8.0/arelle/ViewFileTests.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewUtil.py` & `arelle-release-2.8.0/arelle/ViewUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewUtilFormulae.py` & `arelle-release-2.8.0/arelle/ViewUtilFormulae.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinConcepts.py` & `arelle-release-2.8.0/arelle/ViewWinConcepts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinDTS.py` & `arelle-release-2.8.0/arelle/ViewWinDTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinDiffs.py` & `arelle-release-2.8.0/arelle/ViewWinDiffs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinFactGrid.py` & `arelle-release-2.8.0/arelle/ViewWinFactGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinFactList.py` & `arelle-release-2.8.0/arelle/ViewWinFactList.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinFactTable.py` & `arelle-release-2.8.0/arelle/ViewWinFactTable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinFormulae.py` & `arelle-release-2.8.0/arelle/ViewWinFormulae.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinGrid.py` & `arelle-release-2.8.0/arelle/ViewWinGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinList.py` & `arelle-release-2.8.0/arelle/ViewWinList.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinPane.py` & `arelle-release-2.8.0/arelle/ViewWinPane.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinProperties.py` & `arelle-release-2.8.0/arelle/ViewWinProperties.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinRelationshipSet.py` & `arelle-release-2.8.0/arelle/ViewWinRelationshipSet.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinRenderedGrid.py` & `arelle-release-2.8.0/arelle/ViewWinRenderedGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinRoleTypes.py` & `arelle-release-2.8.0/arelle/ViewWinRoleTypes.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinRssFeed.py` & `arelle-release-2.8.0/arelle/ViewWinRssFeed.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinTests.py` & `arelle-release-2.8.0/arelle/ViewWinTests.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinTkTable.py` & `arelle-release-2.8.0/arelle/ViewWinTkTable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinTree.py` & `arelle-release-2.8.0/arelle/ViewWinTree.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinTupleGrid.py` & `arelle-release-2.8.0/arelle/ViewWinTupleGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinVersReport.py` & `arelle-release-2.8.0/arelle/ViewWinVersReport.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/ViewWinXml.py` & `arelle-release-2.8.0/arelle/ViewWinXml.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/WatchRss.py` & `arelle-release-2.8.0/arelle/WatchRss.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/WebCache.py` & `arelle-release-2.8.0/arelle/WebCache.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 See COPYRIGHT.md for copyright information.
 
 For SEC EDGAR data access see: https://www.sec.gov/os/accessing-edgar-data
 e.g., User-Agent: Sample Company Name AdminContact@<sample company domain>.com
 
 '''
 from __future__ import annotations
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Optional
 import os, posixpath, sys, time, calendar, io, json, logging, shutil, zlib
 import regex as re
 from urllib.parse import quote, unquote
 from urllib.error import URLError, HTTPError, ContentTooShortError
 from http.client import IncompleteRead
 from urllib import request as proxyhandlers
 
@@ -165,18 +165,18 @@
         return self._logDownloads
 
     @logDownloads.setter
     def logDownloads(self, _logDownloads):
         self._logDownloads = _logDownloads
 
     def saveUrlCheckTimes(self) -> None:
-        if self.cachedUrlCheckTimesModified:
+        if self.cachedUrlCheckTimesModified and not self.cntlr.disablePersistentConfig:
             with io.open(self.urlCheckJsonFile, 'wt', encoding='utf-8') as f:
                 f.write(json.dumps(self.cachedUrlCheckTimes, ensure_ascii=False, indent=0))
-        self.cachedUrlCheckTimesModified = False
+            self.cachedUrlCheckTimesModified = False
 
     @property
     def noCertificateCheck(self):
         return self._noCertificateCheck
 
     @noCertificateCheck.setter
     def noCertificateCheck(self, check):
@@ -257,16 +257,15 @@
             ('User-Agent', self.httpUserAgent),
             ('Accept-Encoding', 'gzip, deflate')
             ]
 
         #self.opener.close()
         #self.opener = WebCacheUrlOpener(self.cntlr, proxyDirFmt(httpProxyTuple))
 
-
-    def normalizeUrl(self, url, base=None):
+    def normalizeUrl(self, url:Optional[Any], base: Optional[Any] = None) -> Any:
         if url:
             if url.startswith("file://"): url = url[7:]
             elif url.startswith("file:\\"): url = url[6:]
         if url and not (isHttpUrl(url) or os.path.isabs(url)):
             if base is not None and not isHttpUrl(base) and '%' in url:
                 url = unquote(url)
             if base:
```

### Comparing `arelle-release-2.7.1/arelle/XbrlConst.py` & `arelle-release-2.8.0/arelle/XbrlConst.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/XbrlUtil.py` & `arelle-release-2.8.0/arelle/XbrlUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/XhtmlValidate.py` & `arelle-release-2.8.0/arelle/XhtmlValidate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/XmlUtil.py` & `arelle-release-2.8.0/arelle/XmlUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/XmlValidate.py` & `arelle-release-2.8.0/arelle/XmlValidate.py`

 * *Files 0% similar despite different names*

```diff
@@ -662,15 +662,15 @@
                 if xml:
                     return self.resolve_string(xml, context, base_url=_url)
             else: # probably no active modelXbrl yet, such as when loading packages, use url
                 return self.resolve_filename(url, context)  # type: ignore[attr-defined]
         return self.resolve_empty(context)  # type: ignore[attr-defined]
 
 def lxmlResolvingParser(cntlr: Cntlr, modelXbrl: ModelXbrl | None = None) -> etree.XMLParser:
-    parser = etree.XMLParser()
+    parser = etree.XMLParser(resolve_entities=False)
     resolver = lxmlSchemaResolver(cntlr, modelXbrl)
     parser.resolvers.add(resolver)
     return parser
 
 def lxmlSchemaValidate(modelDocument: ModelDocument, extraSchema : str | None = None) -> None:
     # lxml schema-validate modelDocument
     if modelDocument is None:
```

### Comparing `arelle-release-2.7.1/arelle/XmlValidateParticles.py` & `arelle-release-2.8.0/arelle/XmlValidateParticles.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/XmlValidateSchema.py` & `arelle-release-2.8.0/arelle/XmlValidateSchema.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/arelle_test.ini` & `arelle-release-2.8.0/arelle/config/arelle_test.ini`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/creationSoftwareNames.json` & `arelle-release-2.8.0/arelle/config/creationSoftwareNames.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/disclosuresystems.xml` & `arelle-release-2.8.0/arelle/config/disclosuresystems.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/disclosuresystems.xsd` & `arelle-release-2.8.0/arelle/config/disclosuresystems.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/edbody.dtd` & `arelle-release-2.8.0/arelle/config/edbody.dtd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/erxl.xsd` & `arelle-release-2.8.0/arelle/config/erxl.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/mappings.xml` & `arelle-release-2.8.0/arelle/config/mappings.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/mappings.xsd` & `arelle-release-2.8.0/arelle/config/mappings.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/xbrlschemafiles.xml` & `arelle-release-2.8.0/arelle/config/xbrlschemafiles.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/xhtml-lat1.ent` & `arelle-release-2.8.0/arelle/config/xhtml-lat1.ent`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/xhtml-special.ent` & `arelle-release-2.8.0/arelle/config/xhtml-special.ent`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/xhtml-symbol.ent` & `arelle-release-2.8.0/arelle/config/xhtml-symbol.ent`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/xhtml1-strict-ix.dtd` & `arelle-release-2.8.0/arelle/config/xhtml1-strict-ix.dtd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/config/xhtml1_1-strict-ix.dtd` & `arelle-release-2.8.0/arelle/config/xhtml1_1-strict-ix.dtd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/doc/messagesCatalog.xml` & `arelle-release-2.8.0/arelle/doc/messagesCatalog.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/doc/messagesCatalog.xsd` & `arelle-release-2.8.0/arelle/doc/messagesCatalog.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/CustomLogger.py` & `arelle-release-2.8.0/arelle/examples/CustomLogger.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/LoadEFMvalidate.py` & `arelle-release-2.8.0/arelle/examples/LoadEFMvalidate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/LoadSavePreLbCsv.py` & `arelle-release-2.8.0/arelle/examples/LoadSavePreLbCsv.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/LoadValidate.cs` & `arelle-release-2.8.0/arelle/examples/LoadValidate.cs`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/LoadValidate.py` & `arelle-release-2.8.0/arelle/examples/LoadValidate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/LoadValidateCmdLine.java` & `arelle-release-2.8.0/arelle/examples/LoadValidateCmdLine.java`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/LoadValidatePostedZip.java` & `arelle-release-2.8.0/arelle/examples/LoadValidatePostedZip.java`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/LoadValidateWebService.java` & `arelle-release-2.8.0/arelle/examples/LoadValidateWebService.java`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/SaveTableToExelle.py` & `arelle-release-2.8.0/arelle/examples/SaveTableToExelle.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/TR3toTR4.py` & `arelle-release-2.8.0/arelle/examples/TR3toTR4.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/bigInstance.py` & `arelle-release-2.8.0/arelle/examples/plugin/bigInstance.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/cmdWebServerExtension.py` & `arelle-release-2.8.0/arelle/examples/plugin/cmdWebServerExtension.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/crashTest.py` & `arelle-release-2.8.0/arelle/examples/plugin/crashTest.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/formulaSuiteConverter.py` & `arelle-release-2.8.0/arelle/examples/plugin/formulaSuiteConverter.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/functionsCustom.py` & `arelle-release-2.8.0/arelle/examples/plugin/functionsCustom.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/hello_dolly.py` & `arelle-release-2.8.0/arelle/examples/plugin/hello_dolly.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/hello_i18n.pot` & `arelle-release-2.8.0/arelle/examples/plugin/hello_i18n.pot`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/hello_i18n.py` & `arelle-release-2.8.0/arelle/examples/plugin/hello_i18n.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/importTestChild1.py` & `arelle-release-2.8.0/arelle/examples/plugin/importTestChild1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/importTestChild2.py` & `arelle-release-2.8.0/arelle/examples/plugin/importTestChild2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/importTestGrandchild1.py` & `arelle-release-2.8.0/arelle/examples/plugin/importTestGrandchild1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/importTestGrandchild2.py` & `arelle-release-2.8.0/arelle/examples/plugin/importTestGrandchild2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/importTestImported1.py` & `arelle-release-2.8.0/arelle/examples/plugin/importTestImported1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/importTestImported11.py` & `arelle-release-2.8.0/arelle/examples/plugin/importTestImported11.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/importTestParent.py` & `arelle-release-2.8.0/arelle/examples/plugin/importTestParent.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/locale/fr/LC_MESSAGES/hello_i18n.po` & `arelle-release-2.8.0/arelle/examples/plugin/locale/fr/LC_MESSAGES/hello_i18n.po`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/__init__.py` & `arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/importTestChild1.py` & `arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/importTestChild1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/importTestChild2.py` & `arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/importTestChild2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/importTestGrandchild1.py` & `arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/importTestGrandchild1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/importTestGrandchild2.py` & `arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/importTestGrandchild2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/importTestImported1.py` & `arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/importTestImported1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/importTestImported11.py` & `arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/importTestImported11.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/subdir/importTestImported111.py` & `arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/subdir/importTestImported111.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/importTestImported1111.py` & `arelle-release-2.8.0/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/importTestImported1111.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/sakaCalendar.py` & `arelle-release-2.8.0/arelle/examples/plugin/sakaCalendar.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/saveInstanceInfoset.py` & `arelle-release-2.8.0/arelle/examples/plugin/saveInstanceInfoset.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/streamingExtensions.py` & `arelle-release-2.8.0/arelle/examples/plugin/streamingExtensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/testcaseIxExpectedHtmlFixup.py` & `arelle-release-2.8.0/arelle/examples/plugin/testcaseIxExpectedHtmlFixup.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/updateTableLB.py` & `arelle-release-2.8.0/arelle/examples/plugin/updateTableLB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/validateSchemaLxml.py` & `arelle-release-2.8.0/arelle/examples/plugin/validateSchemaLxml.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/plugin/validateTableInfoset.py` & `arelle-release-2.8.0/arelle/examples/plugin/validateTableInfoset.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/us-gaap-dei-docType-extraction-frm.xml` & `arelle-release-2.8.0/arelle/examples/us-gaap-dei-docType-extraction-frm.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/examples/us-gaap-dei-ratio-cash-frm.xml` & `arelle-release-2.8.0/arelle/examples/us-gaap-dei-ratio-cash-frm.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/formula/FactAspectsCache.py` & `arelle-release-2.8.0/arelle/formula/FactAspectsCache.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/formula/FormulaConsisAsser.py` & `arelle-release-2.8.0/arelle/formula/FormulaConsisAsser.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/formula/FormulaEvaluator.py` & `arelle-release-2.8.0/arelle/formula/FormulaEvaluator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/formula/ValidateFormula.py` & `arelle-release-2.8.0/arelle/formula/ValidateFormula.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/formula/XPathContext.py` & `arelle-release-2.8.0/arelle/formula/XPathContext.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/formula/XPathParser.py` & `arelle-release-2.8.0/arelle/formula/XPathParser.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/arelle-full-word.ico` & `arelle-release-2.8.0/arelle/images/arelle-full-word.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/arelle-mac-icon-4.gif` & `arelle-release-2.8.0/arelle/images/arelle-mac-icon-4.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/arelle-word-only.ico` & `arelle-release-2.8.0/arelle/images/arelle-word-only.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/arelle.gif` & `arelle-release-2.8.0/arelle/images/arelle.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/arelle.icns` & `arelle-release-2.8.0/arelle/images/arelle.icns`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/arelle.icns.zip` & `arelle-release-2.8.0/arelle/images/arelle.icns.zip`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/arelle.ico` & `arelle-release-2.8.0/arelle/images/arelle.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/arelle128.psd` & `arelle-release-2.8.0/arelle/images/arelle128.psd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/arelle16.psd` & `arelle-release-2.8.0/arelle/images/arelle16.psd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/arelle16x16and32x32.ico` & `arelle-release-2.8.0/arelle/images/arelle16x16and32x32.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/arelle32.gif` & `arelle-release-2.8.0/arelle/images/arelle32.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/dmg_background.png` & `arelle-release-2.8.0/arelle/images/dmg_background.png`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/octocat.png` & `arelle-release-2.8.0/arelle/images/octocat.png`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/python-clear.png` & `arelle-release-2.8.0/arelle/images/python-clear.png`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/python-icon-pack-crystalxp.net-842.zip` & `arelle-release-2.8.0/arelle/images/python-icon-pack-crystalxp.net-842.zip`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/toolbarClose.gif` & `arelle-release-2.8.0/arelle/images/toolbarClose.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/toolbarCompare.gif` & `arelle-release-2.8.0/arelle/images/toolbarCompare.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/toolbarFindMenu.gif` & `arelle-release-2.8.0/arelle/images/toolbarFindMenu.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/toolbarLogClear - 1-piece-top.gif` & `arelle-release-2.8.0/arelle/images/toolbarLogClear - 1-piece-top.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/toolbarLogClear-orig.gif` & `arelle-release-2.8.0/arelle/images/toolbarLogClear-orig.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/toolbarLogClear.gif` & `arelle-release-2.8.0/arelle/images/toolbarLogClear.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/toolbarNewFile.gif` & `arelle-release-2.8.0/arelle/images/toolbarNewFile.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/toolbarOpenFile.gif` & `arelle-release-2.8.0/arelle/images/toolbarOpenFile.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/toolbarOpenWeb.gif` & `arelle-release-2.8.0/arelle/images/toolbarOpenWeb.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/toolbarReopen.gif` & `arelle-release-2.8.0/arelle/images/toolbarReopen.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/toolbarSaveFile.gif` & `arelle-release-2.8.0/arelle/images/toolbarSaveFile.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/toolbarValidate.gif` & `arelle-release-2.8.0/arelle/images/toolbarValidate.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/xbrl.gif` & `arelle-release-2.8.0/arelle/images/xbrl.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/xbrl.psd` & `arelle-release-2.8.0/arelle/images/xbrl.psd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/xbrl128-2.gif` & `arelle-release-2.8.0/arelle/images/xbrl128-2.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/xbrl128.gif` & `arelle-release-2.8.0/arelle/images/xbrl128.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/xbrl16.ico` & `arelle-release-2.8.0/arelle/images/xbrl16.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/images/xbrl32.ico` & `arelle-release-2.8.0/arelle/images/xbrl32.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/locale/ar_EG/LC_MESSAGES/ar_EG.po` & `arelle-release-2.8.0/arelle/locale/ar_EG/LC_MESSAGES/ar_EG.po`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/locale/ar_EG/LC_MESSAGES/arelle.mo` & `arelle-release-2.8.0/arelle/locale/ar_EG/LC_MESSAGES/arelle.mo`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/locale/es/LC_MESSAGES/arelle.mo` & `arelle-release-2.8.0/arelle/locale/es/LC_MESSAGES/arelle.mo`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/locale/fr/LC_MESSAGES/arelle.mo` & `arelle-release-2.8.0/arelle/locale/fr/LC_MESSAGES/arelle.mo`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/locale/fr/LC_MESSAGES/fr.po` & `arelle-release-2.8.0/arelle/locale/fr/LC_MESSAGES/fr.po`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/locale/messages.pot` & `arelle-release-2.8.0/arelle/locale/messages.pot`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/locale/ru/LC_MESSAGES/arelle.mo` & `arelle-release-2.8.0/arelle/locale/ru/LC_MESSAGES/arelle.mo`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/locale/ru/LC_MESSAGES/ru.po` & `arelle-release-2.8.0/arelle/locale/ru/LC_MESSAGES/ru.po`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/EdgarRendererAllReports.py` & `arelle-release-2.8.0/arelle/plugin/EdgarRendererAllReports.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/SECCorrespondenceLoader.py` & `arelle-release-2.8.0/arelle/plugin/SECCorrespondenceLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/TDnetLoader.py` & `arelle-release-2.8.0/arelle/plugin/TDnetLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/UKCompaniesHouseLoader.py` & `arelle-release-2.8.0/arelle/plugin/UKCompaniesHouseLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/formulaLoader.py` & `arelle-release-2.8.0/arelle/plugin/formulaLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/formulaSaver.py` & `arelle-release-2.8.0/arelle/plugin/formulaSaver.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/formulaXPathChecker.py` & `arelle-release-2.8.0/arelle/plugin/formulaXPathChecker.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/functionsMath.py` & `arelle-release-2.8.0/arelle/plugin/functionsMath.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/functionsXmlCreation.py` & `arelle-release-2.8.0/arelle/plugin/functionsXmlCreation.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/inlineXbrlDocumentSet.py` & `arelle-release-2.8.0/arelle/plugin/inlineXbrlDocumentSet.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,42 @@
 
 If the file source is a zip, CmdLine will discover the inline files in the zip as thus:
     --file '[{"ixds":[{"file":file1.zip}]}]'
 
 If the file source is a local directory, CmdLine will discover the inline files in the directory as thus:
     --file '[{"ixds":[{"file":dir1}]}]'
 
-For GUI operation specify a formula parameter named ixdsTarget of type xs:string (in formula tools->formula parameters).
+If there is a JSON structure in --file without ixdsTarget the default target is assumed.
 
-If a ixdsTarget parameter is absent or has a value of an empty string it is the default target document and matches
-ix facts and resources with no @target attribute.
+If no JSON structure then formula parameter ixdsTarget may be used to specify a non-default target or the
+special value "(default)" for the default target (e.g., resources with no @target attribute).
+
+For GUI instance loading a pop up selection dialog is provided when there is no formula parameter and there are multiple targets.
+
+Example to load multi-document IXDS and save extracted xBRL-XML target document:
+
+  For GUI using ix11 conformance suite directory multi-io test case "PASS-multiple-input-multiple-output"
+     File->Open File Inline Doc Set->multi-select PASS-multiple-input-multiple-output-ID1.html and PASS-multiple-input-multiple-output-ID2.html
+     Select Target -> (default)
+     Tools->Save Target Document
+     new file PASS-multiple-input-multiple-output-ID1_extracted.xbrl has (default) target xBRL-XML instance
+     close instance
+     Reopen as above and Select Target -> TARGET
+     Tools->Save Target Document
+     replaced file PASS-multiple-input-multiple-output-ID1_extracted.xbrl now has TARGET target xBRL-XML instance
+  For Command Line:
+     arelleCmdLine --plugin inlineXbrlDocumentSet
+                   --file '[{"ixds":[{"file":".../PASS-multiple-input-multiple-output-ID1.html"},
+                                     {"file":".../PASS-multiple-input-multiple-output-ID2.html"}],
+                             "ixdsTarget":"(default)"}]'
+                   --saveInstance
+     For second target specify "ixdsTarget":"TARGET"
+     For default target either omit ixdsTarget or specify (default).
+     File will be saved as PASS-multiple-input-multiple-output-ID1_extracted.xbrl regardless of ixdsTarget parameter
+     For EDGAR style encoding of non-ASCII characters add --encodeSavedXmlChars
 
 See COPYRIGHT.md for copyright information.
 '''
 from arelle import FileSource, ModelXbrl, ValidateXbrlDimensions, XbrlConst
 DialogURL = None # dynamically imported when first used
 from arelle.PrototypeDtsObject import LocPrototype, ArcPrototype
 from arelle.FileSource import archiveFilenameParts, archiveFilenameSuffixes
@@ -39,14 +63,15 @@
 from arelle.ModelValue import qname
 from arelle.PluginManager import pluginClassMethods
 from arelle.PythonUtil import attrdict
 from arelle.UrlUtil import isHttpUrl
 from arelle.ValidateFilingText import CDATApattern
 from arelle.Version import authorLabel, copyrightLabel
 from arelle.XmlUtil import addChild, copyIxFootnoteHtml, elementFragmentIdentifier, elementChildSequence, xmlnsprefix, setXmlns
+from arelle.XmlValidate import validate as xmlValidate
 import os, zipfile
 import regex as re
 from optparse import SUPPRESS_HELP
 from lxml.etree import XML, XMLSyntaxError
 from collections import defaultdict
 
 IXDS_SURROGATE = "_IXDS#?#" # surrogate (fake) file name for inline XBRL doc set (IXDS)
@@ -81,23 +106,23 @@
                                 self.targetDocumentSchemaRefs.add(doc.relativeUri(referencedDoc.uri))
         return True
 
 # this loader is used for test cases of multi-ix doc sets
 def inlineXbrlDocumentSetLoader(modelXbrl, normalizedUri, filepath, isEntry=False, namespace=None, **kwargs):
     if isEntry:
         try:
-            if "entrypoint" in kwargs:
-                _target = kwargs["entrypoint"]["ixdsTarget"]
+            if "entrypoint" in kwargs and "ixdsTarget" in kwargs["entrypoint"]:
+                _target = kwargs["entrypoint"].get("ixdsTarget") # assume None if not specified in entrypoint
             elif "ixdsTarget" in kwargs: # passed from validate (multio test cases)
                 _target = kwargs["ixdsTarget"]
             else:
-                _target = modelXbrl.modelManager.formulaOptions.parameterValues.get("ixdsTarget")[1]
+                _target = modelXbrl.modelManager.formulaOptions.parameterValues["ixdsTarget"][1]
+            modelXbrl.ixdsTarget = None if _target == "(default)" else _target or None
         except (KeyError, AttributeError, IndexError, TypeError):
-            _target = None
-        modelXbrl.ixdsTarget = _target or None # None if an empty string specified
+            pass # set later in selectTargetDocument plugin method
     if IXDS_SURROGATE in normalizedUri:
         # create surrogate entry object for inline document set which references ix documents
         xml = ["<instances>\n"]
         modelXbrl.ixdsDocUrls = []
         schemeFixup = isHttpUrl(normalizedUri) # schemes after separator have // normalized to single /
         msUNCfixup = modelXbrl.modelManager.cntlr.isMSW and normalizedUri.startswith("\\\\") # path starts with double backslash \\
         if schemeFixup:
@@ -612,14 +637,71 @@
         _entrypointFiles = entrypointFiles.copy()
         del entrypointFiles[:]
         entrypointFiles.append( {"ixds": _entrypointFiles} )
 
 def inlineDocsetUrlSeparator():
     return IXDS_DOC_SEPARATOR
 
+def discoverIxdsDts(modelXbrl):
+    return hasattr(modelXbrl, "ixdsTarget") # if no target specified, block ixds discovery until all IX docs are loaded
+
+class TargetChoiceDialog:
+    def __init__(self,parent, choices):
+        from tkinter import Toplevel, Label, Listbox, StringVar
+        parentGeometry = re.match("(\d+)x(\d+)[+]?([-]?\d+)[+]?([-]?\d+)", parent.geometry())
+        dialogX = int(parentGeometry.group(3))
+        dialogY = int(parentGeometry.group(4))
+        self.parent = parent
+        self.t = Toplevel()
+        self.t.transient(self.parent)
+        self.t.geometry("+{0}+{1}".format(dialogX+200,dialogY+200))
+        self.t.title(_("Select Target"))
+        self.selection = choices[0] # default choice in case dialog is closed without selecting an entry
+        self.lb = Listbox(self.t, height=10, width=30, listvariable=StringVar(value=choices))
+        self.lb.grid(row=0, column=0)
+        self.lb.focus_set()
+        self.lb.bind("<<ListboxSelect>>", self.select)
+        self.t.grab_set()
+        self.t.wait_window(self.t)
+
+    def select(self,event):
+        self.parent.focus_set()
+        self.selection = self.lb.selection_get()
+        self.t.destroy()
+
+def selectTargetDocument(modelXbrl):
+    if not hasattr(modelXbrl, "ixdsTarget"): # DTS discoverey deferred until all ix docs loaded
+        # find target attributes
+        _targets = sorted(set(elt.get("target", "(default)")
+                              for htmlElt in modelXbrl.ixdsHtmlElements
+                              for elt in htmlElt.iterfind(f".//{{{htmlElt.modelDocument.ixNS}}}references")))
+        if len(_targets) == 1:
+            _target = _targets[0]
+        elif modelXbrl.modelManager.cntlr.hasGui:
+            dlg = TargetChoiceDialog(modelXbrl.modelManager.cntlr.parent, _targets)
+            _target = dlg.selection
+        else:
+            _target = _targets[0]
+            modelXbrl.warning("arelle:unspecifiedTargetDocument",
+                              _("Target document not specified, loading %(target)s, found targets %(targets)s"),
+                              modelObject=modelXbrl, target=_target, targets=_targets)
+        modelXbrl.ixdsTarget = None if _target == "(default)" else _target or None
+        # load referenced schemas and linkbases (before validating inline HTML
+        for htmlElt in modelXbrl.ixdsHtmlElements:
+            modelDoc = htmlElt.modelDocument
+            for ixRefElt in htmlElt.iterdescendants(tag=modelDoc.ixNStag + "references"):
+                if ixRefElt.get("target") == modelXbrl.ixdsTarget:
+                    modelDoc.schemaLinkbaseRefsDiscover(ixRefElt)
+                    xmlValidate(modelXbrl, ixRefElt) # validate instance elements
+    # now that all ixds doc(s) references loaded, validate resource elements
+    for htmlElt in modelXbrl.ixdsHtmlElements:
+        for inlineElement in htmlElt.iterdescendants(tag=htmlElt.modelDocument.ixNStag + "resources"):
+            xmlValidate(modelXbrl, inlineElement) # validate instance elements
+
+
 __pluginInfo__ = {
     'name': 'Inline XBRL Document Set',
     'version': '1.1',
     'description': "This plug-in adds a feature to read manifest files of inline XBRL document sets "
                     " and to save the embedded XBRL instance document.  "
                     "Support single target instance documents in a single document set.  ",
     'license': 'Apache-2',
@@ -633,12 +715,14 @@
     'CntlrWinMain.Menu.Tools': saveTargetDocumentMenuEntender,
     'CntlrCmdLine.Options': commandLineOptionExtender,
     'CntlrCmdLine.Filing.Start': commandLineFilingStart,
     'CntlrCmdLine.Xbrl.Run': commandLineXbrlRun,
     'ModelDocument.PullLoader': inlineXbrlDocumentSetLoader,
     'ModelDocument.IdentifyType': identifyInlineXbrlDocumentSet,
     'ModelDocument.Discover': discoverInlineXbrlDocumentSet,
+    'ModelDocument.DiscoverIxdsDts': discoverIxdsDts,
+    'ModelDocument.SelectIxdsTarget': selectTargetDocument,
     'ModelTestcaseVariation.ReadMeFirstUris': testcaseVariationReadMeFirstUris,
     'ModelTestcaseVariation.ArchiveIxds': testcaseVariationArchiveIxds,
     'ModelTestcaseVariation.ReportPackageIxds': testcaseVariationReportPackageIxds,
     'ModelTestcaseVariation.ResultXbrlInstanceUri': testcaseVariationResultInstanceUri,
 }
```

### Comparing `arelle-release-2.7.1/arelle/plugin/instanceInfo.py` & `arelle-release-2.8.0/arelle/plugin/instanceInfo.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/HTTPNtlmAuthHandler.py` & `arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/HTTPNtlmAuthHandler.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/U32.py` & `arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/U32.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/__init__.py` & `arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/des.py` & `arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/des.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/des_c.py` & `arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/des_c.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/des_data.py` & `arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/des_data.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/lgpl-3.0-standalone.html` & `arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/lgpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/internet/proxyNTLM/ntlm.py` & `arelle-release-2.8.0/arelle/plugin/internet/proxyNTLM/ntlm.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/loadFromExcel.py` & `arelle-release-2.8.0/arelle/plugin/loadFromExcel.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/loadFromOIM-2018.py` & `arelle-release-2.8.0/arelle/plugin/loadFromOIM-2018.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/loadFromOIM.py` & `arelle-release-2.8.0/arelle/plugin/loadFromOIM.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/logging/dpmSignature.py` & `arelle-release-2.8.0/arelle/plugin/logging/dpmSignature.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/logging/dqcParameters.py` & `arelle-release-2.8.0/arelle/plugin/logging/dqcParameters.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/logging/saveMessages.py` & `arelle-release-2.8.0/arelle/plugin/logging/saveMessages.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/objectmaker.py` & `arelle-release-2.8.0/arelle/plugin/objectmaker.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/profileCmdLine.py` & `arelle-release-2.8.0/arelle/plugin/profileCmdLine.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/profileFormula.py` & `arelle-release-2.8.0/arelle/plugin/profileFormula.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/saveCHComponentFile.py` & `arelle-release-2.8.0/arelle/plugin/saveCHComponentFile.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/saveDTS.py` & `arelle-release-2.8.0/arelle/plugin/saveDTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/saveHtmlEBAtables.py` & `arelle-release-2.8.0/arelle/plugin/saveHtmlEBAtables.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/saveLoadableExcel.py` & `arelle-release-2.8.0/arelle/plugin/saveLoadableExcel.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/saveLoadableOIM.py` & `arelle-release-2.8.0/arelle/plugin/saveLoadableOIM.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/saveSKOS.py` & `arelle-release-2.8.0/arelle/plugin/saveSKOS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/saveSampleInstance.py` & `arelle-release-2.8.0/arelle/plugin/saveSampleInstance.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/security/cryptAES_CBC.py` & `arelle-release-2.8.0/arelle/plugin/security/cryptAES_CBC.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/security/cryptAES_EAX.py` & `arelle-release-2.8.0/arelle/plugin/security/cryptAES_EAX.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/sphinx/FormulaGenerator.py` & `arelle-release-2.8.0/arelle/plugin/sphinx/FormulaGenerator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/sphinx/SphinxContext.py` & `arelle-release-2.8.0/arelle/plugin/sphinx/SphinxContext.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/sphinx/SphinxEvaluator.py` & `arelle-release-2.8.0/arelle/plugin/sphinx/SphinxEvaluator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/sphinx/SphinxMethods.py` & `arelle-release-2.8.0/arelle/plugin/sphinx/SphinxMethods.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/sphinx/SphinxParser.py` & `arelle-release-2.8.0/arelle/plugin/sphinx/SphinxParser.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/sphinx/SphinxValidator.py` & `arelle-release-2.8.0/arelle/plugin/sphinx/SphinxValidator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/sphinx/US-GAAP Ratios Example.xsr` & `arelle-release-2.8.0/arelle/plugin/sphinx/US-GAAP Ratios Example.xsr`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/sphinx/__init__.py` & `arelle-release-2.8.0/arelle/plugin/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/streamingExtensions.py` & `arelle-release-2.8.0/arelle/plugin/streamingExtensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/__init__.py` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/README.md` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/extractTestcase.xsl` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/extractTestcase.xsl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/runIxtSecTests.sh` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/runIxtSecTests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/saxon9.jar` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/saxon9.jar`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/testcase.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/testcase.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/conf/tests.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/conf/tests.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/text2num.py` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/text2num.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-boolballotbox.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-boolballotbox.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-countrynameen.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-countrynameen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-datequarterend.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-datequarterend.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durday.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durday.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durhour.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durhour.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durmonth.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durmonth.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durweek.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durweek.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durwordsen.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durwordsen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-duryear.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-duryear.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-edgarprovcountryen.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-edgarprovcountryen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-entityfilercategoryen.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-entityfilercategoryen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-exchnameen.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-exchnameen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-numwordsen.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-numwordsen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-stateprovnameen.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-stateprovnameen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-yesnoballotbox.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-yesnoballotbox.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/transform-registry.xml` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/transform-registry.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/SEC/transformationRegistry/schema/inlinexbrl-sec-transformation.xsd` & `arelle-release-2.8.0/arelle/plugin/transforms/SEC/transformationRegistry/schema/inlinexbrl-sec-transformation.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/transforms/tester.py` & `arelle-release-2.8.0/arelle/plugin/transforms/tester.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/unpackSecEisFile.py` & `arelle-release-2.8.0/arelle/plugin/unpackSecEisFile.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/CIPC/Const.py` & `arelle-release-2.8.0/arelle/plugin/validate/CIPC/Const.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/CIPC/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/CIPC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/CIPC/config.xml` & `arelle-release-2.8.0/arelle/plugin/validate/CIPC/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EBA/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/EBA/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EBA/config.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EBA/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/Consts.py` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/Consts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/DTS.py` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/DTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/Dimensions.py` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/Dimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/Document.py` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/Document.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/Filing.py` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/Filing.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/PreCalAlignment.py` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/PreCalAlignment.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/Util.py` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/Util.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/config.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/README.md` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/axiswarnings.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/axiswarnings.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/dei-validations.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/dei-validations.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/dqc-us-rules.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/dqc-us-rules.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-16-4.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-16-4.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-0-4.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-0-4.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-1.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-2.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-3-1.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-3-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.1.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.2.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.3.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.3.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-1.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-2.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-3.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-3.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-1.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-2.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-3.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-3.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2012.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2012.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2013.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2013.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2014.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2014.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2015.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2015.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2016.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2016.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-1.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-2.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-3.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-3.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-4.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-4.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1-preview.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1-preview.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2-2.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-4.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-4.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1-1.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-all-years.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-all-years.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/erxl.xsd` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/erxl.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/extendedtaxonomies-all-years.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/extendedtaxonomies-all-years.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrs-taxonomies.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrs-taxonomies.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrstaxonomies-all-years.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrstaxonomies-all-years.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/exch-deprecated-concepts.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/exch-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/ifrs-full-deprecated-concepts.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/ifrs-full-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/invest-deprecated-concepts.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/invest-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/ixbrl-transform-registries.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/ixbrl-transform-registries.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/naics-deprecated-concepts.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/naics-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/rr-deprecated-concepts.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/rr-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/signwarnings.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/signwarnings.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/taxonomy-compatibility.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/taxonomy-compatibility.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/us-gaap-deprecated-concepts.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/us-gaap-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2020.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2020.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2021.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2021.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2022.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2022.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2023.json` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2023.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM/tools/CheckTxmyRefs.py` & `arelle-release-2.8.0/arelle/plugin/validate/EFM/tools/CheckTxmyRefs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM-htm/Const.py` & `arelle-release-2.8.0/arelle/plugin/validate/EFM-htm/Const.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM-htm/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/EFM-htm/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM-htm/config.xml` & `arelle-release-2.8.0/arelle/plugin/validate/EFM-htm/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/EFM-htm/resources/efm-htm.dtd` & `arelle-release-2.8.0/arelle/plugin/validate/EFM-htm/resources/efm-htm.dtd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF/Const.py` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/Const.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 '''
-Filer Guidelines: esma32-60-254_esef_reporting_manual.pdf
+Version 2022 created on September 19, 2022
+
+Filer Guidelines: https://www.esma.europa.eu/sites/default/files/library/esma32-60-254_esef_reporting_manual.pdf
 
 See COPYRIGHT.md for copyright information.
 '''
 from __future__ import annotations
 import regex as re
-from typing import Any, Callable
 from arelle.ModelValue import QName, qname
 from arelle.XbrlConst import all, notAll, hypercubeDimension, dimensionDomain, domainMember, dimensionDefault, widerNarrower
 
 browserMaxBase64ImageLength = 5242880 # 5MB
 
 esefTaxonomyNamespaceURIs = {
     "http://xbrl.ifrs.org/taxonomy/20",
-    "http://xbrl.ifrs.org/taxonomy/20",
+    "https://xbrl.ifrs.org/taxonomy/20",
     }
 
 disallowedURIsPattern = re.compile(
     "http://xbrl.ifrs.org/taxonomy/[0-9-]{10}/full_ifrs/full_ifrs-cor_[0-9-]{10}[.]xsd|"
     "http://www.esma.europa.eu/taxonomy/[0-9-]{10}/esef_all.xsd"
     )
 
+esefCorNsPattern = re.compile(r"https?://www\.esma\.europa\.eu/taxonomy/[0-9-]{10}/esef_cor")
 
-DefaultDimensionLinkroles = ("http://www.esma.europa.eu/xbrl/role/cor/ifrs-dim_role-990000",)
-LineItemsNotQualifiedLinkrole = "http://www.esma.europa.eu/xbrl/role/cor/esef_role-999999"
+DefaultDimensionLinkroles = ("https://www.esma.europa.eu/xbrl/role/cor/ifrs-dim_role-990000", # preferred, new spec
+                             "http://www.esma.europa.eu/xbrl/role/cor/ifrs-dim_role-990000")
+LineItemsNotQualifiedLinkroles = ("https://www.esma.europa.eu/xbrl/role/cor/esef_role-999999", # preferred, new spec
+                                  "http://www.esma.europa.eu/xbrl/role/cor/esef_role-999999")
 
 qnDomainItemTypes = {qname("{http://www.xbrl.org/dtr/type/non-numeric}nonnum:domainItemType"),
                      qname("{http://www.xbrl.org/dtr/type/2020-01-21}nonnum:domainItemType")}
 
 
 linkbaseRefTypes = {
     "http://www.xbrl.org/2003/role/calculationLinkbaseRef": "cal",
@@ -79,14 +83,18 @@
     # from Annex II para 1
     "StatementOfFinancialPositionAbstract",
     "StatementOfProfitOrLossAndOtherComprehensiveIncomeAbstract"
     "StatementOfChangesInEquityAbstract",
     "StatementOfCashFlowsAbstract",
     }
 
+esefNotesStatementConcepts = {
+    "NotesAccountingPoliciesAndMandatoryTags",
+}
+
 esefMandatoryElementNames2020 = (
     "NameOfReportingEntityOrOtherMeansOfIdentification",
     "ExplanationOfChangeInNameOfReportingEntityOrOtherMeansOfIdentificationFromEndOfPrecedingReportingPeriod",
     "DomicileOfEntity",
     "LegalFormOfEntity",
     "CountryOfIncorporation",
     "AddressOfRegisteredOfficeOfEntity",
@@ -337,7 +345,163 @@
     "LengthOfLifeOfLimitedLifeEntity",
     "NameOfParentEntity",
     "NameOfReportingEntityOrOtherMeansOfIdentification",
     "NameOfUltimateParentOfGroup",
     "PrincipalPlaceOfBusiness",
     "StatementOfIFRSCompliance",
 )
+
+htmlEventHandlerAttributes = set((
+    "onabort",
+    "onafterprint",
+    "onbeforeprint",
+    "onbeforeunload",
+    "onblur",
+    "oncanplay",
+    "oncanplaythrough",
+    "onchange",
+    "onclick",
+    "oncontextmenu",
+    "oncopy",
+    "oncuechange",
+    "oncut",
+    "ondblclick",
+    "ondrag",
+    "ondragend",
+    "ondragenter",
+    "ondragleave",
+    "ondragover",
+    "ondragstart",
+    "ondrop",
+    "ondurationchange",
+    "onemptied",
+    "onended",
+    "onerror",
+    "onfocus",
+    "onhashchange",
+    "oninput",
+    "oninvalid",
+    "onkeydown",
+    "onkeypress",
+    "onkeyup",
+    "onload",
+    "onloadeddata",
+    "onloadedmetadata",
+    "onloadstart",
+    "onmessage",
+    "onmousedown",
+    "onmousemove",
+    "onmouseout",
+    "onmouseover",
+    "onmouseup",
+    "onmousewheel",
+    "onoffline",
+    "ononline",
+    "onpagehide",
+    "onpageshow",
+    "onpaste",
+    "onpause",
+    "onplay",
+    "onplaying",
+    "onpopstate",
+    "onprogress",
+    "onratechange",
+    "onreset",
+    "onresize",
+    "onscroll",
+    "onsearch",
+    "onseeked",
+    "onseeking",
+    "onselect",
+    "onstalled",
+    "onstorage",
+    "onsubmit",
+    "onsuspend",
+    "ontimeupdate",
+    "ontoggle",
+    "onunload",
+    "onvolumechange",
+    "onwaiting",
+    "onwheel",
+))
+
+svgEventAttributes = set((
+    "onabort",
+    "onactivate",
+    "onafterprint",
+    "onbeforeprint",
+    "onbegin",
+    "oncancel",
+    "oncanplay",
+    "oncanplaythrough",
+    "onchange",
+    "onclick",
+    "onclose",
+    "oncopy",
+    "oncuechange",
+    "oncut",
+    "ondblclick",
+    "ondrag",
+    "ondragend",
+    "ondragenter",
+    "ondragexit",
+    "ondragleave",
+    "ondragover",
+    "ondragstart",
+    "ondrop",
+    "ondurationchange",
+    "onemptied",
+    "onend",
+    "onended",
+    "onerror",
+    "onfocus",
+    "onfocusin",
+    "onfocusout",
+    "onhashchange",
+    "oninput",
+    "oninvalid",
+    "onkeydown",
+    "onkeypress",
+    "onkeyup",
+    "onload",
+    "onloadeddata",
+    "onloadedmetadata",
+    "onloadstart",
+    "onmessage",
+    "onmousedown",
+    "onmouseenter",
+    "onmouseleave",
+    "onmousemove",
+    "onmouseout",
+    "onmouseover",
+    "onmouseup",
+    "onmousewheel",
+    "onoffline",
+    "ononline",
+    "onpagehide",
+    "onpageshow",
+    "onpaste",
+    "onpause",
+    "onplay",
+    "onplaying",
+    "onpopstate",
+    "onprogress",
+    "onratechange",
+    "onrepeat",
+    "onreset",
+    "onresize",
+    "onscroll",
+    "onseeked",
+    "onseeking",
+    "onselect",
+    "onshow",
+    "onstalled",
+    "onstorage",
+    "onsubmit",
+    "onsuspend",
+    "ontimeupdate",
+    "ontoggle",
+    "onunload",
+    "onvolumechange",
+    "onwaiting",
+    "onzoom"
+))
```

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF/DTS.py` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF/DTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF/Dimensions.py` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF/Dimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF/Util.py` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF/Util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 '''
 Filer Guidelines: ESMA_ESEF Manula 2019.pdf
 
 See COPYRIGHT.md for copyright information.
 '''
 from __future__ import annotations
+from lxml.etree import _Element
+from urllib.parse import unquote
 import os, json
 from arelle.ModelObject import ModelObject
-from .Const import esefTaxonomyNamespaceURIs
+from .Const import esefTaxonomyNamespaceURIs, htmlEventHandlerAttributes, svgEventAttributes
 from lxml.etree import XML, XMLSyntaxError
 from arelle.FileSource import openFileStream
 from arelle.UrlUtil import scheme
 from arelle.ModelManager import ModelManager
 from arelle.ModelXbrl import ModelXbrl
 from arelle.ValidateXbrl import ValidateXbrl
 from typing import Any, Dict, List, Union, cast
@@ -43,45 +45,31 @@
     return (any(ns.startswith(esefNsPrefix) for esefNsPrefix in esefTaxonomyNamespaceURIs))
 
 supportedImgTypes: dict[bool, tuple[str, ...]] = {
     True: ("gif", "jpg", "jpeg", "png"), # file extensions
     False: ("gif", "jpeg", "png") # mime types: jpg is not a valid mime type
     }
 # check image contents against mime/file ext and for Steganography
-def checkImageContents(modelXbrl: ModelXbrl, imgElt: ModelObject, imgType: str, isFile: bool, data: bytes) -> None:
+
+def checkImageContents(modelXbrl: ModelXbrl, imgElt: ModelObject, imgType: str, isFile: bool, data: bytes, consolidated: bool) -> None:
+    guidance = 'ESEF.2.5.1' if consolidated else 'ESEF.4.1.3'
     if "svg" in imgType:
         try:
-            rootElement = True
-            for elt in XML(data).iter():
-                if rootElement:
-                    if elt.tag != "{http://www.w3.org/2000/svg}svg":
-                        modelXbrl.error("ESEF.2.5.1.imageFileCannotBeLoaded",
-                            _("Image SVG has root element which is not svg"),
-                            modelObject=imgElt)
-                    rootElement = False
-                eltTag = elt.tag.rpartition("}")[2] # strip namespace
-                if ((eltTag in ("object", "script")) or
-                    (eltTag in ("audio", "foreignObject", "iframe", "image", "use", "video"))):
-                    href = elt.get("href","")
-                    if eltTag in ("object", "script") or "javascript:" in href:
-                        modelXbrl.error("ESEF.2.5.1.executableCodePresent",
-                            _("Inline XBRL images MUST NOT contain executable code: %(element)s"),
-                            modelObject=imgElt, element=eltTag)
-                    elif scheme(href) in ("http", "https", "ftp"):
-                        modelXbrl.error("ESEF.2.5.1.referencesPointingOutsideOfTheReportingPackagePresent",
-                            _("Inline XBRL instance document [image] MUST NOT contain any reference pointing to resources outside the reporting package: %(element)s"),
-                            modelObject=imgElt, element=eltTag)
-        except (XMLSyntaxError, UnicodeDecodeError) as err:
-            modelXbrl.error("ESEF.2.5.1.imageFileCannotBeLoaded",
+            checkSVGContent(modelXbrl, imgElt, data, guidance)
+        except XMLSyntaxError as err:
+            try:
+                checkSVGContent(modelXbrl, imgElt, unquote(data), guidance)  # Try with utf-8 decoded data as in conformance suite G4-1-3_2/TC2
+            except XMLSyntaxError:
+                modelXbrl.error(f"{guidance}.imageFileCannotBeLoaded",
+                                _("Image SVG has XML error %(error)s"),
+                                modelObject=imgElt, error=err)
+        except UnicodeDecodeError as err:
+            modelXbrl.error(f"{guidance}.imageFileCannotBeLoaded",
                 _("Image SVG has XML error %(error)s"),
                 modelObject=imgElt, error=err)
-    elif not any(it in imgType for it in supportedImgTypes[isFile]):
-        modelXbrl.error("ESEF.2.5.1.imageFormatNotSupported",
-            _("Images included in the XHTML document MUST be saved in PNG, GIF, SVG or JPEG formats: %(imgType)s is not supported"),
-            modelObject=imgElt, imgType=imgType)
     else:
         if data[:3] == b"GIF" and data[3:6] in (b'89a', b'89b', b'87a'):
             headerType = "gif"
         elif data[:2] == b"\xff\xd8":
             headerType = "jpg"
         elif data[:8] == b"\x89PNG\r\n\x1a\n":
             headerType = "png"
@@ -93,22 +81,53 @@
             headerType = "ico"
         elif data[:4] == b"\x00\x00\x02\x00":
             headerType = "cur"
         elif len(data) == 0:
             headerType = "none"
         else:
             headerType = "unrecognized"
-        if (("gif" in imgType and headerType != "gif") or
-            (("jpg" in imgType or "jpeg" in imgType) and headerType != "jpg") or
-            ("png" in imgType and headerType != "png")):
-            modelXbrl.error("ESEF.2.5.1.imageDoesNotMatchItsFileExtension" if isFile
-                            else "ESEF.2.5.1.incorrectMIMETypeSpecified",
-                _("Image type %(imgType)s has wrong header type: %(headerType)s"),
+        if (("gif" not in imgType and headerType == "gif") or
+            ("jpeg" not in imgType and headerType == "jpg") or
+            ("png" not in imgType and headerType == "png")):
+            imageDoesNotMatchItsFileExtension = f"ESEF.{guidance}.imageDoesNotMatchItsFileExtension"
+            incorrectMIMETypeSpecified = f"ESEF.{guidance}.incorrectMIMETypeSpecified"
+            modelXbrl.error(imageDoesNotMatchItsFileExtension if isFile else incorrectMIMETypeSpecified,
+                _("Header type %(headerType)s has wrong image type: %(imgType)s"),
                 modelObject=imgElt, imgType=imgType, headerType=headerType,
-                messageCodes=("ESEF.2.5.1.imageDoesNotMatchItsFileExtension", "ESEF.2.5.1.incorrectMIMETypeSpecified"))
+                messageCodes=(imageDoesNotMatchItsFileExtension, incorrectMIMETypeSpecified))
+        elif not any(it in imgType for it in supportedImgTypes[isFile]):
+            modelXbrl.error(f"{guidance}.imageFormatNotSupported",
+                            _("Images included in the XHTML document MUST be saved in PNG, GIF, SVG or JPEG formats: %(imgType)s is not supported"),
+                            modelObject=imgElt, imgType=imgType)
+
+
+def checkSVGContent(modelXbrl: ModelXbrl, imgElt: ModelObject, data: Union[bytes, Any, str], guidance: str) -> None:
+    rootElement = True
+    for elt in XML(data).iter():
+        if rootElement:
+            if elt.tag != "{http://www.w3.org/2000/svg}svg":
+                modelXbrl.error(f"{guidance}.imageFileCannotBeLoaded",
+                                _("Image SVG has root element which is not svg"),
+                                modelObject=imgElt)
+            rootElement = False
+        eltTag = elt.tag.rpartition("}")[2] # strip namespace
+        if eltTag in ("object", "script", "audio", "foreignObject", "iframe", "image", "use", "video"):
+            href = elt.get("href","")
+            if eltTag in ("object", "script") or "javascript:" in href:
+                modelXbrl.error(f"{guidance}.executableCodePresent",
+                                _("Inline XBRL images MUST NOT contain executable code: %(element)s"),
+                                modelObject=imgElt, element=eltTag)
+            elif scheme(href) in ("http", "https", "ftp"):
+                modelXbrl.error(f"{guidance}.referencesPointingOutsideOfTheReportingPackagePresent",
+                                _("Inline XBRL instance document [image] MUST NOT contain any reference pointing to resources outside the reporting package: %(element)s"),
+                                modelObject=imgElt, element=eltTag)
+        if hasSvgEventAttributes(elt):
+            modelXbrl.error(f"{guidance}.executableCodePresent",
+                            _("Inline XBRL images MUST NOT contain executable code: %(element)s"),
+                            modelObject=imgElt, element=eltTag)
 
 def resourcesFilePath(modelManager: ModelManager, fileName: str) -> str:
     # resourcesDir can be in cache dir (production) or in validate/EFM/resources (for development)
     _resourcesDir = os.path.join( os.path.dirname(__file__), "resources") # dev/testing location
 
     if not os.path.isabs(_resourcesDir):
         _resourcesDir = os.path.abspath(_resourcesDir)
@@ -118,7 +137,18 @@
     return os.path.join(_resourcesDir, fileName)
 
 def loadAuthorityValidations(modelXbrl: ModelXbrl) -> list[Any] | dict[Any, Any]:
     _file = openFileStream(modelXbrl.modelManager.cntlr, resourcesFilePath(modelXbrl.modelManager, "authority-validations.json"), 'rt', encoding='utf-8')
     validations = json.load(_file) # {localName: date, ...}
     _file.close()
     return cast(Union[Dict[Any, Any], List[Any]], validations)
+
+def hasEventHandlerAttributes(elt: Any) -> bool:
+    return _hasEventAttributes(elt, htmlEventHandlerAttributes)
+
+def hasSvgEventAttributes(elt: Any) -> bool:
+    return _hasEventAttributes(elt, svgEventAttributes)
+
+def _hasEventAttributes(elt: Any, attributes: set[str]) -> bool:
+    if isinstance(elt, _Element):
+        return any(a in attributes for a in elt.keys())
+    return False
```

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 Client with curl:
 
    curl -X POST "-HContent-type: application/zip" -T TC1_valid.zip "http://localhost:8080/rest/xbrl/validation?disclosureSystem=esef&media=text"
 
 '''
 from __future__ import annotations
-import os, base64
+import os, base64, binascii
 import regex as re
 from collections import defaultdict
 from math import isnan
 from lxml.etree import _ElementTree, _Comment, _ProcessingInstruction, EntityBase, _Element
 from arelle import LeiUtil, ModelDocument, XbrlConst, XhtmlValidate
 from arelle.FunctionIxt import ixtNamespaces
 from arelle.ModelDtsObject import ModelResource
@@ -63,15 +63,15 @@
                               qnLinkLoc, qnLinkFootnoteArc, qnLinkFootnote, qnIXbrl11Footnote, iso17442)
 from arelle.XmlValidate import VALID
 from arelle.ValidateUtr import ValidateUtr
 from .Const import (mandatory, untransformableTypes,
                     esefPrimaryStatementPlaceholderNames, esefStatementsOfMonetaryDeclarationNames, esefMandatoryElementNames2020)
 from .Dimensions import checkFilingDimensions
 from .DTS import checkFilingDTS
-from .Util import isExtension, checkImageContents, loadAuthorityValidations
+from .Util import isExtension, checkImageContents, loadAuthorityValidations, hasEventHandlerAttributes
 from arelle.typing import TypeGetText
 from arelle.ModelObject import ModelObject
 from arelle.DisclosureSystem import DisclosureSystem
 from arelle.ModelDtsObject import ModelConcept
 from arelle.ModelXbrl import ModelXbrl
 from arelle.ValidateXbrl import ValidateXbrl
 from arelle.formula.XPathContext import XPathContext
@@ -250,15 +250,15 @@
         if not _ifrsNses:
             modelXbrl.warning("ESEF.RTS.ifrsRequired",
                             _("RTS on ESEF requires IFRS taxonomy."),
                             modelObject=modelXbrl)
             return
         if len(_ifrsNses) > 1:
             modelXbrl.error("Arelle.ESEF.multipleIfrsTaxonomies",
-                            _("Multuple IFRS taxonomies were imported %(ifrsNamespaces)s."),
+                            _("Multiple IFRS taxonomies were imported %(ifrsNamespaces)s."),
                             modelObject=modelXbrl, ifrsNamespaces=", ".join(_ifrsNses))
         if _ifrsNses:
             _ifrsNs = _ifrsNses[0]
 
     esefPrimaryStatementPlaceholders = set(qname(_ifrsNs, n) for n in esefPrimaryStatementPlaceholderNames)
     esefStatementsOfMonetaryDeclaration = set(qname(_ifrsNs, n) for n in esefStatementsOfMonetaryDeclarationNames)
     esefMandatoryElements2020 = set(qname(_ifrsNs, n) for n in esefMandatoryElementNames2020)
@@ -359,21 +359,21 @@
                             if len(docDirPath) >= i + 2 and packageName in (docDirPath[i+1],"POSTupload") and docDirPath[i+2] == "reports":
                                 ixdsDocDirs.add("/".join(docDirPath[i+3:-1]))
                                 reportCorrectlyPlacedInPackage = True
                             else:
                                 ixdsDocDirs.add("/".join(docDirPath[i+1:len(docDirPath)-1])) # needed for error msg on orphaned instance docs
                     if not reportIsInZipFile:
                         modelXbrl.error("ESEF.2.6.1.reportIncorrectlyPlacedInPackage",
-                            _("Inline XBRL document MUST be included within an ESEF report package as defined in"
+                            _("Inline XBRL document MUST be included within an ESEF report package as defined in "
                                "http://www.xbrl.org/WGN/report-packages/WGN-2018-08-14/report-packages-WGN-2018-08-14"
                                ".html: %(fileName)s (Document is not in a zip archive)"),
                             modelObject=doc, fileName=doc.basename)
                     elif not reportCorrectlyPlacedInPackage:
                         modelXbrl.error("ESEF.2.6.1.reportIncorrectlyPlacedInPackage",
-                             _("Inline XBRL document MUST be included within an ESEF report package as defined in"
+                             _("Inline XBRL document MUST be included within an ESEF report package as defined in "
                                "http://www.xbrl.org/WGN/report-packages/WGN-2018-08-14/report-packages-WGN-2018-08-14"
                                ".html: %(fileName)s (Document file not in correct place in package)"),
                             modelObject=doc, fileName=doc.basename)
                 else: # non-consolidated
                     if docTypeMatch:
                         if not docTypeMatch.group(1) or docTypeMatch.group(1).lower() == "html":
                             modelXbrl.error("ESEF.RTS.Art.3.htmlDoctype",
@@ -391,15 +391,15 @@
         if modelDocument.type in (ModelDocument.Type.INLINEXBRL, ModelDocument.Type.INLINEXBRLDOCUMENTSET, ModelDocument.Type.UnknownXML):
             hiddenEltIds = {}
             presentedHiddenEltIds = defaultdict(list)
             eligibleForTransformHiddenFacts = []
             requiredToDisplayFacts = []
             requiredToDisplayFactIds: dict[Any, Any] = {}
             firstIxdsDoc = True
-
+            contentOtherThanXHTMLGuidance = 'ESEF.2.5.1' if val.consolidated else 'ESEF.4.1.3'  # Different reference for iXBRL and stand-alone XHTML
             # ModelDocument.load has None as a return type. For typing reasons, we need to guard against that here.
             assert modelXbrl.modelDocument is not None
             for ixdsHtmlRootElt in (modelXbrl.ixdsHtmlElements if val.consolidated else # ix root elements for all ix docs in IXDS
                                     (modelXbrl.modelDocument.xmlRootElement,)): # plain xhtml filing
                 ixNStag = getattr(ixdsHtmlRootElt.modelDocument, "ixNStag", ixbrl11)
                 ixTags = set(ixNStag + ln for ln in ("nonNumeric", "nonFraction", "references", "relationship"))
                 ixTupleTag = ixNStag + "tuple"
@@ -418,16 +418,17 @@
                             if firstIxdsDoc and (not reportXmlLang or depth < firstRootmostXmlLangDepth):
                                 xmlLang = elt.get("{http://www.w3.org/XML/1998/namespace}lang")
                                 if xmlLang:
                                     reportXmlLang = xmlLang
                                     firstRootmostXmlLangDepth = depth
                         if ((eltTag in ("object", "script")) or
                             (eltTag == "a" and "javascript:" in elt.get("href","")) or
-                            (eltTag == "img" and "javascript:" in elt.get("src",""))):
-                            modelXbrl.error("ESEF.2.5.1.executableCodePresent",
+                            (eltTag == "img" and "javascript:" in elt.get("src","")) or
+                            (hasEventHandlerAttributes(elt))):
+                            modelXbrl.error(f"{contentOtherThanXHTMLGuidance}.executableCodePresent",
                                 _("Inline XBRL documents MUST NOT contain executable code: %(element)s"),
                                 modelObject=elt, element=eltTag)
                         elif eltTag == "img":
                             src = elt.get("src","").strip()
                             if scheme(src) in ("http", "https", "ftp"):
                                 modelXbrl.error("ESEF.4.1.6.xHTMLDocumentContainsExternalReferences" if val.unconsolidated
                                                 else "ESEF.3.5.1.inlineXbrlDocumentContainsExternalReferences",
@@ -441,47 +442,47 @@
                                     normalizedUri = elt.modelXbrl.modelManager.cntlr.webCache.normalizeUrl(src, base)
                                     if not elt.modelXbrl.fileSource.isInArchive(normalizedUri):
                                         normalizedUri = elt.modelXbrl.modelManager.cntlr.webCache.getfilename(normalizedUri)
                                     imglen = 0
                                     with elt.modelXbrl.fileSource.file(normalizedUri,binary=True)[0] as fh:
                                         imgContents = fh.read()
                                         imglen += len(imgContents)
-                                        checkImageContents(modelXbrl, elt, os.path.splitext(src)[1], True, imgContents)
+                                        checkImageContents(modelXbrl, elt, os.path.splitext(src)[1], True, imgContents, val.consolidated)
                                         imgContents = None # deref, may be very large
                                     #if imglen < browserMaxBase64ImageLength:
                                     #    modelXbrl.error("ESEF.2.5.1.imageIncludedAndNotEmbeddedAsBase64EncodedString",
                                     #        _("Images MUST be included in the XHTML document as a base64 encoded string unless their size exceeds support of browsers (%(maxImageSize)s): %(file)s."),
                                     #        modelObject=elt, maxImageSize=browserMaxBase64ImageLength, file=os.path.basename(normalizedUri))
                                 except IOError as err:
-                                    modelXbrl.error("ESEF.2.5.1.imageFileCannotBeLoaded",
+                                    modelXbrl.error(f"{contentOtherThanXHTMLGuidance}.imageFileCannotBeLoaded",
                                         _("Image file which isn't openable '%(src)s', error: %(error)s"),
                                         modelObject=elt, src=src, error=err)
                             else:
                                 m = imgDataMediaBase64Pattern.match(src)
                                 if not m or not m.group(2):
-                                    modelXbrl.warning("ESEF.2.5.1.embeddedImageNotUsingBase64Encoding",
+                                    modelXbrl.warning(f"{contentOtherThanXHTMLGuidance}.embeddedImageNotUsingBase64Encoding",
                                         _("Images included in the XHTML document SHOULD be base64 encoded: %(src)s."),
                                         modelObject=elt, src=src[:128])
                                     if m and m.group(1) and m.group(3):
-                                        checkImageContents(modelXbrl, elt, m.group(1), False, m.group(3))
+                                        checkImageContents(modelXbrl, elt, m.group(1), False, m.group(3), val.consolidated)
                                 else:
                                     if not m.group(1):
-                                        modelXbrl.error("ESEF.2.5.1.MIMETypeNotSpecified",
+                                        modelXbrl.error(f"{contentOtherThanXHTMLGuidance}.MIMETypeNotSpecified",
                                             _("Images included in the XHTML document MUST be saved with MIME type specifying PNG, GIF, SVG or JPG/JPEG formats: %(src)s."),
                                             modelObject=elt, src=src[:128])
                                     elif m.group(1) not in ("/gif", "/jpeg", "/jpg", "/png", "/svg+xml"):
-                                        modelXbrl.error("ESEF.2.5.1.imageFormatNotSupported",
+                                        modelXbrl.error(f"{contentOtherThanXHTMLGuidance}.imageFormatNotSupported",
                                             _("Images included in the XHTML document MUST be saved in PNG, GIF, SVG or JPG/JPEG formats: %(src)s."),
                                             modelObject=elt, src=src[:128])
                                     # check for malicious image contents
                                     try: # allow embedded newlines
-                                        checkImageContents(modelXbrl, elt, m.group(1), False, decodeBase64DataImage(m.group(3)))
+                                        checkImageContents(modelXbrl, elt, m.group(1), False, decodeBase64DataImage(m.group(3)), val.consolidated)
                                         imgContents = None # deref, may be very large
-                                    except base64.binascii.Error as err:
-                                        modelXbrl.error("ESEF.2.5.1.embeddedImageNotUsingBase64Encoding",
+                                    except binascii.Error as err:
+                                        modelXbrl.error(f"{contentOtherThanXHTMLGuidance}.embeddedImageNotUsingBase64Encoding",
                                             _("Base64 encoding error %(err)s in image source: %(src)s."),
                                             modelObject=elt, err=str(err), src=src[:128])
                         # links to external documents are allowed as of 2021 per G.2.5.1
                         #    Since ESEF is a format requirement and is not expected to impact the 'human readable layer' of a report,
                         #    this guidance should not be seen as limiting the inclusion of links to external websites, to other documents
                         #    or to other sections of the annual financial report.'''
                         #elif eltTag == "a":
@@ -562,16 +563,16 @@
                 # maliciously hidden facts
                 for cssHiddenElt in ixdsHtmlRootElt.getroottree().iterfind("//{http://www.w3.org/1999/xhtml}*[@style]"):
                     if styleCssHiddenPattern.match(cssHiddenElt.get("style","")):
                         for tag in (ixNStag + "nonNumeric", ixNStag+"nonFraction"):
                             for ixElt in cssHiddenElt.iterdescendants(tag=tag):
                                 if ixElt not in ixHiddenFacts:
                                     modelXbrl.error("ESEF.2.5.4.displayNoneUsedToHideTaggedFacts",
-                                        _("\"display:none\" style applies to a fact that is not in an ix:hidden section."),
-                                        modelObject=ixElt)
+                                        _('CSS MUST not be used to hide tagged facts, e.g. by applying display:none style. Concept "%(concept)s", value: %(value)s - line %(sourceline)s'),
+                                        modelObject=ixElt, concept=ixElt.concept.label(), sourceline=ixElt.sourceline, value=ixElt.effectiveValue)
                 del ixHiddenFacts
 
                 firstIxdsDoc = False
 
             if val.unconsolidated:
                 modelXbrl.modelManager.showStatus(None)
                 return # no more checks apply
@@ -585,16 +586,16 @@
             for ixdsHtmlRootElt in modelXbrl.ixdsHtmlElements:
                 for ixElt in ixdsHtmlRootElt.getroottree().iterfind("//{http://www.w3.org/1999/xhtml}*[@style]"):
                     hiddenFactRefMatch = styleIxHiddenPattern.match(ixElt.get("style",""))
                     if hiddenFactRefMatch:
                         hiddenFactRef = hiddenFactRefMatch.group(2)
                         if hiddenFactRef not in hiddenEltIds:
                             modelXbrl.error("ESEF.2.4.1.esefIxHiddenStyleNotLinkingFactInHiddenSection",
-                                _("\"-esef-ix-hidden\" style identifies @id, %(id)s of a fact that is not in ix:hidden section."),
-                                modelObject=ixElt, id=hiddenFactRef)
+                                _("\"-esef-ix-hidden\" style identifies id attribute of a fact that is not in ix:hidden section: %(factId)s"),
+                                modelObject=ixElt, factId=hiddenFactRef)
                         else:
                             presentedHiddenEltIds[hiddenFactRef].append(ixElt)
             for hiddenEltId, ixElt in hiddenEltIds.items():
                 if (hiddenEltId not in presentedHiddenEltIds and
                     getattr(ixElt, "xValid", 0) >= VALID and # may not be validated
                     (ixElt.concept.baseXsdType in untransformableTypes or ixElt.isNil)):
                     requiredToDisplayFacts.append(ixElt)
@@ -806,15 +807,15 @@
                         if a > aMax: aMax = a
                         if b < bMin: bMin = b
                     if not _inConsistent:
                         _inConsistent = (bMin < aMax)
                     decVals.clear()
                 if _inConsistent:
                     modelXbrl.error(("ESEF.2.2.4.inconsistentDuplicateNumericFactInInlineXbrlDocument"),
-                        "Inconsistent duplicate numeric facts MUST NOT appear in the content of an inline XBRL document. %(fact)s that was used more than once in contexts equivalent to %(contextID)s: values %(values)s.  ",
+                        _("Inconsistent duplicate numeric facts MUST NOT appear in the content of an inline XBRL document. %(fact)s that was used more than once in contexts equivalent to %(contextID)s: values %(values)s."),
                         modelObject=fList, fact=f0.qname, contextID=f0.contextID, values=", ".join(strTruncate(f.value, 128) for f in fList))
 
         if precisionFacts:
             modelXbrl.error("ESEF.2.2.1.precisionAttributeUsed",
                             _("The accuracy of numeric facts MUST be defined with the 'decimals' attribute rather than the 'precision' attribute: %(elements)s."),
                             modelObject=precisionFacts, elements=", ".join(sorted(str(e.qname) for e in precisionFacts)))
 
@@ -828,16 +829,16 @@
             modelXbrl.error("ESEF.2.2.3.incorrectTransformationRuleApplied",
                               _("ESMA recommends applying the Transformation Rules Registry 4, as published by XBRL International or any more recent versions of the Transformation Rules Registry provided with a 'Recommendation' status, for these elements: %(elements)s."),
                               modelObject=transformRegistryErrors,
                               elements=", ".join(sorted(str(fact.qname) for fact in transformRegistryErrors)))
 
         if orphanedFootnotes:
             modelXbrl.warning("ESEF.2.3.1.unusedFootnote",
-                _("Every nonempty link:footnote element SHOULD be linked to at least one fact."),
-                modelObject=orphanedFootnotes)
+                _("Every nonempty link:footnote element SHOULD be linked to at least one fact. Unused footnote ids: %(ids)s"),
+                modelObject=orphanedFootnotes, ids=', '.join([f'"{footnote.id}"' for footnote in orphanedFootnotes]))
 
         # this test removed from Filer Manual July 2020
         #if noLangFootnotes:
         #    modelXbrl.error("ESEF.2.3.1.undefinedLanguageForFootnote",
         #        _("Each footnote MUST have the 'xml:lang' attribute whose value corresponds to the language of the text in the content of the respective footnote."),
         #        modelObject=noLangFootnotes)
         ftLangNotUsedByTextFacts = set()
@@ -887,25 +888,25 @@
             if e in val.extensionImportedUrls:
                 val.modelXbrl.error("ESEF.3.1.2.incorrectEsefTaxonomyVersionUsed",
                      _("The issuer's extension taxonomies MUST import the applicable version of the taxonomy files prepared by ESMA. Outdated entry point: %(url)s"),
                     modelObject=modelDocument, url=e)
                 hasOutdatedUrl = True
 
         if ("authorityRequiredTaxonomyURLs" in val.authParam and
-            not any(e in val.extensionImportedUrls for e in val.authParam["authorityRequiredTaxonomyURLs"])):
+                not any(e in val.extensionImportedUrls for e in val.authParam["authorityRequiredTaxonomyURLs"])):
             val.modelXbrl.error(
                 "UKFRC22.3.requiredFrcEntryPointNotImported",
-                 _("The issuer's extension taxonomies MUST import the FRC entry point of the taxonomy files prepared by %(authority)s."),
+                _("The issuer's extension taxonomies MUST import the FRC entry point of the taxonomy files prepared by %(authority)s."),
                 modelObject=modelDocument, authority=val.authParam["authorityName"])
 
         if not hasOutdatedUrl and not any(e in val.extensionImportedUrls for e in val.authParam["effectiveTaxonomyURLs"]):
             val.modelXbrl.error(
                 "UKFRC22.1.requiredUksefEntryPointNotImported" if val.authority == "UKFRC" else
                 "ESEF.3.1.2.requiredEntryPointNotImported",
-                 _("The issuer's extension taxonomies MUST import the entry point of the taxonomy files prepared by %(authority)s."),
+                _("The issuer's extension taxonomies MUST import the entry point of the taxonomy files prepared by %(authority)s."),
                 modelObject=modelDocument, authority=val.authParam["authorityName"])
 
 
         # unused elements in linkbases
         unreportedLbElts = set()
         for arcroles, error, checkRoots, lbType in (
                     ((parentChild,), "elements{}UsedForTagging{}AppliedInPresentationLinkbase", True, "presentation"),
@@ -1118,15 +1119,15 @@
 
 def validateFormulaCompiled(modelXbrl: ModelXbrl, xpathContext: XPathContext) -> None:
     # request unsatisfied assertions without a message to print a trace
     # this is not conditional on validateESEFplugin so the flag is set even if DisclosureSystemChecks not requested upon compiling but set later in workflow
     xpathContext.formulaOptions.traceUnmessagedUnsatisfiedAssertions = True
 
 def validateFormulaFinished(val: ValidateXbrl, *args: Any, **kwargs: Any) -> None: # runs *after* formula (which is different for test suite from other operation
-    if not (val.validateESEFplugin):
+    if not getattr(val, 'validateESEFplugin', False):
         return
 
     modelXbrl = val.modelXbrl
     if hasattr(val, 'priorFormulaOptionsRunIDs'):  # reset environment formula run IDs if they were saved
         modelXbrl.modelManager.formulaOptions.runIDs = val.priorFormulaOptionsRunIDs
     sumWrnMsgs = sumErrMsgs = 0
     for e in modelXbrl.errors:
```

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF/config.xml` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF/resources/authority-validations.json` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF/resources/authority-validations.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/Const.py` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF/Const.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 '''
-Version 2022 created on September 19, 2022
-
-Filer Guidelines: https://www.esma.europa.eu/sites/default/files/library/esma32-60-254_esef_reporting_manual.pdf
+Filer Guidelines: esma32-60-254_esef_reporting_manual.pdf
 
 See COPYRIGHT.md for copyright information.
 '''
 from __future__ import annotations
 import regex as re
+from typing import Any, Callable
 from arelle.ModelValue import QName, qname
 from arelle.XbrlConst import all, notAll, hypercubeDimension, dimensionDomain, domainMember, dimensionDefault, widerNarrower
 
 browserMaxBase64ImageLength = 5242880 # 5MB
 
 esefTaxonomyNamespaceURIs = {
     "http://xbrl.ifrs.org/taxonomy/20",
-    "https://xbrl.ifrs.org/taxonomy/20",
+    "http://xbrl.ifrs.org/taxonomy/20",
     }
 
 disallowedURIsPattern = re.compile(
     "http://xbrl.ifrs.org/taxonomy/[0-9-]{10}/full_ifrs/full_ifrs-cor_[0-9-]{10}[.]xsd|"
     "http://www.esma.europa.eu/taxonomy/[0-9-]{10}/esef_all.xsd"
     )
 
-esefCorNsPattern = re.compile(r"https?://www\.esma\.europa\.eu/taxonomy/[0-9-]{10}/esef_cor")
 
-DefaultDimensionLinkroles = ("https://www.esma.europa.eu/xbrl/role/cor/ifrs-dim_role-990000", # preferred, new spec
-                             "http://www.esma.europa.eu/xbrl/role/cor/ifrs-dim_role-990000")
-LineItemsNotQualifiedLinkroles = ("https://www.esma.europa.eu/xbrl/role/cor/esef_role-999999", # preferred, new spec
-                                  "http://www.esma.europa.eu/xbrl/role/cor/esef_role-999999")
+DefaultDimensionLinkroles = ("http://www.esma.europa.eu/xbrl/role/cor/ifrs-dim_role-990000",)
+LineItemsNotQualifiedLinkrole = "http://www.esma.europa.eu/xbrl/role/cor/esef_role-999999"
 
 qnDomainItemTypes = {qname("{http://www.xbrl.org/dtr/type/non-numeric}nonnum:domainItemType"),
                      qname("{http://www.xbrl.org/dtr/type/2020-01-21}nonnum:domainItemType")}
 
 
 linkbaseRefTypes = {
     "http://www.xbrl.org/2003/role/calculationLinkbaseRef": "cal",
@@ -83,18 +79,14 @@
     # from Annex II para 1
     "StatementOfFinancialPositionAbstract",
     "StatementOfProfitOrLossAndOtherComprehensiveIncomeAbstract"
     "StatementOfChangesInEquityAbstract",
     "StatementOfCashFlowsAbstract",
     }
 
-esefNotesStatementConcepts = {
-    "NotesAccountingPoliciesAndMandatoryTags",
-}
-
 esefMandatoryElementNames2020 = (
     "NameOfReportingEntityOrOtherMeansOfIdentification",
     "ExplanationOfChangeInNameOfReportingEntityOrOtherMeansOfIdentificationFromEndOfPrecedingReportingPeriod",
     "DomicileOfEntity",
     "LegalFormOfEntity",
     "CountryOfIncorporation",
     "AddressOfRegisteredOfficeOfEntity",
@@ -345,7 +337,163 @@
     "LengthOfLifeOfLimitedLifeEntity",
     "NameOfParentEntity",
     "NameOfReportingEntityOrOtherMeansOfIdentification",
     "NameOfUltimateParentOfGroup",
     "PrincipalPlaceOfBusiness",
     "StatementOfIFRSCompliance",
 )
+
+htmlEventHandlerAttributes = set((
+    "onabort",
+    "onafterprint",
+    "onbeforeprint",
+    "onbeforeunload",
+    "onblur",
+    "oncanplay",
+    "oncanplaythrough",
+    "onchange",
+    "onclick",
+    "oncontextmenu",
+    "oncopy",
+    "oncuechange",
+    "oncut",
+    "ondblclick",
+    "ondrag",
+    "ondragend",
+    "ondragenter",
+    "ondragleave",
+    "ondragover",
+    "ondragstart",
+    "ondrop",
+    "ondurationchange",
+    "onemptied",
+    "onended",
+    "onerror",
+    "onfocus",
+    "onhashchange",
+    "oninput",
+    "oninvalid",
+    "onkeydown",
+    "onkeypress",
+    "onkeyup",
+    "onload",
+    "onloadeddata",
+    "onloadedmetadata",
+    "onloadstart",
+    "onmessage",
+    "onmousedown",
+    "onmousemove",
+    "onmouseout",
+    "onmouseover",
+    "onmouseup",
+    "onmousewheel",
+    "onoffline",
+    "ononline",
+    "onpagehide",
+    "onpageshow",
+    "onpaste",
+    "onpause",
+    "onplay",
+    "onplaying",
+    "onpopstate",
+    "onprogress",
+    "onratechange",
+    "onreset",
+    "onresize",
+    "onscroll",
+    "onsearch",
+    "onseeked",
+    "onseeking",
+    "onselect",
+    "onstalled",
+    "onstorage",
+    "onsubmit",
+    "onsuspend",
+    "ontimeupdate",
+    "ontoggle",
+    "onunload",
+    "onvolumechange",
+    "onwaiting",
+    "onwheel",
+))
+
+svgEventAttributes = set((
+    "onabort",
+    "onactivate",
+    "onafterprint",
+    "onbeforeprint",
+    "onbegin",
+    "oncancel",
+    "oncanplay",
+    "oncanplaythrough",
+    "onchange",
+    "onclick",
+    "onclose",
+    "oncopy",
+    "oncuechange",
+    "oncut",
+    "ondblclick",
+    "ondrag",
+    "ondragend",
+    "ondragenter",
+    "ondragexit",
+    "ondragleave",
+    "ondragover",
+    "ondragstart",
+    "ondrop",
+    "ondurationchange",
+    "onemptied",
+    "onend",
+    "onended",
+    "onerror",
+    "onfocus",
+    "onfocusin",
+    "onfocusout",
+    "onhashchange",
+    "oninput",
+    "oninvalid",
+    "onkeydown",
+    "onkeypress",
+    "onkeyup",
+    "onload",
+    "onloadeddata",
+    "onloadedmetadata",
+    "onloadstart",
+    "onmessage",
+    "onmousedown",
+    "onmouseenter",
+    "onmouseleave",
+    "onmousemove",
+    "onmouseout",
+    "onmouseover",
+    "onmouseup",
+    "onmousewheel",
+    "onoffline",
+    "ononline",
+    "onpagehide",
+    "onpageshow",
+    "onpaste",
+    "onpause",
+    "onplay",
+    "onplaying",
+    "onpopstate",
+    "onprogress",
+    "onratechange",
+    "onrepeat",
+    "onreset",
+    "onresize",
+    "onscroll",
+    "onseeked",
+    "onseeking",
+    "onselect",
+    "onshow",
+    "onstalled",
+    "onstorage",
+    "onsubmit",
+    "onsuspend",
+    "ontimeupdate",
+    "ontoggle",
+    "onunload",
+    "onvolumechange",
+    "onwaiting",
+    "onzoom"
+))
```

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/DTS.py` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/DTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/Dimensions.py` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/Dimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,64 +38,66 @@
 
 Client with curl:
 
    curl -X POST "-HContent-type: application/zip" -T TC1_valid.zip "http://localhost:8080/rest/xbrl/validation?disclosureSystem=esef&media=text"
 
 '''
 from __future__ import annotations
-import os, base64
+import os
 import zipfile
 import regex as re
 from collections import defaultdict
 from math import isnan
-from lxml.etree import _ElementTree, _Comment, _ProcessingInstruction, EntityBase, _Element
-from urllib.parse import unquote
+from lxml.etree import _ElementTree, _Comment, _ProcessingInstruction, EntityBase, parse, XMLSyntaxError, _Element, XMLParser
+import tinycss2  # type: ignore[import]
 from arelle import LeiUtil, ModelDocument, XbrlConst, XhtmlValidate
+from arelle.FileSource import FileSource
 from arelle.FunctionIxt import ixtNamespaces
 from arelle.ModelDtsObject import ModelResource
 from arelle.ModelInstanceObject import ModelFact, ModelInlineFact
 from arelle.ModelValue import qname
 from arelle.PackageManager import validateTaxonomyPackage
-from arelle.PythonUtil import strTruncate, normalizeSpace
+from arelle.PythonUtil import normalizeSpace
 from arelle.Version import authorLabel, copyrightLabel
+from arelle.PythonUtil import strTruncate
 from arelle.UrlUtil import decodeBase64DataImage, isHttpUrl, scheme
 from arelle.XmlValidate import lexicalPatterns
 
 from arelle.ValidateXbrlCalcs import inferredDecimals, rangeValue
 from arelle.XbrlConst import (ixbrl11, xhtml, parentChild, summationItem, standardLabel,
                               all as hc_all, notAll as hc_notAll, dimensionDomain, domainMember,
                               qnLinkLoc, qnLinkFootnoteArc, qnLinkFootnote, qnIXbrl11Footnote, iso17442, widerNarrower)
 from arelle.XmlValidate import VALID
 from arelle.ValidateUtr import ValidateUtr
 from .Const import (mandatory, untransformableTypes,
                     esefPrimaryStatementPlaceholderNames, esefStatementsOfMonetaryDeclarationNames, esefMandatoryElementNames2020)
 from .Dimensions import checkFilingDimensions
 from .DTS import checkFilingDTS
-from .Util import isExtension, checkImageContents, loadAuthorityValidations, checkForMultiLangDuplicates, getEsefNotesStatementConcepts
+from .Util import isExtension, loadAuthorityValidations, checkForMultiLangDuplicates,\
+    getEsefNotesStatementConcepts, hasEventHandlerAttributes, validateImage, checkSVGContentElt
 from arelle.typing import TypeGetText
 from arelle.ModelObject import ModelObject
 from arelle.DisclosureSystem import DisclosureSystem
 from arelle.ModelDtsObject import ModelConcept
 from arelle.ModelXbrl import ModelXbrl
 from arelle.ValidateXbrl import ValidateXbrl
 from arelle.formula.XPathContext import XPathContext
 from arelle.ModelRelationshipSet import ModelRelationshipSet
 from arelle.ModelInstanceObject import ModelInlineFootnote
 from arelle.ModelInstanceObject import ModelContext
-from typing import Any, Dict, cast
+from typing import Any, Dict, cast, List
 from collections.abc import Generator
 from arelle.ModelValue import QName
 
 _: TypeGetText  # Handle gettext
 
 styleIxHiddenPattern = re.compile(r"(.*[^\w]|^)-esef-ix-hidden\s*:\s*([\w.-]+).*")
 styleCssHiddenPattern = re.compile(r"(.*[^\w]|^)display\s*:\s*none([^\w].*|$)")
 ifrsNsPattern = re.compile(r"https?://xbrl.ifrs.org/taxonomy/[0-9-]{10}/ifrs-full")
 datetimePattern = lexicalPatterns["XBRLI_DATEUNION"]
-imgDataMediaBase64Pattern = re.compile(r"data:image([^,;]*)(;base64)?,(.*)$", re.S)
 ixErrorPattern = re.compile(r"ix11[.]|xmlSchema[:]|(?!xbrl.5.2.5.2|xbrl.5.2.6.2)xbrl[.]|xbrld[ti]e[:]|utre[:]")
 docTypeXhtmlPattern = re.compile(r"^<!(?:DOCTYPE\s+)\s*html(?:PUBLIC\s+)?(?:.*-//W3C//DTD\s+(X?HTML)\s)?.*>$", re.IGNORECASE)
 
 FOOTNOTE_LINK_CHILDREN = {qnLinkLoc, qnLinkFootnoteArc, qnLinkFootnote, qnIXbrl11Footnote}
 PERCENT_TYPE = qname("{http://www.xbrl.org/dtr/type/numeric}num:percentItemType")
 IXT_NAMESPACES = {ixtNamespaces["ixt v4"], # only tr4 or newer REC is currently recommended
                   ixtNamespaces["ixt v5"]}
@@ -113,15 +115,15 @@
 def disclosureSystemConfigURL(disclosureSystem: DisclosureSystem, *args: Any, **kwargs: Any) -> str:
     return os.path.join(os.path.dirname(__file__), "config.xml")
 
 def modelXbrlBeforeLoading(modelXbrl: ModelXbrl, normalizedUri: str, filepath: str, isEntry: bool=False, **kwargs: Any) -> ModelDocument.LoadingException | None:
     if getattr(modelXbrl.modelManager.disclosureSystem, "ESEFplugin", False):
         if isEntry:
             if any("unconsolidated" in n for n in modelXbrl.modelManager.disclosureSystem.names):
-                if re.match(".*[.](7z|rar|tar)", normalizedUri):
+                if re.match(r'.*[.](7z|rar|tar|jar)', normalizedUri):
                     modelXbrl.error("ESEF.Arelle.InvalidSubmissionFormat",
                                     _("Unrecognized submission format."),
                                     modelObject=modelXbrl)
                     return ModelDocument.LoadingException("Invalid submission format")
             else:
                 if modelXbrl.fileSource.isArchive:
                     if (not isinstance(modelXbrl.fileSource.selection, list) and
@@ -163,14 +165,49 @@
                             _("RTS Annex III Par 3 and ESEF 3.1.3 requires an XBRL Report Package but one could not be loaded."),
                             modelObject=modelXbrl)
         if (modelXbrl.modelDocument is None or
             not modelXbrl.facts and "ESEF.RTS.Art.6.a.noInlineXbrlTags" not in modelXbrl.errors):
             modelXbrl.error("ESEF.RTS.Art.6.a.noInlineXbrlTags",
                             _("RTS on ESEF requires inline XBRL, no facts were reported."),
                             modelObject=modelXbrl)
+        if modelXbrl.fileSource.isArchive:
+            if modelXbrl.fileSource.dir is not None:
+                for filename in modelXbrl.fileSource.dir:
+                    validateEntity(modelXbrl, filename, modelXbrl.fileSource)
+        else:
+            if isinstance(modelXbrl.fileSource.url, str):
+                validateEntity(modelXbrl, modelXbrl.fileSource.url, modelXbrl.fileSource)
+            elif isinstance(modelXbrl.fileSource.url, list):
+                for filename in modelXbrl.fileSource.url:
+                    validateEntity(modelXbrl, filename, modelXbrl.fileSource)
+            if modelXbrl.modelDocument:
+                # search for the zip of the taxonomy extension
+                entrypointDocs = [referencedDoc for referencedDoc in modelXbrl.modelDocument.referencesDocument.keys() if referencedDoc.type == ModelDocument.Type.SCHEMA]
+                for entrypointDoc in entrypointDocs: # usually only one
+                    for filesource in modelXbrl.fileSource.referencedFileSources.values():
+                        if filesource.exists(entrypointDoc.filepath) and filesource.dir is not None:
+                            for filename in filesource.dir:
+                                validateEntity(modelXbrl, filename, filesource)
+
+def validateEntity(modelXbrl: ModelXbrl, filename:str, filesource: FileSource) -> None:
+    consolidated = not any("unconsolidated" in n for n in modelXbrl.modelManager.disclosureSystem.names)
+    contentOtherThanXHTMLGuidance = 'ESEF.2.5.1' if consolidated else 'ESEF.4.1.3'
+    fullname = filesource.basedUrl(filename)
+    file = filesource.file(fullname)
+    try:
+        parser = XMLParser(load_dtd=True, resolve_entities=False)
+        root = parse(file[0], parser=parser)
+        if root.docinfo.internalDTD:
+            for entity in root.docinfo.internalDTD.iterentities():  # type: ignore[attr-defined]
+                modelXbrl.error(f"{contentOtherThanXHTMLGuidance}.maliciousCodePresent",
+                                _("Documents MUST NOT contain any malicious content. Dangerous XML entity found: %(element)s."),
+                                modelObject=filename, element=entity.name)
+    except (UnicodeDecodeError, XMLSyntaxError) as e:
+        # probably a image or a directory
+        pass
 
 def validateXbrlStart(val: ValidateXbrl, parameters: dict[Any, Any] | None=None, *args: Any, **kwargs: Any) -> None:
     val.validateESEFplugin = val.validateDisclosureSystem and getattr(val.disclosureSystem, "ESEFplugin", False)
     if not (val.validateESEFplugin):
         return
     modelXbrl = val.modelXbrl
     val.extensionImportedUrls = set()
@@ -186,14 +223,26 @@
     authorityValidations = loadAuthorityValidations(val.modelXbrl)
     # loadAuthorityValidations returns either a list or a dict but in this context, we expect a dict.
     # By using cast, we let mypy know that a list is _not_ expected here.
     authorityValidations = cast(Dict[Any, Any], authorityValidations)
 
     val.authParam = authorityValidations["default"]
     val.authParam.update(authorityValidations.get(val.authority, {}))
+    if parameters:
+        overwiteParams = {}
+        for key, value in parameters.items():
+            if str(key) in val.authParam and len(value) == 2 and value[1] not in ("null", "None", None):
+                if isinstance(val.authParam[str(key)], int):
+                    try:
+                        overwiteParams[str(key)] = int(value[1])
+                    except ValueError:
+                        modelXbrl.error("Invalid Parameter", _("%(key)s should be a int, got (value)"), key=key, value=value)
+                else:
+                    overwiteParams[str(key)] = value[1]
+        val.authParam.update(overwiteParams)
     for convertListIntoSet in ("outdatedTaxonomyURLs", "effectiveTaxonomyURLs", "standardTaxonomyURIs", "additionalMandatoryTags"):
         if convertListIntoSet in val.authParam:
             val.authParam[convertListIntoSet] = set(val.authParam[convertListIntoSet])
 
     # add in formula messages if not loaded
     formulaMsgsUrls = val.authParam.get("formulaMessagesAdditionalURLs", ())
     _reCacheRelationships = False
@@ -267,15 +316,15 @@
         if not _ifrsNses:
             modelXbrl.warning("ESEF.RTS.ifrsRequired",
                             _("RTS on ESEF requires IFRS taxonomy."),
                             modelObject=modelXbrl)
             return
         if len(_ifrsNses) > 1:
             modelXbrl.error("Arelle.ESEF.multipleIfrsTaxonomies",
-                            _("Multuple IFRS taxonomies were imported %(ifrsNamespaces)s."),
+                            _("Multiple IFRS taxonomies were imported %(ifrsNamespaces)s."),
                             modelObject=modelXbrl, ifrsNamespaces=", ".join(_ifrsNses))
         if _ifrsNses:
             _ifrsNs = _ifrsNses[0]
         esefNotesConcepts = getEsefNotesStatementConcepts(val.modelXbrl)
 
     esefPrimaryStatementPlaceholders = set(qname(_ifrsNs, n) for n in esefPrimaryStatementPlaceholderNames)
     esefStatementsOfMonetaryDeclaration = set(qname(_ifrsNs, n) for n in esefStatementsOfMonetaryDeclarationNames)
@@ -377,21 +426,21 @@
                             if len(docDirPath) >= i + 2 and packageName in (docDirPath[i+1],"POSTupload") and docDirPath[i+2] == "reports":
                                 ixdsDocDirs.add("/".join(docDirPath[i+3:-1]))
                                 reportCorrectlyPlacedInPackage = True
                             else:
                                 ixdsDocDirs.add("/".join(docDirPath[i+1:len(docDirPath)-1])) # needed for error msg on orphaned instance docs
                     if not reportIsInZipFile:
                         modelXbrl.error("ESEF.2.6.1.reportIncorrectlyPlacedInPackage",
-                            _("Inline XBRL document MUST be included within an ESEF report package as defined in"
+                            _("Inline XBRL document MUST be included within an ESEF report package as defined in "
                                "http://www.xbrl.org/WGN/report-packages/WGN-2018-08-14/report-packages-WGN-2018-08-14"
                                ".html: %(fileName)s (Document is not in a zip archive)"),
                             modelObject=doc, fileName=doc.basename)
                     elif not reportCorrectlyPlacedInPackage:
                         modelXbrl.error("ESEF.2.6.1.reportIncorrectlyPlacedInPackage",
-                             _("Inline XBRL document MUST be included within an ESEF report package as defined in"
+                             _("Inline XBRL document MUST be included within an ESEF report package as defined in "
                                "http://www.xbrl.org/WGN/report-packages/WGN-2018-08-14/report-packages-WGN-2018-08-14"
                                ".html: %(fileName)s (Document file not in correct place in package)"),
                             modelObject=doc, fileName=doc.basename)
                 else: # non-consolidated
                     if docTypeMatch:
                         if not docTypeMatch.group(1) or docTypeMatch.group(1).lower() == "html":
                             modelXbrl.error("ESEF.RTS.Art.3.htmlDoctype",
@@ -409,15 +458,15 @@
         if modelDocument.type in (ModelDocument.Type.INLINEXBRL, ModelDocument.Type.INLINEXBRLDOCUMENTSET, ModelDocument.Type.UnknownXML):
             hiddenEltIds = {}
             presentedHiddenEltIds = defaultdict(list)
             eligibleForTransformHiddenFacts = []
             requiredToDisplayFacts = []
             requiredToDisplayFactIds: dict[Any, Any] = {}
             firstIxdsDoc = True
-
+            contentOtherThanXHTMLGuidance = 'ESEF.2.5.1' if val.consolidated else 'ESEF.4.1.3'  # Different reference for iXBRL and stand-alone XHTML
             # ModelDocument.load has None as a return type. For typing reasons, we need to guard against that here.
             assert modelXbrl.modelDocument is not None
             for ixdsHtmlRootElt in (modelXbrl.ixdsHtmlElements if val.consolidated else # ix root elements for all ix docs in IXDS
                                     (modelXbrl.modelDocument.xmlRootElement,)): # plain xhtml filing
                 ixNStag = getattr(ixdsHtmlRootElt.modelDocument, "ixNStag", ixbrl11)
                 ixTags = set(ixNStag + ln for ln in ("nonNumeric", "nonFraction", "references", "relationship"))
                 ixTupleTag = ixNStag + "tuple"
@@ -438,72 +487,29 @@
                                 xmlLang = elt.get("{http://www.w3.org/XML/1998/namespace}lang")
                                 if xmlLang:
                                     reportXmlLang = xmlLang
                                     firstRootmostXmlLangDepth = depth
                         if ((eltTag in ("object", "script")) or
                             (eltTag == "a" and "javascript:" in elt.get("href", "")) or
                             (eltTag == "img" and "javascript:" in elt.get("src", "")) or
-                            (eltTag == "a" and "mailto" in elt.get("href", ""))):
-                            modelXbrl.error("ESEF.2.5.1.executableCodePresent",
+                            (hasEventHandlerAttributes(elt))):
+                            modelXbrl.error(f"{contentOtherThanXHTMLGuidance}.executableCodePresent",
                                 _("Inline XBRL documents MUST NOT contain executable code: %(element)s"),
                                 modelObject=elt, element=eltTag)
+                        elif eltTag == "a" and "mailto" in elt.get("href", ""):
+                            modelXbrl.warning(f"{contentOtherThanXHTMLGuidance}.executableCodePresent.mailto",
+                                            _("Inline XBRL documents SHOULD NOT contain any 'mailto' URI: %(element)s"),
+                                            modelObject=elt, element=eltTag)
+                        elif eltTag == "{http://www.w3.org/2000/svg}svg":
+                            checkSVGContentElt(elt, elt.modelDocument.baseForElement(elt), modelXbrl, elt,
+                                           contentOtherThanXHTMLGuidance, val)
                         elif eltTag == "img":
                             src = elt.get("src","").strip()
-                            if scheme(src) in ("http", "https", "ftp"):
-                                modelXbrl.error("ESEF.4.1.6.xHTMLDocumentContainsExternalReferences" if val.unconsolidated
-                                                else "ESEF.3.5.1.inlineXbrlDocumentContainsExternalReferences",
-                                    _("Inline XBRL instance documents MUST NOT contain any reference pointing to resources outside the reporting package: %(element)s"),
-                                    modelObject=elt, element=eltTag,
-                                    messageCodes=("ESEF.3.5.1.inlineXbrlDocumentContainsExternalReferences", "ESEF.4.1.6.xHTMLDocumentContainsExternalReferences"))
-                            elif not src.startswith("data:image"):
-                                # presume it to be an image file, check image contents
-                                try:
-                                    base = elt.modelDocument.baseForElement(elt)
-                                    normalizedUri = elt.modelXbrl.modelManager.cntlr.webCache.normalizeUrl(src, base)
-                                    if not elt.modelXbrl.fileSource.isInArchive(normalizedUri):
-                                        normalizedUri = elt.modelXbrl.modelManager.cntlr.webCache.getfilename(normalizedUri)
-                                    imglen = 0
-                                    with elt.modelXbrl.fileSource.file(normalizedUri,binary=True)[0] as fh:
-                                        imgContents = fh.read()
-                                        imglen += len(imgContents)
-                                        checkImageContents(modelXbrl, elt, os.path.splitext(src)[1], True, imgContents)
-                                        imgContents = None # deref, may be very large
-                                    #if imglen < browserMaxBase64ImageLength:
-                                    #    modelXbrl.error("ESEF.2.5.1.imageIncludedAndNotEmbeddedAsBase64EncodedString",
-                                    #        _("Images MUST be included in the XHTML document as a base64 encoded string unless their size exceeds support of browsers (%(maxImageSize)s): %(file)s."),
-                                    #        modelObject=elt, maxImageSize=browserMaxBase64ImageLength, file=os.path.basename(normalizedUri))
-                                except IOError as err:
-                                    modelXbrl.error("ESEF.2.5.1.imageFileCannotBeLoaded",
-                                        _("Image file which isn't openable '%(src)s', error: %(error)s"),
-                                        modelObject=elt, src=src, error=err)
-                            else:
-                                m = imgDataMediaBase64Pattern.match(src)
-                                if not m or not m.group(2):
-                                    modelXbrl.warning("ESEF.2.5.1.embeddedImageNotUsingBase64Encoding",
-                                        _("Images included in the XHTML document SHOULD be base64 encoded: %(src)s."),
-                                        modelObject=elt, src=src[:128])
-                                    if m and m.group(1) and m.group(3):
-                                        checkImageContents(modelXbrl, elt, m.group(1), False, unquote(m.group(3)))
-                                else:
-                                    if not m.group(1):
-                                        modelXbrl.error("ESEF.2.5.1.MIMETypeNotSpecified",
-                                            _("Images included in the XHTML document MUST be saved with MIME type specifying PNG, GIF, SVG or JPG/JPEG formats: %(src)s."),
-                                            modelObject=elt, src=src[:128])
-                                    elif m.group(1) not in ("/gif", "/jpeg", "/jpg", "/png", "/svg+xml"):
-                                        modelXbrl.error("ESEF.2.5.1.imageFormatNotSupported",
-                                            _("Images included in the XHTML document MUST be saved in PNG, GIF, SVG or JPG/JPEG formats: %(src)s."),
-                                            modelObject=elt, src=src[:128])
-                                    # check for malicious image contents
-                                    try: # allow embedded newlines
-                                        checkImageContents(modelXbrl, elt, m.group(1), False, decodeBase64DataImage(m.group(3)))
-                                        imgContents = None # deref, may be very large
-                                    except base64.binascii.Error as err:
-                                        modelXbrl.error("ESEF.2.5.1.embeddedImageNotUsingBase64Encoding",
-                                            _("Base64 encoding error %(err)s in image source: %(src)s."),
-                                            modelObject=elt, err=str(err), src=src[:128])
+                            evaluatedMsg = _('On line {line}, "alt" attribute value: "{alt}"').format(line=elt.sourceline, alt=elt.get("alt"))
+                            validateImage(elt.modelDocument.baseForElement(elt), src, modelXbrl, val, elt, evaluatedMsg, contentOtherThanXHTMLGuidance)
                         # links to external documents are allowed as of 2021 per G.2.5.1
                         #    Since ESEF is a format requirement and is not expected to impact the 'human readable layer' of a report,
                         #    this guidance should not be seen as limiting the inclusion of links to external websites, to other documents
                         #    or to other sections of the annual financial report.'''
                         #elif eltTag == "a":
                         #    href = elt.get("href","").strip()
                         #    if scheme(href) in ("http", "https", "ftp"):
@@ -512,39 +518,50 @@
                         #            _("Inline XBRL instance documents MUST NOT contain any reference pointing to resources outside the reporting package: %(element)s"),
                         #            modelObject=elt, element=eltTag,
                         #            messageCodes=("ESEF.3.5.1.inlineXbrlDocumentContainsExternalReferences", "ESEF.4.1.6.xHTMLDocumentContainsExternalReferences"))
                         elif eltTag == "base":
                             modelXbrl.error("ESEF.2.4.2.htmlOrXmlBaseUsed",
                                 _("The HTML <base> elements MUST NOT be used in the Inline XBRL document."),
                                 modelObject=elt, element=eltTag)
-                        elif eltTag == "link" and elt.get("type") == "text/css":
+                        elif eltTag == "link" and (elt.get("type") == "text/css" or (elt.get("rel") == "stylesheet" and not elt.get("type"))):
+                            #  type can be omitted https://www.w3schools.com/tags/att_link_type.asp
+
+                            base = elt.modelDocument.baseForElement(elt)
+                            normalizedUri = elt.modelXbrl.modelManager.cntlr.webCache.normalizeUrl(elt.get("href"), base)
+                            if not elt.modelXbrl.fileSource.isInArchive(normalizedUri):
+                                normalizedUri = elt.modelXbrl.modelManager.cntlr.webCache.getfilename(normalizedUri)
+
+                            with elt.modelXbrl.fileSource.file(normalizedUri, binary=True)[0] as fh:
+                                cssContents = fh.read()
+                                validateCssUrl(cssContents.decode(), normalizedUri, modelXbrl, val, elt, contentOtherThanXHTMLGuidance)
+                                cssContents = None
                             if val.unconsolidated:
                                 modelXbrl.warning("ESEF.4.1.4.externalCssFileForXhtmlDocument",
                                     _("For XHTML stand-alone documents, the CSS SHOULD be embedded within the document."),
                                     modelObject=elt, element=eltTag)
                             elif len(modelXbrl.ixdsHtmlElements) > 1:
                                 _file = elt.get("href")
                                 if not _file or isHttpUrl(_file) or os.path.isabs(_file):
                                     modelXbrl.warning("ESEF.2.5.4.externalCssReportPackage",
                                         _("The CSS file should be physically stored within the report package: %{file}s."),
                                         modelObject=elt, file=_file)
                             else:
                                 modelXbrl.warning("ESEF.2.5.4.externalCssFileForSingleIXbrlDocument",
                                     _("Where an Inline XBRL document set contains a single document, the CSS SHOULD be embedded within the document."),
                                     modelObject=elt, element=eltTag)
-                        elif val.unconsolidated:
-                            pass # rest of following tests don't apply to unconsolidated
                         elif eltTag == "style" and elt.get("type") == "text/css":
-                            if len(modelXbrl.ixdsHtmlElements) > 1:
-                                modelXbrl.warning("ESEF.2.5.4.embeddedCssForMultiHtmlIXbrlDocumentSets",
-                                    _("Where an Inline XBRL document set contains multiple documents, the CSS SHOULD be defined in a separate file."),
-                                    modelObject=elt, element=eltTag)
-                            if "position:absolute" in elt.stringValue:
-                                # detect absolute positioning such as from Adobe Indesign producing pdf from whic html is extracted
-                                hasAbsolutePositioning = True
+                            validateCssUrl(elt.stringValue, elt.modelDocument.baseForElement(elt), modelXbrl, val, elt, contentOtherThanXHTMLGuidance)
+                            if not val.unconsolidated:
+                                if len(modelXbrl.ixdsHtmlElements) > 1:
+                                    modelXbrl.warning("ESEF.2.5.4.embeddedCssForMultiHtmlIXbrlDocumentSets",
+                                                      _("Where an Inline XBRL document set contains multiple documents, the CSS SHOULD be defined in a separate file."),
+                                                      modelObject=elt, element=eltTag)
+                                if "position:absolute" in elt.stringValue:
+                                    # detect absolute positioning such as from Adobe Indesign producing pdf from whic html is extracted
+                                    hasAbsolutePositioning = True
 
                     if eltTag in ixTags and elt.get("target") and ixTargetUsage != "allowed":
                         modelXbrl.log(ixTargetUsage.upper(),
                             "ESEF.2.5.3.targetAttributeUsedForESEFContents",
                             _("Target attribute %(severityVerb)s not be used unless explicitly required by local jurisdictions: element %(localName)s, target attribute %(target)s."),
                             modelObject=elt, localName=elt.elementQname, target=elt.get("target"),
                             severityVerb={"warning":"SHOULD","error":"MUST"}[ixTargetUsage])
@@ -610,16 +627,16 @@
                 # maliciously hidden facts
                 for cssHiddenElt in ixdsHtmlRootElt.getroottree().iterfind("//{http://www.w3.org/1999/xhtml}*[@style]"):
                     if styleCssHiddenPattern.match(cssHiddenElt.get("style","")):
                         for tag in (ixNStag + "nonNumeric", ixNStag+"nonFraction"):
                             for ixElt in cssHiddenElt.iterdescendants(tag=tag):
                                 if ixElt not in ixHiddenFacts:
                                     modelXbrl.error("ESEF.2.5.4.displayNoneUsedToHideTaggedFacts",
-                                        _("\"display:none\" style applies to a fact that is not in an ix:hidden section."),
-                                        modelObject=ixElt)
+                                        _('CSS MUST not be used to hide tagged facts, e.g. by applying display:none style. Concept "%(concept)s", value: %(value)s - line %(sourceline)s'),
+                                        modelObject=ixElt, concept=ixElt.concept.label(), sourceline=ixElt.sourceline, value=ixElt.effectiveValue)
                 del ixHiddenFacts
 
                 firstIxdsDoc = False
 
             if val.unconsolidated:
                 modelXbrl.modelManager.showStatus(None)
                 return # no more checks apply
@@ -628,21 +645,33 @@
                     _("The ix:hidden section of Inline XBRL document MUST not include elements eligible for transformation. "
                       "%(countEligible)s fact(s) were eligible for transformation: %(elements)s"),
                     modelObject=eligibleForTransformHiddenFacts,
                     countEligible=len(eligibleForTransformHiddenFacts),
                     elements=", ".join(sorted(set(str(f.qname) for f in eligibleForTransformHiddenFacts))))
             for ixdsHtmlRootElt in modelXbrl.ixdsHtmlElements:
                 for ixElt in ixdsHtmlRootElt.getroottree().iterfind("//{http://www.w3.org/1999/xhtml}*[@style]"):
-                    hiddenFactRefMatch = styleIxHiddenPattern.match(ixElt.get("style",""))
+                    styleValue = ixElt.get("style","")
+                    hiddenFactRefMatch = styleIxHiddenPattern.match(styleValue)
+
+                    if styleValue:
+                        for declaration in tinycss2.parse_declaration_list(styleValue):
+                            if isinstance(declaration, tinycss2.ast.Declaration):
+                                validateCssUrlContent(declaration.value, ixElt.modelDocument.baseForElement(ixElt),
+                                                      modelXbrl, val, ixElt, contentOtherThanXHTMLGuidance)
+                            elif isinstance(declaration, tinycss2.ast.ParseError):
+                                modelXbrl.warning("ix.CssParsingError",
+                                                  _("The style attribute contains erroneous CSS declaration \"%(styleContent)s\": %(parseError)s"),
+                                                  modelObject=ixElt, parseError=declaration.message,
+                                                  styleContent=styleValue)
                     if hiddenFactRefMatch:
                         hiddenFactRef = hiddenFactRefMatch.group(2)
                         if hiddenFactRef not in hiddenEltIds:
                             modelXbrl.error("ESEF.2.4.1.esefIxHiddenStyleNotLinkingFactInHiddenSection",
-                                _("\"-esef-ix-hidden\" style identifies @id, %(id)s of a fact that is not in ix:hidden section."),
-                                modelObject=ixElt, id=hiddenFactRef)
+                                _("\"-esef-ix-hidden\" style identifies id attribute of a fact that is not in ix:hidden section: %(factId)s"),
+                                modelObject=ixElt, factId=hiddenFactRef)
                         else:
                             presentedHiddenEltIds[hiddenFactRef].append(ixElt)
             for hiddenEltId, ixElt in hiddenEltIds.items():
                 if (hiddenEltId not in presentedHiddenEltIds and
                     getattr(ixElt, "xValid", 0) >= VALID and # may not be validated
                     (ixElt.concept.baseXsdType in untransformableTypes or ixElt.isNil)):
                     requiredToDisplayFacts.append(ixElt)
@@ -834,14 +863,16 @@
             if len(fList) > 1:
                 f0: ModelFact = fList[0]
                 if any(f.isNil for f in fList):
                     _inConsistent = not all(f.isNil for f in fList)
                 else: # not all have same decimals
                     _d = inferredDecimals(f0)
                     _v = cast(float, f0.xValue)
+                    if _v is None:
+                        continue
                     _inConsistent = isnan(_v) # NaN is incomparable, always makes dups inconsistent
                     decVals[_d] = _v
                     aMax, bMin = rangeValue(_v, _d)
                     for f in fList[1:]:
                         _d = inferredDecimals(f)
                         _v = cast(float, f.xValue)
                         if isnan(_v):
@@ -855,15 +886,15 @@
                         if a > aMax: aMax = a
                         if b < bMin: bMin = b
                     if not _inConsistent:
                         _inConsistent = (bMin < aMax)
                     decVals.clear()
                 if _inConsistent:
                     modelXbrl.error(("ESEF.2.2.4.inconsistentDuplicateNumericFactInInlineXbrlDocument"),
-                        "Inconsistent duplicate numeric facts MUST NOT appear in the content of an inline XBRL document. %(fact)s that was used more than once in contexts equivalent to %(contextID)s: values %(values)s.  ",
+                        _("Inconsistent duplicate numeric facts MUST NOT appear in the content of an inline XBRL document. %(fact)s that was used more than once in contexts equivalent to %(contextID)s: values %(values)s."),
                         modelObject=fList, fact=f0.qname, contextID=f0.contextID, values=", ".join(strTruncate(f.value, 128) for f in fList))
 
         if precisionFacts:
             modelXbrl.error("ESEF.2.2.1.precisionAttributeUsed",
                             _("The accuracy of numeric facts MUST be defined with the 'decimals' attribute rather than the 'precision' attribute: %(elements)s."),
                             modelObject=precisionFacts, elements=", ".join(sorted(str(e.qname) for e in precisionFacts)))
 
@@ -877,16 +908,16 @@
             modelXbrl.error("ESEF.2.2.3.incorrectTransformationRuleApplied",
                               _("ESMA recommends applying the Transformation Rules Registry 4, as published by XBRL International or any more recent versions of the Transformation Rules Registry provided with a 'Recommendation' status, for these elements: %(elements)s."),
                               modelObject=transformRegistryErrors,
                               elements=", ".join(sorted(str(fact.qname) for fact in transformRegistryErrors)))
 
         if orphanedFootnotes:
             modelXbrl.warning("ESEF.2.3.1.unusedFootnote",
-                _("Every nonempty link:footnote element SHOULD be linked to at least one fact."),
-                modelObject=orphanedFootnotes)
+                _("Every nonempty link:footnote element SHOULD be linked to at least one fact. Unused footnote ids: %(ids)s"),
+                modelObject=orphanedFootnotes, ids=', '.join([f'"{footnote.id}"' for footnote in orphanedFootnotes]))
 
         # this test removed from Filer Manual July 2020
         #if noLangFootnotes:
         #    modelXbrl.error("ESEF.2.3.1.undefinedLanguageForFootnote",
         #        _("Each footnote MUST have the 'xml:lang' attribute whose value corresponds to the language of the text in the content of the respective footnote."),
         #        modelObject=noLangFootnotes)
         ftLangNotUsedByTextFacts = set()
@@ -936,25 +967,25 @@
             if e in val.extensionImportedUrls:
                 val.modelXbrl.error("ESEF.3.1.2.incorrectEsefTaxonomyVersionUsed",
                      _("The issuer's extension taxonomies MUST import the applicable version of the taxonomy files prepared by ESMA. Outdated entry point: %(url)s"),
                     modelObject=modelDocument, url=e)
                 hasOutdatedUrl = True
 
         if ("authorityRequiredTaxonomyURLs" in val.authParam and
-            not any(e in val.extensionImportedUrls for e in val.authParam["authorityRequiredTaxonomyURLs"])):
+                not any(e in val.extensionImportedUrls for e in val.authParam["authorityRequiredTaxonomyURLs"])):
             val.modelXbrl.error(
                 "UKFRC22.3.requiredFrcEntryPointNotImported",
-                 _("The issuer's extension taxonomies MUST import the FRC entry point of the taxonomy files prepared by %(authority)s."),
+                _("The issuer's extension taxonomies MUST import the FRC entry point of the taxonomy files prepared by %(authority)s."),
                 modelObject=modelDocument, authority=val.authParam["authorityName"])
 
         if not hasOutdatedUrl and not any(e in val.extensionImportedUrls for e in val.authParam["effectiveTaxonomyURLs"]):
             val.modelXbrl.error(
                 "UKFRC22.1.requiredUksefEntryPointNotImported" if val.authority == "UKFRC" else
                 "ESEF.3.1.2.requiredEntryPointNotImported",
-                 _("The issuer's extension taxonomies MUST import the entry point of the taxonomy files prepared by %(authority)s."),
+                _("The issuer's extension taxonomies MUST import the entry point of the taxonomy files prepared by %(authority)s."),
                 modelObject=modelDocument, authority=val.authParam["authorityName"])
 
 
         # unused elements in linkbases
         unreportedLbElts = set()
         for arcroles, error, checkRoots, lbType in (
                     ((parentChild,), "elements{}UsedForTagging{}AppliedInPresentationLinkbase", True, "presentation"),
@@ -981,17 +1012,19 @@
                             unreportedLbElts.add(to)
                     reportedEltsNotInLb.discard(fr)
                     reportedEltsNotInLb.discard(to)
 
             if reportedEltsNotInLb and lbType == "presentation":
                 # reported pri items excluded from having to be in pre LB
                 nsExcl = val.authParam.get("lineItemsMustBeInPreLbExclusionNsPattern")
+                nsExclPat = None
                 if nsExcl:
                     nsExclPat = re.compile(nsExcl)
-                    reportedEltsNotInLb -= set(c for c in reportedEltsNotInLb if nsExclPat.match(c.qname.namespaceURI))
+                reportedEltsNotInLb -= set(c for c in reportedEltsNotInLb
+                                           if nsExclPat and nsExclPat.match(c.qname.namespaceURI))
             if reportedEltsNotInLb and lbType != "calculation":
                 modelXbrl.warning(f"ESEF.3.4.6.UsableConceptsNotIncludedIn{lbType.title()}Link",
                     _("All concepts used by tagged facts SHOULD be in extension taxonomy %(linkbaseType)s relationships: %(elements)s."),
                     modelObject=reportedEltsNotInLb, elements=", ".join(sorted((str(c.qname) for c in reportedEltsNotInLb))), linkbaseType=lbType)
         if unreportedLbElts:
             modelXbrl.warning("ESEF.3.4.6.UsableConceptsNotAppliedByTaggedFacts",
                 _("All usable concepts in extension taxonomy relationships SHOULD be applied by tagged facts: %(elements)s."),
@@ -1018,15 +1051,15 @@
         pfsConceptsRootInPreLB = set()
         # Annex II para 1 check of monetary declaration
         statementMonetaryUnitReportedConcepts = defaultdict(set) # index is unit, set is concepts
         statementMonetaryUnitFactCounts: dict[Any, Any] = {}
 
         def checkLabels(parent: ModelConcept, relSet: ModelRelationshipSet, labelrole: str | None, visited: set[ModelConcept]) -> None:
             if not parent.label(labelrole,lang=reportXmlLang,fallbackToQname=False):
-                if not labelrole or labelrole == standardLabel:
+                if (not labelrole or labelrole == standardLabel) and isExtension(val, parent):
                     missingConceptLabels[labelrole].add(parent)
             visited.add(parent)
             conceptRels = defaultdict(list) # counts for concepts without preferred label role
             for rel in relSet.fromModelObject(parent):
                 child = rel.toModelObject
                 if child is not None:
                     labelrole = rel.preferredLabel
@@ -1074,18 +1107,19 @@
                     has_extension_label = False
                     for label in labels:
                         if isExtension(val, label):
                             has_extension_label = True
                         else:
                             has_core_label = True
                     if has_core_label and has_extension_label:
+                        labels_files = ['"%s": %s' % (l.text, l.modelDocument.basename) for l in labels]
                         val.modelXbrl.error(
                             "ESEF.3.4.5.taxonomyElementDuplicateLabels",
-                            _("Issuer extension taxonomy with core taxonomy element: %(concept)s is assigned 2 labels using standard label role"),
-                            modelObject=[modelConcept]+labels, concept=modelConcept.qname, lang=lang, labelrole=labelrole)
+                            _("Issuer extension taxonomy with core taxonomy element: %(concept)s is assigned 2 labels using standard label role: %(labels)s"),
+                            modelObject=[modelConcept]+labels, concept=modelConcept.qname, lang=lang, labelrole=labelrole, labels=", ".join(labels_files))
 
         for ELR in modelXbrl.relationshipSet(parentChild).linkRoleUris:
             relSet = modelXbrl.relationshipSet(parentChild, ELR)
             pfsConceptsRootInELR = set()
             nonPfsConceptsRootInELR = set()
 
             for rootConcept in relSet.rootConcepts:
@@ -1179,14 +1213,39 @@
                             modelXbrl.error("ESEF.RTS.Annex.IV.Par.4.1.extensionElementDuplicatesCoreElement",
                         _("Extension elements must not duplicate the existing elements from the core taxonomy and be identifiable %(qname)s."),
                         modelObject=(c,_i), qname=c.qname)
 
     modelXbrl.profileActivity(_statusMsg, minTimeToShow=0.0)
     modelXbrl.modelManager.showStatus(None)
 
+def validateCssUrl(cssContent:str, normalizedUri:str, modelXbrl: ModelXbrl, val: ValidateXbrl, elt: ModelObject, contentOtherThanXHTMLGuidance: str) -> None:
+    css_elements = tinycss2.parse_stylesheet(cssContent)
+    for css_element in css_elements:
+        if isinstance(css_element, tinycss2.ast.AtRule):
+            if css_element.lower_at_keyword == "font-face":
+                for css_rule in css_element.content:
+                    if isinstance(css_rule, tinycss2.ast.URLToken) and "data:font" not in css_rule.value:
+                        modelXbrl.warning(
+                            "ESEF.%s.fontIncludedAndNotEmbeddedAsBase64EncodedString" % contentOtherThanXHTMLGuidance,
+                            _("Fonts SHOULD be included in the XHTML document as a base64 encoded string: %(file)s."),
+                            modelObject=elt, file=css_rule.value)
+        if isinstance(css_element, tinycss2.ast.QualifiedRule):
+            validateCssUrlContent(css_element.content, normalizedUri, modelXbrl, val, elt, contentOtherThanXHTMLGuidance)
+
+
+def validateCssUrlContent(cssRules: List[Any], normalizedUri:str, modelXbrl: ModelXbrl, val: ValidateXbrl, elt: ModelObject, contentOtherThanXHTMLGuidance: str) -> None:
+    for css_rule in cssRules:
+        if isinstance(css_rule, tinycss2.ast.FunctionBlock):
+            if css_rule.lower_name == "url":
+                if len(css_rule.arguments):
+                    css_rule_url = css_rule.arguments[0].value  # url or base64
+                    evaluatedMsg = _('On line {line}').format(line=1) #css_element.source_line)
+                    validateImage(normalizedUri, css_rule_url, modelXbrl, val, elt, evaluatedMsg, contentOtherThanXHTMLGuidance)
+
+
 def validateFinally(val: ValidateXbrl, *args: Any, **kwargs: Any) -> None: # runs all inline checks
     if not (val.validateESEFplugin):
         return
 
     if val.unconsolidated:
         return
 
@@ -1209,15 +1268,15 @@
 
 def validateFormulaCompiled(modelXbrl: ModelXbrl, xpathContext: XPathContext) -> None:
     # request unsatisfied assertions without a message to print a trace
     # this is not conditional on validateESEFplugin so the flag is set even if DisclosureSystemChecks not requested upon compiling but set later in workflow
     xpathContext.formulaOptions.traceUnmessagedUnsatisfiedAssertions = True
 
 def validateFormulaFinished(val: ValidateXbrl, *args: Any, **kwargs: Any) -> None: # runs *after* formula (which is different for test suite from other operation
-    if not (val.validateESEFplugin):
+    if not getattr(val, 'validateESEFplugin', False):
         return
 
     modelXbrl = val.modelXbrl
     if hasattr(val, 'priorFormulaOptionsRunIDs'):  # reset environment formula run IDs if they were saved
         modelXbrl.modelManager.formulaOptions.runIDs = val.priorFormulaOptionsRunIDs
     sumWrnMsgs = sumErrMsgs = 0
     for e in modelXbrl.errors:
```

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/config.xml` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ESEF_2022/resources/authority-validations.json` & `arelle-release-2.8.0/arelle/plugin/validate/ESEF_2022/resources/authority-validations.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916126523204561%*

 * *Differences: {"'LU'": "{'minExternalResourceSizekB': 1024}",*

 * * "'default'": "{'minExternalResourceSizekB': 0}",*

 * * "'description'": "{insert: [(11, 'minExternalResourceSizekB: minimal file size in kB for allowing "*

 * *                  'external resources, 0 if no minimum requirement and -1 if external resources '*

 * *                  "are forbidden')]}"}*

```diff
@@ -68,14 +68,15 @@
     "LI": {
         "name": "Liechtenstein"
     },
     "LT": {
         "name": "Lithuania"
     },
     "LU": {
+        "minExternalResourceSizekB": 1024,
         "name": "Luxembourg"
     },
     "LV": {
         "name": "Latvia"
     },
     "MT": {
         "name": "Malta",
@@ -213,14 +214,15 @@
             "https://www.esma.europa.eu/taxonomy/2021-03-24/esef_cor.xsd": [
                 "https://www.esma.europa.eu/taxonomy/2021-03-24/esef_cor-gen-en.xml"
             ]
         },
         "formulaRunIDs": null,
         "identiferScheme": "http://standards.iso.org/iso/17442",
         "ixTargetUsage": "warning",
+        "minExternalResourceSizekB": 0,
         "name": "Default ESMA ESEF-2022 validations",
         "outdatedTaxonomyURLs": [
             "http://www.esma.europa.eu/taxonomy/2017-03-31/esef_cor.xsd",
             "https://www.esma.europa.eu/taxonomy/2017-03-31/esef_cor.xsd",
             "http://www.esma.europa.eu/taxonomy/2019-03-27/esef_cor.xsd",
             "https://www.esma.europa.eu/taxonomy/2019-03-27/esef_cor.xsd",
             "http://www.esma.europa.eu/taxonomy/2020-03-16/esef_cor.xsd",
@@ -260,14 +262,15 @@
         "A JSON object by authority with objects ",
         "",
         "key: code of the authority",
         "name: authority for which this object applies",
         "authorityName: name of issuing authority, such as ESMA for ESEF and FRC for UKSEF",
         "reference: document(s) pertinent to authority validation",
         "reportPackageMaxMB: max file size in MB or null for unlimited",
+        "minExternalResourceSizekB: minimal file size in kB for allowing external resources, 0 if no minimum requirement and -1 if external resources are forbidden",
         "reportPackageMeasurement: \"zipped\" or \"unzipped\"",
         "ixTargetUsage: allowed, warning or error",
         "extensionAbstractContexts: allowed, warning or error",
         "lineItemsNotDimQualExclusionNsPattern: concepts namespace pattern excluded from check for extensionTaxonomyLineItemNotLinkedToAnyHypercube",
         "lineItemsMustBeInPreLbExclusionNsPattern: concepts namespace pattern excluded from check for required presence in presentation linkbase",
         "LC3CapitalsInWord: true means label \"NonControlling Interest\" matches name \"NoncontrollingInterest\"",
         "reportFileNamePattern: filename pattern where applied by authority, for message display",
```

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/FERC/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/FERC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/FERC/config.xml` & `arelle-release-2.8.0/arelle/plugin/validate/FERC/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/FERC/resources/ferc-utr.xml` & `arelle-release-2.8.0/arelle/plugin/validate/FERC/resources/ferc-utr.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/GFM/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/GFM/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/GFM/config.xml` & `arelle-release-2.8.0/arelle/plugin/validate/GFM/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/HMRC/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/HMRC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/HMRC/config.xml` & `arelle-release-2.8.0/arelle/plugin/validate/HMRC/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/HMRC/consistencyChecksByName.json` & `arelle-release-2.8.0/arelle/plugin/validate/HMRC/consistencyChecksByName.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/HMRC/hmrc-taxonomies.xml` & `arelle-release-2.8.0/arelle/plugin/validate/HMRC/hmrc-taxonomies.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ROS/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/ROS/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/ROS/config.xml` & `arelle-release-2.8.0/arelle/plugin/validate/ROS/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/SBRnl/CustomLoader.py` & `arelle-release-2.8.0/arelle/plugin/validate/SBRnl/CustomLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/SBRnl/DTS.py` & `arelle-release-2.8.0/arelle/plugin/validate/SBRnl/DTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/SBRnl/Dimensions.py` & `arelle-release-2.8.0/arelle/plugin/validate/SBRnl/Dimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/SBRnl/Document.py` & `arelle-release-2.8.0/arelle/plugin/validate/SBRnl/Document.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/SBRnl/Filing.py` & `arelle-release-2.8.0/arelle/plugin/validate/SBRnl/Filing.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/SBRnl/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/SBRnl/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/SBRnl/config.xml` & `arelle-release-2.8.0/arelle/plugin/validate/SBRnl/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/SBRnl/sbr-nl-taxonomies.xml` & `arelle-release-2.8.0/arelle/plugin/validate/SBRnl/sbr-nl-taxonomies.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/USBestPractices.py` & `arelle-release-2.8.0/arelle/plugin/validate/USBestPractices.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/USCorpAction.py` & `arelle-release-2.8.0/arelle/plugin/validate/USCorpAction.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/USSecTagging.py` & `arelle-release-2.8.0/arelle/plugin/validate/USSecTagging.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/XDC/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/XDC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/XDC/config.xml` & `arelle-release-2.8.0/arelle/plugin/validate/XDC/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/XFsyntax/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/XFsyntax/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/XFsyntax/xf.py` & `arelle-release-2.8.0/arelle/plugin/validate/XFsyntax/xf.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/__init__.py` & `arelle-release-2.8.0/arelle/plugin/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validate/calc2.py` & `arelle-release-2.8.0/arelle/plugin/validate/calc2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/validateSBRnl.py` & `arelle-release-2.8.0/arelle/plugin/validateSBRnl.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/DialogRssWatchExtender.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/DialogRssWatchExtender.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/SqlDb.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/SqlDb.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlDpmSqlDB.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlDpmSqlDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlOpenSqlDB.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlOpenSqlDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlPublicPostgresDB.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlPublicPostgresDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlSemanticGraphDB.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlSemanticGraphDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlSemanticJsonDB.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlSemanticJsonDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlSemanticRdfDB.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlSemanticRdfDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/XbrlSemanticSqlDB.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/XbrlSemanticSqlDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/__init__.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/entityInformation.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/entityInformation.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/ext/china.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/ext/china.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/ext/edgar.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/ext/edgar.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/ext/xdc.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/ext/xdc.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/primaryDocumentFacts.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/primaryDocumentFacts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open/ext/chinaPostgresDB.ddl` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open/ext/chinaPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open/ext/edgarPostgresDB.ddl` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open/ext/edgarPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open/ext/xdcPostgresDB.ddl` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open/ext/xdcPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open/xbrlOpenPostgresDB.ddl` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open/xbrlOpenPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/open2/xbrlOpen2PostgresDB.ddl` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/open2/xbrlOpen2PostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/public/xbrlPublicPostgresDB.ddl` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/public/xbrlPublicPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/secDatabaseModelViews.sql` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/secDatabaseModelViews.sql`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticColumnComments.ddl` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticColumnComments.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMSSqlDB.sql` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMSSqlDB.sql`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMySqlDB.ddl` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMySqlDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticOracleDB.sql` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticOracleDB.sql`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticPostgresDB.ddl` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticSQLiteDB.ddl` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticSQLiteDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xbrlDB/tableFacts.py` & `arelle-release-2.8.0/arelle/plugin/xbrlDB/tableFacts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/plugin/xuleSaver.py` & `arelle-release-2.8.0/arelle/plugin/xuleSaver.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/scripts-windows/exportCsvFromXbrlInstance.bat` & `arelle-release-2.8.0/arelle/scripts-windows/exportCsvFromXbrlInstance.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/scripts-windows/runFormulaTests.bat` & `arelle-release-2.8.0/arelle/scripts-windows/runFormulaTests.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/scripts-windows/validateAndRunFormulas.bat` & `arelle-release-2.8.0/arelle/scripts-windows/validateAndRunFormulas.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/typing.py` & `arelle-release-2.8.0/arelle/typing.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/webserver/bottle-no2to3.py` & `arelle-release-2.8.0/arelle/webserver/bottle-no2to3.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle/webserver/bottle.py` & `arelle-release-2.8.0/arelle/webserver/bottle.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelleCmdLine.py` & `arelle-release-2.8.0/arelleCmdLine.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle_release.egg-info/PKG-INFO` & `arelle-release-2.8.0/arelle_release.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arelle-release
-Version: 2.7.1
+Version: 2.8.0
 Summary: An open source XBRL platform.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
@@ -27,14 +27,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: Crypto
 Provides-Extra: DB
 Provides-Extra: EFM
+Provides-Extra: ESEF
 Provides-Extra: ObjectMaker
 Provides-Extra: WebServer
 License-File: LICENSE.md
 
 # Arelle
 
 [![pypi-version](https://img.shields.io/pypi/v/arelle-release.svg)](https://pypi.org/project/arelle-release/)
```

### Comparing `arelle-release-2.7.1/arelle_release.egg-info/SOURCES.txt` & `arelle-release-2.8.0/arelle_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/arelle_test.py` & `arelle-release-2.8.0/arelle_test.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/attic/CntlrGenVersReports.py` & `arelle-release-2.8.0/attic/CntlrGenVersReports.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/buildVersion.py` & `arelle-release-2.8.0/buildVersion.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/conftest.py` & `arelle-release-2.8.0/conftest.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/distro.py` & `arelle-release-2.8.0/distro.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/docker/ubuntu.Dockerfile` & `arelle-release-2.8.0/docker/ubuntu.Dockerfile`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/encodeUtf8PySource.py` & `arelle-release-2.8.0/encodeUtf8PySource.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/generateMessagesCatalog.py` & `arelle-release-2.8.0/generateMessagesCatalog.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/installWin64.nsi` & `arelle-release-2.8.0/installWin64.nsi`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/installWin86.nsi` & `arelle-release-2.8.0/installWin86.nsi`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/linux/Tktable2.11/README.txt` & `arelle-release-2.8.0/libs/linux/Tktable2.11/README.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/linux/Tktable2.11/html/tkTable.html` & `arelle-release-2.8.0/libs/linux/Tktable2.11/html/tkTable.html`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/linux/Tktable2.11/libTktable2.11.so` & `arelle-release-2.8.0/libs/linux/Tktable2.11/libTktable2.11.so`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/linux/Tktable2.11/license.txt` & `arelle-release-2.8.0/libs/linux/Tktable2.11/license.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/linux/Tktable2.11/tkTable.tcl` & `arelle-release-2.8.0/libs/linux/Tktable2.11/tkTable.tcl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/linux/Tktable2.11/tktable.py` & `arelle-release-2.8.0/libs/linux/Tktable2.11/tktable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/macos/Tktable2.11/README.txt` & `arelle-release-2.8.0/libs/macos/Tktable2.11/README.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/macos/Tktable2.11/html/tkTable.html` & `arelle-release-2.8.0/libs/macos/Tktable2.11/html/tkTable.html`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/macos/Tktable2.11/libTktable2.11.dylib` & `arelle-release-2.8.0/libs/macos/Tktable2.11/libTktable2.11.dylib`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/macos/Tktable2.11/license.txt` & `arelle-release-2.8.0/libs/macos/Tktable2.11/license.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/macos/Tktable2.11/tkTable.tcl` & `arelle-release-2.8.0/libs/macos/Tktable2.11/tkTable.tcl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/macos/Tktable2.11/tktable.py` & `arelle-release-2.8.0/libs/macos/Tktable2.11/tktable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/win64/Tktable2.11/Tktable.dll` & `arelle-release-2.8.0/libs/win64/Tktable2.11/Tktable.dll`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/libs/win64/Tktable2.11/tkTable.tcl` & `arelle-release-2.8.0/libs/win64/Tktable2.11/tkTable.tcl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/messages.pot` & `arelle-release-2.8.0/messages.pot`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/msgfmt.py` & `arelle-release-2.8.0/msgfmt.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/plugins/xbrl-us/us-gaap-consistency.py` & `arelle-release-2.8.0/plugins/xbrl-us/us-gaap-consistency.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/pygettext.py` & `arelle-release-2.8.0/pygettext.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/pyproject.toml` & `arelle-release-2.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,17 @@
     'PyMySQL==1.*',
     'pyodbc==4.*',
     'rdflib==5.*',
 ]
 EFM = [
     'holidays==0.*',
 ]
+ESEF = [
+    'tinycss2==1.*',
+]
 ObjectMaker = [
     'graphviz==0.*',
 ]
 WebServer = [
     'cheroot>=8,<10',
     'CherryPy==18.*',
     'tornado==6.*',
@@ -84,14 +87,19 @@
 [tool.setuptools_scm]
 tag_regex = "^(?:[\\w-]+-?)?(?P<version>[vV]?\\d+(?:\\.\\d+){0,2}[^\\+]*)(?:\\+.*)?$"
 write_to = "arelle/_version.py"
 
 [tool.pytest.ini_options]
 xfail_strict = true
 empty_parameter_set_mark = "fail_at_collect"
+addopts = "--strict-markers"
+markers = [
+    "fast: mark automatically applied to tests which don't have the \"slow\" mark applied (deselect with '-m \"not fast\"')",
+    "slow: marks tests as slow (deselect with '-m \"not slow\"')",
+]
 
 [tool.mypy]
 # Warn when a # type: ignore comment does not specify any error codes
 enable_error_code = "ignore-without-code"
 
 python_version = "3.11"
```

### Comparing `arelle-release-2.7.1/requirements.txt` & `arelle-release-2.8.0/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 pycountry==22.3.5
 # plugins
 # EdgarRenderer plugin
 NumPy==1.21.6 ; python_version < "3.8"
 NumPy==1.23.4 ; python_version >= "3.8"
 Matplotlib==3.5.3 ; python_version < "3.8"
 Matplotlib==3.6.1 ; python_version >= "3.8"
-holidays==0.22
+holidays==0.23
 Tornado==6.2
 # security plugin
 PyCryptodome==3.17
 # xbrlDB plugin
 cx_Oracle==8.3.0
 pg8000==1.29.4
 PyMySQL==1.0.3
 pyodbc==4.0.39
 RDFLib==5.0.0
 # other
 graphviz==0.20.1
 Pillow==9.5.0
 pywin32==306 ; sys_platform == "win32"
+tinycss2==1.2.1
```

### Comparing `arelle-release-2.7.1/scripts/buildLinuxDist.sh` & `arelle-release-2.8.0/scripts/buildLinuxDist.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/buildMacDist.sh` & `arelle-release-2.8.0/scripts/buildMacDist.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/buildWinDist.bat` & `arelle-release-2.8.0/scripts/buildWinDist.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/charlieTest.bat` & `arelle-release-2.8.0/scripts/charlieTest.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/exportCsvFormulae.bat` & `arelle-release-2.8.0/scripts/exportCsvFormulae.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/exportCsvFromXbrlInstance.bat` & `arelle-release-2.8.0/scripts/exportCsvFromXbrlInstance.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/generateTestcase.py` & `arelle-release-2.8.0/scripts/generateTestcase.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/reportAllTests.bat` & `arelle-release-2.8.0/scripts/reportAllTests.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/runESMAtests.sh` & `arelle-release-2.8.0/scripts/runESMAtests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/runGenerateVersioningTestcases.bat` & `arelle-release-2.8.0/scripts/runGenerateVersioningTestcases.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/runPackageTests.sh` & `arelle-release-2.8.0/scripts/runPackageTests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/runPyTest.sh` & `arelle-release-2.8.0/scripts/runPyTest.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/runTR2Tests.sh` & `arelle-release-2.8.0/scripts/runTR2Tests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/runTR3Tests.sh` & `arelle-release-2.8.0/scripts/runTR3Tests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/runTR4Tests.sh` & `arelle-release-2.8.0/scripts/runTR4Tests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/runTR5Tests.sh` & `arelle-release-2.8.0/scripts/runTR5Tests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/runTRSECTests.sh` & `arelle-release-2.8.0/scripts/runTRSECTests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/scripts/runVersioningConsumptionTests.bat` & `arelle-release-2.8.0/scripts/runVersioningConsumptionTests.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/setup.cfg` & `arelle-release-2.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/ArelleGUITest.csproj` & `arelle-release-2.8.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/ArelleGUITest.csproj`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Tests.cs` & `arelle-release-2.8.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Tests.cs`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest.sln` & `arelle-release-2.8.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest.sln`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/ui_tests/resources/workiva.zip` & `arelle-release-2.8.0/tests/integration_tests/ui_tests/resources/workiva.zip`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/README.md` & `arelle-release-2.8.0/tests/integration_tests/validation/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_config.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_config.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configs.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/efm_current.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/efm_current.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2021.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2021.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2022.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2022.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2021.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2021.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2022.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2022.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_2_1.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_2_1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_dimensions_1_0.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_dimensions_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_1_0.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_function_registry.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_function_registry.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_ixbrl_1_1.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_ixbrl_1_1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_oim_1_0.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_oim_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_table_linkbase_1_0.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_table_linkbase_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_malformed_1_0.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_malformed_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_registry_1_0.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_registry_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_structure_1_0.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_structure_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/conftest.py` & `arelle-release-2.8.0/tests/integration_tests/validation/conftest.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/download_conformance_suites.py` & `arelle-release-2.8.0/tests/integration_tests/validation/download_conformance_suites.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/run_conformance_suites.py` & `arelle-release-2.8.0/tests/integration_tests/validation/run_conformance_suites.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from tests.integration_tests.validation.conformance_suite_configs import (
     ALL_CONFORMANCE_SUITE_CONFIGS,
     PUBLIC_CONFORMANCE_SUITE_CONFIGS
 )
 from tests.integration_tests.validation.download_conformance_suites import (
     download_conformance_suite, extract_conformance_suite
 )
+from typing import Optional
 
 ARGUMENTS = [
     {
         "name": "--all",
         "action": "store_true",
         "help": "Select all configured conformance suites"
     },
@@ -113,15 +114,15 @@
         test_option=options.test,
         download_option=download_option,
         log_to_file=options.log_to_file,
         offline_option=options.offline
     )
 
 
-def get_download_option(options: Namespace) -> str | None:
+def get_download_option(options: Namespace) -> Optional[str]:
     if options.download_overwrite:
         return DOWNLOAD_OVERWRITE
     elif options.download_missing:
         return DOWNLOAD_MISSING
     return None
```

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/test_conformance_suites.py` & `arelle-release-2.8.0/tests/integration_tests/validation/test_conformance_suites.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/integration_tests/validation/validation_util.py` & `arelle-release-2.8.0/tests/integration_tests/validation/validation_util.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/unit_tests/arelle/formula/test_fact_aspects_cache.py` & `arelle-release-2.8.0/tests/unit_tests/arelle/formula/test_fact_aspects_cache.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/unit_tests/arelle/plugin/test_loadfromoim.py` & `arelle-release-2.8.0/tests/unit_tests/arelle/plugin/test_loadfromoim.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/unit_tests/arelle/test_cntlr.py` & `arelle-release-2.8.0/tests/unit_tests/arelle/test_cntlr.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from mock import patch
 
 from arelle import Cntlr
 
 
 @patch('io.open')
+@patch('os.path.exists')
 @patch('arelle.Cntlr.Cntlr.setUiLanguage')
 @patch('arelle.ModelManager.ModelManager.setLocale')
-def test_cntlr_cache_enabled(_, mock_codes, mock_open):
+def test_cntlr_cache_enabled(_, mock_codes, mock_exists, mock_open):
     mock_codes.return_value = ['en-US', 'en_US', 'en']
+    mock_exists.return_value = True
     cntlr = Cntlr.Cntlr(uiLang=None)
-    assert mock_open.call_count == 1
+    assert mock_open.call_count == 3
     cntlr.saveConfig()
-    assert mock_open.call_count == 2
+    assert mock_open.call_count == 4
 
 @patch('io.open')
+@patch('os.path.exists')
 @patch('arelle.Cntlr.Cntlr.setUiLanguage')
 @patch('arelle.ModelManager.ModelManager.setLocale')
-def test_cntlr_cache_disabled(_, mock_codes, mock_open):
+def test_cntlr_cache_disabled(_, mock_codes, mock_exists, mock_open):
     mock_codes.return_value = ['en-US', 'en_US', 'en']
+    mock_exists.return_value = True
     cntlr = Cntlr.Cntlr(uiLang=None, disable_persistent_config=True)
-    assert mock_open.call_count == 0
+    assert mock_open.call_count == 1
     cntlr.saveConfig()
-    assert mock_open.call_count == 0
+    assert mock_open.call_count == 1
```

### Comparing `arelle-release-2.7.1/tests/unit_tests/arelle/test_import.py` & `arelle-release-2.8.0/tests/unit_tests/arelle/test_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,10 +27,11 @@
         module_name,
         id=module_name,
         marks=[pytest.mark.xfail()] if module_name in KNOWN_FAILURES else []
     ) for module_name in MODULE_NAMES
 ]
 
 
+@pytest.mark.slow
 @pytest.mark.parametrize('module_name', TEST_PARAMS)
 def test(module_name):
     subprocess.run([sys.executable, '-c', f'import {module_name}'], check=True)
```

### Comparing `arelle-release-2.7.1/tests/unit_tests/arelle/test_locale.py` & `arelle-release-2.8.0/tests/unit_tests/arelle/test_locale.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/unit_tests/arelle/test_packagemanager.py` & `arelle-release-2.8.0/tests/unit_tests/arelle/test_packagemanager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/unit_tests/arelle/test_pluginmanager.py` & `arelle-release-2.8.0/tests/unit_tests/arelle/test_pluginmanager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/unit_tests/arelle/test_qname.py` & `arelle-release-2.8.0/tests/unit_tests/arelle/test_qname.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/unit_tests/arelle/test_system_info.py` & `arelle-release-2.8.0/tests/unit_tests/arelle/test_system_info.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/unit_tests/arelle/test_updater.py` & `arelle-release-2.8.0/tests/unit_tests/arelle/test_updater.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/unit_tests/arelle/test_urlutil.py` & `arelle-release-2.8.0/tests/unit_tests/arelle/test_urlutil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/tests/unit_tests/arelle/test_version.py` & `arelle-release-2.8.0/tests/unit_tests/arelle/test_version.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/vms/mac/README.md` & `arelle-release-2.8.0/vms/mac/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.7.1/vms/mac/create-macos-bootable-for-virtualbox.sh` & `arelle-release-2.8.0/vms/mac/create-macos-bootable-for-virtualbox.sh`

 * *Files identical despite different names*

