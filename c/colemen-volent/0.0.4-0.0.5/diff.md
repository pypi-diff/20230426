# Comparing `tmp/colemen_volent-0.0.4.tar.gz` & `tmp/colemen_volent-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colemen_volent-0.0.4.tar", last modified: Tue Apr 25 13:45:50 2023, max compression
+gzip compressed data, was "colemen_volent-0.0.5.tar", last modified: Wed Apr 26 16:57:46 2023, max compression
```

## Comparing `colemen_volent-0.0.4.tar` & `colemen_volent-0.0.5.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.479682 colemen_volent-0.0.4/
--rw-rw-rw-   0        0        0      469 2023-04-25 13:45:50.479682 colemen_volent-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.327681 colemen_volent-0.0.4/colemen_volent.egg-info/
--rw-rw-rw-   0        0        0      469 2023-04-25 13:45:50.000000 colemen_volent-0.0.4/colemen_volent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1685 2023-04-25 13:45:50.000000 colemen_volent-0.0.4/colemen_volent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 13:45:50.000000 colemen_volent-0.0.4/colemen_volent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-25 13:45:50.000000 colemen_volent-0.0.4/colemen_volent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-25 13:45:50.000000 colemen_volent-0.0.4/colemen_volent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 13:45:50.479682 colemen_volent-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1328 2023-04-25 13:45:48.000000 colemen_volent-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.339682 colemen_volent-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0     2077 2023-04-24 15:33:47.000000 colemen_volent-0.0.4/tests/schema_dict_test.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.361681 colemen_volent-0.0.4/volent/
--rw-rw-rw-   0        0        0     5081 2023-04-18 20:41:28.000000 colemen_volent-0.0.4/volent/Column.py
--rw-rw-rw-   0        0        0     8710 2023-04-18 16:18:27.000000 colemen_volent-0.0.4/volent/Database.py
--rw-rw-rw-   0        0        0    10068 2023-04-25 13:43:31.000000 colemen_volent-0.0.4/volent/Field.py
--rw-rw-rw-   0        0        0    21054 2023-04-21 15:21:37.000000 colemen_volent-0.0.4/volent/Model.py
--rw-rw-rw-   0        0        0     7361 2023-04-21 13:52:04.000000 colemen_volent-0.0.4/volent/NestedField.py
--rw-rw-rw-   0        0        0     2855 2023-04-21 13:13:13.000000 colemen_volent-0.0.4/volent/Relationship.py
--rw-rw-rw-   0        0        0    19451 2023-04-24 17:08:49.000000 colemen_volent-0.0.4/volent/Schema.py
--rw-rw-rw-   0        0        0     1478 2023-04-14 12:21:18.000000 colemen_volent-0.0.4/volent/UniqueConstraint.py
--rw-rw-rw-   0        0        0    15413 2023-04-25 13:44:04.000000 colemen_volent-0.0.4/volent/Volent.py
--rw-rw-rw-   0        0        0       59 2023-04-11 20:23:11.000000 colemen_volent-0.0.4/volent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.406681 colemen_volent-0.0.4/volent/data_types/
--rw-rw-rw-   0        0        0      876 2023-04-24 14:12:42.000000 colemen_volent-0.0.4/volent/data_types/BigInt.py
--rw-rw-rw-   0        0        0      695 2023-04-24 14:13:18.000000 colemen_volent-0.0.4/volent/data_types/Bool.py
--rw-rw-rw-   0        0        0     1738 2023-04-24 14:13:06.000000 colemen_volent-0.0.4/volent/data_types/Decimal.py
--rw-rw-rw-   0        0        0     1452 2023-04-24 14:12:30.000000 colemen_volent-0.0.4/volent/data_types/EncodedPrimary.py
--rw-rw-rw-   0        0        0     1656 2023-04-24 17:13:25.000000 colemen_volent-0.0.4/volent/data_types/Integer.py
--rw-rw-rw-   0        0        0     1587 2023-04-11 19:39:38.000000 colemen_volent-0.0.4/volent/data_types/String.py
--rw-rw-rw-   0        0        0      909 2023-04-24 14:13:20.000000 colemen_volent-0.0.4/volent/data_types/TinyInt.py
--rw-rw-rw-   0        0        0     4404 2023-04-18 13:41:38.000000 colemen_volent-0.0.4/volent/data_types/TypeBase.py
--rw-rw-rw-   0        0        0      472 2023-04-21 16:39:20.000000 colemen_volent-0.0.4/volent/data_types/__init__.py
--rw-rw-rw-   0        0        0      873 2023-04-14 13:42:19.000000 colemen_volent-0.0.4/volent/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.417682 colemen_volent-0.0.4/volent/mixins/
--rw-rw-rw-   0        0        0    22897 2023-04-25 13:42:18.000000 colemen_volent-0.0.4/volent/mixins/DatabaseConnection.py
--rw-rw-rw-   0        0        0      729 2023-04-11 19:34:06.000000 colemen_volent-0.0.4/volent/mixins/EntityName.py
--rw-rw-rw-   0        0        0    17876 2023-04-18 14:57:37.000000 colemen_volent-0.0.4/volent/mixins/MySQLGeneratorMixin.py
--rw-rw-rw-   0        0        0     3686 2023-04-13 19:47:45.000000 colemen_volent-0.0.4/volent/mixins/OrderedClass.py
--rw-rw-rw-   0        0        0      346 2023-04-18 13:01:17.000000 colemen_volent-0.0.4/volent/mixins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.438681 colemen_volent-0.0.4/volent/query/
--rw-rw-rw-   0        0        0     2805 2023-04-18 20:17:21.000000 colemen_volent-0.0.4/volent/query/Insert.py
--rw-rw-rw-   0        0        0    13462 2023-04-21 15:47:20.000000 colemen_volent-0.0.4/volent/query/Query.py
--rw-rw-rw-   0        0        0     6815 2023-04-21 15:25:12.000000 colemen_volent-0.0.4/volent/query/Select.py
--rw-rw-rw-   0        0        0     4240 2023-04-21 15:25:16.000000 colemen_volent-0.0.4/volent/query/Update.py
--rw-rw-rw-   0        0        0     2620 2023-04-18 18:54:55.000000 colemen_volent-0.0.4/volent/query/WhereMixin.py
--rw-rw-rw-   0        0        0      155 2023-04-18 19:08:07.000000 colemen_volent-0.0.4/volent/query/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.442684 colemen_volent-0.0.4/volent/settings/
--rw-rw-rw-   0        0        0      129 2023-04-11 19:11:30.000000 colemen_volent-0.0.4/volent/settings/__init__.py
--rw-rw-rw-   0        0        0     6183 2023-04-24 14:05:40.000000 colemen_volent-0.0.4/volent/settings/control.py
--rw-rw-rw-   0        0        0      152 2023-04-11 20:12:31.000000 colemen_volent-0.0.4/volent/settings/globe.py
--rw-rw-rw-   0        0        0     2165 2023-04-18 18:20:43.000000 colemen_volent-0.0.4/volent/settings/types.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.460681 colemen_volent-0.0.4/volent/tests/
--rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.0.4/volent/tests/__init__.py
--rw-rw-rw-   0        0        0     4222 2023-04-24 17:14:04.000000 colemen_volent-0.0.4/volent/tests/schema_dict_test.py
--rw-rw-rw-   0        0        0     8452 2023-04-24 17:01:23.000000 colemen_volent-0.0.4/volent/tests/validators_test.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.477681 colemen_volent-0.0.4/volent/validate/
--rw-rw-rw-   0        0        0     3075 2023-04-24 16:59:56.000000 colemen_volent-0.0.4/volent/validate/CreditCardNumber.py
--rw-rw-rw-   0        0        0     2866 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/Email.py
--rw-rw-rw-   0        0        0     1620 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/Equal.py
--rw-rw-rw-   0        0        0     1709 2023-04-21 16:10:49.000000 colemen_volent-0.0.4/volent/validate/FutureUnixDate.py
--rw-rw-rw-   0        0        0     3915 2023-04-24 16:09:19.000000 colemen_volent-0.0.4/volent/validate/IpAddress.py
--rw-rw-rw-   0        0        0     2448 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/Length.py
--rw-rw-rw-   0        0        0     3658 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/NoneOf.py
--rw-rw-rw-   0        0        0     2761 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/OneOf.py
--rw-rw-rw-   0        0        0     1721 2023-04-21 16:10:42.000000 colemen_volent-0.0.4/volent/validate/PastUnixDate.py
--rw-rw-rw-   0        0        0     2394 2023-04-24 16:42:48.000000 colemen_volent-0.0.4/volent/validate/PhoneNumber.py
--rw-rw-rw-   0        0        0     5757 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/Range.py
--rw-rw-rw-   0        0        0     2725 2023-04-24 17:08:33.000000 colemen_volent-0.0.4/volent/validate/Regex.py
--rw-rw-rw-   0        0        0     2265 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/SocialSecurityNumber.py
--rw-rw-rw-   0        0        0     2490 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/StrongPassword.py
--rw-rw-rw-   0        0        0     1414 2023-04-14 13:25:54.000000 colemen_volent-0.0.4/volent/validate/Validator.py
--rw-rw-rw-   0        0        0      770 2023-04-24 16:48:21.000000 colemen_volent-0.0.4/volent/validate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.389936 colemen_volent-0.0.5/
+-rw-rw-rw-   0        0        0      469 2023-04-26 16:57:46.388936 colemen_volent-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.272935 colemen_volent-0.0.5/colemen_volent.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-04-26 16:57:46.000000 colemen_volent-0.0.5/colemen_volent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1708 2023-04-26 16:57:46.000000 colemen_volent-0.0.5/colemen_volent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 16:57:46.000000 colemen_volent-0.0.5/colemen_volent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-26 16:57:46.000000 colemen_volent-0.0.5/colemen_volent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-26 16:57:46.000000 colemen_volent-0.0.5/colemen_volent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 16:57:46.389936 colemen_volent-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2023-04-26 16:57:45.000000 colemen_volent-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.282936 colemen_volent-0.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     2077 2023-04-24 15:33:47.000000 colemen_volent-0.0.5/tests/schema_dict_test.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.295936 colemen_volent-0.0.5/volent/
+-rw-rw-rw-   0        0        0     5698 2023-04-26 16:27:55.000000 colemen_volent-0.0.5/volent/Column.py
+-rw-rw-rw-   0        0        0     8710 2023-04-18 16:18:27.000000 colemen_volent-0.0.5/volent/Database.py
+-rw-rw-rw-   0        0        0    12556 2023-04-26 16:48:34.000000 colemen_volent-0.0.5/volent/Field.py
+-rw-rw-rw-   0        0        0    21292 2023-04-26 16:52:50.000000 colemen_volent-0.0.5/volent/Model.py
+-rw-rw-rw-   0        0        0     7361 2023-04-21 13:52:04.000000 colemen_volent-0.0.5/volent/NestedField.py
+-rw-rw-rw-   0        0        0     2855 2023-04-21 13:13:13.000000 colemen_volent-0.0.5/volent/Relationship.py
+-rw-rw-rw-   0        0        0    22862 2023-04-26 16:27:13.000000 colemen_volent-0.0.5/volent/Schema.py
+-rw-rw-rw-   0        0        0     1478 2023-04-14 12:21:18.000000 colemen_volent-0.0.5/volent/UniqueConstraint.py
+-rw-rw-rw-   0        0        0    15407 2023-04-26 16:53:59.000000 colemen_volent-0.0.5/volent/Volent.py
+-rw-rw-rw-   0        0        0       59 2023-04-11 20:23:11.000000 colemen_volent-0.0.5/volent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.339935 colemen_volent-0.0.5/volent/data_types/
+-rw-rw-rw-   0        0        0     2345 2023-04-26 13:07:40.000000 colemen_volent-0.0.5/volent/data_types/BigInt.py
+-rw-rw-rw-   0        0        0     1376 2023-04-25 19:35:38.000000 colemen_volent-0.0.5/volent/data_types/Bool.py
+-rw-rw-rw-   0        0        0     1738 2023-04-24 14:13:06.000000 colemen_volent-0.0.5/volent/data_types/Decimal.py
+-rw-rw-rw-   0        0        0     1793 2023-04-26 13:07:50.000000 colemen_volent-0.0.5/volent/data_types/EncodedPrimary.py
+-rw-rw-rw-   0        0        0     1954 2023-04-26 16:26:49.000000 colemen_volent-0.0.5/volent/data_types/Integer.py
+-rw-rw-rw-   0        0        0     1587 2023-04-11 19:39:38.000000 colemen_volent-0.0.5/volent/data_types/String.py
+-rw-rw-rw-   0        0        0      909 2023-04-24 14:13:20.000000 colemen_volent-0.0.5/volent/data_types/TinyInt.py
+-rw-rw-rw-   0        0        0     4404 2023-04-18 13:41:38.000000 colemen_volent-0.0.5/volent/data_types/TypeBase.py
+-rw-rw-rw-   0        0        0      472 2023-04-21 16:39:20.000000 colemen_volent-0.0.5/volent/data_types/__init__.py
+-rw-rw-rw-   0        0        0     1055 2023-04-25 19:27:57.000000 colemen_volent-0.0.5/volent/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.346936 colemen_volent-0.0.5/volent/mixins/
+-rw-rw-rw-   0        0        0    22897 2023-04-26 13:08:22.000000 colemen_volent-0.0.5/volent/mixins/DatabaseConnection.py
+-rw-rw-rw-   0        0        0      729 2023-04-11 19:34:06.000000 colemen_volent-0.0.5/volent/mixins/EntityName.py
+-rw-rw-rw-   0        0        0    17876 2023-04-18 14:57:37.000000 colemen_volent-0.0.5/volent/mixins/MySQLGeneratorMixin.py
+-rw-rw-rw-   0        0        0     3686 2023-04-13 19:47:45.000000 colemen_volent-0.0.5/volent/mixins/OrderedClass.py
+-rw-rw-rw-   0        0        0      346 2023-04-18 13:01:17.000000 colemen_volent-0.0.5/volent/mixins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.355936 colemen_volent-0.0.5/volent/query/
+-rw-rw-rw-   0        0        0     2579 2023-04-26 16:57:41.000000 colemen_volent-0.0.5/volent/query/Delete.py
+-rw-rw-rw-   0        0        0     5324 2023-04-26 16:27:03.000000 colemen_volent-0.0.5/volent/query/Insert.py
+-rw-rw-rw-   0        0        0    15281 2023-04-26 16:28:20.000000 colemen_volent-0.0.5/volent/query/Query.py
+-rw-rw-rw-   0        0        0     7173 2023-04-26 13:08:42.000000 colemen_volent-0.0.5/volent/query/Select.py
+-rw-rw-rw-   0        0        0     4232 2023-04-26 16:51:08.000000 colemen_volent-0.0.5/volent/query/Update.py
+-rw-rw-rw-   0        0        0     5171 2023-04-25 16:18:28.000000 colemen_volent-0.0.5/volent/query/WhereMixin.py
+-rw-rw-rw-   0        0        0      183 2023-04-26 16:50:07.000000 colemen_volent-0.0.5/volent/query/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.360937 colemen_volent-0.0.5/volent/settings/
+-rw-rw-rw-   0        0        0      129 2023-04-11 19:11:30.000000 colemen_volent-0.0.5/volent/settings/__init__.py
+-rw-rw-rw-   0        0        0     6183 2023-04-24 14:05:40.000000 colemen_volent-0.0.5/volent/settings/control.py
+-rw-rw-rw-   0        0        0      152 2023-04-11 20:12:31.000000 colemen_volent-0.0.5/volent/settings/globe.py
+-rw-rw-rw-   0        0        0     2165 2023-04-18 18:20:43.000000 colemen_volent-0.0.5/volent/settings/types.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.370935 colemen_volent-0.0.5/volent/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.0.5/volent/tests/__init__.py
+-rw-rw-rw-   0        0        0     4222 2023-04-24 17:14:04.000000 colemen_volent-0.0.5/volent/tests/schema_dict_test.py
+-rw-rw-rw-   0        0        0     8452 2023-04-24 17:01:23.000000 colemen_volent-0.0.5/volent/tests/validators_test.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.387936 colemen_volent-0.0.5/volent/validate/
+-rw-rw-rw-   0        0        0     3075 2023-04-24 16:59:56.000000 colemen_volent-0.0.5/volent/validate/CreditCardNumber.py
+-rw-rw-rw-   0        0        0     2866 2023-04-14 13:23:23.000000 colemen_volent-0.0.5/volent/validate/Email.py
+-rw-rw-rw-   0        0        0     1620 2023-04-14 13:23:23.000000 colemen_volent-0.0.5/volent/validate/Equal.py
+-rw-rw-rw-   0        0        0     1709 2023-04-21 16:10:49.000000 colemen_volent-0.0.5/volent/validate/FutureUnixDate.py
+-rw-rw-rw-   0        0        0     3993 2023-04-25 15:53:35.000000 colemen_volent-0.0.5/volent/validate/IpAddress.py
+-rw-rw-rw-   0        0        0     2448 2023-04-14 13:23:23.000000 colemen_volent-0.0.5/volent/validate/Length.py
+-rw-rw-rw-   0        0        0     3658 2023-04-14 13:23:23.000000 colemen_volent-0.0.5/volent/validate/NoneOf.py
+-rw-rw-rw-   0        0        0     2771 2023-04-25 15:57:11.000000 colemen_volent-0.0.5/volent/validate/OneOf.py
+-rw-rw-rw-   0        0        0     1721 2023-04-21 16:10:42.000000 colemen_volent-0.0.5/volent/validate/PastUnixDate.py
+-rw-rw-rw-   0        0        0     2394 2023-04-24 16:42:48.000000 colemen_volent-0.0.5/volent/validate/PhoneNumber.py
+-rw-rw-rw-   0        0        0     5995 2023-04-25 15:51:54.000000 colemen_volent-0.0.5/volent/validate/Range.py
+-rw-rw-rw-   0        0        0     2725 2023-04-24 17:08:33.000000 colemen_volent-0.0.5/volent/validate/Regex.py
+-rw-rw-rw-   0        0        0     2265 2023-04-14 13:23:23.000000 colemen_volent-0.0.5/volent/validate/SocialSecurityNumber.py
+-rw-rw-rw-   0        0        0     2490 2023-04-14 13:23:23.000000 colemen_volent-0.0.5/volent/validate/StrongPassword.py
+-rw-rw-rw-   0        0        0     1414 2023-04-14 13:25:54.000000 colemen_volent-0.0.5/volent/validate/Validator.py
+-rw-rw-rw-   0        0        0      770 2023-04-24 16:48:21.000000 colemen_volent-0.0.5/volent/validate/__init__.py
```

### Comparing `colemen_volent-0.0.4/colemen_volent.egg-info/SOURCES.txt` & `colemen_volent-0.0.5/colemen_volent.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 volent/data_types/TypeBase.py
 volent/data_types/__init__.py
 volent/mixins/DatabaseConnection.py
 volent/mixins/EntityName.py
 volent/mixins/MySQLGeneratorMixin.py
 volent/mixins/OrderedClass.py
 volent/mixins/__init__.py
+volent/query/Delete.py
 volent/query/Insert.py
 volent/query/Query.py
 volent/query/Select.py
 volent/query/Update.py
 volent/query/WhereMixin.py
 volent/query/__init__.py
 volent/settings/__init__.py
```

### Comparing `colemen_volent-0.0.4/setup.py` & `colemen_volent-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from glob import glob
 from setuptools import setup, find_packages
 import colemen_utilities.build_utils.general as _gen
 
 
-VERSION='0.0.4'
+VERSION='0.0.5'
 DESCRIPTION = 'volent'
 LONG_DESCRIPTION = 'None'
 
 
 _root_path = f"{os.getcwd()}/volent"
 PY_MODULES = _gen.list_py_modules(
     _root_path,
```

### Comparing `colemen_volent-0.0.4/tests/schema_dict_test.py` & `colemen_volent-0.0.5/tests/schema_dict_test.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/Column.py` & `colemen_volent-0.0.5/volent/Column.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 
 @dataclass
 class Column(MySQLGeneratorMixin):
     model:_t.model_type = None
 
     name:str = None
     data_type:_t.type_base_type = None
-    default = None
+    default = _settings.types.no_default
+    on_update = _t.undefined
+    '''The value to set this column to when an update is performed'''
+    on_insert = _t.undefined
+    '''The value to set this column to when an insertion is performed'''
     nullable:bool = None
     comment:str = None
     is_foreign_key:bool = None
     is_primary:bool = None
     auto_increment = None
     unique:bool = None
     is_private:bool = None
@@ -41,28 +45,32 @@
         comment:str=None,
         is_foreign_key:bool=False,
         is_primary:bool=False,
         auto_increment:bool=False,
         unique:bool=False,
         default=_settings.types.no_default,
         dump_only=False,
+        on_update=_t.undefined,
+        on_insert=_t.undefined,
         ):
 
         self.name = name
         self.data_type = data_type
         self.default = default
+        self.on_update = on_update
+        self.on_insert = on_insert
         self.unique = unique
         self.nullable = nullable
 
         self.comment = comment
         self.is_foreign_key = is_foreign_key
         self.is_primary = is_primary
         self.auto_increment = auto_increment
         self.dump_only = dump_only
-        self._column_value = None
+        self._column_value = _t.undefined
 
     @property
     def summary(self):
         '''
             Get this Column's summary
 
             `default`:None
@@ -130,15 +138,15 @@
             `@memberOf`: Column
             `@property`: value
         '''
         value = self._column_value
         if value == _t.undefined:
             if self.default != _t.no_default:
                 value = self.default
-            self.value = value
+                self._column_value = value
         return value
 
     @value.setter
     def value(self,value):
         '''
             Set the Column's value property
 
@@ -188,12 +196,16 @@
             ----------
             `@author`: Colemen Atwood
             `@created`: 03-27-2023 11:05:37
             `@memberOf`: Column
             `@property`: serialized_value
         '''
         value = self.value
+        if hasattr(self.data_type,"serializer"):
+            return self.data_type.serializer(value,self.name)
         if hasattr(self.data_type,"__deserialize"):
             return self.data_type.__deserialize(value)
+        if hasattr(self.data_type,"deserialized_value"):
+            return self.data_type.deserialized_value(value)
         return value
```

### Comparing `colemen_volent-0.0.4/volent/Database.py` & `colemen_volent-0.0.5/volent/Database.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/Field.py` & `colemen_volent-0.0.5/volent/Field.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,77 +29,98 @@
     schema:_t.schema_type = None
 
 
     name:str = None
 
     # _fields:Iterable[_t.column_type] = None
     _description:str = None
+    _example:str = None
+    _ignore_null:bool = False
     column:_t.column_type = None
 
 
     required:bool = False
     nullable:bool = True
     default = None
     validators = None
     _data_type:_t.type_base_type = None
     _value = None
     '''The value associated to this field if there is no column'''
+    _open_api_location:str = None
 
 
     def __init__(
         self,
         column:str=None,
         required:bool=False,
         nullable:bool=True,
         empty_string_is_null:bool=True,
+        ignore_null:bool=False,
         default=_settings.types.no_default,
         validate=None,
         data_type:_t.type_base_type=None,
         description:str=None,
+        example=None,
+        open_api_location=None,
         ):
         '''
             Create a schema Field
             ----------
 
             Arguments
             -------------------------
             [`column`=None] {str}
                 The name of the column that this field represents.
                 The dot delimited path to the column
 
                 If None, it will attempt to find a matching column in the model.
 
             [`required`=False] {bool}
-                arg_description
+                True if this field MUST have a value.
+                
+            [`nullable`=True] {bool}
+                False if this field does not allow null values.
 
             [`empty_string_is_null`=True] {bool}
                 Treat empty strings as None
 
             [`default`] {any}
                 The default value to assign to this field
 
             [`validate`=None] {any}
                 A list of validators to apply to this field
 
+            [`ignore_null`=False] {bool}
+                A list of validators to apply to this field
+
+            [`description`=None] {any}
+                A description of what this form stores.
+
+            [`example`=None] {any}
+                An example value of what this field stores.
+
             Meta
             ----------
             `author`: Colemen Atwood
             `created`: 03-26-2023 09:34:14
             `memberOf`: Field
             `version`: 1.0
             `method_name`: Field
             * @xxx [04-14-2023 08:24:58]: documentation for Field
         '''
         self.column = column
         self.default = default
         self._description = description
+        self._example = example
         self.required = required
         self.nullable = nullable
         self.empty_string_is_null = empty_string_is_null
+        self._ignore_null = ignore_null
         self._data_type = data_type
+        self._open_api_location = open_api_location
 
         self.validators = c.arr.force_list(validate,allow_nulls=False)
 
 
     @property
     def summary(self):
         '''
@@ -183,14 +204,34 @@
         '''
         if self.column is not None:
             self.column.value = value
         else:
             self._value = value
 
     @property
+    def data_type_instance(self):
+        '''
+            Get this Field's data_type_instance
+
+            `default`:None
+
+
+            Meta
+            ----------
+            `@author`: Colemen Atwood
+            `@created`: 04-25-2023 14:11:58
+            `@memberOf`: Field
+            `@property`: data_type_instance
+        '''
+        if self._data_type is not None:
+            return self._data_type
+        elif self.column is not None:
+            return self.column.data_type
+
+    @property
     def data_type(self):
         '''
             Get this Field's data_type
 
             `default`:None
 
 
@@ -205,42 +246,41 @@
         if self._data_type is not None:
             if hasattr(self._data_type,"open_api_data_type"):
                 value = self._data_type.open_api_data_type
         elif self.column is not None:
             value = self.column.deserialized_value()
         return value
 
-
-
     def validate_value(self,value):
         val = value
         if self._data_type is not None:
+            if hasattr(self._data_type,"serializer"):
+                val = self._data_type.serializer(val,self.name)
             if hasattr(self._data_type,"deserialized_value"):
                 val = self._data_type.deserialized_value(val)
 
 
         if isinstance(val,self._data_type.python_data_type) is False:
             if self.nullable is True and val is None:
                 pass
             else:
-                raise ValidationError(f"{self.name} expects {self._data_type.python__data_type} types.",self.name)
+                raise ValidationError(f"{self.name} expects {self._data_type.python_data_type} types, {type(value)} provided.",self.name)
 
         # if self._less_than_data_len(val) is False:
         #     raise ValidationError(f"{self.name} is too long.",self.name)
 
 
 
         if self._is_null(val):
             raise ValidationError(f"{self.name} cannot be null.",self.name)
 
 
         for valid in self.validators:
             val = valid(val,self.name)
 
-
     def validate(self):
         '''
             Executes the validation methods on this field's value.
 
             if this field is not associated to a column, it will automatically use the validate_value method.
             This is important because columns require additional steps before they can be validated.
 
@@ -252,33 +292,33 @@
             `author`: Colemen Atwood
             `created`: 04-24-2023 09:50:01
             `memberOf`: Field
             `version`: 1.0
             `method_name`: validate
             * @xxx [04-24-2023 09:54:22]: documentation for validate
         '''
+        if self.value is None and self._ignore_null is True:
+            return
         if self.column is None:
             return self.validate_value(self.value)
         # val = self.value
         val = self.column.deserialized_value
         # val = self.column.data_type.
 
         if isinstance(val,self.column.data_type.python_data_type) is False:
             if self.column.is_primary is True:
                 pass
             elif self.column.nullable is True:
                 pass
             else:
-                raise ValidationError(f"{self.column.name} expects {self.column.data_type.python_data_type} types.",self.name)
+                raise ValidationError(f"{self.column.name} expects {self.column.data_type.python_data_type} types, {type(self.value)} provided.",self.name)
 
         if self._less_than_data_len(val) is False:
             raise ValidationError(f"{self.column.name} is too long.",self.name)
 
-
-
         if self._is_null(val):
             raise ValidationError(f"{self.name} cannot be null.",self.name)
 
 
         for valid in self.validators:
             val = valid(val,self.name)
 
@@ -295,14 +335,30 @@
         if isinstance(self.column.data_type.data_length,(int)):
             val = str(val)
             length = len(val)
             if length > self.column.data_type.data_length:
                 return False
         return True
 
+        # "request_id":{
+        #     "type":"string",
+        #     "description":"The encoded request id",
+        #     "example":encoded_id()
+        # },
+
+    def open_api_definition(self):
+        if self.column is not None and self._description is None:
+            self._description = self.column.comment
+        data = {
+            "type":self.data_type,
+            "description":self._description,
+            "example":self._example,
+        }
+        return data
+
     def open_api_data(self,loc:str="body")->dict:
         '''
             Generate a dictionary representation of this field that can be used with the open api library.
 
             ----------
 
             Arguments
@@ -320,33 +376,44 @@
             `created`: 04-24-2023 09:22:02
             `memberOf`: Field
             `version`: 1.0
             `method_name`: open_api_data.
             `throws`: ValueError - if the loc is not "body"/"path"
             * @xxx [04-24-2023 09:23:07]: documentation for open_api_data
         '''
+        if self._open_api_location is not None:
+            loc = self._open_api_location
         if loc not in _settings.control.open_api_param_locations:
             raise ValueError(f"{loc} is not a valid param location, expected: {','.join(_settings.control.open_api_param_locations)}")
+        if self.column is not None and self._description is None:
+            self._description = self.column.comment
 
         data = {
             "name": self.name,
             "description":self._description,
+            "example":self._example,
             "in": loc,
             "type": self.data_type,
             "required": self.required,
         }
         if self.required is False:
-            if self.default is _settings.types.no_default:
-                data['required'] = True
-            else:
+            if self.default != _settings.types.no_default:
                 data['default'] = self.default
+            # else:
+                # print(f"setting {self.name} required to True")
+                # data['required'] = True
 
         return data
 
 
+    @property
+    def should_ignore(self):
+        if self.value is None and self._ignore_null is True:
+            return True
+        return False
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} : {self.name}>"
```

### Comparing `colemen_volent-0.0.4/volent/Model.py` & `colemen_volent-0.0.5/volent/Model.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from volent.Column import Column as _column
 from volent.Relationship import Relationship as _relationship
 from volent.UniqueConstraint import UniqueConstraint as _uniqueConstraint
 from volent.mixins import OrderedClass,MySQLGeneratorMixin
 from volent.query.Insert import Insert as _insert
 from volent.query.Select import Select as _select
 from volent.query.Update import Update as _update
+from volent.query.Delete import Delete as _delete
 
 @dataclass
 # class Model(MySQLGeneratorMixin):
 class Model(MySQLGeneratorMixin,metaclass=OrderedClass):
     _is_root= False
     _name:str = None
     '''The name of this models table'''
@@ -65,15 +66,16 @@
 
 
         for k,v in kwargs.items():
             col = self.get_column(k)
             if col is not None:
                 if col.is_primary is True and v is None:
                     continue
-                col.value = v
+                if v != _t.no_default:
+                    col.value = v
         self._parent_models = []
         self._child_models = []
 
 
 
     def _get_attrs_from_parent(self):
         '''Used internally to apply the root model attributes to this instance.
@@ -247,15 +249,15 @@
         for col in self.columns:
             if col.name == name:
                 return col
 
         return None
 
     @property
-    def columns(self):
+    def columns(self)->Iterable[_t.column_type]:
         '''
             Get this Model's columns
 
             `default`:None
 
 
             Meta
@@ -524,14 +526,18 @@
         s = _select(self,columns=columns)
         return s
 
     def update(self,**columns)->_update:
         # print(f"columns: {columns}")
         s = _update(self,columns=columns)
         return s
+    def delete(self)->_delete:
+        # print(f"columns: {columns}")
+        s = _delete(self)
+        return s
 
 
     def add_parent_model(self,model:_t.model_type):
         '''
             Add a parent model to this model.
             
             This is for internal use do not arbitrarily add models here, they wont do anything.
```

### Comparing `colemen_volent-0.0.4/volent/NestedField.py` & `colemen_volent-0.0.5/volent/NestedField.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/Relationship.py` & `colemen_volent-0.0.5/volent/Relationship.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/Schema.py` & `colemen_volent-0.0.5/volent/Schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -278,15 +278,15 @@
 
     def __validate_dict(self,data:dict):
         '''
             Execute the validation process on all fields associated to this schema
 
             This is used to validate a dictionary as opposed to __validate which will
             validate the values that are assigned to columns.
-            
+
             So this method has a little setup before it can validate which includes
             it associating dictionary keys to matching fields.
 
 
             ----------
 
             Meta
@@ -294,34 +294,54 @@
             `author`: Colemen Atwood
             `created`: 04-21-2023 07:43:15
             `memberOf`: Schema
             `version`: 1.0
             `method_name`: __validate
             * @xxx [04-21-2023 07:44:01]: documentation for __validate
         '''
+        # @Mstep [] convert all keys to snake case for matching.
         data = c.obj.keys_to_snake_case(data)
+        # print(f"data:{data}")
+        # @Mstep [LOOP] iterate all fields associated to this schema
         for f in self.fields:
+            # @Mstep [] set "value" to be no_default
             value = _settings.types.no_default
+            # @Mstep [IF] if field name is not in the data dict
             if f.name not in data:
+                # @Mstep [IF] if the field is required.
                 if f.required is True:
+                    # @Mstep [] raise a validation error.
                     raise ValidationError(f"{f.name} is required.")
+                # @Mstep [IF] if the field name converted to snake case is in the data dict.
                 elif c.string.to_snake_case(f.name) in data:
+                    # @Mstep [] update "value" to be the data dict's value.
                     value = data[c.string.to_snake_case(f.name)]
+                # @Mstep [ELSE] the field was not provided
                 else:
+                    # @Mstep [] set the field._ignore_null to True, so this field will not attempt validation.
+                    f._ignore_null = True
                     continue
+            # @Mstep [ELSE] the field was found in the data dictionary.
             else:
+                # @Mstep [] update "value" to be the data dict's value.
                 value = data[f.name]
 
+            # @Mstep [IF] if "value" is NOT no_default
             if value is not _settings.types.no_default:
-            # if value is not None:
+                # @Mstep [] set the field's value to the "value"'s value.
                 f.value = value
 
+        # @Mstep [] Execute any custom validation methods on this schema
         self.__call_custom_validations()
+        # @Mstep [LOOP] iterate the fields associated to this schema
         for f in self.fields:
-            f.validate()
+            # @Mstep [IF] if the field should NOT be skipped
+            if f.should_ignore is False:
+                # @Mstep [] have the field self-validate
+                f.validate()
 
     def get_field(self,name:str)->_t.field_type:
         '''
             Retrieve a field instance from this schema by its name.
 
             ----------
 
@@ -379,14 +399,21 @@
                 continue
             field = self.get_field(col.name)
             if field is None:
                 continue
 
             col.column_value = data[col]
 
+
+    def open_api_definition(self):
+        value = {}
+        for f in self.fields:
+            value[f.name] = f.open_api_definition()
+        return value
+
     def open_api_data(self,loc:str="body")->Iterable[dict]:
         '''
             Get this Schema's open_api_data
 
             returns a list of dictionaries each representing a field, the dictionaries can
             be used with the open api library for documentation.
 
@@ -416,61 +443,94 @@
         value = []
         if loc not in _settings.control.open_api_param_locations:
             raise ValueError(f"{loc} is not a valid param location, expected: {','.join(_settings.control.open_api_param_locations)}")
         for f in self.fields:
             value.append(f.open_api_data(loc))
         return value
 
-    def dump(self,model:_t.model_type=None,many=False)->dict:
+    def dump(self,model:_t.model_type=None,many=False,ignore_unprovided=False)->dict:
         '''Dump the contents of the model(s) using the fields to filter.'''
 
         if isinstance(model,(dict)):
-            data = self._correlate_to_dict(model)
+            print(f"dictionary provided for dumping.")
+            data = self._correlate_to_dict(model,ignore_unprovided)
             self.__validate_dict(model)
             out_data = {}
             for f in self.fields:
                 if f.name in data:
-                    if hasattr(f.data_type,"serialized_value"):
-                        v = f.data_type.serialized_value(data[f.name])
-                        # print(f"v: {v}")
+                    # print(f"f.value:{f.value}")
+                    if hasattr(f.data_type_instance,"serializer"):
+                        v = f.data_type_instance.serializer(data[f.name],f.name)
                         out_data[f.name] = v
                         continue
-                    out_data[f.name] = data[f.name]
+                    # if hasattr(f.data_type_instance,"serialized_value"):
+                    #     v = f.data_type_instance.serialized_value(data[f.name])
+                    #     print(f"{f.name}:: {v}")
+                    #     out_data[f.name] = v
+                    #     continue
+                    out_data[f.name] = f.value
+                    # out_data[f.name] = data[f.name]
             if many:
                 out_data = c.arr.force_list(out_data)
             return out_data
 
 
 
 
-
+        # print(f"model: {model}")
         if isinstance(model,(list)):
+            # print(f"a list was provided for dumping.")
             result = []
             from volent.Model import Model as _model
             for mdl in model:
                 if isinstance(mdl,_model) is False:
                     c.con.log(f"The mdl is not an instance of model:{mdl}","magenta")
 
                 # mdl = model
                 self.model = mdl
                 self._correlate_to_columns()
                 self.__validate()
                 data = {}
                 for f in self.fields:
-                    data[f.name] = f.value
+                    if hasattr(f.data_type_instance,"serializer"):
+                        v = f.data_type_instance.serializer(f.value,f.name)
+                        data[f.name] = v
+                        continue
+                    if hasattr(f.data_type_instance,"serialized_value"):
+                        v = f.data_type_instance.serialized_value(f.value)
+                        # print(f"{f.name}:: {v}")
+                        # print(f"v: {v}")
+                        data[f.name] = v
+                        continue
+                    v = f.value
+                    data[f.name] = v
+                    # data[f.name] = f.value
                 result.append(data)
             return result
+
+
         if model is not None:
             self.model = model
         # self.model = model
         self._correlate_to_columns()
         self.__validate()
         data = {}
         for f in self.fields:
-            data[f.name] = f.value
+            # print(f"{f.name}:")
+            if f.should_ignore is False:
+                if hasattr(f.data_type_instance,"serializer"):
+                    v = f.data_type_instance.serializer(f.value,f.name)
+                    data[f.name] = v
+                    continue
+                if hasattr(f.data_type_instance,"serialized_value"):
+                    v = f.data_type_instance.serialized_value(f.value)
+                    # print(f"{f.name}:: {v}")
+                    data[f.name] = v
+                    continue
+                data[f.name] = f.value
         if many:
             data = c.arr.force_list(data)
         return data
 
     def new(self)->_t.schema_type:
         '''
             Validate this schema's data and submit it to the model's table in the databse.
@@ -490,21 +550,22 @@
             * @xxx [04-21-2023 07:51:43]: documentation for new
         '''
         # @Mstep [] correlate the fields to their columns in the model.
         self._correlate_to_columns()
         # @Mstep [] validate the schema fields.
         self.__validate()
 
-        data = {}
-        # @Mstep [LOOP] iterate this schema's fields
-        for f in self.fields:
-            # @Mstep [IF] if the field is NOT dump_only
-            if f.dump_only is False:
-                # @Mstep [] add the field to the data dictionary.
-                data[f.name] = f.value
+        # data = {}
+        # # @Mstep [LOOP] iterate this schema's fields
+        # for f in self.fields:
+        #     # @Mstep [IF] if the field is NOT dump_only
+        #     if f.dump_only is False:
+        #         # @Mstep [] add the field to the data dictionary.
+        #         data[f.name] = f.value
+
         # @Mstep [] execute the insert on the model.
         self.model.insert(self)
         # @Mstep [RETURN] return this schema instance.
         return self
 
     def update(self)->_t.schema_type:
         self._correlate_to_columns()
@@ -557,24 +618,28 @@
             props = dir(self)
             # # @Mstep [] find the props that exist on this instance and not on the base.
             value = c.arr.find_list_diff(props,df_props)
             self.__unique_prop_keys = value
 
         return value
 
-    def _correlate_to_dict(self,data:dict):
+    def _correlate_to_dict(self,data:dict,ignore_unprovided=False):
         out_data = {}
         data = c.obj.keys_to_snake_case(data)
         # print(f"_correlate_to_dict: data:{data}")
         for f in self.fields:
             # snake_field = c.string.to_snake_case(f.name)
             # print(f"_correlate_to_dict: snake_field:{snake_field}")
             if f.name in data:
                 out_data[f.name] = data[f.name]
                 continue
+            if ignore_unprovided is False:
+                if f.default != _t.no_default:
+                    out_data[f.name] = f.value
+                
             # if snake_field in data:
             #     print(f"snake case field match: {c.string.to_snake_case(f.name)}")
             #     out_data[c.string.to_snake_case(f.name)] = data[c.string.to_snake_case(f.name)]
             #     continue
 
         return out_data
```

### Comparing `colemen_volent-0.0.4/volent/UniqueConstraint.py` & `colemen_volent-0.0.5/volent/UniqueConstraint.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/Volent.py` & `colemen_volent-0.0.5/volent/Volent.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,17 +42,14 @@
 
         self.relationship_names:Iterable[str] = []
         '''A list of all registered relationship names'''
 
         self.columns:Iterable[_t.column_type] = []
         '''A list of all registered column instances'''
 
-
-
-
         self._databases = []
         _settings.globe.Volent = self
         super().__init__()
         # self.set_defaults()
 
     # def set_defaults(self):
     #     self.settings = c.file.import_project_settings("volent.settings.json")
```

### Comparing `colemen_volent-0.0.4/volent/data_types/BigInt.py` & `colemen_volent-0.0.5/volent/data_types/Decimal.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,26 +7,52 @@
 from typing import Iterable
 import colemen_utils as c
 import volent.settings as _settings
 import volent.settings.types as _t
 from volent.data_types.TypeBase import TypeBase as _type_base
 
 @dataclass
-class BigInt(_type_base):
+class Decimal(_type_base):
 
 
-
-
-    def __init__(self,data_length:int=None) -> None:
+    def __init__(self,data_length:int=10,decimal:int=0) -> None:
         super().__init__(data_length)
         self.min_data_length = 0
-        self.max_data_length = 65535
-        self.sql_type_name = "BIGINT"
-        self.python_data_type = (int)
-        self.open_api_data_type = "integer"
-
-        self._validate_data_length(data_length)
+        self.max_data_length = 65
+        self.sql_type_name = "Decimal"
+        self.python_data_type = (float)
+        self.open_api_data_type = "float"
+
+        self._validate_data_length(data_length,_settings.control.varchar_default_length)
+        if decimal > 30 or decimal < 0:
+            raise ValueError("The decimal for a Decimal must range from 0 to 10")
+
+        self.decimal = decimal
+
+
+    @property
+    def sql(self):
+        '''
+            Get this Decimals SQL data type
+
+            Decimal(10,8)
+
+            `default`:None
+
+
+            Meta
+            ----------
+            `@author`: Colemen Atwood
+            `@created`: 03-24-2023 04:23:20
+            `@memberOf`: String
+            `@property`: mysql
+        '''
+        if _settings.globe.flavor == "mysql":
+            value = f"{self.flavored_name}({self.data_length},{self.decimal})"
+        if _settings.globe.flavor == "sqlite":
+            value = f"{self.flavored_name}({self.data_length},{self.decimal})"
+        return value
 
 
 
     def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} : {self.data_length}>"
+        return f"<{self.__class__.__name__} : {self.data_length} {self.decimal}>"
```

### Comparing `colemen_volent-0.0.4/volent/data_types/Bool.py` & `colemen_volent-0.0.5/volent/data_types/TinyInt.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 from typing import Iterable
 import colemen_utils as c
 import volent.settings as _settings
 import volent.settings.types as _t
 from volent.data_types.TypeBase import TypeBase as _type_base
 
 @dataclass
-class Bool(_type_base):
+class TinyInt(_type_base):
 
+    def __init__(self,data_length:int=None) -> None:
+        super().__init__(data_length)
+        self.min_data_length = 0
+        self.max_data_length = 255
+        self.sql_type_name = "TINYINT"
+        self.python_data_type = (int)
+        self.open_api_data_type = "integer"
 
-    def __init__(self) -> None:
-        super().__init__()
-        self.sql_type_name = "BOOLEAN"
-        self.python_data_type = (bool)
-        self.open_api_data_type = "boolean"
+        self._validate_data_length(data_length,_settings.control.varchar_default_length)
 
 
     def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} >"
+        return f"<{self.__class__.__name__} : {self.data_length}>"
```

### Comparing `colemen_volent-0.0.4/volent/data_types/EncodedPrimary.py` & `colemen_volent-0.0.5/volent/data_types/String.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,45 +4,56 @@
 # pylint: disable=unused-import
 
 from dataclasses import dataclass
 from typing import Iterable
 import colemen_utils as c
 import volent.settings as _settings
 import volent.settings.types as _t
-from volent.exceptions import ValidationError
 from volent.data_types.TypeBase import TypeBase as _type_base
 
-@dataclass
-class EncodedPrimary(_type_base):
-
 
+@dataclass
+class String(_type_base):
 
 
     def __init__(self,data_length:int=None) -> None:
         super().__init__(data_length)
         self.min_data_length = 0
         self.max_data_length = 65535
-        self.sql_type_name = "BIGINT"
-        self.python_data_type = (int,str)
-        self.open_api_data_type = "string"
+        self.sql_type_name = "VARCHAR"
+        self.python_data_type = (str)
 
-        self._validate_data_length(data_length)
+        self._validate_data_length(data_length,_settings.control.varchar_default_length)
 
+    @property
+    def mysql(self):
+        '''
+            Get this String's mysql
+
+            `default`:None
+
+
+            Meta
+            ----------
+            `@author`: Colemen Atwood
+            `@created`: 03-24-2023 04:23:20
+            `@memberOf`: String
+            `@property`: mysql
+        '''
+        value = f"varchar({self.data_length})"
+        return value
 
-    def serialized_value(self,value):
+    def _serialize(self,value):
         if isinstance(value,(str)):
             return value
-        return c.string.string_encode_int(value)
 
-    def deserialized_value(self,value):
-        if isinstance(value,(int)):
-            # return value
-            raise ValidationError(f"Failed to decode the id {value}")
-        
-        val = c.string.string_decode_int(value)
-        if isinstance(val,(int)):
-            return val
-        raise ValidationError(f"Failed to decode the id {value}")
+        if isinstance(value,(int,float)):
+            return str(value)
+
+        if isinstance(value,(bool)):
+            return c.types.bool_to_string(value)
 
+    def _deserialize(self,value):
+        return value
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} : {self.data_length}>"
```

### Comparing `colemen_volent-0.0.4/volent/data_types/Integer.py` & `colemen_volent-0.0.5/volent/data_types/Integer.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,29 +24,38 @@
 
         self._validate_data_length(data_length)
 
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} : {self.data_length}>"
 
-    def serialized_value(self,value):
+    def serialized_value(self,value,field_name:str=None):
         if isinstance(value,(int)):
             return value
 
+        if value is None or value == _t.undefined:
+            return value
+
         if isinstance(value,(str)):
             if c.valid.numeric_only(value):
                 value = int(value)
         if isinstance(value,(float)):
             value = int(value)
 
         if isinstance(value,(int)) is False:
-            raise ValidationError(f"Failed to serialize {value} to integer.")
+            raise ValidationError(f"Failed to serialize {value} to integer.",field_name)
 
         return value
 
-    def deserialized_value(self,value):
+    def deserialized_value(self,value,field_name:str=None):
         if isinstance(value,(int)):
             return value
-        if value is None:
+
+        if value is None or value == _t.undefined:
             return value
+
+        if isinstance(value,(str)):
+            if c.valid.numeric_only(value):
+                return int(value)
+        
         if isinstance(value,(int)) is False:
-            raise ValidationError(f"Failed to deserialize {value} to integer.")
+            raise ValidationError(f"Failed to deserialize {value} to integer.",field_name)
```

### Comparing `colemen_volent-0.0.4/volent/data_types/TypeBase.py` & `colemen_volent-0.0.5/volent/data_types/TypeBase.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/mixins/DatabaseConnection.py` & `colemen_volent-0.0.5/volent/mixins/DatabaseConnection.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/mixins/EntityName.py` & `colemen_volent-0.0.5/volent/mixins/EntityName.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/mixins/MySQLGeneratorMixin.py` & `colemen_volent-0.0.5/volent/mixins/MySQLGeneratorMixin.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/mixins/OrderedClass.py` & `colemen_volent-0.0.5/volent/mixins/OrderedClass.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/query/Query.py` & `colemen_volent-0.0.5/volent/query/Query.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # pylint: disable=line-too-long
 # pylint: disable=unused-import
 
 
 from dataclasses import dataclass
 import re
 from typing import Iterable,OrderedDict, Union
-
+from datetime import datetime
+from datetime import timezone
 
 import colemen_utils as c
 
 
 import volent.settings.types as _t
 import volent.settings as _settings
 from volent.Field import Field as _field
@@ -86,17 +87,36 @@
                         self.add_select(name,alias)
                     if len(col) == 1:
                         col = col[0]
                 if isinstance(col,(str)):
                     self.add_select(col)
 
         if isinstance(update_columns,(dict)):
+            mt_col = self.model.get_column("modified_timestamp")
+            if mt_col is not None:
+                self.add_update("modified_timestamp",round(datetime.now(tz=timezone.utc).timestamp()))
+
+
             for k,v in update_columns.items():
+                col = self.model.get_column(k)
+                # @Mstep [IF] if the column is the primary key of the table
+                if col.is_primary is True:
+                    # @Mstep [] skip
+                    continue
+                # @Mstep [] add a new update clause to this query.
                 self.add_update(k,v)
 
+            for col in self.model.columns:
+                # @Mstep [IF] if the column has an "on_update" value set.
+                if col.on_update != _t.undefined:
+                    # @Mstep [IF] if the column is not already being updated.
+                    if col.name not in self._updates:
+                        # @Mstep [] add a new update clause to this query.
+                        self.add_update(col.name,col.on_update)
+
     def filter_dict_by_columns(self,data:dict)->dict:
         output = {}
         for k,v in data.items():
             col = self.model.get_column(k)
             if col is not None:
                 if v is None and col.nullable is False:
                     continue
@@ -166,40 +186,50 @@
             `@property`: where_string
         '''
         value = self._wheres
         # self._params = {}
         if len(self._wheres) > 0:
             wheres = []
             for where in self._wheres:
-                if where['comparison'] in ["between"]:
-                    min_key =f"{where['column_name']}_minimum"
-                    max_key =f"{where['column_name']}_maximum"
+                wcol = where['column_name']
+                wcomp = where['comparison']
+                wval = str(where['value'])
+
+                if c.string.to_snake_case(wcomp) in ["between"]:
+                    min_key =f"{wcol}_minimum"
+                    max_key =f"{wcol}_maximum"
 
-                    single_where = f"{where['column_name']} {where['comparison'].upper()} :{min_key} AND :{max_key}"
+                    single_where = f"{wcol} {where['comparison'].upper()} :{min_key} AND :{max_key}"
                     self._params[min_key] = where['value']
                     self._params[max_key] = where['max_value']
 
 
-                elif where['comparison'] in ["in","not in"]:
+                elif c.string.to_snake_case(wcomp) in ["in","not_in"]:
                     in_list = []
                     for idx,val in enumerate(where['value']):
                         key = f"{where['column_name']}_{idx}"
                         self._params[key] = val
                         in_list.append(f":{key}")
                     in_list_string = ', '.join(in_list)
                     single_where = f"{where['column_name']} {where['comparison'].upper()} ({in_list_string})"
 
 
-
-                elif where['comparison'] in ["is","is not"]:
-                    single_where = f"{where['column_name']} {where['comparison'].upper()} {str(where['value'])}"
+                # @Mstep [IF] if comparison matches [is,is not]
+                elif c.string.to_snake_case(wcomp) in ["is","is_not"]:
+                    # @Mstep [] generate the where string without applying a parameterized value.
+                    # This can cause issues with "IS NULL" type clauses, because those cannot be parameterized
+                    # single_where = f"{where['column_name']} {where['comparison'].upper()} {str(where['value'])}"
+                    single_where = f"{wcol} {wcomp} {wval}"
+                    # if wval.upper() == "NULL":
+                        # single_where = f"{wcol} {wcomp} {wval}"
                     # params[where['column_name']] = where['value']
                 else:
                     single_where = f"{where['column_name']} {where['comparison']} :{where['column_name']}"
                     self._params[where['column_name']] = where['value']
+
                 wheres.append(single_where)
             wheres = ' AND '.join(wheres)
             value = f" WHERE {wheres}"
         else:
             value = ""
         return value
 
@@ -295,14 +325,16 @@
         self.add_where(column_name,value,comparison)
 
         return self
 
 
 
 
+
+
 def format_null(value):
     if value is None:
         return "NULL"
     return value
 
 
 
@@ -411,18 +443,22 @@
         `version`: 1.0
         `method_name`: _format_query_params
         * @xxx [12-09-2022 10:43:23]: documentation for _format_query_params
     '''
     if isinstance(args,(dict)) is False:
         return sql
     # args = sorted(args.items(), key=lambda x: x[1], reverse=True)
+    # @Mstep [] get a list of the argument keys
     arg_keys = list(args.keys())
+    # @Mstep [] sort the keys from largest to smallest.
     arg_keys.sort(key=len, reverse=True)
+    # @Mstep [] iterate the argument keys.
     for k in arg_keys:
     # for k,v in args.items():
+        # @Mstep [] replace the key with the parameterized version.
         sql = re.sub(fr'[$:]{k}',f"%({k})s",sql)
 
     # matches = re.findall(r'[$:]([a-z_0-9]*)',sql,re.IGNORECASE)
     # if isinstance(matches,(list)):
     #     for match in matches:
     #         if match in args:
     #             sql = sql.replace(f"${match}",f"%({match})s")
```

### Comparing `colemen_volent-0.0.4/volent/query/Select.py` & `colemen_volent-0.0.5/volent/query/Select.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import volent.settings.types as _t
 import volent.settings as _settings
 from volent.Field import Field as _field
 # from volent.Relationship import Relationship as _relationship
 # from volent.UniqueConstraint import UniqueConstraint as _uniqueConstraint
 from volent.query.Query import Query
 from volent.query.WhereMixin import WhereMixin
-
+from mysql.connector.errors import OperationalError,InterfaceError
 
 @dataclass
 class Select(Query,WhereMixin):
     def __init__(self,model:_t.model_type,columns=None,limit:int=100,offset:int=0) -> None:
         self._params = {}
         self._selects = []
         self._joins = []
@@ -126,35 +126,39 @@
         value = self._format_query_params(value,self._params)
         # print(f"value: {value}")
         # print(f"self._params: {self._params}")
         return value,self._params
 
     def execute(self,return_models=True)->Union[bool,dict,int,_t.model_type]:
     # def execute(self)->Union[bool,dict,int]:
-
+        # _mysql_connector.MySQLInterfaceError: Lost connection to MySQL server during query
         sql,args= self.query
 
         if sql is False:
             return False
 
         # print(f"sql:{sql}")
         # print(f"args:{args}")
-
-        # @Mstep [] execute the insert query.
-        result = self.database.run_select(sql,args)
-        if return_models:
-            models = []
-            for r in result:
-                mdl = self.model.__class__(**r)
-                mdl.__doc__ = self.model.__doc__
-                mdl._name = self.model.name
-                mdl._database_name = self.model._database_name
-                mdl._database = self.model._database
-                models.append(mdl)
-            return models
+        try:
+            # @Mstep [] execute the insert query.
+            result = self.database.run_select(sql,args)
+            if return_models:
+                models = []
+                for r in result:
+                    mdl = self.model.__class__(**r)
+                    mdl.__doc__ = self.model.__doc__
+                    mdl._name = self.model.name
+                    mdl._database_name = self.model._database_name
+                    mdl._database = self.model._database
+                    models.append(mdl)
+                return models
+        except OperationalError as e:
+            c.con.log(e,"red")
+        except InterfaceError as e:
+            c.con.log(e,"red")
         return result
 
     def count(self)->_t.query_type:
         self._count = True
         return self
 
     def average(self)->_t.query_type:
```

### Comparing `colemen_volent-0.0.4/volent/query/Update.py` & `colemen_volent-0.0.5/volent/query/Update.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,21 +86,21 @@
 
         if sql is False:
             return False
 
         # print(f"sql:{sql}")
         # print(f"args:{args}")
 
-        # @Mstep [] execute the insert query.
+        # @Mstep [] execute the update query.
         result = self.database.run(sql,args)
         data = self.model.select().add_where_from_wheres(self._wheres).execute(return_models=False)
         data = data[0]
         for k,v in data.items():
             col = self.model.get_column(k)
-            col._column_value = v
+            col.value = v
             self.model._saved = True
         return data
         models = []
         for r in result:
             mdl = self.model.__class__(**r)
             mdl.__doc__ = self.model.__doc__
             mdl._name = self.model.name
```

### Comparing `colemen_volent-0.0.4/volent/settings/control.py` & `colemen_volent-0.0.5/volent/settings/control.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/settings/types.py` & `colemen_volent-0.0.5/volent/settings/types.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/tests/schema_dict_test.py` & `colemen_volent-0.0.5/volent/tests/schema_dict_test.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/tests/validators_test.py` & `colemen_volent-0.0.5/volent/tests/validators_test.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/CreditCardNumber.py` & `colemen_volent-0.0.5/volent/validate/CreditCardNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/Email.py` & `colemen_volent-0.0.5/volent/validate/Email.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/Equal.py` & `colemen_volent-0.0.5/volent/validate/Equal.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/FutureUnixDate.py` & `colemen_volent-0.0.5/volent/validate/FutureUnixDate.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/IpAddress.py` & `colemen_volent-0.0.5/volent/validate/IpAddress.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,16 @@
 
 
     def _repr_args(self) -> str:
         return f"ipv4={self.ipv4!r},ipv6={self.ipv6!r}"
 
     def __call__(self,value:_T,field_name:str=None)->_T:
         self.field_name = field_name
+        if isinstance(value,(str,bytes)) is False:
+            return value
         if self.ipv4 is True:
             if re.search(self.ipv4_regex,value):
             # if self.ipv4_regex.match(value) is True:
                 return value
 
         if self.ipv6 is True:
             if re.search(self.ipv6_regex,value):
```

### Comparing `colemen_volent-0.0.4/volent/validate/Length.py` & `colemen_volent-0.0.5/volent/validate/Length.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/NoneOf.py` & `colemen_volent-0.0.5/volent/validate/NoneOf.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/OneOf.py` & `colemen_volent-0.0.5/volent/validate/OneOf.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         ):
 
         self.choices = choices
         self.choices_str = ', '.join(str(choice) for choice in self.choices)
 
     def _format_error(self, value: Any, message: str) -> str:
         if self.field_name is not None:
-            message = f"{self.field_name} was not in {self.choices}"
+            message = f"{self.field_name} [{value}] was not in {self.choices}"
         return message.format(
             input=value, choices=self.choices_str
         )
 
 
     def _repr_args(self) -> str:
         return f"min={self.min!r}, max={self.max!r}, equal={self.equal!r}"
```

### Comparing `colemen_volent-0.0.4/volent/validate/PastUnixDate.py` & `colemen_volent-0.0.5/volent/validate/PastUnixDate.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/PhoneNumber.py` & `colemen_volent-0.0.5/volent/validate/PhoneNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/Range.py` & `colemen_volent-0.0.5/volent/validate/Range.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,27 +120,32 @@
 
     def _repr_args(self) -> str:
         return f"min={self.min!r},max={self.max!r},min_inclusive={self.min_inclusive!r},max_inclusive={self.max_inclusive!r}"
 
 
     def __call__(self,value:_T,field_name:str=None)->_T:
         self.field_name = field_name
+        if value is None:
+            return value
+        try:
+            if self.min is not None and (
+                value < self.min if self.min_inclusive else value <= self.min
+            ):
+                message = self.message_min if self.max is None else self.message_all
+                raise ValidationError(self._format_error(value, message))
+
+            if self.max is not None and (
+                value > self.max if self.max_inclusive else value >= self.max
+            ):
+                message = self.message_max if self.min is None else self.message_all
+                raise ValidationError(self._format_error(value, message))
+        except TypeError as e:
+            raise ValidationError(f"{field_name} - Cannot compare {type(value)} {e}")
 
-        if self.min is not None and (
-            value < self.min if self.min_inclusive else value <= self.min
-        ):
-            message = self.message_min if self.max is None else self.message_all
-            raise ValidationError(self._format_error(value, message))
-
-        if self.max is not None and (
-            value > self.max if self.max_inclusive else value >= self.max
-        ):
-            message = self.message_max if self.min is None else self.message_all
-            raise ValidationError(self._format_error(value, message))
-
+            
         return value
 
         return value
 
 
 # class ContainsOnly(OneOf):
```

### Comparing `colemen_volent-0.0.4/volent/validate/Regex.py` & `colemen_volent-0.0.5/volent/validate/Regex.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/SocialSecurityNumber.py` & `colemen_volent-0.0.5/volent/validate/SocialSecurityNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/StrongPassword.py` & `colemen_volent-0.0.5/volent/validate/StrongPassword.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/Validator.py` & `colemen_volent-0.0.5/volent/validate/Validator.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.4/volent/validate/__init__.py` & `colemen_volent-0.0.5/volent/validate/__init__.py`

 * *Files identical despite different names*

