# Comparing `tmp/data_diff-0.7.3.tar.gz` & `tmp/data_diff-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_diff-0.7.3.tar", max compression
+gzip compressed data, was "data_diff-0.7.4.tar", max compression
```

## Comparing `data_diff-0.7.3.tar` & `data_diff-0.7.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.3/LICENSE
--rw-r--r--   0        0        0     4773 2023-04-14 15:23:33.906410 data_diff-0.7.3/README.md
--rw-r--r--   0        0        0     8429 2023-04-21 21:58:08.193898 data_diff-0.7.3/data_diff/__init__.py
--rw-r--r--   0        0        0    15816 2023-04-21 21:58:08.194100 data_diff-0.7.3/data_diff/__main__.py
--rw-r--r--   0        0        0      108 2023-04-14 15:23:33.906548 data_diff-0.7.3/data_diff/cloud/__init__.py
--rw-r--r--   0        0        0    11594 2023-04-21 21:58:08.194331 data_diff-0.7.3/data_diff/cloud/data_source.py
--rw-r--r--   0        0        0     9253 2023-04-21 21:58:08.194472 data_diff-0.7.3/data_diff/cloud/datafold_api.py
--rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.3/data_diff/config.py
--rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.3/data_diff/databases/__init__.py
--rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.3/data_diff/databases/_connect.py
--rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.3/data_diff/databases/base.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.3/data_diff/databases/bigquery.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.3/data_diff/databases/clickhouse.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.3/data_diff/databases/databricks.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.3/data_diff/databases/duckdb.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.3/data_diff/databases/mysql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.3/data_diff/databases/oracle.py
--rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.3/data_diff/databases/postgresql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.3/data_diff/databases/presto.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.3/data_diff/databases/redshift.py
--rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.3/data_diff/databases/snowflake.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.3/data_diff/databases/trino.py
--rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.3/data_diff/databases/vertica.py
--rw-r--r--   0        0        0    14002 2023-04-21 21:58:08.196463 data_diff-0.7.3/data_diff/dbt.py
--rw-r--r--   0        0        0    13759 2023-04-21 21:58:08.196614 data_diff-0.7.3/data_diff/dbt_parser.py
--rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.3/data_diff/diff_tables.py
--rw-r--r--   0        0        0     8567 2023-04-21 21:58:08.196909 data_diff-0.7.3/data_diff/hashdiff_tables.py
--rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.3/data_diff/info_tree.py
--rw-r--r--   0        0        0    14768 2023-04-21 21:58:08.197074 data_diff-0.7.3/data_diff/joindiff_tables.py
--rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.3/data_diff/lexicographic_space.py
--rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.3/data_diff/parse_time.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.3/data_diff/query_utils.py
--rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.3/data_diff/sqeleton/__init__.py
--rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.3/data_diff/sqeleton/__main__.py
--rw-r--r--   0        0        0      254 2023-04-21 21:58:08.197672 data_diff-0.7.3/data_diff/sqeleton/abcs/__init__.py
--rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.3/data_diff/sqeleton/abcs/compiler.py
--rw-r--r--   0        0        0    10339 2023-04-21 21:58:08.197842 data_diff-0.7.3/data_diff/sqeleton/abcs/database_types.py
--rw-r--r--   0        0        0     5909 2023-04-21 21:58:08.197929 data_diff-0.7.3/data_diff/sqeleton/abcs/mixins.py
--rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.3/data_diff/sqeleton/bound_exprs.py
--rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.3/data_diff/sqeleton/databases/__init__.py
--rw-r--r--   0        0        0     9131 2023-04-21 21:58:08.198249 data_diff-0.7.3/data_diff/sqeleton/databases/_connect.py
--rw-r--r--   0        0        0    19920 2023-04-21 21:58:08.198404 data_diff-0.7.3/data_diff/sqeleton/databases/base.py
--rw-r--r--   0        0        0     7140 2023-04-21 21:58:08.198520 data_diff-0.7.3/data_diff/sqeleton/databases/bigquery.py
--rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.3/data_diff/sqeleton/databases/clickhouse.py
--rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.3/data_diff/sqeleton/databases/databricks.py
--rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.3/data_diff/sqeleton/databases/duckdb.py
--rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.3/data_diff/sqeleton/databases/mssql.py
--rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.3/data_diff/sqeleton/databases/mysql.py
--rw-r--r--   0        0        0     6523 2023-04-21 21:58:08.199025 data_diff-0.7.3/data_diff/sqeleton/databases/oracle.py
--rw-r--r--   0        0        0     5430 2023-04-21 21:58:08.199106 data_diff-0.7.3/data_diff/sqeleton/databases/postgresql.py
--rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.3/data_diff/sqeleton/databases/presto.py
--rw-r--r--   0        0        0     4844 2023-04-21 21:58:08.199284 data_diff-0.7.3/data_diff/sqeleton/databases/redshift.py
--rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.3/data_diff/sqeleton/databases/snowflake.py
--rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.3/data_diff/sqeleton/databases/trino.py
--rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.3/data_diff/sqeleton/databases/vertica.py
--rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.3/data_diff/sqeleton/queries/__init__.py
--rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.3/data_diff/sqeleton/queries/api.py
--rw-r--r--   0        0        0    30646 2023-04-21 21:58:08.199945 data_diff-0.7.3/data_diff/sqeleton/queries/ast_classes.py
--rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.3/data_diff/sqeleton/queries/base.py
--rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.3/data_diff/sqeleton/queries/compiler.py
--rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.3/data_diff/sqeleton/queries/extras.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.3/data_diff/sqeleton/query_utils.py
--rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.3/data_diff/sqeleton/repl.py
--rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.3/data_diff/sqeleton/schema.py
--rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.3/data_diff/sqeleton/utils.py
--rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.3/data_diff/table_segment.py
--rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.3/data_diff/thread_utils.py
--rw-r--r--   0        0        0     4121 2023-04-15 23:11:48.035287 data_diff-0.7.3/data_diff/tracking.py
--rw-r--r--   0        0        0     4306 2023-04-14 15:23:33.907379 data_diff-0.7.3/data_diff/utils.py
--rw-r--r--   0        0        0       22 2023-04-21 21:58:08.200716 data_diff-0.7.3/data_diff/version.py
--rwxr-xr-x   0        0        0     2865 2023-04-21 21:58:08.202087 data_diff-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     7387 1970-01-01 00:00:00.000000 data_diff-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.4/LICENSE
+-rw-r--r--   0        0        0     4773 2023-04-14 15:23:33.906410 data_diff-0.7.4/README.md
+-rw-r--r--   0        0        0     8429 2023-04-21 21:58:08.193898 data_diff-0.7.4/data_diff/__init__.py
+-rw-r--r--   0        0        0    15816 2023-04-21 21:58:08.194100 data_diff-0.7.4/data_diff/__main__.py
+-rw-r--r--   0        0        0      108 2023-04-14 15:23:33.906548 data_diff-0.7.4/data_diff/cloud/__init__.py
+-rw-r--r--   0        0        0    11594 2023-04-21 21:58:08.194331 data_diff-0.7.4/data_diff/cloud/data_source.py
+-rw-r--r--   0        0        0     9253 2023-04-21 21:58:08.194472 data_diff-0.7.4/data_diff/cloud/datafold_api.py
+-rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.4/data_diff/config.py
+-rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.4/data_diff/databases/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.4/data_diff/databases/_connect.py
+-rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.4/data_diff/databases/base.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.4/data_diff/databases/bigquery.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.4/data_diff/databases/clickhouse.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.4/data_diff/databases/databricks.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.4/data_diff/databases/duckdb.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.4/data_diff/databases/mysql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.4/data_diff/databases/oracle.py
+-rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.4/data_diff/databases/postgresql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.4/data_diff/databases/presto.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.4/data_diff/databases/redshift.py
+-rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.4/data_diff/databases/snowflake.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.4/data_diff/databases/trino.py
+-rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.4/data_diff/databases/vertica.py
+-rw-r--r--   0        0        0    13213 2023-04-25 22:24:15.790768 data_diff-0.7.4/data_diff/dbt.py
+-rw-r--r--   0        0        0    13945 2023-04-25 22:24:15.790989 data_diff-0.7.4/data_diff/dbt_parser.py
+-rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.4/data_diff/diff_tables.py
+-rw-r--r--   0        0        0     8567 2023-04-21 21:58:08.196909 data_diff-0.7.4/data_diff/hashdiff_tables.py
+-rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.4/data_diff/info_tree.py
+-rw-r--r--   0        0        0    14768 2023-04-21 21:58:08.197074 data_diff-0.7.4/data_diff/joindiff_tables.py
+-rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.4/data_diff/lexicographic_space.py
+-rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.4/data_diff/parse_time.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.4/data_diff/query_utils.py
+-rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.4/data_diff/sqeleton/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.4/data_diff/sqeleton/__main__.py
+-rw-r--r--   0        0        0      254 2023-04-21 21:58:08.197672 data_diff-0.7.4/data_diff/sqeleton/abcs/__init__.py
+-rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.4/data_diff/sqeleton/abcs/compiler.py
+-rw-r--r--   0        0        0    10339 2023-04-21 21:58:08.197842 data_diff-0.7.4/data_diff/sqeleton/abcs/database_types.py
+-rw-r--r--   0        0        0     5909 2023-04-21 21:58:08.197929 data_diff-0.7.4/data_diff/sqeleton/abcs/mixins.py
+-rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.4/data_diff/sqeleton/bound_exprs.py
+-rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.4/data_diff/sqeleton/databases/__init__.py
+-rw-r--r--   0        0        0     9131 2023-04-21 21:58:08.198249 data_diff-0.7.4/data_diff/sqeleton/databases/_connect.py
+-rw-r--r--   0        0        0    19920 2023-04-21 21:58:08.198404 data_diff-0.7.4/data_diff/sqeleton/databases/base.py
+-rw-r--r--   0        0        0     7140 2023-04-21 21:58:08.198520 data_diff-0.7.4/data_diff/sqeleton/databases/bigquery.py
+-rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.4/data_diff/sqeleton/databases/clickhouse.py
+-rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.4/data_diff/sqeleton/databases/databricks.py
+-rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.4/data_diff/sqeleton/databases/duckdb.py
+-rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.4/data_diff/sqeleton/databases/mssql.py
+-rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.4/data_diff/sqeleton/databases/mysql.py
+-rw-r--r--   0        0        0     6523 2023-04-21 21:58:08.199025 data_diff-0.7.4/data_diff/sqeleton/databases/oracle.py
+-rw-r--r--   0        0        0     5430 2023-04-21 21:58:08.199106 data_diff-0.7.4/data_diff/sqeleton/databases/postgresql.py
+-rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.4/data_diff/sqeleton/databases/presto.py
+-rw-r--r--   0        0        0     4844 2023-04-21 21:58:08.199284 data_diff-0.7.4/data_diff/sqeleton/databases/redshift.py
+-rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.4/data_diff/sqeleton/databases/snowflake.py
+-rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.4/data_diff/sqeleton/databases/trino.py
+-rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.4/data_diff/sqeleton/databases/vertica.py
+-rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.4/data_diff/sqeleton/queries/__init__.py
+-rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.4/data_diff/sqeleton/queries/api.py
+-rw-r--r--   0        0        0    30646 2023-04-21 21:58:08.199945 data_diff-0.7.4/data_diff/sqeleton/queries/ast_classes.py
+-rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.4/data_diff/sqeleton/queries/base.py
+-rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.4/data_diff/sqeleton/queries/compiler.py
+-rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.4/data_diff/sqeleton/queries/extras.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.4/data_diff/sqeleton/query_utils.py
+-rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.4/data_diff/sqeleton/repl.py
+-rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.4/data_diff/sqeleton/schema.py
+-rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.4/data_diff/sqeleton/utils.py
+-rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.4/data_diff/table_segment.py
+-rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.4/data_diff/thread_utils.py
+-rw-r--r--   0        0        0     4121 2023-04-15 23:11:48.035287 data_diff-0.7.4/data_diff/tracking.py
+-rw-r--r--   0        0        0     4306 2023-04-14 15:23:33.907379 data_diff-0.7.4/data_diff/utils.py
+-rw-r--r--   0        0        0       22 2023-04-25 22:24:15.791131 data_diff-0.7.4/data_diff/version.py
+-rwxr-xr-x   0        0        0     2865 2023-04-25 22:24:15.791298 data_diff-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     7387 1970-01-01 00:00:00.000000 data_diff-0.7.4/PKG-INFO
```

### Comparing `data_diff-0.7.3/LICENSE` & `data_diff-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/README.md` & `data_diff-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/__init__.py` & `data_diff-0.7.4/data_diff/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/__main__.py` & `data_diff-0.7.4/data_diff/__main__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/cloud/data_source.py` & `data_diff-0.7.4/data_diff/cloud/data_source.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/cloud/datafold_api.py` & `data_diff-0.7.4/data_diff/cloud/datafold_api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/config.py` & `data_diff-0.7.4/data_diff/config.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/databases/_connect.py` & `data_diff-0.7.4/data_diff/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/dbt.py` & `data_diff-0.7.4/data_diff/dbt.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import List, Optional, Dict
 from .utils import dbt_diff_string_template, getLogger
 from pathlib import Path
 
 import keyring
 
 from .cloud import DatafoldAPI, TCloudApiDataDiff, get_or_create_data_source
-from .dbt_parser import DbtParser
+from .dbt_parser import DbtParser, PROJECT_FILE
 
 
 logger = getLogger(__name__)
 
 
 def import_dbt():
     try:
@@ -38,37 +38,14 @@
     create_start_event_json,
     send_event_json,
     is_tracking_enabled,
 )
 from .utils import run_as_daemon, truncate_error
 from . import connect_to_table, diff_tables, Algorithm
 
-RUN_RESULTS_PATH = "target/run_results.json"
-MANIFEST_PATH = "target/manifest.json"
-PROJECT_FILE = "dbt_project.yml"
-PROFILES_FILE = "profiles.yml"
-LOWER_DBT_V = "1.0.0"
-UPPER_DBT_V = "1.4.6"
-
-
-# https://github.com/dbt-labs/dbt-core/blob/c952d44ec5c2506995fbad75320acbae49125d3d/core/dbt/cli/resolvers.py#L6
-def default_project_dir() -> Path:
-    paths = list(Path.cwd().parents)
-    paths.insert(0, Path.cwd())
-    return next((x for x in paths if (x / PROJECT_FILE).exists()), Path.cwd())
-
-
-# https://github.com/dbt-labs/dbt-core/blob/c952d44ec5c2506995fbad75320acbae49125d3d/core/dbt/cli/resolvers.py#L12
-def default_profiles_dir() -> Path:
-    return Path.cwd() if (Path.cwd() / PROFILES_FILE).exists() else Path.home() / ".dbt"
-
-
-def legacy_profiles_dir() -> Path:
-    return Path.home() / ".dbt"
-
 
 @dataclass
 class DiffVars:
     dev_path: List[str]
     prod_path: List[str]
     primary_keys: List[str]
     connection: Dict[str, str]
```

### Comparing `data_diff-0.7.3/data_diff/dbt_parser.py` & `data_diff-0.7.4/data_diff/dbt_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,18 @@
         self.dbt_version = self.manifest_obj.metadata.dbt_version
         self.dbt_project_id = self.manifest_obj.metadata.project_id
         self.requires_upper = False
         self.threads = None
         self.unique_columns = self.get_unique_columns()
 
     def get_datadiff_variables(self) -> dict:
-        vars = get_from_dict_with_raise(self.project_dict, "vars", f"No vars: found in dbt_project.yml.")
-        return get_from_dict_with_raise(vars, "data_diff", f"data_diff: section not found in dbt_project.yml vars:.")
+        doc_url = "https://docs.datafold.com/development_testing/open_source#configure-your-dbt-project"
+        error_message = f"vars: data_diff: section not found in dbt_project.yml.\n\nTo solve this, please configure your dbt project: \n{doc_url}\n"
+        vars = get_from_dict_with_raise(self.project_dict, "vars", error_message)
+        return get_from_dict_with_raise(vars, "data_diff", error_message)
 
     def get_models(self):
         with open(self.project_dir / RUN_RESULTS_PATH) as run_results:
             logger.info(f"Parsing file {RUN_RESULTS_PATH}")
             run_results_dict = json.load(run_results)
             run_results_obj = self.parse_run_results(run_results=run_results_dict)
```

### Comparing `data_diff-0.7.3/data_diff/diff_tables.py` & `data_diff-0.7.4/data_diff/diff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/hashdiff_tables.py` & `data_diff-0.7.4/data_diff/hashdiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/info_tree.py` & `data_diff-0.7.4/data_diff/info_tree.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/joindiff_tables.py` & `data_diff-0.7.4/data_diff/joindiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/lexicographic_space.py` & `data_diff-0.7.4/data_diff/lexicographic_space.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/parse_time.py` & `data_diff-0.7.4/data_diff/parse_time.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/query_utils.py` & `data_diff-0.7.4/data_diff/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/abcs/database_types.py` & `data_diff-0.7.4/data_diff/sqeleton/abcs/database_types.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/abcs/mixins.py` & `data_diff-0.7.4/data_diff/sqeleton/abcs/mixins.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/bound_exprs.py` & `data_diff-0.7.4/data_diff/sqeleton/bound_exprs.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/__init__.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/_connect.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/base.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/base.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/bigquery.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/bigquery.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/clickhouse.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/clickhouse.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/databricks.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/databricks.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/duckdb.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/mssql.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/mysql.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/oracle.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/oracle.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/postgresql.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/presto.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/presto.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/redshift.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/redshift.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/snowflake.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/trino.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/trino.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/databases/vertica.py` & `data_diff-0.7.4/data_diff/sqeleton/databases/vertica.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/queries/api.py` & `data_diff-0.7.4/data_diff/sqeleton/queries/api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/queries/ast_classes.py` & `data_diff-0.7.4/data_diff/sqeleton/queries/ast_classes.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/queries/compiler.py` & `data_diff-0.7.4/data_diff/sqeleton/queries/compiler.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/queries/extras.py` & `data_diff-0.7.4/data_diff/sqeleton/queries/extras.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/query_utils.py` & `data_diff-0.7.4/data_diff/sqeleton/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/repl.py` & `data_diff-0.7.4/data_diff/sqeleton/repl.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/schema.py` & `data_diff-0.7.4/data_diff/sqeleton/schema.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/sqeleton/utils.py` & `data_diff-0.7.4/data_diff/sqeleton/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/table_segment.py` & `data_diff-0.7.4/data_diff/table_segment.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/thread_utils.py` & `data_diff-0.7.4/data_diff/thread_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/tracking.py` & `data_diff-0.7.4/data_diff/tracking.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/data_diff/utils.py` & `data_diff-0.7.4/data_diff/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.3/pyproject.toml` & `data_diff-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-diff"
-version = "0.7.3"
+version = "0.7.4"
 description = "Command-line tool and Python library to efficiently diff rows across two different databases."
 authors = ["Datafold <data-diff@datafold.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/datafold/data-diff"
 documentation = ""
 classifiers = [
```

### Comparing `data_diff-0.7.3/PKG-INFO` & `data_diff-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-diff
-Version: 0.7.3
+Version: 0.7.4
 Summary: Command-line tool and Python library to efficiently diff rows across two different databases.
 Home-page: https://github.com/datafold/data-diff
 License: MIT
 Author: Datafold
 Author-email: data-diff@datafold.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

