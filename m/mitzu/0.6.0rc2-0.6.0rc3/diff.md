# Comparing `tmp/mitzu-0.6.0rc2.tar.gz` & `tmp/mitzu-0.6.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.0rc2.tar", max compression
+gzip compressed data, was "mitzu-0.6.0rc3.tar", max compression
```

## Comparing `mitzu-0.6.0rc2.tar` & `mitzu-0.6.0rc3.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1082 2023-04-25 11:40:58.478845 mitzu-0.6.0rc2/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-04-25 11:40:58.478845 mitzu-0.6.0rc2/README.md
--rw-r--r--   0        0        0     6148 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/.DS_Store
--rw-r--r--   0        0        0      865 2023-04-25 11:42:10.543900 mitzu-0.6.0rc2/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1762 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5234 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6072 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2563 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      723 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     4085 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3344 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      660 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0      672 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    39389 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     5009 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     6687 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1760 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/helper.py
--rw-r--r--   0        0        0    54541 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6818 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     5424 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2086 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11435 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7124 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1854 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7547 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5372 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3339 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1261 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    10321 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    13355 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1594 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7392 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2966 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     2595 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     2750 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4833 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8355 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/model.py
--rw-r--r--   0        0        0      408 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     6112 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    15406 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4195 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    21143 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9799 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/dashboards.py
--rw-r--r--   0        0        0    14789 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5299 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    16412 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0    10152 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    11669 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1565 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9783 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1401 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1708 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     3894 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     4898 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1315 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10034 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    11756 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0    10013 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1733 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    35893 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9400 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     4901 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3146 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     2172 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     5302 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0     2105 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     4710 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    20518 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25909 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0      666 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/toast.py
--rw-r--r--   0        0        0     4141 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     2965 2023-04-25 11:42:10.539900 mitzu-0.6.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-25 15:24:54.935289 mitzu-0.6.0rc3/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-04-25 15:24:54.935289 mitzu-0.6.0rc3/README.md
+-rw-r--r--   0        0        0     6148 2023-04-25 15:24:55.327295 mitzu-0.6.0rc3/mitzu/.DS_Store
+-rw-r--r--   0        0        0      865 2023-04-25 15:25:54.424133 mitzu-0.6.0rc3/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1762 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5234 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6072 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2563 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      898 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     4085 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3344 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      660 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0      672 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    39656 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     5009 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     6687 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1394 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/helper.py
+-rw-r--r--   0        0        0    53851 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6818 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     5424 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2086 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11910 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     6951 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1866 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7547 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5767 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3339 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1278 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    10321 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    13549 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1594 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7392 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2966 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     2595 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     2750 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4833 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8355 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      408 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     6112 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    15406 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4195 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    21143 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9799 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/dashboards.py
+-rw-r--r--   0        0        0    14789 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5724 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5564 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    16412 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0    10152 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    10940 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2375 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1565 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0     9783 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1401 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1708 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     3894 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     4898 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1315 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10034 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11756 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0    10013 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1733 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    35893 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9400 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     4901 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3146 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     2172 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     5302 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0     2105 2023-04-25 15:24:55.339295 mitzu-0.6.0rc3/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     4710 2023-04-25 15:24:55.339295 mitzu-0.6.0rc3/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    20518 2023-04-25 15:24:55.339295 mitzu-0.6.0rc3/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25909 2023-04-25 15:24:55.339295 mitzu-0.6.0rc3/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0      666 2023-04-25 15:24:55.339295 mitzu-0.6.0rc3/mitzu/webapp/toast.py
+-rw-r--r--   0        0        0     4141 2023-04-25 15:24:55.339295 mitzu-0.6.0rc3/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     2943 2023-04-25 15:25:54.420133 mitzu-0.6.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc3/PKG-INFO
```

### Comparing `mitzu-0.6.0rc2/LICENSE.txt` & `mitzu-0.6.0rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/README.md` & `mitzu-0.6.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/.DS_Store` & `mitzu-0.6.0rc3/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/__init__.py` & `mitzu-0.6.0rc3/mitzu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.0-rc.2"
+__version__ = "0.6.0-rc.3"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.0rc3/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.0rc3/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.0rc3/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/file_adapter.py` & `mitzu-0.6.0rc3/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.0rc3/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/helper.py` & `mitzu-0.6.0rc3/mitzu/adapters/helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 from typing import Optional
 
 import mitzu.adapters.generic_adapter as GA
 import pandas as pd
 import json
 
 
-def str_to_datetime(val: str) -> Optional[datetime]:
+def str_to_datetime(val: str | pd.Timestamp) -> Optional[datetime]:
     if val is None:
         return None
-    return datetime.fromisoformat(val)
+    if type(val) == str:
+        return datetime.fromisoformat(val)
+    elif type(val) == pd.Timestamp:
+        return val.to_pydatetime()
+    raise ValueError(f"invalid datetime type: {type(val)}")
 
 
 def dataframe_str_to_datetime(pdf: pd.DataFrame, column: str) -> pd.DataFrame:
     pdf[column] = pdf[column].apply(str_to_datetime)
     return pdf
```

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.0rc3/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.0rc3/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.0rc3/mitzu/adapters/redshift_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.0rc3/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/__init__.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/__init__.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -817,29 +817,29 @@
             )
         else:
             raise ValueError(f"Aggregation type {at} is not supported for conversion")
 
     def _get_segmentation_select(self, metric: M.SegmentationMetric) -> Any:
         sub_query = self._get_segment_sub_query(metric._segment, metric, step=0)
         cte: EXP.CTE = aliased(
-            self._get_segment_sub_query_cte(sub_query, metric._group_by)
+            self._get_segment_sub_query_cte(sub_query, metric._segment._group_by)
         )
 
         evt_time_group = (
             self._get_date_trunc(
                 field_ref=cte.columns.get(GA.CTE_DATETIME_COL),
                 time_group=metric._time_group,
             )
             if metric._time_group != M.TimeGroup.TOTAL
             else SA.literal(None)
         )
 
         group_by = (
             cte.columns.get(GA.CTE_GROUP_COL)
-            if metric._group_by is not None
+            if metric._segment._group_by is not None
             else SA.literal(None)
         )
 
         return SA.select(
             columns=[
                 evt_time_group.label(GA.DATETIME_COL),
                 group_by.label(GA.GROUP_COL),
@@ -852,20 +852,25 @@
             ),
         )
 
     def _get_conversion_select(self, metric: M.ConversionMetric) -> Any:
         first_segment = metric._conversion._segments[0]
         first_cte = self._get_segment_sub_query_cte(
             self._get_segment_sub_query(first_segment, metric, step=0),
-            metric._group_by,
+            (
+                metric._conversion._segments[0]._group_by
+                if len(metric._conversion._segments)
+                else None
+            ),
             metric._resolution,
         )
         first_group_by = (
             first_cte.columns.get(GA.CTE_GROUP_COL)
-            if metric._group_by is not None
+            if len(metric._conversion._segments) > 0
+            and metric._conversion._segments[0]._group_by is not None
             else SA.literal(None)
         )
 
         time_group = metric._time_group
         if time_group != M.TimeGroup.TOTAL:
             first_evt_time_group = self._get_date_trunc(
                 field_ref=first_cte.columns.get(GA.CTE_DATETIME_COL),
@@ -938,25 +943,25 @@
                 else [SA.text(GA.DATETIME_COL), SA.text(GA.GROUP_COL)]
             ),
         ).select_from(joined_source)
 
     def _get_retention_select(self, metric: M.RetentionMetric) -> Any:
         initial_cte = self._get_segment_sub_query_cte(
             self._get_segment_sub_query(metric._initial_segment, metric, step=0),
-            metric._group_by,
+            metric._initial_segment._group_by,
             metric._resolution,
         )
 
         retention_index_cte = self._generate_retention_series_cte(
             metric._start_dt, metric._end_dt, metric._retention_window
         ).alias("ret_indeces")
 
         initial_group_by = (
             initial_cte.columns.get(GA.CTE_GROUP_COL)
-            if metric._group_by is not None
+            if metric._initial_segment._group_by is not None
             else SA.literal(None)
         )
 
         time_group = (
             self._get_date_trunc(
                 metric._time_group, initial_cte.columns.get(GA.CTE_DATETIME_COL)
             )
```

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.0rc3/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.0rc3/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/model.py` & `mitzu-0.6.0rc3/mitzu/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,14 @@
 from dateutil.relativedelta import relativedelta
 
 import mitzu.adapters.adapter_factory as factory
 import mitzu.adapters.generic_adapter as GA
 import mitzu.helper as helper
 import mitzu.notebook.model_loader as ML
 import mitzu.project_discovery as D
-import mitzu.visualization.charts as CHRT
-import mitzu.visualization.plot as PLT
 import mitzu.visualization.titles as TI
 import mitzu.project_serialization as PSE
 
 
 ANY_EVENT_NAME = "any_event"
 
 
@@ -1195,15 +1193,14 @@
 @dataclass()
 class MetricConfig:
     start_dt: Optional[datetime] = None
     end_dt: Optional[datetime] = None
     lookback_days: TimeWindow = DEF_LOOK_BACK_DAYS
     time_group: TimeGroup = DEF_TIME_GROUP
     max_group_count: int = DEF_MAX_GROUP_COUNT
-    group_by: Optional[EventFieldDef] = None
     custom_title: Optional[str] = None
     agg_type: Optional[AggType] = None
     agg_param: Optional[Any] = None
     chart_type: Optional[SimpleChartType] = None
     resolution: Resolution = Resolution.EVERY_EVENT
 
 
@@ -1229,18 +1226,14 @@
         return self._config.time_group
 
     @property
     def _resolution(self) -> Resolution:
         return self._config.resolution
 
     @property
-    def _group_by(self) -> Optional[EventFieldDef]:
-        return self._config.group_by
-
-    @property
     def _chart_type(self) -> Optional[SimpleChartType]:
         return self._config.chart_type
 
     @property
     def _custom_title(self) -> Optional[str]:
         return self._config.custom_title
 
@@ -1283,29 +1276,17 @@
 
     def get_df(self) -> pd.DataFrame:
         raise NotImplementedError()
 
     def get_sql(self) -> pd.DataFrame:
         raise NotImplementedError()
 
-    def get_title(self) -> str:
-        raise NotImplementedError()
-
     def print_sql(self):
         print(self.get_sql())
 
-    def get_figure(self):
-        chart = CHRT.get_simple_chart(self)
-        return PLT.plot_chart(chart, self)
-
-    def __repr__(self) -> str:
-        fig = self.get_figure()
-        fig.show(config={"displayModeBar": False})
-        return ""
-
 
 class ConversionMetric(Metric):
     _conversion: Conversion
     _conv_window: TimeWindow
 
     def __init__(
         self,
@@ -1321,21 +1302,14 @@
         project = helper.get_segment_project(self._conversion._segments[0])
         return project.get_adapter().get_conversion_df(self)
 
     def get_sql(self) -> pd.DataFrame:
         project = helper.get_segment_project(self._conversion._segments[0])
         return project.get_adapter().get_conversion_sql(self)
 
-    def get_figure(self):
-        chart = CHRT.get_simple_chart(self)
-        return PLT.plot_chart(chart, self)
-
-    def __repr__(self) -> str:
-        return super().__repr__()
-
     def get_project(self) -> Project:
         curr: Segment = self._conversion._segments[0]
         while not isinstance(curr, SimpleSegment):
             curr = cast(ComplexSegment, curr)._left
         return curr._left._project
 
     def get_title(self) -> str:
@@ -1354,17 +1328,14 @@
         project = helper.get_segment_project(self._segment)
         return project.get_adapter().get_segmentation_df(self)
 
     def get_sql(self) -> str:
         project = helper.get_segment_project(self._segment)
         return project.get_adapter().get_segmentation_sql(self)
 
-    def __repr__(self) -> str:
-        return super().__repr__()
-
     def get_project(self) -> Project:
         curr: Segment = self._segment
         while not isinstance(curr, SimpleSegment):
             curr = cast(ComplexSegment, curr)._left
         return curr._left._project
 
     def get_title(self) -> str:
@@ -1395,15 +1366,14 @@
         start_dt: Optional[str | datetime] = None,
         end_dt: Optional[str | datetime] = None,
         custom_title: Optional[str] = None,
         retention_window: Union[TimeWindow, str] = TimeWindow(
             value=1, period=TimeGroup.WEEK
         ),
         time_group: Union[str, TimeGroup] = TimeGroup.WEEK,
-        group_by: Optional[EventFieldDef] = None,
         max_group_by_count: int = DEF_MAX_GROUP_COUNT,
         lookback_days: Union[int, TimeWindow] = DEF_LOOK_BACK_DAYS,
         chart_type: Optional[Union[str, SimpleChartType]] = None,
         resolution: Union[str, Resolution] = Resolution.EVERY_EVENT,
     ) -> RetentionMetric:
         chart_type = chart_type
         if type(chart_type) == str:
@@ -1414,15 +1384,14 @@
             end_dt=helper.parse_datetime_input(end_dt, None),
             time_group=(
                 time_group
                 if type(time_group) == TimeGroup
                 else TimeGroup.parse(time_group)
             ),
             custom_title=custom_title,
-            group_by=group_by,
             max_group_count=max_group_by_count,
             lookback_days=(
                 lookback_days
                 if type(lookback_days) == TimeWindow
                 else TimeWindow(cast(int, lookback_days), TimeGroup.DAY)
             ),
             agg_type=AggType.RETENTION_RATE,
@@ -1442,17 +1411,14 @@
                 retention_window
                 if type(retention_window) == TimeWindow
                 else TimeWindow.parse(retention_window)
             ),
             config=config,
         )
 
-    def __repr__(self) -> str:
-        return super().__repr__()
-
     def get_df(self) -> pd.DataFrame:
         project = helper.get_segment_project(self._initial_segment)
         return project.get_adapter().get_retention_df(self)
 
     def get_sql(self) -> str:
         project = helper.get_segment_project(self._initial_segment)
         return project.get_adapter().get_retention_sql(self)
@@ -1479,15 +1445,14 @@
 
     def config(
         self,
         conv_window: Optional[Union[str, TimeWindow]] = DEF_CONV_WINDOW,
         start_dt: Optional[Union[str, datetime]] = None,
         end_dt: Optional[Union[str, datetime]] = None,
         time_group: Union[str, TimeGroup] = DEF_TIME_GROUP,
-        group_by: Optional[EventFieldDef] = None,
         max_group_by_count: int = DEF_MAX_GROUP_COUNT,
         lookback_days: Union[int, TimeWindow] = DEF_LOOK_BACK_DAYS,
         custom_title: Optional[str] = None,
         aggregation: Union[str, AggType] = AggType.CONVERSION,
         chart_type: Optional[Union[str, SimpleChartType]] = None,
         resolution: Union[str, Resolution] = Resolution.EVERY_EVENT,
     ) -> ConversionMetric:
@@ -1509,15 +1474,14 @@
             end_dt=helper.parse_datetime_input(end_dt, None),
             time_group=(
                 time_group
                 if type(time_group) == TimeGroup
                 else TimeGroup.parse(time_group)
             ),
             custom_title=custom_title,
-            group_by=group_by,
             max_group_count=max_group_by_count,
             lookback_days=(
                 lookback_days
                 if type(lookback_days) == TimeWindow
                 else TimeWindow(cast(int, lookback_days), TimeGroup.DAY)
             ),
             agg_type=agg_type,
@@ -1533,21 +1497,23 @@
         if conv_window is not None:
             conv_res = ConversionMetric(conversion=self._conversion, config=config)
             conv_res._conv_window = TimeWindow.parse(conv_window)
             return conv_res
         else:
             raise ValueError("conw_window or ret_window must be defined")
 
-    def __repr__(self) -> str:
-        return super().__repr__()
-
 
+@dataclass(frozen=True, init=False)
 class Segment(SegmentationMetric):
-    def __init__(self):
+
+    _group_by: Optional[EventFieldDef]
+
+    def __init__(self, _group_by: Optional[EventFieldDef] = None):
         super().__init__(self, config=MetricConfig())
+        object.__setattr__(self, "_group_by", _group_by)
 
     def __and__(self, right: Segment) -> ComplexSegment:
         return ComplexSegment(self, BinaryOperator.AND, right)
 
     def __or__(self, right: Segment) -> ComplexSegment:
         return ComplexSegment(self, BinaryOperator.OR, right)
 
@@ -1563,15 +1529,14 @@
         )
 
     def config(
         self,
         start_dt: Optional[Union[str, datetime]] = None,
         end_dt: Optional[Union[str, datetime]] = None,
         time_group: Union[str, TimeGroup] = DEF_TIME_GROUP,
-        group_by: Optional[EventFieldDef] = None,
         max_group_by_count: int = DEF_MAX_GROUP_COUNT,
         lookback_days: Union[int, TimeWindow] = DEF_LOOK_BACK_DAYS,
         custom_title: Optional[str] = None,
         aggregation: Union[str, AggType] = AggType.COUNT_UNIQUE_USERS,
         chart_type: Optional[Union[str, SimpleChartType]] = None,
     ) -> SegmentationMetric:
         agg_param = None
@@ -1589,72 +1554,77 @@
             end_dt=helper.parse_datetime_input(end_dt, None),
             time_group=(
                 time_group
                 if type(time_group) == TimeGroup
                 else TimeGroup.parse(time_group)
             ),
             custom_title=custom_title,
-            group_by=group_by,
             max_group_count=max_group_by_count,
             lookback_days=(
                 lookback_days
                 if type(lookback_days) == TimeWindow
                 else TimeWindow(cast(int, lookback_days), TimeGroup.DAY)
             ),
             agg_type=agg_type,
             agg_param=agg_param,
             resolution=Resolution.EVERY_EVENT,
             chart_type=cast(SimpleChartType, chart_type),
         )
 
         return SegmentationMetric(segment=self, config=config)
 
-    def __repr__(self) -> str:
-        return super().__repr__()
-
 
 @dataclass(init=False, frozen=True)
 class ComplexSegment(Segment):
     _left: Segment
     _operator: BinaryOperator
     _right: Segment
 
-    def __init__(self, _left: Segment, _operator: BinaryOperator, _right: Segment):
+    def __init__(
+        self,
+        _left: Segment,
+        _operator: BinaryOperator,
+        _right: Segment,
+        _group_by: Optional[EventFieldDef] = None,
+    ):
         object.__setattr__(self, "_left", _left)
         object.__setattr__(self, "_operator", _operator)
         object.__setattr__(self, "_right", _right)
-        super().__init__()
-
-    def __repr__(self) -> str:
-        return super().__repr__()
+        super().__init__(_group_by=_group_by)
 
     def __hash__(self) -> int:
         return hash(f"{hash(self._left)}{self._operator}{hash(self._right)}")
 
+    def group_by(self, grp_evt_field_def: EventFieldDef):
+        return ComplexSegment(
+            self._left, self._operator, self._right, grp_evt_field_def
+        )
+
 
 @dataclass(init=False, frozen=True)
 class SimpleSegment(Segment):
     _left: EventFieldDef | EventDef  # str is an event_name without any filters
     _operator: Optional[Operator] = None
     _right: Optional[Any] = None
 
     def __init__(
         self,
         _left: EventFieldDef | EventDef,
         _operator: Optional[Operator] = None,
         _right: Optional[Any] = None,
+        _group_by: Optional[EventFieldDef] = None,
     ):
         object.__setattr__(self, "_left", _left)
         object.__setattr__(self, "_operator", _operator)
         object.__setattr__(self, "_right", _right)
-        super().__init__()
-
-    def __repr__(self) -> str:
-        return super().__repr__()
+        super().__init__(_group_by=_group_by)
 
     def __hash__(self) -> int:
         event_property_name = (
             self._left._event_name
             if type(self._left) != EventFieldDef
             else f"{self._left._event_name}.{self._left._field._get_name()}"
         )
         return hash(f"{event_property_name}{self._operator}{self._right}")
+
+    def group_by(self, grp_evt_field_def: EventFieldDef):
+        return SimpleSegment(self._left, self._operator, self._right, grp_evt_field_def)
```

### Comparing `mitzu-0.6.0rc2/mitzu/notebook/model_loader.py` & `mitzu-0.6.0rc3/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/project_discovery.py` & `mitzu-0.6.0rc3/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/project_serialization.py` & `mitzu-0.6.0rc3/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/samples/__init__.py` & `mitzu-0.6.0rc3/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/samples/data_ingestion.py` & `mitzu-0.6.0rc3/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.0rc3/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/serialization.py` & `mitzu-0.6.0rc3/mitzu/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     if isinstance(value, M.MetricConfig):
         res = {
             "sdt": _to_dict(value.start_dt),
             "edt": _to_dict(value.end_dt),
             "lbd": _to_dict(value.lookback_days),
             "tg": _to_dict(value.time_group),
             "mgc": _to_dict(value.max_group_count),
-            "gb": _to_dict(value.group_by),
             "ct": _to_dict(value.custom_title),
             "cat": _to_dict(value.chart_type),
             "res": _to_dict(value.resolution),
         }
         if value.agg_type is not None:
             res["at"] = value.agg_type.to_agg_str(value.agg_param)
         return res
@@ -62,20 +61,22 @@
     if isinstance(value, M.EventFieldDef):
         return {"en": value._event_name, "f": _to_dict(value._field)}
     if isinstance(value, M.SimpleSegment):
         return {
             "l": _to_dict(value._left),
             "op": value._operator.name if value._operator is not None else None,
             "r": _to_dict(value._right) if value._right is not None else None,
+            "gb": _to_dict(value._group_by) if value._group_by is not None else None,
         }
     if isinstance(value, M.ComplexSegment):
         return {
             "l": _to_dict(value._left),
             "bop": value._operator.name,
             "r": _to_dict(value._right),
+            "gb": _to_dict(value._group_by) if value._group_by is not None else None,
         }
     if isinstance(value, M.Conversion):
         return {
             "segs": [_to_dict(seg) for seg in value._segments],
         }
     if isinstance(value, M.ConversionMetric):
         return {
@@ -152,17 +153,14 @@
             start_dt=_from_dict(value.get("sdt"), project, datetime, path + ".sdt"),
             end_dt=_from_dict(value.get("edt"), project, datetime, path + ".edt"),
             lookback_days=_from_dict(
                 value.get("lbd"), project, M.TimeWindow, path + ".lbd"
             ),
             time_group=_from_dict(value.get("tg"), project, M.TimeGroup, path + ".tg"),
             max_group_count=_from_dict(value.get("mgc"), project, int, path + ".mgc"),
-            group_by=_from_dict(
-                value.get("gb"), project, M.EventFieldDef, path + ".gb"
-            ),
             custom_title=_from_dict(value.get("ct"), project, str, path + ".ct"),
             resolution=_from_dict(
                 value.get("res"), project, M.Resolution, path + ".res"
             ),
             chart_type=_from_dict(
                 value.get("cat"), project, M.SimpleChartType, path + ".cat"
             ),
@@ -207,25 +205,39 @@
         if "bop" in value:
             return M.ComplexSegment(
                 _left=_from_dict(value.get("l"), project, M.Segment, path + ".l"),
                 _operator=_from_dict(
                     value.get("bop"), project, M.BinaryOperator, path + ".bop"
                 ),
                 _right=_from_dict(value.get("r"), project, M.Segment, path + ".r"),
+                _group_by=_from_dict(
+                    value.get("gb"), project, M.EventFieldDef, path + ".gb"
+                ),
             )
         elif "op" in value:
             return M.SimpleSegment(
                 _left=_from_dict(value.get("l"), project, EFD_OR_ED_TYPE, path + ".l"),
                 _operator=_from_dict(
                     value.get("op"), project, M.Operator, path + ".op"
                 ),
                 _right=_from_dict(value.get("r"), project, Any, path + ".r"),
+                _group_by=_from_dict(
+                    value.get("gb"), project, M.EventFieldDef, path + ".gb"
+                ),
             )
         return M.SimpleSegment(
-            _left=_from_dict(value.get("l"), project, EFD_OR_ED_TYPE, path + ".l")
+            _left=_from_dict(
+                value.get("l"),
+                project,
+                EFD_OR_ED_TYPE,
+                path + ".l",
+            ),
+            _group_by=_from_dict(
+                value.get("gb"), project, M.EventFieldDef, path + ".gb"
+            ),
         )
 
     if type_hint == M.EventFieldDef:
         event_name = value.get("en")
         edt = find_edt(project, event_name)
         return M.EventFieldDef(
             _event_name=_from_dict(event_name, project, str, path + ".en"),
```

### Comparing `mitzu-0.6.0rc2/mitzu/visualization/charts.py` & `mitzu-0.6.0rc3/mitzu/visualization/charts.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,38 +28,35 @@
         g_users = g_users.sort_values(order_by_col, ascending=False)
     g_users = g_users.head(max)
     top_groups = list(g_users[GA.GROUP_COL].values)
     return pdf[pdf[GA.GROUP_COL].isin(top_groups)]
 
 
 def get_color_label(metric: M.Metric):
-    if metric._group_by is not None:
-        return value_to_label(metric._group_by._field._get_name())
+    if (
+        isinstance(metric, M.SegmentationMetric)
+        and metric._segment._group_by is not None
+    ):
+        return value_to_label(metric._segment._group_by._field._get_name())
+    elif (
+        isinstance(metric, M.ConversionMetric)
+        and len(metric._conversion._segments) > 0
+        and metric._conversion._segments[0]._group_by
+    ):
+        return value_to_label(
+            metric._conversion._segments[0]._group_by._field._get_name()
+        )
     elif (
         isinstance(metric, M.RetentionMetric)
         and metric._chart_type == M.SimpleChartType.LINE
     ):
         return "Cohort"
     return ""
 
 
-def get_hover_mode(pdf: pd.DataFrame, metric: M.Metric) -> str:
-    group_count = len(list(pdf[C.COLOR_COL].values))
-    if metric._time_group == M.TimeGroup.TOTAL:
-        if metric._group_by is None:
-            return "x"
-        else:
-            return "closest" if group_count > 4 else "x"
-    else:
-        if metric._group_by is None:
-            return "x"
-        else:
-            return "closest" if group_count > 4 else "x"
-
-
 def get_default_chart_type(metric: M.Metric) -> M.SimpleChartType:
     if metric._time_group == M.TimeGroup.TOTAL:
         return M.SimpleChartType.BAR
     else:
         if isinstance(metric, M.SegmentationMetric) or isinstance(
             metric, M.ConversionMetric
         ):
@@ -165,15 +162,14 @@
 
     if isinstance(metric, M.SegmentationMetric):
         pdf = get_preprocessed_segmentation_dataframe(result_df, metric)
         return C.SimpleChart(
             x_axis_label="",
             y_axis_label=y_axis_label,
             color_label=color_label,
-            hover_mode=get_hover_mode(pdf, metric),
             chart_type=chart_type,
             title=TI.get_segmentation_title(metric),
             yaxis_ticksuffix="",
             dataframe=pdf,
             x_axis_labels_func=x_axis_label_func,
         )
 
@@ -182,15 +178,14 @@
         pdf = get_preprocessed_conversion_dataframe(result_df, metric, suffix)
         return C.SimpleChart(
             x_axis_label="",
             y_axis_label=y_axis_label,
             color_label=color_label,
             title=TI.get_conversion_title(metric),
             chart_type=chart_type,
-            hover_mode=get_hover_mode(pdf, metric),
             yaxis_ticksuffix=suffix,
             dataframe=pdf,
             x_axis_labels_func=x_axis_label_func,
         )
 
     if isinstance(metric, M.RetentionMetric):
         pdf = get_preprocessed_retention_dataframe(result_df, metric)
```

### Comparing `mitzu-0.6.0rc2/mitzu/visualization/common.py` & `mitzu-0.6.0rc3/mitzu/visualization/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 class SimpleChart:
 
     title: str
     x_axis_label: str
     y_axis_label: str
     color_label: str
     yaxis_ticksuffix: str
-    hover_mode: str
     chart_type: M.SimpleChartType
     dataframe: pd.DataFrame
+    hover_mode: str = "closest"
     x_axis_labels_func: Optional[Callable[[Any, M.Metric], Any]] = None
     y_axis_labels_func: Optional[Callable[[Any, M.Metric], Any]] = None
     color_labels_func: Optional[Callable[[Any, M.Metric], Any]] = None
 
     def __eq__(self, value: object) -> bool:
         if not isinstance(value, SimpleChart):
             return False
```

### Comparing `mitzu-0.6.0rc2/mitzu/visualization/labels.py` & `mitzu-0.6.0rc3/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/visualization/plot.py` & `mitzu-0.6.0rc3/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/visualization/titles.py` & `mitzu-0.6.0rc3/mitzu/visualization/titles.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,26 @@
         return (
             f"between <b>{format_date(metric,metric._start_dt)}</b> "
             f"and <b>{format_date(metric,metric._end_dt,1)}</b>"
         )
 
 
 def get_grouped_by_str(metric: M.Metric) -> str:
-    if metric._group_by:
-        grp = metric._group_by._field._name
+    grp_field = None
+    if isinstance(metric, M.SegmentationMetric):
+        grp_field = metric._segment._group_by
+    elif (
+        isinstance(metric, M.ConversionMetric) and len(metric._conversion._segments) > 0
+    ):
+        grp_field = metric._conversion._segments[0]._group_by
+    elif isinstance(metric, M.RetentionMetric):
+        grp_field = metric._initial_segment._group_by
+
+    if grp_field is not None:
+        grp = grp_field._field._name
         return f"grouped by <b>{grp}</b> (top {metric._max_group_count})"
     return ""
 
 
 def fix_title_text(title_text: str, max_length=MAX_SEGMENT_LENGTH) -> str:
     if len(title_text) > max_length:
         return title_text[:max_length] + "..."
@@ -90,15 +100,15 @@
         return metric._config.custom_title
     segment_str = fix_title_text(get_segment_title_text(metric._segment))
     tg = get_time_group_text(metric._time_group).title()
     lines = [
         f"{tg} count of unique users",
         f"who did {segment_str}",
     ]
-    if metric._group_by is not None:
+    if metric._segment._group_by is not None:
         lines.append(get_grouped_by_str(metric))
     lines.append(get_timeframe_str(metric))
     return "<br />".join(lines)
 
 
 def get_conversion_title(metric: M.ConversionMetric) -> str:
     if metric._config.custom_title is not None:
```

### Comparing `mitzu-0.6.0rc2/mitzu/visualization/tooltips.py` & `mitzu-0.6.0rc3/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/visualization/transform_conv.py` & `mitzu-0.6.0rc3/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/visualization/transform_retention.py` & `mitzu-0.6.0rc3/mitzu/visualization/transform_retention.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     if metric._time_group == M.TimeGroup.TOTAL:
         mapping = {
             GA.RETENTION_INDEX: C.X_AXIS_COL,
             GA.AGG_VALUE_COL: C.Y_AXIS_COL,
             GA.GROUP_COL: C.COLOR_COL,
         }
     else:
-        if metric._group_by is not None:
+        if metric._initial_segment._group_by is not None:
             raise Exception(
                 "Break downs are not supported for retention over time metric"
             )
         mapping = {
             GA.RETENTION_INDEX: C.X_AXIS_COL,
             GA.AGG_VALUE_COL: C.Y_AXIS_COL,
             GA.DATETIME_COL: C.COLOR_COL,
```

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/.DS_Store` & `mitzu-0.6.0rc3/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.0rc3/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.0rc3/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/logo.png` & `mitzu-0.6.0rc3/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.0rc3/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.0rc3/mitzu/webapp/auth/authorizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,18 +203,21 @@
 
     def _validate_token(self, token: str) -> Optional[Dict]:
         try:
             claims = jwt.decode(
                 token, self._config.token_signing_key, algorithms=[JWT_ALGORITHM]
             )
 
-            user_id = claims["sub"]
-            user = self._config.user_service.get_user_by_id(user_id)
+            token_subject = claims["sub"]
+            user = self._config.user_service.get_user_by_id(token_subject)
             if user is None:
-                raise Exception("User not found")
+                # SSO tokens contains the email not the use id
+                user = self._config.user_service.get_user_by_email(token_subject)
+                if user is None:
+                    raise Exception("User not found")
             claims[JWT_CLAIM_ROLE] = user.role
             return claims
         except Exception as e:
             LOGGER.warning(f"Failed to validate token: {str(e)}")
             return None
 
     def _validate_foreign_token(self, token) -> Optional[str]:
```

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.0rc3/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.0rc3/mitzu/webapp/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/auth/google.py` & `mitzu-0.6.0rc3/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/cache.py` & `mitzu-0.6.0rc3/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.0rc3/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/configs.py` & `mitzu-0.6.0rc3/mitzu/webapp/configs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/dependencies.py` & `mitzu-0.6.0rc3/mitzu/webapp/dependencies.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/helper.py` & `mitzu-0.6.0rc3/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/model.py` & `mitzu-0.6.0rc3/mitzu/webapp/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/offcanvas.py` & `mitzu-0.6.0rc3/mitzu/webapp/offcanvas.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/connections_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/dashboards.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/dashboards.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/edit_user.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import mitzu.webapp.pages.explore.metric_type_handler as MTH
 from dash import html
 from mitzu.webapp.helper import (
     CHILDREN,
     get_event_names,
     get_property_name_label,
     WITH_VALUE_CLS,
+    find_event_field_def,
 )
 import dash_mantine_components as dmc
 
 COMPLEX_SEGMENT = "complex_segment"
 COMPLEX_SEGMENT_BODY = "complex_segment_body"
 COMPLEX_SEGMENT_FOOTER = "complex_segment_footer"
 COMPLEX_SEGMENT_GROUP_BY = "complex_segment_group_by"
@@ -44,21 +45,19 @@
                 )
     options.sort(key=lambda v: ".".join(v["value"].split(".")[1:]))
     return options
 
 
 def create_group_by_dropdown(
     index: str,
-    metric: Optional[M.Metric],
     segment: M.Segment,
     discovered_project: M.DiscoveredProject,
 ) -> dmc.Select:
     event_names = get_event_names(segment)
-    group_by_efd = metric._config.group_by if metric is not None else None
-
+    group_by_efd = segment._group_by
     value = None
     if group_by_efd is not None:
         value = f"{group_by_efd._event_name}.{group_by_efd._field._get_name()}"
 
     options = get_group_by_options(discovered_project, event_names)
     if value not in [v["value"] for v in options]:
         value = None
@@ -128,15 +127,15 @@
         and funnel_step == 0
         and not (
             isinstance(metric, M.RetentionMetric)
             and metric._time_group != M.TimeGroup.TOTAL
         )
     ):
         group_by_dd = html.Div(
-            [create_group_by_dropdown(type_index, metric, segment, discovered_project)],
+            [create_group_by_dropdown(type_index, segment, discovered_project)],
             className=COMPLEX_SEGMENT_FOOTER,
         )
         body_children.append(group_by_dd)
 
     card_body = dbc.CardBody(
         children=body_children,
         className=COMPLEX_SEGMENT_BODY + " fw-normal p-0",
@@ -160,8 +159,18 @@
         if event_segment is None:
             continue
         if res_segment is None:
             res_segment = event_segment
         else:
             res_segment = res_segment | event_segment
 
+    if res_segment is not None:
+        gp = complex_segment.get(COMPLEX_SEGMENT_GROUP_BY)
+        group_by = find_event_field_def(gp, discovered_project) if gp else None
+        if group_by is not None:
+            group_by._project._discovered_project.set_value(discovered_project)
+            if isinstance(res_segment, M.SimpleSegment) or isinstance(
+                res_segment, M.ComplexSegment
+            ):
+                res_segment = res_segment.group_by(group_by)
+
     return res_segment
```

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/explore_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,25 +5,19 @@
 
 import dash.development.base_component as bc
 import dash_bootstrap_components as dbc
 import mitzu.model as M
 from mitzu.helper import parse_datetime_input
 
 import mitzu.webapp.pages.explore.dates_selector_handler as DS
-import mitzu.webapp.pages.explore.complex_segment_handler as CS
 import mitzu.webapp.pages.explore.metric_type_handler as MTH
 import mitzu.webapp.pages.explore.toolbar_handler as TH
 from dash import html, ctx
 import dash_mantine_components as dmc
-from mitzu.webapp.helper import (
-    CHILDREN,
-    METRIC_SEGMENTS,
-    find_event_field_def,
-    value_to_label,
-)
+from mitzu.webapp.helper import value_to_label
 
 METRICS_CONFIG_CONTAINER = "metrics_config_container"
 
 TIME_WINDOW = "time_window"
 TIME_WINDOW_INTERVAL = "time_window_interval"
 TIME_WINDOW_INTERVAL_STEPS = "time_window_interval_steps"
 AGGREGATION_TYPE = "aggregation_type"
@@ -307,31 +301,19 @@
                 all_inputs.get(TIME_WINDOW_INTERVAL_STEPS, M.TimeGroup.DAY)
             ),
         )
 
     chart_type_val = all_inputs.get(TH.CHART_TYPE_DD, None)
     chart_type = M.SimpleChartType.parse(chart_type_val)
 
-    group_by: Optional[M.EventFieldDef] = None
-    if discovered_project is not None:
-        group_by_paths = all_inputs[METRIC_SEGMENTS][CHILDREN]
-        if len(group_by_paths) >= 1 and not (
-            metric_type == MTH.MetricType.RETENTION and time_group != M.TimeGroup.TOTAL
-        ):
-            gp = group_by_paths[0].get(CS.COMPLEX_SEGMENT_GROUP_BY)
-            group_by = find_event_field_def(gp, discovered_project) if gp else None
-            if group_by is not None:
-                group_by._project._discovered_project.set_value(discovered_project)
-
     res_config = M.MetricConfig(
         start_dt=parse_datetime_input(start_dt, None),
         end_dt=parse_datetime_input(end_dt, None),
         lookback_days=lookback_days,
         time_group=time_group,
         agg_type=agg_type,
         agg_param=agg_param,
         chart_type=chart_type,
         resolution=resolution,
-        group_by=group_by,
         custom_title="",
     )
     return res_config, time_window
```

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/home.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/home.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/login.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/login.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/manage_connection.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/manage_event_defs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/manage_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/paths.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/projects_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/pages/users.py` & `mitzu-0.6.0rc3/mitzu/webapp/pages/users.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/service/events_service.py` & `mitzu-0.6.0rc3/mitzu/webapp/service/events_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.0rc3/mitzu/webapp/service/navbar_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.0rc3/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/service/user_service.py` & `mitzu-0.6.0rc3/mitzu/webapp/service/user_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/storage.py` & `mitzu-0.6.0rc3/mitzu/webapp/storage.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/storage_model.py` & `mitzu-0.6.0rc3/mitzu/webapp/storage_model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/toast.py` & `mitzu-0.6.0rc3/mitzu/webapp/toast.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/mitzu/webapp/webapp.py` & `mitzu-0.6.0rc3/mitzu/webapp/webapp.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc2/pyproject.toml` & `mitzu-0.6.0rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.0-rc.2"
+version = "0.6.0-rc.3"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
@@ -67,15 +67,14 @@
 
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.982"
 pytest = "^6.2.5"
 black = "^22.1.0"
 pytest-cov = "^3.0.0"
-jupyterlab = "^3.4.2"
 apig-wsgi = "^2.14.0"
 types-python-dateutil = "^2.8.18"
 flake8 = "^5.0.4"
 autoflake = "^1.4"
 types-requests = "^2.28.8"
 freezegun = "^1.2.2"
 pyclean = "^2.2.0"
```

### Comparing `mitzu-0.6.0rc2/PKG-INFO` & `mitzu-0.6.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.0rc2
+Version: 0.6.0rc3
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

