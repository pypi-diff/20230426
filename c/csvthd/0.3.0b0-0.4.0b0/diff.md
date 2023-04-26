# Comparing `tmp/csvthd-0.3.0b0.tar.gz` & `tmp/csvthd-0.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvthd-0.3.0b0.tar", max compression
+gzip compressed data, was "csvthd-0.4.0b0.tar", max compression
```

## Comparing `csvthd-0.3.0b0.tar` & `csvthd-0.4.0b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4050 2023-04-26 02:58:44.271303 csvthd-0.3.0b0/README.md
--rw-r--r--   0        0        0        0 2023-04-23 14:03:39.147538 csvthd-0.3.0b0/csvthd/__init__.py
--rw-r--r--   0        0        0       59 2023-04-24 05:21:37.075961 csvthd-0.3.0b0/csvthd/__main__.py
--rw-r--r--   0        0        0      114 2023-04-26 03:03:33.332370 csvthd-0.3.0b0/csvthd/__version__.py
--rw-r--r--   0        0        0     3251 2023-04-26 02:45:12.296711 csvthd-0.3.0b0/csvthd/cli.py
--rw-r--r--   0        0        0      623 2023-04-25 14:26:47.536086 csvthd-0.3.0b0/csvthd/commandline.py
--rw-r--r--   0        0        0      683 2023-04-25 14:29:47.324668 csvthd-0.3.0b0/csvthd/config.py
--rw-r--r--   0        0        0     2561 2023-04-26 02:41:40.145596 csvthd-0.3.0b0/csvthd/filters.py
--rw-r--r--   0        0        0      246 2023-04-25 13:00:43.420813 csvthd-0.3.0b0/csvthd/reducers.py
--rw-r--r--   0        0        0      941 2023-04-24 05:00:16.609784 csvthd-0.3.0b0/csvthd/transactions.py
--rw-r--r--   0        0        0     1046 2023-04-26 03:03:26.884586 csvthd-0.3.0b0/pyproject.toml
--rw-r--r--   0        0        0     4975 1970-01-01 00:00:00.000000 csvthd-0.3.0b0/PKG-INFO
+-rw-r--r--   0        0        0     4515 2023-04-26 04:46:52.053337 csvthd-0.4.0b0/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 14:03:39.147538 csvthd-0.4.0b0/csvthd/__init__.py
+-rw-r--r--   0        0        0       59 2023-04-24 05:21:37.075961 csvthd-0.4.0b0/csvthd/__main__.py
+-rw-r--r--   0        0        0      114 2023-04-26 05:28:34.442698 csvthd-0.4.0b0/csvthd/__version__.py
+-rw-r--r--   0        0        0     3495 2023-04-26 05:02:47.807005 csvthd-0.4.0b0/csvthd/cli.py
+-rw-r--r--   0        0        0      623 2023-04-25 14:26:47.536086 csvthd-0.4.0b0/csvthd/commandline.py
+-rw-r--r--   0        0        0      683 2023-04-25 14:29:47.324668 csvthd-0.4.0b0/csvthd/config.py
+-rw-r--r--   0        0        0     2904 2023-04-26 04:32:58.115627 csvthd-0.4.0b0/csvthd/filters.py
+-rw-r--r--   0        0        0      959 2023-04-26 05:03:30.975285 csvthd-0.4.0b0/csvthd/reducers.py
+-rw-r--r--   0        0        0     1709 2023-04-26 05:03:13.125557 csvthd-0.4.0b0/csvthd/transactions.py
+-rw-r--r--   0        0        0     1046 2023-04-26 05:28:28.798642 csvthd-0.4.0b0/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 csvthd-0.4.0b0/PKG-INFO
```

### Comparing `csvthd-0.3.0b0/README.md` & `csvthd-0.4.0b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 ## Installation
 
 ```bash
 pip install csvthd
 ```
 
+<!-- TODO: add a "features" section that highlights the capabilities of csvthd in a non-technical way. i.e. filtering/sorting/reporting/etc. options -->
+
 ## Usage
 
 ### Show help
 
 ```bash
 csvthd --help
 ```
@@ -101,14 +103,28 @@
 # only show transactions with details containing "paypal" where money received
 csvthd -i paypal -t in
 
 # get the sum of all money received with "paypal" in details but not "return"
 csvthd -i paypal -t in -E return -S
 ```
 
+#### Account Name
+
+`-A/--account-name`
+
+Only show transactions from account names that include the provided text.
+
+```bash
+# only show transactions where the account name includes "commbank"
+csvthd -A commbank
+
+# get the sum of all transactions where the account name includes "paypal"
+csvthd -A paypal -S
+```
+
 ### Sorting
 
 #### Sort by
 
 `-s/--sort-by`
 
 ```bash
```

### Comparing `csvthd-0.3.0b0/csvthd/cli.py` & `csvthd-0.4.0b0/csvthd/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 
 # package
 from .filters import (
     details_include_filter,
     details_exclude_filter,
     amount_is_filter,
     transaction_type_filter,
+    account_name_filter,
 )
 from .commandline import print_transaction, style_amount
 from .transactions import get_transactions
 from .config import load_config
 from .reducers import sum_transaction_amount
 
 # TODO: consider looking into (odx?) other formats because someone mentioned apparently there
 # ... are some other commons ones that are standardized.
 
-# TODO: add option to get calculate total sum of filtered out transactions
-
 
 @click.command()
 @click.option(
     "-i",
     "--include",
     multiple=True,
     help="Only show transactions that contain the given substring in their details.",
@@ -46,14 +45,19 @@
 @click.option(
     "-t",
     "--transaction-type",
     type=click.Choice(["out", "in"]),
     help="Only show transactions where money is sent/received.",
 )
 @click.option(
+    "-A",
+    "--account-name",
+    help="Only show transactions from account names that include this text.",
+)
+@click.option(
     "-s",
     "--sort-by",
     type=click.Choice(["date", "amount"]),
     default="date",
     help="Sort transactions by given property.",
 )
 @click.option(
@@ -62,22 +66,33 @@
 @click.option(
     "-S",
     "--sum",
     is_flag=True,
     help="Give a sum of all transaction amounts after filtering.",
 )
 def cli(
-    include, exclude, amount, transaction_type, sort_by, reverse_sort, sum
+    include,
+    exclude,
+    amount,
+    transaction_type,
+    account_name,
+    sort_by,
+    reverse_sort,
+    sum,
 ):
     filters = []
 
     # create transaction type filter
     if transaction_type is not None:
         filters.append(transaction_type_filter(transaction_type))
 
+    # create account name filter
+    if account_name is not None:
+        filters.append(account_name_filter(account_name))
+
     # create include filters
     filters.append(details_include_filter(include))
 
     # create exclude filters
     filters.append(details_exclude_filter(exclude))
 
     # create amount is filters
```

### Comparing `csvthd-0.3.0b0/csvthd/commandline.py` & `csvthd-0.4.0b0/csvthd/commandline.py`

 * *Files identical despite different names*

### Comparing `csvthd-0.3.0b0/csvthd/config.py` & `csvthd-0.4.0b0/csvthd/config.py`

 * *Files identical despite different names*

### Comparing `csvthd-0.3.0b0/csvthd/filters.py` & `csvthd-0.4.0b0/csvthd/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,7 +78,19 @@
             return _amount < 0
         elif transaction_type == "in":
             return _amount >= 0
         else:
             raise ValueError("transaction_type must by `in` or `out`")
 
     return _func
+
+
+def account_name_filter(account_name):
+    """Only return transactions with account names that contain the provided string."""
+
+    # transform account name to lowercase for comparison
+    _account_name = account_name.lower()
+
+    def _func(transaction):
+        return _account_name in transaction["account_name"].lower()
+
+    return _func
```

### Comparing `csvthd-0.3.0b0/pyproject.toml` & `csvthd-0.4.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "csvthd"
-version = "0.3.0b0"
+version = "0.4.0b0"
 description = "CSV Transaction History Detective"
 authors = ["DrTexx <denver.opensource@tutanota.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 repository = "https://gitlab.com/DrTexx/csv-transaction-history-detective/"
 documentation = "https://gitlab.com/DrTexx/csv-transaction-history-detective/#getting-started"
 keywords = ["finance", "csv", "transactions", "tax", "accounting"]
```

### Comparing `csvthd-0.3.0b0/PKG-INFO` & `csvthd-0.4.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvthd
-Version: 0.3.0b0
+Version: 0.4.0b0
 Summary: CSV Transaction History Detective
 Home-page: https://gitlab.com/DrTexx/csv-transaction-history-detective/
 License: AGPL-3.0-only
 Keywords: finance,csv,transactions,tax,accounting
 Author: DrTexx
 Author-email: denver.opensource@tutanota.com
 Requires-Python: >=3.8,<4.0
@@ -35,14 +35,16 @@
 
 ## Installation
 
 ```bash
 pip install csvthd
 ```
 
+<!-- TODO: add a "features" section that highlights the capabilities of csvthd in a non-technical way. i.e. filtering/sorting/reporting/etc. options -->
+
 ## Usage
 
 ### Show help
 
 ```bash
 csvthd --help
 ```
@@ -122,14 +124,28 @@
 # only show transactions with details containing "paypal" where money received
 csvthd -i paypal -t in
 
 # get the sum of all money received with "paypal" in details but not "return"
 csvthd -i paypal -t in -E return -S
 ```
 
+#### Account Name
+
+`-A/--account-name`
+
+Only show transactions from account names that include the provided text.
+
+```bash
+# only show transactions where the account name includes "commbank"
+csvthd -A commbank
+
+# get the sum of all transactions where the account name includes "paypal"
+csvthd -A paypal -S
+```
+
 ### Sorting
 
 #### Sort by
 
 `-s/--sort-by`
 
 ```bash
```

