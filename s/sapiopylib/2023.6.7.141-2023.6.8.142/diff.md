# Comparing `tmp/sapiopylib-2023.6.7.141.tar.gz` & `tmp/sapiopylib-2023.6.8.142.tar.gz`

## Comparing `sapiopylib-2023.6.7.141.tar` & `sapiopylib-2023.6.8.142.tar`

### file list

```diff
@@ -1,97 +1,100 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/__init__.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/PyCspFieldMap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/__init__.py
--rw-r--r--   0        0        0    36940 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/jarvis/QQPlotComputer.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    18143 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/GroupManagerService.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/UserManagerService.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/UserInfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25176 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/CompresionUtil.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    46781 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/tests/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/LICENSE
--rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/README.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/pyproject.toml
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 sapiopylib-2023.6.7.141/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36940 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/jarvis/QQPlotComputer.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    18143 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/GroupManagerService.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/MessengerService.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/UserManagerService.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/Message.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/UserInfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25176 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/CompresionUtil.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    46781 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/tests/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/LICENSE
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/README.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/pyproject.toml
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 sapiopylib-2023.6.8.142/PKG-INFO
```

### Comparing `sapiopylib-2023.6.7.141/INSTALL.md` & `sapiopylib-2023.6.8.142/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/PyCspFieldMap.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/PyCspFieldMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/PlotlyCspData.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/PlotlyCspData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/jarvis/QQPlotComputer.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/jarvis/QQPlotComputer.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/DataMgmtService.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from sapiopylib.rest.DataTypeService import DataTypeManager
 
 from sapiopylib.rest.AccessionService import AccessionManager
 from sapiopylib.rest.CustomReportService import CustomReportManager
 from sapiopylib.rest.DataRecordManagerService import DataRecordManager
 from sapiopylib.rest.ELNService import ElnManager
 from sapiopylib.rest.GroupManagerService import VeloxGroupManager
+from sapiopylib.rest.MessengerService import SapioMessenger
 from sapiopylib.rest.PicklistService import PicklistManager
 from sapiopylib.rest.User import SapioUser
 from sapiopylib.rest.UserManagerService import VeloxUserManager
 
 
 class DataMgmtServer:
     """
@@ -81,7 +82,11 @@
 
     @staticmethod
     def get_group_manager(user: SapioUser) -> VeloxGroupManager:
         """
         Get the group manager that contains info about groups and user memberships into groups.
         """
         return VeloxGroupManager(user)
+
+    @staticmethod
+    def get_messenger(user: SapioUser) -> SapioMessenger:
+        return SapioMessenger(user)
```

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/ELNService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/GroupManagerService.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/GroupManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/User.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/User.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/UserManagerService.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/UserManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/WebhookService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/UserInfo.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/UserInfo.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from sapiopylib.rest.ELNService import ElnManager
 
 from sapiopylib.rest.DataRecordManagerService import DataRecordManager
 
 from sapiopylib.rest.pojo.DataRecord import DataRecord
 
 from sapiopylib.rest.User import SapioUser, UserSessionAdditionalData, parse_session_additional_data
+from sapiopylib.rest.pojo.eln.ElnEntryPosition import ElnEntryPosition
 from sapiopylib.rest.pojo.eln.ElnExperiment import ElnExperiment, ELNExperimentParser
 from sapiopylib.rest.pojo.eln.ExperimentEntry import ExperimentEntry, ExperimentEntryParser
 from sapiopylib.rest.pojo.reportbuilder.VeloxReportBuilder import RbTemplatePopulatorData, VeloxReportBuilderParser
 from sapiopylib.rest.pojo.webhook.ClientCallbackResult import ClientCallbackResultParser, AbstractClientCallbackResult
 from sapiopylib.rest.pojo.webhook.VeloxRules import VeloxTypedRuleResult, ElnEntryRecordResult, VeloxRuleParser
 from sapiopylib.rest.pojo.webhook.WebhookEnums import WebhookEndpointType
 from sapiopylib.rest.utils.Protocols import AbstractProtocol, ElnExperimentProtocol, \
@@ -53,14 +54,16 @@
 
     field_map_list: Optional[List[Dict[str, Any]]]
     field_map: Optional[Dict[str, Any]]
     selected_field_map_index_list: Optional[List[int]]
 
     context_data: str
 
+    entry_position: Optional[ElnEntryPosition]
+
     def __init__(self, user: SapioUser, end_point_type: WebhookEndpointType):
         self.user = user
         self.end_point_type = end_point_type
         self.data_record_manager = DataMgmtServer.get_data_record_manager(user)
         self.eln_manager = DataMgmtServer.get_eln_manager(user)
 
 
@@ -142,14 +145,18 @@
             report_builder_template_populator_data = VeloxReportBuilderParser.parse_template_populator_data(
                 json_dct.get('rbTemplatePopulatorDataPojo'))
 
         field_map_list: Optional[List[Dict[str, Any]]] = json_dct.get('fieldMapList')
         field_map: Optional[Dict[str, Any]] = json_dct.get('fieldMap')
         selected_field_map_index_list: Optional[List[int]] = json_dct.get('selectedFieldMapIdxList')
 
+        entry_position: Optional[ElnEntryPosition] = None
+        if json_dct.get("elnExperimentEntryPositionPojo") is not None:
+            entry_position = ElnEntryPosition.from_json(json_dct.get("elnExperimentEntryPositionPojo"))
+
         ret: SapioWebhookContext = SapioWebhookContext(user, end_point_type)
         ret.context_data = context_data
         ret.data_record = data_record
         ret.base_data_record = base_data_record
         ret.data_record_list = data_record_list
         ret.data_type_name = data_type_name
         ret.data_field_name = data_field_name
@@ -160,14 +167,15 @@
         ret.eln_experiment = notebook_experiment
         ret.client_callback_result = client_callback_result
         ret.is_client_callback_available = is_client_callback_available
         ret.report_builder_template_populator_data = report_builder_template_populator_data
         ret.field_map_list = field_map_list
         ret.field_map = field_map
         ret.selected_field_map_index_list = selected_field_map_index_list
+        ret.entry_position = entry_position
 
         if ret.eln_experiment is not None:
             ret.active_protocol = ElnExperimentProtocol(eln_experiment=ret.eln_experiment, user=ret.user)
             if ret.experiment_entry is not None:
                 ret.active_step = ElnEntryStep(protocol=ret.active_protocol, eln_entry=ret.experiment_entry)
 
         return ret
```

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,20 @@
     VELOXONSAVERULEACTION = 'Velox On Save Rule Action', True
     VELOX_RULE_ACTION = 'Velox Rule Action', True
     VELOXELNRULEACTION = 'Velox ELN Rule Action', True
     NOTEBOOKEXPERIMENTMAINTOOLBAR = 'Notebook Experiment Main Toolbar Button', False
     EXPERIMENTENTRYTOOLBAR = 'Notebook Experiment Entry Toolbar Button', False
     SELECTIONDATAFIELD = 'Selection Data Field', False
     REPORT_BUILDER_TEMPLATE_DATA_POPULATOR = 'Report Builder Template Data Populator Plugin', False
-    SCHEDULEDPLUGIN = 'Scheduled Plugin', False
+    SCHEDULEDPLUGIN = 'Scheduled Plugin', False,
+    ACTIONDATAFIELD = 'Action Data Field', False
+    CALENDAR_EVENT_CLICK_HANDLER = 'Calendar Event Click Handler Plugin', False
+    CUSTOM = 'Custom Plugin Point', False,
+    ACTION_TEXT_FIELD = 'Action Text Field Plugin', False
+    NOTEBOOKEXPERIMENTGRABBER = 'Notebook Experiment Grabber', False
 
     display_name: str
     retry_endpoint: bool
 
     def __init__(self, display_name: str, retry_endpoint: bool):
         self.display_name = display_name
         self.retry_endpoint = retry_endpoint
```

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,43 +22,55 @@
     passed: bool
     display_text: Optional[str]
     list_values: Optional[List[str]]
     directive: Optional[AbstractWebhookDirective]
     client_callback_request: Optional[AbstractClientCallbackRequest]
     refresh_data: bool
     report_builder_template_populator_data: Optional[RbTemplatePopulatorData]
+    auto_invoke_next_row: bool
+    commit_message: Optional[str]
 
     def __init__(self, passed: bool, display_text: Optional[str] = None,
                  list_values: Optional[List[str]] = None,
                  directive: Optional[AbstractWebhookDirective] = None,
                  client_callback_request: Optional[AbstractClientCallbackRequest] = None,
                  refresh_data: bool = False,
-                 report_builder_template_populator_data: Optional[RbTemplatePopulatorData] = None):
+                 report_builder_template_populator_data: Optional[RbTemplatePopulatorData] = None,
+                 auto_invoke_next_row: bool = False, commit_message: Optional[str] = None):
         """
         Returned webhook result from webhook handler to sapio platform.
 
         :param passed: Whether the handler had successfully handled request.
         "False" value may cause transaction to be rolled back.
 
         :param display_text: If this is selection list populator handler, the possible values for user to select in
         selection list.
 
         :param directive: Any place we will navigate player to after receiving this request.
 
         :param client_callback_request: A popup request asking client for more information in UI.
 
         :param refresh_data: Whether forces the client to refresh existing data in the page.
+
+        :param auto_invoke_next_row Whether the client should automatically invoke the plugin for this field on the next
+        row when viewing this field in a table of data.
+        This boolean is only relevant for the ActionTextField plugin point.
+
+        :param commit_message The commit message to be used when committing the transaction after the webhook completes.
+        Only relevant when webhook is configured as transactional.
         """
         self.passed = passed
         self.display_text = display_text
         self.list_values = list_values
         self.directive = directive
         self.client_callback_request = client_callback_request
         self.refresh_data = refresh_data
         self.report_builder_template_populator_data = report_builder_template_populator_data
+        self.auto_invoke_next_row = auto_invoke_next_row
+        self.commit_message = commit_message
 
     def to_json(self) -> Dict[str, Any]:
         directive_pojo = None
         if self.directive is not None:
             directive_pojo = self.directive.to_json()
         client_callback_pojo = None
         if self.client_callback_request is not None:
@@ -69,9 +81,11 @@
         return {
             'passed': self.passed,
             'displayText': self.display_text,
             'listValues': self.list_values,
             'directive': directive_pojo,
             'clientCallbackRequest': client_callback_pojo,
             'refreshData': self.refresh_data,
-            'rbTemplatePopulatorDataPojo': report_builder_populator_pojo
+            'rbTemplatePopulatorDataPojo': report_builder_populator_pojo,
+            'autoInvokeNextRow': self.auto_invoke_next_row,
+            'commitMessage': self.commit_message
         }
```

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/CompresionUtil.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/CompresionUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/Protocols.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2023.6.8.142/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/LICENSE` & `sapiopylib-2023.6.8.142/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/README.md` & `sapiopylib-2023.6.8.142/README.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.6.7.141/pyproject.toml` & `sapiopylib-2023.6.8.142/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2023.06.07.141'
+version='2023.06.08.142'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `sapiopylib-2023.6.7.141/PKG-INFO` & `sapiopylib-2023.6.8.142/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapiopylib
-Version: 2023.6.7.141
+Version: 2023.6.8.142
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
```

