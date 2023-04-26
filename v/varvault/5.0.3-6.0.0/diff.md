# Comparing `tmp/varvault-5.0.3.tar.gz` & `tmp/varvault-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvault-5.0.3.tar", last modified: Wed Mar 22 06:53:48 2023, max compression
+gzip compressed data, was "varvault-6.0.0.tar", last modified: Wed Apr 26 14:12:48 2023, max compression
```

## Comparing `varvault-5.0.3.tar` & `varvault-6.0.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-03-22 06:53:48.255244 varvault-5.0.3/
--rw-r--r--   0 chloe      (501) staff       (20)    11357 2021-11-12 15:14:41.000000 varvault-5.0.3/LICENSE
--rw-r--r--   0 chloe      (501) staff       (20)    10914 2023-03-22 06:53:48.254874 varvault-5.0.3/PKG-INFO
--rw-r--r--   0 chloe      (501) staff       (20)    10406 2022-12-05 20:24:44.000000 varvault-5.0.3/README.md
--rw-r--r--   0 chloe      (501) staff       (20)       38 2023-03-22 06:53:48.255325 varvault-5.0.3/setup.cfg
--rw-r--r--   0 chloe      (501) staff       (20)     2868 2023-03-16 10:09:05.000000 varvault-5.0.3/setup.py
-drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-03-22 06:53:48.249725 varvault-5.0.3/tests/
--rw-r--r--   0 chloe      (501) staff       (20)    18876 2023-01-13 12:24:13.000000 varvault-5.0.3/tests/test_large_scale_vault.py
--rw-r--r--   0 chloe      (501) staff       (20)     4917 2022-12-05 20:24:44.000000 varvault-5.0.3/tests/test_live_update.py
--rw-r--r--   0 chloe      (501) staff       (20)    11097 2022-12-05 20:24:44.000000 varvault-5.0.3/tests/test_logging.py
--rw-r--r--   0 chloe      (501) staff       (20)    12700 2022-12-05 20:24:44.000000 varvault-5.0.3/tests/test_structs.py
--rw-r--r--   0 chloe      (501) staff       (20)    51568 2023-01-13 12:53:40.000000 varvault-5.0.3/tests/test_vault.py
--rw-r--r--   0 chloe      (501) staff       (20)     4448 2022-12-05 20:24:44.000000 varvault-5.0.3/tests/test_xml_vault.py
-drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-03-22 06:53:48.253367 varvault-5.0.3/varvault/
--rw-r--r--   0 chloe      (501) staff       (20)     4992 2023-03-22 06:53:20.000000 varvault-5.0.3/varvault/__init__.py
--rw-r--r--   0 chloe      (501) staff       (20)     3547 2022-12-05 20:24:44.000000 varvault-5.0.3/varvault/factory.py
--rw-r--r--   0 chloe      (501) staff       (20)     4700 2022-12-05 20:24:44.000000 varvault-5.0.3/varvault/flags.py
--rw-r--r--   0 chloe      (501) staff       (20)     7154 2022-12-05 20:24:44.000000 varvault-5.0.3/varvault/keyring.py
--rw-r--r--   0 chloe      (501) staff       (20)     2604 2022-12-05 20:24:44.000000 varvault-5.0.3/varvault/logger.py
--rw-r--r--   0 chloe      (501) staff       (20)     1627 2023-01-13 12:55:44.000000 varvault-5.0.3/varvault/minivault.py
--rw-r--r--   0 chloe      (501) staff       (20)    11178 2022-12-05 20:24:44.000000 varvault-5.0.3/varvault/resource.py
--rw-r--r--   0 chloe      (501) staff       (20)     2155 2022-12-05 20:24:44.000000 varvault-5.0.3/varvault/utils.py
--rw-r--r--   0 chloe      (501) staff       (20)     5385 2022-12-05 20:24:44.000000 varvault-5.0.3/varvault/validator.py
--rw-r--r--   0 chloe      (501) staff       (20)    32619 2023-01-13 14:21:41.000000 varvault-5.0.3/varvault/vault.py
--rw-r--r--   0 chloe      (501) staff       (20)      930 2022-12-05 20:24:44.000000 varvault-5.0.3/varvault/vaultstructs.py
-drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-03-22 06:53:48.254513 varvault-5.0.3/varvault.egg-info/
--rw-r--r--   0 chloe      (501) staff       (20)    10914 2023-03-22 06:53:48.000000 varvault-5.0.3/varvault.egg-info/PKG-INFO
--rw-r--r--   0 chloe      (501) staff       (20)      524 2023-03-22 06:53:48.000000 varvault-5.0.3/varvault.egg-info/SOURCES.txt
--rw-r--r--   0 chloe      (501) staff       (20)        1 2023-03-22 06:53:48.000000 varvault-5.0.3/varvault.egg-info/dependency_links.txt
--rw-r--r--   0 chloe      (501) staff       (20)        9 2023-03-22 06:53:48.000000 varvault-5.0.3/varvault.egg-info/top_level.txt
+drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-04-26 14:12:48.849854 varvault-6.0.0/
+-rw-r--r--   0 chloe      (501) staff       (20)    11357 2021-11-12 15:14:41.000000 varvault-6.0.0/LICENSE
+-rw-r--r--   0 chloe      (501) staff       (20)    10885 2023-04-26 14:12:48.849532 varvault-6.0.0/PKG-INFO
+-rw-r--r--   0 chloe      (501) staff       (20)    10377 2023-04-24 18:48:06.000000 varvault-6.0.0/README.md
+-rw-r--r--   0 chloe      (501) staff       (20)       38 2023-04-26 14:12:48.849942 varvault-6.0.0/setup.cfg
+-rw-r--r--   0 chloe      (501) staff       (20)     2868 2023-04-24 06:37:05.000000 varvault-6.0.0/setup.py
+drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-04-26 14:12:48.843066 varvault-6.0.0/tests/
+-rw-r--r--   0 chloe      (501) staff       (20)    15646 2023-04-24 18:16:29.000000 varvault-6.0.0/tests/test_automatic.py
+-rw-r--r--   0 chloe      (501) staff       (20)    18858 2023-04-24 06:37:05.000000 varvault-6.0.0/tests/test_large_scale_vault.py
+-rw-r--r--   0 chloe      (501) staff       (20)     4944 2023-04-24 06:37:05.000000 varvault-6.0.0/tests/test_live_update.py
+-rw-r--r--   0 chloe      (501) staff       (20)    11049 2023-04-24 06:37:05.000000 varvault-6.0.0/tests/test_logging.py
+-rw-r--r--   0 chloe      (501) staff       (20)    12664 2023-04-24 06:37:05.000000 varvault-6.0.0/tests/test_structs.py
+-rw-r--r--   0 chloe      (501) staff       (20)    51616 2023-04-24 06:37:05.000000 varvault-6.0.0/tests/test_vault.py
+-rw-r--r--   0 chloe      (501) staff       (20)     4427 2023-04-24 06:37:05.000000 varvault-6.0.0/tests/test_xml_vault.py
+drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-04-26 14:12:48.847468 varvault-6.0.0/varvault/
+-rw-r--r--   0 chloe      (501) staff       (20)     4983 2023-04-24 06:37:05.000000 varvault-6.0.0/varvault/__init__.py
+-rw-r--r--   0 chloe      (501) staff       (20)     3547 2022-12-05 20:24:44.000000 varvault-6.0.0/varvault/factory.py
+-rw-r--r--   0 chloe      (501) staff       (20)     5609 2023-04-24 18:16:29.000000 varvault-6.0.0/varvault/flags.py
+-rw-r--r--   0 chloe      (501) staff       (20)     7154 2022-12-05 20:24:44.000000 varvault-6.0.0/varvault/keyring.py
+-rw-r--r--   0 chloe      (501) staff       (20)     2604 2022-12-05 20:24:44.000000 varvault-6.0.0/varvault/logger.py
+-rw-r--r--   0 chloe      (501) staff       (20)     1627 2023-01-13 12:55:44.000000 varvault-6.0.0/varvault/minivault.py
+-rw-r--r--   0 chloe      (501) staff       (20)    11207 2023-04-24 06:37:05.000000 varvault-6.0.0/varvault/resource.py
+-rw-r--r--   0 chloe      (501) staff       (20)      520 2023-04-24 06:37:06.000000 varvault-6.0.0/varvault/subscriber_thread.py
+-rw-r--r--   0 chloe      (501) staff       (20)     2155 2022-12-05 20:24:44.000000 varvault-6.0.0/varvault/utils.py
+-rw-r--r--   0 chloe      (501) staff       (20)     5385 2022-12-05 20:24:44.000000 varvault-6.0.0/varvault/validator.py
+-rw-r--r--   0 chloe      (501) staff       (20)    40136 2023-04-24 18:53:37.000000 varvault-6.0.0/varvault/vault.py
+-rw-r--r--   0 chloe      (501) staff       (20)      930 2022-12-05 20:24:44.000000 varvault-6.0.0/varvault/vaultstructs.py
+drwxr-xr-x   0 chloe      (501) staff       (20)        0 2023-04-26 14:12:48.849195 varvault-6.0.0/varvault.egg-info/
+-rw-r--r--   0 chloe      (501) staff       (20)    10885 2023-04-26 14:12:48.000000 varvault-6.0.0/varvault.egg-info/PKG-INFO
+-rw-r--r--   0 chloe      (501) staff       (20)      578 2023-04-26 14:12:48.000000 varvault-6.0.0/varvault.egg-info/SOURCES.txt
+-rw-r--r--   0 chloe      (501) staff       (20)        1 2023-04-26 14:12:48.000000 varvault-6.0.0/varvault.egg-info/dependency_links.txt
+-rw-r--r--   0 chloe      (501) staff       (20)        9 2023-04-26 14:12:48.000000 varvault-6.0.0/varvault.egg-info/top_level.txt
```

### Comparing `varvault-5.0.3/LICENSE` & `varvault-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `varvault-5.0.3/PKG-INFO` & `varvault-6.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,118 +1,105 @@
-Metadata-Version: 2.1
-Name: varvault
-Version: 5.0.3
-Summary: A package that sets up a key-value vault to store and access variables in a global context.
-Home-page: https://github.com/data-ductus/varvault
-Author: Chloe Holst
-Author-email: chloe.holst@dataductus.se
-License: Apache 2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # README
 
 ## TL;DR
 ### Introduction
 A Python library for storing and using variables from a Python process in a global context and saving the variables to a file for being reused and/or debugging.  
 
 ### Install
 ```
 pip3 install varvault
 ```
 
 ### Contact
-calle.holst@dataductus.se
+chloe.holst@dataductus.se
 
 
 ## What is this? 
 This is a package that allows you to create a key-value vault for storing variables in a global context. It allows 
 you to set up a keyring with pre-defined constants which act as keys for the vault. These constants are then what is 
 stored inside the vault. A key is just a string, but the value that the key is mapped to can be assigned to any type of 
 object in Python. If the object is serializable (like a list or a dict), it can also be writen to something like a JSON file.    
 You can then use a decorator to annotate functions that you want to have use this vault to either store return variables 
 in or to extract variables to be used as input for the function.  
 
 ## How does it work? 
-The way this works is that when you write a function, you annotate it with a special decorator (`varvault.Vault.vaulter`)
-that takes some arguments. This decorator will then handle any input arguments and return variables for you.
+The way this works is that when you write a function, you annotate it with a special decorator (`varvault.Vault.manual` or `varvault.Vault.automatic`)
+that takes some arguments. The decorator will then handle any input arguments and return variables for you.
 The decorator takes some arguments that defines certain keys and flags to tweak the behavior.
 
 ### How about an example?
-The best examples can be found in the test suites which can give a very good idea how it works and is guaranteed to be up-to-date. 
+The best examples can be found in the test suites which can give a very good idea how it works and is guaranteed to be up-to-date.
+
 ```python
 import varvault
 
 
 class Keyring(varvault.Keyring):
-    arg1 = varvault.Key("arg1", valid_type=int)
-    arg2 = varvault.Key("arg2", valid_type=int)
+   arg1 = varvault.Key("arg1", valid_type=int)
+   arg2 = varvault.Key("arg2", valid_type=int)
 
 
 vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource("~/test.json", mode=varvault.ResourceModes.WRITE))
 
 
-@vault.vaulter(return_keys=[Keyring.arg1, Keyring.arg2])
+@vault.manual(output=(Keyring.arg1, Keyring.arg2))
 def create_args(arg1, arg2):
-    return arg1, arg2
+   return arg1, arg2
 
 
-@vault.vaulter(input_keys=[Keyring.arg1, Keyring.arg2])
+@vault.manual(input=(Keyring.arg1, Keyring.arg2))
 def use_args(arg1: int = varvault.AssignedByVault, arg2: int = varvault.AssignedByVault):
-    print(f"{Keyring.arg1}: {arg1}, {Keyring.arg2}: {arg2}")
+   print(f"{Keyring.arg1}: {arg1}, {Keyring.arg2}: {arg2}")
 
 
 def run_create_args():
-    create_args(1, 2)
-    
+   create_args(1, 2)
+
 
 def run_use_args():
-    use_args()
+   use_args()
 
 
 if __name__ == "__main__":
-    run_create_args()
-    
-    run_use_args()    
+   run_create_args()
+
+   run_use_args()    
 ```
 1. In this example, we start by creating a class that defines a keyring. This keyring will be the keys used
    in the vault. Any key you use for storing variables or take variables out should be defined as a constant 
    in this keyring (by default, this is the way to use it, but it is possible to be more flexible).
 
 2. Then we create the actual Vault-object. It's entirely possible to create a Vault without using the factory function,
    but the factory function will do some things for you to make it slightly easier. Creating the vault requires only
    a single argument to be defined and that is a class that inherits from the `varvault.Keyring` (a class based on the Keyring class here).
    Optionally, you can define some flags to further tweak the behavior of the vault. These tweaked behaviors include
    allowing for existing key-value pairs to be modified (this is not allowed by default), allowing return variables from
-   functions defined with return keys to be None, and setting a flag to write some additional debug logs.
+   functions defined with output keys to be `None`, and setting a flag to write some additional debug logs.
    We also define the input parameter `resource` which is a `varvault.JsonResource` object that points to a `.JSON` file. This resource will be used  
    as a vault file to store all the arguments in. 
 
 3. We define a function called `create_args` that takes some arguments (we have to insert variables
    into the vault somehow, right?) that we annotate with the vault decorator. We pass an argument to the
-   decorator called `return_keys`. This argument tells the vault which keys this function will assign its
-   return variables to. Note that the order of the return keys matter. In this case, the ingoing argument `arg1` will
+   decorator called `ouput`. This argument tells the vault which keys this function will assign its
+   return variables to. Note that the order of the output keys matter. In this case, the ingoing argument `arg1` will
    be assigned to `Keyring.arg1`, and the ingoing argument `arg2` will be assigned to `Keyring.arg2`. It's very possible
-   to set `return_keys` to a single `Key` as well if you only have one variable to return. If you want more control
+   to set `output` to a single `Key` as well if you only have one variable to return. If you want more control
    over how return variables are handled, please see `varvault.MiniVault` and make use of that to ensure that
    return-variables are handled exactly as you want. 
    
    **Note:** When this function is called, and it finishes, the decorator here will capture the return variables and then store 
-   those return variables in the vault with the keys that were passed to the decorator as `return_keys`. These variables can then be 
+   those return variables in the vault with the keys that were passed to the decorator as `output`. These variables can then be 
    accessed by another function that uses the same vault-object as this one does to decorate a function.
 
 4. We then create a new function called `use_args` that we also annotate with the vault decorator. We pass a different
-   argument to the decorator this time called `input_keys`. This argument tells the vault which keys in the vault
+   argument to the decorator this time called `input`. This argument tells the vault which keys in the vault
    we want passed to this function. The order of the keys doesn't really matter here, the order is mostly aesthetic.
    
    **Note:** What ends up happening when this function is called, is that the decorator will try to extract keys defined in
-   `input_keys` from the vault and then pass those variables to the function as a dictionary (by defining the arguments as
+   `input` from the vault and then pass those variables to the function as a dictionary (by defining the arguments as
    keyword arguments, these arguments won't need to be provided when the method is called). 
    It is possible to just bundle all the arguments in the signature of the function as a `**kwargs` structure (in this case the signature
    would be `def use_args(**kwargs)`). One of the benefits of doing like in the example is that you can easily see what 
    arguments will be provided by the vault when you use the function, so you know which arguments you have to provide and which are provided by the vault.
 
 5. We create a very simple function called `run_create_args` which doesn't get annotated. This function is simply made
    to demonstrate what makes this vault so useful. When this function is called, it will obviously call `create_args`,
@@ -141,15 +128,15 @@
        arg2 = varvault.Key("arg2")
       
    vault = varvault.create(varvault.Flags.permit_modifications, 
                            keyring=Keyring,                           
                            resource=varvault.JsonResource("~/test.json", mode=varvault.ResourceModes.APPEND))
    ```
    When re-creating a vault from an existing file it's recommended to allow modifications 
-   (see `varvault.VaultFlags.permit_modifications`) in-case you are planning to write the same
+   (see `varvault.Flags.permit_modifications`) in-case you are planning to write the same
    arguments to the vault again. 
 
 ## Conclusion
 This README demonstrates what this functionality can be used for. With this vault, the context for where
 a function executes doesn't matter as long as the keys the function require have been assigned in the vault and the
 functions exists in the scope. The functions become building blocks that you can call regardless of context provided
 the above criteria have been met. You don't need to clutter your main function calls with tons of input variables being passed around
```

### Comparing `varvault-5.0.3/README.md` & `varvault-6.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,104 +1,119 @@
+Metadata-Version: 2.1
+Name: varvault
+Version: 6.0.0
+Summary: A package that sets up a key-value vault to store and access variables in a global context.
+Home-page: https://github.com/data-ductus/varvault
+Author: Chloe Holst
+Author-email: chloe.holst@dataductus.se
+License: Apache 2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # README
 
 ## TL;DR
 ### Introduction
 A Python library for storing and using variables from a Python process in a global context and saving the variables to a file for being reused and/or debugging.  
 
 ### Install
 ```
 pip3 install varvault
 ```
 
 ### Contact
-calle.holst@dataductus.se
+chloe.holst@dataductus.se
 
 
 ## What is this? 
 This is a package that allows you to create a key-value vault for storing variables in a global context. It allows 
 you to set up a keyring with pre-defined constants which act as keys for the vault. These constants are then what is 
 stored inside the vault. A key is just a string, but the value that the key is mapped to can be assigned to any type of 
 object in Python. If the object is serializable (like a list or a dict), it can also be writen to something like a JSON file.    
 You can then use a decorator to annotate functions that you want to have use this vault to either store return variables 
 in or to extract variables to be used as input for the function.  
 
 ## How does it work? 
-The way this works is that when you write a function, you annotate it with a special decorator (`varvault.Vault.vaulter`)
-that takes some arguments. This decorator will then handle any input arguments and return variables for you.
+The way this works is that when you write a function, you annotate it with a special decorator (`varvault.Vault.manual` or `varvault.Vault.automatic`)
+that takes some arguments. The decorator will then handle any input arguments and return variables for you.
 The decorator takes some arguments that defines certain keys and flags to tweak the behavior.
 
 ### How about an example?
-The best examples can be found in the test suites which can give a very good idea how it works and is guaranteed to be up-to-date. 
+The best examples can be found in the test suites which can give a very good idea how it works and is guaranteed to be up-to-date.
+
 ```python
 import varvault
 
 
 class Keyring(varvault.Keyring):
-    arg1 = varvault.Key("arg1", valid_type=int)
-    arg2 = varvault.Key("arg2", valid_type=int)
+   arg1 = varvault.Key("arg1", valid_type=int)
+   arg2 = varvault.Key("arg2", valid_type=int)
 
 
 vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource("~/test.json", mode=varvault.ResourceModes.WRITE))
 
 
-@vault.vaulter(return_keys=[Keyring.arg1, Keyring.arg2])
+@vault.manual(output=(Keyring.arg1, Keyring.arg2))
 def create_args(arg1, arg2):
-    return arg1, arg2
+   return arg1, arg2
 
 
-@vault.vaulter(input_keys=[Keyring.arg1, Keyring.arg2])
+@vault.manual(input=(Keyring.arg1, Keyring.arg2))
 def use_args(arg1: int = varvault.AssignedByVault, arg2: int = varvault.AssignedByVault):
-    print(f"{Keyring.arg1}: {arg1}, {Keyring.arg2}: {arg2}")
+   print(f"{Keyring.arg1}: {arg1}, {Keyring.arg2}: {arg2}")
 
 
 def run_create_args():
-    create_args(1, 2)
-    
+   create_args(1, 2)
+
 
 def run_use_args():
-    use_args()
+   use_args()
 
 
 if __name__ == "__main__":
-    run_create_args()
-    
-    run_use_args()    
+   run_create_args()
+
+   run_use_args()    
 ```
 1. In this example, we start by creating a class that defines a keyring. This keyring will be the keys used
    in the vault. Any key you use for storing variables or take variables out should be defined as a constant 
    in this keyring (by default, this is the way to use it, but it is possible to be more flexible).
 
 2. Then we create the actual Vault-object. It's entirely possible to create a Vault without using the factory function,
    but the factory function will do some things for you to make it slightly easier. Creating the vault requires only
    a single argument to be defined and that is a class that inherits from the `varvault.Keyring` (a class based on the Keyring class here).
    Optionally, you can define some flags to further tweak the behavior of the vault. These tweaked behaviors include
    allowing for existing key-value pairs to be modified (this is not allowed by default), allowing return variables from
-   functions defined with return keys to be None, and setting a flag to write some additional debug logs.
+   functions defined with output keys to be `None`, and setting a flag to write some additional debug logs.
    We also define the input parameter `resource` which is a `varvault.JsonResource` object that points to a `.JSON` file. This resource will be used  
    as a vault file to store all the arguments in. 
 
 3. We define a function called `create_args` that takes some arguments (we have to insert variables
    into the vault somehow, right?) that we annotate with the vault decorator. We pass an argument to the
-   decorator called `return_keys`. This argument tells the vault which keys this function will assign its
-   return variables to. Note that the order of the return keys matter. In this case, the ingoing argument `arg1` will
+   decorator called `ouput`. This argument tells the vault which keys this function will assign its
+   return variables to. Note that the order of the output keys matter. In this case, the ingoing argument `arg1` will
    be assigned to `Keyring.arg1`, and the ingoing argument `arg2` will be assigned to `Keyring.arg2`. It's very possible
-   to set `return_keys` to a single `Key` as well if you only have one variable to return. If you want more control
+   to set `output` to a single `Key` as well if you only have one variable to return. If you want more control
    over how return variables are handled, please see `varvault.MiniVault` and make use of that to ensure that
    return-variables are handled exactly as you want. 
    
    **Note:** When this function is called, and it finishes, the decorator here will capture the return variables and then store 
-   those return variables in the vault with the keys that were passed to the decorator as `return_keys`. These variables can then be 
+   those return variables in the vault with the keys that were passed to the decorator as `output`. These variables can then be 
    accessed by another function that uses the same vault-object as this one does to decorate a function.
 
 4. We then create a new function called `use_args` that we also annotate with the vault decorator. We pass a different
-   argument to the decorator this time called `input_keys`. This argument tells the vault which keys in the vault
+   argument to the decorator this time called `input`. This argument tells the vault which keys in the vault
    we want passed to this function. The order of the keys doesn't really matter here, the order is mostly aesthetic.
    
    **Note:** What ends up happening when this function is called, is that the decorator will try to extract keys defined in
-   `input_keys` from the vault and then pass those variables to the function as a dictionary (by defining the arguments as
+   `input` from the vault and then pass those variables to the function as a dictionary (by defining the arguments as
    keyword arguments, these arguments won't need to be provided when the method is called). 
    It is possible to just bundle all the arguments in the signature of the function as a `**kwargs` structure (in this case the signature
    would be `def use_args(**kwargs)`). One of the benefits of doing like in the example is that you can easily see what 
    arguments will be provided by the vault when you use the function, so you know which arguments you have to provide and which are provided by the vault.
 
 5. We create a very simple function called `run_create_args` which doesn't get annotated. This function is simply made
    to demonstrate what makes this vault so useful. When this function is called, it will obviously call `create_args`,
@@ -127,15 +142,15 @@
        arg2 = varvault.Key("arg2")
       
    vault = varvault.create(varvault.Flags.permit_modifications, 
                            keyring=Keyring,                           
                            resource=varvault.JsonResource("~/test.json", mode=varvault.ResourceModes.APPEND))
    ```
    When re-creating a vault from an existing file it's recommended to allow modifications 
-   (see `varvault.VaultFlags.permit_modifications`) in-case you are planning to write the same
+   (see `varvault.Flags.permit_modifications`) in-case you are planning to write the same
    arguments to the vault again. 
 
 ## Conclusion
 This README demonstrates what this functionality can be used for. With this vault, the context for where
 a function executes doesn't matter as long as the keys the function require have been assigned in the vault and the
 functions exists in the scope. The functions become building blocks that you can call regardless of context provided
 the above criteria have been met. You don't need to clutter your main function calls with tons of input variables being passed around
```

### Comparing `varvault-5.0.3/setup.py` & `varvault-6.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = pathlib.Path(f"{HERE}/README.md").read_text()
 
 # Version handling
 # A good way to tell if we are backwards compatible is to run the test suite and if the tests pass without requiring any changes, we can pretty safely assume we are backwards compatible.
-MAJOR = 5  # Change this if the previous MAJOR is incompatible with this build. Set MINOR and PATCH to 0
+MAJOR = 6  # Change this if the previous MAJOR is incompatible with this build. Set MINOR and PATCH to 0
 MINOR = 0  # Change this if the functionality has changed, but we are still backwards compatible with previous MINOR versions. Set PATCH to 0
-PATCH = 3  # Change this is if we are fixing a bug that doesn't change the functionality. If a bug-fix has caused functionality to be changed, see MINOR instead
+PATCH = 0  # Change this is if we are fixing a bug that doesn't change the functionality. If a bug-fix has caused functionality to be changed, see MINOR instead
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 
 assert varvault.__version__ == VERSION, f"Version mismatch: {varvault.__version__} != {VERSION}"
 
 
 def find_todos_for_version_in_code():
```

### Comparing `varvault-5.0.3/tests/test_large_scale_vault.py` & `varvault-6.0.0/tests/test_large_scale_vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
                 KeyringLargeScale.end_time,
                 KeyringLargeScale.validation_result,
                 KeyringLargeScale.validation_errors,
                 KeyringLargeScale.result_to_upload,
                 KeyringLargeScale.result,
                 ]
 
-        @vault.vaulter(input_keys=keys)
+        @vault.manual(input=keys)
         def _get(**kwargs):
             assert len([k for k in keys if k in kwargs]) == len(keys)
         _get()
 
     def test_get_threaded(self):
         resource_mv = varvault.JsonResource(large_vault_file, mode="r").create_mv(**KeyringLargeScale.get_keys())
         vault = varvault.create(varvault.Flags.remove_existing_log_file, keyring=KeyringLargeScale, resource=varvault.JsonResource(vault_file_new, "w"))
@@ -288,15 +288,15 @@
                 KeyringLargeScale.validation_errors,
                 KeyringLargeScale.result_to_upload,
                 KeyringLargeScale.result,
                 ]
 
         # Note the use of varvault.Flags.silent here. It will speed up the processing significantly.
         # It brings processing down from 3 seconds to 0.6 seconds for 500 parallel requests.
-        @vault.vaulter(varvault.Flags.silent, input_keys=keys)
+        @vault.manual(varvault.Flags.silent, input=keys)
         async def _get(thread_id, **kwargs):
             assert isinstance(thread_id, int)
             assert len([k for k in keys if k in kwargs]) == len(keys)
 
         num_threads = 500
         thread_ids = [i for i in range(num_threads)]
         logger.info(f"Number of threads: {len(thread_ids)}")
@@ -354,11 +354,11 @@
                 ]
 
         # Load the existing vault file and write the contents to the temporary file
         contents = json.load(open(large_vault_file))
         json.dump(contents, open(vault_file_new, "w"), indent=2)
 
         # Since we use live update, the contents of the existing vault file should now be loaded into the vault.
-        @vault.vaulter(input_keys=keys)
+        @vault.manual(input=keys)
         def _get(**kwargs):
             assert len([k for k in keys if k in kwargs]) == len(keys)
         _get()
```

### Comparing `varvault-5.0.3/tests/test_live_update.py` & `varvault-6.0.0/tests/test_live_update.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,44 +29,44 @@
         except:
             pass
 
     def test_live_update_vault(self):
         vault_new = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w+"))
         vault_from = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="r+"))
 
-        @vault_new.vaulter(return_keys=Keyring.key_valid_type_is_str)
+        @vault_new.manual(output=Keyring.key_valid_type_is_str)
         def _set():
             return "valid"
         _set()
 
         assert Keyring.key_valid_type_is_str not in vault_from, f"{Keyring.key_valid_type_is_str} already in the vault; This should not be the case"
 
-        @vault_from.vaulter(input_keys=Keyring.key_valid_type_is_str)
+        @vault_from.manual(input=Keyring.key_valid_type_is_str)
         def _get(**kwargs):
             v = kwargs.get(Keyring.key_valid_type_is_str)
             assert v == "valid", f"Value {v} is not correct; Live-update doesn't work"
         _get()
 
     def test_live_update_on_main_vault(self):
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w+"))
 
-        @vault.vaulter(return_keys=Keyring.key_valid_type_is_str)
+        @vault.manual(output=Keyring.key_valid_type_is_str)
         def _set():
             return "valid"
         _set()
 
         assert Keyring.key_valid_type_is_int not in vault, f"{Keyring.key_valid_type_is_int} already in vault; This should not be possible"
 
         vault_data = json.load(open(vault_file_new))
         vault_data[Keyring.key_valid_type_is_int] = 1
         json.dump(vault_data, open(vault_file_new, "w"), indent=2)
 
         assert Keyring.key_valid_type_is_int not in vault, f"{Keyring.key_valid_type_is_int} already in vault; This should not be possible"
 
-        @vault.vaulter(input_keys=Keyring.key_valid_type_is_int)
+        @vault.manual(input=Keyring.key_valid_type_is_int)
         def _get(**kwargs):
             key_valid_type_is_int = kwargs.get(Keyring.key_valid_type_is_int)
             assert key_valid_type_is_int == 1
         _get()
 
     def test_create_live_update_vault(self):
         assert not os.path.exists(vault_file_new)
@@ -94,28 +94,28 @@
         vault_outer = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="r+"))
         assert not os.path.exists(vault_file_new), "Vault file is created when it shouldn't be"
 
         t = threading.Thread(target=runner)
         t.start()
         t.join()
 
-        @vault_outer.vaulter(input_keys=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
+        @vault_outer.manual(input=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
         def validate(key_valid_type_is_str=None, key_valid_type_is_int=None):
             assert key_valid_type_is_str == "valid"
             assert key_valid_type_is_int == 1
         validate()
 
     def test_resource_live_update(self):
-        fh = varvault.JsonResource(vault_file_new, mode="w+")
-        assert not fh.exists()
-        fh.create_resource()
-        assert fh.exists()
-        pre_state = fh.state
+        resource = varvault.JsonResource(vault_file_new, mode="w+")
+        assert not resource.exists()
+        resource.create()
+        assert resource.exists()
+        pre_state = resource.state
         json.dump({Keyring.key_valid_type_is_str: "valid", Keyring.key_valid_type_is_int: 1}, open(vault_file_new, "w"))
-        assert fh.resource_has_changed()
-        assert fh.cached_state != pre_state
-        data = fh.read()
+        assert resource.resource_has_changed()
+        assert resource.cached_state != pre_state
+        data = resource.read()
         assert data[Keyring.key_valid_type_is_str] == "valid"
         assert data[Keyring.key_valid_type_is_int] == 1
-        fh.update_state()
+        resource.update_state()
 
-        assert fh.last_known_state == fh.cached_state
+        assert resource.last_known_state == resource.cached_state
```

### Comparing `varvault-5.0.3/tests/test_logging.py` & `varvault-6.0.0/tests/test_logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def test_silent(self):
         temp_log_file = os.path.join(tempfile.gettempdir(), "varvault-logs", "varvault-vault-stream.log")
         vault_log_file = os.path.join(tempfile.gettempdir(), "varvault-logs", "varvault.log")
         vault_new = varvault.create(varvault.Flags.silent, varvault.Flags.remove_existing_log_file, keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
         vault_new.logger.addHandler(logging.StreamHandler(open(temp_log_file, "w")))
 
-        @vault_new.vaulter(return_keys=Keyring.key_valid_type_is_str)
+        @vault_new.manual(output=Keyring.key_valid_type_is_str)
         def _set():
             return "valid"
         _set()
         assert len(open(temp_log_file).readlines()) <= 2, f"There appears to be more lines in the log file than what there should be. " \
                                                           f"There should only be 2 at most. {varvault.Flags.silent} appears to not function correctly"
         assert len(open(vault_log_file).readlines()) <= 2, f"There appears to be more lines in the log file than what there should be. " \
                                                            f"There should only be 2 at most. {varvault.Flags.silent} appears to not function correctly. " \
@@ -55,39 +55,39 @@
         temp_log_file = os.path.join(tempfile.gettempdir(), "varvault-logs", "varvault-vault-stream.log")
         vault_log_file = os.path.join(tempfile.gettempdir(), "varvault-logs", "varvault.log")
         vault_new = varvault.create(varvault.Flags.debug, keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
         # Create and set a file to act as a StreamHandler for the logger object in varvault.
         # This way, we can easily capture stdout to a file and assert that the output is the expected
         vault_new.logger.addHandler(logging.StreamHandler(open(temp_log_file, "w")))
 
-        @vault_new.vaulter(return_keys=Keyring.key_valid_type_is_str)
+        @vault_new.manual(output=Keyring.key_valid_type_is_str)
         def _set():
             return "valid"
         _set()
 
         assert len(open(temp_log_file).readlines()) >= 10, f"There appears to be fewer lines in the log file than what there should be. " \
                                                            f"There should only be 12 at least. {varvault.Flags.debug} appears to not function correctly"
         assert len(open(vault_log_file).readlines()) >= 12, f"There appears to be fewer lines in the log file than what there should be. " \
                                                             f"There should only be 12 at least. {varvault.Flags.debug} appears to not function correctly"
 
-        @vault_new.vaulter(input_keys=Keyring.key_valid_type_is_str)
+        @vault_new.manual(input=Keyring.key_valid_type_is_str)
         def _use(key_valid_type_is_str: str = varvault.AssignedByVault):
             return key_valid_type_is_str
 
         assert _use() == "valid", "The value returned by the function is not the same as the value that was set"
 
     def test_silent_and_debug(self):
         temp_log_file = os.path.join(tempfile.gettempdir(), "varvault-logs", "varvault-vault-stream.log")
         vault_log_file = os.path.join(tempfile.gettempdir(), "varvault-logs", "varvault.log")
         vault_new = varvault.create(varvault.Flags.debug, keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
         # Create and set a file to act as a StreamHandler for the logger object in varvault.
         # This way, we can easily capture stdout to a file and assert that the output is the expected
         vault_new.logger.addHandler(logging.StreamHandler(open(temp_log_file, "w")))
 
-        @vault_new.vaulter(varvault.Flags.silent, return_keys=Keyring.key_valid_type_is_str)
+        @vault_new.manual(varvault.Flags.silent, output=Keyring.key_valid_type_is_str)
         def _set():
             return "valid"
         _set()
 
         assert len(open(temp_log_file).readlines()) == 0, f"There appears to be more lines in the log file than what there should be. " \
                                                           f"There should be 0 at most. {varvault.Flags.debug} with {varvault.Flags.silent} appears to not function correctly"
         assert len(open(vault_log_file).readlines()) == 12, f"There appears to be fewer lines in the log file than what there should be. " \
@@ -101,25 +101,25 @@
             pass
         assert not os.path.exists(vault_log_file), f"{vault_log_file} still exists, weird"
 
         vault_new = varvault.create(varvault.Flags.disable_logger, keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
         assert vault_new.logger is None, "logger object is not None; it should be"
         assert not os.path.exists(vault_log_file), f"{vault_log_file} exists after creating the vault when saying there shouldn't be a logger object"
 
-        @vault_new.vaulter(varvault.Flags.silent, return_keys=Keyring.key_valid_type_is_str)
+        @vault_new.manual(varvault.Flags.silent, output=Keyring.key_valid_type_is_str)
         def _set():
             return "valid"
         _set()
         assert not os.path.exists(vault_log_file), f"{vault_log_file} exists after using the vault. How?!"
 
     def test_remove_existing_log_file(self):
         vault_log_file = os.path.join(tempfile.gettempdir(), "varvault-logs", "varvault.log")
         vault_new = varvault.create(varvault.Flags.debug, keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault_new.vaulter(varvault.Flags.silent, return_keys=Keyring.key_valid_type_is_str)
+        @vault_new.manual(varvault.Flags.silent, output=Keyring.key_valid_type_is_str)
         def _doset():
             return "valid"
         _doset()
         with open(vault_log_file) as f1:
             vault_log_file_lines = f1.readlines()
             assert len(vault_log_file_lines) == 12, f"There should be exactly 12 lines in the log-file:\n{''.join(vault_log_file_lines)}"
         vault_from = varvault.create(varvault.Flags.remove_existing_log_file, keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="r"))
@@ -145,15 +145,15 @@
             logger.handlers.clear()
             logger.addHandler(logging.StreamHandler(open(temp_log_file, "w")))
             logger.addHandler(logging.FileHandler(filename=vault_log_file))
 
             vault_new = varvault.create(varvault.Flags.debug, varvault.Flags.remove_existing_log_file, keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"), logger=logger)
             assert vault_new.logger.name == "pytest"  # The logger used for pytest here is called pytest
 
-            @vault_new.vaulter(varvault.Flags.silent, return_keys=Keyring.key_valid_type_is_str)
+            @vault_new.manual(varvault.Flags.silent, output=Keyring.key_valid_type_is_str)
             def _set():
                 return "valid"
             _set()
             temp_log_file_lines = open(temp_log_file).readlines()
             assert len(temp_log_file_lines) == 1, f"There appears to be more lines in the log file than what there should be. There should be 1 at most. \n{''.join(temp_log_file_lines)}"
             vault_log_file_lines = open(vault_log_file).readlines()
             assert len(vault_log_file_lines) == 11, f"There appears to be fewer lines in the log file than what there should be. There should be 11 at most. \n{''.join(vault_log_file_lines)}"
@@ -166,15 +166,15 @@
         temp_log_file = os.path.join(tempfile.gettempdir(), "varvault-logs", "varvault-vault-stream.log")
         vault_log_file = os.path.join(tempfile.gettempdir(), "varvault-logs", "varvault.log")
         vault_new = varvault.create(varvault.Flags.debug, keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
         # Create and set a file to act as a StreamHandler for the logger object in varvault.
         # This way, we can easily capture stdout to a file and assert that the output is the expected
         vault_new.logger.addHandler(logging.StreamHandler(open(temp_log_file, "w")))
 
-        @vault_new.vaulter(varvault.Flags.no_error_logging, return_keys=Keyring.key_valid_type_is_str)
+        @vault_new.manual(varvault.Flags.no_error_logging, output=Keyring.key_valid_type_is_str)
         def _set():
             raise Exception("Failing deliberately")
 
         try:
             _set()
         except:
             pass
```

### Comparing `varvault-5.0.3/tests/test_structs.py` & `varvault-6.0.0/tests/test_structs.py`

 * *Files 8% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             os.remove(vault_file_new)
         except:
             pass
 
     def test_vault_struct_dict(self):
         vault = varvault.create(keyring=KeyringVaultStruct, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault.vaulter(return_keys=KeyringVaultStruct.key_vault_struct_dict)
+        @vault.manual(output=KeyringVaultStruct.key_vault_struct_dict)
         def _set():
             return VaultStructDict("v1", 1)
 
         _set()
         assert isinstance(vault.get(KeyringVaultStruct.key_vault_struct_dict), VaultStructDict)
         logger.info(vault.get(KeyringVaultStruct.key_vault_struct_dict))
         vault_struct_dict = vault.get(KeyringVaultStruct.key_vault_struct_dict)
@@ -143,15 +143,15 @@
         assert hasattr(from_vault.get(KeyringVaultStruct.key_vault_struct_dict), "internal_function")
         assert hasattr(from_vault.get(KeyringVaultStruct.key_vault_struct_dict), "value_1")
         assert hasattr(from_vault.get(KeyringVaultStruct.key_vault_struct_dict), "value_2")
 
     def test_vault_struct_list(self):
         vault = varvault.create(keyring=KeyringVaultStruct, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault.vaulter(return_keys=KeyringVaultStruct.key_vault_struct_list)
+        @vault.manual(output=KeyringVaultStruct.key_vault_struct_list)
         def _set():
             return VaultStructList("v1", 1)
 
         _set()
         assert isinstance(vault.get(KeyringVaultStruct.key_vault_struct_list), VaultStructList)
         logger.info(vault.get(KeyringVaultStruct.key_vault_struct_list))
 
@@ -160,15 +160,15 @@
         assert hasattr(from_vault.get(KeyringVaultStruct.key_vault_struct_list), "internal_function")
         assert hasattr(from_vault.get(KeyringVaultStruct.key_vault_struct_list), "value_1")
         assert hasattr(from_vault.get(KeyringVaultStruct.key_vault_struct_list), "value_2")
 
     def test_vault_struct_string(self):
         vault = varvault.create(keyring=KeyringVaultStruct, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault.vaulter(return_keys=KeyringVaultStruct.key_vault_struct_string)
+        @vault.manual(output=KeyringVaultStruct.key_vault_struct_string)
         def _set():
             return VaultStructString("string-value", "extra-value-here")
 
         _set()
         assert isinstance(vault.get(KeyringVaultStruct.key_vault_struct_string), VaultStructString)
         logger.info(vault.get(KeyringVaultStruct.key_vault_struct_string))
 
@@ -176,15 +176,15 @@
         assert isinstance(from_vault.get(KeyringVaultStruct.key_vault_struct_string), VaultStructString)
         assert hasattr(from_vault.get(KeyringVaultStruct.key_vault_struct_string), "internal_function")
         assert hasattr(from_vault.get(KeyringVaultStruct.key_vault_struct_string), "string_value")
 
     def test_vault_struct_float(self):
         vault = varvault.create(keyring=KeyringVaultStruct, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault.vaulter(return_keys=KeyringVaultStruct.key_vault_struct_float)
+        @vault.manual(output=KeyringVaultStruct.key_vault_struct_float)
         def _set():
             return VaultStructFloat(3.14, "extra-value-here")
 
         _set()
         assert isinstance(vault.get(KeyringVaultStruct.key_vault_struct_float), VaultStructFloat)
         logger.info(vault.get(KeyringVaultStruct.key_vault_struct_float))
 
@@ -192,15 +192,15 @@
         assert isinstance(from_vault.get(KeyringVaultStruct.key_vault_struct_float), VaultStructFloat)
         assert hasattr(from_vault.get(KeyringVaultStruct.key_vault_struct_float), "internal_function")
         assert hasattr(from_vault.get(KeyringVaultStruct.key_vault_struct_float), "float_value")
 
     def test_vault_struct_int(self):
         vault = varvault.create(keyring=KeyringVaultStruct, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault.vaulter(return_keys=KeyringVaultStruct.key_vault_struct_int)
+        @vault.manual(output=KeyringVaultStruct.key_vault_struct_int)
         def _set():
             return VaultStructInt(1, "extra-value-here")
         _set()
 
         assert isinstance(vault.get(KeyringVaultStruct.key_vault_struct_int), VaultStructInt)
         logger.info(vault.get(KeyringVaultStruct.key_vault_struct_int))
 
@@ -208,15 +208,15 @@
         assert isinstance(from_vault.get(KeyringVaultStruct.key_vault_struct_int), VaultStructInt)
         assert hasattr(from_vault.get(KeyringVaultStruct.key_vault_struct_int), "internal_function")
         assert hasattr(from_vault.get(KeyringVaultStruct.key_vault_struct_int), "int_value")
 
     def test_invalid_vault_struct(self):
         vault = varvault.create(keyring=KeyringVaultStruct, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault.vaulter(return_keys=KeyringVaultStruct.key_vault_struct_dict_invalid)
+        @vault.manual(output=KeyringVaultStruct.key_vault_struct_dict_invalid)
         def _set():
             return VaultStructDictInvalid("v1", 1)
 
         _set()
         assert isinstance(vault.get(KeyringVaultStruct.key_vault_struct_dict_invalid), VaultStructDictInvalid)
         try:
             from_vault = varvault.create(keyring=KeyringVaultStruct, resource=varvault.JsonResource(vault_file_new, mode="r"))
```

### Comparing `varvault-5.0.3/tests/test_vault.py` & `varvault-6.0.0/tests/test_vault.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,42 +32,57 @@
             os.remove(vault_file_new_secondary)
         except:
             pass
 
     def test_create_new_vault(self):
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault.vaulter(return_keys=Keyring.key_valid_type_is_str)
+        @vault.manual(output=Keyring.key_valid_type_is_str)
         def _set_valid():
             return "valid-key"
 
         _set_valid()
         assert vault.get(Keyring.key_valid_type_is_str) == "valid-key"
 
-        @vault.vaulter(return_keys=Keyring.key_valid_type_is_int)
+        @vault.manual(output=Keyring.key_valid_type_is_int)
         def _set_invalid():
             return "invalid-key; must be int"
 
         try:
             _set_invalid()
             pytest.fail(f"Somehow managed to set an invalid value to key {Keyring.key_valid_type_is_int} (valid type: {Keyring.key_valid_type_is_int.valid_type})")
         except Exception as e:
             assert "Key 'key_valid_type_is_int' requires type to be '<class 'int'>'" in str(e), f"Unexpected error: {e}"
             logger.info(f"Expected error received; test passed")
             assert Keyring.key_valid_type_is_int not in vault
 
+    def test_no_keys(self):
+        vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
+        called = False
+        vault.manual()
+
+        def _set_valid():
+            nonlocal called
+            called = True
+            return "valid-key"
+
+        _set_valid()
+        assert called
+
+
+
     def test_put(self):
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
         mv = varvault.MiniVault({Keyring.key_valid_type_is_str: "value", Keyring.key_valid_type_is_int: 1})
-        vault.vault.put(mv)
+        vault._put(mv)
         assert Keyring.key_valid_type_is_str in vault
         assert Keyring.key_valid_type_is_int in vault
 
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
-        vault.vault.put(Keyring.key_valid_type_is_str, "value")
+        vault._put(Keyring.key_valid_type_is_str, "value")
         assert Keyring.key_valid_type_is_str in vault
         assert Keyring.key_valid_type_is_int not in vault
 
     def test_create_create_vault(self):
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(existing_vault, mode="r"))
         logger.info(vault)
         assert Keyring.key_valid_type_is_str in vault
@@ -79,15 +94,15 @@
 
     def test_load_from_one_write_to_another(self):
         existing = varvault.JsonResource(existing_vault, "r").create_mv(**Keyring.get_keys())
         logger.info(f"Existing vault: {existing}")
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
         vault.insert_minivault(existing)
 
-        @vault.vaulter(varvault.Flags.permit_modifications, input_keys=Keyring.key_valid_type_is_str, return_keys=Keyring.key_valid_type_is_str)
+        @vault.manual(varvault.Flags.permit_modifications, input=Keyring.key_valid_type_is_str, output=Keyring.key_valid_type_is_str)
         def mod(**kwargs):
             key_valid_type_is_str = kwargs.get(Keyring.key_valid_type_is_str)
             assert key_valid_type_is_str == "valid"
             modded = f"modded"
             return modded
         mod()
 
@@ -102,34 +117,34 @@
 
         vault = varvault.create(keyring=KeyringTemp, resource=varvault.JsonResource(existing_vault, mode="r"))
 
     def test_permit_modifications(self):
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
         vault.insert(Keyring.key_valid_type_is_str, "valid")
         try:
-            @vault.vaulter(return_keys=Keyring.key_valid_type_is_str)
+            @vault.manual(output=Keyring.key_valid_type_is_str)
             def _set():
                 return "new-value-that-should-not-go-in"
             _set()
 
             pytest.fail("Managed to set a new value to an existing key while modifications are not permitted")
         except Exception as e:
             logger.info(f"Expected error received; test passed")
             assert vault.get(Keyring.key_valid_type_is_str) == "valid", f"Value for {Keyring.key_valid_type_is_str} is not what it should be"
 
-        @vault.vaulter(varvault.Flags.permit_modifications, return_keys=Keyring.key_valid_type_is_str)
+        @vault.manual(varvault.Flags.permit_modifications, output=Keyring.key_valid_type_is_str)
         def _set():
             return "new-modified-value"
         _set()
 
         assert vault.get(Keyring.key_valid_type_is_str) == "new-modified-value", f"Value for {Keyring.key_valid_type_is_str} is not what it should be"
 
         new_vault = varvault.create(varvault.Flags.permit_modifications, keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @new_vault.vaulter(return_keys=Keyring.key_valid_type_is_str)
+        @new_vault.manual(output=Keyring.key_valid_type_is_str)
         def _set():
             return "new-modified-value-gen-2"
         _set()
 
         assert new_vault.get(Keyring.key_valid_type_is_str) == "new-modified-value-gen-2", f"Value for {Keyring.key_valid_type_is_str} is not what it should be"
 
     def test_create_readonly_vault(self):
@@ -137,15 +152,15 @@
         try:
             vault.insert(Keyring.key_valid_type_is_int, 1)
             pytest.fail("Insert: Somehow managed to insert a value into a vault that is supposed to be read-only")
         except Exception as e:
             logger.info(f"Expected error received; test passed: {e}")
 
         try:
-            @vault.vaulter(return_keys=Keyring.key_valid_type_is_int)
+            @vault.manual(output=Keyring.key_valid_type_is_int)
             def _set():
                 return 1
             _set()
 
             pytest.fail("Vaulter: Somehow managed to insert a value into a vault that is supposed to be read-only")
         except Exception as e:
             logger.info(f"Expected error received; test passed: {e}")
@@ -201,134 +216,134 @@
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
         try:
             vault.insert(Keyring.key_valid_type_is_int, "this-should-not-work")
             assert False, "Somehow managed to insert a value for a key that should not work"
         except Exception as e:
             logger.info(f"Expected error received; test passed: {e}")
 
-    def test_clean_return_keys(self):
+    def test_clean_output_keys(self):
         vault_new = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault_new.vaulter(return_keys=Keyring.key_valid_type_is_str)
+        @vault_new.manual(output=Keyring.key_valid_type_is_str)
         def _set():
             return "valid"
         _set()
 
         assert vault_new.get(Keyring.key_valid_type_is_str) == "valid"
 
-        @vault_new.vaulter(varvault.Flags.clean_return_keys, return_keys=Keyring.key_valid_type_is_str)
+        @vault_new.manual(varvault.Flags.clean_output_keys, output=Keyring.key_valid_type_is_str)
         def _clean():
             return
 
         _clean()
         assert Keyring.key_valid_type_is_str in vault_new, f"No {Keyring.key_valid_type_is_str} in vault"
         assert vault_new.get(Keyring.key_valid_type_is_str) == "", f"Key {Keyring.key_valid_type_is_str} is not an empty string; {vault_new.get(Keyring.key_valid_type_is_str)}"
 
     def test_extra_keys(self):
         extra_key1 = varvault.Key("extra_key1", valid_type=dict)
         vault_new = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"), extra_key1=varvault.Key("extra_key1", valid_type=dict))
 
-        @vault_new.vaulter(return_keys=extra_key1)
+        @vault_new.manual(output=extra_key1)
         def _set_invalid():
             return [1, 2, 3]
         try:
             _set_invalid()
             pytest.fail("Unexpectedly managed to set an invalid value to an extra key")
         except Exception as e:
             assert "Key 'extra_key1' requires type to be '<class 'dict'>'" in str(e), f"Unexpected error message: {e}"
             logger.info(f"Expected error received; test passed: {e}")
 
-        @vault_new.vaulter(return_keys=extra_key1)
+        @vault_new.manual(output=extra_key1)
         def _set_valid():
             return {"a": 1, "b": 2, "c": 3}
         _set_valid()
 
-        @vault_new.vaulter(varvault.Flags.clean_return_keys, return_keys=extra_key1)
+        @vault_new.manual(varvault.Flags.clean_output_keys, output=extra_key1)
         def _clean():
             return
         _clean()
 
         assert vault_new.get(extra_key1) == {}
 
     def test_return_tuple_is_single_item(self):
         tuple_item = varvault.Key("tuple_item", valid_type=tuple)
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"), tuple_item=tuple_item)
 
-        @vault.vaulter(varvault.Flags.return_tuple_is_single_item, return_keys=tuple_item)
+        @vault.manual(varvault.Flags.return_tuple_is_single_item, output=tuple_item)
         def _set():
             return 1, 2, 3
         _set()
 
         assert tuple_item in vault, f"Flag: No {tuple_item} found in vault"
         assert vault.get(tuple_item) == (1, 2, 3), "Flag: missmatch"
 
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"), tuple_item=tuple_item)
 
-        @vault.vaulter(return_keys=tuple_item)
+        @vault.manual(output=tuple_item)
         def _set():
             return 1, 2, 3
         _set()
 
         assert tuple_item in vault, f"No flag: No {tuple_item} found in vault"
         assert vault.get(tuple_item) == (1, 2, 3), "No flag: Missmatch"
 
-    def test_split_return_keys(self):
+    def test_split_output_keys(self):
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
         vault_secondary = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new_secondary, mode="w"))
 
-        @vault.vaulter(varvault.Flags.split_return_keys, return_keys=Keyring.key_valid_type_is_str)
-        @vault_secondary.vaulter(varvault.Flags.split_return_keys, return_keys=Keyring.key_valid_type_is_int)
+        @vault.manual(varvault.Flags.split_output_keys, output=Keyring.key_valid_type_is_str)
+        @vault_secondary.manual(varvault.Flags.split_output_keys, output=Keyring.key_valid_type_is_int)
         def _set():
             return varvault.MiniVault({Keyring.key_valid_type_is_str: "valid", Keyring.key_valid_type_is_int: 1})
         _set()
 
         assert Keyring.key_valid_type_is_str in vault and Keyring.key_valid_type_is_int not in vault
         assert Keyring.key_valid_type_is_int in vault_secondary and Keyring.key_valid_type_is_str not in vault_secondary
 
         assert vault.get(Keyring.key_valid_type_is_str) == "valid"
         assert vault_secondary.get(Keyring.key_valid_type_is_int) == 1
 
     def test_return_key_can_be_missing(self):
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault.vaulter(return_keys=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
+        @vault.manual(output=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
         def _set_failed():
             return "valid"
 
         try:
             # Should fail saying that number of returned items do not match the number of keys
             _set_failed()
             pytest.fail("Managed to set a single variable to two keys or something")
         except Exception:
             logger.info("Expected error received; test passed")
 
-        @vault.vaulter(varvault.Flags.return_key_can_be_missing, return_keys=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
+        @vault.manual(varvault.Flags.output_key_can_be_missing, output=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
         def _set_failed_again():
             return "valid"
 
         try:
             _set_failed_again()
-            pytest.fail(f"Managed to set a single variable when {varvault.Flags.return_key_can_be_missing} is defined; "
+            pytest.fail(f"Managed to set a single variable when {varvault.Flags.output_key_can_be_missing} is defined; "
                         f"Should have failed saying return var must be of type {varvault.MiniVault}")
         except Exception:
             logger.info("Expected error received; test passed")
 
-        @vault.vaulter(varvault.Flags.return_key_can_be_missing, return_keys=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
+        @vault.manual(varvault.Flags.output_key_can_be_missing, output=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
         def _set_working():
             return varvault.MiniVault({Keyring.key_valid_type_is_str: "valid"})
 
         _set_working()
         assert Keyring.key_valid_type_is_str in vault
         assert Keyring.key_valid_type_is_int not in vault
         assert vault.get(Keyring.key_valid_type_is_str) == "valid"
 
     def test_validate_types_in_minivault_return_values(self):
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault.vaulter(return_keys=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
+        @vault.manual(output=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
         def _set_failed():
             return varvault.MiniVault({Keyring.key_valid_type_is_str: 1, Keyring.key_valid_type_is_int: "invalid"})
         try:
             _set_failed()
             pytest.fail("Managed to set invalid values to the vault by returning them in a minivault.")
         except Exception as e:
             logger.info(f"Expected error received; test passed: {e}")
@@ -401,15 +416,15 @@
 
         vault = varvault.create(keyring=KeyringKeyValidationFunction, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
         with pytest.raises(varvault.ValidatorException) as e:
             vault.insert(KeyringKeyValidationFunction.int_must_be_even_number, 1)
         assert "must_be_even" in str(e.value)
 
-        @vault.vaulter(return_keys=KeyringKeyValidationFunction.int_must_be_even_number)
+        @vault.manual(output=KeyringKeyValidationFunction.int_must_be_even_number)
         def set_failed():
             return 5
         with pytest.raises(varvault.ValidatorException) as e:
             set_failed()
         assert "must_be_even" in str(e.value)
 
         with pytest.raises(varvault.ValidatorException) as e:
@@ -419,15 +434,15 @@
         vault.insert(KeyringKeyValidationFunction.int_must_be_even_number, 2)
         assert KeyringKeyValidationFunction.int_must_be_even_number in vault and vault.get(KeyringKeyValidationFunction.int_must_be_even_number) == 2
 
         with pytest.raises(varvault.ValidatorException) as e:
             vault.insert(KeyringKeyValidationFunction.validator_returns_no_bool, 1)
         assert "The return value is of type" in str(e.value)
 
-        @vault.vaulter(varvault.Flags.permit_modifications, return_keys=KeyringKeyValidationFunction.int_must_be_even_number)
+        @vault.manual(varvault.Flags.permit_modifications, output=KeyringKeyValidationFunction.int_must_be_even_number)
         def set():
             return 4
         set()
 
         assert KeyringKeyValidationFunction.int_must_be_even_number in vault and vault.get(KeyringKeyValidationFunction.int_must_be_even_number) == 4
 
     def test_key_validation_error_message(self):
@@ -445,15 +460,15 @@
         except Exception as e:
             assert KeyringTemp.int_must_be_above_zero in str(e), f"Expected the key {KeyringTemp.int_must_be_above_zero} to be mentioned in the error message, but it was not. Error message: {e}"
             logger.info(e)
 
     def test_add_minivault_function(self):
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault.vaulter(return_keys=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
+        @vault.manual(output=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
         def insert():
             mv = varvault.MiniVault()
             mv.add(Keyring.key_valid_type_is_str, "valid")
             mv.add(Keyring.key_valid_type_is_int, 1)
 
             return mv
 
@@ -504,25 +519,25 @@
     def test_get_multiple_with_input_key_can_be_missing_flag(self):
         vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
         vault.insert(Keyring.key_valid_type_is_str, "valid")
 
         assert Keyring.key_valid_type_is_int not in vault
 
-        @vault.vaulter(input_keys=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
+        @vault.manual(input=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
         def noflag(**kwargs):
             pass
 
         try:
             noflag()
             pytest.fail(f"We managed to get this far, which shouldn't be possible: {vault}")
         except:
             pass
 
-        @vault.vaulter(varvault.Flags.input_key_can_be_missing, input_keys=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
+        @vault.manual(varvault.Flags.input_key_can_be_missing, input=(Keyring.key_valid_type_is_str, Keyring.key_valid_type_is_int))
         def withflag(key_valid_type_is_str: str = None, key_valid_type_is_int: int = None):
             key_valid_type_is_int = key_valid_type_is_int or 1
             assert key_valid_type_is_str == "valid"
             assert key_valid_type_is_int == 1, f"'key_valid_type_is_int' was not {None} when it came into the function: {key_valid_type_is_int}"
 
         withflag()
 
@@ -563,71 +578,71 @@
 
     def test_input_keys_as_kw_vars_only(self):
         vault = varvault.create(varvault.Flags.use_signature_for_input_keys, keyring=Keyring, resource=varvault.JsonResource(vault_file_new, mode="w"))
 
         vault.insert(Keyring.key_valid_type_is_str, "valid")
         vault.insert(Keyring.key_valid_type_is_int, 1)
 
-        @vault.vaulter()
+        @vault.manual()
         def fn_pure_kw_only(*, key_valid_type_is_str=varvault.AssignedByVault, key_valid_type_is_int=varvault.AssignedByVault):
             assert key_valid_type_is_str == "valid"
             assert key_valid_type_is_int == 1
 
         fn_pure_kw_only()
 
-        @vault.vaulter()
+        @vault.manual()
         def fn_pure_kw_or_positional(key_valid_type_is_str=varvault.AssignedByVault, key_valid_type_is_int=varvault.AssignedByVault):
             assert key_valid_type_is_str == "valid"
             assert key_valid_type_is_int == 1
 
         fn_pure_kw_or_positional()
 
-        @vault.vaulter(input_keys=Keyring.key_valid_type_is_str)
+        @vault.manual(input=Keyring.key_valid_type_is_str)
         def fn_mixed(key_valid_type_is_str=varvault.AssignedByVault, key_valid_type_is_int=varvault.AssignedByVault):
             assert key_valid_type_is_str == "valid"
             assert key_valid_type_is_int == 1
 
         fn_mixed()
 
-        @vault.vaulter()
+        @vault.manual()
         def fn_pure_with_args(a1, key_valid_type_is_str=varvault.AssignedByVault, key_valid_type_is_int=varvault.AssignedByVault):
             assert a1 == 3.14
             assert key_valid_type_is_str == "valid"
             assert key_valid_type_is_int == 1
 
         fn_pure_with_args(3.14)
 
-        @vault.vaulter(input_keys=Keyring.key_valid_type_is_str)
+        @vault.manual(input=Keyring.key_valid_type_is_str)
         def fn_mixed_with_args(a1, key_valid_type_is_str=varvault.AssignedByVault, key_valid_type_is_int=varvault.AssignedByVault):
             assert a1 == 3.14
             assert key_valid_type_is_str == "valid"
             assert key_valid_type_is_int == 1
 
         fn_mixed_with_args(3.14)
 
         try:
-            @vault.vaulter()
+            @vault.manual()
             def fn_with_typo(key_valid_type_is_string=varvault.AssignedByVault, key_valid_type_is_integer=varvault.AssignedByVault):  # Note the typos in the key names
                 assert key_valid_type_is_string is None
                 assert key_valid_type_is_integer is None
             pytest.fail("We managed to get this far, which shouldn't be possible")
         except AssertionError:
             pass
 
         try:
-            @vault.vaulter()
+            @vault.manual()
             def fn_faulty_default_assignment(key_valid_type_is_str=None, key_valid_type_is_int=None):
                 assert key_valid_type_is_str == "valid"
                 assert key_valid_type_is_int == 1
             pytest.fail("We managed to get this far, which shouldn't be possible")
         except AssertionError as e:
             pass
 
         try:
-            @vault.vaulter()
+            @vault.manual()
             def fn_mixed_faulty_default_assignment(key_valid_type_is_str=None, key_valid_type_is_integer=varvault.AssignedByVault):
                 assert key_valid_type_is_str == "valid"
                 assert key_valid_type_is_integer == 1
             pytest.fail("We managed to get this far, which shouldn't be possible")
         except AssertionError as e:
             pass
 
@@ -649,41 +664,41 @@
 
     def test_key_usages(self):
         class KeyringTemporary(varvault.Keyring):
             k1 = varvault.Key("k1")
             k2 = varvault.Key("k2")
             k3 = varvault.Key("k3")
         vault = varvault.create(keyring=KeyringTemporary, name="vault")
-        @vault.vaulter(return_keys=(KeyringTemporary.k1, KeyringTemporary.k2, KeyringTemporary.k3))
+        @vault.manual(output=(KeyringTemporary.k1, KeyringTemporary.k2, KeyringTemporary.k3))
         def _set():
             return 1, "valid", 3.14
 
         try:
             vault.get(KeyringTemporary.k1)
             pytest.fail("We managed to get this far, which shouldn't be possible")
         except KeyError as e:
             logger.info(e.args[0])
             assert "test_vault._set" in e.args[0]
 
         _set()
 
-        @vault.vaulter(input_keys=(KeyringTemporary.k1, KeyringTemporary.k2))
+        @vault.manual(input=(KeyringTemporary.k1, KeyringTemporary.k2))
         def _use_first(k1=varvault.AssignedByVault, k2=varvault.AssignedByVault):
             assert k1 == 1
             assert k2 == "valid"
 
         _use_first()
 
-        @vault.vaulter(input_keys=KeyringTemporary.k3)
+        @vault.manual(input=KeyringTemporary.k3)
         def _use_second(k3=varvault.AssignedByVault):
             assert k3 == 3.14
 
         _use_second()
 
-        @vault.vaulter(varvault.Flags.permit_modifications, input_keys=KeyringTemporary.k3, return_keys=KeyringTemporary.k3)
+        @vault.manual(varvault.Flags.permit_modifications, input=KeyringTemporary.k3, output=KeyringTemporary.k3)
         def _override(k3):
             assert k3 == 3.14
             return k3 * 2
         _override()
 
         assert vault.get(KeyringTemporary.k3) == 6.28
         assert KeyringTemporary.k1.usages.as_input == ['test_vault._use_first']
@@ -695,15 +710,15 @@
 
     def test_signature_with_missing_input_keys(self):
         vault = varvault.create(varvault.Flags.use_signature_for_input_keys,
                                 keyring=Keyring,
                                 name="vault",
                                 resource=varvault.JsonResource(vault_file_new, mode="w"))
 
-        @vault.vaulter(varvault.Flags.input_key_can_be_missing, input_keys=Keyring.key_valid_type_is_str)
+        @vault.manual(varvault.Flags.input_key_can_be_missing, input=Keyring.key_valid_type_is_str)
         def _use(key_valid_type_is_str=varvault.AssignedByVault):
             assert not key_valid_type_is_str
             assert key_valid_type_is_str is None, f"It's {type(key_valid_type_is_str)}, not {None}, which is what it should be"
 
         _use()
 
     def test_load_from_backup(self):
@@ -716,15 +731,15 @@
 
         assert not os.path.exists(f"{vault_file_new}.bak"), "This file should have been renamed to remove extension '.bak'"
 
     def test_lambdas(self):
         vault = varvault.create(keyring=Keyring, name="vault")
 
         # Define the lambda function that will be used to set the value of the key
-        setter: Callable = vault.lambdavaulter(lambda: 1, return_keys=Keyring.key_valid_type_is_int)
+        setter: Callable = vault.lambdavaulter(lambda: 1, output_keys=Keyring.key_valid_type_is_int)
         assert callable(setter)
 
         # Define the lambda function that will be used to get the value of the key. Note that the name of the input variable is identical to the name of the key.
         getter: Callable = vault.lambdavaulter(lambda key_valid_type_is_int: key_valid_type_is_int * 3, input_keys=Keyring.key_valid_type_is_int)
         assert callable(getter)
 
         # Set the value of the key using the lambda
@@ -812,77 +827,77 @@
             resource.write({Keyring.key_valid_type_is_str: "should not be written"})
         assert Keyring.key_valid_type_is_str not in resource.create_mv(**Keyring.get_keys()), "The key should not have been written to the file"
 
     def test_faulty_put_on_vault(self):
         # For coverage
         vault = varvault.create(keyring=Keyring)
         with pytest.raises(NotImplementedError) as e:
-            vault.vault.put({Keyring.key_valid_type_is_str: "valid"})
+            vault._put({Keyring.key_valid_type_is_str: "valid"})
         assert "Not implemented" in str(e.value.args[0]), e
 
     def test_vaulted_function_raises_exception(self):
         vault = varvault.create(keyring=Keyring)
         vault.insert(Keyring.key_valid_type_is_str, "valid")
 
-        @vault.vaulter(input_keys=Keyring.key_valid_type_is_str)
+        @vault.manual(input=Keyring.key_valid_type_is_str)
         async def async_func(id, key_valid_type_is_str: str = varvault.AssignedByVault):
             raise ValueError(key_valid_type_is_str)
 
         with pytest.raises(ValueError) as e:
             varvault.concurrent_execution(async_func, [1])
         assert "valid" in str(e.value.args[0]), e
 
-        @vault.vaulter(input_keys=Keyring.key_valid_type_is_str)
+        @vault.manual(input=Keyring.key_valid_type_is_str)
         def func(key_valid_type_is_str: str = varvault.AssignedByVault):
             raise ValueError(key_valid_type_is_str)
 
         with pytest.raises(ValueError) as e:
             func()
         assert "valid" in str(e.value.args[0]), e
 
     def test_no_error_logging_flag(self):
         vault = varvault.create(keyring=Keyring)
         vault.insert(Keyring.key_valid_type_is_str, "valid")
 
-        @vault.vaulter(varvault.Flags.no_error_logging, input_keys=Keyring.key_valid_type_is_str)
+        @vault.manual(varvault.Flags.no_error_logging, input=Keyring.key_valid_type_is_str)
         async def async_func(id, key_valid_type_is_str: str = varvault.AssignedByVault):
             raise ValueError(key_valid_type_is_str)
 
         with pytest.raises(ValueError) as e:
             varvault.concurrent_execution(async_func, [1])
         assert "valid" in str(e.value.args[0]), e
 
-        @vault.vaulter(varvault.Flags.no_error_logging, input_keys=Keyring.key_valid_type_is_str)
+        @vault.manual(varvault.Flags.no_error_logging, input=Keyring.key_valid_type_is_str)
         def func(key_valid_type_is_str: str = varvault.AssignedByVault):
             raise ValueError(key_valid_type_is_str)
 
         with pytest.raises(ValueError) as e:
             func()
         assert "valid" in str(e.value.args[0]), e
 
     def test_flag_is_invalid_type(self):
         vault = varvault.create(keyring=Keyring)
         with pytest.raises(TypeError) as e:
             vault.insert(Keyring.key_valid_type_is_str, "valid", varvault.Flags.permit_modifications.value)
         assert "is not of type" in str(e.value.args[0]), e
 
         with pytest.raises(TypeError) as e:
-            @vault.vaulter(varvault.Flags.permit_modifications.value, return_keys=Keyring.key_valid_type_is_str)
+            @vault.manual(varvault.Flags.permit_modifications.value, output=Keyring.key_valid_type_is_str)
             def func():
                 return "valid"
             func()
 
         assert "is not of type" in str(e.value.args[0]), e
 
     def test_return_values_cannot_be_none(self):
         class KeyringTemp:
             key_valid_type_is_str = varvault.Key("key_valid_type_is_str", valid_type=str, can_be_none=True)
         vault = varvault.create(keyring=Keyring)
         with pytest.raises(ValueError) as e:
-            @vault.vaulter(varvault.Flags.return_values_cannot_be_none, return_keys=KeyringTemp.key_valid_type_is_str)
+            @vault.manual(varvault.Flags.return_values_cannot_be_none, output=KeyringTemp.key_valid_type_is_str)
             def func():
                 return None
             func()
         assert "The value mapped to key_valid_type_is_str is None and Flags.return_values_cannot_be_none is defined" in str(e.value.args[0]), e
 
     def test_get(self):
         vault = varvault.create(keyring=Keyring)
@@ -912,15 +927,15 @@
             key_no_valid_type = varvault.Key("key_no_valid_type")
             key_special_valid_type = varvault.Key("key_special_valid_type", valid_type=Temp)
 
         vault = varvault.create(keyring=KeyringTemp)
         vault.insert(KeyringTemp.key_no_valid_type, "valid")
         vault.insert(KeyringTemp.key_special_valid_type, Temp("a1", "a2"))
 
-        @vault.vaulter(varvault.Flags.clean_return_keys, return_keys=(KeyringTemp.key_no_valid_type, KeyringTemp.key_special_valid_type))
+        @vault.manual(varvault.Flags.clean_output_keys, output=(KeyringTemp.key_no_valid_type, KeyringTemp.key_special_valid_type))
         def clean():
             return
 
         clean()
         assert vault.get(KeyringTemp.key_no_valid_type) is None, vault.get(KeyringTemp.key_no_valid_type)
         assert vault.get(KeyringTemp.key_special_valid_type) is None, vault.get(KeyringTemp.key_special_valid_type)
 
@@ -1001,29 +1016,29 @@
             d = dict(k=Temp)
             assert not resource.writable(d)
             resource.write(d)
         assert "Failed to write to the resource:" in str(e.value.args[0]), e
 
     def test_resource_invalid_value_read(self):
         resource = varvault.JsonResource(vault_file_new, mode="w")
-        resource.create_resource()
+        resource.create()
         open(vault_file_new, "w").write("invalid")
 
         try:
             resource.read()
         except varvault.ResourceNotFoundError as e:
             assert "Failed to read from the resource" in str(e), e
         resource = varvault.JsonResource(vault_file_new, mode="r")
         with pytest.raises(varvault.ResourceNotFoundError) as e:
-            resource.create_resource()
+            resource.create()
         assert "Unable to read from resource at" in str(e.value.args[0]), e
 
     def test_append_resource_mode(self):
         resource = varvault.JsonResource(vault_file_new, mode="a")
-        resource.create_resource()
+        resource.create()
         resource.write({"key": "value"})
         resource = varvault.JsonResource(vault_file_new, mode="r")
         assert resource.read() == {"key": "value"}, resource.read()
 
     def test_modifier_plus_validator_on_insert(self):
         @varvault.validator(function_returns_bool=True)
         def no_dashes_in_str(value: str) -> bool:
```

### Comparing `varvault-5.0.3/tests/test_xml_vault.py` & `varvault-6.0.0/tests/test_xml_vault.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.file_io = None
         super(XmlResource, self).__init__(path, mode)
 
     @property
     def resource(self) -> TextIO:
         return self.file_io
 
-    def create_resource(self) -> None:
+    def create(self) -> None:
         """Creates the resource self.file_io for this handler which we'll use to read and write to."""
         path = self.path
         assert path, "Path is not defined"
         dirname = os.path.dirname(path)
 
         create_dir = lambda: os.makedirs(dirname, exist_ok=True) if dirname else None
         write = lambda: self.do_write({})
@@ -104,15 +104,15 @@
             os.remove(vault_file_new)
         except:
             pass
 
     def test_create_xml_vault(self):
         vault = varvault.create(keyring=Keyring, resource=XmlResource(vault_file_new, mode="w"))
 
-        @vault.vaulter(return_keys=(Keyring.string_value, Keyring.int_value, Keyring.list_value))
+        @vault.manual(output=(Keyring.string_value, Keyring.int_value, Keyring.list_value))
         def _set():
             return "valid", 1, [1, 2, 3, 4, 5]
 
         _set()
 
         data_in_file = xmltodict.parse(open(vault_file_new, "rb"))[XmlResource.KEY]
         logger.info(data_in_file)
@@ -120,14 +120,14 @@
         # XML data is actually just strings. But we still want to support using XML files, but it will take some manual labour to get it working correctly.
         assert Keyring.int_value in data_in_file and data_in_file[Keyring.int_value] == "1"
         assert Keyring.list_value in data_in_file
 
     def test_read_from_xml_vault(self):
         vault = varvault.create(keyring=Keyring, resource=XmlResource(existing_vault, "r"))
 
-        @vault.vaulter(input_keys=(Keyring.string_value, Keyring.int_value))
+        @vault.manual(input=(Keyring.string_value, Keyring.int_value))
         def _get(string_value=None, int_value=None):
             assert string_value == "valid"
             assert int_value == "1"
 
         _get()
```

### Comparing `varvault-5.0.3/varvault/__init__.py` & `varvault-6.0.0/varvault/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "5.0.3"
+__version__ = "6.0.0"
 
 import os
 import json
 
 from typing import Dict, TextIO, AnyStr, Literal, Union
 
 from .resource import ResourceModes
@@ -74,15 +74,15 @@
         return hash_md5.hexdigest()
 
     @property
     def resource(self) -> TextIO:
         """Returns the file resource object for this handler."""
         return self.file_io
 
-    def create_resource(self) -> None:
+    def create(self) -> None:
         """Creates the resource self.file_io for this handler which we'll use to read and write to."""
         path = self.path
         assert path, "Path is not defined"
         dirname = os.path.dirname(path)
 
         create_dir = lambda: os.makedirs(dirname, exist_ok=True) if dirname else None
         write = lambda: self.do_write({})
```

### Comparing `varvault-5.0.3/varvault/factory.py` & `varvault-6.0.0/varvault/factory.py`

 * *Files identical despite different names*

### Comparing `varvault-5.0.3/varvault/flags.py` & `varvault-6.0.0/varvault/flags.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,56 +12,71 @@
             return any([f in flags for f in flag])
         return flag in flags
 
     f"""Flag to set if return values must be something other than {None}. By default, this is fine, but you can enforce return variables to be something other than {None}"""
     return_values_cannot_be_none = enum.auto()
 
     f"""Flag to set if variables may be modified either in the vault itself or for a specific decorated function. 
-        By default, varvault doesn't permit modifications to existing keys as this can cause unintended behavior."""
+    By default, varvault doesn't permit modifications to existing keys as this can cause unintended behavior. 
+    
+    Note that combined with the 'automatic' decorator to subscribe on one or more keys, replacing a key will effectively trigger all subscribed methods again. 
+    """
     permit_modifications = enum.auto()
 
     f"""Flag to set if an input variable may be missing in a vault when it is accessed. In this case, the key will be sent to kwargs but it will be mapped to {None}."""
     input_key_can_be_missing = enum.auto()
 
-    f"""Flag to clean return keys in a vault defined for a decorated function. This can be used during a cleanup stage. 
+    f"""Flag to clean output keys in a vault defined for a decorated function. This can be used during a cleanup stage. 
     Varvault will try to map the key to a default value for the valid type, like for example str(), or list(). If it doesn't work, the key will be mapped to {None}."""
-    clean_return_keys = enum.auto()
+    clean_output_keys = enum.auto()
 
     f"""Flag to enable debug mode for logger output to the console to help you with debugging. By default, varvault will write debug logs to the logfile, but not the console. 
     By setting this, you'll have a much easier time debugging unintended behavior. Using this and 'silent' (see further down) in conjunction will cancel each other out and make logging the default."""
     debug = enum.auto()
 
     f"""Flag to enable silent mode for a vault. This will completely remove debug logs being written to the logfile. This can be used to reduce unnecessary
          bloat and make debugging much more easy to do. Using this and {debug} in conjunction will cancel each other out and make logging the default."""
     silent = enum.auto()
 
     f"""Flag to tell varvault that the return value is a tuple that should be mapped to a single return-key. Varvault cannot tell if 
     a tuple is multiple return values or a single item meant for a single key as this how Python handles multiple return values"""
     return_tuple_is_single_item = enum.auto()
 
-    f"""Flag to tell varvault that the return keys provided in a MiniVault being returned are split between multiple vaults decorating the same function. 
-    By default, any return values from a decorated function must be able to be mapped to the keys defined as return keys. If two vaults are taking return values separately, 
+    f"""Flag to tell varvault that the output keys provided in a MiniVault being returned are split between multiple vaults decorating the same function. 
+    By default, any return values from a decorated function must be able to be mapped to the keys defined as output keys. If two vaults are taking return values separately, 
     this wouldn't be possible. Usage of this flag REQUIRES that the return value is a MiniVault-object."""
-    split_return_keys = enum.auto()
+    split_output_keys = enum.auto()
 
     f"""Flag to tell varvault to disable logger completely and not log anything to a log-file."""
     disable_logger = enum.auto()
 
     f"""Flag to ignore keys not in keyring when creating a vault from an existing vault-resource. If resource is configured as read-only, this behavior will be enabled by default."""
     ignore_keys_not_in_keyring = enum.auto()
 
     f"""Flag to tell varvault to delete an existing log file when creating a vault from an existing vault-file"""
     remove_existing_log_file = enum.auto()
 
     f"""Flag to tell varvault when using a vaulter-decorated function and not returning objects for all keys to not fail and just set the keys defined.
      If this is set, the return variables MUST be inside a MiniVault object, otherwise varvault cannot determine what variable belongs to what key."""
-    return_key_can_be_missing = enum.auto()
+    output_key_can_be_missing = enum.auto()
 
     f"""Flag to tell a vaulter-decorated function to not log exceptions. Exceptions can sometimes be expected,
     and sometimes it might be preferable to not log errors using varvault and just log them normally."""
     no_error_logging = enum.auto()
 
     f"""Flag to tell varvault to use the keyword args in the signature of a decorated function to determine the keys to extract from the vault. This effectively removes 
     the need to define input keys through the decorator. Instead, you just need to define the input keys in the signature of the decorated function by calling the keyword 
     argument the same as the key. This will make tracking where the keys in the Keyring are used harder, but reduces the amount of boilerplate required. Can be defined 
     for the entire vault, or for a specific decorated function only."""
     use_signature_for_input_keys = enum.auto()
+
+    f"""Flag to tell varvault to replace the input key with the output key. This is useful when you want to update the value of a key in the vault.
+    When using the 'automatic' decorator, this can be useful if one function has to create a structure, something else happens using that structure, and then the structure is updated.
+    Using this flag, you can update the structure in the vault by having multiple keys that act as intermediate keys.
+    
+    Example:
+    @vault.automatic(Flags.output_key_replaces_input_key, input=Keyring.intermediate, output=Keyring.final)
+    def func(intermediate=AssignedByVault):
+        intermediate['key'] = 'value'
+        return intermediate
+    """
+    output_key_replaces_input_key = enum.auto()
```

### Comparing `varvault-5.0.3/varvault/keyring.py` & `varvault-6.0.0/varvault/keyring.py`

 * *Files identical despite different names*

### Comparing `varvault-5.0.3/varvault/logger.py` & `varvault-6.0.0/varvault/logger.py`

 * *Files identical despite different names*

### Comparing `varvault-5.0.3/varvault/minivault.py` & `varvault-6.0.0/varvault/minivault.py`

 * *Files identical despite different names*

### Comparing `varvault-5.0.3/varvault/resource.py` & `varvault-6.0.0/varvault/resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     @property
     @abc.abstractmethod
     def state(self):
         """Meant to return the state of the resource, such as a hash of the resource."""
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def create_resource(self):
+    def create(self):
         """Meant to create the resource to store the vault in a database."""
         raise NotImplementedError()
 
     @property
     @abc.abstractmethod
     def path(self) -> Union[AnyStr, Any]:
         """Meant to return the path to the database that stores the vault."""
@@ -162,25 +162,25 @@
         """Meant to return a bool which says if the resource exists or not"""
         raise NotImplementedError()
 
     # ================================================================================================================
     # Write
     # ================================================================================================================
     def write(self, vault: dict) -> None:
-        f"""Writes the vault to the database by calling the implemented '{self.do_write}' method."""
+        f"""Writes the vault to the database by calling the implemented '{self.do_write}' method. Not meant to be overridden."""
         if not vault:
             # No point writing an empty dict and it's not the job of this method to create the file
             return
 
         if self.mode_properties.read_only:
             warnings.warn("Tried to write to a resource defined as read-only. This is not permitted by varvault.")
             return
 
         if not self.resource:
-            self.create_resource()
+            self.create()
         try:
             with self.lock:
                 self.do_write(vault)
         except Exception as e:
             raise ResourceNotFoundError(f"Failed to write to the resource: {e}", self)
         self.update_state()
 
@@ -199,17 +199,17 @@
         """
         raise NotImplementedError()
 
     # ================================================================================================================
     # Read
     # ================================================================================================================
     def read(self) -> Dict:
-        f"""Reads the vault from the database by calling the implemented '{self.do_read}' method."""
+        f"""Reads the vault from the database by calling the implemented '{self.do_read}' method. Not meant to be overridden."""
         if not self.resource:
-            self.create_resource()
+            self.create()
         with self.lock:
             if self.exists():
                 try:
                     data = self.do_read()
                     self.update_state()
                     return data
                 except Exception as e:
```

### Comparing `varvault-5.0.3/varvault/utils.py` & `varvault-6.0.0/varvault/utils.py`

 * *Files identical despite different names*

### Comparing `varvault-5.0.3/varvault/validator.py` & `varvault-6.0.0/varvault/validator.py`

 * *Files identical despite different names*

### Comparing `varvault-5.0.3/varvault/vault.py` & `varvault-6.0.0/varvault/vault.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 from __future__ import annotations
 
+import json
 import asyncio
 import inspect
 import logging
+import time
+import warnings
 import functools
 import traceback
-import warnings
 
 from typing import *
 from threading import Lock
 
 from .resource import BaseResource
 from .keyring import Keyring, Key
 from .logger import get_logger, configure_logger
 from .minivault import MiniVault
+from .subscriber_thread import SubscriberThread
 from .utils import concurrent_execution, AssignedByVault, assert_and_raise
 from .flags import Flags
 
 
-class VarVault(object):
-    class Vault(dict):
-        def __init__(self, vault_resource: BaseResource = None, initial_vars: MiniVault = None):
-            super(VarVault.Vault, self).__init__()
-            self.writable_args = dict()
-            self.resource = vault_resource
-            self.initialized = False
-            if initial_vars and isinstance(initial_vars, MiniVault):
-                self.put(initial_vars)
-            self.initialized = True
-
-        def __setitem__(self, key, value):
-            data = {key: value}
-            if self.resource and self.resource.writable(data):
-                self.writable_args.update(data)
-
-            super(VarVault.Vault, self).__setitem__(key, value)
-
-        @functools.singledispatchmethod
-        def put(self, *args, **kwargs):
-            raise NotImplementedError("Not implemented")
-
-        @put.register
-        def _mv(self, mini: MiniVault):
-            f"""{self.put} to add a MiniVault"""
-
-            async def _put(item):
-                key, value = item
-                self.__setitem__(key, value)
-            concurrent_execution(_put, mini.items())
-            self.write()
-
-        @put.register
-        def _k_v(self, key: Key, value: object):
-            f"""{self.put} to add a key-value pair"""
+class VarVault(dict):
+
+    def __setitem__(self, key, value):
+        data = {key: value}
+        if self.resource and self.resource.writable(data):
+            self.writable_args.update(data)
+
+        super(VarVault, self).__setitem__(key, value)
+
+    def __delitem__(self, key):
+        if self.resource and key in self.writable_args:
+            del self.writable_args[key]
+
+        super(VarVault, self).__delitem__(key)
+
+    @functools.singledispatchmethod
+    def _put(self, *args, **kwargs):
+        raise NotImplementedError("Not implemented")
+
+    @_put.register
+    def _mv(self, mini: MiniVault):
+        f"""{self._put} to add a MiniVault"""
+
+        async def _put(item):
+            key, value = item
             self.__setitem__(key, value)
-            self.write()
+        concurrent_execution(_put, mini.items())
+        self.write()
 
-        def write(self):
-            # No resource has been defined, which means we cannot write anything to the file
-            if not self.resource:
-                return
+    @_put.register
+    def _k_v(self, key: Key, value: object):
+        f"""{self._put} to add a key-value pair"""
+        self.__setitem__(key, value)
+        self.write()
+
+    def write(self):
+        # No resource has been defined, which means we cannot write anything to the file
+        if not self.resource:
+            return
 
-            # Write is not permitted
-            if not self.resource.mode_properties.write:
-                # If it's initialized and live-update isn't permitted, then we should raise a warning because we are clearly trying to write to a file that we cannot write to
-                if self.initialized and not self.resource.mode_properties.live_update:
-                    warnings.warn("It appears you are trying to write to a resource that is not permitted to write to and the vault has already been initialized. "
-                                  "This is not permitted and you should consider removing the action that triggered this.")
-                return
+        # Write is not permitted
+        if not self.resource.mode_properties.write:
+            # If it's initialized and live-update isn't permitted, then we should raise a warning because we are clearly trying to write to a file that we cannot write to
+            if self.initialized and not self.resource.mode_properties.live_update:
+                warnings.warn("It appears you are trying to write to a resource that is not permitted to write to and the vault has already been initialized. "
+                              "This is not permitted and you should consider removing the action that triggered this.")
+            return
 
-            # Try to write writable_args to vault_file if it has been defined
-            self.resource.write(self.writable_args)
+        # Try to write writable_args to vault_file if it has been defined
+        self.resource.write(self.writable_args)
 
     def __init__(self,
                  *flags: Flags,
                  keyring: Type[Keyring] = None,
                  name: str = None,
                  resource: BaseResource = None,
                  logger: logging.Logger = None,
@@ -89,73 +89,95 @@
         :param resource: The resource to for the vault.  
         :param logger: Optional. A specific logger to log to in-case you do not want to use the built-in logger in varvault.
         :param initial_vars: Optional. A {MiniVault} containing variables to be added to the vault when it is created. 
          The factory function 'create' will provide this if the mode for a resource is allowed to do 'load'. 
         :param extra_keys: Optional. A kwargs-object with extra keys that are not defined in the {keyring}. This can be useful when you have a lot of keys that you might 
          want to handle in a programmatic sense rather than in a pre-defined sense. 
         """
+        super().__init__()
+
         assert_and_raise(keyring is not None and issubclass(keyring, Keyring),
                          ValueError(f"{self.__init__.__name__} requires a {Keyring} class to be passed as the {keyring} argument"))
 
         assert_and_raise(name is None or isinstance(name, str),
                          ValueError(f"'name' must be of type {str}, or {None}, not ({type(name)})"))
 
         assert_and_raise(resource is None or isinstance(resource, BaseResource),
                          ValueError(f"'resource' must be of type {BaseResource}, or {None}, not {type(resource)}"))
 
         assert_and_raise(logger is None or isinstance(logger, logging.Logger),
                          ValueError(f"'logger' must be of type {logging.Logger}, or {None}, not {type(logger)}"))
 
-        assert_and_raise(not Flags.is_set(Flags.clean_return_keys, *flags),
-                         ValueError(f"You really should not set the flag {Flags.clean_return_keys} to the vault itself as that would be an extremely bad idea."))
+        assert_and_raise(not Flags.is_set(Flags.clean_output_keys, *flags),
+                         ValueError(f"You really should not set the flag {Flags.clean_output_keys} to the vault itself as that would be an extremely bad idea."))
 
         for key_name, key in extra_keys.items():
             assert_and_raise(isinstance(key_name, str) and isinstance(key, Key),
                              ValueError(f"extra_keys is not setup correctly; The pattern {{{key_name} ({type(key_name)}): {key} ({type(key)})}} is incorrect. Correct pattern would be {{{key_name} ({str}): {key} ({Key})}}"))
 
         disable_logger = Flags.is_set(Flags.disable_logger, *flags)
         remove_existing_log_file = Flags.is_set(Flags.remove_existing_log_file, *flags)
         if logger:
             self.logger = logger
         else:
             self.logger = get_logger(name, remove_existing_log_file) if not disable_logger else None
+        self.writable_args = dict()
+        self.initialized = False
         self.times_taken = dict()
         self.keyring_class = keyring
         self.flags: set = set(flags)
         self.resource: BaseResource = resource
+        self.functions_as_automatics: Dict[Key, List[Callable]] = dict()
+        self.keys_used_by_automatics: Dict[Callable, List[Key]] = dict()
+        self.automatic_conditionals: Dict[Callable, Callable] = dict()
+        self.running_tasks: Set[SubscriberThread] = set()
+        self.threaded_automatics = set()
+
+        if initial_vars and isinstance(initial_vars, MiniVault):
+            self._put(initial_vars)
+        self.initialized = True
 
         if self.resource and not self.resource.resource:
-            self.resource.create_resource()
+            self.resource.create()
 
         self.lock = Lock()
 
         # Get the keys from the keyring and expand it with extra keys
         self.keys: Dict[str, Key] = self.keyring_class.get_keys()
         self.keys.update(extra_keys)
 
-        # Create the inner vault
-        self._inner_vault = self.Vault(self.resource, initial_vars)
-
         if self.resource:
             self.log(f"Vault writing data to '{self.resource.path}'", level=logging.DEBUG, all_flags=flags)
             if self.resource.mode_properties.live_update:
                 self.log(f"Vault doing live updates from '{self.resource.path}' whenever the vault is accessed.", level=logging.DEBUG, all_flags=flags)
 
     def __contains__(self, key: Key):
         self._assert_key_is_correct_type(key, msg=f"{self.__contains__.__name__} may only be used with a {Key}-object, not {type(key)}")
 
         if key.key_name not in self.keys:
             warnings.warn(f"{key.key_name} is not defined in the keyring. This is not a problem, but trying to check if the "
                           f"vault contains this key will never succeed; Consider removing the call that triggered this warning.")
             return False
 
-        return key in self.vault
+        return super().__contains__(key)
 
     def __str__(self):
-        return self._inner_vault.__str__()
+
+        return super().__str__()
+
+    def as_json_str(self):
+        """
+        Returns the vault as a json-string, if possible. If not, return as a string.
+        :return: A json-string containing the vault.
+        """
+        try:
+            return json.dumps(self, indent=2)
+        except json.JSONDecodeError:
+            # Probably some objects in the vault that cannot be serialized. Just return the string representation of the vault then.
+            return self.__str__()
 
     def log(self, msg: object, *args, level: int = logging.DEBUG, exception: BaseException = None, all_flags: Union[Set[Flags], Tuple[Flags]] = None):
         if self.logger:
             all_flags = all_flags or self.flags
             assert isinstance(level, int), "Log level must be defined as an integer"
             self._configure_log_levels_based_on_flags(*all_flags)
             self.logger.log(level, msg, *args, exc_info=exception)
@@ -175,156 +197,66 @@
 
     def _reset_log_levels(self):
         if not self.logger:
             # No logger has been assigned for this vault. Just return then.
             return
         configure_logger(self.logger, overall_level=logging.DEBUG, stream_level=logging.INFO, file_level=logging.DEBUG)
 
-    @property
-    def vault(self) -> Vault:
-        return self._inner_vault
-
-    # =========================================================================================================================================
-    # vaulter
-    # =========================================================================================================================================
-    def vaulter(self,
-                *flags: Flags,
-                input_keys: Union[Key, List[Key, ...], Tuple[Key, ...]] = None,
-                return_keys: Union[Key, List[Key, ...], Tuple[Key, ...]] = None) -> Callable:
+    # ============================================================
+    # manual
+    # ============================================================
+    def manual(self,
+               *flags: Flags,
+               input: Union[Key, List[Key], Tuple[Key, ...]] = None,
+               output: Union[Key, List[Key], Tuple[Key, ...]] = None) -> Callable:
         f"""
-        Decorator to define a function as a vaulted function.
+        Decorator to register a function as a vaulted function that must be called MANUALLY.
         A vaulted function works a lot different to a normal function.
         A vault works like a key-value storage. A vaulted function will get its arguments
         by accessing them from the vault, and then store any returned value back in the vault.
 
-        :param input_keys: Can be of type: {Key}, {list}, {tuple}. Default: {None}. Keys must be defined in the
+        :param input: Can be of type: {Key}, {list}, {tuple}. Default: {None}. Keys must be defined in the
          keyring for this specific vault.
-        :param return_keys: Can be of type: {str}, {list}, {tuple}. Default: {None}. Keys must be defined in the
+        :param output: Can be of type: {Key}, {list}, {tuple}. Default: {None}. Keys must be defined in the
          keyring for this specific vault.
         :param flags: Optional argument for defining some flags for this vaulted function. Flags that have an effect:
          {Flags.debug},
          {Flags.silent},
          {Flags.input_key_can_be_missing},
          {Flags.permit_modifications},
-         {Flags.split_return_keys},
-         {Flags.return_key_can_be_missing},
-         {Flags.clean_return_keys},
+         {Flags.split_output_keys},
+         {Flags.output_key_can_be_missing},
+         {Flags.clean_output_keys},
          {Flags.no_error_logging},
          {Flags.use_signature_for_input_keys},
+         {Flags.output_key_replaces_input_key},
         """
-        input_keys = input_keys if input_keys else list()
-        return_keys = return_keys if return_keys else list()
         all_flags = self._get_all_flags(*flags)
-        # Validate the input to the decorator
-        self._vaulter__validate_input(input_keys, return_keys)
 
-        # Convert input- and return keys to a list if it's a single key to make it easier to handle
-        input_keys, return_keys = self._vaulter__convert_input_keys_and_return_keys(input_keys, return_keys)
+        # Convert input- and output keys to a list if it's a single key to make it easier to handle
+        input, output = self._convert_input_keys_and_output_keys(input, output)
 
         # Assert that the keys are in the keyring
-        self._assert_keys_in_keyring(input_keys)
-        self._assert_keys_in_keyring(return_keys)
+        self._assert_keys_in_keyring(input)
+        self._assert_keys_in_keyring(output)
 
         def wrap_outer(func):
-            func_module_name = f"{func.__module__}.{func.__name__}"
-            [key.usages.add_input(func) for key in input_keys]
-            [key.usages.add_return(func) for key in return_keys]
+            [key.usages.add_input(func) for key in input]
+            [key.usages.add_return(func) for key in output]
             if Flags.is_set(Flags.use_signature_for_input_keys, *all_flags):
-                self._vaulter__populate_input_keys_from_signature(func, input_keys)
+                self._manual__populate_input_keys_from_signature(func, input)
 
             # Separate handling if the decorated function uses the coroutine API
             if asyncio.iscoroutinefunction(func):
-                @functools.wraps(func)
-                async def wrap_inner_async(*args, **kwargs):
-                    #
-                    # Do pre-call related stuff
-                    #
-                    input_kwargs = self._vaulter__pre_call(input_keys, func_module_name, *all_flags, **kwargs)
-                    try:
-                        ret = await func(*args, **input_kwargs)
-                    except Exception as e:
-                        if not Flags.is_set(Flags.no_error_logging, *all_flags):
-                            # Flag to not log error is NOT set, so we should log the error and then raise the error
-                            self.log(f"Failed to run {func_module_name}: {e}", level=logging.ERROR, all_flags=all_flags)
-                            self.log(str(traceback.format_exc()).rstrip("\n"), level=logging.ERROR, all_flags=all_flags)
-                        raise
-
-                    #
-                    # Do post-call related stuff
-                    #
-                    self._vaulter__post_call(ret, return_keys, func_module_name, *all_flags)
-
-                    return ret
-                return wrap_inner_async
+                return self._inner_async(func, *all_flags, input=input, output=output)
             else:
-                @functools.wraps(func)
-                def wrap_inner(*args, **kwargs):
-                    #
-                    # Do pre-call related stuff
-                    #
-                    input_kwargs = self._vaulter__pre_call(input_keys, func_module_name, *all_flags, **kwargs)
-
-                    try:
-                        ret = func(*args, **input_kwargs)
-                    except Exception as e:
-                        if not Flags.is_set(Flags.no_error_logging, *all_flags):
-                            # Flag to not log error is NOT set, so we should log the error and then raise the error
-                            self.log(f"Failed to run {func_module_name}: {e}", level=logging.ERROR, all_flags=all_flags)
-                            self.log(str(traceback.format_exc()).rstrip("\n"), level=logging.ERROR, all_flags=all_flags)
-                        raise
-
-                    #
-                    # Do post-call related stuff
-                    #
-                    self._vaulter__post_call(ret, return_keys, func_module_name, *all_flags)
-
-                    return ret
-                return wrap_inner
+                return self._inner_standard(func, *all_flags, input=input, output=output)
         return wrap_outer
 
-    def _vaulter__pre_call(self, input_keys: Union[List[Key], Tuple[Key]], func_module_name: str, *all_flags: Flags, **kwargs):
-        input_kwargs = self._vaulter__build_input_vars(input_keys, *all_flags, **kwargs)
-        kwargs.update(input_kwargs)
-
-        self.log(f"======{'=' * len(func_module_name)}=", all_flags=all_flags)
-        self.log(f">>>>> {func_module_name}:", all_flags=all_flags)
-        if input_kwargs:
-            self.log(f"-------------", all_flags=all_flags)
-            self.log(f"Input kwargs:", all_flags=all_flags)
-            for kwarg_key, kwarg_value in input_kwargs.items():
-                self.log(f"--> {kwarg_key}: ({type(kwarg_value)}) -- {kwarg_value}", all_flags=all_flags)
-            self.log(f"-------------", all_flags=all_flags)
-        input_kwargs.update(kwargs)
-
-        self.log(f"======= Calling {func_module_name} ========", all_flags=all_flags)
-        return input_kwargs
-
-    def _vaulter__post_call(self, ret, return_keys, func_module_name, *all_flags: Flags):
-        self._vaulter__handle_return_vars(ret, return_keys, *all_flags)
-        self.log(f"<<<<< {func_module_name}:", all_flags=all_flags)
-        self.log(f"======{'=' * len(func_module_name)}=\n", all_flags=all_flags)
-        self._reset_log_levels()
-
-    def _vaulter__validate_input(self, input_keys, return_keys):
-        assert_and_raise(isinstance(input_keys, (Key, list, tuple)),
-                         TypeError(f"input_keys must be of type {Key}, {list}, or {tuple}"))
-        assert_and_raise(isinstance(return_keys, (Key, list, tuple)),
-                         TypeError(f"return_keys must be of type {Key}, {list}, or {tuple}"))
-
-    def _vaulter__convert_input_keys_and_return_keys(self, input_keys: Union[Key, List, Tuple], return_keys: Union[Key, List, Tuple]):
-        if isinstance(input_keys, Key):
-            input_keys = [input_keys]
-        if isinstance(return_keys, Key):
-            return_keys = [return_keys]
-
-        assert_and_raise(isinstance(input_keys, (list, tuple)), TypeError(f"Input keys doesn't have the correct type; actual type: {type(input_keys)}"))
-        assert_and_raise(isinstance(return_keys, (list, tuple)), TypeError(f"Return keys doesn't have the correct type; actual type: {type(input_keys)}"))
-        return input_keys, return_keys
-
-    def _vaulter__populate_input_keys_from_signature(self, func, input_keys):
+    def _manual__populate_input_keys_from_signature(self, func, input_keys):
         signature = inspect.signature(func)
         faulty_params = list()
         keys = self.keyring_class.get_keys()
         for parameter in signature.parameters.values():
             valid_kind = parameter.kind == inspect.Parameter.POSITIONAL_OR_KEYWORD or parameter.kind == inspect.Parameter.KEYWORD_ONLY
 
             param_name = parameter.name
@@ -336,57 +268,97 @@
                     input_keys.append(self.keyring_class.get_key_by_matching_string(parameter.name))
             elif correct_default and param_name not in keys:
                 faulty_params.append((param_name, "You assigned the parameter a correct default value, but the parameter doesn't exist as a key in the keyring. "
                                                   "Did you make a typo in the parameter name? We'll be failing this for you because you more than likely made a mistake"))
         if faulty_params:
             raise AssertionError(f"Errors found in the signature: {faulty_params}")
 
-    def _vaulter__build_input_vars(self, input_keys, *all_flags, **kwargs):
+    def _manual__build_input_keys(self, input_keys, *all_flags, **kwargs):
         mini = self.get(input_keys, *all_flags)
         if Flags.is_set(Flags.input_key_can_be_missing, *all_flags):
             [mini.add(key, None) for key in input_keys if key not in mini]
 
         assert len(input_keys) == len(mini), \
             f"The number of items acquired from {self.get.__name__} is not the same as the number of input-keys to the method, " \
             f"which it should be. This is probably a bug."
 
         for key in mini.keys():
-            assert key not in kwargs, f"Key {key} seems to already exist in kwargs used for the function decorated with '@{self.vaulter.__name__}'"
+            assert key not in kwargs, f"Key {key} seems to already exist in kwargs used for the function decorated with '@{self.manual.__name__}'"
 
         return mini
 
-    def _vaulter__handle_return_vars(self, ret, return_keys, *all_flags):
+    # ============================================================
+    # automatic
+    # ============================================================
+    def automatic(self, *flags: Flags, input: Union[Key, List, Tuple] = None, output: Union[Key, List, Tuple] = None, condition: Callable = lambda: True, threaded: bool = False):
+        f"""
+        Registers a function as a subscriber to the vault. The function will be called AUTOMATICALLY whenever all of the given input_keys is inserted into the vault.
+        
+        Note that since this function runs within the context of varvault, there is no way to insert other arguments to the subscribed function, 
+        or to capture any of the return variables. If you need to do that, you can use the {self.manual} decorator instead.
+        
+        It's entirely possible to chain multiple automatic functions together that each depend on each other. They will run as soon as all of their input keys are configured in the vault. 
+        
+        :param input: Can be of type: {Key}, {list}, {tuple}. Default: {None}. Keys must be defined in the
+         keyring for this specific vault.
+        :param output: Can be of type: {Key}, {list}, {tuple}. Default: {None}. Keys must be defined in the
+         keyring for this specific vault.
+        :param condition: A function, like a lambda, that returns a boolean. If the function returns {False}, the subscriber will not be called even if the required keys exist in the vault.
+        :param threaded: If set to {True}, the subscriber will be called in a separate thread. This is useful if the function doesn't need to be monitored and takes long to run.
+        :param flags: Optional argument for defining some flags for this vaulted function. Flags that have an effect:
+         {Flags.debug},
+         {Flags.silent},
+         {Flags.input_key_can_be_missing},
+         {Flags.permit_modifications},
+         {Flags.split_output_keys},
+         {Flags.output_key_can_be_missing},
+         {Flags.clean_output_keys},
+         {Flags.no_error_logging},
+         {Flags.use_signature_for_input_keys},
+         {Flags.output_key_replaces_input_key},
+        """
+        input, output = self._convert_input_keys_and_output_keys(input, output)
 
-        if not return_keys:
-            # No return keys were defined; Just return from here then as there is nothing else to do.
-            return
+        assert_and_raise(all(isinstance(key, Key) for key in input),
+                         TypeError(f"input_keys must be of type {Key}, {List} or {Tuple}"))
 
-        if Flags.is_set(Flags.split_return_keys, *all_flags):
-            assert_and_raise(isinstance(ret, MiniVault),
-                             ValueError(f"If {Flags.split_return_keys} is defined, you MUST return values in the form of a {MiniVault} object or we cannot determine which keys go where"))
-            ret = MiniVault({key: value for key, value in ret.items() if key in return_keys})
-        if Flags.is_set(Flags.return_key_can_be_missing, *all_flags):
-            assert_and_raise(isinstance(ret, MiniVault),
-                             ValueError(f"If {Flags.return_key_can_be_missing} is defined, you MUST return values in the form of a {MiniVault} object or we "
-                                        f"cannot determine which keys should be assigned to the vault and which should be skipped."))
-        if Flags.is_set(Flags.clean_return_keys, *all_flags):
-            self._clean_return_keys(return_keys, *all_flags)
-        else:
-            mini = self._to_minivault(return_keys, ret, *all_flags)
+        assert_and_raise(not any(key in output for key in input),
+                         KeyError(f"input and output cannot contain the same keys. This would effectively mean that the function subscribes "
+                                  f"to itself and would run forever if {Flags.permit_modifications.name} is set, or crash if it's not set."))
 
-            async def validate_keys_in_mini_vault(key, can_be_missing=False):
-                assert key in mini or can_be_missing, f"Key {key} isn't present in MiniVault; keys in mini: {mini.keys()}. " \
-                                                      f"You can set the vault-flag {Flags.return_key_can_be_missing} to skip this validation step"
-            concurrent_execution(validate_keys_in_mini_vault, return_keys, can_be_missing=Flags.is_set(Flags.return_key_can_be_missing, *all_flags))
+        all_flags = self._get_all_flags(*flags)
 
-            async def validate_keys_in_return_keys(key):
-                assert key in return_keys, f"Key {key} isn't defined as a return-key; return keys: {return_keys}"
-            concurrent_execution(validate_keys_in_return_keys, mini.keys())
+        def wrap_outer(func):
 
-            self.insert_minivault(mini, *all_flags)
+            [key.usages.add_input(func) for key in input]
+            [key.usages.add_return(func) for key in output]
+            # Separate handling if the decorated function uses the coroutine API
+            if asyncio.iscoroutinefunction(func):
+                raise ValueError(f"Async subscriber functions do not work because async functions cannot truly run in the background. Use {self.automatic.__name__} with 'threaded={True}' instead.")
+
+            else:
+                f = self._inner_standard(func, *all_flags, input=input, output=output)
+            if threaded:
+                self.threaded_automatics.add(f)
+            self.keys_used_by_automatics[f] = list()
+            self.automatic_conditionals[f] = condition
+            for key in input:
+                if key not in self.functions_as_automatics:
+                    self.functions_as_automatics[key] = list()
+                self.functions_as_automatics[key].append(f)
+                self.keys_used_by_automatics[f].append(key)
+            self._dispatch_subscribers(input)
+            return f
+
+        return wrap_outer
+
+    def purge_stopped_thread(self, subscriber_thread: SubscriberThread):
+        if subscriber_thread in self.running_tasks:
+            self.logger.info(f"Removing stopped thread {subscriber_thread} from the running tasks")
+            self.running_tasks.remove(subscriber_thread)
 
     # ============================================================
     # insert
     # ============================================================
     def insert(self, key: Key, value: object, *flags: Flags):
         f"""
         Inserts a {value} into the vault mapped to {key}.
@@ -399,17 +371,17 @@
          {Flags.debug},
          {Flags.silent}
         """
         # Key must be as an iterable, but value doesn't have to be
         mini = self._to_minivault([key], value, *self._get_all_flags(*flags))
         self.insert_minivault(mini, *self._get_all_flags(*flags))
 
-    # ==================================================
+    # ============================================================
     # insert_minivault
-    # ==================================================
+    # ============================================================
     def insert_minivault(self, mini: MiniVault, *flags):
         f"""
         Inserts a {MiniVault} into the vault.
         
         :param mini: The {MiniVault} to insert into the vault. 
         :param flags: An optional set of flags to tweak the behavior of the insert. Flags that have an effect: 
          {Flags.permit_modifications},
@@ -437,27 +409,29 @@
         concurrent_execution(assert_key_and_value_may_be_inserted, mini.items())
 
         with self.lock:
             self.log("-------------------", all_flags=all_flags)
             self.log("Variables going in:", all_flags=all_flags)
             for ret_key, ret_value in mini.items():
                 self.log(f"<-- {ret_key}: ({type(ret_value)}) -- {ret_value}", all_flags=all_flags)
-            self.vault.put(mini)
+            self._put(mini)
+
             self.log("-----------------", all_flags=all_flags)
+        self._dispatch_subscribers(mini.keys())
 
     def _insert__assert_value_may_be_inserted(self, key: Key, value: object, modifications_permitted=False):
         # Validate that key doesn't already exist in the vault, or that modifications_permitted==True
-        assert key not in self or modifications_permitted, f"Key {key} already exists in the vault and modifications to existing variables are not permitted."
+        assert_and_raise(key not in self or modifications_permitted, KeyError(f"Key {key} already exists in the vault and modifications to existing variables are not permitted."))
 
         # Validate the type of the value to insert into the vault
         assert_and_raise(key.type_is_valid(value), ValueError(f"Key '{key}' requires type to be '{key.valid_type}', but type for value is '{type(value)}'."))
 
-    # ========================================================
+    # ============================================================
     # get
-    # ========================================================
+    # ============================================================
     @overload
     def get(self, key: Key, *flags: Flags, default=None) -> Any:
         f"""
         Get an object from the vault that is mapped to {key}. 
         
         :param key: The key to get an object for. Must be of type {Key}
         :param flags: An optional set of flags to tweak the behavior of the get. Flags that have an effect:
@@ -492,16 +466,16 @@
                 self._try_reload_from_file(*all_flags)
 
                 if not Flags.is_set(Flags.input_key_can_be_missing, *all_flags):
                     for key in keys:
                         assert_and_raise(key in self, KeyError(f"Key {key} is not mapped to an object in the vault; it appears to be missing in the vault. "
                                                                f"You can set the flag '{Flags.input_key_can_be_missing}' to avoid this, "
                                                                f"in which case the value will be {None}, or make sure a value is mapped to it. "
-                                                               f"Known functions/methods where this key is used as a return key: {key.usages.as_return}"))
-                [mini.update({key: self.vault.get(key)}) for key in keys if key in self]
+                                                               f"Known functions/methods where this key is used as an output key: {key.usages.as_return}"))
+                [mini.update({key: self[key]}) for key in keys if key in self]
             return mini
 
         def single(key, *flags, default=None):
             mv = multiple([key], *flags)
             if Flags.is_set(Flags.input_key_can_be_missing, *flags):
                 return mv.get(key, default)
             return mv.get(key)
@@ -510,40 +484,223 @@
         if isinstance(keys, (list, tuple)):
             return multiple(keys, *flags)
         elif isinstance(keys, Key):
             return single(keys, *flags, default=kwargs.get("default"))
         else:
             raise NotImplementedError(f"Type {type(keys)} is not supported for the 'get' method. Supported types are: {Key}, {list} and {tuple}.")
 
-    # =======================================================================
+    # ============================================================
     # lambdavaulter
-    # =======================================================================
+    # ============================================================
     def lambdavaulter(self,
                       lambda_func: Callable,
                       *flags: Flags,
                       input_keys: Union[Key, List[Key, ...], Tuple[Key, ...]] = None,
-                      return_keys: Union[Key, List[Key, ...], Tuple[Key, ...]] = None):
+                      output_keys: Union[Key, List[Key, ...], Tuple[Key, ...]] = None):
         f"""
         Function to wrap a lambda like you would decorate a function. 
         
-        Uses the {self.vaulter} function to wrap the lambda. See {self.vaulter} function for information about flags that have an effect on this function.
+        Uses the {self.manual} function to wrap the lambda. See {self.manual} function for information about flags that have an effect on this function.
         
         Why you would like to do this, who knows. But you can do it. 
         
         :param lambda_func: The lambda to wrap. 
         :param flags: A set of flags to use when wrapping the lambda. 
         :param input_keys: The keys to use as input for the lambda. 
-        :param return_keys: The keys to return from the lambda. 
+        :param output_keys: The keys to return from the lambda. 
         :return: A wrapped lambda. 
         """
-        return self.vaulter(*flags, input_keys=input_keys, return_keys=return_keys)(lambda_func)
+        return self.manual(*flags, input=input_keys, output=output_keys)(lambda_func)
 
-    # ==================================================
+    def await_running_tasks(self, timeout: float = 0, exception: Exception = None):
+        f"""
+        Wait for all running tasks to finish.
+        
+        :param timeout: The timeout in seconds to wait for all tasks to finish. Default is 0, which literally means 0 seconds. If this function is called with {timeout}=0, 
+         it means you expect all tasks to be finished by now. If you don't expect all tasks to be finished by now, you should probably set a timeout.
+        """
+        start = time.time()
+        while self.running_tasks:
+            if time.time() - start > timeout:
+                self.logger.info(f"Timeout of {timeout} seconds reached while waiting for no running tasks. ")
+                if exception:
+                    raise exception
+                raise TimeoutError(f"Timeout of {timeout} seconds reached while waiting for no running tasks.")
+
+    # ============================================================
     # privates
-    # ==================================================
+    # ============================================================
+
+    def _convert_input_keys_and_output_keys(self, input: Union[Key, List, Tuple], output: Union[Key, List, Tuple]) -> Tuple[List, List]:
+        input = input if input else list()
+        output = output if output else list()
+
+        # Validate the input to the decorator
+        self._validate_input(input, output)
+
+        if isinstance(input, Key):
+            input = [input]
+        if isinstance(output, Key):
+            output = [output]
+
+        assert_and_raise(isinstance(input, (list, tuple)), TypeError(f"Input keys doesn't have the correct type; actual type: {type(input)}"))
+        assert_and_raise(isinstance(output, (list, tuple)), TypeError(f"Output keys doesn't have the correct type; actual type: {type(output)}"))
+        return input, output
+
+    def _validate_input(self, input_keys, output_keys):
+        assert_and_raise(isinstance(input_keys, (Key, list, tuple)),
+                         TypeError(f"input_keys must be of type {Key}, {list}, or {tuple}"))
+        assert_and_raise(isinstance(output_keys, (Key, list, tuple)),
+                         TypeError(f"output_keys must be of type {Key}, {list}, or {tuple}"))
+
+    def _inner_async(self, func, *all_flags: Flags, input: List[Key] = None, output: List[Key] = None):
+        f"""Inner async wrapper for {self.manual}/{self.automatic} decorators"""
+        func_module_name = f"{func.__module__}.{func.__name__}"
+
+        @functools.wraps(func)
+        async def wrap_inner_async(*args, **kwargs):
+            #
+            # Do pre-call related stuff
+            #
+            input_kwargs = self._pre_call(input, func_module_name, *all_flags, **kwargs)
+            try:
+                ret = await func(*args, **input_kwargs)
+            except Exception as e:
+                if not Flags.is_set(Flags.no_error_logging, *all_flags):
+                    # Flag to not log error is NOT set, so we should log the error and then raise the error
+                    self.log(f"Failed to run {func_module_name}: {e}", level=logging.ERROR, all_flags=all_flags)
+                    self.log(str(traceback.format_exc()).rstrip("\n"), level=logging.ERROR, all_flags=all_flags)
+                raise
+
+            #
+            # Do post-call related stuff
+            #
+            self._post_call(ret, input, output, func_module_name, *all_flags)
+
+            return ret
+        return wrap_inner_async
+
+    def _inner_standard(self, func, *all_flags: Flags, input: List[Key] = None, output: List[Key] = None):
+        f"""Inner standard wrapper for {self.manual}/{self.automatic} decorators"""
+        func_module_name = f"{func.__module__}.{func.__name__}"
+
+        @functools.wraps(func)
+        def wrap_inner(*args, **kwargs):
+            #
+            # Do pre-call related stuff
+            #
+            input_kwargs = self._pre_call(input, func_module_name, *all_flags, **kwargs)
+
+            try:
+                ret = func(*args, **input_kwargs)
+            except Exception as e:
+                if not Flags.is_set(Flags.no_error_logging, *all_flags):
+                    # Flag to not log error is NOT set, so we should log the error and then raise the error
+                    self.log(f"Failed to run {func_module_name}: {e}", level=logging.ERROR, all_flags=all_flags)
+                    self.log(str(traceback.format_exc()).rstrip("\n"), level=logging.ERROR, all_flags=all_flags)
+                raise
+
+            #
+            # Do post-call related stuff
+            #
+            self._post_call(ret, input, output, func_module_name, *all_flags)
+
+            return ret
+        return wrap_inner
+
+    def _pre_call(self, input: Union[List[Key], Tuple[Key]], func_module_name: str, *all_flags: Flags, **kwargs):
+        input_kwargs = self._manual__build_input_keys(input, *all_flags, **kwargs)
+        kwargs.update(input_kwargs)
+
+        self.log(f"======{'=' * len(func_module_name)}=", all_flags=all_flags)
+        self.log(f">>>>> {func_module_name}:", all_flags=all_flags)
+        if input_kwargs:
+            self.log(f"-------------", all_flags=all_flags)
+            self.log(f"Input kwargs:", all_flags=all_flags)
+            for kwarg_key, kwarg_value in input_kwargs.items():
+                self.log(f"--> {kwarg_key}: ({type(kwarg_value)}) -- {kwarg_value}", all_flags=all_flags)
+            self.log(f"-------------", all_flags=all_flags)
+        input_kwargs.update(kwargs)
+
+        self.log(f"======= Calling {func_module_name} ========", all_flags=all_flags)
+        return input_kwargs
+
+    def _post_call(self, ret, input_keys, output_keys, func_module_name, *all_flags: Flags):
+        self._handle_output_keys(ret, input_keys, output_keys, *all_flags)
+        self.log(f"<<<<< {func_module_name}:", all_flags=all_flags)
+        self.log(f"======{'=' * len(func_module_name)}=\n", all_flags=all_flags)
+        self._reset_log_levels()
+
+    def _handle_output_keys(self, ret, input_keys, output_keys, *all_flags):
+
+        if not output_keys:
+            # No output keys were defined; Just return from here then as there is nothing else to do.
+            return
+
+        if Flags.is_set(Flags.split_output_keys, *all_flags):
+            assert_and_raise(isinstance(ret, MiniVault),
+                             ValueError(f"If {Flags.split_output_keys} is defined, you MUST return values in the form of a {MiniVault} object or we cannot determine which keys go where"))
+            ret = MiniVault({key: value for key, value in ret.items() if key in output_keys})
+        if Flags.is_set(Flags.output_key_can_be_missing, *all_flags):
+            assert_and_raise(isinstance(ret, MiniVault),
+                             ValueError(f"If {Flags.output_key_can_be_missing} is defined, you MUST return values in the form of a {MiniVault} object or we "
+                                        f"cannot determine which keys should be assigned to the vault and which should be skipped."))
+        if Flags.is_set(Flags.clean_output_keys, *all_flags):
+            self._clean_output_keys(output_keys, *all_flags)
+        else:
+            mini = self._to_minivault(output_keys, ret, *all_flags)
+            if Flags.is_set(Flags.output_key_replaces_input_key, *all_flags):
+                assert_and_raise(len(input_keys) == 1 and len(output_keys) == 1, ValueError(f"If {Flags.output_key_replaces_input_key} is defined, you MUST define "
+                                                                                            f"exactly one input key and one output key."))
+                del self[input_keys[0]]
+
+            async def validate_keys_in_mini_vault(key, can_be_missing=False):
+                assert key in mini or can_be_missing, f"Key {key} isn't present in MiniVault; keys in mini: {mini.keys()}. " \
+                                                      f"You can set the vault-flag {Flags.output_key_can_be_missing} to skip this validation step"
+            concurrent_execution(validate_keys_in_mini_vault, output_keys, can_be_missing=Flags.is_set(Flags.output_key_can_be_missing, *all_flags))
+
+            async def validate_keys_in_output_keys(key):
+                assert key in output_keys, f"Key {key} isn't defined as an output-key; output keys: {output_keys}"
+            concurrent_execution(validate_keys_in_output_keys, mini.keys())
+
+            self.insert_minivault(mini, *all_flags)
+
+    def _dispatch_subscribers(self, keys: List[Key]):
+        potential_functions_to_dispatch = set()
+        functions_to_dispatch = set()
+        threaded_functions_to_dispatch = set()
+        for key in keys:
+            functions = self.functions_as_automatics.get(key, [])
+            for function in functions:
+                potential_functions_to_dispatch.add(function)
+        for function in potential_functions_to_dispatch:
+            keys_that_must_be_in_vault = self.keys_used_by_automatics.get(function, [])
+            may_dispatch = True
+            for key in keys_that_must_be_in_vault:
+                if key not in self:
+                    # Key does not exist in vault. Dispatch is impossible.
+                    may_dispatch = False
+                    break
+            if may_dispatch:
+                conditional: Callable = self.automatic_conditionals[function]
+                if conditional():
+                    if function in self.threaded_automatics:
+                        threaded_functions_to_dispatch.add(function)
+                    else:
+                        functions_to_dispatch.add(function)
+        for function in threaded_functions_to_dispatch:
+            # Dispatch threaded functions.
+            thread = SubscriberThread(function, self)
+            self.running_tasks.add(thread)
+            thread.start()
+
+        for function in functions_to_dispatch:
+            # Dispatch the function.
+            function()
+
     def _get_all_flags(self, *flags):
         self._assert_flag_is_correct_type(*flags)
         all_flags = self.flags.copy()
         all_flags.update(flags)
         return all_flags
 
     def _assert_flag_is_correct_type(self, *flags: Flags):
@@ -565,46 +722,46 @@
     def _try_reload_from_file(self, *all_flags: Flags):
         """Can be used to reload from a file if changes has been made to it since it was read last time."""
         if self.resource and self.resource.mode_properties.live_update:
             if not self.resource.resource_has_changed():
                 return
             self.log(f"Reloading from {self.resource.path}; The content has changed and live-update is enabled.", all_flags=all_flags)
             mv = self.resource.create_mv(**self.keys)
-            self.vault.put(mv)
+            self._put(mv)
 
-    def _clean_return_keys(self, return_keys: Union[List[Key], Tuple[Key]], *all_flags: Flags):
-        self.log(f"Cleaning return var keys: {return_keys}", all_flags=all_flags)
-        for key in return_keys:
+    def _clean_output_keys(self, output_keys: Union[List[Key], Tuple[Key]], *all_flags: Flags):
+        self.log(f"Cleaning output keys: {output_keys}", all_flags=all_flags)
+        for key in output_keys:
             if not key.valid_type:
                 temp = None
                 self.log(f"Cleaning key {key} by setting it to None (no valid_type defined for {key})", all_flags=all_flags)
             else:
                 try:
                     temp = key.valid_type()
                     self.log(f"Cleaning key {key} by setting it to '{temp}' (key.valid_type = {key.valid_type})", all_flags=all_flags)
                 except:
                     temp = None
                     self.log(f"Cleaning key {key} by setting it to '{None}' (valid_type is defined, but no default constructor appears to exist for {key.valid_type})", all_flags=all_flags)
-            self.vault.put(key, temp)
+            self._put(key, temp)
 
-    def _to_minivault(self, return_keys, ret, *all_flags) -> MiniVault:
+    def _to_minivault(self, output_keys, ret, *all_flags) -> MiniVault:
         if isinstance(ret, MiniVault):
             mini = ret
         else:
             # It's not a MiniVault; Let's turn it into one.
             if isinstance(ret, tuple):
                 # It's a tuple, which means it's either meant as a single item, or there are multiple return objects
-                if len(return_keys) == 1:
-                    # There's only one return key defined, which means the keys valid type should be tuple, OR the flag return_tuple_is_single_item is set
-                    assert return_keys[0].valid_type == tuple or Flags.is_set(Flags.return_tuple_is_single_item, *all_flags), \
-                        f"You have defined only a single return key, yet you are returning multiple items, while the valid type for key " \
-                        f"{self.keyring_class.__name__}.{return_keys[0]} is not {tuple}, nor is {Flags.return_tuple_is_single_item} set."
+                if len(output_keys) == 1:
+                    # There's only one output key defined, which means the keys valid type should be tuple, OR the flag return_tuple_is_single_item is set
+                    assert output_keys[0].valid_type == tuple or Flags.is_set(Flags.return_tuple_is_single_item, *all_flags), \
+                        f"You have defined only a single output key, yet you are returning multiple items, while the valid type for key " \
+                        f"{self.keyring_class.__name__}.{output_keys[0]} is not {tuple}, nor is {Flags.return_tuple_is_single_item} set."
 
-                    mini = MiniVault.build(return_keys, [ret])
+                    mini = MiniVault.build(output_keys, [ret])
                 else:
-                    assert len(return_keys) == len(ret), "The number of return variables and the number of return keys must be identical in order to map the keys to the return variables"
-                    mini = MiniVault.build(return_keys, ret)
+                    assert len(output_keys) == len(ret), "The number of returned variables and the number of output keys must be identical in order to map the keys to the returned variables"
+                    mini = MiniVault.build(output_keys, ret)
             else:
                 # ret is a single item
-                assert len(return_keys) == 1, "There appear to be more than 1 return-key defined, but only a single item that is returned"
-                mini = MiniVault.build(return_keys, [ret])
+                assert len(output_keys) == 1, "There appear to be more than 1 return-key defined, but only a single item that is returned"
+                mini = MiniVault.build(output_keys, [ret])
         return mini
```

### Comparing `varvault-5.0.3/varvault/vaultstructs.py` & `varvault-6.0.0/varvault/vaultstructs.py`

 * *Files identical despite different names*

### Comparing `varvault-5.0.3/varvault.egg-info/PKG-INFO` & `varvault-6.0.0/varvault.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvault
-Version: 5.0.3
+Version: 6.0.0
 Summary: A package that sets up a key-value vault to store and access variables in a global context.
 Home-page: https://github.com/data-ductus/varvault
 Author: Chloe Holst
 Author-email: chloe.holst@dataductus.se
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -20,99 +20,100 @@
 
 ### Install
 ```
 pip3 install varvault
 ```
 
 ### Contact
-calle.holst@dataductus.se
+chloe.holst@dataductus.se
 
 
 ## What is this? 
 This is a package that allows you to create a key-value vault for storing variables in a global context. It allows 
 you to set up a keyring with pre-defined constants which act as keys for the vault. These constants are then what is 
 stored inside the vault. A key is just a string, but the value that the key is mapped to can be assigned to any type of 
 object in Python. If the object is serializable (like a list or a dict), it can also be writen to something like a JSON file.    
 You can then use a decorator to annotate functions that you want to have use this vault to either store return variables 
 in or to extract variables to be used as input for the function.  
 
 ## How does it work? 
-The way this works is that when you write a function, you annotate it with a special decorator (`varvault.Vault.vaulter`)
-that takes some arguments. This decorator will then handle any input arguments and return variables for you.
+The way this works is that when you write a function, you annotate it with a special decorator (`varvault.Vault.manual` or `varvault.Vault.automatic`)
+that takes some arguments. The decorator will then handle any input arguments and return variables for you.
 The decorator takes some arguments that defines certain keys and flags to tweak the behavior.
 
 ### How about an example?
-The best examples can be found in the test suites which can give a very good idea how it works and is guaranteed to be up-to-date. 
+The best examples can be found in the test suites which can give a very good idea how it works and is guaranteed to be up-to-date.
+
 ```python
 import varvault
 
 
 class Keyring(varvault.Keyring):
-    arg1 = varvault.Key("arg1", valid_type=int)
-    arg2 = varvault.Key("arg2", valid_type=int)
+   arg1 = varvault.Key("arg1", valid_type=int)
+   arg2 = varvault.Key("arg2", valid_type=int)
 
 
 vault = varvault.create(keyring=Keyring, resource=varvault.JsonResource("~/test.json", mode=varvault.ResourceModes.WRITE))
 
 
-@vault.vaulter(return_keys=[Keyring.arg1, Keyring.arg2])
+@vault.manual(output=(Keyring.arg1, Keyring.arg2))
 def create_args(arg1, arg2):
-    return arg1, arg2
+   return arg1, arg2
 
 
-@vault.vaulter(input_keys=[Keyring.arg1, Keyring.arg2])
+@vault.manual(input=(Keyring.arg1, Keyring.arg2))
 def use_args(arg1: int = varvault.AssignedByVault, arg2: int = varvault.AssignedByVault):
-    print(f"{Keyring.arg1}: {arg1}, {Keyring.arg2}: {arg2}")
+   print(f"{Keyring.arg1}: {arg1}, {Keyring.arg2}: {arg2}")
 
 
 def run_create_args():
-    create_args(1, 2)
-    
+   create_args(1, 2)
+
 
 def run_use_args():
-    use_args()
+   use_args()
 
 
 if __name__ == "__main__":
-    run_create_args()
-    
-    run_use_args()    
+   run_create_args()
+
+   run_use_args()    
 ```
 1. In this example, we start by creating a class that defines a keyring. This keyring will be the keys used
    in the vault. Any key you use for storing variables or take variables out should be defined as a constant 
    in this keyring (by default, this is the way to use it, but it is possible to be more flexible).
 
 2. Then we create the actual Vault-object. It's entirely possible to create a Vault without using the factory function,
    but the factory function will do some things for you to make it slightly easier. Creating the vault requires only
    a single argument to be defined and that is a class that inherits from the `varvault.Keyring` (a class based on the Keyring class here).
    Optionally, you can define some flags to further tweak the behavior of the vault. These tweaked behaviors include
    allowing for existing key-value pairs to be modified (this is not allowed by default), allowing return variables from
-   functions defined with return keys to be None, and setting a flag to write some additional debug logs.
+   functions defined with output keys to be `None`, and setting a flag to write some additional debug logs.
    We also define the input parameter `resource` which is a `varvault.JsonResource` object that points to a `.JSON` file. This resource will be used  
    as a vault file to store all the arguments in. 
 
 3. We define a function called `create_args` that takes some arguments (we have to insert variables
    into the vault somehow, right?) that we annotate with the vault decorator. We pass an argument to the
-   decorator called `return_keys`. This argument tells the vault which keys this function will assign its
-   return variables to. Note that the order of the return keys matter. In this case, the ingoing argument `arg1` will
+   decorator called `ouput`. This argument tells the vault which keys this function will assign its
+   return variables to. Note that the order of the output keys matter. In this case, the ingoing argument `arg1` will
    be assigned to `Keyring.arg1`, and the ingoing argument `arg2` will be assigned to `Keyring.arg2`. It's very possible
-   to set `return_keys` to a single `Key` as well if you only have one variable to return. If you want more control
+   to set `output` to a single `Key` as well if you only have one variable to return. If you want more control
    over how return variables are handled, please see `varvault.MiniVault` and make use of that to ensure that
    return-variables are handled exactly as you want. 
    
    **Note:** When this function is called, and it finishes, the decorator here will capture the return variables and then store 
-   those return variables in the vault with the keys that were passed to the decorator as `return_keys`. These variables can then be 
+   those return variables in the vault with the keys that were passed to the decorator as `output`. These variables can then be 
    accessed by another function that uses the same vault-object as this one does to decorate a function.
 
 4. We then create a new function called `use_args` that we also annotate with the vault decorator. We pass a different
-   argument to the decorator this time called `input_keys`. This argument tells the vault which keys in the vault
+   argument to the decorator this time called `input`. This argument tells the vault which keys in the vault
    we want passed to this function. The order of the keys doesn't really matter here, the order is mostly aesthetic.
    
    **Note:** What ends up happening when this function is called, is that the decorator will try to extract keys defined in
-   `input_keys` from the vault and then pass those variables to the function as a dictionary (by defining the arguments as
+   `input` from the vault and then pass those variables to the function as a dictionary (by defining the arguments as
    keyword arguments, these arguments won't need to be provided when the method is called). 
    It is possible to just bundle all the arguments in the signature of the function as a `**kwargs` structure (in this case the signature
    would be `def use_args(**kwargs)`). One of the benefits of doing like in the example is that you can easily see what 
    arguments will be provided by the vault when you use the function, so you know which arguments you have to provide and which are provided by the vault.
 
 5. We create a very simple function called `run_create_args` which doesn't get annotated. This function is simply made
    to demonstrate what makes this vault so useful. When this function is called, it will obviously call `create_args`,
@@ -141,15 +142,15 @@
        arg2 = varvault.Key("arg2")
       
    vault = varvault.create(varvault.Flags.permit_modifications, 
                            keyring=Keyring,                           
                            resource=varvault.JsonResource("~/test.json", mode=varvault.ResourceModes.APPEND))
    ```
    When re-creating a vault from an existing file it's recommended to allow modifications 
-   (see `varvault.VaultFlags.permit_modifications`) in-case you are planning to write the same
+   (see `varvault.Flags.permit_modifications`) in-case you are planning to write the same
    arguments to the vault again. 
 
 ## Conclusion
 This README demonstrates what this functionality can be used for. With this vault, the context for where
 a function executes doesn't matter as long as the keys the function require have been assigned in the vault and the
 functions exists in the scope. The functions become building blocks that you can call regardless of context provided
 the above criteria have been met. You don't need to clutter your main function calls with tons of input variables being passed around
```

### Comparing `varvault-5.0.3/varvault.egg-info/SOURCES.txt` & `varvault-6.0.0/varvault.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE
 README.md
 setup.py
+tests/test_automatic.py
 tests/test_large_scale_vault.py
 tests/test_live_update.py
 tests/test_logging.py
 tests/test_structs.py
 tests/test_vault.py
 tests/test_xml_vault.py
 varvault/__init__.py
 varvault/factory.py
 varvault/flags.py
 varvault/keyring.py
 varvault/logger.py
 varvault/minivault.py
 varvault/resource.py
+varvault/subscriber_thread.py
 varvault/utils.py
 varvault/validator.py
 varvault/vault.py
 varvault/vaultstructs.py
 varvault.egg-info/PKG-INFO
 varvault.egg-info/SOURCES.txt
 varvault.egg-info/dependency_links.txt
```

