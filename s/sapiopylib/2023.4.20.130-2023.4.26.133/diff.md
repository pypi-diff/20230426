# Comparing `tmp/sapiopylib-2023.4.20.130.tar.gz` & `tmp/sapiopylib-2023.4.26.133.tar.gz`

## Comparing `sapiopylib-2023.4.20.130.tar` & `sapiopylib-2023.4.26.133.tar`

### file list

```diff
@@ -1,92 +1,93 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/__init__.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/PyCspFieldMap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/__init__.py
--rw-r--r--   0        0        0    36589 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
--rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
--rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/plotly/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    21409 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    45312 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/tests/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/LICENSE
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/README.md
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/pyproject.toml
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36940 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/jarvis/QQPlotComputer.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    45312 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/tests/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/LICENSE
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/README.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/pyproject.toml
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/PKG-INFO
```

### Comparing `sapiopylib-2023.4.20.130/INSTALL.md` & `sapiopylib-2023.4.26.133/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/PyCspFieldMap.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/PyCspFieldMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/plotly/PlotlyCspData.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/PlotlyCspData.py`

 * *Files 0% similar despite different names*

```diff
@@ -707,27 +707,37 @@
     HIST_NORM__FIELD_NAME = "HistNorm"
     NUM_DESIRED_BINS_X__FIELD_NAME = "nbinsx"
     NUM_DESIRED_BINS_Y__FIELD_NAME = "nbinsy"
     Z_MIN__FIELD_NAME = "zmin"
     Z_MAX__FIELD_NAME = "zmax"
     X_AXIS = "XAxis"
     Y_AXIS = "YAxis"
+    FILL__FIELD_NAME = "Fill"
 
     def get_hist_norm_func(self) -> Optional[PlotlyHistNorm]:
         name = self.get_string_value(self.HIST_NORM__FIELD_NAME)
         if name is None:
             return None
         return PlotlyHistNorm[name]
 
     def set_hist_norm_func(self, value: Optional[PlotlyHistNorm]) -> None:
         if value is None:
             self[self.HIST_NORM__FIELD_NAME] = None
         else:
             self[self.HIST_NORM__FIELD_NAME] = value.name
 
+    def get_fill_method(self) -> Optional[str]:
+        return self.get_string_value(self.FILL__FIELD_NAME)
+
+    def set_fill_method(self, value: Optional[PlotlyFill]) -> None:
+        if value is None:
+            self[self.FILL__FIELD_NAME] = None
+        else:
+            self[self.FILL__FIELD_NAME] = value.plotly_id
+
     def get_z_min(self) -> Optional[float]:
         return self.get_float_value(self.Z_MIN__FIELD_NAME)
 
     def get_z_max(self) -> Optional[float]:
         return self.get_float_value(self.Z_MAX__FIELD_NAME)
 
     def set_z_value_range(self, z_min: float, z_max: float):
@@ -1016,9 +1026,8 @@
     def set_grid(self, grid: PlotlyCspGrid) -> None:
         self.set_csp_data(self.GRID_CONFIG, grid)
 
     def get_margins(self) -> Optional[PlotlyCspMargins]:
         return self.get_csp_data(self.MARGINS, PlotlyCspMargins)
 
     def set_margins(self, value: Optional[PlotlyCspMargins]) -> None:
-        self.set_csp_data(self.MARGINS, value)
-
+        self.set_csp_data(self.MARGINS, value)
```

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py`

 * *Files 6% similar despite different names*

```diff
@@ -252,14 +252,15 @@
     @staticmethod
     def from_plotly_id(plotly_id: Optional[str]) -> Optional[PlotlyBarNorm]:
         for v in PlotlyBarNorm:
             if v.plotly_id == plotly_id:
                 return v
         return None
 
+
 class PlotlyAxisCategoryOrder(Enum):
     TRACE = "trace", "Trace of Data"
     CATEGORY_ASC = "category ascending", "Category Ascending"
     CATEGORY_DESC = "category descending", "Category Descending"
     ARRAY = "array", "Custom Order Array (Requires setting category array)"
     TOTAL_ASC = "total ascending", "Total Ascending"
     TOTAL_DESC = "total descending", "Total Descending"
@@ -286,15 +287,15 @@
         for v in PlotlyAxisCategoryOrder:
             if v.plotly_id == plotly_id:
                 return v
         return None
 
 
 class PlotlyAxisRangeMode(Enum):
-    NORMAL= "normal", "Normal"
+    NORMAL = "normal", "Normal"
     INCLUDE_ZERO = "tozero", "Includes 0"
     NON_NEGATIVE = "nonnegative", "Non-Negative"
 
     plotly_id: str
     display_name: str
 
     def __init__(self, plotly_id: str, display_name: str):
@@ -326,7 +327,29 @@
 
     @staticmethod
     def from_plotly_id(plotly_id: Optional[str]) -> Optional[PlotlyAxisType]:
         for v in PlotlyAxisType:
             if v.plotly_id == plotly_id:
                 return v
         return None
+
+
+class PlotlyFill(Enum):
+    NONE = "none"
+    TO_NEXT_Y = "tonexty"
+    TO_NEXT_X = "tonextx"
+    TO_ZERO_Y = "tozeroy"
+    TO_ZERO_X = "tozerox"
+    TO_NEXT = "tonext"
+    TO_SELF = "toself"
+
+    plotly_id: str
+
+    def __init__(self, plotly_id: str):
+        self.plotly_id = plotly_id
+
+    @staticmethod
+    def from_plotly_id(plotly_id: Optional[str]) -> Optional[PlotlyFill]:
+        for v in PlotlyFill:
+            if v.plotly_id == plotly_id:
+                return v
+        return None
```

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         'opacity': opacity,
         'symbol': symbol,
         'color': color,
         'size': size
     }
     if color_array:
         ret['color_array'] = color_array
+    return ret
 
 
 def _get_plotly_line(csp_line: Optional[PlotlyCspLine]):
     if csp_line is None:
         return None
     color: Optional[str] = csp_line.get_line_color()
     dash: Optional[str] = csp_line.get_dash_style()
@@ -53,14 +54,15 @@
         csp_line = csp_series.get_line()
         line = _get_plotly_line(csp_line)
         error_x = csp_series.get_x_error_bar()
         error_y = csp_series.get_y_error_bar()
         box_points = csp_series.get_box_points()
         jitter = csp_series.get_jitter()
         point_pos = csp_series.get_points_position()
+        fill_method = csp_series.get_fill_method()
         fill_color = csp_series.get_fill_color()
         mode = csp_series.get_data_mode()
         color_scale = csp_series.get_color_scale()
         is_reverse_scale = csp_series.is_reverse_scale()
         is_show_scale = csp_series.is_show_scale()
         n_contours = csp_series.get_num_contours()
 
@@ -69,22 +71,21 @@
         if hist_norm_func is not None:
             hist_norm = hist_norm_func.plotly_id
 
         n_bin_x = csp_series.get_num_bins_x()
         n_bin_y = csp_series.get_num_bins_y()
         custom_data_list = csp_series.get_custom_data_list()
         dt: PlotlyDataType = PlotlyDataType.from_plotly_id(csp_series.get_data_type())
-        chart: Optional[BaseTraceType] = None
+        chart: Optional[BaseTraceType]
         if dt == PlotlyDataType.HEAT_MAP:
             chart = Heatmap(x=x, y=y, z=z, customdata=custom_data_list, name=series_name,
                             colorscale=color_scale, reversescale=is_reverse_scale, showscale=is_show_scale)
-            raise CspDataException("Unsupported series data type: " + dt.name)
         elif dt == PlotlyDataType.SCATTER or dt == PlotlyDataType.SCATTER_GL:
             chart = Scatter(x=x, y=y, error_x=error_x, error_y=error_y, customdata=custom_data_list, mode=mode,
-                            fillcolor=fill_color, line=line, marker=marker, name=series_name)
+                            fillcolor=fill_color, fill=fill_method, line=line, marker=marker, name=series_name)
         elif dt == PlotlyDataType.BAR:
             chart = Bar(x=x, y=y, error_x=error_x, error_y=error_y, customdata=custom_data_list,
                         marker=marker, name=series_name)
         elif dt == PlotlyDataType.BOX:
             chart = Box(x=x, y=y, customdata=custom_data_list, jitter=jitter, boxpoints=box_points, pointpos=point_pos,
                         fillcolor=fill_color, line=line, marker=marker, name=series_name)
         elif dt == PlotlyDataType.DENSITY_MAP:
```

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/DataMgmtService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/ELNService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/User.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/User.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/WebhookService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     provides_template_data: Optional[bool]
     source_entry_id: Optional[int]
     attachment_data_base64: Optional[str]
     attachment_file_name: Optional[str]
     temp_data_plugin_path: Optional[str]
 
     def __init__(self, entry_type: ElnEntryType, entry_name: Optional[str],
-                 data_type_name: Optional[str] = None, order: Optional[int] = None, is_shown_in_template: Optional[
+                 data_type_name: Optional[str], order: int, is_shown_in_template: Optional[
                 bool] = None,
                  notebook_experiment_tab_id: Optional[int] = None, column_order: Optional[int] = None,
                  column_span: Optional[int] = None, is_removable: Optional[bool] = None, is_renamable: Optional[
                 bool] = None,
                  is_static_view: Optional[bool] = None, enb_field_set_id: Optional[int] = None,
                  related_entry_set: Optional[List[int]] = None,
                  dependency_set: Optional[List[int]] = None,
```

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/Protocols.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/LICENSE` & `sapiopylib-2023.4.26.133/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.20.130/README.md` & `sapiopylib-2023.4.26.133/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 ## Dependencies
 The following dependencies are required for this package:
 - [requests - Requests is an Apache2 Licensed HTTP library, written in Python, for human beings.](https://pypi.org/project/requests/2.7.0/)
 - [pandas - pandasis a fast, powerful, flexible and easy to use open source data analysis and manipulation tool,  
   built on top of the Python programming language.](https://pandas.pydata.org/)
 - [Flask - A simple framework for building complex web applications.](https://pypi.org/project/Flask/)
 - [buslane - A simple implementation of event-bus system with proper type hinting](https://pypi.org/project/buslane/)
+- [plotly.py - An open-source, interactive data visualization library for Python](https://pypi.org/project/plotly/)
+- [kaleido - Static image export for web-based visualization libraries with zero dependencies](https://pypi.org/project/kaleido/)
 
 ## Documentation
 All documentations, including code examples and installation guide, are provided at [our sapiopylib tutorial github](https://github.com/sapiosciences/sapio-py-tutorials).
 
 ## Getting Help
 If you have support contract with Sapio Sciences, please use our technical support channels. support@sapiosciences.com
```

### Comparing `sapiopylib-2023.4.20.130/pyproject.toml` & `sapiopylib-2023.4.26.133/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2023.04.20.130'
+version='2023.04.26.133'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
-    'requests>=2.28.1', 'pandas>=1.3.0', 'flask>=2.2.0', 'buslane>=0.0.5', 'plotly>=5.14.0', 'kaleido>=0.2.0'
+    'requests>=2.28.1', 'pandas>=1.3.0', 'flask>=2.2.0', 'buslane>=0.0.5', 'plotly>=5.14.0', 'kaleido>=0.2.0',
+    "numpyencoder>=0.3.0"
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Healthcare Industry",
     "Programming Language :: Python :: 3.7",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
```

### Comparing `sapiopylib-2023.4.20.130/PKG-INFO` & `sapiopylib-2023.4.26.133/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapiopylib
-Version: 2023.4.20.130
+Version: 2023.4.26.133
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: buslane>=0.0.5
 Requires-Dist: flask>=2.2.0
 Requires-Dist: kaleido>=0.2.0
+Requires-Dist: numpyencoder>=0.3.0
 Requires-Dist: pandas>=1.3.0
 Requires-Dist: plotly>=5.14.0
 Requires-Dist: requests>=2.28.1
 Description-Content-Type: text/markdown
 
 
 # sapiopylib: Official Sapio Informatics Platform Python API
@@ -69,14 +70,16 @@
 ## Dependencies
 The following dependencies are required for this package:
 - [requests - Requests is an Apache2 Licensed HTTP library, written in Python, for human beings.](https://pypi.org/project/requests/2.7.0/)
 - [pandas - pandasis a fast, powerful, flexible and easy to use open source data analysis and manipulation tool,  
   built on top of the Python programming language.](https://pandas.pydata.org/)
 - [Flask - A simple framework for building complex web applications.](https://pypi.org/project/Flask/)
 - [buslane - A simple implementation of event-bus system with proper type hinting](https://pypi.org/project/buslane/)
+- [plotly.py - An open-source, interactive data visualization library for Python](https://pypi.org/project/plotly/)
+- [kaleido - Static image export for web-based visualization libraries with zero dependencies](https://pypi.org/project/kaleido/)
 
 ## Documentation
 All documentations, including code examples and installation guide, are provided at [our sapiopylib tutorial github](https://github.com/sapiosciences/sapio-py-tutorials).
 
 ## Getting Help
 If you have support contract with Sapio Sciences, please use our technical support channels. support@sapiosciences.com
```

