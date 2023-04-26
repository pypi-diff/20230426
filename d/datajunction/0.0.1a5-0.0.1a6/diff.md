# Comparing `tmp/datajunction-0.0.1a5.tar.gz` & `tmp/datajunction-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datajunction-0.0.1a5.tar", max compression
+gzip compressed data, was "datajunction-0.0.1a6.tar", max compression
```

## Comparing `datajunction-0.0.1a5.tar` & `datajunction-0.0.1a6.tar`

### file list

```diff
@@ -1,66 +1,7 @@
--rw-r--r--   0        0        0     1081 2023-03-09 19:29:41.743091 datajunction-0.0.1a5/LICENSE.txt
--rw-r--r--   0        0        0     5589 2023-03-09 19:29:41.743202 datajunction-0.0.1a5/README.rst
--rw-r--r--   0        0        0      384 2023-03-09 22:42:36.169164 datajunction-0.0.1a5/dj/__init__.py
--rw-r--r--   0        0        0        0 2023-03-09 19:29:41.770645 datajunction-0.0.1a5/dj/api/__init__.py
--rw-r--r--   0        0        0     4692 2023-04-13 18:17:17.325178 datajunction-0.0.1a5/dj/api/attributes.py
--rw-r--r--   0        0        0     2862 2023-04-13 18:17:17.325699 datajunction-0.0.1a5/dj/api/catalogs.py
--rw-r--r--   0        0        0      654 2023-04-13 18:17:17.326024 datajunction-0.0.1a5/dj/api/cubes.py
--rw-r--r--   0        0        0     5036 2023-04-16 15:31:28.665337 datajunction-0.0.1a5/dj/api/data.py
--rw-r--r--   0        0        0     1457 2023-04-16 03:55:14.641955 datajunction-0.0.1a5/dj/api/engines.py
--rw-r--r--   0        0        0     1220 2023-04-13 18:17:17.327030 datajunction-0.0.1a5/dj/api/health.py
--rw-r--r--   0        0        0    12980 2023-04-16 15:31:28.665743 datajunction-0.0.1a5/dj/api/helpers.py
--rw-r--r--   0        0        0     3061 2023-04-17 19:39:28.361836 datajunction-0.0.1a5/dj/api/main.py
--rw-r--r--   0        0        0     2781 2023-04-13 18:17:17.327629 datajunction-0.0.1a5/dj/api/metrics.py
--rw-r--r--   0        0        0     2205 2023-04-17 19:39:28.362005 datajunction-0.0.1a5/dj/api/namespaces.py
--rw-r--r--   0        0        0    30136 2023-04-17 19:39:28.362281 datajunction-0.0.1a5/dj/api/nodes.py
--rw-r--r--   0        0        0      702 2023-04-13 18:17:17.328235 datajunction-0.0.1a5/dj/api/query.py
--rw-r--r--   0        0        0     1345 2023-04-16 15:31:28.666447 datajunction-0.0.1a5/dj/api/sql.py
--rw-r--r--   0        0        0     3358 2023-04-13 18:17:17.328723 datajunction-0.0.1a5/dj/api/tags.py
--rw-r--r--   0        0        0     2239 2023-04-13 18:17:17.329272 datajunction-0.0.1a5/dj/config.py
--rw-r--r--   0        0        0      412 2023-03-09 19:29:41.772659 datajunction-0.0.1a5/dj/constants.py
--rwxr-xr-x   0        0        0        0 2023-03-09 19:29:41.772720 datajunction-0.0.1a5/dj/construction/__init__.py
--rwxr-xr-x   0        0        0    18129 2023-04-16 15:31:28.666684 datajunction-0.0.1a5/dj/construction/build.py
--rw-r--r--   0        0        0     6561 2023-04-06 15:30:00.095444 datajunction-0.0.1a5/dj/construction/dj_query.py
--rwxr-xr-x   0        0        0     1495 2023-03-09 19:29:41.773112 datajunction-0.0.1a5/dj/construction/exceptions.py
--rwxr-xr-x   0        0        0     2679 2023-04-06 15:30:00.095544 datajunction-0.0.1a5/dj/construction/utils.py
--rw-r--r--   0        0        0     5900 2023-04-06 15:30:00.095933 datajunction-0.0.1a5/dj/errors.py
--rw-r--r--   0        0        0      518 2023-03-24 07:12:07.926290 datajunction-0.0.1a5/dj/models/__init__.py
--rw-r--r--   0        0        0     2146 2023-03-09 19:29:41.773677 datajunction-0.0.1a5/dj/models/attribute.py
--rw-r--r--   0        0        0     1592 2023-03-09 19:29:41.773734 datajunction-0.0.1a5/dj/models/base.py
--rw-r--r--   0        0        0     2155 2023-03-24 07:12:07.926414 datajunction-0.0.1a5/dj/models/catalog.py
--rw-r--r--   0        0        0     2661 2023-04-06 15:30:00.096245 datajunction-0.0.1a5/dj/models/column.py
--rw-r--r--   0        0        0      858 2023-03-24 07:12:07.926823 datajunction-0.0.1a5/dj/models/cube.py
--rw-r--r--   0        0        0     2019 2023-03-24 07:12:07.927108 datajunction-0.0.1a5/dj/models/database.py
--rw-r--r--   0        0        0      791 2023-04-16 15:31:28.667119 datajunction-0.0.1a5/dj/models/engine.py
--rw-r--r--   0        0        0     1258 2023-04-16 15:31:28.667317 datajunction-0.0.1a5/dj/models/metric.py
--rw-r--r--   0        0        0    20833 2023-04-17 19:39:28.362596 datajunction-0.0.1a5/dj/models/node.py
--rw-r--r--   0        0        0     3711 2023-04-13 18:09:39.316286 datajunction-0.0.1a5/dj/models/query.py
--rw-r--r--   0        0        0     2449 2023-03-24 07:12:07.927968 datajunction-0.0.1a5/dj/models/table.py
--rw-r--r--   0        0        0     2567 2023-03-09 19:29:41.774456 datajunction-0.0.1a5/dj/models/tag.py
--rw-r--r--   0        0        0     4043 2023-04-14 00:40:01.549543 datajunction-0.0.1a5/dj/service_clients.py
--rw-r--r--   0        0        0        0 2023-03-09 19:29:41.774583 datajunction-0.0.1a5/dj/sql/__init__.py
--rw-r--r--   0        0        0     1243 2023-04-13 18:09:39.316464 datajunction-0.0.1a5/dj/sql/dag.py
--rw-r--r--   0        0        0    34351 2023-04-17 19:39:28.362882 datajunction-0.0.1a5/dj/sql/functions.py
--rw-r--r--   0        0        0      644 2023-04-06 15:30:00.097501 datajunction-0.0.1a5/dj/sql/parse.py
--rw-r--r--   0        0        0       55 2023-04-06 15:30:00.097814 datajunction-0.0.1a5/dj/sql/parsing/__init__.py
--rw-r--r--   0        0        0    65402 2023-04-17 19:39:28.363345 datajunction-0.0.1a5/dj/sql/parsing/ast.py
--rw-r--r--   0        0        0        0 2023-03-09 19:29:41.775867 datajunction-0.0.1a5/dj/sql/parsing/backends/__init__.py
--rw-r--r--   0        0        0    30630 2023-04-16 15:31:28.668409 datajunction-0.0.1a5/dj/sql/parsing/backends/antlr4.py
--rw-r--r--   0        0        0      192 2023-03-09 19:29:41.775929 datajunction-0.0.1a5/dj/sql/parsing/backends/exceptions.py
--rw-r--r--   0        0        0     8733 2023-03-26 08:42:46.249360 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4
--rw-r--r--   0        0        0    49854 2023-03-26 08:42:46.249545 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/SqlBaseParser.g4
--rw-r--r--   0        0        0        0 2023-03-26 08:42:46.249595 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/__init__.py
--rw-r--r--   0        0        0   117820 2023-03-26 08:42:46.250054 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp
--rw-r--r--   0        0        0   114725 2023-03-26 08:42:46.250494 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py
--rw-r--r--   0        0        0     8131 2023-03-26 08:42:46.250603 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens
--rw-r--r--   0        0        0   142799 2023-03-26 08:42:46.251524 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp
--rw-r--r--   0        0        0  1020523 2023-03-26 08:42:46.255771 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py
--rw-r--r--   0        0        0     8131 2023-03-26 08:42:46.255887 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens
--rw-r--r--   0        0        0   102489 2023-03-26 08:42:46.256283 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py
--rw-r--r--   0        0        0    60656 2023-03-26 08:42:46.256504 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py
--rw-r--r--   0        0        0    26308 2023-04-17 19:39:28.363635 datajunction-0.0.1a5/dj/sql/parsing/types.py
--rw-r--r--   0        0        0     3812 2023-03-09 19:29:41.776529 datajunction-0.0.1a5/dj/superset.py
--rw-r--r--   0        0        0     6467 2023-04-06 15:30:00.099751 datajunction-0.0.1a5/dj/typing.py
--rw-r--r--   0        0        0     4042 2023-04-14 18:39:42.363510 datajunction-0.0.1a5/dj/utils.py
--rw-r--r--   0        0        0     1418 2023-04-18 03:34:03.317288 datajunction-0.0.1a5/pyproject.toml
--rw-r--r--   0        0        0     7328 1970-01-01 00:00:00.000000 datajunction-0.0.1a5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-26 08:42:43.476435 datajunction-0.0.1a6/LICENSE.txt
+-rw-r--r--   0        0        0     2503 2023-04-22 17:55:26.982921 datajunction-0.0.1a6/README.md
+-rw-r--r--   0        0        0      780 2023-04-25 14:27:09.403307 datajunction-0.0.1a6/datajunction/__init__.py
+-rw-r--r--   0        0        0    20307 2023-04-25 14:27:09.403874 datajunction-0.0.1a6/datajunction/client.py
+-rw-r--r--   0        0        0      108 2023-04-22 17:55:26.983612 datajunction-0.0.1a6/datajunction/exceptions.py
+-rw-r--r--   0        0        0     1075 2023-04-26 16:55:41.582167 datajunction-0.0.1a6/pyproject.toml
+-rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 datajunction-0.0.1a6/PKG-INFO
```

### Comparing `datajunction-0.0.1a5/LICENSE.txt` & `datajunction-0.0.1a6/LICENSE.txt`

 * *Files identical despite different names*

