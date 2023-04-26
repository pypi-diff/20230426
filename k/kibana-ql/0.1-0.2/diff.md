# Comparing `tmp/kibana_ql-0.1.tar.gz` & `tmp/kibana_ql-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kibana_ql-0.1.tar", last modified: Thu Apr 20 08:53:26 2023, max compression
+gzip compressed data, was "kibana_ql-0.2.tar", last modified: Wed Apr 26 02:21:16 2023, max compression
```

## Comparing `kibana_ql-0.1.tar` & `kibana_ql-0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1075 2023-04-20 08:53:10.839458 kibana_ql-0.1/LICENSE
--rw-r--r--   0        0        0      231 2023-04-20 08:53:10.839458 kibana_ql-0.1/README.md
--rw-r--r--   0        0        0      135 2023-04-20 08:53:10.839458 kibana_ql-0.1/kibana_ql/__init__.py
--rw-r--r--   0        0        0     1760 2023-04-20 08:53:10.839458 kibana_ql-0.1/kibana_ql/kql.parsimonious
--rw-r--r--   0        0        0      372 2023-04-20 08:53:10.839458 kibana_ql-0.1/kibana_ql/kql.py
--rw-r--r--   0        0        0        0 2023-04-20 08:53:10.839458 kibana_ql-0.1/kibana_ql/py.typed
--rw-r--r--   0        0        0      814 2023-04-20 08:53:10.839458 kibana_ql-0.1/pyproject.toml
--rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 kibana_ql-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-26 02:21:03.653805 kibana_ql-0.2/LICENSE
+-rw-r--r--   0        0        0      659 2023-04-26 02:21:03.653805 kibana_ql-0.2/README.md
+-rw-r--r--   0        0        0      135 2023-04-26 02:21:03.653805 kibana_ql-0.2/kibana_ql/__init__.py
+-rw-r--r--   0        0        0     1836 2023-04-26 02:21:03.653805 kibana_ql-0.2/kibana_ql/kql.parsimonious
+-rw-r--r--   0        0        0     8411 2023-04-26 02:21:03.653805 kibana_ql-0.2/kibana_ql/kql.py
+-rw-r--r--   0        0        0        0 2023-04-26 02:21:03.653805 kibana_ql-0.2/kibana_ql/py.typed
+-rw-r--r--   0        0        0      840 2023-04-26 02:21:03.653805 kibana_ql-0.2/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 kibana_ql-0.2/PKG-INFO
```

### Comparing `kibana_ql-0.1/LICENSE` & `kibana_ql-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kibana_ql-0.1/kibana_ql/kql.parsimonious` & `kibana_ql-0.2/kibana_ql/kql.parsimonious`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 start = Space* OrQuery? OptionalSpace
 OrQuery = (AndQuery (Or AndQuery)+) / AndQuery
 AndQuery = (NotQuery (And NotQuery)+) / NotQuery
 NotQuery = (Not SubQuery) / SubQuery
 SubQuery = ('(' Space* OrQuery OptionalSpace ')') / NestedQuery
 NestedQuery = (Field Space* ':' Space* '{' Space* OrQuery OptionalSpace '}') / Expression
 Expression = FieldRangeExpression / FieldValueExpression / ValueExpression
-Field = Literal
+Field = Literal / "\0"  # see parsimonious/issues/131
 FieldRangeExpression = Field Space* RangeOperator Space* Literal
 FieldValueExpression = Field Space* ':' Space* ListOfValues
-ValueExpression = Value
+ValueExpression = Value / "\0"  # see parsimonious/issues/131
 ListOfValues = ('(' Space* OrListOfValues OptionalSpace ')') / Value
 OrListOfValues = (AndListOfValues (Or AndListOfValues)+) / AndListOfValues
 AndListOfValues = (NotListOfValues (And NotListOfValues)+) / NotListOfValues
 NotListOfValues = (Not ListOfValues) / ListOfValues
 Value = QuotedString / UnquotedLiteral
 Or = Space+ ~r'or'i Space+
 And = Space+ ~r'and'i Space+
```

### Comparing `kibana_ql-0.1/pyproject.toml` & `kibana_ql-0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 authors = [{name = "Dobatymo", email = "Dobatymo@users.noreply.github.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 dependencies = [
+    "genutility[string]",
     "parsimonious",
 ]
 
 [project.urls]
 Source = "https://github.com/Dobatymo/kibana-ql-python"
 
 [tool.black]
```

