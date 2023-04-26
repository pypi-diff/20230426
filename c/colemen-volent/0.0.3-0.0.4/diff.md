# Comparing `tmp/colemen_volent-0.0.3.tar.gz` & `tmp/colemen_volent-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colemen_volent-0.0.3.tar", last modified: Mon Apr 24 13:21:43 2023, max compression
+gzip compressed data, was "colemen_volent-0.0.4.tar", last modified: Tue Apr 25 13:45:50 2023, max compression
```

## Comparing `colemen_volent-0.0.3.tar` & `colemen_volent-0.0.4.tar`

### file list

```diff
@@ -1,67 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.533555 colemen_volent-0.0.3/
--rw-rw-rw-   0        0        0      469 2023-04-24 13:21:43.533555 colemen_volent-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.165588 colemen_volent-0.0.3/colemen_volent.egg-info/
--rw-rw-rw-   0        0        0      469 2023-04-24 13:21:43.000000 colemen_volent-0.0.3/colemen_volent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1551 2023-04-24 13:21:43.000000 colemen_volent-0.0.3/colemen_volent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 13:21:43.000000 colemen_volent-0.0.3/colemen_volent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-24 13:21:43.000000 colemen_volent-0.0.3/colemen_volent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-24 13:21:43.000000 colemen_volent-0.0.3/colemen_volent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 13:21:43.534555 colemen_volent-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1328 2023-04-24 13:21:41.000000 colemen_volent-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.241587 colemen_volent-0.0.3/volent/
--rw-rw-rw-   0        0        0     5081 2023-04-18 20:41:28.000000 colemen_volent-0.0.3/volent/Column.py
--rw-rw-rw-   0        0        0     8710 2023-04-18 16:18:27.000000 colemen_volent-0.0.3/volent/Database.py
--rw-rw-rw-   0        0        0     6358 2023-04-21 16:52:42.000000 colemen_volent-0.0.3/volent/Field.py
--rw-rw-rw-   0        0        0    21054 2023-04-21 15:21:37.000000 colemen_volent-0.0.3/volent/Model.py
--rw-rw-rw-   0        0        0     7361 2023-04-21 13:52:04.000000 colemen_volent-0.0.3/volent/NestedField.py
--rw-rw-rw-   0        0        0     2855 2023-04-21 13:13:13.000000 colemen_volent-0.0.3/volent/Relationship.py
--rw-rw-rw-   0        0        0    16475 2023-04-21 16:50:12.000000 colemen_volent-0.0.3/volent/Schema.py
--rw-rw-rw-   0        0        0     1478 2023-04-14 12:21:18.000000 colemen_volent-0.0.3/volent/UniqueConstraint.py
--rw-rw-rw-   0        0        0    11968 2023-04-21 14:11:15.000000 colemen_volent-0.0.3/volent/Volent.py
--rw-rw-rw-   0        0        0       59 2023-04-11 20:23:11.000000 colemen_volent-0.0.3/volent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.306591 colemen_volent-0.0.3/volent/data_types/
--rw-rw-rw-   0        0        0      831 2023-04-11 19:39:38.000000 colemen_volent-0.0.3/volent/data_types/BigInt.py
--rw-rw-rw-   0        0        0      650 2023-04-11 19:39:38.000000 colemen_volent-0.0.3/volent/data_types/Bool.py
--rw-rw-rw-   0        0        0     1695 2023-04-11 19:39:38.000000 colemen_volent-0.0.3/volent/data_types/Decimal.py
--rw-rw-rw-   0        0        0     1408 2023-04-21 16:46:29.000000 colemen_volent-0.0.3/volent/data_types/EncodedPrimary.py
--rw-rw-rw-   0        0        0     1558 2023-04-21 16:38:30.000000 colemen_volent-0.0.3/volent/data_types/Integer.py
--rw-rw-rw-   0        0        0     1587 2023-04-11 19:39:38.000000 colemen_volent-0.0.3/volent/data_types/String.py
--rw-rw-rw-   0        0        0      864 2023-04-11 19:39:38.000000 colemen_volent-0.0.3/volent/data_types/TinyInt.py
--rw-rw-rw-   0        0        0     4404 2023-04-18 13:41:38.000000 colemen_volent-0.0.3/volent/data_types/TypeBase.py
--rw-rw-rw-   0        0        0      472 2023-04-21 16:39:20.000000 colemen_volent-0.0.3/volent/data_types/__init__.py
--rw-rw-rw-   0        0        0      873 2023-04-14 13:42:19.000000 colemen_volent-0.0.3/volent/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.336555 colemen_volent-0.0.3/volent/mixins/
--rw-rw-rw-   0        0        0    22731 2023-04-21 13:08:09.000000 colemen_volent-0.0.3/volent/mixins/DatabaseConnection.py
--rw-rw-rw-   0        0        0      729 2023-04-11 19:34:06.000000 colemen_volent-0.0.3/volent/mixins/EntityName.py
--rw-rw-rw-   0        0        0    17876 2023-04-18 14:57:37.000000 colemen_volent-0.0.3/volent/mixins/MySQLGeneratorMixin.py
--rw-rw-rw-   0        0        0     3686 2023-04-13 19:47:45.000000 colemen_volent-0.0.3/volent/mixins/OrderedClass.py
--rw-rw-rw-   0        0        0      346 2023-04-18 13:01:17.000000 colemen_volent-0.0.3/volent/mixins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.379558 colemen_volent-0.0.3/volent/query/
--rw-rw-rw-   0        0        0     2805 2023-04-18 20:17:21.000000 colemen_volent-0.0.3/volent/query/Insert.py
--rw-rw-rw-   0        0        0    13462 2023-04-21 15:47:20.000000 colemen_volent-0.0.3/volent/query/Query.py
--rw-rw-rw-   0        0        0     6815 2023-04-21 15:25:12.000000 colemen_volent-0.0.3/volent/query/Select.py
--rw-rw-rw-   0        0        0     4240 2023-04-21 15:25:16.000000 colemen_volent-0.0.3/volent/query/Update.py
--rw-rw-rw-   0        0        0     2620 2023-04-18 18:54:55.000000 colemen_volent-0.0.3/volent/query/WhereMixin.py
--rw-rw-rw-   0        0        0      155 2023-04-18 19:08:07.000000 colemen_volent-0.0.3/volent/query/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.400555 colemen_volent-0.0.3/volent/settings/
--rw-rw-rw-   0        0        0      129 2023-04-11 19:11:30.000000 colemen_volent-0.0.3/volent/settings/__init__.py
--rw-rw-rw-   0        0        0     6137 2023-04-11 20:08:44.000000 colemen_volent-0.0.3/volent/settings/control.py
--rw-rw-rw-   0        0        0      152 2023-04-11 20:12:31.000000 colemen_volent-0.0.3/volent/settings/globe.py
--rw-rw-rw-   0        0        0     2165 2023-04-18 18:20:43.000000 colemen_volent-0.0.3/volent/settings/types.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.531557 colemen_volent-0.0.3/volent/validate/
--rw-rw-rw-   0        0        0     2426 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/CreditCardNumber.py
--rw-rw-rw-   0        0        0     2866 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/Email.py
--rw-rw-rw-   0        0        0     1620 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/Equal.py
--rw-rw-rw-   0        0        0     1709 2023-04-21 16:10:49.000000 colemen_volent-0.0.3/volent/validate/FutureUnixDate.py
--rw-rw-rw-   0        0        0     3391 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/IpAddress.py
--rw-rw-rw-   0        0        0     2448 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/Length.py
--rw-rw-rw-   0        0        0     3658 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/NoneOf.py
--rw-rw-rw-   0        0        0     2761 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/OneOf.py
--rw-rw-rw-   0        0        0     1721 2023-04-21 16:10:42.000000 colemen_volent-0.0.3/volent/validate/PastUnixDate.py
--rw-rw-rw-   0        0        0     2237 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/PhoneNumber.py
--rw-rw-rw-   0        0        0     5757 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/Range.py
--rw-rw-rw-   0        0        0     2725 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/Regex.py
--rw-rw-rw-   0        0        0     2265 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/SocialSecurityNumber.py
--rw-rw-rw-   0        0        0     2490 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/StrongPassword.py
--rw-rw-rw-   0        0        0     1414 2023-04-14 13:25:54.000000 colemen_volent-0.0.3/volent/validate/Validator.py
--rw-rw-rw-   0        0        0      729 2023-04-21 16:11:07.000000 colemen_volent-0.0.3/volent/validate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.479682 colemen_volent-0.0.4/
+-rw-rw-rw-   0        0        0      469 2023-04-25 13:45:50.479682 colemen_volent-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.327681 colemen_volent-0.0.4/colemen_volent.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-04-25 13:45:50.000000 colemen_volent-0.0.4/colemen_volent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1685 2023-04-25 13:45:50.000000 colemen_volent-0.0.4/colemen_volent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:45:50.000000 colemen_volent-0.0.4/colemen_volent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-25 13:45:50.000000 colemen_volent-0.0.4/colemen_volent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-25 13:45:50.000000 colemen_volent-0.0.4/colemen_volent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 13:45:50.479682 colemen_volent-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2023-04-25 13:45:48.000000 colemen_volent-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.339682 colemen_volent-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     2077 2023-04-24 15:33:47.000000 colemen_volent-0.0.4/tests/schema_dict_test.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.361681 colemen_volent-0.0.4/volent/
+-rw-rw-rw-   0        0        0     5081 2023-04-18 20:41:28.000000 colemen_volent-0.0.4/volent/Column.py
+-rw-rw-rw-   0        0        0     8710 2023-04-18 16:18:27.000000 colemen_volent-0.0.4/volent/Database.py
+-rw-rw-rw-   0        0        0    10068 2023-04-25 13:43:31.000000 colemen_volent-0.0.4/volent/Field.py
+-rw-rw-rw-   0        0        0    21054 2023-04-21 15:21:37.000000 colemen_volent-0.0.4/volent/Model.py
+-rw-rw-rw-   0        0        0     7361 2023-04-21 13:52:04.000000 colemen_volent-0.0.4/volent/NestedField.py
+-rw-rw-rw-   0        0        0     2855 2023-04-21 13:13:13.000000 colemen_volent-0.0.4/volent/Relationship.py
+-rw-rw-rw-   0        0        0    19451 2023-04-24 17:08:49.000000 colemen_volent-0.0.4/volent/Schema.py
+-rw-rw-rw-   0        0        0     1478 2023-04-14 12:21:18.000000 colemen_volent-0.0.4/volent/UniqueConstraint.py
+-rw-rw-rw-   0        0        0    15413 2023-04-25 13:44:04.000000 colemen_volent-0.0.4/volent/Volent.py
+-rw-rw-rw-   0        0        0       59 2023-04-11 20:23:11.000000 colemen_volent-0.0.4/volent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.406681 colemen_volent-0.0.4/volent/data_types/
+-rw-rw-rw-   0        0        0      876 2023-04-24 14:12:42.000000 colemen_volent-0.0.4/volent/data_types/BigInt.py
+-rw-rw-rw-   0        0        0      695 2023-04-24 14:13:18.000000 colemen_volent-0.0.4/volent/data_types/Bool.py
+-rw-rw-rw-   0        0        0     1738 2023-04-24 14:13:06.000000 colemen_volent-0.0.4/volent/data_types/Decimal.py
+-rw-rw-rw-   0        0        0     1452 2023-04-24 14:12:30.000000 colemen_volent-0.0.4/volent/data_types/EncodedPrimary.py
+-rw-rw-rw-   0        0        0     1656 2023-04-24 17:13:25.000000 colemen_volent-0.0.4/volent/data_types/Integer.py
+-rw-rw-rw-   0        0        0     1587 2023-04-11 19:39:38.000000 colemen_volent-0.0.4/volent/data_types/String.py
+-rw-rw-rw-   0        0        0      909 2023-04-24 14:13:20.000000 colemen_volent-0.0.4/volent/data_types/TinyInt.py
+-rw-rw-rw-   0        0        0     4404 2023-04-18 13:41:38.000000 colemen_volent-0.0.4/volent/data_types/TypeBase.py
+-rw-rw-rw-   0        0        0      472 2023-04-21 16:39:20.000000 colemen_volent-0.0.4/volent/data_types/__init__.py
+-rw-rw-rw-   0        0        0      873 2023-04-14 13:42:19.000000 colemen_volent-0.0.4/volent/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.417682 colemen_volent-0.0.4/volent/mixins/
+-rw-rw-rw-   0        0        0    22897 2023-04-25 13:42:18.000000 colemen_volent-0.0.4/volent/mixins/DatabaseConnection.py
+-rw-rw-rw-   0        0        0      729 2023-04-11 19:34:06.000000 colemen_volent-0.0.4/volent/mixins/EntityName.py
+-rw-rw-rw-   0        0        0    17876 2023-04-18 14:57:37.000000 colemen_volent-0.0.4/volent/mixins/MySQLGeneratorMixin.py
+-rw-rw-rw-   0        0        0     3686 2023-04-13 19:47:45.000000 colemen_volent-0.0.4/volent/mixins/OrderedClass.py
+-rw-rw-rw-   0        0        0      346 2023-04-18 13:01:17.000000 colemen_volent-0.0.4/volent/mixins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.438681 colemen_volent-0.0.4/volent/query/
+-rw-rw-rw-   0        0        0     2805 2023-04-18 20:17:21.000000 colemen_volent-0.0.4/volent/query/Insert.py
+-rw-rw-rw-   0        0        0    13462 2023-04-21 15:47:20.000000 colemen_volent-0.0.4/volent/query/Query.py
+-rw-rw-rw-   0        0        0     6815 2023-04-21 15:25:12.000000 colemen_volent-0.0.4/volent/query/Select.py
+-rw-rw-rw-   0        0        0     4240 2023-04-21 15:25:16.000000 colemen_volent-0.0.4/volent/query/Update.py
+-rw-rw-rw-   0        0        0     2620 2023-04-18 18:54:55.000000 colemen_volent-0.0.4/volent/query/WhereMixin.py
+-rw-rw-rw-   0        0        0      155 2023-04-18 19:08:07.000000 colemen_volent-0.0.4/volent/query/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.442684 colemen_volent-0.0.4/volent/settings/
+-rw-rw-rw-   0        0        0      129 2023-04-11 19:11:30.000000 colemen_volent-0.0.4/volent/settings/__init__.py
+-rw-rw-rw-   0        0        0     6183 2023-04-24 14:05:40.000000 colemen_volent-0.0.4/volent/settings/control.py
+-rw-rw-rw-   0        0        0      152 2023-04-11 20:12:31.000000 colemen_volent-0.0.4/volent/settings/globe.py
+-rw-rw-rw-   0        0        0     2165 2023-04-18 18:20:43.000000 colemen_volent-0.0.4/volent/settings/types.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.460681 colemen_volent-0.0.4/volent/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.0.4/volent/tests/__init__.py
+-rw-rw-rw-   0        0        0     4222 2023-04-24 17:14:04.000000 colemen_volent-0.0.4/volent/tests/schema_dict_test.py
+-rw-rw-rw-   0        0        0     8452 2023-04-24 17:01:23.000000 colemen_volent-0.0.4/volent/tests/validators_test.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:45:50.477681 colemen_volent-0.0.4/volent/validate/
+-rw-rw-rw-   0        0        0     3075 2023-04-24 16:59:56.000000 colemen_volent-0.0.4/volent/validate/CreditCardNumber.py
+-rw-rw-rw-   0        0        0     2866 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/Email.py
+-rw-rw-rw-   0        0        0     1620 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/Equal.py
+-rw-rw-rw-   0        0        0     1709 2023-04-21 16:10:49.000000 colemen_volent-0.0.4/volent/validate/FutureUnixDate.py
+-rw-rw-rw-   0        0        0     3915 2023-04-24 16:09:19.000000 colemen_volent-0.0.4/volent/validate/IpAddress.py
+-rw-rw-rw-   0        0        0     2448 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/Length.py
+-rw-rw-rw-   0        0        0     3658 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/NoneOf.py
+-rw-rw-rw-   0        0        0     2761 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/OneOf.py
+-rw-rw-rw-   0        0        0     1721 2023-04-21 16:10:42.000000 colemen_volent-0.0.4/volent/validate/PastUnixDate.py
+-rw-rw-rw-   0        0        0     2394 2023-04-24 16:42:48.000000 colemen_volent-0.0.4/volent/validate/PhoneNumber.py
+-rw-rw-rw-   0        0        0     5757 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/Range.py
+-rw-rw-rw-   0        0        0     2725 2023-04-24 17:08:33.000000 colemen_volent-0.0.4/volent/validate/Regex.py
+-rw-rw-rw-   0        0        0     2265 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/SocialSecurityNumber.py
+-rw-rw-rw-   0        0        0     2490 2023-04-14 13:23:23.000000 colemen_volent-0.0.4/volent/validate/StrongPassword.py
+-rw-rw-rw-   0        0        0     1414 2023-04-14 13:25:54.000000 colemen_volent-0.0.4/volent/validate/Validator.py
+-rw-rw-rw-   0        0        0      770 2023-04-24 16:48:21.000000 colemen_volent-0.0.4/volent/validate/__init__.py
```

### Comparing `colemen_volent-0.0.3/colemen_volent.egg-info/SOURCES.txt` & `colemen_volent-0.0.4/colemen_volent.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 setup.py
 colemen_volent.egg-info/PKG-INFO
 colemen_volent.egg-info/SOURCES.txt
 colemen_volent.egg-info/dependency_links.txt
 colemen_volent.egg-info/requires.txt
 colemen_volent.egg-info/top_level.txt
+tests/__init__.py
+tests/schema_dict_test.py
 volent/Column.py
 volent/Database.py
 volent/Field.py
 volent/Model.py
 volent/NestedField.py
 volent/Relationship.py
 volent/Schema.py
@@ -35,14 +37,17 @@
 volent/query/Update.py
 volent/query/WhereMixin.py
 volent/query/__init__.py
 volent/settings/__init__.py
 volent/settings/control.py
 volent/settings/globe.py
 volent/settings/types.py
+volent/tests/__init__.py
+volent/tests/schema_dict_test.py
+volent/tests/validators_test.py
 volent/validate/CreditCardNumber.py
 volent/validate/Email.py
 volent/validate/Equal.py
 volent/validate/FutureUnixDate.py
 volent/validate/IpAddress.py
 volent/validate/Length.py
 volent/validate/NoneOf.py
```

### Comparing `colemen_volent-0.0.3/setup.py` & `colemen_volent-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from glob import glob
 from setuptools import setup, find_packages
 import colemen_utilities.build_utils.general as _gen
 
 
-VERSION='0.0.3'
+VERSION='0.0.4'
 DESCRIPTION = 'volent'
 LONG_DESCRIPTION = 'None'
 
 
 _root_path = f"{os.getcwd()}/volent"
 PY_MODULES = _gen.list_py_modules(
     _root_path,
```

### Comparing `colemen_volent-0.0.3/volent/Column.py` & `colemen_volent-0.0.4/volent/Column.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/Database.py` & `colemen_volent-0.0.4/volent/Database.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/Field.py` & `colemen_volent-0.0.4/volent/NestedField.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,86 +18,86 @@
 from volent.UniqueConstraint import UniqueConstraint as _uniqueConstraint
 from volent.mixins import MySQLGeneratorMixin
 from collections import OrderedDict
 from volent.exceptions import ValidationError
 
 
 @dataclass
-class Field:
-    main = None
-    # database:_t.database_type = None
+class NestedField:
+    '''A schema field used for retrieving related schemas as a list. '''
+    
+    
+    main:_t._main_type = None
     model:_t.model_type = None
     schema:_t.schema_type = None
+    child_schema:_t.schema_type = None
+    child_table:str = None
+    '''The name of the model that this field references.'''
 
 
     name:str = None
+    '''The name of this nested field.'''
 
-    # _fields:Iterable[_t.column_type] = None
     _description:str = None
     column:_t.column_type = None
 
 
     required:bool = False
     nullable:bool = True
     default = None
     validators = None
-    data_type:_t.type_base_type = None
 
 
     def __init__(
         self,
-        column:str=None,
-        required:bool=False,
-        nullable:bool=True,
-        empty_string_is_null:bool=True,
+        child_table:str=None,
+        child_schema:_t.schema_type=None,
         default=_settings.types.no_default,
-        validate=None,
-        data_type:_t.type_base_type=None
         ):
-        '''
-            Create a schema Field
-            ----------
-
-            Arguments
-            -------------------------
-            [`column`=None] {str}
-                The name of the column that this field represents.
-                The dot delimited path to the column
-
-                If None, it will attempt to find a matching column in the model.
-
-            [`required`=False] {bool}
-                arg_description
-
-            [`empty_string_is_null`=True] {bool}
-                Treat empty strings as None
-
-            [`default`] {any}
-                The default value to assign to this field
-
-            [`validate`=None] {any}
-                A list of validators to apply to this field
-
-            Meta
-            ----------
-            `author`: Colemen Atwood
-            `created`: 03-26-2023 09:34:14
-            `memberOf`: Field
-            `version`: 1.0
-            `method_name`: Field
-            * @xxx [04-14-2023 08:24:58]: documentation for Field
-        '''
-        self.column = column
+        # '''
+        #     Create a schema Field
+        #     ----------
+
+        #     Arguments
+        #     -------------------------
+        #     [`column`=None] {str}
+        #         The name of the column that this field represents.
+        #         The dot delimited path to the column
+
+        #         If None, it will attempt to find a matching column in the model.
+
+        #     [`required`=False] {bool}
+        #         arg_description
+
+        #     [`empty_string_is_null`=True] {bool}
+        #         Treat empty strings as None
+
+        #     [`default`] {any}
+        #         The default value to assign to this field
+
+        #     [`validate`=None] {any}
+        #         A list of validators to apply to this field
+
+        #     Meta
+        #     ----------
+        #     `author`: Colemen Atwood
+        #     `created`: 03-26-2023 09:34:14
+        #     `memberOf`: Field
+        #     `version`: 1.0
+        #     `method_name`: Field
+        #     * @xxx [04-14-2023 08:24:58]: documentation for Field
+        # '''
+        self.child_table = child_table
+        self.child_schema = child_schema
         self.default = default
-        self.required = required
-        self.nullable = nullable
-        self.empty_string_is_null = empty_string_is_null
-        self.data_type = data_type
+        # self.required = required
+        # self.nullable = nullable
+        # self.empty_string_is_null = empty_string_is_null
 
-        self.validators = c.arr.force_list(validate,allow_nulls=False)
+        # self.validators = c.arr.force_list(validate,allow_nulls=False)
 
 
     @property
     def summary(self):
         '''
             Get this Model's summary
 
@@ -150,42 +150,14 @@
             `@created`: 03-25-2023 12:02:50
             `@memberOf`: Field
             `@property`: value
         '''
         value = self.column.value
         return value
 
-
-
-    def validate_value(self,value):
-        val = value
-        if self.data_type is not None:
-            if hasattr(self.data_type,"deserialized_value"):
-                val = self.data_type.deserialized_value(val)
-        # val = self.column.data_type.
-
-        if isinstance(val,self.data_type.python_data_type) is False:
-            if self.nullable is True and val is None:
-                pass
-            else:
-                raise ValidationError(f"{self.name} expects {self.data_type.python_data_type} types.",self.name)
-
-        # if self._less_than_data_len(val) is False:
-        #     raise ValidationError(f"{self.name} is too long.",self.name)
-
-
-
-        if self._is_null(val):
-            raise ValidationError(f"{self.name} cannot be null.",self.name)
-
-
-        for valid in self.validators:
-            val = valid(val,self.name)
-
-
     def validate(self):
         # val = self.value
         val = self.column.deserialized_value
         # val = self.column.data_type.
 
         if isinstance(val,self.column.data_type.python_data_type) is False:
             if self.column.is_primary is True:
@@ -228,11 +200,61 @@
 
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} : {self.name}>"
 
 
 
+# def _gather_subs(model:_t.model_type):
+#     columns = []
+#     relationships:Iterable[_t.relationship_type] = []
+
+
+#     # @Mstep [] create an base instance to compare to.
+#     # print(f"model.__dataclass_fields__:{model.__fields__}")
+#     # print(list(model.__dict__.keys()))
+#     # print("\n\n\n")
+#     # print(dir(Model()))
+#     df_props = dir(Model())
+#     # @Mstep [] gather the props of this instance.
+#     props = dir(model)
+#     # @Mstep [] find the props that exist on this instance and not on the base.
+#     dif = c.arr.find_list_diff(props,df_props)
+
+#     for prop in dif:
+#         # print(f"prop: {prop} - {type(prop)}")
+#         if isinstance(getattr(model,prop),_column):
+#             prop:_t.model_type = getattr(model,prop)
+#             prop.database = model.database
+#             prop.main = model.main
+#             prop.model = model
+#             columns.append(prop)
+#             continue
+
+#         if isinstance(getattr(model,prop),_relationship):
+#             prop:_t.model_type = getattr(model,prop)
+#             prop.database = model.database
+#             prop.main = model.main
+#             prop.child_model = model
+#             if isinstance(prop.child,_column):
+#                 prop.child_column = prop.child
+#             if isinstance(prop,(str)):
+#                 prop.child_column = model.get_column(prop)
+#             relationships.append(prop)
+
+#     order_cols = []
+#     for k in list(model.__fields__):
+#         for col in columns:
+#             if col.name == k:
+#                 order_cols.append(col)
+#         # if k in columns:
+#         #     order_cols.append(columns[])
+
+
+
+#     model._columns = order_cols
+#     model._relationships = relationships
+
```

### Comparing `colemen_volent-0.0.3/volent/Model.py` & `colemen_volent-0.0.4/volent/Model.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/Relationship.py` & `colemen_volent-0.0.4/volent/Relationship.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/Schema.py` & `colemen_volent-0.0.4/volent/Schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 import volent.settings.types as _t
 import volent.settings as _settings
 from volent.Field import Field as _field
 from volent.NestedField import NestedField as _nested_field
 from volent.mixins import OrderedClass
+from volent.exceptions import ValidationError
 
 
 
 @dataclass
 class Schema(metaclass=OrderedClass):
     main = None
     # database:_t.database_type = None
@@ -215,67 +216,117 @@
 
 
             # return props
         self._fields = value
         return value
 
 
+    def __call_custom_validations(self):
+        '''
+            Searches for methods that start with "valid" and executes them.
+
+            This is allows custom validation methods to be added to the schema.
+            They are executed before the standard validations so that the custom ones can also
+            coerce values.
 
+            If ANY exception is raised in the custom method, this will raise a validationError.
+
+            ----------
+
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-24-2023 09:41:34
+            `memberOf`: Schema
+            `version`: 1.0
+            `method_name`: __call_custom_validations
+            * @xxx [04-24-2023 09:44:30]: documentation for __call_custom_validations
+        '''
+        for func in dir(self):
+            if func.startswith("valid"):
+                vm = getattr(self,func)
+                if callable(vm):
+                    try:
+                        vm()
+                    except Exception as e:
+                        raise ValidationError(e)
+                    # print(f"func: {func}")
+        # method_list = [func for func in dir(self) if callable(getattr(self, func))]
 
 
     def __validate(self):
         '''
             Execute the validation process on all fields associated to this schema
+
+            This will execute the custom validations before calling built it ones.
+
             ----------
 
             Meta
             ----------
             `author`: Colemen Atwood
             `created`: 04-21-2023 07:43:15
             `memberOf`: Schema
             `version`: 1.0
             `method_name`: __validate
             * @xxx [04-21-2023 07:44:01]: documentation for __validate
         '''
+        self.__call_custom_validations()
         for f in self.fields:
             f.validate()
 
 
     def __validate_dict(self,data:dict):
         '''
             Execute the validation process on all fields associated to this schema
+
+            This is used to validate a dictionary as opposed to __validate which will
+            validate the values that are assigned to columns.
+            
+            So this method has a little setup before it can validate which includes
+            it associating dictionary keys to matching fields.
+
+
             ----------
 
             Meta
             ----------
             `author`: Colemen Atwood
             `created`: 04-21-2023 07:43:15
             `memberOf`: Schema
             `version`: 1.0
             `method_name`: __validate
             * @xxx [04-21-2023 07:44:01]: documentation for __validate
         '''
         data = c.obj.keys_to_snake_case(data)
         for f in self.fields:
-            value = None
+            value = _settings.types.no_default
             if f.name not in data:
                 if f.required is True:
-                    raise ValueError(f"{f.name} is required.")
+                    raise ValidationError(f"{f.name} is required.")
                 elif c.string.to_snake_case(f.name) in data:
                     value = data[c.string.to_snake_case(f.name)]
                 else:
                     continue
             else:
                 value = data[f.name]
-            if value is not None:
-                f.validate_value(value)
+
+            if value is not _settings.types.no_default:
+            # if value is not None:
+                f.value = value
+
+        self.__call_custom_validations()
+        for f in self.fields:
+            f.validate()
 
     def get_field(self,name:str)->_t.field_type:
         '''
-            Retrieve a field from this schema
+            Retrieve a field instance from this schema by its name.
+
             ----------
 
             Arguments
             -------------------------
             `name` {string}
                 The name of the field to search for.
 
@@ -288,14 +339,15 @@
             `author`: Colemen Atwood
             `created`: 04-21-2023 07:44:07
             `memberOf`: Schema
             `version`: 1.0
             `method_name`: get_field
             * @xxx [04-21-2023 07:44:52]: documentation for get_field
         '''
+        name = c.string.to_snake_case(name)
         for field in self.fields:
             if field.name == name:
                 return field
         return None
 
     def from_dict(self,data:dict):
         '''
@@ -327,19 +379,54 @@
                 continue
             field = self.get_field(col.name)
             if field is None:
                 continue
 
             col.column_value = data[col]
 
+    def open_api_data(self,loc:str="body")->Iterable[dict]:
+        '''
+            Get this Schema's open_api_data
+
+            returns a list of dictionaries each representing a field, the dictionaries can
+            be used with the open api library for documentation.
+
+            ----------
+
+            Arguments
+            -------------------------
+            [`loc`='body'] {str}
+                Where the field's value can be found in a request ['body','path']
+
+
+            Return {list}
+            ----------------------
+            A list of dictionaries.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-24-2023 09:17:49
+            `memberOf`: Schema
+            `version`: 1.0
+            `method_name`: open_api_data
+            `throws`: ValueError - if the loc is not "body"/"path"
+            * @xxx [04-24-2023 09:19:05]: documentation for open_api_data
+        '''
+
+        value = []
+        if loc not in _settings.control.open_api_param_locations:
+            raise ValueError(f"{loc} is not a valid param location, expected: {','.join(_settings.control.open_api_param_locations)}")
+        for f in self.fields:
+            value.append(f.open_api_data(loc))
+        return value
 
     def dump(self,model:_t.model_type=None,many=False)->dict:
         '''Dump the contents of the model(s) using the fields to filter.'''
-        
-        
+
         if isinstance(model,(dict)):
             data = self._correlate_to_dict(model)
             self.__validate_dict(model)
             out_data = {}
             for f in self.fields:
                 if f.name in data:
                     if hasattr(f.data_type,"serialized_value"):
@@ -347,18 +434,18 @@
                         # print(f"v: {v}")
                         out_data[f.name] = v
                         continue
                     out_data[f.name] = data[f.name]
             if many:
                 out_data = c.arr.force_list(out_data)
             return out_data
-        
-        
-        
-        
+
+
+
+
 
         if isinstance(model,(list)):
             result = []
             from volent.Model import Model as _model
             for mdl in model:
                 if isinstance(mdl,_model) is False:
                     c.con.log(f"The mdl is not an instance of model:{mdl}","magenta")
@@ -425,23 +512,14 @@
         data = {}
         for f in self.fields:
             if f.dump_only is False:
                 data[f.name] = f.value
         self.model.update(**data).is_(self.model.primary_column.name,self.model.primary_column.value).execute()
         return self
 
-    # def to_dict(self):
-    #     data = {}
-    #     for f in self.fields:
-    #         data[f.name] = f.value
-
-    #     # for col in self.model.columns:
-    #     #     data[col.name] = col.column_value
-    #     return data
-
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} : {self.name.s}>"
 
 
     def __setattr__(self, name, value):
         super().__setattr__(name, value)
@@ -518,13 +596,13 @@
             raise ValueError(f"No Model Provided to {self.name}")
         for f in self.fields:
             if isinstance(f,_nested_field):
                 pri_col = self.model.primary_column
                 child_model = _settings.globe.Volent.get_model(f.child_table)
                 if child_model is not None:
                     child_model.select().is_(column_name=pri_col.name,value=pri_col.value)
-                
+
             # print(f"{self.__class__.__name__} - self.model:{self.model}")
             col = self.model.get_column(f.name)
             if col is not None:
                 f.column = col
```

### Comparing `colemen_volent-0.0.3/volent/UniqueConstraint.py` & `colemen_volent-0.0.4/volent/UniqueConstraint.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/Volent.py` & `colemen_volent-0.0.4/volent/Volent.py`

 * *Files 21% similar despite different names*

```diff
@@ -56,37 +56,96 @@
 
     # def set_defaults(self):
     #     self.settings = c.file.import_project_settings("volent.settings.json")
 
     def master(self):
         print("master")
 
-    def summary(self,file_path:str=None):
+    def summary(self,file_path:str=None)->dict:
+        '''
+            Generate a dictionary of summary data for all databases.
+
+            ----------
+
+            Arguments
+            -------------------------
+            [`file_path`=None] {str}
+                The path to save the summary to, if not provided, it is saved to the working directory.
+
+            Return {dict}
+            ----------------------
+            returns the summary dictionary
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-25-2023 08:05:45
+            `memberOf`: Volent
+            `version`: 1.0
+            `method_name`: summary
+            * @xxx [04-25-2023 08:26:06]: documentation for summary
+        '''
         if file_path is None:
             file_path = f"{os.getcwd()}/summary.json"
 
         data = {
             "databases":[x.summary for x in self.databases]
         }
         c.file.writer.to_json(file_path,data)
         return data
 
 
     def start(self):
+        '''
+            Initiate the models, determine their relationships and connect to the databse.
+
+            Raises a runtime error if it fails to connect to the database.
+
+            ----------
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-25-2023 08:04:33
+            `memberOf`: Volent
+            `version`: 1.0
+            `method_name`: start
+            * @TODO []: documentation for start
+        '''
         self._deep_registration()
         self._determine_relationships()
         self._generate_databases()
-        self.connect()
-        
-        
-        for db in self.databases:
-            db.existing_tables()
+        # result = self.connect()
+        if self.connect() is False:
+            raise RuntimeError("Failed to connect to the database.")
+        else:
+            for db in self.databases:
+                db.existing_tables()
 
 
     def register(self,instance):
+        '''
+            Used internally for registration and mapping of the database structure.
+
+            ----------
+
+            Arguments
+            -------------------------
+            `instance` {any}
+                The entity to register.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-25-2023 08:26:17
+            `memberOf`: Volent
+            `version`: 1.0
+            `method_name`: register
+            * @xxx [04-25-2023 08:26:56]: documentation for register
+        '''
         if isinstance(instance,Model):
             # c.con.log(f"Registering New Model: {instance.name}","info")
             if instance.name in self.model_names:
                 raise ValueError(f"Duplicate Name for Model : {instance.name}")
             self.models.append(instance)
             self.model_names.append(instance.name)
 
@@ -160,36 +219,60 @@
             if model is None:
                 raise ValueError(f"Failed to locate column from {name} - Could not find model {mdl_name}")
             column = model.get_column(col_name)
             if column is None:
                 raise ValueError(f"Failed to locate column from {name} - Could not find column {col_name}")
             return column
 
-
     def get_model(self,name:str)->_t.model_type:
+        '''
+            Retrieve a model by searching for its name.
+
+            ----------
+
+            Arguments
+            -------------------------
+            `name` {str}
+                The name of the model to search for.
+
+                This can also be a dot path: database_name.table_name
+
+
+            Return {model}
+            ----------------------
+            The model instance if successfull, None otherwise.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-25-2023 08:27:11
+            `memberOf`: Volent
+            `version`: 1.0
+            `method_name`: get_model
+            * @xxx [04-25-2023 08:28:14]: documentation for get_model
+        '''
         name = c.string.strip_excessive_chars(name,["."])
         nl = name.split(".")
         if len(nl) == 2:
             name = nl[0]
         for md in self.models:
             if md.name == name:
                 # print(f"---------------------------------name: {name}")
                 return md
 
         return None
-    
+
     # def get_base_model(self,)
 
     def _deep_registration(self):
         '''This will iterate all models to have their sub entities register with this instance.'''
         c.con.log("Initiating Deep Registration","info")
         for mdl in self.models:
             mdl.volent_register_subs()
 
-
     def _determine_relationships(self):
         c.con.log("Determining relationships between tables","info")
 
         # @Mstep [LOOP] iterate all relationship instances.
         # for rel in self.relationships:
         #     # @Mstep [] Attempt to retrieve the parent
         #     parent_string = rel.parent
@@ -199,17 +282,17 @@
         #         rel.parent_model = pm
         #     else:
         #         c.con.log(f"Failed to locate parent model for relationship {rel.name} from dot_path: {parent_string}","red")
 
         #     pc = self.get_column(parent_string)
         #     if pc is not None:
         #         rel.parent_column = pc
-                
-                
-            
+
+
+
 
 
 
 
 
     # ---------------------------------------------------------------------------- #
     #                                   DATABASES                                  #
@@ -296,15 +379,41 @@
 
 
 
 
 
 
 
-    def generate_sql(self,file_path:str=None,drops:bool=True):
+    def generate_sql(self,file_path:str=None,drops:bool=True)->str:
+        '''
+            Generate the master SQL file for the database.
+
+            ----------
+
+            Arguments
+            -------------------------
+            [`file_path`=None] {str}
+                The path to save the SQL to, it will default to the cwd/master.sql
+
+            [`drops`=True] {bool}
+                If False, it will not drop existing tables before creating them.
+
+            Return {str}
+            ----------------------
+            The master SQL content as a string.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-25-2023 08:29:02
+            `memberOf`: Volent
+            `version`: 1.0
+            `method_name`: generate_sql
+            * @TODO []: documentation for generate_sql
+        '''
         if file_path is None:
             file_path = f"{os.getcwd()}/master.sql"
         sql = self.master_sql(file_path,drops)
         return sql
 
 
     def drop_all_tables(self):
@@ -324,14 +433,15 @@
 
         for db in self.databases:
             db.drop_tables()
 
     def create_all(self,force=False):
         '''
             Create all schemas and tables in the database.
+            
             ----------
 
             Arguments
             -------------------------
             [`force`=bool] {False}
                 If True, this will drop the tables then recreate them
```

### Comparing `colemen_volent-0.0.3/volent/data_types/BigInt.py` & `colemen_volent-0.0.4/volent/data_types/TinyInt.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,22 @@
 from typing import Iterable
 import colemen_utils as c
 import volent.settings as _settings
 import volent.settings.types as _t
 from volent.data_types.TypeBase import TypeBase as _type_base
 
 @dataclass
-class BigInt(_type_base):
-
-
-
+class TinyInt(_type_base):
 
     def __init__(self,data_length:int=None) -> None:
         super().__init__(data_length)
         self.min_data_length = 0
-        self.max_data_length = 65535
-        self.sql_type_name = "BIGINT"
+        self.max_data_length = 255
+        self.sql_type_name = "TINYINT"
         self.python_data_type = (int)
+        self.open_api_data_type = "integer"
 
-        self._validate_data_length(data_length)
-
+        self._validate_data_length(data_length,_settings.control.varchar_default_length)
 
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} : {self.data_length}>"
```

### Comparing `colemen_volent-0.0.3/volent/data_types/Bool.py` & `colemen_volent-0.0.4/volent/data_types/Bool.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 class Bool(_type_base):
 
 
     def __init__(self) -> None:
         super().__init__()
         self.sql_type_name = "BOOLEAN"
         self.python_data_type = (bool)
+        self.open_api_data_type = "boolean"
 
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} >"
```

### Comparing `colemen_volent-0.0.3/volent/data_types/Decimal.py` & `colemen_volent-0.0.4/volent/data_types/Decimal.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     def __init__(self,data_length:int=10,decimal:int=0) -> None:
         super().__init__(data_length)
         self.min_data_length = 0
         self.max_data_length = 65
         self.sql_type_name = "Decimal"
         self.python_data_type = (float)
+        self.open_api_data_type = "float"
 
         self._validate_data_length(data_length,_settings.control.varchar_default_length)
         if decimal > 30 or decimal < 0:
             raise ValueError("The decimal for a Decimal must range from 0 to 10")
 
         self.decimal = decimal
```

### Comparing `colemen_volent-0.0.3/volent/data_types/EncodedPrimary.py` & `colemen_volent-0.0.4/volent/data_types/EncodedPrimary.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
     def __init__(self,data_length:int=None) -> None:
         super().__init__(data_length)
         self.min_data_length = 0
         self.max_data_length = 65535
         self.sql_type_name = "BIGINT"
         self.python_data_type = (int,str)
+        self.open_api_data_type = "string"
 
         self._validate_data_length(data_length)
 
 
     def serialized_value(self,value):
         if isinstance(value,(str)):
             return value
```

### Comparing `colemen_volent-0.0.3/volent/data_types/Integer.py` & `colemen_volent-0.0.4/volent/data_types/Integer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     def __init__(self,data_length:int=None) -> None:
         super().__init__(data_length)
         self.min_data_length = 0
         self.max_data_length = 4294967295
         self.sql_type_name = "INTEGER"
         self.python_data_type = (int)
+        self.open_api_data_type = "integer"
 
         self._validate_data_length(data_length)
 
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} : {self.data_length}>"
 
@@ -41,9 +42,11 @@
             raise ValidationError(f"Failed to serialize {value} to integer.")
 
         return value
 
     def deserialized_value(self,value):
         if isinstance(value,(int)):
             return value
+        if value is None:
+            return value
         if isinstance(value,(int)) is False:
             raise ValidationError(f"Failed to deserialize {value} to integer.")
```

### Comparing `colemen_volent-0.0.3/volent/data_types/String.py` & `colemen_volent-0.0.4/volent/data_types/String.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/data_types/TinyInt.py` & `colemen_volent-0.0.4/volent/data_types/BigInt.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,21 +7,26 @@
 from typing import Iterable
 import colemen_utils as c
 import volent.settings as _settings
 import volent.settings.types as _t
 from volent.data_types.TypeBase import TypeBase as _type_base
 
 @dataclass
-class TinyInt(_type_base):
+class BigInt(_type_base):
+
+
+
 
     def __init__(self,data_length:int=None) -> None:
         super().__init__(data_length)
         self.min_data_length = 0
-        self.max_data_length = 255
-        self.sql_type_name = "TINYINT"
+        self.max_data_length = 65535
+        self.sql_type_name = "BIGINT"
         self.python_data_type = (int)
+        self.open_api_data_type = "integer"
+
+        self._validate_data_length(data_length)
 
-        self._validate_data_length(data_length,_settings.control.varchar_default_length)
 
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} : {self.data_length}>"
```

### Comparing `colemen_volent-0.0.3/volent/data_types/TypeBase.py` & `colemen_volent-0.0.4/volent/data_types/TypeBase.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/exceptions.py` & `colemen_volent-0.0.4/volent/exceptions.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/mixins/DatabaseConnection.py` & `colemen_volent-0.0.4/volent/mixins/DatabaseConnection.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,24 +89,28 @@
             if db_creds is None:
                 c.con.log(f"Failed to locate credentials for database: {db}","error")
             else:
                 connect_success = self.__connect_to_my_sqldb(db_creds)
                 if connect_success:
                     # _traceback.print_stack()
                     c.con.log(f"Successfully connected to {db_creds['database']}","green")
+                    # connect_success = True
+                    return True
 
         else:
-
             from volent.Volent import Volent as _bv
             if isinstance(self,_bv):
                 for db in self.databases:
                     result = db.connect()
                     if result is False:
                         c.con.log(f"Failed to connect to {db.name}","warning")
                         connect_success = False
+                        return False
+                return True
+                    
 
 
 
         # if _settings.globe.flavor == "mysql":
         #     if db_creds is None:
         #         db_creds = self.credentials()
         #     if isinstance(db_creds,(dict)):
```

### Comparing `colemen_volent-0.0.3/volent/mixins/EntityName.py` & `colemen_volent-0.0.4/volent/mixins/EntityName.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/mixins/MySQLGeneratorMixin.py` & `colemen_volent-0.0.4/volent/mixins/MySQLGeneratorMixin.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/mixins/OrderedClass.py` & `colemen_volent-0.0.4/volent/mixins/OrderedClass.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/query/Insert.py` & `colemen_volent-0.0.4/volent/query/Insert.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/query/Query.py` & `colemen_volent-0.0.4/volent/query/Query.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/query/Select.py` & `colemen_volent-0.0.4/volent/query/Select.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/query/Update.py` & `colemen_volent-0.0.4/volent/query/Update.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/query/WhereMixin.py` & `colemen_volent-0.0.4/volent/query/WhereMixin.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/settings/control.py` & `colemen_volent-0.0.4/volent/settings/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 '''
 
 
 
 
 from typing import Union
 
+open_api_param_locations = ["body","path"]
+
 
 sql_quote_char:str = "`"
 '''The character to use for quoting strings in the sql output'''
 varchar_default_length:int = 50
 '''The default character length for varchar columns'''
```

### Comparing `colemen_volent-0.0.3/volent/settings/types.py` & `colemen_volent-0.0.4/volent/settings/types.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/CreditCardNumber.py` & `colemen_volent-0.0.4/volent/validate/CreditCardNumber.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,14 +70,42 @@
 
 
     def _repr_args(self) -> str:
         return f""
 
     def __call__(self,value:_T,field_name:str=None)->_T:
         self.field_name = field_name
-        if self.regex.match(value) is None:
+
+        if luhn_checksum(value) != 0:
             raise ValidationError(self._format_error(value))
+        else:
+            return value
+
+
+
+
+
+
+
+
+        # if re.search(self.regex,value) is None:
+        # # if self.regex.match(value) is None:
+        #     raise ValidationError(self._format_error(value))
+
+
+        # return value
 
 
-        return value
 
+def luhn_checksum(card_number):
+    def digits_of(n):
+        return [int(d) for d in str(n)]
+    digits = digits_of(card_number)
+    odd_digits = digits[-1::-2]
+    even_digits = digits[-2::-2]
+    checksum = 0
+    checksum += sum(odd_digits)
+    for d in even_digits:
+        checksum += sum(digits_of(d*2))
+    return checksum % 10
 
+# print('Valid') if luhn_checksum("4532015112830366")==0 else print('Invalid')
```

### Comparing `colemen_volent-0.0.3/volent/validate/Email.py` & `colemen_volent-0.0.4/volent/validate/Email.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/Equal.py` & `colemen_volent-0.0.4/volent/validate/Equal.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/FutureUnixDate.py` & `colemen_volent-0.0.4/volent/validate/FutureUnixDate.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/IpAddress.py` & `colemen_volent-0.0.4/volent/validate/IpAddress.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,16 +59,21 @@
             `memberOf`: NoneOf
             `version`: 1.0
             `method_name`: NoneOf
             * @xxx [03-27-2023 09:13:12]: documentation for NoneOf
         '''
         self.ipv4 = ipv4
         self.ipv6 = ipv6
-        self.ipv4_regex = re.compile(r"(?:[0-9]{1,3}\.){3}[0-9]{1,3}")
-        self.ipv6_regex = re.compile(r"(([0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,7}:|([0-9a-fA-F]{1,4}:){1,6}:[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,5}(:[0-9a-fA-F]{1,4}){1,2}|([0-9a-fA-F]{1,4}:){1,4}(:[0-9a-fA-F]{1,4}){1,3}|([0-9a-fA-F]{1,4}:){1,3}(:[0-9a-fA-F]{1,4}){1,4}|([0-9a-fA-F]{1,4}:){1,2}(:[0-9a-fA-F]{1,4}){1,5}|[0-9a-fA-F]{1,4}:((:[0-9a-fA-F]{1,4}){1,6})|:((:[0-9a-fA-F]{1,4}){1,7}|:)|fe80:(:[0-9a-fA-F]{0,4}){0,4}%[0-9a-zA-Z]{1,}|::(ffff(:0{1,4}){0,1}:){0,1}((25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])|([0-9a-fA-F]{1,4}:){1,4}:((25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9]))")
+        # self.ipv4_regex = re.compile(r"^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$")
+        self.ipv4_regex = re.compile(r"^((25[0-5]|2[0-4][0-9]|1[0-9][0-9]|[1-9]?[0-9])\.){3}(25[0-5]|2[0-4][0-9]|1[0-9][0-9]|[1-9]?[0-9])$")
+        # self.ipv4_regex = re.compile(r"(?:[0-9]{1,3}\.){3}[0-9]{1,3}")
+        ipv6_regex = "((([0-9a-fA-F]){1,4})\\:){7}"\
+            "([0-9a-fA-F]){1,4}"
+        self.ipv6_regex = re.compile(ipv6_regex)
+        # self.ipv6_regex = re.compile(r"(([0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,7}:|([0-9a-fA-F]{1,4}:){1,6}:[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,5}(:[0-9a-fA-F]{1,4}){1,2}|([0-9a-fA-F]{1,4}:){1,4}(:[0-9a-fA-F]{1,4}){1,3}|([0-9a-fA-F]{1,4}:){1,3}(:[0-9a-fA-F]{1,4}){1,4}|([0-9a-fA-F]{1,4}:){1,2}(:[0-9a-fA-F]{1,4}){1,5}|[0-9a-fA-F]{1,4}:((:[0-9a-fA-F]{1,4}){1,6})|:((:[0-9a-fA-F]{1,4}){1,7}|:)|fe80:(:[0-9a-fA-F]{0,4}){0,4}%[0-9a-zA-Z]{1,}|::(ffff(:0{1,4}){0,1}:){0,1}((25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])|([0-9a-fA-F]{1,4}:){1,4}:((25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9]))")
 
         self.error = error or self.default_message  # type: str
 
 
     def _format_error(self, value: Union[str,bytes]) -> str:
         args = {
             "input":value,
@@ -81,17 +86,19 @@
 
     def _repr_args(self) -> str:
         return f"ipv4={self.ipv4!r},ipv6={self.ipv6!r}"
 
     def __call__(self,value:_T,field_name:str=None)->_T:
         self.field_name = field_name
         if self.ipv4 is True:
-            if self.ipv4_regex.match(value) is True:
+            if re.search(self.ipv4_regex,value):
+            # if self.ipv4_regex.match(value) is True:
                 return value
 
         if self.ipv6 is True:
-            if self.ipv6_regex.match(value) is True:
+            if re.search(self.ipv6_regex,value):
+            # if self.ipv6_regex.match(value) is True:
                 return value
 
         raise ValidationError(self._format_error(value))
```

### Comparing `colemen_volent-0.0.3/volent/validate/Length.py` & `colemen_volent-0.0.4/volent/validate/Length.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/NoneOf.py` & `colemen_volent-0.0.4/volent/validate/NoneOf.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/OneOf.py` & `colemen_volent-0.0.4/volent/validate/OneOf.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/PastUnixDate.py` & `colemen_volent-0.0.4/volent/validate/PastUnixDate.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/PhoneNumber.py` & `colemen_volent-0.0.4/volent/validate/PhoneNumber.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,15 +50,16 @@
             `author`: Colemen Atwood
             `created`: 03-27-2023 09:10:41
             `memberOf`: NoneOf
             `version`: 1.0
             `method_name`: NoneOf
             * @xxx [03-27-2023 09:13:12]: documentation for NoneOf
         '''
-        self.regex = re.compile(r"^[\+]?[(]?[0-9]{3}[)]?[-\s\.]?[0-9]{3}[-\s\.]?[0-9]{4,6}$")
+        self.regex = re.compile(r"^(?:\+?\d{1,3}[\s.-]?)?\(?\d{3}\)?[\s.-]?\d{3}[\s.-]?\d{4}(?:x?\d{1,5}?)?$")
+        # self.regex = re.compile(r"^[\+]?[(]?[0-9]{3}[)]?[-\s\.]?[0-9]{3}[-\s\.]?[0-9]{4,6}$")
         self.error = error or self.default_message  # type: str
 
 
     def _format_error(self, value: Union[str,bytes]) -> str:
         args = {
             "input":value,
         }
@@ -69,14 +70,15 @@
 
 
     def _repr_args(self) -> str:
         return f""
 
     def __call__(self,value:_T,field_name:str=None)->_T:
         self.field_name = field_name
-        if self.regex.match(value) is None:
-            raise ValidationError(self._format_error(value))
+        if re.search(self.regex,value):
+            return value
+        # if self.regex.match(value) is None:
+        raise ValidationError(self._format_error(value))
 
 
-        return value
```

### Comparing `colemen_volent-0.0.3/volent/validate/Range.py` & `colemen_volent-0.0.4/volent/validate/Range.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/Regex.py` & `colemen_volent-0.0.4/volent/validate/Regex.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/SocialSecurityNumber.py` & `colemen_volent-0.0.4/volent/validate/SocialSecurityNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/StrongPassword.py` & `colemen_volent-0.0.4/volent/validate/StrongPassword.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/Validator.py` & `colemen_volent-0.0.4/volent/validate/Validator.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.3/volent/validate/__init__.py` & `colemen_volent-0.0.4/volent/validate/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from volent.validate.Validator import Validator
 from volent.validate.Length import Length
 from volent.validate.OneOf import OneOf,ContainsOnly
 from volent.validate.Email import Email
 from volent.validate.Equal import Equal
 from volent.validate.NoneOf import NoneOf
 from volent.validate.Range import Range
+from volent.validate.Regex import Regex
 from volent.validate.IpAddress import IpAddress
 from volent.validate.CreditCardNumber import CreditCardNumber
 from volent.validate.PhoneNumber import PhoneNumber
 from volent.validate.SocialSecurityNumber import SocialSecurityNumber
 from volent.validate.StrongPassword import StrongPassword
 from volent.validate.FutureUnixDate import FutureUnixDate
 from volent.validate.PastUnixDate import PastUnixDate
```

