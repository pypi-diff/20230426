# Comparing `tmp/smartnoise-sql-0.2.9.2.tar.gz` & `tmp/smartnoise-sql-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartnoise-sql-0.2.9.2.tar", max compression
+gzip compressed data, was "smartnoise-sql-1.0.0.tar", max compression
```

## Comparing `smartnoise-sql-0.2.9.2.tar` & `smartnoise-sql-1.0.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     8241 2023-02-18 22:13:33.740254 smartnoise-sql-0.2.9.2/README.md
--rw-r--r--   0        0        0      644 2023-03-01 22:28:41.285337 smartnoise-sql-0.2.9.2/pyproject.toml
--rw-r--r--   0        0        0      182 2023-02-18 22:13:33.767421 smartnoise-sql-0.2.9.2/snsql/__init__.py
--rw-r--r--   0        0        0        0 2023-02-18 22:13:33.767476 smartnoise-sql-0.2.9.2/snsql/_ast/__init__.py
--rw-r--r--   0        0        0    20935 2023-02-18 22:13:33.767874 smartnoise-sql-0.2.9.2/snsql/_ast/ast.py
--rw-r--r--   0        0        0     2878 2023-02-18 22:13:33.767948 smartnoise-sql-0.2.9.2/snsql/_ast/expression.py
--rw-r--r--   0        0        0        0 2023-02-18 22:13:33.768000 smartnoise-sql-0.2.9.2/snsql/_ast/expressions/__init__.py
--rw-r--r--   0        0        0     4486 2023-02-18 22:13:33.768084 smartnoise-sql-0.2.9.2/snsql/_ast/expressions/date.py
--rw-r--r--   0        0        0    12150 2023-02-18 22:13:33.768330 smartnoise-sql-0.2.9.2/snsql/_ast/expressions/logical.py
--rw-r--r--   0        0        0     7007 2023-02-18 22:13:33.768402 smartnoise-sql-0.2.9.2/snsql/_ast/expressions/numeric.py
--rw-r--r--   0        0        0     6405 2023-02-18 22:13:33.768648 smartnoise-sql-0.2.9.2/snsql/_ast/expressions/sql.py
--rw-r--r--   0        0        0     5258 2023-02-18 22:13:33.768711 smartnoise-sql-0.2.9.2/snsql/_ast/expressions/string.py
--rw-r--r--   0        0        0     1613 2023-02-18 22:13:33.768761 smartnoise-sql-0.2.9.2/snsql/_ast/expressions/types.py
--rw-r--r--   0        0        0    13833 2023-02-18 22:13:33.769141 smartnoise-sql-0.2.9.2/snsql/_ast/tokens.py
--rw-r--r--   0        0        0     5484 2023-02-18 22:13:33.769240 smartnoise-sql-0.2.9.2/snsql/_ast/validate.py
--rw-r--r--   0        0        0     2400 2023-02-18 22:13:33.769301 smartnoise-sql-0.2.9.2/snsql/connect.py
--rw-r--r--   0        0        0    20665 2023-02-18 22:13:33.769672 smartnoise-sql-0.2.9.2/snsql/metadata.py
--rw-r--r--   0        0        0       48 2023-02-18 22:13:33.769924 smartnoise-sql-0.2.9.2/snsql/reader/__init__.py
--rw-r--r--   0        0        0     2096 2023-02-18 22:13:33.769990 smartnoise-sql-0.2.9.2/snsql/reader/base.py
--rw-r--r--   0        0        0       41 2023-02-18 22:13:33.770057 smartnoise-sql-0.2.9.2/snsql/sql/__init__.py
--rw-r--r--   0        0        0      251 2023-02-18 22:13:33.770458 smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/__init__.py
--rw-r--r--   0        0        0     3576 2023-02-18 22:13:33.770852 smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/approx_bounds.py
--rw-r--r--   0        0        0     2990 2023-02-18 22:13:33.771151 smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/base.py
--rw-r--r--   0        0        0     3495 2023-02-18 22:13:33.771319 smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/discrete_gaussian.py
--rw-r--r--   0        0        0     3106 2023-02-18 22:13:33.771572 smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/discrete_laplace.py
--rw-r--r--   0        0        0     2921 2023-02-18 22:13:33.771721 smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/laplace.py
--rw-r--r--   0        0        0     3502 2023-02-18 22:13:33.771936 smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/normal.py
--rw-r--r--   0        0        0      328 2023-02-18 22:13:33.771985 smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/rand.py
--rw-r--r--   0        0        0     3739 2023-02-18 22:13:33.772068 smartnoise-sql-0.2.9.2/snsql/sql/dpsu.py
--rw-r--r--   0        0        0     3026 2023-02-18 22:13:33.772125 smartnoise-sql-0.2.9.2/snsql/sql/odometer.py
--rw-r--r--   0        0        0    18985 2023-02-18 22:13:33.772385 smartnoise-sql-0.2.9.2/snsql/sql/parse.py
--rw-r--r--   0        0        0       60 2023-02-18 22:13:33.772479 smartnoise-sql-0.2.9.2/snsql/sql/parser/.gitignore
--rw-r--r--   0        0        0      679 2023-02-18 22:13:33.773049 smartnoise-sql-0.2.9.2/snsql/sql/parser/Makefile
--rw-r--r--   0        0        0      441 2023-02-18 22:13:33.773104 smartnoise-sql-0.2.9.2/snsql/sql/parser/README.md
--rw-r--r--   0        0        0    12171 2023-02-18 22:13:33.773544 smartnoise-sql-0.2.9.2/snsql/sql/parser/SqlSmall.g4
--rw-r--r--   0        0        0     1612 2023-02-18 22:13:33.773610 smartnoise-sql-0.2.9.2/snsql/sql/parser/SqlSmallErrorListener.py
--rw-r--r--   0        0        0    71022 2023-02-18 22:13:33.774105 smartnoise-sql-0.2.9.2/snsql/sql/parser/SqlSmallLexer.py
--rw-r--r--   0        0        0   275434 2023-02-18 22:13:33.774968 smartnoise-sql-0.2.9.2/snsql/sql/parser/SqlSmallParser.py
--rw-r--r--   0        0        0    19760 2023-02-18 22:13:33.775115 smartnoise-sql-0.2.9.2/snsql/sql/parser/SqlSmallVisitor.py
--rw-r--r--   0        0        0        0 2023-02-18 22:13:33.775145 smartnoise-sql-0.2.9.2/snsql/sql/parser/__init__.py
--rw-r--r--   0        0        0     3374 2023-02-18 22:13:33.775515 smartnoise-sql-0.2.9.2/snsql/sql/privacy.py
--rw-r--r--   0        0        0    35239 2023-02-18 22:13:33.775938 smartnoise-sql-0.2.9.2/snsql/sql/private_reader.py
--rw-r--r--   0        0        0    15495 2023-02-18 22:13:33.776183 smartnoise-sql-0.2.9.2/snsql/sql/private_rewriter.py
--rw-r--r--   0        0        0      325 2023-02-18 22:13:33.776273 smartnoise-sql-0.2.9.2/snsql/sql/reader/__init__.py
--rw-r--r--   0        0        0     9029 2023-02-18 22:13:33.776459 smartnoise-sql-0.2.9.2/snsql/sql/reader/base.py
--rw-r--r--   0        0        0     3918 2023-02-18 22:13:33.776828 smartnoise-sql-0.2.9.2/snsql/sql/reader/bigquery.py
--rw-r--r--   0        0        0      465 2023-02-18 22:13:33.777016 smartnoise-sql-0.2.9.2/snsql/sql/reader/engine.py
--rw-r--r--   0        0        0     2417 2023-02-18 22:13:33.777431 smartnoise-sql-0.2.9.2/snsql/sql/reader/mysql.py
--rw-r--r--   0        0        0     6427 2023-02-18 22:13:33.777510 smartnoise-sql-0.2.9.2/snsql/sql/reader/pandas.py
--rw-r--r--   0        0        0     3502 2023-02-18 22:13:33.777743 smartnoise-sql-0.2.9.2/snsql/sql/reader/postgres.py
--rw-r--r--   0        0        0     2966 2023-02-18 22:13:33.777984 smartnoise-sql-0.2.9.2/snsql/sql/reader/presto.py
--rw-r--r--   0        0        0     3227 2023-02-18 22:13:33.778112 smartnoise-sql-0.2.9.2/snsql/sql/reader/probe.py
--rw-r--r--   0        0        0     1902 2023-02-18 22:13:33.778268 smartnoise-sql-0.2.9.2/snsql/sql/reader/spark.py
--rw-r--r--   0        0        0     4389 2023-02-18 22:13:33.778451 smartnoise-sql-0.2.9.2/snsql/sql/reader/sql_server.py
--rw-r--r--   0        0        0     2044 2023-02-18 22:13:33.778680 smartnoise-sql-0.2.9.2/snsql/sql/reader/sqlite.py
--rw-r--r--   0        0        0        0 2023-02-18 22:13:33.778740 smartnoise-sql-0.2.9.2/snsql/xpath/__init__.py
--rw-r--r--   0        0        0     8951 2023-02-18 22:13:33.778827 smartnoise-sql-0.2.9.2/snsql/xpath/ast.py
--rw-r--r--   0        0        0     4783 2023-02-18 22:13:33.778888 smartnoise-sql-0.2.9.2/snsql/xpath/parse.py
--rw-r--r--   0        0        0       57 2023-02-18 22:13:33.778962 smartnoise-sql-0.2.9.2/snsql/xpath/parser/.gitignore
--rw-r--r--   0        0        0      661 2023-02-18 22:13:33.779272 smartnoise-sql-0.2.9.2/snsql/xpath/parser/Makefile
--rw-r--r--   0        0        0     2790 2023-02-18 22:13:33.779339 smartnoise-sql-0.2.9.2/snsql/xpath/parser/XPath.g4
--rw-r--r--   0        0        0     1362 2023-02-18 22:13:33.779393 smartnoise-sql-0.2.9.2/snsql/xpath/parser/XPathErrorListener.py
--rw-r--r--   0        0        0    14203 2023-02-18 22:13:33.779671 smartnoise-sql-0.2.9.2/snsql/xpath/parser/XPathLexer.py
--rw-r--r--   0        0        0    53099 2023-02-18 22:13:33.780085 smartnoise-sql-0.2.9.2/snsql/xpath/parser/XPathParser.py
--rw-r--r--   0        0        0     4070 2023-02-18 22:13:33.780237 smartnoise-sql-0.2.9.2/snsql/xpath/parser/XPathVisitor.py
--rw-r--r--   0        0        0        0 2023-02-18 22:13:33.780267 smartnoise-sql-0.2.9.2/snsql/xpath/parser/__init__.py
--rw-r--r--   0        0        0     9423 2023-03-01 22:28:59.875354 smartnoise-sql-0.2.9.2/setup.py
--rw-r--r--   0        0        0     9140 2023-03-01 22:28:59.875802 smartnoise-sql-0.2.9.2/PKG-INFO
+-rw-r--r--   0        0        0     8241 2023-02-18 22:13:33.740254 smartnoise-sql-1.0.0/README.md
+-rw-r--r--   0        0        0      638 2023-04-26 04:03:19.514431 smartnoise-sql-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      182 2023-02-18 22:13:33.767421 smartnoise-sql-1.0.0/snsql/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-18 22:13:33.767476 smartnoise-sql-1.0.0/snsql/_ast/__init__.py
+-rw-r--r--   0        0        0    21496 2023-04-26 04:00:06.105916 smartnoise-sql-1.0.0/snsql/_ast/ast.py
+-rw-r--r--   0        0        0     2878 2023-02-18 22:13:33.767948 smartnoise-sql-1.0.0/snsql/_ast/expression.py
+-rw-r--r--   0        0        0        0 2023-02-18 22:13:33.768000 smartnoise-sql-1.0.0/snsql/_ast/expressions/__init__.py
+-rw-r--r--   0        0        0     4485 2023-04-13 02:01:02.698944 smartnoise-sql-1.0.0/snsql/_ast/expressions/date.py
+-rw-r--r--   0        0        0    12150 2023-02-18 22:13:33.768330 smartnoise-sql-1.0.0/snsql/_ast/expressions/logical.py
+-rw-r--r--   0        0        0     7007 2023-02-18 22:13:33.768402 smartnoise-sql-1.0.0/snsql/_ast/expressions/numeric.py
+-rw-r--r--   0        0        0     6510 2023-04-17 21:31:42.310775 smartnoise-sql-1.0.0/snsql/_ast/expressions/sql.py
+-rw-r--r--   0        0        0     5258 2023-02-18 22:13:33.768711 smartnoise-sql-1.0.0/snsql/_ast/expressions/string.py
+-rw-r--r--   0        0        0     1613 2023-02-18 22:13:33.768761 smartnoise-sql-1.0.0/snsql/_ast/expressions/types.py
+-rw-r--r--   0        0        0    13833 2023-02-18 22:13:33.769141 smartnoise-sql-1.0.0/snsql/_ast/tokens.py
+-rw-r--r--   0        0        0     5484 2023-02-18 22:13:33.769240 smartnoise-sql-1.0.0/snsql/_ast/validate.py
+-rw-r--r--   0        0        0     2400 2023-02-18 22:13:33.769301 smartnoise-sql-1.0.0/snsql/connect.py
+-rw-r--r--   0        0        0    20665 2023-04-23 02:41:53.046121 smartnoise-sql-1.0.0/snsql/metadata.py
+-rw-r--r--   0        0        0       48 2023-02-18 22:13:33.769924 smartnoise-sql-1.0.0/snsql/reader/__init__.py
+-rw-r--r--   0        0        0     2096 2023-02-18 22:13:33.769990 smartnoise-sql-1.0.0/snsql/reader/base.py
+-rw-r--r--   0        0        0       41 2023-02-18 22:13:33.770057 smartnoise-sql-1.0.0/snsql/sql/__init__.py
+-rw-r--r--   0        0        0      251 2023-02-18 22:13:33.770458 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/__init__.py
+-rw-r--r--   0        0        0     3487 2023-04-12 02:24:35.798160 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/approx_bounds.py
+-rw-r--r--   0        0        0     2990 2023-02-18 22:13:33.771151 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/base.py
+-rw-r--r--   0        0        0     3495 2023-02-18 22:13:33.771319 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/discrete_gaussian.py
+-rw-r--r--   0        0        0     3106 2023-02-18 22:13:33.771572 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/discrete_laplace.py
+-rw-r--r--   0        0        0     2921 2023-02-18 22:13:33.771721 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/laplace.py
+-rw-r--r--   0        0        0     3502 2023-02-18 22:13:33.771936 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/normal.py
+-rw-r--r--   0        0        0      328 2023-02-18 22:13:33.771985 smartnoise-sql-1.0.0/snsql/sql/_mechanisms/rand.py
+-rw-r--r--   0        0        0     3739 2023-02-18 22:13:33.772068 smartnoise-sql-1.0.0/snsql/sql/dpsu.py
+-rw-r--r--   0        0        0     3026 2023-02-18 22:13:33.772125 smartnoise-sql-1.0.0/snsql/sql/odometer.py
+-rw-r--r--   0        0        0    18985 2023-02-18 22:13:33.772385 smartnoise-sql-1.0.0/snsql/sql/parse.py
+-rw-r--r--   0        0        0       60 2023-02-18 22:13:33.772479 smartnoise-sql-1.0.0/snsql/sql/parser/.gitignore
+-rw-r--r--   0        0        0      679 2023-02-18 22:13:33.773049 smartnoise-sql-1.0.0/snsql/sql/parser/Makefile
+-rw-r--r--   0        0        0      441 2023-02-18 22:13:33.773104 smartnoise-sql-1.0.0/snsql/sql/parser/README.md
+-rw-r--r--   0        0        0    12171 2023-02-18 22:13:33.773544 smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmall.g4
+-rw-r--r--   0        0        0     1612 2023-02-18 22:13:33.773610 smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallErrorListener.py
+-rw-r--r--   0        0        0    71022 2023-02-18 22:13:33.774105 smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallLexer.py
+-rw-r--r--   0        0        0   275434 2023-02-18 22:13:33.774968 smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallParser.py
+-rw-r--r--   0        0        0    19760 2023-02-18 22:13:33.775115 smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallVisitor.py
+-rw-r--r--   0        0        0        0 2023-02-18 22:13:33.775145 smartnoise-sql-1.0.0/snsql/sql/parser/__init__.py
+-rw-r--r--   0        0        0     3374 2023-02-18 22:13:33.775515 smartnoise-sql-1.0.0/snsql/sql/privacy.py
+-rw-r--r--   0        0        0    35627 2023-04-26 04:00:06.106219 smartnoise-sql-1.0.0/snsql/sql/private_reader.py
+-rw-r--r--   0        0        0    15548 2023-04-17 21:31:42.310975 smartnoise-sql-1.0.0/snsql/sql/private_rewriter.py
+-rw-r--r--   0        0        0      325 2023-02-18 22:13:33.776273 smartnoise-sql-1.0.0/snsql/sql/reader/__init__.py
+-rw-r--r--   0        0        0     9029 2023-02-18 22:13:33.776459 smartnoise-sql-1.0.0/snsql/sql/reader/base.py
+-rw-r--r--   0        0        0     3918 2023-02-18 22:13:33.776828 smartnoise-sql-1.0.0/snsql/sql/reader/bigquery.py
+-rw-r--r--   0        0        0      465 2023-02-18 22:13:33.777016 smartnoise-sql-1.0.0/snsql/sql/reader/engine.py
+-rw-r--r--   0        0        0     2417 2023-02-18 22:13:33.777431 smartnoise-sql-1.0.0/snsql/sql/reader/mysql.py
+-rw-r--r--   0        0        0     7024 2023-04-26 04:00:06.106399 smartnoise-sql-1.0.0/snsql/sql/reader/pandas.py
+-rw-r--r--   0        0        0     3502 2023-02-18 22:13:33.777743 smartnoise-sql-1.0.0/snsql/sql/reader/postgres.py
+-rw-r--r--   0        0        0     2966 2023-02-18 22:13:33.777984 smartnoise-sql-1.0.0/snsql/sql/reader/presto.py
+-rw-r--r--   0        0        0     3698 2023-04-26 04:00:06.106547 smartnoise-sql-1.0.0/snsql/sql/reader/probe.py
+-rw-r--r--   0        0        0     1902 2023-02-18 22:13:33.778268 smartnoise-sql-1.0.0/snsql/sql/reader/spark.py
+-rw-r--r--   0        0        0     4389 2023-02-18 22:13:33.778451 smartnoise-sql-1.0.0/snsql/sql/reader/sql_server.py
+-rw-r--r--   0        0        0     2044 2023-02-18 22:13:33.778680 smartnoise-sql-1.0.0/snsql/sql/reader/sqlite.py
+-rw-r--r--   0        0        0        0 2023-02-18 22:13:33.778740 smartnoise-sql-1.0.0/snsql/xpath/__init__.py
+-rw-r--r--   0        0        0     8951 2023-02-18 22:13:33.778827 smartnoise-sql-1.0.0/snsql/xpath/ast.py
+-rw-r--r--   0        0        0     4783 2023-02-18 22:13:33.778888 smartnoise-sql-1.0.0/snsql/xpath/parse.py
+-rw-r--r--   0        0        0       57 2023-02-18 22:13:33.778962 smartnoise-sql-1.0.0/snsql/xpath/parser/.gitignore
+-rw-r--r--   0        0        0      661 2023-02-18 22:13:33.779272 smartnoise-sql-1.0.0/snsql/xpath/parser/Makefile
+-rw-r--r--   0        0        0     2790 2023-02-18 22:13:33.779339 smartnoise-sql-1.0.0/snsql/xpath/parser/XPath.g4
+-rw-r--r--   0        0        0     1362 2023-02-18 22:13:33.779393 smartnoise-sql-1.0.0/snsql/xpath/parser/XPathErrorListener.py
+-rw-r--r--   0        0        0    14203 2023-02-18 22:13:33.779671 smartnoise-sql-1.0.0/snsql/xpath/parser/XPathLexer.py
+-rw-r--r--   0        0        0    53099 2023-02-18 22:13:33.780085 smartnoise-sql-1.0.0/snsql/xpath/parser/XPathParser.py
+-rw-r--r--   0        0        0     4070 2023-02-18 22:13:33.780237 smartnoise-sql-1.0.0/snsql/xpath/parser/XPathVisitor.py
+-rw-r--r--   0        0        0        0 2023-02-18 22:13:33.780267 smartnoise-sql-1.0.0/snsql/xpath/parser/__init__.py
+-rw-r--r--   0        0        0     9417 2023-04-26 04:03:28.741811 smartnoise-sql-1.0.0/setup.py
+-rw-r--r--   0        0        0     9134 2023-04-26 04:03:28.742243 smartnoise-sql-1.0.0/PKG-INFO
```

### Comparing `smartnoise-sql-0.2.9.2/README.md` & `smartnoise-sql-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/pyproject.toml` & `smartnoise-sql-1.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "smartnoise-sql"
-version = "0.2.9.2"
+version = "1.0.0"
 description = "Differentially Private SQL Queries"
 authors = ["SmartNoise Team <smartnoise@opendp.org>"]
 license = "MIT"
 packages = [{include="snsql"}]
 homepage = "https://smartnoise.org"
 repository = "https://github.com/opendp/smartnoise-sdk"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<=3.11"
+python = ">=3.7,<3.12"
 opendp = "^0.6.0"
 antlr4-python3-runtime = "4.9.3"
-pandasql = "^0.7.3"
 PyYAML = "^5.4.1"
 graphviz = "^0.17"
-sqlalchemy = "^1.4.23"
+sqlalchemy = "^2.0.0"
+pandas = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `smartnoise-sql-0.2.9.2/snsql/_ast/ast.py` & `smartnoise-sql-1.0.0/snsql/_ast/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,17 @@
             # grab the first column in the table, to extract table metadata
             tables.append(t._select_symbols[0].expression)
         if len(tables) > 0:
             self.max_ids = max(tc.max_ids for tc in tables)
             self.sample_max_ids = any(tc.sample_max_ids for tc in tables)
             self.row_privacy = any(tc.row_privacy for tc in tables)
             self.censor_dims = any(tc.censor_dims for tc in tables)
+            self.clamp_counts = any(tc.clamp_counts for tc in tables)
+            self.clamp_columns = any(tc.clamp_columns for tc in tables)
+            self.use_dpsu = any(tc.use_dpsu for tc in tables)
 
         # get grouping expression symbols
         self._grouping_symbols = []
         if self.agg:
             self._grouping_symbols = []
             for ge in self.agg.groupingExpressions:
                 try:
@@ -436,14 +439,17 @@
                     nullable=tc[name].nullable if hasattr(tc[name], "nullable") else True,
                     missing_value=tc[name].missing_value if hasattr(tc[name], "missing_value") else None,
                     sensitivity=tc[name].sensitivity if hasattr(tc[name], "sensitivity") else None,
                     max_ids=table.max_ids,
                     sample_max_ids=table.sample_max_ids,
                     row_privacy=table.row_privacy,
                     censor_dims=table.censor_dims,
+                    clamp_columns=table.clamp_columns,
+                    clamp_counts=table.clamp_counts,
+                    use_dpsu=table.use_dpsu,
                     compare=metadata.compare
                 )
             self._select_symbols = [Symbol(get_table_expr(name), name) for name in tc.keys()]
 
     def escaped(self):
         # is any part of this identifier escaped?
         parts = str(self).split(".")
@@ -536,15 +542,18 @@
         max_ids=1,
         sample_max_ids=True,
         row_privacy=False,
         censor_dims=False,
         compare=None,
         nullable = True,
         missing_value = None,
-        sensitivity = None
+        sensitivity = None,
+        clamp_counts = False,
+        clamp_columns = True,
+        use_dpsu = False,
     ):
         self.tablename = tablename
         self.colname = colname
         self.valtype = valtype
         self.is_key = is_key
         self.lower = lower
         self.upper = upper
@@ -552,14 +561,17 @@
         self.sample_max_ids = sample_max_ids
         self.row_privacy = row_privacy
         self.censor_dims = censor_dims
         self.unbounded = lower is None or upper is None
         self.nullable = nullable
         self.missing_value = missing_value
         self._sensitivity = sensitivity
+        self.clamp_counts = clamp_counts
+        self.clamp_columns = clamp_columns
+        self.use_dpsu = use_dpsu
         self.compare = compare
 
     def __str__(self):
         return self.tablename + "." + self.colname
 
     def __eq__(self, other):
         return isinstance(self, type(other)) and self.tablename == other.tablename and self.colname == other.colname
```

### Comparing `smartnoise-sql-0.2.9.2/snsql/_ast/expression.py` & `smartnoise-sql-1.0.0/snsql/_ast/expression.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/_ast/expressions/date.py` & `smartnoise-sql-1.0.0/snsql/_ast/expressions/date.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,9 +122,8 @@
         elif self.date_part == 'microsecond':
             if isinstance(parsed, datetime.date) and not isinstance(parsed, datetime.datetime):
                 return 0
             return parsed.microsecond
         else:
             raise ValueError(f"Unknown date part requested: {self.date_part}")
     def symbol(self, relations):
-        return ExtractFunction(self.expression.symbol(relations), self.date_part)
-
+        return ExtractFunction(self.date_part, self.expression.symbol(relations))
```

### Comparing `smartnoise-sql-0.2.9.2/snsql/_ast/expressions/logical.py` & `smartnoise-sql-1.0.0/snsql/_ast/expressions/logical.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/_ast/expressions/numeric.py` & `smartnoise-sql-1.0.0/snsql/_ast/expressions/numeric.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/_ast/expressions/sql.py` & `smartnoise-sql-1.0.0/snsql/_ast/expressions/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,17 @@
         self.table = table
 
     def __str__(self):
         return (self.table + "." if self.table is not None else "") + "*"
 
     def __hash__(self):
         return hash(str(self))
+    
+    def __eq__(self, other):
+        return type(self) == type(other) and self.table == other.table
 
     def symbol_name(self):
         return 'star'
 
     def all_symbols(self, relations):
         sym = [r.all_symbols(self) for r in relations if r.alias_match(str(self))]
         if len(sym) == 0:
```

### Comparing `smartnoise-sql-0.2.9.2/snsql/_ast/expressions/string.py` & `smartnoise-sql-1.0.0/snsql/_ast/expressions/string.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/_ast/expressions/types.py` & `smartnoise-sql-1.0.0/snsql/_ast/expressions/types.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/_ast/tokens.py` & `smartnoise-sql-1.0.0/snsql/_ast/tokens.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/_ast/validate.py` & `smartnoise-sql-1.0.0/snsql/_ast/validate.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/connect.py` & `smartnoise-sql-1.0.0/snsql/connect.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/metadata.py` & `smartnoise-sql-1.0.0/snsql/metadata.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/reader/base.py` & `smartnoise-sql-1.0.0/snsql/reader/base.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/approx_bounds.py` & `smartnoise-sql-1.0.0/snsql/sql/_mechanisms/approx_bounds.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,31 +57,27 @@
             return (0.0, 1.0)
         elif idx > bins:
             return (2.0 ** (idx - bins - 1), 2.0 ** (idx - bins))
         elif idx == bins - 1:
             return (-1.0, -0.0)
         else:
             return (-1 * 2.0 ** np.abs(bins - idx - 1), -1 * 2.0 ** np.abs(bins - idx - 2))
+        
+    edge_list = [edges(idx) for idx in range(len(hist))]
 
     # compute histograms
     for v in vals:
-        if v >= 0 and v < 1.0:
-            bin = bins
-            hist[bin] += 1
-        elif v >= 1.0:
-            bin = int(np.trunc(np.log2(v))) + bins + 1
-            if bin < len(hist):
-                hist[bin] += 1
-        elif v < 0 and v >= -1.0:
-            bin = bins - 1
-            hist[bin] += 1
-        else:
-            bin = bins - int(np.trunc(np.log2(-v + 1))) - 1
-            if bin > 0:
-                hist[bin] += 1
+        bin = None
+        for idx, (l, u) in enumerate(edge_list):
+            if l <= v < u:
+                bin = idx
+                break
+        if bin is None:
+            raise ValueError(f"Value {v} is outside of the range we can use to infer bounds")
+        hist[bin] += 1
 
         # for testing
         l, u = edges(bin)
         assert(l <= v < u)
 
     enable_features('floating-point', 'contrib')
     discovered_scale = 1.0 / epsilon
```

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/base.py` & `smartnoise-sql-1.0.0/snsql/sql/_mechanisms/base.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/discrete_gaussian.py` & `smartnoise-sql-1.0.0/snsql/sql/_mechanisms/discrete_gaussian.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/discrete_laplace.py` & `smartnoise-sql-1.0.0/snsql/sql/_mechanisms/discrete_laplace.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/laplace.py` & `smartnoise-sql-1.0.0/snsql/sql/_mechanisms/laplace.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/_mechanisms/normal.py` & `smartnoise-sql-1.0.0/snsql/sql/_mechanisms/normal.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/dpsu.py` & `smartnoise-sql-1.0.0/snsql/sql/dpsu.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/odometer.py` & `smartnoise-sql-1.0.0/snsql/sql/odometer.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/parse.py` & `smartnoise-sql-1.0.0/snsql/sql/parse.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/parser/Makefile` & `smartnoise-sql-1.0.0/snsql/sql/parser/Makefile`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/parser/SqlSmall.g4` & `smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmall.g4`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/parser/SqlSmallErrorListener.py` & `smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallErrorListener.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/parser/SqlSmallLexer.py` & `smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallLexer.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/parser/SqlSmallParser.py` & `smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallParser.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/parser/SqlSmallVisitor.py` & `smartnoise-sql-1.0.0/snsql/sql/parser/SqlSmallVisitor.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/privacy.py` & `smartnoise-sql-1.0.0/snsql/sql/privacy.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/private_reader.py` & `smartnoise-sql-1.0.0/snsql/sql/private_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         if isinstance(reader, Reader):
             self.reader = reader
         else:
             raise ValueError("Parameter reader must be of type Reader")
         self.metadata = Metadata.from_(metadata)
         self.rewriter = Rewriter(metadata)
         self._options = PrivateReaderOptions()
+        self._initial_options()
 
         if privacy:
             self.privacy = privacy
         else:
             raise ValueError("Must pass in a Privacy object with privacy parameters.")
         
         self.odometer = OdometerHeterogeneous(self.privacy)
@@ -91,44 +92,36 @@
 
             df = pd.read_csv('datasets/PUMS.csv')
             reader = from_connection(df, metadata=metadata, privacy=privacy)
             assert(reader.engine == 'pandas')
         """
         return self.reader.engine
 
-    def _refresh_options(self):
-        self.rewriter = Rewriter(self.metadata, privacy=self.privacy)
-        self.metadata.compare = self.reader.compare
+    def _initial_options(self):
         tables = self.metadata.tables()
         self._options.row_privacy = any([t.row_privacy for t in tables])
         self._options.censor_dims = not any([not t.censor_dims for t in tables])
         self._options.reservoir_sample = any([t.sample_max_ids for t in tables])
         self._options.clamp_counts = any([t.clamp_counts for t in tables])
-        self._options.max_contrib = max([t.max_ids for t in tables])
         self._options.use_dpsu = any([t.use_dpsu for t in tables])
         self._options.clamp_columns = any([t.clamp_columns for t in tables])
+    def _refresh_options(self):
+        self.rewriter = Rewriter(self.metadata, privacy=self.privacy)
+        self.metadata.compare = self.reader.compare
 
         self.rewriter.options.row_privacy = self._options.row_privacy
         self.rewriter.options.reservoir_sample = self._options.reservoir_sample
         self.rewriter.options.clamp_columns = self._options.clamp_columns
         self.rewriter.options.max_contrib = self._options.max_contrib
         self.rewriter.options.censor_dims = self._options.censor_dims
 
     def _warn_mechanisms(self):
         """
         Warn if any of the current settings could result in unsafe floating point mechanisms.
         """
-        if self._options.censor_dims:
-            warnings.warn(
-f"""Dimension censoring is enabled, with {self.privacy.mechanisms.map[Stat.threshold]} as the thresholding mechanism. 
-This is an unsafe floating point mechanism.  Counts used for censoring will be revealed in any queries that request COUNT DISTINCT(person), 
-leading to potential privacy leaks. If your query workload needs to reveal distinct counts of individuals, consider doing the dimension
-censoring as a preprocessing step.  See the documentation for more information."""
-            )
-
         mechs = self.privacy.mechanisms
         tables = self.metadata.tables()
         floats = []
         large_ints = []
         large = mechs.large
         for table in tables:
             for col in table.columns():
@@ -284,16 +277,15 @@
         query = self.parse_query_string(query_string)
         return self._rewrite_ast(query)
 
     def _rewrite_ast(self, query):
         if isinstance(query, str):
             raise ValueError("Please pass a Query AST object to _rewrite_ast()")
         query_max_contrib = query.max_ids
-        if self._options.max_contrib is None or self._options.max_contrib > query_max_contrib:
-            self._options.max_contrib = query_max_contrib
+        self._options.max_contrib = query_max_contrib
 
         self._refresh_options()
         query = self.rewriter.query(query)
         query.compare = self.reader.compare
         subquery = query.source.relations[0].primary.query
         subquery.compare = self.reader.compare
         return (subquery, query)
@@ -500,14 +492,30 @@
         )
 
     def _execute_ast(self, query, *ignore, accuracy:bool=False, pre_aggregated=None, postprocess=True):
         if isinstance(query, str):
             raise ValueError("Please pass AST to _execute_ast.")
 
         _orig_query = query
+
+        agg_names = []
+        for col in _orig_query.select.namedExpressions:
+            if isinstance(col.expression, ast.AggFunction):
+                agg_names.append(col.expression.name)
+            else:
+                agg_names.append(None)
+
+        self._options.row_privacy = query.row_privacy
+        self._options.censor_dims = query.censor_dims
+        self._options.reservoir_sample = query.sample_max_ids
+        self._options.clamp_counts = query.clamp_counts
+        self._options.use_dpsu = query.use_dpsu
+        self._options.clamp_columns = query.clamp_columns
+        self._refresh_options()
+
         subquery, query = self._rewrite_ast(query)
 
         if pre_aggregated is not None:
             exact_aggregates = self._check_pre_aggregated_columns(pre_aggregated, subquery)
         else:
             exact_aggregates = self._get_reader(subquery)._execute_ast(subquery)
 
@@ -620,14 +628,24 @@
                 raise ValueError("Can't convert type " + type)
         
         alphas = [alpha for alpha in self.privacy.alphas]
 
         def process_out_row(row):
             bindings = dict((name.lower(), val) for name, val in zip(source_col_names, row))
             out_row = [c.expression.evaluate(bindings) for c in query.select.namedExpressions]
+            # fix up case where variance is negative
+            out_row_fixed = []
+            for val, agg in zip(out_row, agg_names):
+                if agg == 'VAR' and val < 0:
+                    out_row_fixed.append(0.0)
+                elif agg == 'STDDEV' and np.isnan(val):
+                    out_row_fixed.append(0.0)
+                else:
+                    out_row_fixed.append(val)
+            out_row = out_row_fixed
             try:
                 out_row =[convert(val, type) for val, type in zip(out_row, out_types)]
             except Exception as e:
                 raise ValueError(
                     f"Error converting output row: {e}\n"
                     f"Expecting types {out_types}"
                 )
```

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/private_rewriter.py` & `smartnoise-sql-1.0.0/snsql/sql/private_rewriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,15 +361,18 @@
                 else:
                     pass
             else:
                 self.expressions[proposed] = expression
                 return proposed
 
         # see if the expression has been used
-        names = [name for name in self.expressions.keys() if self.expressions[name] == expression]
+        names = []
+        for name in self.expressions.keys():
+            if self.expressions[name] == expression:
+                names.append(name)
         if len(names) > 0:
             return names[0]
 
         # see if the expression has been used under the symbol name
         proposed = expression.symbol_name()
         if proposed in self.expressions:
             if self.expressions[proposed] == expression:
```

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/reader/base.py` & `smartnoise-sql-1.0.0/snsql/sql/reader/base.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/reader/bigquery.py` & `smartnoise-sql-1.0.0/snsql/sql/reader/bigquery.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/reader/mysql.py` & `smartnoise-sql-1.0.0/snsql/sql/reader/mysql.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/reader/pandas.py` & `smartnoise-sql-1.0.0/snsql/sql/reader/pandas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,56 @@
 import importlib
-
-#from snsql.metadata import Metadata
+import pandas as pd
+from sqlalchemy import create_engine, text
 from .base import SqlReader, NameCompare, Serializer
 from .engine import Engine
 import copy
 import warnings
 import re
 
 
 class PandasReader(SqlReader):
     ENGINE = Engine.PANDAS
 
-    def __init__(self, df=None, metadata=None, conn=None, **kwargs):
+    def __init__(self, df=None, metadata=None, conn=None, *ignore, table_name=None, **kwargs):
         super().__init__(self.ENGINE)
+        if metadata is not None:
+            self.metadata = metadata
+            class_ = getattr(importlib.import_module("snsql.metadata"), "Metadata")
+            self.metadata = class_.from_(metadata)
         if conn is not None:
             df = conn
-        if metadata is None:
-            raise ValueError("Load without metadata is not yet implemented")
         if df is None:
             raise ValueError("Pass in a Pandas dataframe")
-        self.df = df
-
-        # we can replace this when we remove
-        # Metadata from pandas cleaning
-        class_ = getattr(importlib.import_module("snsql.metadata"), "Metadata")
-        metadata = class_.from_(metadata)
+        table_dict = {}
+        if isinstance(df, pd.DataFrame):        
+            if table_name is None:
+                if metadata is None:
+                    raise ValueError("Must pass in table_name if metadata is not provided")
+                table_names = list(self.metadata.m_tables.keys())
+                if len(table_names) > 1:
+                    raise ValueError(
+                        "Must pass in table_name if metadata has more than one table"
+                    )
+                table_name = table_names[0]
+            else:
+                if metadata is not None:
+                    table_names = list(metadata.m_tables.keys())
+                    if table_name not in table_names:
+                        raise ValueError(
+                            "table_name {} not in metadata".format(table_name)
+                        )
+            table_dict[table_name] = df
+        elif not isinstance(df, dict):
+            raise ValueError("df must be a Pandas dataframe or a dictionary of dataframes")
+        else:
+            table_dict = df
 
-        self.metadata, self.original_column_names = self._sanitize_metadata(metadata)
+        # check minimum version of sqlite
         import sqlite3
-
         ver = [int(part) for part in sqlite3.sqlite_version.split(".")]
         if len(ver) == 3:
             # all historical versions of SQLite have 3 parts
             if (
                 ver[0] < 3
                 or (ver[0] == 3 and ver[1] < 2)
                 or (ver[0] == 3 and ver[1] == 2 and ver[2] < 6)
@@ -40,14 +58,26 @@
                 warnings.warn(
                     "This python environment has outdated sqlite version {0}.  PandasReader will fail on queries that use private_key.  Please upgrade to a newer Python environment (with sqlite >= 3.2.6), or ensure that you only use row_privacy.".format(
                         sqlite3.sqlite_version
                     ),
                     Warning,
                 )
 
+        # load all dataframes into a single sqlite database
+        table_names = list(table_dict.keys())
+        self.table_names = table_names
+
+        table_name_fixed = [t.replace(".", "_") for t in table_names]
+        if len(table_names) != len(set(table_name_fixed)):
+            raise ValueError("Table names must be unique after replacing '.' with '_'.")
+        db_engine = create_engine('sqlite://', echo=False)
+        for table_name, df in table_dict.items():
+            df.to_sql(table_name.replace('.','_'), con=db_engine, index=False)
+        self.db_engine = db_engine
+
     def _sanitize_column_name(self, column_name):
         x = re.search(r".*[a-zA-Z0-9()_]", column_name)
         if x is None:
             raise Exception(
                 "Unsupported column name {}. Column names must be alphanumeric or _, (, ).".format(
                     column_name
                 )
@@ -109,51 +139,30 @@
 
     def execute(self, query, *ignore, accuracy:bool=False):
         """
             Executes a raw SQL string against the database and returns
             tuples for rows.  This will NOT fix the query to target the
             specific SQL dialect.  Call execute_typed to fix dialect.
         """
-        query = self._sanitize_query(query)
-        from pandasql import sqldf
-
         if not isinstance(query, str):
             raise ValueError("Please pass strings to execute.  To execute ASTs, use execute_typed.")
-        table_names = list(self.metadata.m_tables.keys())
-        if len(table_names) > 1:
-            raise Exception(
-                "PandasReader only supports one table, {} found.".format(len(table_names))
-            )
-
-        df_name = "df_for_diffpriv1234"
-        table_name = table_names[0]
-
-        def clean_query(query):
-            for column in self.metadata.m_tables[table_name].m_columns:
-                if " " in column or "(" in column or ")" in column:
-                    new_column_name = column.replace(" ", "_").replace("(", "_").replace(")", "_")
-                    query = query.replace(column, new_column_name)
-                    query = query.replace("'{}'".format(new_column_name), new_column_name)
-            return query.replace(table_name, df_name)
-
-        for column in self.metadata.m_tables[table_name].m_columns:
-            new_column_name = column.replace(" ", "_").replace("(", "_").replace(")", "_")
-            if self.metadata.m_tables[table_name].m_columns[column].is_key:
-                if column not in self.df:
-                    self.df[column] = range(len(self.df))
-            else:
-                if new_column_name not in self.df:
-                    self.df[new_column_name] = self.df[column]
-
-        df_for_diffpriv1234 = self.df
-        q_result = sqldf(clean_query(query), locals())
-        return [tuple([col for col in q_result.columns])] + [
-            val[1:] for val in q_result.itertuples()
-        ]
+        
+        # this is a hack; should use AST
+        for table_name in self.table_names:
+            query = query.replace(table_name, table_name.replace('.', '_'))
+        with self.db_engine.connect() as conn:
+            result_proxy = conn.execute(text(query))
+            column_names = [tuple(c for c in result_proxy.keys())]
+            result = [tuple(row) for row in result_proxy.fetchall()]
+            return column_names + result
 
 class PandasNameCompare(NameCompare):
     def __init__(self, search_path=None):
         super().__init__(search_path)
 
 class PandasSerializer(Serializer):
     def __init__(self):
         super().__init__()
+    def serialize(self, query):
+        if isinstance(query, str):
+            raise ValueError("We need an AST to validate and serialize.")
+        return str(query)
```

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/reader/postgres.py` & `smartnoise-sql-1.0.0/snsql/sql/reader/postgres.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/reader/presto.py` & `smartnoise-sql-1.0.0/snsql/sql/reader/presto.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/reader/probe.py` & `smartnoise-sql-1.0.0/snsql/sql/reader/probe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 class Probe:
     @classmethod
     def engine(cls, conn) -> str:
         """
         Probes a connection and tries to determine which engine it uses
         """
+        if isinstance(conn, dict):
+            mods = []
+            classes = []
+            for k, v in conn.items():
+                mods.append(v.__class__.__module__)
+                classes.append(v.__class__.__name__)
+            mods = list(set(mods))
+            classes = list(set(classes))
+            if len(mods) == 1 and len(classes) == 1:
+                if mods[0] == 'pandas.core.frame' and classes[0] == 'DataFrame':
+                    return "pandas"
         conn_mod = conn.__class__.__module__
         conn_class = conn.__class__.__name__
         if (
             conn_mod == 'pandas.core.frame' and
             conn_class == 'DataFrame'
         ):
             return "pandas"
```

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/reader/spark.py` & `smartnoise-sql-1.0.0/snsql/sql/reader/spark.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/reader/sql_server.py` & `smartnoise-sql-1.0.0/snsql/sql/reader/sql_server.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/sql/reader/sqlite.py` & `smartnoise-sql-1.0.0/snsql/sql/reader/sqlite.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/xpath/ast.py` & `smartnoise-sql-1.0.0/snsql/xpath/ast.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/xpath/parse.py` & `smartnoise-sql-1.0.0/snsql/xpath/parse.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/xpath/parser/Makefile` & `smartnoise-sql-1.0.0/snsql/xpath/parser/Makefile`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/xpath/parser/XPath.g4` & `smartnoise-sql-1.0.0/snsql/xpath/parser/XPath.g4`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/xpath/parser/XPathErrorListener.py` & `smartnoise-sql-1.0.0/snsql/xpath/parser/XPathErrorListener.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/xpath/parser/XPathLexer.py` & `smartnoise-sql-1.0.0/snsql/xpath/parser/XPathLexer.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/xpath/parser/XPathParser.py` & `smartnoise-sql-1.0.0/snsql/xpath/parser/XPathParser.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/snsql/xpath/parser/XPathVisitor.py` & `smartnoise-sql-1.0.0/snsql/xpath/parser/XPathVisitor.py`

 * *Files identical despite different names*

### Comparing `smartnoise-sql-0.2.9.2/setup.py` & `smartnoise-sql-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=5.4.1,<6.0.0',
  'antlr4-python3-runtime==4.9.3',
  'graphviz>=0.17,<0.18',
  'opendp>=0.6.0,<0.7.0',
- 'pandasql>=0.7.3,<0.8.0',
- 'sqlalchemy>=1.4.23,<2.0.0']
+ 'pandas>=2.0.1,<3.0.0',
+ 'sqlalchemy>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'smartnoise-sql',
-    'version': '0.2.9.2',
+    'version': '1.0.0',
     'description': 'Differentially Private SQL Queries',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8-blue)](https://www.python.org/)\n\n<a href="https://smartnoise.org"><img src="https://github.com/opendp/smartnoise-sdk/raw/main/images/SmartNoise/SVG/Logo%20Mark_grey.svg" align="left" height="65" vspace="8" hspace="18"></a>\n\n## SmartNoise SQL\n\nDifferentially private SQL queries.  Tested with:\n* PostgreSQL\n* SQL Server\n* Spark\n* Pandas (SQLite)\n* PrestoDB\n* BigQuery\n\nSmartNoise is intended for scenarios where the analyst is trusted by the data owner.  SmartNoise uses the [OpenDP](https://github.com/opendp/opendp) library of differential privacy algorithms.\n\n## Installation\n\n```\npip install smartnoise-sql\n```\n\n## Querying a Pandas DataFrame\n\nUse the `from_df` method to create a private reader that can issue queries against a pandas dataframe.\n\n```python\nimport snsql\nfrom snsql import Privacy\nimport pandas as pd\nprivacy = Privacy(epsilon=1.0, delta=0.01)\n\ncsv_path = \'PUMS.csv\'\nmeta_path = \'PUMS.yaml\'\n\npums = pd.read_csv(csv_path)\nreader = snsql.from_df(pums, privacy=privacy, metadata=meta_path)\n\nresult = reader.execute(\'SELECT sex, AVG(age) AS age FROM PUMS.PUMS GROUP BY sex\')\n```\n\n## Querying a SQL Database\n\nUse `from_connection` to wrap an existing database connection.\n\n```python\nimport snsql\nfrom snsql import Privacy\nimport psycopg2\n\nprivacy = Privacy(epsilon=1.0, delta=0.01)\nmeta_path = \'PUMS.yaml\'\n\npumsdb = psycopg2.connect(user=\'postgres\', host=\'localhost\', database=\'PUMS\')\nreader = snsql.from_connection(pumsdb, privacy=privacy, metadata=meta_path)\n\nresult = reader.execute(\'SELECT sex, AVG(age) AS age FROM PUMS.PUMS GROUP BY sex\')\n```\n\n## Querying a Spark DataFrame\n\nUse `from_connection` to wrap a spark session.\n\n```python\nimport pyspark\nfrom pyspark.sql import SparkSession\nspark = SparkSession.builder.getOrCreate()\nfrom snsql import *\n\npums = spark.read.load(...)  # load a Spark DataFrame\npums.createOrReplaceTempView("PUMS_large")\n\nmetadata = \'PUMS_large.yaml\'\n\nprivate_reader = from_connection(\n    spark, \n    metadata=metadata, \n    privacy=Privacy(epsilon=3.0, delta=1/1_000_000)\n)\nprivate_reader.reader.compare.search_path = ["PUMS"]\n\n\nres = private_reader.execute(\'SELECT COUNT(*) FROM PUMS_large\')\nres.show()\n```\n\n## Privacy Cost\n\nThe privacy parameters epsilon and delta are passed in to the private connection at instantiation time, and apply to each computed column during the life of the session.  Privacy cost accrues indefinitely as new queries are executed, with the total accumulated privacy cost being available via the `spent` property of the connection\'s `odometer`:\n\n```python\nprivacy = Privacy(epsilon=0.1, delta=10e-7)\n\nreader = from_connection(conn, metadata=metadata, privacy=privacy)\nprint(reader.odometer.spent)  # (0.0, 0.0)\n\nresult = reader.execute(\'SELECT COUNT(*) FROM PUMS.PUMS\')\nprint(reader.odometer.spent)  # approximately (0.1, 10e-7)\n```\n\nThe privacy cost increases with the number of columns:\n\n```python\nreader = from_connection(conn, metadata=metadata, privacy=privacy)\nprint(reader.odometer.spent)  # (0.0, 0.0)\n\nresult = reader.execute(\'SELECT AVG(age), AVG(income) FROM PUMS.PUMS\')\nprint(reader.odometer.spent)  # approximately (0.4, 10e-6)\n```\n\nThe odometer is advanced immediately before the differentially private query result is returned to the caller.  If the caller wishes to estimate the privacy cost of a query without running it, `get_privacy_cost` can be used:\n\n```python\nreader = from_connection(conn, metadata=metadata, privacy=privacy)\nprint(reader.odometer.spent)  # (0.0, 0.0)\n\ncost = reader.get_privacy_cost(\'SELECT AVG(age), AVG(income) FROM PUMS.PUMS\')\nprint(cost)  # approximately (0.4, 10e-6)\n\nprint(reader.odometer.spent)  # (0.0, 0.0)\n```\n\nNote that the total privacy cost of a session accrues at a slower rate than the sum of the individual query costs obtained by `get_privacy_cost`.  The odometer accrues all invocations of mechanisms for the life of a session, and uses them to compute total spend.\n\n```python\nreader = from_connection(conn, metadata=metadata, privacy=privacy)\nquery = \'SELECT COUNT(*) FROM PUMS.PUMS\'\nepsilon_single, _ = reader.get_privacy_cost(query)\nprint(epsilon_single)  # 0.1\n\n# no queries executed yet\nprint(reader.odometer.spent)  # (0.0, 0.0)\n\nfor _ in range(100):\n    reader.execute(query)\n\nepsilon_many, _ = reader.odometer.spent\nprint(f\'{epsilon_many} < {epsilon_single * 100}\')\n```\n\n## Histograms\n\nSQL `group by` queries represent histograms binned by grouping key.  Queries over a grouping key with unbounded or non-public dimensions expose privacy risk. For example:\n\n```sql\nSELECT last_name, COUNT(*) FROM Sales GROUP BY last_name\n```\n\nIn the above query, if someone with a distinctive last name is included in the database, that person\'s record might accidentally be revealed, even if the noisy count returns 0 or negative.  To prevent this from happening, the system will automatically censor dimensions which would violate differential privacy.\n\n## Private Synopsis\n\nA private synopsis is a pre-computed set of differentially private aggregates that can be filtered and aggregated in various ways to produce new reports.  Because the private synopsis is differentially private, reports generated from the synopsis do not need to have additional privacy applied, and the synopsis can be distributed without risk of additional privacy loss.  Reports over the synopsis can be generated with non-private SQL, within an Excel Pivot Table, or through other common reporting tools.\n\nYou can see a sample [notebook for creating private synopsis](samples/Synopsis.ipynb) suitable for consumption in Excel or SQL.\n\n## Limitations\n\nYou can think of the data access layer as simple middleware that allows composition of `opendp` computations using the SQL language.  The SQL language provides a limited subset of what can be expressed through the full `opendp` library.  For example, the SQL language does not provide a way to set per-field privacy budget.\n\nBecause we delegate the computation of exact aggregates to the underlying database engines, execution through the SQL layer can be considerably faster, particularly with database engines optimized for precomputed aggregates.  However, this design choice means that analysis graphs composed with SQL language do not access data in the engine on a per-row basis.  Therefore, SQL queries do not currently support algorithms that require per-row access, such as quantile algorithms that use underlying values.  This is a limitation that future releases will relax for database engines that support row-based access, such as Spark.\n\nThe SQL processing layer has limited support for bounding contributions when individuals can appear more than once in the data.  This includes ability to perform reservoir sampling to bound contributions of an individual, and to scale the sensitivity parameter.  These parameters are important when querying reporting tables that might be produced from subqueries and joins, but require caution to use safely.\n\nFor this release, we recommend using the SQL functionality while bounding user contribution to 1 row.  The platform defaults to this option by setting `max_contrib` to 1, and should only be overridden if you know what you are doing.  Future releases will focus on making these options easier for non-experts to use safely.\n\n\n## Communication\n\n- You are encouraged to join us on [GitHub Discussions](https://github.com/opendp/opendp/discussions/categories/smartnoise)\n- Please use [GitHub Issues](https://github.com/opendp/smartnoise-sdk/issues) for bug reports and feature requests.\n- For other requests, including security issues, please contact us at [smartnoise@opendp.org](mailto:smartnoise@opendp.org).\n\n## Releases and Contributing\n\nPlease let us know if you encounter a bug by [creating an issue](https://github.com/opendp/smartnoise-sdk/issues).\n\nWe appreciate all contributions. Please review the [contributors guide](../contributing.rst). We welcome pull requests with bug-fixes without prior discussion.\n\nIf you plan to contribute new features, utility functions or extensions, please first open an issue and discuss the feature with us.\n',
     'author': 'SmartNoise Team',
     'author_email': 'smartnoise@opendp.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://smartnoise.org',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<=3.11',
+    'python_requires': '>=3.7,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['snsql',
 'snsql._ast', 'snsql._ast.expressions', 'snsql.reader', 'snsql.sql',
 'snsql.sql._mechanisms', 'snsql.sql.parser', 'snsql.sql.reader', 'snsql.xpath',
 'snsql.xpath.parser'] package_data = \ {'': ['*']} install_requires = \
 ['PyYAML>=5.4.1,<6.0.0', 'antlr4-python3-runtime==4.9.3',
-'graphviz>=0.17,<0.18', 'opendp>=0.6.0,<0.7.0', 'pandasql>=0.7.3,<0.8.0',
-'sqlalchemy>=1.4.23,<2.0.0'] setup_kwargs = { 'name': 'smartnoise-sql',
-'version': '0.2.9.2', 'description': 'Differentially Private SQL Queries',
+'graphviz>=0.17,<0.18', 'opendp>=0.6.0,<0.7.0', 'pandas>=2.0.1,<3.0.0',
+'sqlalchemy>=2.0.0,<3.0.0'] setup_kwargs = { 'name': 'smartnoise-sql',
+'version': '1.0.0', 'description': 'Differentially Private SQL Queries',
 'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-
 yellow.svg)](https://opensource.org/licenses/MIT) [![Python](https://
 img.shields.io/badge/python-3.7%20%7C%203.8-blue)](https://www.python.org/)\n\n
 [https://github.com/opendp/smartnoise-sdk/raw/main/images/SmartNoise/SVG/
 Logo%20Mark_grey.svg]\n\n## SmartNoise SQL\n\nDifferentially private SQL
 queries. Tested with:\n* PostgreSQL\n* SQL Server\n* Spark\n* Pandas
 (SQLite)\n* PrestoDB\n* BigQuery\n\nSmartNoise is intended for scenarios where
@@ -117,8 +117,8 @@
 contributions. Please review the [contributors guide](../contributing.rst). We
 welcome pull requests with bug-fixes without prior discussion.\n\nIf you plan
 to contribute new features, utility functions or extensions, please first open
 an issue and discuss the feature with us.\n', 'author': 'SmartNoise Team',
 'author_email': 'smartnoise@opendp.org', 'maintainer': None,
 'maintainer_email': None, 'url': 'https://smartnoise.org', 'packages':
 packages, 'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.7,<=3.11', } setup(**setup_kwargs)
+'python_requires': '>=3.7,<3.12', } setup(**setup_kwargs)
```

### Comparing `smartnoise-sql-0.2.9.2/PKG-INFO` & `smartnoise-sql-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: smartnoise-sql
-Version: 0.2.9.2
+Version: 1.0.0
 Summary: Differentially Private SQL Queries
 Home-page: https://smartnoise.org
 License: MIT
 Author: SmartNoise Team
 Author-email: smartnoise@opendp.org
-Requires-Python: >=3.7,<=3.11
+Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
 Requires-Dist: antlr4-python3-runtime (==4.9.3)
 Requires-Dist: graphviz (>=0.17,<0.18)
 Requires-Dist: opendp (>=0.6.0,<0.7.0)
-Requires-Dist: pandasql (>=0.7.3,<0.8.0)
-Requires-Dist: sqlalchemy (>=1.4.23,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/opendp/smartnoise-sdk
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8-blue)](https://www.python.org/)
 
 <a href="https://smartnoise.org"><img src="https://github.com/opendp/smartnoise-sdk/raw/main/images/SmartNoise/SVG/Logo%20Mark_grey.svg" align="left" height="65" vspace="8" hspace="18"></a>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: smartnoise-sql Version: 0.2.9.2 Summary:
+Metadata-Version: 2.1 Name: smartnoise-sql Version: 1.0.0 Summary:
 Differentially Private SQL Queries Home-page: https://smartnoise.org License:
 MIT Author: SmartNoise Team Author-email: smartnoise@opendp.org Requires-
-Python: >=3.7,<=3.11 Classifier: License :: OSI Approved :: MIT License
+Python: >=3.7,<3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Requires-Dist: PyYAML (>=5.4.1,<6.0.0) Requires-Dist:
 antlr4-python3-runtime (==4.9.3) Requires-Dist: graphviz (>=0.17,<0.18)
-Requires-Dist: opendp (>=0.6.0,<0.7.0) Requires-Dist: pandasql (>=0.7.3,<0.8.0)
-Requires-Dist: sqlalchemy (>=1.4.23,<2.0.0) Project-URL: Repository, https://
+Requires-Dist: opendp (>=0.6.0,<0.7.0) Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.0,<3.0.0) Project-URL: Repository, https://
 github.com/opendp/smartnoise-sdk Description-Content-Type: text/markdown [!
 [License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
 opensource.org/licenses/MIT) [![Python](https://img.shields.io/badge/python-
 3.7%20%7C%203.8-blue)](https://www.python.org/) [https://github.com/opendp/
 smartnoise-sdk/raw/main/images/SmartNoise/SVG/Logo%20Mark_grey.svg] ##
 SmartNoise SQL Differentially private SQL queries. Tested with: * PostgreSQL *
 SQL Server * Spark * Pandas (SQLite) * PrestoDB * BigQuery SmartNoise is
```

