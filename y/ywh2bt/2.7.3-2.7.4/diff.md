# Comparing `tmp/ywh2bt-2.7.3.tar.gz` & `tmp/ywh2bt-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ywh2bt-2.7.3.tar", max compression
+gzip compressed data, was "ywh2bt-2.7.4.tar", max compression
```

## Comparing `ywh2bt-2.7.3.tar` & `ywh2bt-2.7.4.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0     4515 2022-11-14 12:29:40.124367 ywh2bt-2.7.3/README.md
--rw-r--r--   0        0        0     1603 2022-11-14 13:48:49.244133 ywh2bt-2.7.3/pyproject.toml
--rw-r--r--   0        0        0       66 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/__init__.py
--rw-r--r--   0        0        0       47 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/cli/__init__.py
--rw-r--r--   0        0        0       45 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/cli/commands/__init__.py
--rw-r--r--   0        0        0     2323 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/cli/commands/convert.py
--rw-r--r--   0        0        0      865 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/cli/commands/schema.py
--rw-r--r--   0        0        0     1486 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/cli/commands/synchronize.py
--rw-r--r--   0        0        0     1359 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/cli/commands/test.py
--rw-r--r--   0        0        0      680 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/cli/commands/validate.py
--rw-r--r--   0        0        0      147 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/cli/error.py
--rw-r--r--   0        0        0     7318 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/cli/listener.py
--rw-r--r--   0        0        0     6039 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/cli/main.py
--rw-r--r--   0        0        0       66 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/__init__.py
--rw-r--r--   0        0        0       49 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/__init__.py
--rw-r--r--   0        0        0      261 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/client.py
--rw-r--r--   0        0        0       61 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/formatter/__init__.py
--rw-r--r--   0        0        0    11483 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/formatter/formatter.py
--rw-r--r--   0        0        0     3870 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/formatter/markdown.py
--rw-r--r--   0        0        0    12250 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/mapping.py
--rw-r--r--   0        0        0       14 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/models/__init__.py
--rw-r--r--   0        0        0     7865 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/models/report.py
--rw-r--r--   0        0        0     7644 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/tracker.py
--rw-r--r--   0        0        0       95 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/trackers/__init__.py
--rw-r--r--   0        0        0       96 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/trackers/github/__init__.py
--rw-r--r--   0        0        0     9444 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/trackers/github/attachment.py
--rw-r--r--   0        0        0    19792 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/trackers/github/tracker.py
--rw-r--r--   0        0        0    17557 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/trackers/gitlab.py
--rw-r--r--   0        0        0       94 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/trackers/jira/__init__.py
--rw-r--r--   0        0        0     6706 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/trackers/jira/formatter.py
--rw-r--r--   0        0        0    18588 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/trackers/jira/tracker.py
--rw-r--r--   0        0        0      100 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/trackers/servicenow/__init__.py
--rw-r--r--   0        0        0     3512 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/trackers/servicenow/formatter.py
--rw-r--r--   0        0        0     3190 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/trackers/servicenow/model.py
--rw-r--r--   0        0        0    31810 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/trackers/servicenow/tracker.py
--rw-r--r--   0        0        0    13560 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/api/yeswehack.py
--rw-r--r--   0        0        0       80 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/configuration/__init__.py
--rw-r--r--   0        0        0    21298 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/configuration/attribute.py
--rw-r--r--   0        0        0     2667 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/configuration/error.py
--rw-r--r--   0        0        0      327 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/configuration/exportable.py
--rw-r--r--   0        0        0      206 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/configuration/headers.py
--rw-r--r--   0        0        0     4298 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/configuration/root.py
--rw-r--r--   0        0        0     5889 2022-11-14 12:29:40.144368 ywh2bt-2.7.3/ywh2bt/core/configuration/subtypable.py
--rw-r--r--   0        0        0     2282 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/configuration/tracker.py
--rw-r--r--   0        0        0       47 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/configuration/trackers/__init__.py
--rw-r--r--   0        0        0     4846 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/configuration/trackers/github.py
--rw-r--r--   0        0        0     2568 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/configuration/trackers/gitlab.py
--rw-r--r--   0        0        0     3242 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/configuration/trackers/jira.py
--rw-r--r--   0        0        0     2604 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/configuration/trackers/servicenow.py
--rw-r--r--   0        0        0      606 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/configuration/validatable.py
--rw-r--r--   0        0        0     3724 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/configuration/validator.py
--rw-r--r--   0        0        0    11522 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/configuration/yeswehack.py
--rw-r--r--   0        0        0       56 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/converter/__init__.py
--rw-r--r--   0        0        0    29722 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/converter/html2jira.py
--rw-r--r--   0        0        0     8931 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/converter/jira2markdown.py
--rw-r--r--   0        0        0     3447 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/core.py
--rw-r--r--   0        0        0       50 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/crypt/__init__.py
--rw-r--r--   0        0        0     1229 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/crypt/decrypt.py
--rw-r--r--   0        0        0     1200 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/crypt/encrypt.py
--rw-r--r--   0        0        0      100 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/crypt/error.py
--rw-r--r--   0        0        0     1501 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/crypt/key.py
--rw-r--r--   0        0        0     3624 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/error.py
--rw-r--r--   0        0        0      102 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/exceptions.py
--rw-r--r--   0        0        0       17 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/factories/__init__.py
--rw-r--r--   0        0        0     5449 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/factories/tracker_clients.py
--rw-r--r--   0        0        0     1892 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/factories/yeswehack_api_clients.py
--rw-r--r--   0        0        0     4741 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/html.py
--rw-r--r--   0        0        0      495 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/listener.py
--rw-r--r--   0        0        0     3864 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/loader.py
--rw-r--r--   0        0        0      799 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/markdown.py
--rw-r--r--   0        0        0       44 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/schema/__init__.py
--rw-r--r--   0        0        0      160 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/schema/error.py
--rw-r--r--   0        0        0     7830 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/schema/json.py
--rw-r--r--   0        0        0     5396 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/schema/markdown.py
--rw-r--r--   0        0        0      263 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/schema/protocol.py
--rw-r--r--   0        0        0     4950 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/schema/text.py
--rw-r--r--   0        0        0      807 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/serde.py
--rw-r--r--   0        0        0       72 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/serializers/__init__.py
--rw-r--r--   0        0        0     1197 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/serializers/json.py
--rw-r--r--   0        0        0     1324 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/serializers/yaml.py
--rw-r--r--   0        0        0       57 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/state/__init__.py
--rw-r--r--   0        0        0     2315 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/state/decrypt.py
--rw-r--r--   0        0        0     2095 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/state/encrypt.py
--rw-r--r--   0        0        0      100 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/state/error.py
--rw-r--r--   0        0        0      294 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/state/state.py
--rw-r--r--   0        0        0       89 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/synchronizer/__init__.py
--rw-r--r--   0        0        0      185 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/synchronizer/error.py
--rw-r--r--   0        0        0     2785 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/synchronizer/listener.py
--rw-r--r--   0        0        0    36284 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/synchronizer/synchronizer.py
--rw-r--r--   0        0        0       78 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/tester/__init__.py
--rw-r--r--   0        0        0      165 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/tester/error.py
--rw-r--r--   0        0        0     1915 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/tester/listener.py
--rw-r--r--   0        0        0     5153 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/core/tester/tester.py
--rw-r--r--   0        0        0       44 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/gui/__init__.py
--rw-r--r--   0        0        0       22 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/gui/dialog/__init__.py
--rw-r--r--   0        0        0     1495 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/gui/dialog/error.py
--rw-r--r--   0        0        0     2444 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/gui/dialog/file.py
--rw-r--r--   0        0        0     2043 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/gui/dialog/schema.py
--rw-r--r--   0        0        0      627 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/gui/hashing.py
--rw-r--r--   0        0        0     1588 2022-11-14 12:29:40.148368 ywh2bt-2.7.3/ywh2bt/gui/main.py
--rw-r--r--   0        0        0    10953 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/hide.png
--rw-r--r--   0        0        0     9963 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/show.png
--rw-r--r--   0        0        0     8215 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration-2x.png
--rw-r--r--   0        0        0     6601 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration.png
--rw-r--r--   0        0        0    11199 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration-2x.png
--rw-r--r--   0        0        0     7837 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration.png
--rw-r--r--   0        0        0     9711 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration-2x.png
--rw-r--r--   0        0        0     7608 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration.png
--rw-r--r--   0        0        0     2375 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration-2x.png
--rw-r--r--   0        0        0     1551 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration.png
--rw-r--r--   0        0        0     8133 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration-2x.png
--rw-r--r--   0        0        0     6361 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration.png
--rw-r--r--   0        0        0     8133 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/icons/ywh2bt.png
--rw-r--r--   0        0        0      103 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/translations/fr_FR.qm
--rw-r--r--   0        0        0      311 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/resources/translations/fr_FR.ts
--rw-r--r--   0        0        0   238701 2022-11-14 13:49:38.248759 ywh2bt-2.7.3/ywh2bt/gui/resources.py
--rw-r--r--   0        0        0     1184 2022-11-14 13:49:32.820689 ywh2bt-2.7.3/ywh2bt/gui/resources.qrc
--rw-r--r--   0        0        0      134 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/settings.py
--rw-r--r--   0        0        0     1640 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/update_resources_file.py
--rw-r--r--   0        0        0       22 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/__init__.py
--rw-r--r--   0        0        0       44 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/__init__.py
--rw-r--r--   0        0        0      342 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/attributes_container_dict_entry.py
--rw-r--r--   0        0        0     2980 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/attributes_container_dict_entry_widget.py
--rw-r--r--   0        0        0    12960 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/attributes_container_dict_widget.py
--rw-r--r--   0        0        0     7032 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/attributes_container_list_widget.py
--rw-r--r--   0        0        0    18891 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/attributes_container_widget.py
--rw-r--r--   0        0        0    11074 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/exportable_dict_widget.py
--rw-r--r--   0        0        0    10553 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/exportable_list_widget.py
--rw-r--r--   0        0        0      803 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/constants.py
--rw-r--r--   0        0        0     2958 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/hinted_check_box_widget.py
--rw-r--r--   0        0        0     5390 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/logs_widget.py
--rw-r--r--   0        0        0    17657 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/main_window.py
--rw-r--r--   0        0        0     7547 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/root_configuration_entry.py
--rw-r--r--   0        0        0    17635 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/root_configuration_widget.py
--rw-r--r--   0        0        0    13117 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/root_configurations_widget.py
--rw-r--r--   0        0        0     3012 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/secret_line_edit_widget.py
--rw-r--r--   0        0        0      483 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/tab_widget_helper.py
--rw-r--r--   0        0        0       51 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/thread/__init__.py
--rw-r--r--   0        0        0     7883 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/thread/synchronizer.py
--rw-r--r--   0        0        0     5260 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/thread/tester.py
--rw-r--r--   0        0        0      444 2022-11-14 12:29:40.152368 ywh2bt-2.7.3/ywh2bt/gui/widgets/typing.py
--rw-r--r--   0        0        0      635 2022-11-14 12:29:40.156368 ywh2bt-2.7.3/ywh2bt/version.py
--rw-r--r--   0        0        0     6837 1970-01-01 00:00:00.000000 ywh2bt-2.7.3/setup.py
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 ywh2bt-2.7.3/PKG-INFO
+-rw-r--r--   0        0        0     4739 2023-04-26 12:52:27.026394 ywh2bt-2.7.4/README.md
+-rw-r--r--   0        0        0     1603 2023-04-26 13:05:06.939498 ywh2bt-2.7.4/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/cli/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2323 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/cli/commands/convert.py
+-rw-r--r--   0        0        0      865 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/cli/commands/schema.py
+-rw-r--r--   0        0        0     1486 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/cli/commands/synchronize.py
+-rw-r--r--   0        0        0     1359 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/cli/commands/test.py
+-rw-r--r--   0        0        0      680 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/cli/commands/validate.py
+-rw-r--r--   0        0        0      147 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/cli/error.py
+-rw-r--r--   0        0        0     7318 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/cli/listener.py
+-rw-r--r--   0        0        0     6039 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/cli/main.py
+-rw-r--r--   0        0        0       66 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/__init__.py
+-rw-r--r--   0        0        0       49 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/api/__init__.py
+-rw-r--r--   0        0        0      261 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/api/client.py
+-rw-r--r--   0        0        0       61 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/api/formatter/__init__.py
+-rw-r--r--   0        0        0    11483 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/api/formatter/formatter.py
+-rw-r--r--   0        0        0     3870 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/api/formatter/markdown.py
+-rw-r--r--   0        0        0    12250 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/api/mapping.py
+-rw-r--r--   0        0        0       14 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/api/models/__init__.py
+-rw-r--r--   0        0        0     7865 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/api/models/report.py
+-rw-r--r--   0        0        0     7644 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/api/tracker.py
+-rw-r--r--   0        0        0       95 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/api/trackers/__init__.py
+-rw-r--r--   0        0        0       96 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/api/trackers/github/__init__.py
+-rw-r--r--   0        0        0     9444 2023-04-26 12:52:27.042394 ywh2bt-2.7.4/ywh2bt/core/api/trackers/github/attachment.py
+-rw-r--r--   0        0        0    19792 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/api/trackers/github/tracker.py
+-rw-r--r--   0        0        0    17557 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/api/trackers/gitlab.py
+-rw-r--r--   0        0        0       94 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/api/trackers/jira/__init__.py
+-rw-r--r--   0        0        0     6706 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/api/trackers/jira/formatter.py
+-rw-r--r--   0        0        0    18588 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/api/trackers/jira/tracker.py
+-rw-r--r--   0        0        0      100 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/api/trackers/servicenow/__init__.py
+-rw-r--r--   0        0        0     3512 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/api/trackers/servicenow/formatter.py
+-rw-r--r--   0        0        0     3190 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/api/trackers/servicenow/model.py
+-rw-r--r--   0        0        0    31810 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/api/trackers/servicenow/tracker.py
+-rw-r--r--   0        0        0    13703 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/api/yeswehack.py
+-rw-r--r--   0        0        0       80 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/__init__.py
+-rw-r--r--   0        0        0    21298 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/attribute.py
+-rw-r--r--   0        0        0     2667 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/error.py
+-rw-r--r--   0        0        0      327 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/exportable.py
+-rw-r--r--   0        0        0      206 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/headers.py
+-rw-r--r--   0        0        0     4298 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/root.py
+-rw-r--r--   0        0        0     5889 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/subtypable.py
+-rw-r--r--   0        0        0     2282 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/tracker.py
+-rw-r--r--   0        0        0       47 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/trackers/__init__.py
+-rw-r--r--   0        0        0     4846 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/trackers/github.py
+-rw-r--r--   0        0        0     2568 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/trackers/gitlab.py
+-rw-r--r--   0        0        0     3242 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/trackers/jira.py
+-rw-r--r--   0        0        0     2604 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/trackers/servicenow.py
+-rw-r--r--   0        0        0      606 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/validatable.py
+-rw-r--r--   0        0        0     3724 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/validator.py
+-rw-r--r--   0        0        0    11522 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/configuration/yeswehack.py
+-rw-r--r--   0        0        0       56 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/converter/__init__.py
+-rw-r--r--   0        0        0    29722 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/converter/html2jira.py
+-rw-r--r--   0        0        0     8931 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/converter/jira2markdown.py
+-rw-r--r--   0        0        0     3447 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/core.py
+-rw-r--r--   0        0        0       50 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/crypt/__init__.py
+-rw-r--r--   0        0        0     1229 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/crypt/decrypt.py
+-rw-r--r--   0        0        0     1200 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/crypt/encrypt.py
+-rw-r--r--   0        0        0      100 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/crypt/error.py
+-rw-r--r--   0        0        0     1501 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/crypt/key.py
+-rw-r--r--   0        0        0     3624 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/error.py
+-rw-r--r--   0        0        0      102 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/exceptions.py
+-rw-r--r--   0        0        0       17 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/factories/__init__.py
+-rw-r--r--   0        0        0     5449 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/factories/tracker_clients.py
+-rw-r--r--   0        0        0     1892 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/factories/yeswehack_api_clients.py
+-rw-r--r--   0        0        0     4741 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/html.py
+-rw-r--r--   0        0        0      495 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/listener.py
+-rw-r--r--   0        0        0     3864 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/loader.py
+-rw-r--r--   0        0        0      799 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/markdown.py
+-rw-r--r--   0        0        0       44 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/schema/__init__.py
+-rw-r--r--   0        0        0      160 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/schema/error.py
+-rw-r--r--   0        0        0     7830 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/schema/json.py
+-rw-r--r--   0        0        0     5396 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/schema/markdown.py
+-rw-r--r--   0        0        0      263 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/schema/protocol.py
+-rw-r--r--   0        0        0     4950 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/schema/text.py
+-rw-r--r--   0        0        0      807 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/serde.py
+-rw-r--r--   0        0        0       72 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/serializers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/serializers/json.py
+-rw-r--r--   0        0        0     1324 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/serializers/yaml.py
+-rw-r--r--   0        0        0       57 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/state/__init__.py
+-rw-r--r--   0        0        0     2315 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/state/decrypt.py
+-rw-r--r--   0        0        0     2095 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/state/encrypt.py
+-rw-r--r--   0        0        0      100 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/state/error.py
+-rw-r--r--   0        0        0      294 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/state/state.py
+-rw-r--r--   0        0        0       89 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/synchronizer/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/synchronizer/error.py
+-rw-r--r--   0        0        0     2785 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/synchronizer/listener.py
+-rw-r--r--   0        0        0    37758 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/synchronizer/synchronizer.py
+-rw-r--r--   0        0        0       78 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/tester/__init__.py
+-rw-r--r--   0        0        0      165 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/tester/error.py
+-rw-r--r--   0        0        0     1915 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/tester/listener.py
+-rw-r--r--   0        0        0     5153 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/core/tester/tester.py
+-rw-r--r--   0        0        0       44 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/gui/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/gui/dialog/__init__.py
+-rw-r--r--   0        0        0     1495 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/gui/dialog/error.py
+-rw-r--r--   0        0        0     2444 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/gui/dialog/file.py
+-rw-r--r--   0        0        0     2043 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/gui/dialog/schema.py
+-rw-r--r--   0        0        0      627 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/gui/hashing.py
+-rw-r--r--   0        0        0     1588 2023-04-26 12:52:27.046394 ywh2bt-2.7.4/ywh2bt/gui/main.py
+-rw-r--r--   0        0        0    10953 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/hide.png
+-rw-r--r--   0        0        0     9963 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/show.png
+-rw-r--r--   0        0        0     8215 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration-2x.png
+-rw-r--r--   0        0        0     6601 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration.png
+-rw-r--r--   0        0        0    11199 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration-2x.png
+-rw-r--r--   0        0        0     7837 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration.png
+-rw-r--r--   0        0        0     9711 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration-2x.png
+-rw-r--r--   0        0        0     7608 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration.png
+-rw-r--r--   0        0        0     2375 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration-2x.png
+-rw-r--r--   0        0        0     1551 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration.png
+-rw-r--r--   0        0        0     8133 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration-2x.png
+-rw-r--r--   0        0        0     6361 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration.png
+-rw-r--r--   0        0        0     8133 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/icons/ywh2bt.png
+-rw-r--r--   0        0        0      103 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/translations/fr_FR.qm
+-rw-r--r--   0        0        0      311 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/resources/translations/fr_FR.ts
+-rw-r--r--   0        0        0   238662 2023-04-26 13:05:48.443339 ywh2bt-2.7.4/ywh2bt/gui/resources.py
+-rw-r--r--   0        0        0     1184 2023-04-26 13:05:46.191348 ywh2bt-2.7.4/ywh2bt/gui/resources.qrc
+-rw-r--r--   0        0        0      134 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/settings.py
+-rw-r--r--   0        0        0     1640 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/update_resources_file.py
+-rw-r--r--   0        0        0       22 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/__init__.py
+-rw-r--r--   0        0        0      342 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/attributes_container_dict_entry.py
+-rw-r--r--   0        0        0     2980 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/attributes_container_dict_entry_widget.py
+-rw-r--r--   0        0        0    12960 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/attributes_container_dict_widget.py
+-rw-r--r--   0        0        0     7032 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/attributes_container_list_widget.py
+-rw-r--r--   0        0        0    18891 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/attributes_container_widget.py
+-rw-r--r--   0        0        0    11074 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/exportable_dict_widget.py
+-rw-r--r--   0        0        0    10553 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/exportable_list_widget.py
+-rw-r--r--   0        0        0      803 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/constants.py
+-rw-r--r--   0        0        0     2958 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/hinted_check_box_widget.py
+-rw-r--r--   0        0        0     5390 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/logs_widget.py
+-rw-r--r--   0        0        0    17657 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/main_window.py
+-rw-r--r--   0        0        0     7547 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/root_configuration_entry.py
+-rw-r--r--   0        0        0    17635 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/root_configuration_widget.py
+-rw-r--r--   0        0        0    13117 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/root_configurations_widget.py
+-rw-r--r--   0        0        0     3012 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/secret_line_edit_widget.py
+-rw-r--r--   0        0        0      483 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/tab_widget_helper.py
+-rw-r--r--   0        0        0       51 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/thread/__init__.py
+-rw-r--r--   0        0        0     7883 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/thread/synchronizer.py
+-rw-r--r--   0        0        0     5260 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/thread/tester.py
+-rw-r--r--   0        0        0      444 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/gui/widgets/typing.py
+-rw-r--r--   0        0        0      955 2023-04-26 12:52:27.050394 ywh2bt-2.7.4/ywh2bt/size.py
+-rw-r--r--   0        0        0      635 2023-04-26 12:52:27.054394 ywh2bt-2.7.4/ywh2bt/version.py
+-rw-r--r--   0        0        0     6587 1970-01-01 00:00:00.000000 ywh2bt-2.7.4/PKG-INFO
```

### Comparing `ywh2bt-2.7.3/README.md` & `ywh2bt-2.7.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 - servicenow
 
 ## Changelog
 
 - v2.7:
     - added synchronization of "fix verification" logs when "Upload status updates" is checked
     - fixed an issue with jira when scope contains special markdown characters
+    - fixed an issue when "Download bug trackers comments" feedback option is activated
+      and bug tracker attachments do not meet platform attachments requirements (unacceptable mime-type, maximum allowed size exceeded)
 - v2.6:
     - added work around bug trackers maximum size allowed for the text of the issues/comments (content put in Markdown file attachment when necessary)
 - v2.5:
     - added Personal Access Token (PAT) authentication
     - removed OAuth authentication
 - v2.4:
     - added option to prevent recreation of issues that were created by a previous synchronization
```

### Comparing `ywh2bt-2.7.3/pyproject.toml` & `ywh2bt-2.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ywh2bt"
-version = "2.7.3"
+version = "2.7.4"
 description = "ywh2bt - YesWeHack to Bug Tracker"
 readme = "README.md"
 authors = ["m.honel <m.honel@yeswehack.com>"]
 maintainers = ["YesWeHack <project@yeswehack.com>"]
 repository = "https://github.com/yeswehack/ywh2bugtracker"
 classifiers = [
     "Environment :: Console",
```

### Comparing `ywh2bt-2.7.3/ywh2bt/cli/commands/convert.py` & `ywh2bt-2.7.4/ywh2bt/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/cli/commands/schema.py` & `ywh2bt-2.7.4/ywh2bt/cli/commands/schema.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/cli/commands/synchronize.py` & `ywh2bt-2.7.4/ywh2bt/cli/commands/synchronize.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/cli/commands/test.py` & `ywh2bt-2.7.4/ywh2bt/cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/cli/commands/validate.py` & `ywh2bt-2.7.4/ywh2bt/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/cli/listener.py` & `ywh2bt-2.7.4/ywh2bt/cli/listener.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/cli/main.py` & `ywh2bt-2.7.4/ywh2bt/cli/main.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/formatter/formatter.py` & `ywh2bt-2.7.4/ywh2bt/core/api/formatter/formatter.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/formatter/markdown.py` & `ywh2bt-2.7.4/ywh2bt/core/api/formatter/markdown.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/mapping.py` & `ywh2bt-2.7.4/ywh2bt/core/api/mapping.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/models/report.py` & `ywh2bt-2.7.4/ywh2bt/core/api/models/report.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/tracker.py` & `ywh2bt-2.7.4/ywh2bt/core/api/tracker.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/trackers/github/attachment.py` & `ywh2bt-2.7.4/ywh2bt/core/api/trackers/github/attachment.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/trackers/github/tracker.py` & `ywh2bt-2.7.4/ywh2bt/core/api/trackers/github/tracker.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/trackers/gitlab.py` & `ywh2bt-2.7.4/ywh2bt/core/api/trackers/gitlab.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/trackers/jira/formatter.py` & `ywh2bt-2.7.4/ywh2bt/core/api/trackers/jira/formatter.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/trackers/jira/tracker.py` & `ywh2bt-2.7.4/ywh2bt/core/api/trackers/jira/tracker.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/trackers/servicenow/formatter.py` & `ywh2bt-2.7.4/ywh2bt/core/api/trackers/servicenow/formatter.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/trackers/servicenow/model.py` & `ywh2bt-2.7.4/ywh2bt/core/api/trackers/servicenow/model.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/trackers/servicenow/tracker.py` & `ywh2bt-2.7.4/ywh2bt/core/api/trackers/servicenow/tracker.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/api/yeswehack.py` & `ywh2bt-2.7.4/ywh2bt/core/api/yeswehack.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     Log,
     Report,
 )
 from ywh2bt.core.configuration.yeswehack import (
     YesWeHackConfiguration,
 )
 from ywh2bt.core.exceptions import CoreException
+from ywh2bt.version import __VERSION__
 
 
 class YesWeHackApiClientError(CoreException):
     """A YesWeHack API client error."""
 
 
 class YesWeHackApiClient(TestableApiClient):
@@ -79,14 +80,17 @@
             client = YesWeHackRawApiClient(
                 api_url=self._normalize_api_url(
                     api_url=cast(str, configuration.api_url),
                 ),
                 pat=configuration.pat,
                 verify=configuration.verify,
                 lazy=True,
+                headers={
+                    'User-Agent': f'ywh2bt/{__VERSION__}',
+                },
             )
         except (YesWeHackRawAPiError, requests.RequestException) as e:
             raise YesWeHackApiClientError('Unable to initialize YesWeHack API client') from e
         return client
 
     def _normalize_api_url(
         self,
```

### Comparing `ywh2bt-2.7.3/ywh2bt/core/configuration/attribute.py` & `ywh2bt-2.7.4/ywh2bt/core/configuration/attribute.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/configuration/error.py` & `ywh2bt-2.7.4/ywh2bt/core/configuration/error.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/configuration/root.py` & `ywh2bt-2.7.4/ywh2bt/core/configuration/root.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/configuration/subtypable.py` & `ywh2bt-2.7.4/ywh2bt/core/configuration/subtypable.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/configuration/tracker.py` & `ywh2bt-2.7.4/ywh2bt/core/configuration/tracker.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/configuration/trackers/github.py` & `ywh2bt-2.7.4/ywh2bt/core/configuration/trackers/github.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/configuration/trackers/gitlab.py` & `ywh2bt-2.7.4/ywh2bt/core/configuration/trackers/gitlab.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/configuration/trackers/jira.py` & `ywh2bt-2.7.4/ywh2bt/core/configuration/trackers/jira.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/configuration/trackers/servicenow.py` & `ywh2bt-2.7.4/ywh2bt/core/configuration/trackers/servicenow.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/configuration/validatable.py` & `ywh2bt-2.7.4/ywh2bt/core/configuration/validatable.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/configuration/validator.py` & `ywh2bt-2.7.4/ywh2bt/core/configuration/validator.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/configuration/yeswehack.py` & `ywh2bt-2.7.4/ywh2bt/core/configuration/yeswehack.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/converter/html2jira.py` & `ywh2bt-2.7.4/ywh2bt/core/converter/html2jira.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/converter/jira2markdown.py` & `ywh2bt-2.7.4/ywh2bt/core/converter/jira2markdown.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/core.py` & `ywh2bt-2.7.4/ywh2bt/core/core.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/crypt/decrypt.py` & `ywh2bt-2.7.4/ywh2bt/core/crypt/decrypt.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/crypt/encrypt.py` & `ywh2bt-2.7.4/ywh2bt/core/crypt/encrypt.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/crypt/key.py` & `ywh2bt-2.7.4/ywh2bt/core/crypt/key.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/error.py` & `ywh2bt-2.7.4/ywh2bt/core/error.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/factories/tracker_clients.py` & `ywh2bt-2.7.4/ywh2bt/core/factories/tracker_clients.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/factories/yeswehack_api_clients.py` & `ywh2bt-2.7.4/ywh2bt/core/factories/yeswehack_api_clients.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/html.py` & `ywh2bt-2.7.4/ywh2bt/core/html.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/loader.py` & `ywh2bt-2.7.4/ywh2bt/core/loader.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/markdown.py` & `ywh2bt-2.7.4/ywh2bt/core/markdown.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/schema/json.py` & `ywh2bt-2.7.4/ywh2bt/core/schema/json.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/schema/markdown.py` & `ywh2bt-2.7.4/ywh2bt/core/schema/markdown.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/schema/text.py` & `ywh2bt-2.7.4/ywh2bt/core/schema/text.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/serde.py` & `ywh2bt-2.7.4/ywh2bt/core/serde.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/serializers/json.py` & `ywh2bt-2.7.4/ywh2bt/core/serializers/json.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/serializers/yaml.py` & `ywh2bt-2.7.4/ywh2bt/core/serializers/yaml.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/state/decrypt.py` & `ywh2bt-2.7.4/ywh2bt/core/state/decrypt.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/state/encrypt.py` & `ywh2bt-2.7.4/ywh2bt/core/state/encrypt.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/synchronizer/listener.py` & `ywh2bt-2.7.4/ywh2bt/core/synchronizer/listener.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/synchronizer/synchronizer.py` & `ywh2bt-2.7.4/ywh2bt/core/synchronizer/synchronizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     RewardLog,
     StatusUpdateLog,
     TrackerUpdateLog,
     TrackingStatusLog,
 )
 from ywh2bt.core.api.tracker import (
     SendLogsResult,
+    TrackerAttachment,
     TrackerClient,
     TrackerClientError,
     TrackerIssue,
     TrackerIssueComment,
     TrackerIssueComments,
     TrackerIssueState,
 )
@@ -72,14 +73,15 @@
     SynchronizerEndSendReportEvent,
     SynchronizerEvent,
     SynchronizerListener,
     SynchronizerStartEvent,
     SynchronizerStartFetchReportsEvent,
     SynchronizerStartSendReportEvent,
 )
+from ywh2bt.size import sizeof_fmt_si
 
 
 class Synchronizer:
     """A class used for data synchronisation between YesWeHack and trackers."""
 
     _configuration: RootConfiguration
     _yes_we_hack_api_clients_factory: YesWeHackApiClientsAbstractFactory
@@ -620,37 +622,38 @@
             ) from issue_comments_error
 
     def _download_comment(
         self,
         tracker_issue: TrackerIssue,
         tracker_comment: TrackerIssueComment,
     ) -> None:
+        failed_attachments = {}
         attachments = {}
         for attachment_key, attachment in tracker_comment.attachments.items():
             try:
                 uploaded_attachment = self._yeswehack_client.post_report_attachment(
                     report=self._report,
                     filename=attachment.filename,
                     file_content=attachment.content,
                     file_type=attachment.mime_type,
                 )
-            except YesWeHackApiClientError as upload_attachment_error:
-                raise SynchronizerError(
-                    f'Unable to upload attachment {attachment.filename} for report #{self._report.report_id}',
-                ) from upload_attachment_error
+            except YesWeHackApiClientError:
+                failed_attachments[attachment_key] = attachment
+                continue
             attachments[attachment_key] = uploaded_attachment
         try:
             self._yeswehack_client.post_report_tracker_message(
                 report=self._report,
                 tracker_name=self._tracker_name,
                 issue_id=tracker_issue.issue_id,
                 issue_url=tracker_issue.issue_url,
                 comment=self._message_formatter.format_download_comment(
                     comment=tracker_comment,
                     attachments=attachments,
+                    failed_attachments=failed_attachments,
                 ),
                 attachments=[uploaded_attachment.name for attachment_key, uploaded_attachment in attachments.items()],
             )
         except YesWeHackApiClientError as tracker_message_error:
             raise SynchronizerError(
                 f'Unable to download comment {tracker_comment.comment_id} for report #{self._report.report_id}',
             ) from tracker_message_error
@@ -779,21 +782,23 @@
         """
 
     @abstractmethod
     def format_download_comment(
         self,
         comment: TrackerIssueComment,
         attachments: Dict[str, Attachment],
+        failed_attachments: Dict[str, TrackerAttachment],
     ) -> str:
         """
         Format a downloaded comment.
 
         Args:
             comment: a comment
             attachments: a dict of attachments
+            failed_attachments: a dict of tracker attachments that failed to be uploaded
         """
 
     @abstractmethod
     def format_status_update_comment(
         self,
         comment: str,
     ) -> str:
@@ -831,14 +836,23 @@
         + '\n'
         + 'Date: ${date}'
         + '\n'
         + 'Author: ${author}'
         + '\n\n'
         + '${comment}',
     )
+    _failed_attachments_template: Template = Template(
+        '**YWH2BT note:**'
+        + '\n*There was an issue while uploading the following attachments from the bugtracker*:'
+        + '\n\n'
+        + '${attachments}',
+    )
+    _failed_attachment_template: Template = Template(
+        '- ${filename} (size=${size}, mime=${mimetype})',
+    )
     _status_update_comment_template: Template = Template(
         '${comment}',
     )
 
     def format_tracking_status_update_message(
         self,
         tracker_type: str,
@@ -905,33 +919,50 @@
             issue_status=issue_status,
         )
 
     def format_download_comment(
         self,
         comment: TrackerIssueComment,
         attachments: Dict[str, Attachment],
+        failed_attachments: Dict[str, TrackerAttachment],
     ) -> str:
         """
         Format a downloaded comment.
 
         Args:
             comment: a comment
             attachments: a dict of attachments
+            failed_attachments: a dict of tracker attachments that failed to be uploaded
 
         Returns:
             a formatted comment
         """
-        return self._download_comment_template.substitute(
+        formatted_comment = self._download_comment_template.substitute(
             date=comment.created_at,
             author=comment.author,
             comment=markdown_to_ywh(
                 message=comment.body,
                 attachments=attachments,
             ),
         )
+        if failed_attachments:
+            formatted_attachments = []
+            for _attachment_key, failed_attachment in failed_attachments.items():
+                formatted_attachments.append(
+                    self._failed_attachment_template.substitute(
+                        filename=failed_attachment.filename,
+                        mimetype=failed_attachment.mime_type,
+                        size=sizeof_fmt_si(len(failed_attachment.content), precision=2),
+                    ),
+                )
+            formatted_failed_attachments = self._failed_attachments_template.substitute(
+                attachments='\n'.join(formatted_attachments),
+            )
+            formatted_comment = f'{formatted_comment}\n\n{formatted_failed_attachments}'
+        return formatted_comment
 
     def format_status_update_comment(
         self,
         comment: str,
     ) -> str:
         """
         Format a report status update comment.
```

### Comparing `ywh2bt-2.7.3/ywh2bt/core/tester/listener.py` & `ywh2bt-2.7.4/ywh2bt/core/tester/listener.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/core/tester/tester.py` & `ywh2bt-2.7.4/ywh2bt/core/tester/tester.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/dialog/error.py` & `ywh2bt-2.7.4/ywh2bt/gui/dialog/error.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/dialog/file.py` & `ywh2bt-2.7.4/ywh2bt/gui/dialog/file.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/dialog/schema.py` & `ywh2bt-2.7.4/ywh2bt/gui/dialog/schema.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/hashing.py` & `ywh2bt-2.7.4/ywh2bt/gui/hashing.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/main.py` & `ywh2bt-2.7.4/ywh2bt/gui/main.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/hide.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/hide.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/show.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/show.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration-2x.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration-2x.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration-2x.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration-2x.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration-2x.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration-2x.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration-2x.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration-2x.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration-2x.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration-2x.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources/icons/ywh2bt.png` & `ywh2bt-2.7.4/ywh2bt/gui/resources/icons/ywh2bt.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources.py` & `ywh2bt-2.7.4/ywh2bt/gui/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,45 +2,14 @@
 # Created by: object code
 # Created by: The Resource Compiler for Qt version 5.15.2
 # WARNING! All changes made in this file will be lost!
 
 from PySide2 import QtCore
 
 qt_resource_data = b"\
-\x00\x00\x017\
-<\
-?xml version=\x221.\
-0\x22 encoding=\x22utf\
--8\x22?>\x0a<!DOCTYPE \
-TS><TS version=\x22\
-1.1\x22 language=\x22f\
-r_FR\x22>\x0a<context>\
-\x0a    <name>MainW\
-indow</name>\x0a   \
- <message>\x0a     \
-   <location fil\
-ename=\x22main_wind\
-ow.py\x22 line=\x2299\x22\
-/>\x0a        <sour\
-ce>&amp;File</so\
-urce>\x0a        <t\
-ranslation>&amp;\
-Fichier</transla\
-tion>\x0a    </mess\
-age>\x0a</context>\x0a\
-</TS>\x0a\
-\x00\x00\x00g\
-<\
-\xb8d\x18\xca\xef\x9c\x95\xcd!\x1c\xbf`\xa1\xbd\xdd\xa7\
-\x00\x00\x00\x05fr_FRB\x00\x00\x00\x08\x00*\
-\xd0%\x00\x00\x00\x00i\x00\x00\x004\x03\x00\x00\x00\x10\
-\x00&\x00F\x00i\x00c\x00h\x00i\x00e\x00r\
-\x08\x00\x00\x00\x00\x06\x00\x00\x00\x05&File\x07\
-\x00\x00\x00\x0aMainWindow\x01\x88\
-\x00\x00\x00\x02\x03\x01\
 \x00\x00&\xeb\
 \x89\
 PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
 \x00\x02\x00\x00\x00\x02\x00\x08\x03\x00\x00\x00\xc3\xa6$\xc8\
 \x00\x00\x00\x03sBIT\x08\x08\x08\xdb\xe1O\xe0\x00\
 \x00\x00\x09pHYs\x00\x00\x17\xdc\x00\x00\x17\xdc\x01\
 \x19\x04WV\x00\x00\x00\x19tEXtSoft\
@@ -3245,14 +3214,429 @@
 \xc0\xfb@\x96\xb0\xd1\x115%4%\xf6t\xf6\xdc\x98\
 \x89H\x9c7\x80\xcf\x01\x0fm$4E\xb8\xed\x06\x01\
 (\xe7\xe4\x0a\xce\x93\xadD}\x10\x89\x9ddr\xe4\x91\
 \xac\xec\xc9gn<\x8e\xf3\x22\xf0\x15\x22}F\xb0]\
 \xbf\x0b\xa6\x9f\xf3 \x81\xe4`\x17\xbaR\xddz\xe3\xfd\
 o\xedO\x05aLT\xe7\x01\x15\x85\x00\x00\x00\x00I\
 END\xaeB`\x82\
+\x00\x00\x19\xc9\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
+\x00\x00\x04=zTXtRaw prof\
+ile type exif\x00\x00x\
+\xda\xadVm\x96\xac(\x0c\xfd\x9fU\xcc\x12L\xc2\xe7\
+rP\xe4\x9c\xd9\xc1,\x7fn@m\xb5>\xba\xba\xdf\
+\xd3S\x04\x02\x84\xe4\xde\x04\x8b\xd6\xff\xfem\xf4\x0f\x1e\
+\xe1)\x90\xf31\x85\x1c\xc2\x84\xc7e\x97\xa5\xa0\x93\xa6\
+\xf1\x94\xde\xf2\xe4z\xdb\x1f\xd9\xa60\xbe\xe8\xe9\x98\x10\
+\xa8\x14R\xc70\x85m\xfd\xae\xe7\xc3\xc0\x10\x05=\x7f\
+2\x94\x96mb\xbeNd\xb7\xd9O7C\xdb\xc9j\
+\x1eY\xbfn\x86\xf2fHeL\xf0f\xa0\x8c\xb0\xa6\
+\x90S<\x870\xafC\xd6=\x924~d\x8dKW\
+\xb7\x1f\xc6\x11\xe8U\x8fsTdU\xd6\x09\xad\xa8\x0c\
+\x07\xb4\xffH\x8bM\xf46\xc8P\x17\xf5\x18Y\xbb{\
+\x02@\x9e\xe14\x9d\xbc\xa2;+G\x8f_\xe8o\xa4\
+h\x18z\x82\xe2\x0af8\xe4S=\xfb\x9b~3H\
+\x1d\xe2\xd3\xc9\xba\x1c'_\xf4-\x1eG\x5c@\xb6_\
+k5Qk\xeb\x88\xae\xb8\x00H\xc3\x16\xd4\x1eJ\xef\
+a\xe1\x0c\xc8\xb5o\x0bx\xcd\xa8G?\xf67\xe3M\
+\x84\xec]@y\x9d\x96i\xc6\xbbpf\x01\xfa\x8d\x1d\
+W.\xdcx\xedr\xe1\x05.:Y%B\x8a,\xa2\
+]\x974J\x96\xc5Xcu\xf6r\x93\xa8Y\xab&\
+0\xb7\x80^\x85V\x0e_\xb8\x9f\x9b\xfbq\x0b'\x1c\
+\x5c\x19+\x85a\x8c-\x15\xc8\x9a\xbf\xf1\xbe4\xd4\x9a\
+\xa5<\xf3\x94\x0e\xac\xe0\x97X\x12\xc2\x0dc\xceZ\xac\
+\x02!\xdc\xf6<\xf2\x1d\xe0\xfd\xbd?\xc6\xab\x82A\xdf\
+aN\x08\xb0L\xf301{\xder\xcb\xf2H;\xd1\
+\x8a\x85\x1er\xd4\x1a\xc7\xba\x19\x00D8\xdb\xc3\x19V\
+00\x05V\xcf\x81\xa7(\x12\x99\x81c\x02?\x05\x86\
+\x92\xa8\x93\x19\x14\xb0\xf7R\xe1\xa58E\xb5DIb\
+gcO\xe4\xbeV\xbc\x0c5\xee,\x10\xe15h\x04\
+5Y\x0b\xb8r\xb8\xd8\x90?\xd1%\xe4P\xf1\xea\x9d\
+\xf7>\xf8\xe8\x93\xcf\xbe\x04\x0d.\xf8\x10B\x0cv\xf9\
+\x95\xa8\xd1E\x1fC\x8c1\xc5\x1cK\xd2\xe4\x92O!\
+\xc5\x94(\xe5T\xb2d\xc5\xe5\xe8s\xc81\xa7\x9cs\
+)8\xb4\xc0r\xc1\xee\x82\x05\xa5\xcc2\xeb\xecf?\
+\x879\xcei\xcesY\x90>\x8b[\xfc\x12\x96\xb8$\
+Z\xf2R\xaaT\xad\xb8'j\xa8\xb1\xa6\x9akYy\
+E*\xadn\xf5kX\xe3\x9a\xd6\xbc\x96\x86Tk\xda\
+\x5c\xf3-\xb4\xd8R\xcb\xad\x1c\xac1\x0dZ\x1f\xde\xcf\
+Y\xe3\x9d5\xe9L\xd9\xc2x\xb0\x86\xad1\xee&\xd8\
+\xae\x13o\x9c\x811q\x0c\xc6\xa31\x80\x84\x16\xe3l\
+J\xec\x9c\x90Qg\x9cMYP\x15^\xe0\xa57r\
+*\x1bc`\xd0\xad,\xbe\xf1\xc1\xdd\x17s\x17\xde\xc8\
+\xb9?\xe2Mv\xe6\xc8\xa8\xfb\x1b\xcc\x91Q\xf7\x82\xb9\
+G\xde\x9e\xb0V\xedk\xb3LJ\x9d!+C\x03u\
+R\x94\x1f\x16\xac\xa9H*\xf6Q{)k@\x17_\
+\xad\xae\xe2\xe4\x89\x9d\xb7O\x99\x7f/9\xab\xf3a\xb6\
+.\xfc\x1f\xbbw+C\xd2]q\x978\xf9\xf0$t\
+\xab\xde\xbe\xa2\x0f\x92^M<\x95\xc1U\xf6\xa5z\xf8\
+\x87b\xbf\xc4KW\x00f_\xce\x81\x7f\x16w\x97\xf4\
+\xe9\xc2\x13P\xf0\x0b\x19\x7f\xc3\x81\x14>\xbc\x04\x00[\
+\xb0\xf1\xa3\xd0\x1f1\xea\x00p\xa9o`\xea\xfe%\xc3\
+a\x96\xb0\xa1A\xcf\xe1\xe8Q\xd8F\x84\x00\xde:\xe3\
+Sw~t\xef\x81\xa9\xa7cN\xbb\xfd\xdb\xf4\xcb\xb0\
+\xe1\xf7A_\xcfMzG\xcf\xd9\xaf7\xa9&_\xa1\
+=q\xb5|\x9f\x83\x17IO\x9d\x95\xefk\xed.\xe9\
+\xaa\xb8\x10\xf1\xa3\xb4\xa4\x1f\x01\xf1F\xd2\x1f\x01s\xaa\
+=\xfa\x15 \x0fr\xb6<\xfaE\x91\x8e\xd2\xb9$\x08\
+\xfd\x1e\x98\x9e\x87\x07\x0e\xf4\xf9et\x03\xc6\xdc\xd0Q\
+\x0a\x16\x1f}\x0e\xc4\xfd\x96\xbe\xc6K\xa7r\x18\xf8\xdb\
+a\x07\x03\x9f\xf3G_\xb7\xc2v\xf6\x08\xfd\xc7\xd8\xd3\
+\xed\xc2{\x9eK\xaf\xee\xa8SY\xd1c\x1a\xfd\xa2L\
+\x80\x0b=\x94\xc7\xf5\x1e\xbb8w\xe7k\xc0?\xba\xd4\
+\xb7=a\xe9G~\xe1\x04\xfa\xa6\x5c\xdf\xf8wE\x8a\
+^\xdd@\x1fy4\xbe\x04\xdd\x11\xba{2\xaf\xad\xf5\
+\xf1\xa4\xebO\xc6d\x0a\x0e\xa6XG\x08\x8f#\xc4\xd6\
+f\xfb\x87\x82\x7f*\xc9|~6\xa21\xb4@^[\
+:\x8dv'\x1eF\xf4n\x12\x7f\x97Z\xcd\xb8\xd8\xff\
+\x07z\xfa\xca_!\xc5\x8b\x88\x00\x00\x01\x84iCC\
+PICC profile\x00\x00x\x9c\
+}\x91=H\xc3@\x1c\xc5_S\xa5R*\x8av\x10\
+q\xc8P\x9d,\x14\x15q\xd4*\x14\xa1B\xa8\x15Z\
+u0\xb9\xf4\x0b\x9a4$).\x8e\x82k\xc1\xc1\x8f\
+\xc5\xaa\x83\x8b\xb3\xae\x0e\xae\x82 \xf8\x01\xe2\xe4\xe8\xa4\
+\xe8\x22%\xfe/)\xb4\x88\xf5\xe0\xb8\x1f\xef\xee=\xee\
+\xde\x01B\xbd\xcc4\xab+\x06h\xbam\xa6\x12q1\
+\x93]\x15\x03\xaf\x08\xa2\x1f\x03\x88\xc1/3\xcb\x98\x93\
+\xa4$:\x8e\xaf{\xf8\xf8z\x17\xe5Y\x9d\xcf\xfd9\
+z\xd5\x9c\xc5\x00\x9fH<\xcb\x0c\xd3&\xde \x9e\xde\
+\xb4\x0d\xce\xfb\xc4aV\x94U\xe2s\xe2q\x93.H\
+\xfc\xc8u\xc5\xe37\xce\x05\x97\x05\x9e\x196\xd3\xa9y\
+\xe20\xb1Xhc\xa5\x8dY\xd1\xd4\x88\xa7\x88#\xaa\
+\xa6S\xbe\x90\xf1X\xe5\xbc\xc5Y+WY\xf3\x9e\xfc\
+\x85\xa1\x9c\xbe\xb2\xccu\x9a#H`\x11K\x90 B\
+A\x15%\x94a#J\xabN\x8a\x85\x14\xed\xc7;\xf8\
+\x87]\xbfD.\x85\x5c%0r,\xa0\x02\x0d\xb2\xeb\
+\x07\xff\x83\xdf\xddZ\xf9\xc9\x09/)\x14\x07\xba_\x1c\
+\xe7c\x14\x08\xec\x02\x8d\x9a\xe3|\x1f;N\xe3\x04\xf0\
+?\x03Wz\xcb_\xa9\x033\x9f\xa4\xd7ZZ\xe4\x08\
+\xe8\xdb\x06.\xae[\x9a\xb2\x07\x5c\xee\x00CO\x86l\
+\xca\xae\xe4\xa7)\xe4\xf3\xc0\xfb\x19}S\x16\x18\xbc\x05\
+\x82k^o\xcd}\x9c>\x00i\xea*y\x03\x1c\x1c\
+\x02c\x05\xca^\xef\xf0\xee\x9e\xf6\xde\xfe=\xd3\xec\xef\
+\x07W\xdar\x9c\x98\xfc\x90>\x00\x00\x10XiTX\
+tXML:com.adobe.x\
+mp\x00\x00\x00\x00\x00<?xpacket\
+ begin=\x22\xef\xbb\xbf\x22 id=\
+\x22W5M0MpCehiHzreS\
+zNTczkc9d\x22?>\x0a<x:\
+xmpmeta xmlns:x=\
+\x22adobe:ns:meta/\x22\
+ x:xmptk=\x22XMP Co\
+re 4.4.0-Exiv2\x22>\
+\x0a <rdf:RDF xmlns\
+:rdf=\x22http://www\
+.w3.org/1999/02/\
+22-rdf-syntax-ns\
+#\x22>\x0a  <rdf:Descr\
+iption rdf:about\
+=\x22\x22\x0a    xmlns:ip\
+tcExt=\x22http://ip\
+tc.org/std/Iptc4\
+xmpExt/2008-02-2\
+9/\x22\x0a    xmlns:xm\
+pMM=\x22http://ns.a\
+dobe.com/xap/1.0\
+/mm/\x22\x0a    xmlns:\
+stEvt=\x22http://ns\
+.adobe.com/xap/1\
+.0/sType/Resourc\
+eEvent#\x22\x0a    xml\
+ns:stRef=\x22http:/\
+/ns.adobe.com/xa\
+p/1.0/sType/Reso\
+urceRef#\x22\x0a    xm\
+lns:plus=\x22http:/\
+/ns.useplus.org/\
+ldf/xmp/1.0/\x22\x0a  \
+  xmlns:GIMP=\x22ht\
+tp://www.gimp.or\
+g/xmp/\x22\x0a    xmln\
+s:dc=\x22http://pur\
+l.org/dc/element\
+s/1.1/\x22\x0a    xmln\
+s:tiff=\x22http://n\
+s.adobe.com/tiff\
+/1.0/\x22\x0a    xmlns\
+:xmp=\x22http://ns.\
+adobe.com/xap/1.\
+0/\x22\x0a   xmpMM:Doc\
+umentID=\x22xmp.did\
+:E5178A2B99A011E\
+29A15BC1046A8904\
+D\x22\x0a   xmpMM:Inst\
+anceID=\x22xmp.iid:\
+00063360-f1d7-4f\
+09-8a41-bcb20a92\
+0a27\x22\x0a   xmpMM:O\
+riginalDocumentI\
+D=\x22xmp.did:12f20\
+251-8048-4234-bd\
+37-6117502ec313\x22\
+\x0a   GIMP:API=\x222.\
+0\x22\x0a   GIMP:Platf\
+orm=\x22Linux\x22\x0a   G\
+IMP:TimeStamp=\x221\
+602874314737681\x22\
+\x0a   GIMP:Version\
+=\x222.10.22\x22\x0a   dc\
+:Format=\x22image/p\
+ng\x22\x0a   tiff:Orie\
+ntation=\x221\x22\x0a   x\
+mp:CreatorTool=\x22\
+GIMP 2.10\x22>\x0a   <\
+iptcExt:Location\
+Created>\x0a    <rd\
+f:Bag/>\x0a   </ipt\
+cExt:LocationCre\
+ated>\x0a   <iptcEx\
+t:LocationShown>\
+\x0a    <rdf:Bag/>\x0a\
+   </iptcExt:Loc\
+ationShown>\x0a   <\
+iptcExt:ArtworkO\
+rObject>\x0a    <rd\
+f:Bag/>\x0a   </ipt\
+cExt:ArtworkOrOb\
+ject>\x0a   <iptcEx\
+t:RegistryId>\x0a  \
+  <rdf:Bag/>\x0a   \
+</iptcExt:Regist\
+ryId>\x0a   <xmpMM:\
+History>\x0a    <rd\
+f:Seq>\x0a     <rdf\
+:li\x0a      stEvt:\
+action=\x22saved\x22\x0a \
+     stEvt:chang\
+ed=\x22/\x22\x0a      stE\
+vt:instanceID=\x22x\
+mp.iid:825a5a7d-\
+c3bc-49ee-80d2-1\
+4d4aaaff7f7\x22\x0a   \
+   stEvt:softwar\
+eAgent=\x22Gimp 2.1\
+0 (Linux)\x22\x0a     \
+ stEvt:when=\x22+02\
+:00\x22/>\x0a    </rdf\
+:Seq>\x0a   </xmpMM\
+:History>\x0a   <xm\
+pMM:DerivedFrom\x0a\
+    stRef:docume\
+ntID=\x22xmp.did:E5\
+178A2999A011E29A\
+15BC1046A8904D\x22\x0a\
+    stRef:instan\
+ceID=\x22xmp.iid:E5\
+178A2899A011E29A\
+15BC1046A8904D\x22/\
+>\x0a   <plus:Image\
+Supplier>\x0a    <r\
+df:Seq/>\x0a   </pl\
+us:ImageSupplier\
+>\x0a   <plus:Image\
+Creator>\x0a    <rd\
+f:Seq/>\x0a   </plu\
+s:ImageCreator>\x0a\
+   <plus:Copyrig\
+htOwner>\x0a    <rd\
+f:Seq/>\x0a   </plu\
+s:CopyrightOwner\
+>\x0a   <plus:Licen\
+sor>\x0a    <rdf:Se\
+q/>\x0a   </plus:Li\
+censor>\x0a  </rdf:\
+Description>\x0a </\
+rdf:RDF>\x0a</x:xmp\
+meta>\x0a          \
+                \
+                \
+                \
+                \
+                \
+          \x0a     \
+                \
+                \
+                \
+                \
+                \
+               \x0a\
+                \
+                \
+                \
+                \
+                \
+                \
+    \x0a           \
+                \
+                \
+                \
+                \
+                \
+         \x0a      \
+                \
+                \
+                \
+                \
+                \
+              \x0a \
+                \
+                \
+                \
+                \
+                \
+                \
+   \x0a            \
+                \
+                \
+                \
+                \
+                \
+        \x0a       \
+                \
+                \
+                \
+                \
+                \
+             \x0a  \
+                \
+                \
+                \
+                \
+                \
+                \
+  \x0a             \
+                \
+                \
+                \
+                \
+                \
+       \x0a        \
+                \
+                \
+                \
+                \
+                \
+            \x0a   \
+                \
+                \
+                \
+                \
+                \
+                \
+ \x0a              \
+                \
+                \
+                \
+                \
+                \
+      \x0a         \
+                \
+                \
+                \
+                \
+                \
+           \x0a    \
+                \
+                \
+                \
+                \
+                \
+                \
+\x0a               \
+                \
+                \
+                \
+                \
+                \
+     \x0a          \
+                \
+                \
+                \
+                \
+                \
+          \x0a     \
+                \
+                \
+                \
+                \
+                \
+               \x0a\
+                \
+                \
+                \
+                \
+                \
+                \
+    \x0a           \
+                \
+                \
+                \
+                \
+                \
+         \x0a      \
+                \
+     \x0a<?xpacket \
+end=\x22w\x22?>\xc2(:\xc2\x00\x00\x00\
+\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\xa7\x93\x00\
+\x00\x00\x09pHYs\x00\x00\x0b\x13\x00\x00\x0b\x13\x01\
+\x00\x9a\x9c\x18\x00\x00\x00\x07tIME\x07\xe4\x0a\x10\
+\x1236\x7f\xdb;\xbd\x00\x00\x03\x19IDATX\
+\xc3\xcd\xd7]\x88UU\x14\x07\xf0\xdf=M\x94\xe1X\
+J\xf7\xdc+AM\x14\x05\x81\x86\x99=\xd5CCT\
+H8\xa4=\x04=6}=\x04\x81\x05a\x0f\x15\xc1\
+\x18hR\x11\x14A\x8f\xbd\x8dZI\x10$\x06\xa1\xf4\
+P\xd3@>XQ\x0eZ\x92\xfbl\xb1\xfc \xec\xc3\
+\xa6\x97=t\xbc\x9c3\x9d\xb9\xdd\x81\x16\x9c\x87\xb3\xd6\
+\xde\xff\xf5_\xeb\xec\xb5\xf6:-\x0d\xa5\xd3\xce\xaf\xc4\
+\x18\xee\xc4j\x5c\x8b\xa5\xc9|\x163\xf8\x0a\x9f\xe0\xfd\
+\x10\x8b\x13Mp[\x0d\x1c\xaf\xc1\xb3\xd8\x88\xa1\x86|\
+\xff\xc4.\xbc\x1cb1\xdd\x17\x81N;\xbf\x1c\xdb\xf1\
+p\x13\xa252\x8bw\xf0t\x88\xc5\xa9\xc6\x04R\xd4\
+;S\x9a\x07!3\xd8T\x95\x8dV\x85\xf3Q\xec\xc6\
+2\x83\x95\xd3\xb8?\xc4b_-\x81N;_\x8b}\
+\x8b\xe0\xbcLb4\xc4bjN\x91\x95\x9c/\xc7d\
+\x8f\xf3C\xe90\x9d\xee\xd3\xd9\xae\x841'\xcb0\x99\
+|]H\x00\xaf`\xa4\x07d\x22\xc4b\x13r\x8c#\
+\x94\xca\xee >M\xcf\xc1\xa4\x93\xd6\x8c#O{'\
+z0G\x92\xaf\x7f>A\xa7\x9d\xdf\x8a\xcf+\xa2X\
+\x1bb\xf1eOe\xac\xc4\xb7!\x16\x7f\xf5|\xbe\x0c\
+7\xe0\xa7\xf2\x89\xef\xb4\xf3[0U\x81\xbd.\xc4\xe2\
+\x8b\xb9\xba\xdeR\x93\xc6\x8b\xca/\x09\xb8\xb2\x9c\x12\xa1\
+\xaf\xff\x0d\xa3$[\xb01\xeb\xb4\xf3.6\xd4,\xba\
+i\x00\x07\xaf\x0ecC\xa7\x9dw\xb3\xd4^\xabX\xfe\
+\x88=\x03 \xb0\x07?\xd4df,\xc3h\xcd\xc6\xe7\
+C,N\xfeW\xef\x09\xe3\x85\x1a\xf3h\x86U\x15\x86\
+\xf3\xa9\x13\x0eJv&\xcc^Y\x95U\x94\x1e\x1c\xab\
+\xeb\xdd}f\xe1\x14\x8eU\x98F2,\xa90\xfc\xbe\
+\x08]\xf0\x8f\x0a\xdd\x92\xac\xee2\x5c\x04\x02y\x952\
+\xc3\x99\x0a\xfdp\xa7\x9d\xe7\x83\xf2\x9c\xb0\x86+Lg\
+2\x1c\xae\xd9w\xef\x00\xa3\xaf\xc3:\x9c\xd5\xb4I\xd8\
+\xdci\xe7C\x03\x88~\x08\x9bk\xccS\x19\xf6\xd6\x18\
+Wc\xdb\x00\xa2\xdf\x96\xb0\xaado\xab\xd3\xce\x87q\
+\x1c\x97\xd5,\x9a\xc4\x93!\x16\xc7\x17\x18\xf9J\xbc\x8e\
+\x07j\x96\xfc\x8a\xee\xdcm\xf8&\x1e/1\xfe\x10/\
+\xe1\x8eR\x09\xbd\x87\x8f1\x8d\xe9\x10\x8b\xf3\x15\xa9^\
+\x87\x9bq7\xee\xc3\xc5\xf3p|+\xc4\xe2\x899\x02\
+W\xe3\x1b\x5c\x9a\x06\xc9g\xf0F\xba\xebo\xeb\xd9\xb8\
+;\xcdw\xb3=\x04Z\xc96\xd6 A\xe7pc\x88\
+\xc5\xd1,u\xaa\xa3\xd8Z\x9a\x11\xb6c\x0d\x1e\xac\xb8\
+Hv\xf4:O\x18\xb3\xd8\xd1\xf0\x0bmM>/\x98\
+\x88&p\xa0\xf4\xfeb\x88\xc5L:@\xe3x\x0e\xf7\
+\xe0\xb3y\x80\x0f5p~\xa0<%\xf5\x0e\xa5]\xec\
+\xc7uI\xf5T\x88\xc5k\x0b8xW\xe0\xe7y\x96\
+|\x8f\xdb\xcb\x07\xbaj,\xbf&\x95\xe6\xf5I\xb5\x1f\
+\x1f \xa2\x8bWC,\xce\xf5A\xe0;\xdc\x15bq\
+\xa4\xc9\x8f\xc9\x0a\xbc[\xd3\xc1\x96\x87X\xfc\xb2@\x02\
+\x1f\xe1\xa1\xaa\xf9\x22\x9bg\x88X\x8fGR\xe4\xfd\xca\
+\x09<\x8a\xf5u\xc3M\x93\x9f\xd3\xa5x,=+p\
+U\x88\xc5o5k/I\xf7\xfeI\xbc\x9dj\xfd\xac\
+\xff\xb3\xfc\x0dTj\x06\x16\x12.K\x86\x00\x00\x00\x00\
+IEND\xaeB`\x82\
 \x00\x00+\xbf\
 \x89\
 PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
 \x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
 \x00\x00\x12\xc6zTXtRaw prof\
 ile type exif\x00\x00x\
 \xda\xad\x9akv\xe38\xb2\x84\xffc\x15\xb3\x04\xe2\x0d\
@@ -3947,429 +4331,14 @@
 `Q\xdf\x04J\x0f\xd0\xc15`\xbfj\x98\x07\x1b\xb5\
 '\xa5\x91\x00\xa8\x86\xf9)\xd0\xcf<\xbe\xa5\xa3@\xfd\
 xs\x1e\xa5\x1d\xe8\xe0\x94\xe8\xdb\x0f6rO\x0d\x05\
 @\x80p\x0e\xd8D\x17\xaf&:\xf3\xb9\xf8\xc2<t\
 sP\xe4\xf6\x9f\xb9\x9d\xec\xe6\x1b\xe9\xcdW\x0f\xf4\xed\
 b\xd6fm\xd6fm\x9a\xec?\x02\x8bq57f\
 \x16\xda\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x19\xc9\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
-\x00\x00\x04=zTXtRaw prof\
-ile type exif\x00\x00x\
-\xda\xadVm\x96\xac(\x0c\xfd\x9fU\xcc\x12L\xc2\xe7\
-rP\xe4\x9c\xd9\xc1,\x7fn@m\xb5>\xba\xba\xdf\
-\xd3S\x04\x02\x84\xe4\xde\x04\x8b\xd6\xff\xfem\xf4\x0f\x1e\
-\xe1)\x90\xf31\x85\x1c\xc2\x84\xc7e\x97\xa5\xa0\x93\xa6\
-\xf1\x94\xde\xf2\xe4z\xdb\x1f\xd9\xa60\xbe\xe8\xe9\x98\x10\
-\xa8\x14R\xc70\x85m\xfd\xae\xe7\xc3\xc0\x10\x05=\x7f\
-2\x94\x96mb\xbeNd\xb7\xd9O7C\xdb\xc9j\
-\x1eY\xbfn\x86\xf2fHeL\xf0f\xa0\x8c\xb0\xa6\
-\x90S<\x870\xafC\xd6=\x924~d\x8dKW\
-\xb7\x1f\xc6\x11\xe8U\x8fsTdU\xd6\x09\xad\xa8\x0c\
-\x07\xb4\xffH\x8bM\xf46\xc8P\x17\xf5\x18Y\xbb{\
-\x02@\x9e\xe14\x9d\xbc\xa2;+G\x8f_\xe8o\xa4\
-h\x18z\x82\xe2\x0af8\xe4S=\xfb\x9b~3H\
-\x1d\xe2\xd3\xc9\xba\x1c'_\xf4-\x1eG\x5c@\xb6_\
-k5Qk\xeb\x88\xae\xb8\x00H\xc3\x16\xd4\x1eJ\xef\
-a\xe1\x0c\xc8\xb5o\x0bx\xcd\xa8G?\xf67\xe3M\
-\x84\xec]@y\x9d\x96i\xc6\xbbpf\x01\xfa\x8d\x1d\
-W.\xdcx\xedr\xe1\x05.:Y%B\x8a,\xa2\
-]\x974J\x96\xc5Xcu\xf6r\x93\xa8Y\xab&\
-0\xb7\x80^\x85V\x0e_\xb8\x9f\x9b\xfbq\x0b'\x1c\
-\x5c\x19+\x85a\x8c-\x15\xc8\x9a\xbf\xf1\xbe4\xd4\x9a\
-\xa5<\xf3\x94\x0e\xac\xe0\x97X\x12\xc2\x0dc\xceZ\xac\
-\x02!\xdc\xf6<\xf2\x1d\xe0\xfd\xbd?\xc6\xab\x82A\xdf\
-aN\x08\xb0L\xf301{\xder\xcb\xf2H;\xd1\
-\x8a\x85\x1er\xd4\x1a\xc7\xba\x19\x00D8\xdb\xc3\x19V\
-00\x05V\xcf\x81\xa7(\x12\x99\x81c\x02?\x05\x86\
-\x92\xa8\x93\x19\x14\xb0\xf7R\xe1\xa58E\xb5DIb\
-gcO\xe4\xbeV\xbc\x0c5\xee,\x10\xe15h\x04\
-5Y\x0b\xb8r\xb8\xd8\x90?\xd1%\xe4P\xf1\xea\x9d\
-\xf7>\xf8\xe8\x93\xcf\xbe\x04\x0d.\xf8\x10B\x0cv\xf9\
-\x95\xa8\xd1E\x1fC\x8c1\xc5\x1cK\xd2\xe4\x92O!\
-\xc5\x94(\xe5T\xb2d\xc5\xe5\xe8s\xc81\xa7\x9cs\
-)8\xb4\xc0r\xc1\xee\x82\x05\xa5\xcc2\xeb\xecf?\
-\x879\xcei\xcesY\x90>\x8b[\xfc\x12\x96\xb8$\
-Z\xf2R\xaaT\xad\xb8'j\xa8\xb1\xa6\x9akYy\
-E*\xadn\xf5kX\xe3\x9a\xd6\xbc\x96\x86Tk\xda\
-\x5c\xf3-\xb4\xd8R\xcb\xad\x1c\xac1\x0dZ\x1f\xde\xcf\
-Y\xe3\x9d5\xe9L\xd9\xc2x\xb0\x86\xad1\xee&\xd8\
-\xae\x13o\x9c\x811q\x0c\xc6\xa31\x80\x84\x16\xe3l\
-J\xec\x9c\x90Qg\x9cMYP\x15^\xe0\xa57r\
-*\x1bc`\xd0\xad,\xbe\xf1\xc1\xdd\x17s\x17\xde\xc8\
-\xb9?\xe2Mv\xe6\xc8\xa8\xfb\x1b\xcc\x91Q\xf7\x82\xb9\
-G\xde\x9e\xb0V\xedk\xb3LJ\x9d!+C\x03u\
-R\x94\x1f\x16\xac\xa9H*\xf6Q{)k@\x17_\
-\xad\xae\xe2\xe4\x89\x9d\xb7O\x99\x7f/9\xab\xf3a\xb6\
-.\xfc\x1f\xbbw+C\xd2]q\x978\xf9\xf0$t\
-\xab\xde\xbe\xa2\x0f\x92^M<\x95\xc1U\xf6\xa5z\xf8\
-\x87b\xbf\xc4KW\x00f_\xce\x81\x7f\x16w\x97\xf4\
-\xe9\xc2\x13P\xf0\x0b\x19\x7f\xc3\x81\x14>\xbc\x04\x00[\
-\xb0\xf1\xa3\xd0\x1f1\xea\x00p\xa9o`\xea\xfe%\xc3\
-a\x96\xb0\xa1A\xcf\xe1\xe8Q\xd8F\x84\x00\xde:\xe3\
-Sw~t\xef\x81\xa9\xa7cN\xbb\xfd\xdb\xf4\xcb\xb0\
-\xe1\xf7A_\xcfMzG\xcf\xd9\xaf7\xa9&_\xa1\
-=q\xb5|\x9f\x83\x17IO\x9d\x95\xefk\xed.\xe9\
-\xaa\xb8\x10\xf1\xa3\xb4\xa4\x1f\x01\xf1F\xd2\x1f\x01s\xaa\
-=\xfa\x15 \x0fr\xb6<\xfaE\x91\x8e\xd2\xb9$\x08\
-\xfd\x1e\x98\x9e\x87\x07\x0e\xf4\xf9et\x03\xc6\xdc\xd0Q\
-\x0a\x16\x1f}\x0e\xc4\xfd\x96\xbe\xc6K\xa7r\x18\xf8\xdb\
-a\x07\x03\x9f\xf3G_\xb7\xc2v\xf6\x08\xfd\xc7\xd8\xd3\
-\xed\xc2{\x9eK\xaf\xee\xa8SY\xd1c\x1a\xfd\xa2L\
-\x80\x0b=\x94\xc7\xf5\x1e\xbb8w\xe7k\xc0?\xba\xd4\
-\xb7=a\xe9G~\xe1\x04\xfa\xa6\x5c\xdf\xf8wE\x8a\
-^\xdd@\x1fy4\xbe\x04\xdd\x11\xba{2\xaf\xad\xf5\
-\xf1\xa4\xebO\xc6d\x0a\x0e\xa6XG\x08\x8f#\xc4\xd6\
-f\xfb\x87\x82\x7f*\xc9|~6\xa21\xb4@^[\
-:\x8dv'\x1eF\xf4n\x12\x7f\x97Z\xcd\xb8\xd8\xff\
-\x07z\xfa\xca_!\xc5\x8b\x88\x00\x00\x01\x84iCC\
-PICC profile\x00\x00x\x9c\
-}\x91=H\xc3@\x1c\xc5_S\xa5R*\x8av\x10\
-q\xc8P\x9d,\x14\x15q\xd4*\x14\xa1B\xa8\x15Z\
-u0\xb9\xf4\x0b\x9a4$).\x8e\x82k\xc1\xc1\x8f\
-\xc5\xaa\x83\x8b\xb3\xae\x0e\xae\x82 \xf8\x01\xe2\xe4\xe8\xa4\
-\xe8\x22%\xfe/)\xb4\x88\xf5\xe0\xb8\x1f\xef\xee=\xee\
-\xde\x01B\xbd\xcc4\xab+\x06h\xbam\xa6\x12q1\
-\x93]\x15\x03\xaf\x08\xa2\x1f\x03\x88\xc1/3\xcb\x98\x93\
-\xa4$:\x8e\xaf{\xf8\xf8z\x17\xe5Y\x9d\xcf\xfd9\
-z\xd5\x9c\xc5\x00\x9fH<\xcb\x0c\xd3&\xde \x9e\xde\
-\xb4\x0d\xce\xfb\xc4aV\x94U\xe2s\xe2q\x93.H\
-\xfc\xc8u\xc5\xe37\xce\x05\x97\x05\x9e\x196\xd3\xa9y\
-\xe20\xb1Xhc\xa5\x8dY\xd1\xd4\x88\xa7\x88#\xaa\
-\xa6S\xbe\x90\xf1X\xe5\xbc\xc5Y+WY\xf3\x9e\xfc\
-\x85\xa1\x9c\xbe\xb2\xccu\x9a#H`\x11K\x90 B\
-A\x15%\x94a#J\xabN\x8a\x85\x14\xed\xc7;\xf8\
-\x87]\xbfD.\x85\x5c%0r,\xa0\x02\x0d\xb2\xeb\
-\x07\xff\x83\xdf\xddZ\xf9\xc9\x09/)\x14\x07\xba_\x1c\
-\xe7c\x14\x08\xec\x02\x8d\x9a\xe3|\x1f;N\xe3\x04\xf0\
-?\x03Wz\xcb_\xa9\x033\x9f\xa4\xd7ZZ\xe4\x08\
-\xe8\xdb\x06.\xae[\x9a\xb2\x07\x5c\xee\x00CO\x86l\
-\xca\xae\xe4\xa7)\xe4\xf3\xc0\xfb\x19}S\x16\x18\xbc\x05\
-\x82k^o\xcd}\x9c>\x00i\xea*y\x03\x1c\x1c\
-\x02c\x05\xca^\xef\xf0\xee\x9e\xf6\xde\xfe=\xd3\xec\xef\
-\x07W\xdar\x9c\x98\xfc\x90>\x00\x00\x10XiTX\
-tXML:com.adobe.x\
-mp\x00\x00\x00\x00\x00<?xpacket\
- begin=\x22\xef\xbb\xbf\x22 id=\
-\x22W5M0MpCehiHzreS\
-zNTczkc9d\x22?>\x0a<x:\
-xmpmeta xmlns:x=\
-\x22adobe:ns:meta/\x22\
- x:xmptk=\x22XMP Co\
-re 4.4.0-Exiv2\x22>\
-\x0a <rdf:RDF xmlns\
-:rdf=\x22http://www\
-.w3.org/1999/02/\
-22-rdf-syntax-ns\
-#\x22>\x0a  <rdf:Descr\
-iption rdf:about\
-=\x22\x22\x0a    xmlns:ip\
-tcExt=\x22http://ip\
-tc.org/std/Iptc4\
-xmpExt/2008-02-2\
-9/\x22\x0a    xmlns:xm\
-pMM=\x22http://ns.a\
-dobe.com/xap/1.0\
-/mm/\x22\x0a    xmlns:\
-stEvt=\x22http://ns\
-.adobe.com/xap/1\
-.0/sType/Resourc\
-eEvent#\x22\x0a    xml\
-ns:stRef=\x22http:/\
-/ns.adobe.com/xa\
-p/1.0/sType/Reso\
-urceRef#\x22\x0a    xm\
-lns:plus=\x22http:/\
-/ns.useplus.org/\
-ldf/xmp/1.0/\x22\x0a  \
-  xmlns:GIMP=\x22ht\
-tp://www.gimp.or\
-g/xmp/\x22\x0a    xmln\
-s:dc=\x22http://pur\
-l.org/dc/element\
-s/1.1/\x22\x0a    xmln\
-s:tiff=\x22http://n\
-s.adobe.com/tiff\
-/1.0/\x22\x0a    xmlns\
-:xmp=\x22http://ns.\
-adobe.com/xap/1.\
-0/\x22\x0a   xmpMM:Doc\
-umentID=\x22xmp.did\
-:E5178A2B99A011E\
-29A15BC1046A8904\
-D\x22\x0a   xmpMM:Inst\
-anceID=\x22xmp.iid:\
-00063360-f1d7-4f\
-09-8a41-bcb20a92\
-0a27\x22\x0a   xmpMM:O\
-riginalDocumentI\
-D=\x22xmp.did:12f20\
-251-8048-4234-bd\
-37-6117502ec313\x22\
-\x0a   GIMP:API=\x222.\
-0\x22\x0a   GIMP:Platf\
-orm=\x22Linux\x22\x0a   G\
-IMP:TimeStamp=\x221\
-602874314737681\x22\
-\x0a   GIMP:Version\
-=\x222.10.22\x22\x0a   dc\
-:Format=\x22image/p\
-ng\x22\x0a   tiff:Orie\
-ntation=\x221\x22\x0a   x\
-mp:CreatorTool=\x22\
-GIMP 2.10\x22>\x0a   <\
-iptcExt:Location\
-Created>\x0a    <rd\
-f:Bag/>\x0a   </ipt\
-cExt:LocationCre\
-ated>\x0a   <iptcEx\
-t:LocationShown>\
-\x0a    <rdf:Bag/>\x0a\
-   </iptcExt:Loc\
-ationShown>\x0a   <\
-iptcExt:ArtworkO\
-rObject>\x0a    <rd\
-f:Bag/>\x0a   </ipt\
-cExt:ArtworkOrOb\
-ject>\x0a   <iptcEx\
-t:RegistryId>\x0a  \
-  <rdf:Bag/>\x0a   \
-</iptcExt:Regist\
-ryId>\x0a   <xmpMM:\
-History>\x0a    <rd\
-f:Seq>\x0a     <rdf\
-:li\x0a      stEvt:\
-action=\x22saved\x22\x0a \
-     stEvt:chang\
-ed=\x22/\x22\x0a      stE\
-vt:instanceID=\x22x\
-mp.iid:825a5a7d-\
-c3bc-49ee-80d2-1\
-4d4aaaff7f7\x22\x0a   \
-   stEvt:softwar\
-eAgent=\x22Gimp 2.1\
-0 (Linux)\x22\x0a     \
- stEvt:when=\x22+02\
-:00\x22/>\x0a    </rdf\
-:Seq>\x0a   </xmpMM\
-:History>\x0a   <xm\
-pMM:DerivedFrom\x0a\
-    stRef:docume\
-ntID=\x22xmp.did:E5\
-178A2999A011E29A\
-15BC1046A8904D\x22\x0a\
-    stRef:instan\
-ceID=\x22xmp.iid:E5\
-178A2899A011E29A\
-15BC1046A8904D\x22/\
->\x0a   <plus:Image\
-Supplier>\x0a    <r\
-df:Seq/>\x0a   </pl\
-us:ImageSupplier\
->\x0a   <plus:Image\
-Creator>\x0a    <rd\
-f:Seq/>\x0a   </plu\
-s:ImageCreator>\x0a\
-   <plus:Copyrig\
-htOwner>\x0a    <rd\
-f:Seq/>\x0a   </plu\
-s:CopyrightOwner\
->\x0a   <plus:Licen\
-sor>\x0a    <rdf:Se\
-q/>\x0a   </plus:Li\
-censor>\x0a  </rdf:\
-Description>\x0a </\
-rdf:RDF>\x0a</x:xmp\
-meta>\x0a          \
-                \
-                \
-                \
-                \
-                \
-          \x0a     \
-                \
-                \
-                \
-                \
-                \
-               \x0a\
-                \
-                \
-                \
-                \
-                \
-                \
-    \x0a           \
-                \
-                \
-                \
-                \
-                \
-         \x0a      \
-                \
-                \
-                \
-                \
-                \
-              \x0a \
-                \
-                \
-                \
-                \
-                \
-                \
-   \x0a            \
-                \
-                \
-                \
-                \
-                \
-        \x0a       \
-                \
-                \
-                \
-                \
-                \
-             \x0a  \
-                \
-                \
-                \
-                \
-                \
-                \
-  \x0a             \
-                \
-                \
-                \
-                \
-                \
-       \x0a        \
-                \
-                \
-                \
-                \
-                \
-            \x0a   \
-                \
-                \
-                \
-                \
-                \
-                \
- \x0a              \
-                \
-                \
-                \
-                \
-                \
-      \x0a         \
-                \
-                \
-                \
-                \
-                \
-           \x0a    \
-                \
-                \
-                \
-                \
-                \
-                \
-\x0a               \
-                \
-                \
-                \
-                \
-                \
-     \x0a          \
-                \
-                \
-                \
-                \
-                \
-          \x0a     \
-                \
-                \
-                \
-                \
-                \
-               \x0a\
-                \
-                \
-                \
-                \
-                \
-                \
-    \x0a           \
-                \
-                \
-                \
-                \
-                \
-         \x0a      \
-                \
-     \x0a<?xpacket \
-end=\x22w\x22?>\xc2(:\xc2\x00\x00\x00\
-\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\xa7\x93\x00\
-\x00\x00\x09pHYs\x00\x00\x0b\x13\x00\x00\x0b\x13\x01\
-\x00\x9a\x9c\x18\x00\x00\x00\x07tIME\x07\xe4\x0a\x10\
-\x1236\x7f\xdb;\xbd\x00\x00\x03\x19IDATX\
-\xc3\xcd\xd7]\x88UU\x14\x07\xf0\xdf=M\x94\xe1X\
-J\xf7\xdc+AM\x14\x05\x81\x86\x99=\xd5CCT\
-H8\xa4=\x04=6}=\x04\x81\x05a\x0f\x15\xc1\
-\x18hR\x11\x14A\x8f\xbd\x8dZI\x10$\x06\xa1\xf4\
-P\xd3@>XQ\x0eZ\x92\xfbl\xb1\xfc \xec\xc3\
-\xa6\x97=t\xbc\x9c3\x9d\xb9\xdd\x81\x16\x9c\x87\xb3\xd6\
-\xde\xff\xf5_\xeb\xec\xb5\xf6:-\x0d\xa5\xd3\xce\xaf\xc4\
-\x18\xee\xc4j\x5c\x8b\xa5\xc9|\x163\xf8\x0a\x9f\xe0\xfd\
-\x10\x8b\x13Mp[\x0d\x1c\xaf\xc1\xb3\xd8\x88\xa1\x86|\
-\xff\xc4.\xbc\x1cb1\xdd\x17\x81N;\xbf\x1c\xdb\xf1\
-p\x13\xa252\x8bw\xf0t\x88\xc5\xa9\xc6\x04R\xd4\
-;S\x9a\x07!3\xd8T\x95\x8dV\x85\xf3Q\xec\xc6\
-2\x83\x95\xd3\xb8?\xc4b_-\x81N;_\x8b}\
-\x8b\xe0\xbcLb4\xc4bjN\x91\x95\x9c/\xc7d\
-\x8f\xf3C\xe90\x9d\xee\xd3\xd9\xae\x841'\xcb0\x99\
-|]H\x00\xaf`\xa4\x07d\x22\xc4b\x13r\x8c#\
-\x94\xca\xee >M\xcf\xc1\xa4\x93\xd6\x8c#O{'\
-z0G\x92\xaf\x7f>A\xa7\x9d\xdf\x8a\xcf+\xa2X\
-\x1bb\xf1eOe\xac\xc4\xb7!\x16\x7f\xf5|\xbe\x0c\
-7\xe0\xa7\xf2\x89\xef\xb4\xf3[0U\x81\xbd.\xc4\xe2\
-\x8b\xb9\xba\xdeR\x93\xc6\x8b\xca/\x09\xb8\xb2\x9c\x12\xa1\
-\xaf\xff\x0d\xa3$[\xb01\xeb\xb4\xf3.6\xd4,\xba\
-i\x00\x07\xaf\x0ecC\xa7\x9dw\xb3\xd4^\xabX\xfe\
-\x88=\x03 \xb0\x07?\xd4df,\xc3h\xcd\xc6\xe7\
-C,N\xfeW\xef\x09\xe3\x85\x1a\xf3h\x86U\x15\x86\
-\xf3\xa9\x13\x0eJv&\xcc^Y\x95U\x94\x1e\x1c\xab\
-\xeb\xdd}f\xe1\x14\x8eU\x98F2,\xa90\xfc\xbe\
-\x08]\xf0\x8f\x0a\xdd\x92\xac\xee2\x5c\x04\x02y\x952\
-\xc3\x99\x0a\xfdp\xa7\x9d\xe7\x83\xf2\x9c\xb0\x86+Lg\
-2\x1c\xae\xd9w\xef\x00\xa3\xaf\xc3:\x9c\xd5\xb4I\xd8\
-\xdci\xe7C\x03\x88~\x08\x9bk\xccS\x19\xf6\xd6\x18\
-Wc\xdb\x00\xa2\xdf\x96\xb0\xaado\xab\xd3\xce\x87q\
-\x1c\x97\xd5,\x9a\xc4\x93!\x16\xc7\x17\x18\xf9J\xbc\x8e\
-\x07j\x96\xfc\x8a\xee\xdcm\xf8&\x1e/1\xfe\x10/\
-\xe1\x8eR\x09\xbd\x87\x8f1\x8d\xe9\x10\x8b\xf3\x15\xa9^\
-\x87\x9bq7\xee\xc3\xc5\xf3p|+\xc4\xe2\x899\x02\
-W\xe3\x1b\x5c\x9a\x06\xc9g\xf0F\xba\xebo\xeb\xd9\xb8\
-;\xcdw\xb3=\x04Z\xc96\xd6 A\xe7pc\x88\
-\xc5\xd1,u\xaa\xa3\xd8Z\x9a\x11\xb6c\x0d\x1e\xac\xb8\
-Hv\xf4:O\x18\xb3\xd8\xd1\xf0\x0bmM>/\x98\
-\x88&p\xa0\xf4\xfeb\x88\xc5L:@\xe3x\x0e\xf7\
-\xe0\xb3y\x80\x0f5p~\xa0<%\xf5\x0e\xa5]\xec\
-\xc7uI\xf5T\x88\xc5k\x0b8xW\xe0\xe7y\x96\
-|\x8f\xdb\xcb\x07\xbaj,\xbf&\x95\xe6\xf5I\xb5\x1f\
-\x1f \xa2\x8bWC,\xce\xf5A\xe0;\xdc\x15bq\
-\xa4\xc9\x8f\xc9\x0a\xbc[\xd3\xc1\x96\x87X\xfc\xb2@\x02\
-\x1f\xe1\xa1\xaa\xf9\x22\x9bg\x88X\x8fGR\xe4\xfd\xca\
-\x09<\x8a\xf5u\xc3M\x93\x9f\xd3\xa5x,=+p\
-U\x88\xc5o5k/I\xf7\xfeI\xbc\x9dj\xfd\xac\
-\xff\xb3\xfc\x0dTj\x06\x16\x12.K\x86\x00\x00\x00\x00\
-IEND\xaeB`\x82\
 \x00\x00 \x17\
 \x89\
 PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
 \x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
 \x00\x00\x07\x15zTXtRaw prof\
 ile type exif\x00\x00x\
 \xda\xadWY\xb2\xe4(\x0c\xfc\xe7\x14s\x04\x04\x88\xe5\
@@ -6229,37 +6198,60 @@
 a\xa4\xea4\xd8\xe2K\x9b\x01\x00o\x1ek\x87\xa6\xef\
 u\xe6Wc\xd5_\x8c\x03\xb8\xbc\x00\xf4\xd26\x82\x17\
 \xe5\xac\x99\x09B&]z\x00\x9a\xc9yD\xf0\xe5\xa9\
 )\xb3V\xff?J+Y\xc0\xcdg\xb1e\xc6o\x0b\
 l\x0an\x1fw\xdc\x98-\xfb\xbf\xc7\xd7\xb1\x8eu\xac\
 c\x1d\xebX\xc7:\xce\xc4\xff\x00u\x01\xcb)\x0dd\
 \x0b\xbe\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x017\
+<\
+?xml version=\x221.\
+0\x22 encoding=\x22utf\
+-8\x22?>\x0a<!DOCTYPE \
+TS><TS version=\x22\
+1.1\x22 language=\x22f\
+r_FR\x22>\x0a<context>\
+\x0a    <name>MainW\
+indow</name>\x0a   \
+ <message>\x0a     \
+   <location fil\
+ename=\x22main_wind\
+ow.py\x22 line=\x2299\x22\
+/>\x0a        <sour\
+ce>&amp;File</so\
+urce>\x0a        <t\
+ranslation>&amp;\
+Fichier</transla\
+tion>\x0a    </mess\
+age>\x0a</context>\x0a\
+</TS>\x0a\
+\x00\x00\x00g\
+<\
+\xb8d\x18\xca\xef\x9c\x95\xcd!\x1c\xbf`\xa1\xbd\xdd\xa7\
+\x00\x00\x00\x05fr_FRB\x00\x00\x00\x08\x00*\
+\xd0%\x00\x00\x00\x00i\x00\x00\x004\x03\x00\x00\x00\x10\
+\x00&\x00F\x00i\x00c\x00h\x00i\x00e\x00r\
+\x08\x00\x00\x00\x00\x06\x00\x00\x00\x05&File\x07\
+\x00\x00\x00\x0aMainWindow\x01\x88\
+\x00\x00\x00\x02\x03\x01\
 "
 
 qt_resource_name = b"\
 \x00\x09\
 \x0alxC\
 \x00r\
 \x00e\x00s\x00o\x00u\x00r\x00c\x00e\x00s\
-\x00\x05\
-\x00o\xa6S\
-\x00i\
-\x00c\x00o\x00n\x00s\
 \x00\x0c\
 \x0d\xfc\x11\x13\
 \x00t\
 \x00r\x00a\x00n\x00s\x00l\x00a\x00t\x00i\x00o\x00n\x00s\
-\x00\x08\
-\x08;X\x13\
-\x00f\
-\x00r\x00_\x00F\x00R\x00.\x00t\x00s\
-\x00\x08\
-\x08;X\xdd\
-\x00f\
-\x00r\x00_\x00F\x00R\x00.\x00q\x00m\
+\x00\x05\
+\x00o\xa6S\
+\x00i\
+\x00c\x00o\x00n\x00s\
 \x00\x08\
 \x0fjXg\
 \x00s\
 \x00h\x00o\x00w\x00.\x00p\x00n\x00g\
 \x00\x0a\
 \x08\x87L'\
 \x00y\
@@ -6288,25 +6280,25 @@
 \x00e\x00s\x00W\x00e\x00H\x00a\x00c\x00k\x00C\x00o\x00n\x00f\x00i\x00g\x00u\x00r\
 \x00a\x00t\x00i\x00o\x00n\x00-\x002\x00x\x00.\x00p\x00n\x00g\
 \x00\x15\
 \x03\x14]g\
 \x00J\
 \x00i\x00r\x00a\x00C\x00o\x00n\x00f\x00i\x00g\x00u\x00r\x00a\x00t\x00i\x00o\x00n\
 \x00.\x00p\x00n\x00g\
-\x00\x1a\
-\x0c-[g\
-\x00G\
-\x00i\x00t\x00L\x00a\x00b\x00C\x00o\x00n\x00f\x00i\x00g\x00u\x00r\x00a\x00t\x00i\
-\x00o\x00n\x00-\x002\x00x\x00.\x00p\x00n\x00g\
 \x00\x17\
 \x00a\x92\x87\
 \x00G\
 \x00i\x00t\x00H\x00u\x00b\x00C\x00o\x00n\x00f\x00i\x00g\x00u\x00r\x00a\x00t\x00i\
 \x00o\x00n\x00.\x00p\x00n\x00g\
 \x00\x1a\
+\x0c-[g\
+\x00G\
+\x00i\x00t\x00L\x00a\x00b\x00C\x00o\x00n\x00f\x00i\x00g\x00u\x00r\x00a\x00t\x00i\
+\x00o\x00n\x00-\x002\x00x\x00.\x00p\x00n\x00g\
+\x00\x1a\
 \x0c\xc7[g\
 \x00G\
 \x00i\x00t\x00H\x00u\x00b\x00C\x00o\x00n\x00f\x00i\x00g\x00u\x00r\x00a\x00t\x00i\
 \x00o\x00n\x00-\x002\x00x\x00.\x00p\x00n\x00g\
 \x00\x17\
 \x00a\x9c'\
 \x00G\
@@ -6323,59 +6315,67 @@
 \x00e\x00r\x00v\x00i\x00c\x00e\x00N\x00o\x00w\x00C\x00o\x00n\x00f\x00i\x00g\x00u\
 \x00r\x00a\x00t\x00i\x00o\x00n\x00-\x002\x00x\x00.\x00p\x00n\x00g\
 \x00\x18\
 \x0095\xc7\
 \x00J\
 \x00i\x00r\x00a\x00C\x00o\x00n\x00f\x00i\x00g\x00u\x00r\x00a\x00t\x00i\x00o\x00n\
 \x00-\x002\x00x\x00.\x00p\x00n\x00g\
+\x00\x08\
+\x08;X\x13\
+\x00f\
+\x00r\x00_\x00F\x00R\x00.\x00t\x00s\
+\x00\x08\
+\x08;X\xdd\
+\x00f\
+\x00r\x00_\x00F\x00R\x00.\x00q\x00m\
 "
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x02\x00\x00\x00\x02\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x18\x00\x02\x00\x00\x00\x04\x00\x00\x00\x06\
+\x00\x00\x006\x00\x02\x00\x00\x00\x04\x00\x00\x00\x06\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00(\x00\x02\x00\x00\x00\x02\x00\x00\x00\x04\
+\x00\x00\x00\x18\x00\x02\x00\x00\x00\x02\x00\x00\x00\x04\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00F\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x00\x5c\x00\x00\x00\x00\x00\x01\x00\x00\x01;\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x00\xb8\x00\x02\x00\x00\x00\x03\x00\x00\x00\x0a\
+\x00\x00\x03\x04\x00\x00\x00\x00\x00\x01\x00\x01\x81\x84\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x03\x1a\x00\x00\x00\x00\x00\x01\x00\x01\x82\xbf\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x00\x8c\x00\x02\x00\x00\x00\x03\x00\x00\x00\x0a\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x88\x00\x00\x00\x00\x00\x01\x00\x00(\x95\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x00r\x00\x00\x00\x00\x00\x01\x00\x00\x01\xa6\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x00\xa2\x00\x00\x00\x00\x00\x01\x00\x00H^\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x010\x00\x00\x00\x00\x00\x01\x00\x00\x8c\x08\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x00\xf6\x00\x00\x00\x00\x00\x01\x00\x00s+\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x00\xc8\x00\x02\x00\x00\x00\x08\x00\x00\x00\x0d\
+\x00\x00\x00\x5c\x00\x00\x00\x00\x00\x01\x00\x00&\xef\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x00F\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x00v\x00\x00\x00\x00\x00\x01\x00\x00F\xb8\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x01\x04\x00\x00\x00\x00\x00\x01\x00\x00\x8ab\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x00\xca\x00\x00\x00\x00\x00\x01\x00\x00q\x85\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x00\x9c\x00\x02\x00\x00\x00\x08\x00\x00\x00\x0d\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x02\xfa\x00\x00\x00\x00\x00\x01\x00\x01]7\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x01\xda\x00\x00\x00\x00\x00\x01\x00\x00\xf5P\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x02H\x00\x00\x00\x00\x00\x01\x00\x01/8\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x01p\x00\x00\x00\x00\x00\x01\x00\x00\xab\xd1\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x02|\x00\x00\x00\x00\x00\x01\x00\x01M\xd9\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x01\xa0\x00\x00\x00\x00\x00\x01\x00\x00\xc9\x8d\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x02\x0e\x00\x00\x00\x00\x00\x01\x00\x01\x0f\x1d\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
-\x00\x00\x02\xb8\x00\x00\x00\x00\x00\x01\x00\x01S\xec\
-\x00\x00\x01\x84v\x1d\xdf\xb8\
+\x00\x00\x02\xce\x00\x00\x00\x00\x00\x01\x00\x01[\x91\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x01t\x00\x00\x00\x00\x00\x01\x00\x00\xc7\xe7\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x02\x1c\x00\x00\x00\x00\x00\x01\x00\x01-\x92\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x01D\x00\x00\x00\x00\x00\x01\x00\x00\xaa+\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x02P\x00\x00\x00\x00\x00\x01\x00\x01L3\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x01\xa8\x00\x00\x00\x00\x00\x01\x00\x00\xe1\xb4\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x01\xe2\x00\x00\x00\x00\x00\x01\x00\x01\x0dw\
+\x00\x00\x01\x87\xbd\x9fO*\
+\x00\x00\x02\x8c\x00\x00\x00\x00\x00\x01\x00\x01RF\
+\x00\x00\x01\x87\xbd\x9fO*\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/resources.qrc` & `ywh2bt-2.7.4/ywh2bt/gui/resources.qrc`

 * *Files 0% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 00000000: 3c21 444f 4354 5950 4520 5243 433e 0a3c  <!DOCTYPE RCC>.<
 00000010: 5243 4320 7665 7273 696f 6e3d 2231 2e30  RCC version="1.0
 00000020: 223e 0a20 2020 203c 7172 6573 6f75 7263  ">.    <qresourc
 00000030: 653e 0a20 2020 2020 2020 203c 6669 6c65  e>.        <file
-00000040: 3e72 6573 6f75 7263 6573 2f69 636f 6e73  >resources/icons
-00000050: 2f73 686f 772e 706e 673c 2f66 696c 653e  /show.png</file>
-00000060: 0a20 2020 2020 2020 203c 6669 6c65 3e72  .        <file>r
-00000070: 6573 6f75 7263 6573 2f69 636f 6e73 2f79  esources/icons/y
-00000080: 7768 3262 742e 706e 673c 2f66 696c 653e  wh2bt.png</file>
-00000090: 0a20 2020 2020 2020 203c 6669 6c65 3e72  .        <file>r
-000000a0: 6573 6f75 7263 6573 2f69 636f 6e73 2f68  esources/icons/h
-000000b0: 6964 652e 706e 673c 2f66 696c 653e 0a20  ide.png</file>. 
-000000c0: 2020 2020 2020 203c 6669 6c65 3e72 6573         <file>res
-000000d0: 6f75 7263 6573 2f69 636f 6e73 2f74 7970  ources/icons/typ
-000000e0: 6573 2f59 6573 5765 4861 636b 436f 6e66  es/YesWeHackConf
-000000f0: 6967 7572 6174 696f 6e2d 3278 2e70 6e67  iguration-2x.png
-00000100: 3c2f 6669 6c65 3e0a 2020 2020 2020 2020  </file>.        
-00000110: 3c66 696c 653e 7265 736f 7572 6365 732f  <file>resources/
-00000120: 6963 6f6e 732f 7479 7065 732f 5965 7357  icons/types/YesW
-00000130: 6548 6163 6b43 6f6e 6669 6775 7261 7469  eHackConfigurati
-00000140: 6f6e 2e70 6e67 3c2f 6669 6c65 3e0a 2020  on.png</file>.  
-00000150: 2020 2020 2020 3c66 696c 653e 7265 736f        <file>reso
-00000160: 7572 6365 732f 6963 6f6e 732f 7479 7065  urces/icons/type
-00000170: 732f 5472 6163 6b65 7243 6f6e 6669 6775  s/TrackerConfigu
-00000180: 7261 7469 6f6e 2f47 6974 4c61 6243 6f6e  ration/GitLabCon
-00000190: 6669 6775 7261 7469 6f6e 2d32 782e 706e  figuration-2x.pn
-000001a0: 673c 2f66 696c 653e 0a20 2020 2020 2020  g</file>.       
-000001b0: 203c 6669 6c65 3e72 6573 6f75 7263 6573   <file>resources
-000001c0: 2f69 636f 6e73 2f74 7970 6573 2f54 7261  /icons/types/Tra
-000001d0: 636b 6572 436f 6e66 6967 7572 6174 696f  ckerConfiguratio
-000001e0: 6e2f 5365 7276 6963 654e 6f77 436f 6e66  n/ServiceNowConf
-000001f0: 6967 7572 6174 696f 6e2d 3278 2e70 6e67  iguration-2x.png
-00000200: 3c2f 6669 6c65 3e0a 2020 2020 2020 2020  </file>.        
-00000210: 3c66 696c 653e 7265 736f 7572 6365 732f  <file>resources/
-00000220: 6963 6f6e 732f 7479 7065 732f 5472 6163  icons/types/Trac
-00000230: 6b65 7243 6f6e 6669 6775 7261 7469 6f6e  kerConfiguration
-00000240: 2f4a 6972 6143 6f6e 6669 6775 7261 7469  /JiraConfigurati
-00000250: 6f6e 2d32 782e 706e 673c 2f66 696c 653e  on-2x.png</file>
-00000260: 0a20 2020 2020 2020 203c 6669 6c65 3e72  .        <file>r
-00000270: 6573 6f75 7263 6573 2f69 636f 6e73 2f74  esources/icons/t
-00000280: 7970 6573 2f54 7261 636b 6572 436f 6e66  ypes/TrackerConf
-00000290: 6967 7572 6174 696f 6e2f 4769 7448 7562  iguration/GitHub
-000002a0: 436f 6e66 6967 7572 6174 696f 6e2e 706e  Configuration.pn
-000002b0: 673c 2f66 696c 653e 0a20 2020 2020 2020  g</file>.       
-000002c0: 203c 6669 6c65 3e72 6573 6f75 7263 6573   <file>resources
-000002d0: 2f69 636f 6e73 2f74 7970 6573 2f54 7261  /icons/types/Tra
-000002e0: 636b 6572 436f 6e66 6967 7572 6174 696f  ckerConfiguratio
-000002f0: 6e2f 4769 744c 6162 436f 6e66 6967 7572  n/GitLabConfigur
-00000300: 6174 696f 6e2e 706e 673c 2f66 696c 653e  ation.png</file>
-00000310: 0a20 2020 2020 2020 203c 6669 6c65 3e72  .        <file>r
-00000320: 6573 6f75 7263 6573 2f69 636f 6e73 2f74  esources/icons/t
-00000330: 7970 6573 2f54 7261 636b 6572 436f 6e66  ypes/TrackerConf
-00000340: 6967 7572 6174 696f 6e2f 4a69 7261 436f  iguration/JiraCo
-00000350: 6e66 6967 7572 6174 696f 6e2e 706e 673c  nfiguration.png<
-00000360: 2f66 696c 653e 0a20 2020 2020 2020 203c  /file>.        <
-00000370: 6669 6c65 3e72 6573 6f75 7263 6573 2f69  file>resources/i
-00000380: 636f 6e73 2f74 7970 6573 2f54 7261 636b  cons/types/Track
-00000390: 6572 436f 6e66 6967 7572 6174 696f 6e2f  erConfiguration/
-000003a0: 4769 7448 7562 436f 6e66 6967 7572 6174  GitHubConfigurat
-000003b0: 696f 6e2d 3278 2e70 6e67 3c2f 6669 6c65  ion-2x.png</file
-000003c0: 3e0a 2020 2020 2020 2020 3c66 696c 653e  >.        <file>
-000003d0: 7265 736f 7572 6365 732f 6963 6f6e 732f  resources/icons/
-000003e0: 7479 7065 732f 5472 6163 6b65 7243 6f6e  types/TrackerCon
-000003f0: 6669 6775 7261 7469 6f6e 2f53 6572 7669  figuration/Servi
-00000400: 6365 4e6f 7743 6f6e 6669 6775 7261 7469  ceNowConfigurati
-00000410: 6f6e 2e70 6e67 3c2f 6669 6c65 3e0a 2020  on.png</file>.  
-00000420: 2020 2020 2020 3c66 696c 653e 7265 736f        <file>reso
-00000430: 7572 6365 732f 7472 616e 736c 6174 696f  urces/translatio
-00000440: 6e73 2f66 725f 4652 2e74 733c 2f66 696c  ns/fr_FR.ts</fil
-00000450: 653e 0a20 2020 2020 2020 203c 6669 6c65  e>.        <file
-00000460: 3e72 6573 6f75 7263 6573 2f74 7261 6e73  >resources/trans
-00000470: 6c61 7469 6f6e 732f 6672 5f46 522e 716d  lations/fr_FR.qm
+00000040: 3e72 6573 6f75 7263 6573 2f74 7261 6e73  >resources/trans
+00000050: 6c61 7469 6f6e 732f 6672 5f46 522e 7473  lations/fr_FR.ts
+00000060: 3c2f 6669 6c65 3e0a 2020 2020 2020 2020  </file>.        
+00000070: 3c66 696c 653e 7265 736f 7572 6365 732f  <file>resources/
+00000080: 7472 616e 736c 6174 696f 6e73 2f66 725f  translations/fr_
+00000090: 4652 2e71 6d3c 2f66 696c 653e 0a20 2020  FR.qm</file>.   
+000000a0: 2020 2020 203c 6669 6c65 3e72 6573 6f75       <file>resou
+000000b0: 7263 6573 2f69 636f 6e73 2f79 7768 3262  rces/icons/ywh2b
+000000c0: 742e 706e 673c 2f66 696c 653e 0a20 2020  t.png</file>.   
+000000d0: 2020 2020 203c 6669 6c65 3e72 6573 6f75       <file>resou
+000000e0: 7263 6573 2f69 636f 6e73 2f73 686f 772e  rces/icons/show.
+000000f0: 706e 673c 2f66 696c 653e 0a20 2020 2020  png</file>.     
+00000100: 2020 203c 6669 6c65 3e72 6573 6f75 7263     <file>resourc
+00000110: 6573 2f69 636f 6e73 2f68 6964 652e 706e  es/icons/hide.pn
+00000120: 673c 2f66 696c 653e 0a20 2020 2020 2020  g</file>.       
+00000130: 203c 6669 6c65 3e72 6573 6f75 7263 6573   <file>resources
+00000140: 2f69 636f 6e73 2f74 7970 6573 2f59 6573  /icons/types/Yes
+00000150: 5765 4861 636b 436f 6e66 6967 7572 6174  WeHackConfigurat
+00000160: 696f 6e2d 3278 2e70 6e67 3c2f 6669 6c65  ion-2x.png</file
+00000170: 3e0a 2020 2020 2020 2020 3c66 696c 653e  >.        <file>
+00000180: 7265 736f 7572 6365 732f 6963 6f6e 732f  resources/icons/
+00000190: 7479 7065 732f 5965 7357 6548 6163 6b43  types/YesWeHackC
+000001a0: 6f6e 6669 6775 7261 7469 6f6e 2e70 6e67  onfiguration.png
+000001b0: 3c2f 6669 6c65 3e0a 2020 2020 2020 2020  </file>.        
+000001c0: 3c66 696c 653e 7265 736f 7572 6365 732f  <file>resources/
+000001d0: 6963 6f6e 732f 7479 7065 732f 5472 6163  icons/types/Trac
+000001e0: 6b65 7243 6f6e 6669 6775 7261 7469 6f6e  kerConfiguration
+000001f0: 2f47 6974 4c61 6243 6f6e 6669 6775 7261  /GitLabConfigura
+00000200: 7469 6f6e 2e70 6e67 3c2f 6669 6c65 3e0a  tion.png</file>.
+00000210: 2020 2020 2020 2020 3c66 696c 653e 7265          <file>re
+00000220: 736f 7572 6365 732f 6963 6f6e 732f 7479  sources/icons/ty
+00000230: 7065 732f 5472 6163 6b65 7243 6f6e 6669  pes/TrackerConfi
+00000240: 6775 7261 7469 6f6e 2f53 6572 7669 6365  guration/Service
+00000250: 4e6f 7743 6f6e 6669 6775 7261 7469 6f6e  NowConfiguration
+00000260: 2d32 782e 706e 673c 2f66 696c 653e 0a20  -2x.png</file>. 
+00000270: 2020 2020 2020 203c 6669 6c65 3e72 6573         <file>res
+00000280: 6f75 7263 6573 2f69 636f 6e73 2f74 7970  ources/icons/typ
+00000290: 6573 2f54 7261 636b 6572 436f 6e66 6967  es/TrackerConfig
+000002a0: 7572 6174 696f 6e2f 4769 7448 7562 436f  uration/GitHubCo
+000002b0: 6e66 6967 7572 6174 696f 6e2d 3278 2e70  nfiguration-2x.p
+000002c0: 6e67 3c2f 6669 6c65 3e0a 2020 2020 2020  ng</file>.      
+000002d0: 2020 3c66 696c 653e 7265 736f 7572 6365    <file>resource
+000002e0: 732f 6963 6f6e 732f 7479 7065 732f 5472  s/icons/types/Tr
+000002f0: 6163 6b65 7243 6f6e 6669 6775 7261 7469  ackerConfigurati
+00000300: 6f6e 2f47 6974 4875 6243 6f6e 6669 6775  on/GitHubConfigu
+00000310: 7261 7469 6f6e 2e70 6e67 3c2f 6669 6c65  ration.png</file
+00000320: 3e0a 2020 2020 2020 2020 3c66 696c 653e  >.        <file>
+00000330: 7265 736f 7572 6365 732f 6963 6f6e 732f  resources/icons/
+00000340: 7479 7065 732f 5472 6163 6b65 7243 6f6e  types/TrackerCon
+00000350: 6669 6775 7261 7469 6f6e 2f4a 6972 6143  figuration/JiraC
+00000360: 6f6e 6669 6775 7261 7469 6f6e 2d32 782e  onfiguration-2x.
+00000370: 706e 673c 2f66 696c 653e 0a20 2020 2020  png</file>.     
+00000380: 2020 203c 6669 6c65 3e72 6573 6f75 7263     <file>resourc
+00000390: 6573 2f69 636f 6e73 2f74 7970 6573 2f54  es/icons/types/T
+000003a0: 7261 636b 6572 436f 6e66 6967 7572 6174  rackerConfigurat
+000003b0: 696f 6e2f 4a69 7261 436f 6e66 6967 7572  ion/JiraConfigur
+000003c0: 6174 696f 6e2e 706e 673c 2f66 696c 653e  ation.png</file>
+000003d0: 0a20 2020 2020 2020 203c 6669 6c65 3e72  .        <file>r
+000003e0: 6573 6f75 7263 6573 2f69 636f 6e73 2f74  esources/icons/t
+000003f0: 7970 6573 2f54 7261 636b 6572 436f 6e66  ypes/TrackerConf
+00000400: 6967 7572 6174 696f 6e2f 5365 7276 6963  iguration/Servic
+00000410: 654e 6f77 436f 6e66 6967 7572 6174 696f  eNowConfiguratio
+00000420: 6e2e 706e 673c 2f66 696c 653e 0a20 2020  n.png</file>.   
+00000430: 2020 2020 203c 6669 6c65 3e72 6573 6f75       <file>resou
+00000440: 7263 6573 2f69 636f 6e73 2f74 7970 6573  rces/icons/types
+00000450: 2f54 7261 636b 6572 436f 6e66 6967 7572  /TrackerConfigur
+00000460: 6174 696f 6e2f 4769 744c 6162 436f 6e66  ation/GitLabConf
+00000470: 6967 7572 6174 696f 6e2d 3278 2e70 6e67  iguration-2x.png
 00000480: 3c2f 6669 6c65 3e0a 2020 2020 3c2f 7172  </file>.    </qr
 00000490: 6573 6f75 7263 653e 0a3c 2f52 4343 3e0a  esource>.</RCC>.
```

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/update_resources_file.py` & `ywh2bt-2.7.4/ywh2bt/gui/update_resources_file.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/attributes_container_dict_entry_widget.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/attributes_container_dict_entry_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/attributes_container_dict_widget.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/attributes_container_dict_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/attributes_container_list_widget.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/attributes_container_list_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/attributes_container_widget.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/attributes_container_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/exportable_dict_widget.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/exportable_dict_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/attribute/exportable_list_widget.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/attribute/exportable_list_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/constants.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/constants.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/hinted_check_box_widget.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/hinted_check_box_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/logs_widget.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/logs_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/main_window.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/root_configuration_entry.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/root_configuration_entry.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/root_configuration_widget.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/root_configuration_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/root_configurations_widget.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/root_configurations_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/secret_line_edit_widget.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/secret_line_edit_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/thread/synchronizer.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/thread/synchronizer.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/gui/widgets/thread/tester.py` & `ywh2bt-2.7.4/ywh2bt/gui/widgets/thread/tester.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/ywh2bt/version.py` & `ywh2bt-2.7.4/ywh2bt/version.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.7.3/PKG-INFO` & `ywh2bt-2.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ywh2bt
-Version: 2.7.3
+Version: 2.7.4
 Summary: ywh2bt - YesWeHack to Bug Tracker
 Home-page: https://github.com/yeswehack/ywh2bugtracker
 Author: m.honel
 Author-email: m.honel@yeswehack.com
 Maintainer: YesWeHack
 Maintainer-email: project@yeswehack.com
 Requires-Python: >=3.7.0,<3.10
@@ -95,14 +95,16 @@
 - servicenow
 
 ## Changelog
 
 - v2.7:
     - added synchronization of "fix verification" logs when "Upload status updates" is checked
     - fixed an issue with jira when scope contains special markdown characters
+    - fixed an issue when "Download bug trackers comments" feedback option is activated
+      and bug tracker attachments do not meet platform attachments requirements (unacceptable mime-type, maximum allowed size exceeded)
 - v2.6:
     - added work around bug trackers maximum size allowed for the text of the issues/comments (content put in Markdown file attachment when necessary)
 - v2.5:
     - added Personal Access Token (PAT) authentication
     - removed OAuth authentication
 - v2.4:
     - added option to prevent recreation of issues that were created by a previous synchronization
```

