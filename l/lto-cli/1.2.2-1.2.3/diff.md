# Comparing `tmp/lto-cli-1.2.2.tar.gz` & `tmp/lto-cli-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lto-cli-1.2.2.tar", last modified: Mon Oct 31 15:33:45 2022, max compression
+gzip compressed data, was "lto-cli-1.2.3.tar", last modified: Tue Apr 25 15:39:08 2023, max compression
```

## Comparing `lto-cli-1.2.2.tar` & `lto-cli-1.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-31 15:33:45.094036 lto-cli-1.2.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2022-10-31 15:33:20.000000 lto-cli-1.2.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     4452 2022-10-31 15:33:45.094036 lto-cli-1.2.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3970 2022-10-31 15:33:20.000000 lto-cli-1.2.2/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      107 2022-10-31 15:33:20.000000 lto-cli-1.2.2/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      765 2022-10-31 15:33:45.094036 lto-cli-1.2.2/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-31 15:33:45.078028 lto-cli-1.2.2/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-31 15:33:45.086032 lto-cli-1.2.2/src/lto_cli/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    31833 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/cli.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-31 15:33:45.094036 lto-cli-1.2.2/src/lto_cli/commands/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2609 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/account.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2980 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/anchor.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3444 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/association.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1799 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/balance.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1170 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/broadcast.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1084 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/burn.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2497 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/data.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3485 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/leasing.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1503 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/mass_transfer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1026 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/node.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1134 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/script.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2906 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/sponsorship.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1147 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/commands/transfer.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7065 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/config.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2743 2022-10-31 15:33:20.000000 lto-cli-1.2.2/src/lto_cli/handle_default.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-31 15:33:45.090034 lto-cli-1.2.2/src/lto_cli.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4452 2022-10-31 15:33:45.000000 lto-cli-1.2.2/src/lto_cli.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      804 2022-10-31 15:33:45.000000 lto-cli-1.2.2/src/lto_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-10-31 15:33:45.000000 lto-cli-1.2.2/src/lto_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2022-10-31 15:33:45.000000 lto-cli-1.2.2/src/lto_cli.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2022-10-31 15:33:45.000000 lto-cli-1.2.2/src/lto_cli.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2022-10-31 15:33:45.000000 lto-cli-1.2.2/src/lto_cli.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 15:39:08.965473 lto-cli-1.2.3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2023-04-25 15:38:46.000000 lto-cli-1.2.3/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4452 2023-04-25 15:39:08.965473 lto-cli-1.2.3/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3970 2023-04-25 15:38:46.000000 lto-cli-1.2.3/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      107 2023-04-25 15:38:46.000000 lto-cli-1.2.3/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      765 2023-04-25 15:39:08.965473 lto-cli-1.2.3/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 15:39:08.885433 lto-cli-1.2.3/src/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 15:39:08.905443 lto-cli-1.2.3/src/lto_cli/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35885 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/cli.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 15:39:08.965473 lto-cli-1.2.3/src/lto_cli/commands/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2581 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2980 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/anchor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3241 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/association.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1536 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/balance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/broadcast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1084 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/burn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2478 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3197 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/leasing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1503 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/mass_transfer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      965 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/node.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1134 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2720 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/sponsorship.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/commands/transfer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7096 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3146 2023-04-25 15:38:46.000000 lto-cli-1.2.3/src/lto_cli/handle_default.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 15:39:08.921451 lto-cli-1.2.3/src/lto_cli.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4452 2023-04-25 15:39:08.000000 lto-cli-1.2.3/src/lto_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      804 2023-04-25 15:39:08.000000 lto-cli-1.2.3/src/lto_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-25 15:39:08.000000 lto-cli-1.2.3/src/lto_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       41 2023-04-25 15:39:08.000000 lto-cli-1.2.3/src/lto_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2023-04-25 15:39:08.000000 lto-cli-1.2.3/src/lto_cli.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-25 15:39:08.000000 lto-cli-1.2.3/src/lto_cli.egg-info/top_level.txt
```

### Comparing `lto-cli-1.2.2/LICENSE` & `lto-cli-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lto-cli-1.2.2/PKG-INFO` & `lto-cli-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lto-cli
-Version: 1.2.2
+Version: 1.2.3
 Summary: LTO Network CLI
 Home-page: https://github.com/ltonetwork/lto-cli
 Author: LTO Network
 Author-email: info@ltonetwork.com
 Project-URL: Bug Tracker, https://github.com/ltonetwork/lto-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lto-cli-1.2.2/README.md` & `lto-cli-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lto-cli-1.2.2/setup.cfg` & `lto-cli-1.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lto-cli
-version = v1.2.2
+version = v1.2.3
 author = LTO Network
 author_email = info@ltonetwork.com
 description = LTO Network CLI
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ltonetwork/lto-cli
 project_urls =
```

### Comparing `lto-cli-1.2.2/src/lto_cli/cli.py` & `lto-cli-1.2.3/src/lto_cli/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,272 +55,301 @@
     parser_data = subparsers.add_parser('data', help="Create a data transaction or get the data associated with one account, type 'lto data --help' for more informations")
     data_subparser = parser_data.add_subparsers(dest='subparser-name-data')
 
     parser_set = data_subparser.add_parser('set', help="Create a data transaction, for more information on how to pipe the data type 'lto data set --help")
     parser_set.add_argument('stdin', nargs='?', type=argparse.FileType('r'), default=sys.stdin,  help="Takes the data as input: echo 'my data' | lto data set")
     parser_set.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_set.add_argument('--network', type=str, nargs=1, required=False, help='Optional network parameter, if not specified default is L')
+    parser_set.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
     parser_set.add_argument('--sponsor', type=str , nargs=1, required=False, help="Use this option to select an account for sponsoring the transaction")
     parser_set.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_set.add_argument('--unsigned', action='store_true', required=False, help="Use this option to not sign the transaction. Use in combination with the '--no-broadcast' option")
 
     parser_get = data_subparser.add_parser('get', help="Retrive the data associated with one account, if not specified the default account is selected, for more infotmations type 'lto data get --help")
     parser_get.add_argument('address', nargs='?', type=str, help='Insert the desired account address')
     parser_get.add_argument('--key', type=str, nargs=1, required=False, help="Use this option to retrieve the value of a specific entry")
     parser_get.add_argument('--account', type=str, nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_get.add_argument('--network', type=str, nargs=1, required=False, help='Optional network parameter, if not specified default is L')
+    parser_get.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
 
     # --------------------------------------------------------------
     parser_account = subparsers.add_parser('account', help="Create remove and manage accounts, type 'lto account --help' for more informations")
     account_subparser = parser_account.add_subparsers(dest='subparser-name-account')
 
     parser_create = account_subparser.add_parser('create', help="Allow to create an account with two optional parameter, --name and --network")
     parser_create.add_argument('--name', required=False, type=str, nargs=1)
-    parser_create.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_create.add_argument('--network', type=str, nargs=1, required=False, help='Optional network parameter, if not specified default is L')
+    parser_create.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
 
     parser_list = account_subparser.add_parser('list', help="Returns the list of accounts stored locally")
-    parser_list.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
-
+    parser_list.add_argument('--network', type=str, nargs=1, required=False, help='Optional network parameter, if not specified default is L')
+    parser_list.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
 
     parser_setDefault = account_subparser.add_parser('set-default', help="Sets the specified account as default account")
     parser_setDefault.add_argument('address', type=str, nargs=1)
     parser_setDefault.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
-
+    parser_setDefault.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
 
     parser_remove = account_subparser.add_parser('remove', help="Remove an account, if not specified, the default account is selected")
     parser_remove.add_argument('address', nargs='?', type=str, help='Insert the desired account address')
     parser_remove.add_argument('--account', type=str, nargs=1, required=False, help="Remove the specified account, the account can be identified by address or name")
     parser_remove.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
-
+    parser_remove.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
 
     parser_show = account_subparser.add_parser('show', help="Show the information about the account, if not specified, the default account is selected")
     parser_show.add_argument('address', nargs='?', type=str, help='Insert the desired account address')
     parser_show.add_argument('--account', type=str, nargs=1, required=False, help="The account can be identified by address or name")
     parser_show.add_argument('--network', type=str, nargs=1, required=False, help='Optional network parameter, if not specified default is L')
-
+    parser_show.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
 
     parser_seed = account_subparser.add_parser('seed', help="Create an account from seed, for more information on how to pipe the seed type 'lto account seed --help")
     parser_seed.add_argument('stdin', nargs='?', type=argparse.FileType('r'), default=sys.stdin, help="Takes the seeds as input: echo 'my seed' | lto account seed")
     parser_seed.add_argument('--name', required=False, type=str, nargs=1)
     parser_seed.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_seed.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
+
     # --------------------------------------------------------------
     parser_balance = subparsers.add_parser('balance', help="Get the account balance, if not specified the default account is selected")
     parser_balance.add_argument('address', nargs='?', type=str, help='Insert the desired account address')
     parser_balance.add_argument('--account', type=str, nargs=1, required=False, help="The account can be identified by address or name. In addition, an address of an account not stored locally can also be used")
     parser_balance.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
-    parser_balance.add_argument('--regular', action='store_true', required=False, help="Use this option to show the regular balance")
-    parser_balance.add_argument('--generating', action='store_true', required=False, help="Use this option to show the generating balance")
-    parser_balance.add_argument('--available', action='store_true', required=False, help="Use this option to show the available balance")
-    parser_balance.add_argument('--effective', action='store_true', required=False, help="Use this option to to show the effective balance")
+    parser_balance.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
+    parser_balance.add_argument('--regular', action='append_const', dest='types', const='regular', required=False, help="Use this option to show the regular balance")
+    parser_balance.add_argument('--available', action='append_const', dest='types', const='available', required=False, help="Use this option to show the available balance")
+    parser_balance.add_argument('--leasing', action='append_const', dest='types', const='leasing', required=False, help="Use this option to show the available balance")
+    parser_balance.add_argument('--unbonding', action='append_const', dest='types', const='unbonding', required=False, help="Use this option to show the available balance")
+    parser_balance.add_argument('--generating', action='append_const', dest='types', const='generating', required=False, help="Use this option to show the generating balance")
+    parser_balance.add_argument('--effective', action='append_const', dest='types', const='effective', required=False, help="Use this option to to show the effective balance")
 
     # --------------------------------------------------------------
     parser_anchor = subparsers.add_parser(name='anchor', help="Create an Anchor Transaction, type 'lto anchor --help' for more information")
     parser_anchor.add_argument('stdin', nargs='?', type=argparse.FileType('r'), default=sys.stdin,  help="Takes the hash as input: echo 'my hahs' | lto anchor")
     parser_anchor.add_argument('--hash', action="append", type=str, nargs=1, help="The hash that will be anchored to the chain")
     parser_anchor.add_argument('--algo', type=str , nargs=1, required=False, help="Use this option to specify an algorithm to hash the input file")
     parser_anchor.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_anchor.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_anchor.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
     parser_anchor.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_anchor.add_argument('--unsigned', action='store_true', required=False, help="Use this option to not sign the transaction. Use in combination with the '--no-broadcast' option")
     parser_anchor.add_argument('--sponsor', type=str , nargs=1, required=False, help="Use this option to select an account for sponsoring the transaction")
     parser_anchor.add_argument('--encoding', type=str , nargs=1, required=False, help="Use this option to provide the hash in a different encoding then hexadecimal (base58 or base64)")
     # --------------------------------------------------------------
     parser_association = subparsers.add_parser('association', help="Create an Association Transaction, type 'lto association --help' for more information")
     association_subparser = parser_association.add_subparsers(dest='subparser-name-association')
 
-    parser_association_incoming = association_subparser.add_parser('incoming', help="Show the incomgin associations related to an account")
-    parser_association_incoming.add_argument('--account', type=str, nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
-    parser_association_incoming.add_argument('--network', type=str, nargs=1, required=False, help='Optional network parameter, if not specified default is L')
-
-    parser_association_outgoing = association_subparser.add_parser('outgoing', help="Show the incomgin associations related to an account")
-    parser_association_outgoing.add_argument('--account', type=str, nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
-    parser_association_outgoing.add_argument('--network', type=str, nargs=1, required=False, help='Optional network parameter, if not specified default is L')
+    parser_association_in = association_subparser.add_parser('in', help="Show the inbound associations related to an account")
+    parser_association_in.add_argument('--account', type=str, nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
+    parser_association_in.add_argument('--network', type=str, nargs=1, required=False, help='Optional network parameter, if not specified default is L')
+    parser_association_in.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
+
+    parser_association_out = association_subparser.add_parser('out', help="Show the outbound associations related to an account")
+    parser_association_out.add_argument('--account', type=str, nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
+    parser_association_out.add_argument('--network', type=str, nargs=1, required=False, help='Optional network parameter, if not specified default is L')
+    parser_association_out.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
 
     parser_association_issue = association_subparser.add_parser('issue', help="Create an association transaction")
     parser_association_issue.add_argument('--subject', type=str, nargs=1, help = "Optional hash argument")
     parser_association_issue.add_argument('--recipient', type=str, nargs=1, required=True, help= 'The recipient')
     parser_association_issue.add_argument('--type', type=int, nargs=1, required=True, help='The association type')
     parser_association_issue.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_association_issue.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_association_issue.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
     parser_association_issue.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_association_issue.add_argument('--unsigned', action='store_true', required=False, help="Use this option to not sign the transaction. Use in combination with the '--no-broadcast' option")
     parser_association_issue.add_argument('--sponsor', type=str , nargs=1, required=False, help="Use this option to select an account for sponsoring the transaction")
 
-
     parser_association_revoke = association_subparser.add_parser('revoke', help="Create a revoke association transaction")
     parser_association_revoke.add_argument('--subject', type=str, nargs=1, help = "Optional hash argument")
     parser_association_revoke.add_argument('--recipient', type=str, nargs=1, required=True, help= 'The recipient')
     parser_association_revoke.add_argument('--type', type=int, nargs=1, required=True, help='The association type')
     parser_association_revoke.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_association_revoke.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_association_revoke.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
     parser_association_revoke.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_association_revoke.add_argument('--unsigned', action='store_true', required=False, help="Use this option to not sign the transaction. Use in combination with the '--no-broadcast' option")
     parser_association_revoke.add_argument('--sponsor', type=str , nargs=1, required=False, help="Use this option to select an account for sponsoring the transaction")
+
     # --------------------------------------------------------------
     parser_broadcast = subparsers.add_parser('broadcast', help="Takes as input a transaction (signed or unsigned) and broadcast it to the network, type 'lto broadcast --help' for more informations")
     parser_broadcast.add_argument('stdin', nargs='?', type=argparse.FileType('r'), default=sys.stdin, help="Takes the json transaction as input: echo '$TX_JSON' | lto broadcast")
     parser_broadcast.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored for signing the transaction. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_broadcast.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_broadcast.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
     parser_broadcast.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_broadcast.add_argument('--unsigned', action='store_true', required=False, help="Use this option to ensure the transaction is already signed, and will not be signed by the CLI wallett")
-    # --------------------------------------------------------------
+
     # --------------------------------------------------------------
     parser_script = subparsers.add_parser('script', help="Set a script for the account, type 'lto script --help' for more informations")
     parser_script.add_argument('stdin', nargs='?', type=argparse.FileType('r'), default=sys.stdin, help="Takes the ride script as input: echo '$SCRIPT' | lto script")
     parser_script.add_argument('--account', type=str, nargs=1, required=False, help="Use this option to select one of the accounts previously stored for signing the transaction. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_script.add_argument('--network', type=str, nargs=1, required=False, help='Optional network parameter, if not specified default is L')
     parser_script.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_script.add_argument('--unsigned', action='store_true', required=False, help="Use this option to ensure the transaction is already signed, and will not be signed by the CLI wallett")
+
     # --------------------------------------------------------------
     parser_lease = subparsers.add_parser('lease', help="Create a Lease Transaction, type 'lto lease --help' for more information")
     lease_subparser = parser_lease.add_subparsers(dest='subparser-name-lease')
 
     parser_lease_create = lease_subparser.add_parser('create', help='To create a lease, --recipient and --amount are required')
     parser_lease_create.add_argument('--recipient', type=str, nargs=1, required=True)
     parser_lease_create.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_lease_create.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_lease_create.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
     parser_lease_create.add_argument('--amount', type=float, nargs=1, required=True)
     parser_lease_create.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_lease_create.add_argument('--unsigned', action='store_true', required=False, help="Use this option to not sign the transaction. Use in combination with the '--no-broadcast' option")
     parser_lease_create.add_argument('--sponsor', type=str , nargs=1, required=False, help="Use this option to select an account for sponsoring the transaction")
 
     parser_lease_cancel = lease_subparser.add_parser('cancel', help="To cancel a lease --leaseId is required")
     parser_lease_cancel.add_argument('--leaseId', type=str, nargs=1, required=True)
     parser_lease_cancel.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_lease_cancel.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_lease_cancel.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
     parser_lease_cancel.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_lease_cancel.add_argument('--unsigned', action='store_true', required=False, help="Use this option to not sign the transaction. Use in combination with the '--no-broadcast' option")
     parser_lease_cancel.add_argument('--sponsor', type=str , nargs=1, required=False, help="Use this option to select an account for sponsoring the transaction")
 
-    parser_lease_incoming = lease_subparser.add_parser('incoming', help="Returns the list of leasing that the user has conceded")
-    parser_lease_incoming.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
-    parser_lease_incoming.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
-
-    parser_lease_list_outgoing = lease_subparser.add_parser('outgoing', help="Returns the list of leasing in favor of the user")
-    parser_lease_list_outgoing.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
-    parser_lease_list_outgoing.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_lease_in = lease_subparser.add_parser('in', help="Returns the list of leasing that the user has conceded")
+    parser_lease_in.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
+    parser_lease_in.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_lease_in.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
+
+    parser_lease_list_out = lease_subparser.add_parser('out', help="Returns the list of leasing in favor of the user")
+    parser_lease_list_out.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
+    parser_lease_list_out.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_lease_list_out.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
+
     # --------------------------------------------------------------
     parser_massTransfer = subparsers.add_parser('mass-transfer', help="Create a Mass-Transfer Transaction, type 'lto mass-transfer --help' for more information")
     parser_massTransfer.add_argument('stdin', nargs='?', type=argparse.FileType('r'),
                                      default=sys.stdin, help="Takes the transfers as input: echo 'address1:amount address2:amount' | lto mass-transfer")
     parser_massTransfer.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_massTransfer.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_massTransfer.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
     parser_massTransfer.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_massTransfer.add_argument('--unsigned', action='store_true', required=False, help="Use this option to not sign the transaction. Use in combination with the '--no-broadcast' option")
     parser_massTransfer.add_argument('--sponsor', type=str , nargs=1, required=False, help="Use this option to select an account for sponsoring the transaction")
+
     # --------------------------------------------------------------
     parser_node = subparsers.add_parser('node', help="Allows to performs operation regarding the node, type 'lto node --help' for more information")
     node_subparser = parser_node.add_subparsers(dest='subparser-name-node')
 
     parser_node_set = node_subparser.add_parser('set', help="Allows to set the preferred node to connect to and an optional network parameter, type 'lto node set --help' for more information")
     parser_node_set.add_argument('url', type=str, nargs=1, help="url of the node to connect to")
     parser_node_set.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_node_set.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
 
     parser_node_show = node_subparser.add_parser('show', help="Displays the node url, type 'lto node show --help' for more information")
     parser_node_show.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_node_show.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
 
     parser_node_status = node_subparser.add_parser('status', help="Allows to show the status of the node, type 'lto node status --help' for more information")
     parser_node_status.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
-
-
-
-
+    parser_node_status.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
 
     # --------------------------------------------------------------
     parser_sponsorship = subparsers.add_parser('sponsorship', help="Create a Sponsorship Transaction, type 'lto sponsorship --help' for more information")
     sponsorship_subparser = parser_sponsorship.add_subparsers(dest='subparser-name-sponsorship')
 
-
     parser_sponsorship_create = sponsorship_subparser.add_parser('create',  help='To create a sponsorhip the --recipient is required')
     parser_sponsorship_create.add_argument('--recipient', type=str, nargs=1, required=True)
     parser_sponsorship_create.add_argument('--account', type=str, nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_sponsorship_create.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_sponsorship_create.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
     parser_sponsorship_create.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_sponsorship_create.add_argument('--unsigned', action='store_true', required=False, help="Use this option to not sign the transaction. Use in combination with the '--no-broadcast' option")
     parser_sponsorship_create.add_argument('--sponsor', type=str , nargs=1, required=False, help="Use this option to select an account for sponsoring the transaction")
 
-
     parser_sponsorship_cancel = sponsorship_subparser.add_parser('cancel', help='To cancel a sponsorhip the --recipient is required')
     parser_sponsorship_cancel.add_argument('--recipient', type=str, nargs=1, required = True)
     parser_sponsorship_cancel.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_sponsorship_cancel.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_sponsorship_cancel.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
     parser_sponsorship_cancel.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_sponsorship_cancel.add_argument('--unsigned', action='store_true', required=False, help="Use this option to not sign the transaction. Use in combination with the '--no-broadcast' option")
     parser_sponsorship_cancel.add_argument('--sponsor', type=str , nargs=1, required=False, help="Use this option to select an account for sponsoring the transaction")
 
-    # The end-point needs to be added
-    #parser_sponsorship_list = sponsorship_subparser.add_parser('list', help="Returns the list of accounts that the user is sponsoring")
-    #parser_sponsorship_list.add_argument('--account', type=str, nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
-
-    parser_sponsorship_outgoing = sponsorship_subparser.add_parser('outgoing', help="Returns the list of accounts that are sponsoring the user")
-    parser_sponsorship_outgoing.add_argument('--account', type=str, nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
-    parser_sponsorship_outgoing.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_sponsorship_in = sponsorship_subparser.add_parser('in', help="Returns the list of accounts that are sponsoring the user")
+    parser_sponsorship_in.add_argument('--account', type=str, nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
+    parser_sponsorship_in.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_sponsorship_in.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
+
     # --------------------------------------------------------------
     parser_transfer = subparsers.add_parser('transfer', help="Create a Transfer Transaction, type 'lto transfer --help' for more information")
     parser_transfer.add_argument('--recipient', type=str, nargs=1, required=True)
     parser_transfer.add_argument('--amount', type=float, nargs=1, required=True)
     parser_transfer.add_argument('--account', type=str , nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_transfer.add_argument('--network', type=str, nargs=1, required=False, help ='Optional network parameter, if not specified default is L')
+    parser_transfer.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
     parser_transfer.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_transfer.add_argument('--unsigned', action='store_true', required=False, help="Use this option to not sign the transaction. Use in combination with the '--no-broadcast' option")
     parser_transfer.add_argument('--sponsor', type=str , nargs=1, required=False, help="Use this option to select an account for sponsoring the transaction")
+
     # --------------------------------------------------------------
     parser_burn = subparsers.add_parser('burn', help="Create a Burn Transaction, type 'lto burn --help' for more informations")
     parser_burn.add_argument('--amount', type=float, nargs=1, required=True, help="Specify the amounts of token to burn, 1 equals 1 LTO")
     parser_burn.add_argument('--account', type=str, nargs=1, required=False, help="Use this option to select one of the accounts previously stored. The account can be referenced by name or address, if this option is omitted, the default account is used")
     parser_burn.add_argument('--network', type=str, nargs=1, required=False,  help='Optional network parameter, if not specified default is L')
+    parser_burn.add_argument('--testnet', '-T', action='store_const', dest='network', const='T', required=False, help='Short for --network=T')
     parser_burn.add_argument('--no-broadcast', action='store_true', required=False, help="Use this option to not broadcast the transaction to the node")
     parser_burn.add_argument('--unsigned', action='store_true', required=False, help="Use this option to not sign the transaction. Use in combination with the '--no-broadcast' option")
     parser_burn.add_argument('--sponsor', type=str, nargs=1, required=False, help="Use this option to select an account for sponsoring the transaction")
 
-    process_args(parser.parse_args(), parser)
+    # --------------------------------------------------------------
+    try:    
+      process_args(parser.parse_args(), parser, subparsers)
+    except Exception as e:
+      parser.error(e)
+
 
-def process_args(name_space, parser):
+def process_args(name_space, parser, subparsers):
+    subcommand = vars(name_space)['subparser-name']
+    subparser = subparsers.choices[subcommand] if subcommand else None
 
     if vars(name_space)['version']:
         print('Version:', version('lto_cli'))
 
-    elif vars(name_space)['subparser-name'] == 'account':
-        account.func(name_space, parser)
+    elif subcommand == 'account':
+        account.func(name_space, parser, subparser)
 
-    elif vars(name_space)['subparser-name'] == 'anchor':
+    elif subcommand == 'anchor':
         anchor.func(name_space, parser)
 
-    elif vars(name_space)['subparser-name'] == 'transfer':
+    elif subcommand == 'transfer':
         transfer.func(name_space, parser)
 
-    elif vars(name_space)['subparser-name'] == 'burn':
+    elif subcommand == 'burn':
         burn.func(name_space, parser)
 
-    elif vars(name_space)['subparser-name'] == 'sponsorship':
-        sponsorship.func(name_space, parser)
+    elif subcommand == 'sponsorship':
+        sponsorship.func(name_space, parser, subparser)
 
-    elif vars(name_space)['subparser-name'] == 'association':
-        association.func(name_space, parser)
+    elif subcommand == 'association':
+        association.func(name_space, parser, subparser)
 
-    elif vars(name_space)['subparser-name'] == 'mass-transfer':
+    elif subcommand == 'mass-transfer':
         mass_transfer.func(name_space, parser)
 
-    elif vars(name_space)['subparser-name'] == 'lease':
-        leasing.func(name_space, parser)
+    elif subcommand == 'lease':
+        leasing.func(name_space, parser, subparser)
 
-    elif vars(name_space)['subparser-name'] == 'node':
-        node.func(name_space, parser)
+    elif subcommand == 'node':
+        node.func(name_space, parser, subparser)
 
-    elif vars(name_space)['subparser-name'] == 'broadcast':
+    elif subcommand == 'broadcast':
         broadcast.func(name_space, parser)
 
-    elif vars(name_space)['subparser-name'] == 'script':
+    elif subcommand == 'script':
         script.func(name_space, parser)
 
-    elif vars(name_space)['subparser-name'] == 'balance':
+    elif subcommand == 'balance':
         balance.func(name_space, parser)
 
-    elif vars(name_space)['subparser-name'] == 'data':
-        data.func(name_space, parser)
+    elif subcommand == 'data':
+        data.func(name_space, parser, subparser)
 
     else:
         parser.print_help()
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `lto-cli-1.2.2/src/lto_cli/commands/account.py` & `lto-cli-1.2.3/src/lto_cli/commands/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from lto.accounts.ed25519.account_factory_ed25519 import AccountFactoryED25519 as AccountFactory
 from lto_cli import config
 from lto_cli import handle_default as handle
 
 
-def func(name_space, parser):
+def func(name_space, parser, subparser):
     if not vars(name_space)['subparser-name-account']:
-        parser.error('No option selected, type lto account --help for instructions')
+        subparser.print_help()
+        return
 
     chain_id = name_space.network[0] if name_space.network else 'L'
     chain_id = chain_id.upper() if not chain_id.isupper() else chain_id
 
     if vars(name_space)['subparser-name-account'] == 'create':
         if not (chain_id.isalpha() and len(chain_id) == 1):
             parser.error('The --network parameter accepts only CHAR type')
```

### Comparing `lto-cli-1.2.2/src/lto_cli/commands/anchor.py` & `lto-cli-1.2.3/src/lto_cli/commands/anchor.py`

 * *Files identical despite different names*

### Comparing `lto-cli-1.2.2/src/lto_cli/commands/association.py` & `lto-cli-1.2.3/src/lto_cli/commands/association.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 from lto_cli import handle_default as handle
 from lto.transactions.association import Association
 from lto.transactions.revoke_association import RevokeAssociation
 import json
 from lto.crypto import decode
 
 
-def func(name_space, parser):
-    if vars(name_space)['subparser-name-association']:
-        chain_id = handle.check(name_space.network[0], parser) if name_space.network else 'L'
-        account_name = vars(name_space)['account'][0] if vars(name_space)['account'] else ''
-        if vars(name_space)['subparser-name-association'] in ['issue','revoke']:
-            sponsor = vars(name_space)['sponsor'][0] if vars(name_space)['sponsor'] else None
-            association_type = name_space.type[0]
-            recipient = name_space.recipient[0]
-            subject = ''
-            if name_space.subject:
-                subject = name_space.subject[0]
-            if vars(name_space)['subparser-name-association'] == 'issue':
-                transaction = Association(recipient=recipient, association_type=association_type, subject=decode(subject, "hex"))
-                if vars(name_space)['unsigned'] is False:
+def func(name_space, parser, subparser):
+    if not vars(name_space)['subparser-name-association']:
+        subparser.print_help()
+        return
+        
+    chain_id = handle.check(name_space.network[0], parser) if name_space.network else 'L'
+    account_name = vars(name_space)['account'][0] if vars(name_space)['account'] else ''
+    if vars(name_space)['subparser-name-association'] in ['issue','revoke']:
+        sponsor = vars(name_space)['sponsor'][0] if vars(name_space)['sponsor'] else None
+        association_type = name_space.type[0]
+        recipient = name_space.recipient[0]
+        subject = ''
+        if name_space.subject:
+            subject = name_space.subject[0]
+        if vars(name_space)['subparser-name-association'] == 'issue':
+            transaction = Association(recipient=recipient, association_type=association_type, subject=decode(subject, "hex"))
+            if vars(name_space)['unsigned'] is False:
+                transaction.sign_with(handle.get_account(chain_id, parser, account_name))
+                if sponsor:
+                    transaction.sponsor_with(handle.get_account(chain_id, parser, sponsor))
+                if vars(name_space)['no_broadcast'] is False:
+                    transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
+            elif vars(name_space)['no_broadcast'] is False:
+                parser.error(
+                    "Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto association issue --help' for more informations ")
+        else:  # revoke case
+            transaction = RevokeAssociation(recipient=recipient, association_type=association_type, subject=decode(subject, "hex"))
+            if vars(name_space)['unsigned'] is False:
+                if vars(name_space)['account']:
                     transaction.sign_with(handle.get_account(chain_id, parser, account_name))
                     if sponsor:
                         transaction.sponsor_with(handle.get_account(chain_id, parser, sponsor))
-                    if vars(name_space)['no_broadcast'] is False:
-                        transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
-                elif vars(name_space)['no_broadcast'] is False:
-                    parser.error(
-                        "Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto association issue --help' for more informations ")
-            else:  # revoke case
-                transaction = RevokeAssociation(recipient=recipient, association_type=association_type, subject=decode(subject, "hex"))
-                if vars(name_space)['unsigned'] is False:
-                    if vars(name_space)['account']:
-                        transaction.sign_with(handle.get_account(chain_id, parser, account_name))
-                        if sponsor:
-                            transaction.sponsor_with(handle.get_account(chain_id, parser, sponsor))
-                    if vars(name_space)['no_broadcast'] is False:
-                        transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
-                elif vars(name_space)['no_broadcast'] is False:
-                    parser.error(
-                        "Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto association revoke --help' for more informations ")
-            handle.pretty_print(transaction)
-        else:
-            node = handle.get_node(chain_id, parser)
-            account = handle.get_account(chain_id, parser, account_name)
+                if vars(name_space)['no_broadcast'] is False:
+                    transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
+            elif vars(name_space)['no_broadcast'] is False:
+                parser.error(
+                    "Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto association revoke --help' for more informations ")
+        handle.pretty_print(transaction)
+    else:
+        node = handle.get_node(chain_id, parser)
+        account = handle.get_account(chain_id, parser, account_name)
 
-            if vars(name_space)['subparser-name-association'] == 'incoming':
-                list = node.association_list(account.address)['incoming']
-                for association in list:
-                    print(json.dumps(association, indent=2))
-            else:  # outgoing
-                list = node.association_list(account.address)['outgoing']
-                for association in list:
-                    print(json.dumps(association, indent=2))
+        if vars(name_space)['subparser-name-association'] == 'in':
+            list = node.association_list(account.address)['incoming']
+            for association in list:
+                print(json.dumps(association, indent=2))
+        else:
+            list = node.association_list(account.address)['outgoing']
+            for association in list:
+                print(json.dumps(association, indent=2))
 
-    else:
-        parser.error('Type lto association --help for instructions')
```

### Comparing `lto-cli-1.2.2/src/lto_cli/commands/broadcast.py` & `lto-cli-1.2.3/src/lto_cli/commands/broadcast.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,7 @@
                 parser.error(
                     "Transaction needs to be signed before broadcasting, type 'lto broadcast --help' for instruction")
             else:
                 transaction = transaction.broadcast_to(node)
 
     handle.pretty_print(transaction)
 
-
```

### Comparing `lto-cli-1.2.2/src/lto_cli/commands/burn.py` & `lto-cli-1.2.3/src/lto_cli/commands/burn.py`

 * *Files identical despite different names*

### Comparing `lto-cli-1.2.2/src/lto_cli/commands/data.py` & `lto-cli-1.2.3/src/lto_cli/commands/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,17 @@
         if not value:
             print('No data found for {}'.format(address))
         else:
             for x in value:
                 print(x)
 
 
-def func(name_space, parser):
+def func(name_space, parser, subparser):
     if vars(name_space)['subparser-name-data'] == 'set':
         data_set(name_space, parser)
 
     elif vars(name_space)['subparser-name-data'] == 'get':
         data_get(name_space, parser)
 
     else:
-        parser.error('Type lto data --help for instructions')
+        subparser.print_help()
+
```

### Comparing `lto-cli-1.2.2/src/lto_cli/commands/leasing.py` & `lto-cli-1.2.3/src/lto_cli/commands/leasing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 from lto_cli import handle_default as handle
 from lto.transactions.lease import Lease
 from lto.transactions.cancel_lease import CancelLease
 
 
-def func(name_space, parser):
-    if vars(name_space)['subparser-name-lease']:
-        chain_id = handle.check(name_space.network[0], parser) if name_space.network else 'L'
-        account_name = vars(name_space)['account'][0] if vars(name_space)['account'] else ''
-
-        if vars(name_space)['subparser-name-lease'] == 'create':
-            sponsor = vars(name_space)['sponsor'][0] if vars(name_space)['sponsor'] else None
-            transaction = Lease(recipient=name_space.recipient[0], amount=int(name_space.amount[0] * 100000000))
-            if vars(name_space)['unsigned'] is False:
-                transaction.sign_with(handle.get_account(chain_id, parser, account_name))
-                if sponsor:
-                    transaction.sponsor_with(handle.get_account(chain_id, parser, sponsor))
-                if vars(name_space)['no_broadcast'] is False:
-                    transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
-            elif vars(name_space)['no_broadcast'] is False:
-                parser.error(
-                    "Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto lease create --help' for more informations ")
-            handle.pretty_print(transaction)
-
-        elif vars(name_space)['subparser-name-lease'] == 'cancel':
-            sponsor = vars(name_space)['sponsor'][0] if vars(name_space)['sponsor'] else None
-            transaction = CancelLease(lease_id=name_space.leaseId[0])
-            if vars(name_space)['unsigned'] is False:
-                transaction.sign_with(handle.get_account(chain_id, parser, account_name))
-                if sponsor:
-                    transaction.sponsor_with(handle.get_account(chain_id, parser, sponsor))
-                if vars(name_space)['no_broadcast'] is False:
-                    transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
-            elif vars(name_space)['no_broadcast'] is False:
-                parser.error(
-                    "Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto lease cancel --help' for more informations ")
-            handle.pretty_print(transaction)
-
-        elif vars(name_space)['subparser-name-lease'] == 'incoming':  # The lease that I'm giving
-            node = handle.get_node(chain_id, parser)
-            address = handle.get_account(chain_id, parser, account_name).address
-            value = node.lease_list(address)
-            flag = 0
-            for x in value:
-                if x['sender'] == address:  # outbound
-                    print(x['sender'], ':', x['amount'] /100000000)
-                    flag +=1
-            if flag == 0:
-                print("No incoming lease found")
-
-        else:  # outgoing : The lease that I've received
-            node = handle.get_node(chain_id, parser)
-            address = handle.get_account(chain_id, parser, account_name).address
-            value = node.lease_list(address)
-            flag = 0
-            for x in value:
-                if x['recipient'] == address:  # inbound
-                    print(x['sender'], ':', x['amount'] / 100000000)
-                    flag +=1
-            if flag == 0:
-                print("No outgoing lease found")
+def func(name_space, parser, subparser):
+    if not vars(name_space)['subparser-name-lease']:
+        subparser.print_help()
+        return
+    
+    chain_id = handle.check(name_space.network[0], parser) if name_space.network else 'L'
+    account_name = vars(name_space)['account'][0] if vars(name_space)['account'] else ''
+
+    if vars(name_space)['subparser-name-lease'] == 'create':
+        sponsor = vars(name_space)['sponsor'][0] if vars(name_space)['sponsor'] else None
+        transaction = Lease(recipient=name_space.recipient[0], amount=int(name_space.amount[0] * 100000000))
+        if vars(name_space)['unsigned'] is False:
+            transaction.sign_with(handle.get_account(chain_id, parser, account_name))
+            if sponsor:
+                transaction.sponsor_with(handle.get_account(chain_id, parser, sponsor))
+            if vars(name_space)['no_broadcast'] is False:
+                transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
+        elif vars(name_space)['no_broadcast'] is False:
+            parser.error(
+                "Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto lease create --help' for more informations ")
+        handle.pretty_print(transaction)
+
+    elif vars(name_space)['subparser-name-lease'] == 'cancel':
+        sponsor = vars(name_space)['sponsor'][0] if vars(name_space)['sponsor'] else None
+        transaction = CancelLease(lease_id=name_space.leaseId[0])
+        if vars(name_space)['unsigned'] is False:
+            transaction.sign_with(handle.get_account(chain_id, parser, account_name))
+            if sponsor:
+                transaction.sponsor_with(handle.get_account(chain_id, parser, sponsor))
+            if vars(name_space)['no_broadcast'] is False:
+                transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
+        elif vars(name_space)['no_broadcast'] is False:
+            parser.error(
+                "Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto lease cancel --help' for more informations ")
+        handle.pretty_print(transaction)
+
+    elif vars(name_space)['subparser-name-lease'] == 'out':
+        node = handle.get_node(chain_id, parser)
+        address = handle.get_account(chain_id, parser, account_name).address
+        value = node.lease_list(address)
+        flag = 0
+        for x in value:
+            if x['sender'] == address:  # outbound
+                print(x['sender'], ':', x['amount'] /100000000)
+                flag +=1
+        if flag == 0:
+            print("No outbound leases")
+
+    else:  # out
+        node = handle.get_node(chain_id, parser)
+        address = handle.get_account(chain_id, parser, account_name).address
+        value = node.lease_list(address)
+        flag = 0
+        for x in value:
+            if x['recipient'] == address:  # inbound
+                print(x['sender'], ':', x['amount'] / 100000000)
+                flag +=1
+        if flag == 0:
+            print("No inbound leases")
 
-    else:
-        parser.error('Type lto lease --help for instructions')
```

### Comparing `lto-cli-1.2.2/src/lto_cli/commands/mass_transfer.py` & `lto-cli-1.2.3/src/lto_cli/commands/mass_transfer.py`

 * *Files identical despite different names*

### Comparing `lto-cli-1.2.2/src/lto_cli/commands/node.py` & `lto-cli-1.2.3/src/lto_cli/commands/node.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from lto_cli import config
 from lto_cli import handle_default as handle
 
-def func(name_space, parser):
+def func(name_space, parser, subparser):
     if vars(name_space)['subparser-name-node'] == 'show':
         chain_id = handle.check(name_space.network[0], parser) if name_space.network else 'L'
         print(handle.get_node(chain_id, parser).url)
     elif vars(name_space)['subparser-name-node'] == 'set':
         config.set_node(name_space, parser)
     elif vars(name_space)['subparser-name-node'] == 'status':
         chain_id = handle.check(name_space.network[0], parser) if name_space.network else 'L'
@@ -14,9 +14,9 @@
 
         print('Blockchain Height  : ', status['blockchainHeight'])
         print('State Height       : ', status['stateHeight'])
         print('Updated Timestamp  : ', status['updatedTimestamp'])
         print('Updated Date       : ', status['updatedDate'])
 
     else:
-        parser.error('Type "lto node --help" for instructions')
-    #config.set_node(name_space, parser)
+        subparser.print_help()
+
```

### Comparing `lto-cli-1.2.2/src/lto_cli/commands/script.py` & `lto-cli-1.2.3/src/lto_cli/commands/script.py`

 * *Files identical despite different names*

### Comparing `lto-cli-1.2.2/src/lto_cli/commands/sponsorship.py` & `lto-cli-1.2.3/src/lto_cli/commands/sponsorship.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 from lto_cli import handle_default as handle
 from lto.transactions.sponsorship import Sponsorship
 from lto.transactions.cancel_sponsorship import CancelSponsorship
 
 
-def func(name_space,parser):
-    if vars(name_space)['subparser-name-sponsorship']:
-        chain_id = handle.check(name_space.network[0], parser) if name_space.network else 'L'
-        account_name = vars(name_space)['account'][0] if vars(name_space)['account'] else ''
-
-        if vars(name_space)['subparser-name-sponsorship'] == 'create':
-            sponsor = vars(name_space)['sponsor'][0] if vars(name_space)['sponsor'] else None
-            transaction = Sponsorship(name_space.recipient[0])
-            if vars(name_space)['unsigned'] is False:
-                transaction.sign_with(handle.get_account(chain_id, parser, account_name))
-                if sponsor:
-                    transaction.sponsor_with(handle.get_account(chain_id, parser, sponsor))
-                if vars(name_space)['no_broadcast'] is False:
-                    transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
-            elif vars(name_space)['no_broadcast'] is False:
-                parser.error(
-                    "Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto sponsorship create --help' for more informations ")
-            handle.pretty_print(transaction)
-
-        elif vars(name_space)['subparser-name-sponsorship'] == 'cancel':
-            sponsor = vars(name_space)['sponsor'][0] if vars(name_space)['sponsor'] else None
-            transaction = CancelSponsorship(name_space.recipient[0])
-            if vars(name_space)['unsigned'] is False:
-                transaction.sign_with(handle.get_account(chain_id, parser, account_name))
-                if sponsor:
-                    transaction.sponsor_with(handle.get_account(chain_id, parser, sponsor))
-                if vars(name_space)['no_broadcast'] is False:
-                    transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
-            elif vars(name_space)['no_broadcast'] is False:
-                parser.error(
-                    "Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto sponsorship cancel --help' for more informations ")
-            handle.pretty_print(transaction)
-
-        elif vars(name_space)['subparser-name-sponsorship'] == 'list':
-            pass
-
-        else:  # outgoing
-            node = handle.get_node(chain_id, parser)
-            address = handle.get_account(chain_id, parser, account_name).address
-            value = node.sponsorship_list(address)
-            if value['sponsor']:
-                for x in value['sponsor']:
-                    print(x)
-            else:
-                print('No outgoing sponsorships found')
-
-    else:
-        parser.error('Type lto sponsorship --help for instructions')
-
-
+def func(name_space, parser, subparser):
+    if not vars(name_space)['subparser-name-sponsorship']:
+        subparser.print_help()
+        return
+        
+    chain_id = handle.check(name_space.network[0], parser) if name_space.network else 'L'
+    account_name = vars(name_space)['account'][0] if vars(name_space)['account'] else ''
+
+    if vars(name_space)['subparser-name-sponsorship'] == 'create':
+        sponsor = vars(name_space)['sponsor'][0] if vars(name_space)['sponsor'] else None
+        transaction = Sponsorship(name_space.recipient[0])
+        if vars(name_space)['unsigned'] is False:
+            transaction.sign_with(handle.get_account(chain_id, parser, account_name))
+            if sponsor:
+                transaction.sponsor_with(handle.get_account(chain_id, parser, sponsor))
+            if vars(name_space)['no_broadcast'] is False:
+                transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
+        elif vars(name_space)['no_broadcast'] is False:
+            parser.error(
+                "Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto sponsorship create --help' for more informations ")
+        handle.pretty_print(transaction)
+
+    elif vars(name_space)['subparser-name-sponsorship'] == 'cancel':
+        sponsor = vars(name_space)['sponsor'][0] if vars(name_space)['sponsor'] else None
+        transaction = CancelSponsorship(name_space.recipient[0])
+        if vars(name_space)['unsigned'] is False:
+            transaction.sign_with(handle.get_account(chain_id, parser, account_name))
+            if sponsor:
+                transaction.sponsor_with(handle.get_account(chain_id, parser, sponsor))
+            if vars(name_space)['no_broadcast'] is False:
+                transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
+        elif vars(name_space)['no_broadcast'] is False:
+            parser.error(
+                "Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto sponsorship cancel --help' for more informations ")
+        handle.pretty_print(transaction)
+
+    elif vars(name_space)['subparser-name-sponsorship'] == 'out':
+        pass
+
+    else:  # inbound
+        node = handle.get_node(chain_id, parser)
+        address = handle.get_account(chain_id, parser, account_name).address
+        value = node.sponsorship_list(address)
+        if value['sponsor']:
+            for x in value['sponsor']:
+                print(x)
+        else:
+            print('Not sponsered')
```

### Comparing `lto-cli-1.2.2/src/lto_cli/commands/transfer.py` & `lto-cli-1.2.3/src/lto_cli/commands/transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,10 +13,12 @@
 
     if vars(name_space)['unsigned'] is False:
         transaction.sign_with(handle.get_account(chain_id, parser, account_name))
         if sponsor:
             transaction.sponsor_with(handle.get_account(chain_id, parser, sponsor))
         if vars(name_space)['no_broadcast'] is False:
             transaction = transaction.broadcast_to(handle.get_node(chain_id, parser))
+    
     elif vars(name_space)['no_broadcast'] is False:
         parser.error("Use the '--unsigned' option only in combination with the '--no-broadcast' option. Type 'lto transaction --help' for more informations ")
-    handle.pretty_print(transaction)
+    
+    handle.pretty_print(transaction)
```

### Comparing `lto-cli-1.2.2/src/lto_cli/config.py` & `lto-cli-1.2.3/src/lto_cli/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,30 +19,30 @@
     if not sec_name:
         sec_name = account.address
 
     config = ConfigParser()
     config.read(Path.joinpath(relative_path, 'accounts.ini'))
 
     if find_account_in_config(config=config, address=account.address, name=sec_name):
-        parser.error("An account with the same id is already present, type 'lto accounts create --help' for instructions or 'lto accounts list' to visualize the previously stored accounts")
+        parser.error("An account with the same id is already present, type 'lto account create --help' for instructions or 'lto account list' to visualize the previously stored accounts")
 
     config.add_section(sec_name)
     config.set(sec_name, 'Address', account.address)
     config.set(sec_name, 'Public_key', base58.b58encode(account.public_key.__bytes__()))
     config.set(sec_name, 'Private_key', base58.b58encode(account.private_key.__bytes__()))
     config.set(sec_name, 'Seed', account.seed)
     config.write(open(Path.joinpath(relative_path, 'accounts.ini'), 'w'))
     write_default_account(account, chain_id)
 
 
 def find_account_in_config(config, address='', name=''):
     for sec in config.sections():
         if address == config.get(sec, 'address') or name == sec or name == config.get(sec, 'address'):
-            seed = config.get(sec, 'seed')
-            private_key = config.get(sec, 'private_key')
+            seed = config.get(sec, 'seed', fallback = '')
+            private_key = config.get(sec, 'private_key', fallback = '')
             public_key = config.get(sec, 'public_key')
             address = config.get(sec, 'address')
             return [seed, private_key, public_key, address]
     return False
 
 
 #  Change is set to false, so it won't change the predetermined default account
@@ -68,15 +68,15 @@
     config.write(open(local_path, 'w'))
 
 
 def list_accounts(chain_id, parser):
     list = []
     local_path = Path.joinpath(path, chain_id, "accounts.ini")
     if not os.path.exists(local_path):
-        parser.error("No account found for {} network, type 'lto accounts --help' for instructions".format(chain_id))
+        parser.error("No account found for {} network, type 'lto account --help' for instructions".format(chain_id))
     else:
         config = ConfigParser()
         config.read(local_path)
         for section in config.sections():
             list.append([section, config.get(section, 'address')])
     return list
 
@@ -108,26 +108,26 @@
         os.mkdir(Path.joinpath(path, dir))
 
 
 def set_default_accounts(chain_id, name, parser):
     config = get_config_from_chain_id(chain_id)
     value = find_account_in_config(config, name=name)
     if not value:
-        parser.error("No account found with this id, type 'lto accounts create --help' for instructions or 'lto accounts list' to visualize the previously stored accounts")
+        parser.error("No account found with this id, type 'lto account create --help' for instructions or 'lto account list' to visualize the previously stored accounts")
 
     account = Account(seed=value[0], private_key=value[1], public_key=value[2], address=value[3])
     write_default_account(account, chain_id, change=True)
 
 
 def remove_account(chain_id, name, parser):
     config = get_config_from_chain_id(chain_id)
     value = find_account_in_config(config, name=name)
 
     if not value:
-        parser.error("No account found with this id, type 'lto accounts remove --help' for instructions or 'lto accounts list' to visualize the previously stored accounts")
+        parser.error("No account found with this id, type 'lto account remove --help' for instructions or 'lto account list' to visualize the previously stored accounts")
 
     config.remove_section(get_section_name_from_address(config, value[3]))
     config.write(open(Path.joinpath(path, chain_id, 'accounts.ini'), 'w'))
     remove_default_account(value[3], chain_id)
     delete_if_empty(Path.joinpath(path, chain_id, 'accounts.ini'))
 
 
@@ -164,29 +164,28 @@
     config.write(open(Path.joinpath(path, chain_id, 'config.ini'), 'w'))
 
 
 def show(chain_id, id, parser):
     config = get_config_from_chain_id(chain_id)
     value = find_account_in_config(config, address=id, name=id)
     if not value:
-        parser.error("No matching account fo {}, type 'lto accounts --help' for instructions")
+        parser.error("No matching account fo {}, type 'lto account --help' for instructions")
 
-    print('Name    : ', id) if id != value[3] else None
-    print('Address : ', value[3])
-    print('Sign    :')
-    print('   SecretKey   : ', value[1])
-    print('   Public_key  : ', value[2])
-    print('Seed    : ', value[0])
+    print('Name        :', id) if id != value[3] else None
+    print('Address     :', value[3])
+    print('Public key  :', value[2])
+    print('Private key :', value[1] or '[unknown]')
+    print('Seed        :', value[0] or '[unknown]')
 
 
 def get_config_from_chain_id(chain_id):
     config_file = Path.joinpath(path, chain_id, 'accounts.ini')
     config = ConfigParser()
     config.read(config_file)
     return config
 
 def get_section_name_from_address(config, address):
     sections = config.sections()
     for sec in sections:
         if config.get(sec, 'address') == address:
             return sec
-    return None
+    return None
```

### Comparing `lto-cli-1.2.2/src/lto_cli/handle_default.py` & `lto-cli-1.2.3/src/lto_cli/handle_default.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,22 +33,28 @@
 
     if not os.path.exists(local_path):
         parser.error("No account found for {} network, type 'lto account --help' for instructions".format(chain_id))
 
     config = ConfigParser()
     config.read(local_path)
     if name:
-        if name in config.sections():
+        if not name in config.sections():
+            parser.error("No account found for {} network with name {}, use 'lto account list' to see all accounts".format(chain_id, name))
+        elif 'seed' in config[name]:
             return AccountFactory(chain_id).create_from_seed(config.get(name, 'seed'))
+        elif 'private_key' in config[name]:
+            return AccountFactory(chain_id).create_from_private_key(config.get(name, 'private_key'))
+        elif 'public_key' in config[name]:
+            return AccountFactory(chain_id).create_from_public_key(config.get(name, 'public_key'))
         else:
-            parser.error("No account found for {} network with name {}, type 'lto account --help' for instructions".format(chain_id, name))
+            parser.error("Invalid settings of account {}".format(name))
     else:
         local_path = Path.joinpath(path, "{}/config.ini".format(chain_id))
         if not os.path.exists(local_path):
-            parser.error("No account found for {} network, type 'lto account --help' for instructions".format(chain_id))
+            parser.error("No Default account set, type 'lto account set-default --help' for instructions".format(chain_id))
         config.clear()
         config.read(local_path)
         if not 'Default' in config.sections():
             parser.error("No Default account set, type 'lto account set-default --help' for instructions")
         else:
             address = config.get('Default', 'address')
             config.clear()
```

### Comparing `lto-cli-1.2.2/src/lto_cli.egg-info/PKG-INFO` & `lto-cli-1.2.3/src/lto_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lto-cli
-Version: 1.2.2
+Version: 1.2.3
 Summary: LTO Network CLI
 Home-page: https://github.com/ltonetwork/lto-cli
 Author: LTO Network
 Author-email: info@ltonetwork.com
 Project-URL: Bug Tracker, https://github.com/ltonetwork/lto-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lto-cli-1.2.2/src/lto_cli.egg-info/SOURCES.txt` & `lto-cli-1.2.3/src/lto_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

