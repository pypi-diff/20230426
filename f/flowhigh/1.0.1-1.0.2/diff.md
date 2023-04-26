# Comparing `tmp/flowhigh-1.0.1.tar.gz` & `tmp/flowhigh-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowhigh-1.0.1.tar", last modified: Fri Apr 21 13:43:28 2023, max compression
+gzip compressed data, was "flowhigh-1.0.2.tar", last modified: Wed Apr 26 10:35:19 2023, max compression
```

## Comparing `flowhigh-1.0.1.tar` & `flowhigh-1.0.2.tar`

### file list

```diff
@@ -1,99 +1,105 @@
--rw-r--r--   0        0        0       36 2023-04-21 13:35:23.000000 flowhigh-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-21 13:41:46.000000 flowhigh-1.0.1/flowhigh/__init__.py
--rw-r--r--   0        0        0       56 2023-04-21 13:35:23.000000 flowhigh-1.0.1/flowhigh/auth/__init__.py
--rw-r--r--   0        0        0     8327 2023-04-21 13:35:23.000000 flowhigh-1.0.1/flowhigh/auth/authentication.py
--rw-r--r--   0        0        0        0 2023-04-21 13:41:46.000000 flowhigh-1.0.1/flowhigh/extraction/__init__.py
--rw-r--r--   0        0        0     7073 2023-04-21 13:35:23.000000 flowhigh-1.0.1/flowhigh/extraction/extractor.py
--rw-r--r--   0        0        0       49 2023-04-21 13:35:23.000000 flowhigh-1.0.1/flowhigh/format/__init__.py
--rw-r--r--   0        0        0    10952 2023-04-21 13:35:23.000000 flowhigh-1.0.1/flowhigh/format/formatting.py
--rw-r--r--   0        0        0      930 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/AP_Types.py
--rw-r--r--   0        0        0     1082 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/Agg.py
--rw-r--r--   0        0        0     8613 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/AntiPattern.py
--rw-r--r--   0        0        0      702 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/AntiPatterns.py
--rw-r--r--   0        0        0     1842 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/Asterisk.py
--rw-r--r--   0        0        0     1895 2023-04-21 13:41:57.000000 flowhigh-1.0.1/flowhigh/model/Attr.py
--rw-r--r--   0        0        0      314 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/BaseExpr.py
--rw-r--r--   0        0        0      298 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/BaseExprCollectionHolder.py
--rw-r--r--   0        0        0      296 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/BaseExprHolder.py
--rw-r--r--   0        0        0       77 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/BetweenType.py
--rw-r--r--   0        0        0     1486 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/Case.py
--rw-r--r--   0        0        0     1134 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/Cast.py
--rw-r--r--   0        0        0     1083 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/ColumnDef.py
--rw-r--r--   0        0        0      974 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/Const.py
--rw-r--r--   0        0        0      156 2023-04-21 13:42:01.000000 flowhigh-1.0.1/flowhigh/model/CoordinateBlock.py
--rw-r--r--   0        0        0     3198 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/Copy.py
--rw-r--r--   0        0        0     2264 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/Create.py
--rw-r--r--   0        0        0     1808 2023-04-21 13:41:57.000000 flowhigh-1.0.1/flowhigh/model/CreateStage.py
--rw-r--r--   0        0        0     1529 2023-04-21 13:41:57.000000 flowhigh-1.0.1/flowhigh/model/CreateView.py
--rw-r--r--   0        0        0      946 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/Current.py
--rw-r--r--   0        0        0      984 2023-04-21 13:41:56.000000 flowhigh-1.0.1/flowhigh/model/Delete.py
--rw-r--r--   0        0        0     3269 2023-04-21 13:41:57.000000 flowhigh-1.0.1/flowhigh/model/DeleteStatement.py
--rw-r--r--   0        0        0       73 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/Direction.py
--rw-r--r--   0        0        0     5253 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/Ds.py
--rw-r--r--   0        0        0      122 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/DsAction.py
--rw-r--r--   0        0        0      130 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/DsSubType.py
--rw-r--r--   0        0        0      153 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/DsType.py
--rw-r--r--   0        0        0     1624 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/Edge.py
--rw-r--r--   0        0        0      713 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/Else.py
--rw-r--r--   0        0        0      636 2023-04-21 13:42:01.000000 flowhigh-1.0.1/flowhigh/model/Error.py
--rw-r--r--   0        0        0      125 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/Expr.py
--rw-r--r--   0        0        0       94 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/ExprCollectionHolder.py
--rw-r--r--   0        0        0      378 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/ExprExprCollectionHolder.py
--rw-r--r--   0        0        0      319 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/ExprExprHolder.py
--rw-r--r--   0        0        0       84 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/ExprHolder.py
--rw-r--r--   0        0        0      726 2023-04-21 13:42:01.000000 flowhigh-1.0.1/flowhigh/model/Filter.py
--rw-r--r--   0        0        0     1948 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/Frame.py
--rw-r--r--   0        0        0     1955 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/Func.py
--rw-r--r--   0        0        0       89 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/FuncType.py
--rw-r--r--   0        0        0      750 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/In.py
--rw-r--r--   0        0        0     1065 2023-04-21 13:41:56.000000 flowhigh-1.0.1/flowhigh/model/InlineTable.py
--rw-r--r--   0        0        0     1805 2023-04-21 13:41:57.000000 flowhigh-1.0.1/flowhigh/model/Insert.py
--rw-r--r--   0        0        0     3269 2023-04-21 13:41:57.000000 flowhigh-1.0.1/flowhigh/model/InsertStatement.py
--rw-r--r--   0        0        0     1733 2023-04-21 13:42:01.000000 flowhigh-1.0.1/flowhigh/model/Join.py
--rw-r--r--   0        0        0       90 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/JoinSubType.py
--rw-r--r--   0        0        0      105 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/JoinType.py
--rw-r--r--   0        0        0     1857 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/MatchRecognize.py
--rw-r--r--   0        0        0      996 2023-04-21 13:42:01.000000 flowhigh-1.0.1/flowhigh/model/Merge.py
--rw-r--r--   0        0        0     3265 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/MergeStatement.py
--rw-r--r--   0        0        0     1061 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/MultiValue.py
--rw-r--r--   0        0        0       79 2023-04-21 13:42:01.000000 flowhigh-1.0.1/flowhigh/model/Named.py
--rw-r--r--   0        0        0     1278 2023-04-21 13:41:56.000000 flowhigh-1.0.1/flowhigh/model/Op.py
--rw-r--r--   0        0        0     1624 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/OpType.py
--rw-r--r--   0        0        0       81 2023-04-21 13:41:56.000000 flowhigh-1.0.1/flowhigh/model/Ordered.py
--rw-r--r--   0        0        0     1074 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/Out.py
--rw-r--r--   0        0        0      984 2023-04-21 13:41:57.000000 flowhigh-1.0.1/flowhigh/model/Page.py
--rw-r--r--   0        0        0       87 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/PageType.py
--rw-r--r--   0        0        0     1501 2023-04-21 13:42:01.000000 flowhigh-1.0.1/flowhigh/model/ParSeQL.py
--rw-r--r--   0        0        0      104 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/ParSeQLStatus.py
--rw-r--r--   0        0        0     1253 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/Position.py
--rw-r--r--   0        0        0       78 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/Quantifier.py
--rw-r--r--   0        0        0     1220 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/QueryingStage.py
--rw-r--r--   0        0        0      125 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/ReferencableExpr.py
--rw-r--r--   0        0        0     2201 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/Rotate.py
--rw-r--r--   0        0        0       84 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/Searchable.py
--rw-r--r--   0        0        0      758 2023-04-21 13:41:57.000000 flowhigh-1.0.1/flowhigh/model/Sort.py
--rw-r--r--   0        0        0     3355 2023-04-21 13:42:01.000000 flowhigh-1.0.1/flowhigh/model/Statement.py
--rw-r--r--   0        0        0     1669 2023-04-21 13:42:00.000000 flowhigh-1.0.1/flowhigh/model/StructRef.py
--rw-r--r--   0        0        0      241 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/SubString.py
--rw-r--r--   0        0        0     5979 2023-04-21 13:42:01.000000 flowhigh-1.0.1/flowhigh/model/TableFunc.py
--rw-r--r--   0        0        0     1633 2023-04-21 13:42:01.000000 flowhigh-1.0.1/flowhigh/model/TableSample.py
--rw-r--r--   0        0        0      992 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/Then.py
--rw-r--r--   0        0        0     1266 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/TreeNode.py
--rw-r--r--   0        0        0       82 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/TypeCast.py
--rw-r--r--   0        0        0      984 2023-04-21 13:41:57.000000 flowhigh-1.0.1/flowhigh/model/Update.py
--rw-r--r--   0        0        0     3269 2023-04-21 13:41:58.000000 flowhigh-1.0.1/flowhigh/model/UpdateStatement.py
--rw-r--r--   0        0        0      768 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/Vagg.py
--rw-r--r--   0        0        0      770 2023-04-21 13:41:59.000000 flowhigh-1.0.1/flowhigh/model/Vfilter.py
--rw-r--r--   0        0        0      162 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/WFuncType.py
--rw-r--r--   0        0        0     1906 2023-04-21 13:42:01.000000 flowhigh-1.0.1/flowhigh/model/Wfunc.py
--rw-r--r--   0        0        0     1235 2023-04-21 13:42:01.000000 flowhigh-1.0.1/flowhigh/model/When.py
--rw-r--r--   0        0        0     3874 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/model/__init__.py
--rw-r--r--   0        0        0       60 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/utils/__init__.py
--rw-r--r--   0        0        0    53547 2023-04-21 13:42:02.000000 flowhigh-1.0.1/flowhigh/utils/converter.py
--rw-r--r--   0        0        0     1254 2023-04-21 13:38:28.000000 flowhigh-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 13:41:46.000000 flowhigh-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 13:41:46.000000 flowhigh-1.0.1/tests/formatting-test/__init__.py
--rw-r--r--   0        0        0    82533 2023-04-21 13:35:23.000000 flowhigh-1.0.1/tests/formatting-test/format_test.py
--rw-r--r--   0        0        0     2899 2023-04-21 13:35:23.000000 flowhigh-1.0.1/tests/input.json
--rw-r--r--   0        0        0      879 2023-04-21 13:35:23.000000 flowhigh-1.0.1/tests/test.py
--rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 flowhigh-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       36 2023-04-26 09:11:00.000000 flowhigh-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 10:33:56.000000 flowhigh-1.0.2/flowhigh/__init__.py
+-rw-r--r--   0        0        0       56 2023-04-26 09:11:00.000000 flowhigh-1.0.2/flowhigh/auth/__init__.py
+-rw-r--r--   0        0        0     8326 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/auth/authentication.py
+-rw-r--r--   0        0        0        0 2023-04-26 10:33:56.000000 flowhigh-1.0.2/flowhigh/extraction/__init__.py
+-rw-r--r--   0        0        0     7073 2023-04-26 09:11:00.000000 flowhigh-1.0.2/flowhigh/extraction/extractor.py
+-rw-r--r--   0        0        0       49 2023-04-26 09:11:00.000000 flowhigh-1.0.2/flowhigh/format/__init__.py
+-rw-r--r--   0        0        0    10952 2023-04-26 09:11:00.000000 flowhigh-1.0.2/flowhigh/format/formatting.py
+-rw-r--r--   0        0        0      930 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/AP_Types.py
+-rw-r--r--   0        0        0     1254 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/Agg.py
+-rw-r--r--   0        0        0       79 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/AggType.py
+-rw-r--r--   0        0        0     8613 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/AntiPattern.py
+-rw-r--r--   0        0        0      702 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/AntiPatterns.py
+-rw-r--r--   0        0        0     1842 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/Asterisk.py
+-rw-r--r--   0        0        0     2159 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/Attr.py
+-rw-r--r--   0        0        0      314 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/BaseExpr.py
+-rw-r--r--   0        0        0      298 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/BaseExprCollectionHolder.py
+-rw-r--r--   0        0        0      276 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/BaseExprHolder.py
+-rw-r--r--   0        0        0       77 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/BetweenType.py
+-rw-r--r--   0        0        0     1525 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Case.py
+-rw-r--r--   0        0        0     1173 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Cast.py
+-rw-r--r--   0        0        0     1083 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/ColumnDef.py
+-rw-r--r--   0        0        0      974 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/Const.py
+-rw-r--r--   0        0        0      156 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/CoordinateBlock.py
+-rw-r--r--   0        0        0     3437 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Copy.py
+-rw-r--r--   0        0        0     2518 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/Create.py
+-rw-r--r--   0        0        0     1808 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/CreateStage.py
+-rw-r--r--   0        0        0     3289 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/CreateTableStatement.py
+-rw-r--r--   0        0        0     1529 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/CreateView.py
+-rw-r--r--   0        0        0      946 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Current.py
+-rw-r--r--   0        0        0     1493 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/DBO.py
+-rw-r--r--   0        0        0      634 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/DBOHier.py
+-rw-r--r--   0        0        0       65 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/DBOSubType.py
+-rw-r--r--   0        0        0      101 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/DBOType.py
+-rw-r--r--   0        0        0       99 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/DefinedAsType.py
+-rw-r--r--   0        0        0      984 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/Delete.py
+-rw-r--r--   0        0        0     3269 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/DeleteStatement.py
+-rw-r--r--   0        0        0       73 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/Direction.py
+-rw-r--r--   0        0        0     4748 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/Ds.py
+-rw-r--r--   0        0        0      445 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/DsAction.py
+-rw-r--r--   0        0        0      130 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/DsSubType.py
+-rw-r--r--   0        0        0      153 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/DsType.py
+-rw-r--r--   0        0        0     1576 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/Edge.py
+-rw-r--r--   0        0        0     1031 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/Else.py
+-rw-r--r--   0        0        0      636 2023-04-26 10:34:10.000000 flowhigh-1.0.2/flowhigh/model/Error.py
+-rw-r--r--   0        0        0      125 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/Expr.py
+-rw-r--r--   0        0        0       94 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/ExprCollectionHolder.py
+-rw-r--r--   0        0        0      378 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/ExprExprCollectionHolder.py
+-rw-r--r--   0        0        0      319 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/ExprExprHolder.py
+-rw-r--r--   0        0        0       84 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/ExprHolder.py
+-rw-r--r--   0        0        0      915 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/Filter.py
+-rw-r--r--   0        0        0       82 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/FilterType.py
+-rw-r--r--   0        0        0     1848 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Frame.py
+-rw-r--r--   0        0        0     2925 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Func.py
+-rw-r--r--   0        0        0      405 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/FuncType.py
+-rw-r--r--   0        0        0      750 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/In.py
+-rw-r--r--   0        0        0     1065 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/InlineTable.py
+-rw-r--r--   0        0        0     2056 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/Insert.py
+-rw-r--r--   0        0        0     3269 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/InsertStatement.py
+-rw-r--r--   0        0        0     1816 2023-04-26 10:34:10.000000 flowhigh-1.0.2/flowhigh/model/Join.py
+-rw-r--r--   0        0        0       90 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/JoinSubType.py
+-rw-r--r--   0        0        0      105 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/JoinType.py
+-rw-r--r--   0        0        0     1857 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/MatchRecognize.py
+-rw-r--r--   0        0        0      996 2023-04-26 10:34:12.000000 flowhigh-1.0.2/flowhigh/model/Merge.py
+-rw-r--r--   0        0        0     3265 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/MergeStatement.py
+-rw-r--r--   0        0        0     1061 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/MultiValue.py
+-rw-r--r--   0        0        0       79 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/Named.py
+-rw-r--r--   0        0        0     1278 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/Op.py
+-rw-r--r--   0        0        0     1784 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/OpType.py
+-rw-r--r--   0        0        0       81 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/Ordered.py
+-rw-r--r--   0        0        0      935 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/Out.py
+-rw-r--r--   0        0        0      984 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/Page.py
+-rw-r--r--   0        0        0       87 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/PageType.py
+-rw-r--r--   0        0        0     2067 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/ParSeQL.py
+-rw-r--r--   0        0        0      104 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/ParSeQLStatus.py
+-rw-r--r--   0        0        0     1253 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/Position.py
+-rw-r--r--   0        0        0       78 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/Quantifier.py
+-rw-r--r--   0        0        0     1220 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/QueryingStage.py
+-rw-r--r--   0        0        0      125 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/ReferencableExpr.py
+-rw-r--r--   0        0        0     2201 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/Rotate.py
+-rw-r--r--   0        0        0       84 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/Searchable.py
+-rw-r--r--   0        0        0      758 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/Sort.py
+-rw-r--r--   0        0        0     3355 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/Statement.py
+-rw-r--r--   0        0        0     1887 2023-04-26 10:34:09.000000 flowhigh-1.0.2/flowhigh/model/StructRef.py
+-rw-r--r--   0        0        0      241 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/SubString.py
+-rw-r--r--   0        0        0     5522 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/TableFunc.py
+-rw-r--r--   0        0        0     1633 2023-04-26 10:34:10.000000 flowhigh-1.0.2/flowhigh/model/TableSample.py
+-rw-r--r--   0        0        0      992 2023-04-26 10:34:06.000000 flowhigh-1.0.2/flowhigh/model/Then.py
+-rw-r--r--   0        0        0     1266 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/TreeNode.py
+-rw-r--r--   0        0        0       82 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/TypeCast.py
+-rw-r--r--   0        0        0      984 2023-04-26 10:34:05.000000 flowhigh-1.0.2/flowhigh/model/Update.py
+-rw-r--r--   0        0        0     3269 2023-04-26 10:34:07.000000 flowhigh-1.0.2/flowhigh/model/UpdateStatement.py
+-rw-r--r--   0        0        0     1274 2023-04-26 10:34:12.000000 flowhigh-1.0.2/flowhigh/model/When.py
+-rw-r--r--   0        0        0      648 2023-04-26 10:34:10.000000 flowhigh-1.0.2/flowhigh/model/WrappedExpr.py
+-rw-r--r--   0        0        0      107 2023-04-26 10:34:08.000000 flowhigh-1.0.2/flowhigh/model/WrappedExprs.py
+-rw-r--r--   0        0        0     4040 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/model/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-26 09:11:00.000000 flowhigh-1.0.2/flowhigh/utils/__init__.py
+-rw-r--r--   0        0        0    63547 2023-04-26 10:34:13.000000 flowhigh-1.0.2/flowhigh/utils/converter.py
+-rw-r--r--   0        0        0     1254 2023-04-26 09:11:00.000000 flowhigh-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 10:33:56.000000 flowhigh-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 10:33:56.000000 flowhigh-1.0.2/tests/formatting-test/__init__.py
+-rw-r--r--   0        0        0    82533 2023-04-26 09:11:00.000000 flowhigh-1.0.2/tests/formatting-test/format_test.py
+-rw-r--r--   0        0        0    24130 2023-04-26 09:11:00.000000 flowhigh-1.0.2/tests/input.json
+-rw-r--r--   0        0        0      879 2023-04-26 09:11:00.000000 flowhigh-1.0.2/tests/test.py
+-rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 flowhigh-1.0.2/PKG-INFO
```

### Comparing `flowhigh-1.0.1/flowhigh/auth/authentication.py` & `flowhigh-1.0.2/flowhigh/auth/authentication.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -191,8 +191,8 @@
                     token = infile.read()
                 token = json.loads(token)
             except:
                 os.remove(cls.TOKEN_PATH)
                 raise Exception("Unable to Read the token file in storage. Deleting the file, try again. If it doesn't "
                                 "work the second time, check for permissions")
 
-        return token
+        return token
```

### Comparing `flowhigh-1.0.1/flowhigh/extraction/extractor.py` & `flowhigh-1.0.2/flowhigh/extraction/extractor.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/format/formatting.py` & `flowhigh-1.0.2/flowhigh/format/formatting.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/AP_Types.py` & `flowhigh-1.0.2/flowhigh/model/AP_Types.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Agg.py` & `flowhigh-1.0.2/flowhigh/model/Agg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
-from flowhigh.model.Filter import Filter
-from flowhigh.model.BaseExprCollectionHolder import BaseExprCollectionHolder
+from flowhigh.model.AggType import AggType
+from flowhigh.model.CoordinateBlock import CoordinateBlock
 from flowhigh.model.Searchable import Searchable
 
 
-class Agg(BaseExprCollectionHolder, Searchable):
-    filter_: Filter = None
+class Agg(CoordinateBlock, Searchable):
+    filter_: list = []
+    exprs: list = []
+    type_: AggType = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
@@ -18,25 +20,29 @@
     construction: Agg
 
     
     def __init__(self) -> None:
         super().__init__()
         self.construction = Agg()
     
-    def with_filter(self, filter_: Filter):
+    def with_filter(self, filter_: list):
         child = filter_
-        if TreeNode in Filter.mro():
-            self.construction.add_child(child)
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), filter_)):
+            self.construction.add_child(node)
         self.construction.filter_ = child
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
     def with_exprs(self, exprs: list):
         child = exprs
         for node in list(filter(lambda el: TreeNode in el.__class__.mro(), exprs)):
             self.construction.add_child(node)
         self.construction.exprs = child
+    
+    def with_type(self, type_: AggType):
+        child = type_
+        self.construction.type_ = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/AntiPattern.py` & `flowhigh-1.0.2/flowhigh/model/AntiPattern.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/AntiPatterns.py` & `flowhigh-1.0.2/flowhigh/model/AntiPatterns.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Asterisk.py` & `flowhigh-1.0.2/flowhigh/model/Asterisk.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Attr.py` & `flowhigh-1.0.2/flowhigh/model/Attr.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     refvar: str = None
     fullref: str = None
     refdb: str = None
     pos: str = None
     refds: str = None
     refatt: str = None
     alias: str = None
+    attref: str = None
     refoutidx: str = None
+    dboref: str = None
     direction: Direction = None
 
     def __init__(self):
         super().__init__()
 
 
 
@@ -60,17 +62,25 @@
         child = refatt
         self.construction.refatt = child
     
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
+    def with_attref(self, attref: str):
+        child = attref
+        self.construction.attref = child
+    
     def with_refoutidx(self, refoutidx: str):
         child = refoutidx
         self.construction.refoutidx = child
     
+    def with_dboref(self, dboref: str):
+        child = dboref
+        self.construction.dboref = child
+    
     def with_direction(self, direction: Direction):
         child = direction
         self.construction.direction = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Case.py` & `flowhigh-1.0.2/flowhigh/model/Case.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 
+from flowhigh.model.WrappedExpr import WrappedExpr
 from flowhigh.model.Else import Else
 from flowhigh.model.Direction import Direction
-from flowhigh.model.Expr import Expr
-from flowhigh.model.ExprExprHolder import ExprExprHolder
+from flowhigh.model.BaseExpr import BaseExpr
 
 
-class Case(ExprExprHolder):
+class Case(BaseExpr):
     Else: Else = None
+    expr: WrappedExpr = None
     when: list = []
 
     def __init__(self):
         super().__init__()
 
 
 
@@ -34,17 +35,17 @@
             self.construction.add_child(child)
         self.construction.Else = child
     
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
-    def with_expr(self, expr: Expr):
+    def with_expr(self, expr: WrappedExpr):
         child = expr
-        if TreeNode in Expr.mro():
+        if TreeNode in WrappedExpr.mro():
             self.construction.add_child(child)
         self.construction.expr = child
     
     def with_when(self, when: list):
         child = when
         for node in list(filter(lambda el: TreeNode in el.__class__.mro(), when)):
             self.construction.add_child(node)
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Cast.py` & `flowhigh-1.0.2/flowhigh/model/Then.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 
 from flowhigh.model.Direction import Direction
 from flowhigh.model.Expr import Expr
 from flowhigh.model.ExprExprHolder import ExprExprHolder
 
 
-class Cast(ExprExprHolder):
-    dataType: str = None
+class Then(ExprExprHolder):
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class CastBuilder (object):
-    construction: Cast
+class ThenBuilder (object):
+    construction: Then
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = Cast()
+        self.construction = Then()
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
-    def with_dataType(self, dataType: str):
-        child = dataType
-        self.construction.dataType = child
-    
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
     def with_expr(self, expr: Expr):
         child = expr
         if TreeNode in Expr.mro():
```

### Comparing `flowhigh-1.0.1/flowhigh/model/ColumnDef.py` & `flowhigh-1.0.2/flowhigh/model/ColumnDef.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Const.py` & `flowhigh-1.0.2/flowhigh/model/Const.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Copy.py` & `flowhigh-1.0.2/flowhigh/model/Copy.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 class Copy(CoordinateBlock):
     fromExp: list = []
     targetColumns: list = []
     pattern: str = None
     copyOptions: str = None
+    ds: list = []
     selectElements: list = []
     into: Ds = None
     fromStage: Ds = None
     partition: list = []
     file: str = None
     fromQuery: Ds = None
     header: bool = None
@@ -49,14 +50,20 @@
         child = pattern
         self.construction.pattern = child
     
     def with_copyOptions(self, copyOptions: str):
         child = copyOptions
         self.construction.copyOptions = child
     
+    def with_ds(self, ds: list):
+        child = ds
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), ds)):
+            self.construction.add_child(node)
+        self.construction.ds = child
+    
     def with_selectElements(self, selectElements: list):
         child = selectElements
         for node in list(filter(lambda el: TreeNode in el.__class__.mro(), selectElements)):
             self.construction.add_child(node)
         self.construction.selectElements = child
     
     def with_fromStage(self, fromStage: Ds):
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Create.py` & `flowhigh-1.0.2/flowhigh/model/Create.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 
 
 class Create(BaseExpr, ReferencableExpr):
     refsch: str = None
     refdb: str = None
     scope: str = None
     refds: str = None
+    query: Ds = None
     columnDef: list = []
     type_: str = None
-    ds: Ds = None
     clusterBy: list = []
+    ds: list = []
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
@@ -46,14 +47,20 @@
         child = scope
         self.construction.scope = child
     
     def with_refds(self, refds: str):
         child = refds
         self.construction.refds = child
     
+    def with_query(self, query: Ds):
+        child = query
+        if TreeNode in Ds.mro():
+            self.construction.add_child(child)
+        self.construction.query = child
+    
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
     def with_columnDef(self, columnDef: list):
         child = columnDef
         for node in list(filter(lambda el: TreeNode in el.__class__.mro(), columnDef)):
@@ -64,21 +71,21 @@
         child = type_
         self.construction.type_ = child
     
     def with_direction(self, direction: Direction):
         child = direction
         self.construction.direction = child
     
-    def with_ds(self, ds: Ds):
-        child = ds
-        if TreeNode in Ds.mro():
-            self.construction.add_child(child)
-        self.construction.ds = child
-    
     def with_clusterBy(self, clusterBy: list):
         child = clusterBy
         for node in list(filter(lambda el: TreeNode in el.__class__.mro(), clusterBy)):
             self.construction.add_child(node)
         self.construction.clusterBy = child
+    
+    def with_ds(self, ds: list):
+        child = ds
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), ds)):
+            self.construction.add_child(node)
+        self.construction.ds = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/CreateStage.py` & `flowhigh-1.0.2/flowhigh/model/CreateStage.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/CreateView.py` & `flowhigh-1.0.2/flowhigh/model/CreateView.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Current.py` & `flowhigh-1.0.2/flowhigh/model/Current.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Delete.py` & `flowhigh-1.0.2/flowhigh/model/Delete.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/DeleteStatement.py` & `flowhigh-1.0.2/flowhigh/model/DeleteStatement.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Ds.py` & `flowhigh-1.0.2/flowhigh/model/Ds.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 
 from flowhigh.model.DsType import DsType
 from flowhigh.model.DsSubType import DsSubType
 from flowhigh.model.DsAction import DsAction
 from flowhigh.model.Out import Out
 from flowhigh.model.In import In
-from flowhigh.model.Filter import Filter
 from flowhigh.model.Agg import Agg
-from flowhigh.model.Vagg import Vagg
 from flowhigh.model.Sort import Sort
 from flowhigh.model.Page import Page
 from flowhigh.model.MatchRecognize import MatchRecognize
 from flowhigh.model.TableSample import TableSample
 from flowhigh.model.Direction import Direction
 from flowhigh.model.BaseExpr import BaseExpr
 from flowhigh.model.ReferencableExpr import ReferencableExpr
@@ -26,26 +24,24 @@
     refdb: str = None
     in_: In = None
     matchRecognize: MatchRecognize = None
     setOp: list = []
     sort: Sort = None
     type_: DsType = None
     out: Out = None
-    filter_: Filter = None
+    filter_: list = []
     tableSample: TableSample = None
     pos: str = None
     refds: str = None
     name: str = None
     action: DsAction = None
     alias: str = None
     subType: DsSubType = None
     refTo: str = None
     page: Page = None
-    vagg: Vagg = None
-    sameAs: list = []
     direction: Direction = None
 
     def __init__(self):
         super().__init__()
 
 
 
@@ -113,18 +109,18 @@
     
     def with_tableSample(self, tableSample: TableSample):
         child = tableSample
         if TreeNode in TableSample.mro():
             self.construction.add_child(child)
         self.construction.tableSample = child
     
-    def with_filter(self, filter_: Filter):
+    def with_filter(self, filter_: list):
         child = filter_
-        if TreeNode in Filter.mro():
-            self.construction.add_child(child)
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), filter_)):
+            self.construction.add_child(node)
         self.construction.filter_ = child
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
     def with_refds(self, refds: str):
@@ -153,25 +149,13 @@
             self.construction.add_child(child)
         self.construction.page = child
     
     def with_refTo(self, refTo: str):
         child = refTo
         self.construction.refTo = child
     
-    def with_vagg(self, vagg: Vagg):
-        child = vagg
-        if TreeNode in Vagg.mro():
-            self.construction.add_child(child)
-        self.construction.vagg = child
-    
-    def with_sameAs(self, sameAs: list):
-        child = sameAs
-        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), sameAs)):
-            self.construction.add_child(node)
-        self.construction.sameAs = child
-    
     def with_direction(self, direction: Direction):
         child = direction
         self.construction.direction = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Edge.py` & `flowhigh-1.0.2/flowhigh/model/Edge.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from flowhigh.model.Direction import Direction
-from flowhigh.model.ExprExprCollectionHolder import ExprExprCollectionHolder
+from flowhigh.model.BaseExpr import BaseExpr
 
 
-class Edge(ExprExprCollectionHolder):
+class Edge(BaseExpr):
     generator: str = None
     exprs: list = []
     type_: str = None
     columnAlias: list = []
 
     def __init__(self):
         super().__init__()
@@ -24,24 +24,24 @@
         super().__init__()
         self.construction = Edge()
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
-    def with_generator(self, generator: str):
-        child = generator
-        self.construction.generator = child
-    
     def with_exprs(self, exprs: list):
         child = exprs
         for node in list(filter(lambda el: TreeNode in el.__class__.mro(), exprs)):
             self.construction.add_child(node)
         self.construction.exprs = child
     
+    def with_generator(self, generator: str):
+        child = generator
+        self.construction.generator = child
+    
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
     def with_type(self, type_: str):
         child = type_
         self.construction.type_ = child
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Else.py` & `flowhigh-1.0.2/flowhigh/model/Update.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 
-from flowhigh.model.Expr import Expr
-from flowhigh.model.BaseExprHolder import BaseExprHolder
+from flowhigh.model.Ds import Ds
+from flowhigh.model.Direction import Direction
+from flowhigh.model.BaseExpr import BaseExpr
 
 
-class Else(BaseExprHolder):
+class Update(BaseExpr):
+    ds: Ds = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class ElseBuilder (object):
-    construction: Else
+class UpdateBuilder (object):
+    construction: Update
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = Else()
+        self.construction = Update()
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
-    def with_expr(self, expr: Expr):
-        child = expr
-        if TreeNode in Expr.mro():
+    def with_alias(self, alias: str):
+        child = alias
+        self.construction.alias = child
+    
+    def with_ds(self, ds: Ds):
+        child = ds
+        if TreeNode in Ds.mro():
             self.construction.add_child(child)
-        self.construction.expr = child
+        self.construction.ds = child
+    
+    def with_direction(self, direction: Direction):
+        child = direction
+        self.construction.direction = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Error.py` & `flowhigh-1.0.2/flowhigh/model/Error.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Filter.py` & `flowhigh-1.0.2/flowhigh/model/Page.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 
-from flowhigh.model.Op import Op
+from flowhigh.model.PageType import PageType
+from flowhigh.model.Const import Const
 from flowhigh.model.CoordinateBlock import CoordinateBlock
+from flowhigh.model.TypeCast import TypeCast
 
 
-class Filter(CoordinateBlock):
-    op: Op = None
+class Page(CoordinateBlock, TypeCast):
+    type_: PageType = None
+    value: Const = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class FilterBuilder (object):
-    construction: Filter
+class PageBuilder (object):
+    construction: Page
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = Filter()
-    
-    def with_op(self, op: Op):
-        child = op
-        if TreeNode in Op.mro():
-            self.construction.add_child(child)
-        self.construction.op = child
+        self.construction = Page()
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
+    
+    def with_type(self, type_: PageType):
+        child = type_
+        self.construction.type_ = child
+    
+    def with_value(self, value: Const):
+        child = value
+        if TreeNode in Const.mro():
+            self.construction.add_child(child)
+        self.construction.value = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Frame.py` & `flowhigh-1.0.2/flowhigh/model/MatchRecognize.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 
-from flowhigh.model.BetweenType import BetweenType
 from flowhigh.model.Direction import Direction
-from flowhigh.model.ExprExprCollectionHolder import ExprExprCollectionHolder
-from flowhigh.model.TypeCast import TypeCast
+from flowhigh.model.BaseExpr import BaseExpr
 
 
-class Frame(ExprExprCollectionHolder, TypeCast):
-    upperPosition: str = None
-    lowerPosition: str = None
-    exprs: list = []
-    upperLimit: str = None
-    lowerLimit: str = None
-    type_: BetweenType = None
+class MatchRecognize(BaseExpr):
+    partitionBy: str = None
+    measures: str = None
+    pattern: str = None
+    define: str = None
+    orderBy: str = None
+    rowMatchAction: str = None
+    rowMatchCondition: str = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class FrameBuilder (object):
-    construction: Frame
+class MatchRecognizeBuilder (object):
+    construction: MatchRecognize
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = Frame()
+        self.construction = MatchRecognize()
     
-    def with_upperPosition(self, upperPosition: str):
-        child = upperPosition
-        self.construction.upperPosition = child
+    def with_partitionBy(self, partitionBy: str):
+        child = partitionBy
+        self.construction.partitionBy = child
+    
+    def with_measures(self, measures: str):
+        child = measures
+        self.construction.measures = child
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
-    def with_lowerPosition(self, lowerPosition: str):
-        child = lowerPosition
-        self.construction.lowerPosition = child
+    def with_define(self, define: str):
+        child = define
+        self.construction.define = child
+    
+    def with_pattern(self, pattern: str):
+        child = pattern
+        self.construction.pattern = child
+    
+    def with_rowMatchAction(self, rowMatchAction: str):
+        child = rowMatchAction
+        self.construction.rowMatchAction = child
+    
+    def with_orderBy(self, orderBy: str):
+        child = orderBy
+        self.construction.orderBy = child
     
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
-    def with_exprs(self, exprs: list):
-        child = exprs
-        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), exprs)):
-            self.construction.add_child(node)
-        self.construction.exprs = child
-    
-    def with_upperLimit(self, upperLimit: str):
-        child = upperLimit
-        self.construction.upperLimit = child
-    
-    def with_lowerLimit(self, lowerLimit: str):
-        child = lowerLimit
-        self.construction.lowerLimit = child
-    
-    def with_type(self, type_: BetweenType):
-        child = type_
-        self.construction.type_ = child
+    def with_rowMatchCondition(self, rowMatchCondition: str):
+        child = rowMatchCondition
+        self.construction.rowMatchCondition = child
     
     def with_direction(self, direction: Direction):
         child = direction
         self.construction.direction = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Func.py` & `flowhigh-1.0.2/flowhigh/model/Func.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 
 from flowhigh.model.FuncType import FuncType
 from flowhigh.model.Quantifier import Quantifier
 from flowhigh.model.Sort import Sort
+from flowhigh.model.WrappedExpr import WrappedExpr
+from flowhigh.model.Frame import Frame
 from flowhigh.model.Direction import Direction
-from flowhigh.model.ExprExprCollectionHolder import ExprExprCollectionHolder
+from flowhigh.model.BaseExpr import BaseExpr
 from flowhigh.model.Named import Named
 from flowhigh.model.TypeCast import TypeCast
 
 
-class Func(ExprExprCollectionHolder, Named, TypeCast):
+class Func(BaseExpr, Named, TypeCast):
+    partition: list = []
     name: str = None
     withinGroup: Sort = None
     exprs: list = []
+    expr: WrappedExpr = None
+    sort: Sort = None
     type_: FuncType = None
     quantifier: Quantifier = None
+    frame: Frame = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
@@ -26,14 +32,20 @@
     construction: Func
 
     
     def __init__(self) -> None:
         super().__init__()
         self.construction = Func()
     
+    def with_partition(self, partition: list):
+        child = partition
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), partition)):
+            self.construction.add_child(node)
+        self.construction.partition = child
+    
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
     def with_withinGroup(self, withinGroup: Sort):
         child = withinGroup
         if TreeNode in Sort.mro():
@@ -50,21 +62,39 @@
             self.construction.add_child(node)
         self.construction.exprs = child
     
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
+    def with_expr(self, expr: WrappedExpr):
+        child = expr
+        if TreeNode in WrappedExpr.mro():
+            self.construction.add_child(child)
+        self.construction.expr = child
+    
+    def with_sort(self, sort: Sort):
+        child = sort
+        if TreeNode in Sort.mro():
+            self.construction.add_child(child)
+        self.construction.sort = child
+    
     def with_quantifier(self, quantifier: Quantifier):
         child = quantifier
         self.construction.quantifier = child
     
     def with_type(self, type_: FuncType):
         child = type_
         self.construction.type_ = child
     
+    def with_frame(self, frame: Frame):
+        child = frame
+        if TreeNode in Frame.mro():
+            self.construction.add_child(child)
+        self.construction.frame = child
+    
     def with_direction(self, direction: Direction):
         child = direction
         self.construction.direction = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/In.py` & `flowhigh-1.0.2/flowhigh/model/In.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/InlineTable.py` & `flowhigh-1.0.2/flowhigh/model/InlineTable.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Insert.py` & `flowhigh-1.0.2/flowhigh/model/Insert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 from flowhigh.model.Direction import Direction
 from flowhigh.model.BaseExpr import BaseExpr
 
 
 class Insert(BaseExpr):
     isElse: bool = None
+    ctes: list = []
     elseIntos: list = []
     insert_type: str = None
     conditionalIntos: list = []
     overwrite: bool = None
 
     def __init__(self):
         super().__init__()
@@ -21,14 +22,20 @@
     construction: Insert
 
     
     def __init__(self) -> None:
         super().__init__()
         self.construction = Insert()
     
+    def with_ctes(self, ctes: list):
+        child = ctes
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), ctes)):
+            self.construction.add_child(node)
+        self.construction.ctes = child
+    
     def with_isElse(self, isElse: bool):
         child = isElse
         self.construction.isElse = child
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
```

### Comparing `flowhigh-1.0.1/flowhigh/model/InsertStatement.py` & `flowhigh-1.0.2/flowhigh/model/InsertStatement.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Join.py` & `flowhigh-1.0.2/flowhigh/model/Frame.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 
-from flowhigh.model.JoinType import JoinType
-from flowhigh.model.JoinSubType import JoinSubType
-from flowhigh.model.Ds import Ds
-from flowhigh.model.Expr import Expr
+from flowhigh.model.BetweenType import BetweenType
 from flowhigh.model.Direction import Direction
-from flowhigh.model.BaseExpr import BaseExpr
+from flowhigh.model.ExprExprCollectionHolder import ExprExprCollectionHolder
+from flowhigh.model.TypeCast import TypeCast
 
 
-class Join(BaseExpr):
-    op: Expr = None
-    natural: bool = None
-    subType: JoinSubType = None
-    type_: JoinType = None
-    ds: Ds = None
+class Frame(ExprExprCollectionHolder, TypeCast):
+    low_val: str = None
+    hi_rel: str = None
+    exprs: list = []
+    low_rel: str = None
+    type_: BetweenType = None
+    hi_val: str = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class JoinBuilder (object):
-    construction: Join
+class FrameBuilder (object):
+    construction: Frame
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = Join()
+        self.construction = Frame()
     
-    def with_op(self, op: Expr):
-        child = op
-        if TreeNode in Expr.mro():
-            self.construction.add_child(child)
-        self.construction.op = child
-    
-    def with_natural(self, natural: bool):
-        child = natural
-        self.construction.natural = child
+    def with_low_val(self, low_val: str):
+        child = low_val
+        self.construction.low_val = child
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
+    def with_hi_rel(self, hi_rel: str):
+        child = hi_rel
+        self.construction.hi_rel = child
+    
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
-    def with_subType(self, subType: JoinSubType):
-        child = subType
-        self.construction.subType = child
+    def with_exprs(self, exprs: list):
+        child = exprs
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), exprs)):
+            self.construction.add_child(node)
+        self.construction.exprs = child
+    
+    def with_low_rel(self, low_rel: str):
+        child = low_rel
+        self.construction.low_rel = child
     
-    def with_type(self, type_: JoinType):
+    def with_type(self, type_: BetweenType):
         child = type_
         self.construction.type_ = child
     
-    def with_ds(self, ds: Ds):
-        child = ds
-        if TreeNode in Ds.mro():
-            self.construction.add_child(child)
-        self.construction.ds = child
-    
     def with_direction(self, direction: Direction):
         child = direction
         self.construction.direction = child
+    
+    def with_hi_val(self, hi_val: str):
+        child = hi_val
+        self.construction.hi_val = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/MatchRecognize.py` & `flowhigh-1.0.2/flowhigh/model/Position.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,51 @@
 
+from flowhigh.model.Expr import Expr
 from flowhigh.model.Direction import Direction
 from flowhigh.model.BaseExpr import BaseExpr
 
 
-class MatchRecognize(BaseExpr):
-    partitionBy: str = None
-    measures: str = None
-    pattern: str = None
-    define: str = None
-    orderBy: str = None
-    rowMatchAction: str = None
-    rowMatchCondition: str = None
+class Position(BaseExpr):
+    string: Expr = None
+    subString: Expr = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class MatchRecognizeBuilder (object):
-    construction: MatchRecognize
+class PositionBuilder (object):
+    construction: Position
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = MatchRecognize()
+        self.construction = Position()
     
-    def with_partitionBy(self, partitionBy: str):
-        child = partitionBy
-        self.construction.partitionBy = child
-    
-    def with_measures(self, measures: str):
-        child = measures
-        self.construction.measures = child
+    def with_string(self, string: Expr):
+        child = string
+        if TreeNode in Expr.mro():
+            self.construction.add_child(child)
+        self.construction.string = child
+    
+    def with_subString(self, subString: Expr):
+        child = subString
+        if TreeNode in Expr.mro():
+            self.construction.add_child(child)
+        self.construction.subString = child
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
-    def with_define(self, define: str):
-        child = define
-        self.construction.define = child
-    
-    def with_pattern(self, pattern: str):
-        child = pattern
-        self.construction.pattern = child
-    
-    def with_rowMatchAction(self, rowMatchAction: str):
-        child = rowMatchAction
-        self.construction.rowMatchAction = child
-    
-    def with_orderBy(self, orderBy: str):
-        child = orderBy
-        self.construction.orderBy = child
-    
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
-    def with_rowMatchCondition(self, rowMatchCondition: str):
-        child = rowMatchCondition
-        self.construction.rowMatchCondition = child
-    
     def with_direction(self, direction: Direction):
         child = direction
         self.construction.direction = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Merge.py` & `flowhigh-1.0.2/flowhigh/model/Merge.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/MergeStatement.py` & `flowhigh-1.0.2/flowhigh/model/MergeStatement.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/MultiValue.py` & `flowhigh-1.0.2/flowhigh/model/MultiValue.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Op.py` & `flowhigh-1.0.2/flowhigh/model/Op.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/OpType.py` & `flowhigh-1.0.2/flowhigh/model/OpType.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,81 +16,89 @@
     NOT = 12
     LIKE = 13
     RLIKE = 14
     REGEX = 15
     NOT_LIKE = 16
     IS = 17
     IS_DISTINCT = 18
-    LIKE_ALL = 19
-    LIKE_SOME = 20
-    LIKE_ANY = 21
-    IS_NOT_DISTINCT = 22
-    IS_DISTINCT_FROM = 23
-    IS_NOT_DISTINCT_FROM = 24
-    IN = 25
-    ANY = 26
-    ALL = 27
-    MOD = 28
-    LT = 29
-    GT = 30
-    GTE = 31
-    LTE = 32
-    IS_NOT = 33
-    PARENTHESIS = 34
-    NOT_EXISTS = 35
-    DIV = 36
-    MULTI = 37
-    BETWEEN = 38
-    NEQJ = 39
-    EXISTS = 40
-    INTERSECT = 41
-    UNION = 42
-    EXCEPT = 43
-    SETMINUS = 44
-    UNION_ALL = 45
-    UNION_DISTINCT = 46
-    REGEXP = 47
-    ASSIGN = 48
-    MATCH = 49
-    NOT_MATCH = 50
-    COLLATE = 51
-    NOT_LIKE_ALL = 52
-    NOT_LIKE_ANY = 53
-    NOT_LIKE_SOME = 54
-    NOT_IN = 55
-    NOT_RLIKE_ALL = 56
-    NOT_RLIKE_ANY = 57
-    NOT_RLIKE_SOME = 58
-    NOT_REGEXP_ALL = 59
-    NOT_REGEXP_ANY = 60
-    NOT_REGEXP_SOME = 61
-    NOT_REGEXP = 62
-    NOT_RLIKE = 63
-    RLIKE_ANY = 64
-    RLIKE_ALL = 65
-    RLIKE_SOME = 66
-    REGEXP_ANY = 67
-    REGEXP_SOME = 68
-    REGEXP_ALL = 69
-    EQ_ALL = 70
-    EQ_ANY = 71
-    NEQ_ALL = 72
-    NEQ_ANY = 73
-    NEQJ_ALL = 74
-    NEQJ_ANY = 75
-    LT_ALL = 76
-    LT_ANY = 77
-    LTE_ALL = 78
-    LTE_ANY = 79
-    GT_ALL = 80
-    GT_ANY = 81
-    GTE_ALL = 82
-    GTE_ANY = 83
-    NSEQ_ANY = 84
-    NSEQ_ALL = 85
-    NSEQ = 86
-    CASE = 87
-    AMPERSAND = 88
-    SOME = 89
-    BOOL_TRUE = 90
-    BOOL_FALSE = 91
+    IS_TRUE = 19
+    IS_FALSE = 20
+    IS_NULL = 21
+    IS_UNKNOWN = 22
+    LIKE_ALL = 23
+    LIKE_SOME = 24
+    LIKE_ANY = 25
+    IS_NOT_DISTINCT = 26
+    IS_DISTINCT_FROM = 27
+    IS_NOT_DISTINCT_FROM = 28
+    IN = 29
+    ANY = 30
+    ALL = 31
+    MOD = 32
+    LT = 33
+    GT = 34
+    GTE = 35
+    LTE = 36
+    IS_NOT = 37
+    IS_NOT_NULL = 38
+    IS_NOT_TRUE = 39
+    IS_NOT_FALSE = 40
+    IS_NOT_UNKNOWN = 41
+    PARENTHESIS = 42
+    NOT_EXISTS = 43
+    DIV = 44
+    MULTI = 45
+    BETWEEN = 46
+    NEQJ = 47
+    EXISTS = 48
+    INTERSECT = 49
+    UNION = 50
+    EXCEPT = 51
+    SETMINUS = 52
+    UNION_ALL = 53
+    UNION_DISTINCT = 54
+    REGEXP = 55
+    ASSIGN = 56
+    MATCH = 57
+    NOT_MATCH = 58
+    COLLATE = 59
+    NOT_LIKE_ALL = 60
+    NOT_LIKE_ANY = 61
+    NOT_LIKE_SOME = 62
+    NOT_IN = 63
+    NOT_RLIKE_ALL = 64
+    NOT_RLIKE_ANY = 65
+    NOT_RLIKE_SOME = 66
+    NOT_REGEXP_ALL = 67
+    NOT_REGEXP_ANY = 68
+    NOT_REGEXP_SOME = 69
+    NOT_REGEXP = 70
+    NOT_RLIKE = 71
+    RLIKE_ANY = 72
+    RLIKE_ALL = 73
+    RLIKE_SOME = 74
+    REGEXP_ANY = 75
+    REGEXP_SOME = 76
+    REGEXP_ALL = 77
+    EQ_ALL = 78
+    EQ_ANY = 79
+    NEQ_ALL = 80
+    NEQ_ANY = 81
+    NEQJ_ALL = 82
+    NEQJ_ANY = 83
+    LT_ALL = 84
+    LT_ANY = 85
+    LTE_ALL = 86
+    LTE_ANY = 87
+    GT_ALL = 88
+    GT_ANY = 89
+    GTE_ALL = 90
+    GTE_ANY = 91
+    NSEQ_ANY = 92
+    NSEQ_ALL = 93
+    NSEQ = 94
+    CASE = 95
+    AMPERSAND = 96
+    SOME = 97
+    BOOL_TRUE = 98
+    BOOL_FALSE = 99
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Out.py` & `flowhigh-1.0.2/flowhigh/model/Out.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 from flowhigh.model.BaseExprCollectionHolder import BaseExprCollectionHolder
 from flowhigh.model.TypeCast import TypeCast
 
 
 class Out(BaseExprCollectionHolder, TypeCast):
     type_: str = None
-    derived: bool = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
@@ -31,14 +30,10 @@
         for node in list(filter(lambda el: TreeNode in el.__class__.mro(), exprs)):
             self.construction.add_child(node)
         self.construction.exprs = child
     
     def with_type(self, type_: str):
         child = type_
         self.construction.type_ = child
-    
-    def with_derived(self, derived: bool):
-        child = derived
-        self.construction.derived = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Page.py` & `flowhigh-1.0.2/flowhigh/model/Else.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 
-from flowhigh.model.PageType import PageType
-from flowhigh.model.Const import Const
-from flowhigh.model.CoordinateBlock import CoordinateBlock
-from flowhigh.model.TypeCast import TypeCast
+from flowhigh.model.WrappedExpr import WrappedExpr
+from flowhigh.model.Direction import Direction
+from flowhigh.model.BaseExpr import BaseExpr
 
 
-class Page(CoordinateBlock, TypeCast):
-    type_: PageType = None
-    value: Const = None
+class Else(BaseExpr):
+    expr: WrappedExpr = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class PageBuilder (object):
-    construction: Page
+class ElseBuilder (object):
+    construction: Else
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = Page()
+        self.construction = Else()
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
-    def with_type(self, type_: PageType):
-        child = type_
-        self.construction.type_ = child
+    def with_alias(self, alias: str):
+        child = alias
+        self.construction.alias = child
     
-    def with_value(self, value: Const):
-        child = value
-        if TreeNode in Const.mro():
+    def with_expr(self, expr: WrappedExpr):
+        child = expr
+        if TreeNode in WrappedExpr.mro():
             self.construction.add_child(child)
-        self.construction.value = child
+        self.construction.expr = child
+    
+    def with_direction(self, direction: Direction):
+        child = direction
+        self.construction.direction = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/ParSeQL.py` & `flowhigh-1.0.2/flowhigh/model/When.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 
-from flowhigh.model.ParSeQLStatus import ParSeQLStatus
-from flowhigh.model.CoordinateBlock import CoordinateBlock
+from flowhigh.model.WrappedExpr import WrappedExpr
+from flowhigh.model.Then import Then
+from flowhigh.model.Direction import Direction
+from flowhigh.model.BaseExpr import BaseExpr
 
 
-class ParSeQL(CoordinateBlock):
-    statement: list = []
-    error: list = []
-    version: str = None
-    status: ParSeQLStatus = None
-    ts: str = None
+class When(BaseExpr):
+    expr: WrappedExpr = None
+    then: Then = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class ParSeQLBuilder (object):
-    construction: ParSeQL
+class WhenBuilder (object):
+    construction: When
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = ParSeQL()
+        self.construction = When()
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
-    def with_statement(self, statement: list):
-        child = statement
-        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), statement)):
-            self.construction.add_child(node)
-        self.construction.statement = child
-    
-    def with_error(self, error: list):
-        child = error
-        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), error)):
-            self.construction.add_child(node)
-        self.construction.error = child
-    
-    def with_version(self, version: str):
-        child = version
-        self.construction.version = child
-    
-    def with_ts(self, ts: str):
-        child = ts
-        self.construction.ts = child
-    
-    def with_status(self, status: ParSeQLStatus):
-        child = status
-        self.construction.status = child
+    def with_alias(self, alias: str):
+        child = alias
+        self.construction.alias = child
+    
+    def with_expr(self, expr: WrappedExpr):
+        child = expr
+        if TreeNode in WrappedExpr.mro():
+            self.construction.add_child(child)
+        self.construction.expr = child
+    
+    def with_then(self, then: Then):
+        child = then
+        if TreeNode in Then.mro():
+            self.construction.add_child(child)
+        self.construction.then = child
+    
+    def with_direction(self, direction: Direction):
+        child = direction
+        self.construction.direction = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Position.py` & `flowhigh-1.0.2/flowhigh/model/TableSample.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,66 @@
 
-from flowhigh.model.Expr import Expr
 from flowhigh.model.Direction import Direction
 from flowhigh.model.BaseExpr import BaseExpr
 
 
-class Position(BaseExpr):
-    string: Expr = None
-    subString: Expr = None
+class TableSample(BaseExpr):
+    sampleMethod: str = None
+    seedType: str = None
+    seed: str = None
+    probability: str = None
+    num: str = None
+    sampleType: str = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class PositionBuilder (object):
-    construction: Position
+class TableSampleBuilder (object):
+    construction: TableSample
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = Position()
+        self.construction = TableSample()
     
-    def with_string(self, string: Expr):
-        child = string
-        if TreeNode in Expr.mro():
-            self.construction.add_child(child)
-        self.construction.string = child
-    
-    def with_subString(self, subString: Expr):
-        child = subString
-        if TreeNode in Expr.mro():
-            self.construction.add_child(child)
-        self.construction.subString = child
+    def with_sampleMethod(self, sampleMethod: str):
+        child = sampleMethod
+        self.construction.sampleMethod = child
+    
+    def with_seed(self, seed: str):
+        child = seed
+        self.construction.seed = child
+    
+    def with_seedType(self, seedType: str):
+        child = seedType
+        self.construction.seedType = child
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
+    def with_probability(self, probability: str):
+        child = probability
+        self.construction.probability = child
+    
+    def with_num(self, num: str):
+        child = num
+        self.construction.num = child
+    
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
+    def with_sampleType(self, sampleType: str):
+        child = sampleType
+        self.construction.sampleType = child
+    
     def with_direction(self, direction: Direction):
         child = direction
         self.construction.direction = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/QueryingStage.py` & `flowhigh-1.0.2/flowhigh/model/QueryingStage.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Rotate.py` & `flowhigh-1.0.2/flowhigh/model/Rotate.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Sort.py` & `flowhigh-1.0.2/flowhigh/model/Sort.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Statement.py` & `flowhigh-1.0.2/flowhigh/model/Statement.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/StructRef.py` & `flowhigh-1.0.2/flowhigh/model/StructRef.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,45 +25,53 @@
         child = refsch
         self.construction.refsch = child
     
     def with_fullref(self, fullref: str):
         child = fullref
         self.construction.fullref = child
     
-    def with_refvar(self, refvar: str):
-        child = refvar
-        self.construction.refvar = child
-    
     def with_refdb(self, refdb: str):
         child = refdb
         self.construction.refdb = child
     
+    def with_refpath(self, refpath: str):
+        child = refpath
+        self.construction.refpath = child
+    
+    def with_refatt(self, refatt: str):
+        child = refatt
+        self.construction.refatt = child
+    
+    def with_attref(self, attref: str):
+        child = attref
+        self.construction.attref = child
+    
+    def with_refvar(self, refvar: str):
+        child = refvar
+        self.construction.refvar = child
+    
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
     def with_refds(self, refds: str):
         child = refds
         self.construction.refds = child
     
-    def with_refpath(self, refpath: str):
-        child = refpath
-        self.construction.refpath = child
-    
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
-    def with_refatt(self, refatt: str):
-        child = refatt
-        self.construction.refatt = child
-    
     def with_refoutidx(self, refoutidx: str):
         child = refoutidx
         self.construction.refoutidx = child
     
     def with_direction(self, direction: Direction):
         child = direction
         self.construction.direction = child
+    
+    def with_dboref(self, dboref: str):
+        child = dboref
+        self.construction.dboref = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/TableFunc.py` & `flowhigh-1.0.2/flowhigh/model/TableFunc.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 from flowhigh.model.Frame import Frame
 from flowhigh.model.Ds import Ds
 from flowhigh.model.DsType import DsType
 from flowhigh.model.DsSubType import DsSubType
 from flowhigh.model.DsAction import DsAction
 from flowhigh.model.Out import Out
 from flowhigh.model.In import In
-from flowhigh.model.Filter import Filter
 from flowhigh.model.Agg import Agg
-from flowhigh.model.Vagg import Vagg
 from flowhigh.model.Page import Page
 from flowhigh.model.MatchRecognize import MatchRecognize
 from flowhigh.model.TableSample import TableSample
 from flowhigh.model.Direction import Direction
 from flowhigh.model.Ordered import Ordered
 
 
@@ -135,18 +133,18 @@
     
     def with_subQuery(self, subQuery: Ds):
         child = subQuery
         if TreeNode in Ds.mro():
             self.construction.add_child(child)
         self.construction.subQuery = child
     
-    def with_filter(self, filter_: Filter):
+    def with_filter(self, filter_: list):
         child = filter_
-        if TreeNode in Filter.mro():
-            self.construction.add_child(child)
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), filter_)):
+            self.construction.add_child(node)
         self.construction.filter_ = child
     
     def with_tableSample(self, tableSample: TableSample):
         child = tableSample
         if TreeNode in TableSample.mro():
             self.construction.add_child(child)
         self.construction.tableSample = child
@@ -167,26 +165,14 @@
     
     def with_page(self, page: Page):
         child = page
         if TreeNode in Page.mro():
             self.construction.add_child(child)
         self.construction.page = child
     
-    def with_vagg(self, vagg: Vagg):
-        child = vagg
-        if TreeNode in Vagg.mro():
-            self.construction.add_child(child)
-        self.construction.vagg = child
-    
-    def with_sameAs(self, sameAs: list):
-        child = sameAs
-        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), sameAs)):
-            self.construction.add_child(node)
-        self.construction.sameAs = child
-    
     def with_frame(self, frame: Frame):
         child = frame
         if TreeNode in Frame.mro():
             self.construction.add_child(child)
         self.construction.frame = child
 
     def build(self):
```

### Comparing `flowhigh-1.0.1/flowhigh/model/TableSample.py` & `flowhigh-1.0.2/flowhigh/model/Cast.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,49 @@
 
+from flowhigh.model.WrappedExpr import WrappedExpr
 from flowhigh.model.Direction import Direction
 from flowhigh.model.BaseExpr import BaseExpr
 
 
-class TableSample(BaseExpr):
-    sampleMethod: str = None
-    seedType: str = None
-    seed: str = None
-    probability: str = None
-    num: str = None
-    sampleType: str = None
+class Cast(BaseExpr):
+    dataType: str = None
+    expr: WrappedExpr = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class TableSampleBuilder (object):
-    construction: TableSample
+class CastBuilder (object):
+    construction: Cast
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = TableSample()
-    
-    def with_sampleMethod(self, sampleMethod: str):
-        child = sampleMethod
-        self.construction.sampleMethod = child
-    
-    def with_seed(self, seed: str):
-        child = seed
-        self.construction.seed = child
-    
-    def with_seedType(self, seedType: str):
-        child = seedType
-        self.construction.seedType = child
+        self.construction = Cast()
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
-    def with_probability(self, probability: str):
-        child = probability
-        self.construction.probability = child
-    
-    def with_num(self, num: str):
-        child = num
-        self.construction.num = child
+    def with_dataType(self, dataType: str):
+        child = dataType
+        self.construction.dataType = child
     
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
-    def with_sampleType(self, sampleType: str):
-        child = sampleType
-        self.construction.sampleType = child
+    def with_expr(self, expr: WrappedExpr):
+        child = expr
+        if TreeNode in WrappedExpr.mro():
+            self.construction.add_child(child)
+        self.construction.expr = child
     
     def with_direction(self, direction: Direction):
         child = direction
         self.construction.direction = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Then.py` & `flowhigh-1.0.2/flowhigh/model/DBOHier.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,30 @@
 
-from flowhigh.model.Direction import Direction
-from flowhigh.model.Expr import Expr
-from flowhigh.model.ExprExprHolder import ExprExprHolder
+from flowhigh.model.TreeNode import TreeNode
 
 
-class Then(ExprExprHolder):
+class DBOHier(TreeNode):
+    dbo: list = []
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class ThenBuilder (object):
-    construction: Then
+class DBOHierBuilder (object):
+    construction: DBOHier
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = Then()
-    
-    def with_pos(self, pos: str):
-        child = pos
-        self.construction.pos = child
-    
-    def with_alias(self, alias: str):
-        child = alias
-        self.construction.alias = child
-    
-    def with_expr(self, expr: Expr):
-        child = expr
-        if TreeNode in Expr.mro():
-            self.construction.add_child(child)
-        self.construction.expr = child
+        self.construction = DBOHier()
     
-    def with_direction(self, direction: Direction):
-        child = direction
-        self.construction.direction = child
+    def with_dbo(self, dbo: list):
+        child = dbo
+        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), dbo)):
+            self.construction.add_child(node)
+        self.construction.dbo = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/TreeNode.py` & `flowhigh-1.0.2/flowhigh/model/TreeNode.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/UpdateStatement.py` & `flowhigh-1.0.2/flowhigh/model/UpdateStatement.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/flowhigh/model/Vfilter.py` & `flowhigh-1.0.2/flowhigh/model/Filter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 
-from flowhigh.model.BaseExprCollectionHolder import BaseExprCollectionHolder
+from flowhigh.model.FilterType import FilterType
+from flowhigh.model.Op import Op
+from flowhigh.model.CoordinateBlock import CoordinateBlock
 
 
-class Vfilter(BaseExprCollectionHolder):
+class Filter(CoordinateBlock):
+    op: Op = None
+    type_: FilterType = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class VfilterBuilder (object):
-    construction: Vfilter
+class FilterBuilder (object):
+    construction: Filter
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = Vfilter()
+        self.construction = Filter()
+    
+    def with_op(self, op: Op):
+        child = op
+        if TreeNode in Op.mro():
+            self.construction.add_child(child)
+        self.construction.op = child
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
-    def with_exprs(self, exprs: list):
-        child = exprs
-        for node in list(filter(lambda el: TreeNode in el.__class__.mro(), exprs)):
-            self.construction.add_child(node)
-        self.construction.exprs = child
+    def with_type(self, type_: FilterType):
+        child = type_
+        self.construction.type_ = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/Wfunc.py` & `flowhigh-1.0.2/flowhigh/model/Join.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,70 @@
 
-from flowhigh.model.WFuncType import WFuncType
-from flowhigh.model.Sort import Sort
-from flowhigh.model.Frame import Frame
-from flowhigh.model.Direction import Direction
+from flowhigh.model.JoinType import JoinType
+from flowhigh.model.JoinSubType import JoinSubType
+from flowhigh.model.DefinedAsType import DefinedAsType
+from flowhigh.model.Ds import Ds
 from flowhigh.model.Expr import Expr
-from flowhigh.model.ExprExprHolder import ExprExprHolder
-from flowhigh.model.TypeCast import TypeCast
-from flowhigh.model.Ordered import Ordered
+from flowhigh.model.Direction import Direction
+from flowhigh.model.BaseExpr import BaseExpr
 
 
-class Wfunc(ExprExprHolder, TypeCast, Ordered):
-    name: str = None
-    sort: Sort = None
-    type_: WFuncType = None
-    frame: Frame = None
+class Join(BaseExpr):
+    op: Expr = None
+    definedAs: DefinedAsType = None
+    subType: JoinSubType = None
+    type_: JoinType = None
+    ds: Ds = None
 
     def __init__(self):
         super().__init__()
 
 
 
 from flowhigh.model.TreeNode import TreeNode
 
-class WfuncBuilder (object):
-    construction: Wfunc
+class JoinBuilder (object):
+    construction: Join
 
     
     def __init__(self) -> None:
         super().__init__()
-        self.construction = Wfunc()
+        self.construction = Join()
+    
+    def with_op(self, op: Expr):
+        child = op
+        if TreeNode in Expr.mro():
+            self.construction.add_child(child)
+        self.construction.op = child
+    
+    def with_definedAs(self, definedAs: DefinedAsType):
+        child = definedAs
+        self.construction.definedAs = child
     
     def with_pos(self, pos: str):
         child = pos
         self.construction.pos = child
     
-    def with_name(self, name: str):
-        child = name
-        self.construction.name = child
-    
     def with_alias(self, alias: str):
         child = alias
         self.construction.alias = child
     
-    def with_expr(self, expr: Expr):
-        child = expr
-        if TreeNode in Expr.mro():
-            self.construction.add_child(child)
-        self.construction.expr = child
-    
-    def with_sort(self, sort: Sort):
-        child = sort
-        if TreeNode in Sort.mro():
-            self.construction.add_child(child)
-        self.construction.sort = child
+    def with_subType(self, subType: JoinSubType):
+        child = subType
+        self.construction.subType = child
     
-    def with_type(self, type_: WFuncType):
+    def with_type(self, type_: JoinType):
         child = type_
         self.construction.type_ = child
     
-    def with_frame(self, frame: Frame):
-        child = frame
-        if TreeNode in Frame.mro():
+    def with_ds(self, ds: Ds):
+        child = ds
+        if TreeNode in Ds.mro():
             self.construction.add_child(child)
-        self.construction.frame = child
+        self.construction.ds = child
     
     def with_direction(self, direction: Direction):
         child = direction
         self.construction.direction = child
 
     def build(self):
         return self.construction
```

### Comparing `flowhigh-1.0.1/flowhigh/model/__init__.py` & `flowhigh-1.0.2/flowhigh/model/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from flowhigh.model.Page import Page, PageBuilder
 from flowhigh.model.Insert import Insert, InsertBuilder
 from flowhigh.model.Update import Update, UpdateBuilder
 from flowhigh.model.DeleteStatement import DeleteStatement, DeleteStatementBuilder
 from flowhigh.model.CreateView import CreateView, CreateViewBuilder
 from flowhigh.model.InsertStatement import InsertStatement, InsertStatementBuilder
 from flowhigh.model.Attr import Attr, AttrBuilder
+from flowhigh.model.DBO import DBO, DBOBuilder
 from flowhigh.model.TreeNode import TreeNode
 from flowhigh.model.CreateStage import CreateStage, CreateStageBuilder
 from flowhigh.model.Sort import Sort, SortBuilder
 from flowhigh.model.Then import Then, ThenBuilder
 from flowhigh.model.MergeStatement import MergeStatement, MergeStatementBuilder
 from flowhigh.model.MultiValue import MultiValue, MultiValueBuilder
 from flowhigh.model.AntiPattern import AntiPattern, AntiPatternBuilder
@@ -21,48 +22,49 @@
 from flowhigh.model.BaseExprHolder import BaseExprHolder
 from flowhigh.model.UpdateStatement import UpdateStatement, UpdateStatementBuilder
 from flowhigh.model.QueryingStage import QueryingStage, QueryingStageBuilder
 from flowhigh.model.Position import Position, PositionBuilder
 from flowhigh.model.ExprCollectionHolder import ExprCollectionHolder
 from flowhigh.model.Const import Const, ConstBuilder
 from flowhigh.model.SubString import SubString
+from flowhigh.model.CreateTableStatement import CreateTableStatement, CreateTableStatementBuilder
 from flowhigh.model.ColumnDef import ColumnDef, ColumnDefBuilder
-from flowhigh.model.Vfilter import Vfilter, VfilterBuilder
 from flowhigh.model.Ds import Ds, DsBuilder
 from flowhigh.model.Out import Out, OutBuilder
 from flowhigh.model.BaseExpr import BaseExpr
 from flowhigh.model.Expr import Expr
 from flowhigh.model.ExprHolder import ExprHolder
 from flowhigh.model.Copy import Copy, CopyBuilder
 from flowhigh.model.ExprExprCollectionHolder import ExprExprCollectionHolder
 from flowhigh.model.TypeCast import TypeCast
 from flowhigh.model.Current import Current, CurrentBuilder
 from flowhigh.model.Cast import Cast, CastBuilder
 from flowhigh.model.Frame import Frame, FrameBuilder
-from flowhigh.model.Vagg import Vagg, VaggBuilder
+from flowhigh.model.WrappedExprs import WrappedExprs
 from flowhigh.model.Rotate import Rotate, RotateBuilder
 from flowhigh.model.BaseExprCollectionHolder import BaseExprCollectionHolder
 from flowhigh.model.In import In, InBuilder
 from flowhigh.model.Func import Func, FuncBuilder
 from flowhigh.model.ReferencableExpr import ReferencableExpr
 from flowhigh.model.Case import Case, CaseBuilder
 from flowhigh.model.StructRef import StructRef, StructRefBuilder
 from flowhigh.model.AntiPatterns import AntiPatterns, AntiPatternsBuilder
 from flowhigh.model.Create import Create, CreateBuilder
 from flowhigh.model.Searchable import Searchable
 from flowhigh.model.MatchRecognize import MatchRecognize, MatchRecognizeBuilder
+from flowhigh.model.DBOHier import DBOHier, DBOHierBuilder
 from flowhigh.model.Asterisk import Asterisk, AsteriskBuilder
 from flowhigh.model.Agg import Agg, AggBuilder
 from flowhigh.model.Named import Named
-from flowhigh.model.Wfunc import Wfunc, WfuncBuilder
 from flowhigh.model.Statement import Statement, StatementBuilder
 from flowhigh.model.CoordinateBlock import CoordinateBlock
 from flowhigh.model.ParSeQL import ParSeQL, ParSeQLBuilder
 from flowhigh.model.TableSample import TableSample, TableSampleBuilder
-from flowhigh.model.Error import Error, ErrorBuilder
 from flowhigh.model.Join import Join, JoinBuilder
+from flowhigh.model.Error import Error, ErrorBuilder
+from flowhigh.model.WrappedExpr import WrappedExpr, WrappedExprBuilder
 from flowhigh.model.When import When, WhenBuilder
 from flowhigh.model.Merge import Merge, MergeBuilder
 from flowhigh.model.Filter import Filter, FilterBuilder
 from flowhigh.model.TableFunc import TableFunc, TableFuncBuilder
 from flowhigh.model.Else import Else, ElseBuilder
 from flowhigh.model.Edge import Edge, EdgeBuilder
```

### Comparing `flowhigh-1.0.1/pyproject.toml` & `flowhigh-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flowhigh"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python SDK for FlowHigh"
 authors = [
     { name = "sonra", email = "support@sonra.io" },
 ]
 dependencies = [
     "requests>=2.14.0",
 ]
```

### Comparing `flowhigh-1.0.1/tests/formatting-test/format_test.py` & `flowhigh-1.0.2/tests/formatting-test/format_test.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/tests/test.py` & `flowhigh-1.0.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `flowhigh-1.0.1/PKG-INFO` & `flowhigh-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowhigh
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python SDK for FlowHigh
 License: Proprietary
 Keywords: SQLAnalyzer SDK Python
 Author-email: sonra <support@sonra.io>
 Requires-Python: >=3.6
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

