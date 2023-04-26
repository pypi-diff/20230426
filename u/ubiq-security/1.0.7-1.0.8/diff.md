# Comparing `tmp/ubiq-security-1.0.7.tar.gz` & `tmp/ubiq-security-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ubiq-security-1.0.7.tar", last modified: Wed Oct 28 23:46:53 2020, max compression
+gzip compressed data, was "dist/ubiq-security-1.0.8.tar", last modified: Mon Jan 18 22:15:36 2021, max compression
```

## Comparing `ubiq-security-1.0.7.tar` & `ubiq-security-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gary      (1000) gary      (1000)        0 2020-10-28 23:46:53.000000 ubiq-security-1.0.7/
--rw-r--r--   0 gary      (1000) gary      (1000)       38 2020-10-28 23:46:53.000000 ubiq-security-1.0.7/setup.cfg
--rw-r--r--   0 gary      (1000) gary      (1000)     1742 2020-10-28 23:43:02.000000 ubiq-security-1.0.7/setup.py
--rw-r--r--   0 gary      (1000) gary      (1000)       27 2020-08-10 21:43:24.000000 ubiq-security-1.0.7/requirements.txt
--rw-r--r--   0 gary      (1000) gary      (1000)     7724 2020-10-28 23:46:53.000000 ubiq-security-1.0.7/PKG-INFO
--rw-r--r--   0 gary      (1000) gary      (1000)      372 2020-10-28 23:44:09.000000 ubiq-security-1.0.7/CHANGELOG.md
-drwxr-xr-x   0 gary      (1000) gary      (1000)        0 2020-10-28 23:46:53.000000 ubiq-security-1.0.7/examples/
--rw-r--r--   0 gary      (1000) gary      (1000)       77 2020-10-28 23:42:53.000000 ubiq-security-1.0.7/examples/credentials
--rw-r--r--   0 gary      (1000) gary      (1000)    11582 2020-09-14 23:58:03.000000 ubiq-security-1.0.7/examples/ubiq_sample.py
--rw-r--r--   0 gary      (1000) gary      (1000)     2575 2020-08-19 18:12:24.000000 ubiq-security-1.0.7/examples/README.md
--rw-r--r--   0 gary      (1000) gary      (1000)     1104 2020-10-28 23:43:02.000000 ubiq-security-1.0.7/LICENSE
-drwxr-xr-x   0 gary      (1000) gary      (1000)        0 2020-10-28 23:46:53.000000 ubiq-security-1.0.7/ubiq_security.egg-info/
--rw-r--r--   0 gary      (1000) gary      (1000)      483 2020-10-28 23:46:53.000000 ubiq-security-1.0.7/ubiq_security.egg-info/SOURCES.txt
--rw-r--r--   0 gary      (1000) gary      (1000)       14 2020-10-28 23:46:53.000000 ubiq-security-1.0.7/ubiq_security.egg-info/top_level.txt
--rw-r--r--   0 gary      (1000) gary      (1000)        1 2020-10-28 23:46:53.000000 ubiq-security-1.0.7/ubiq_security.egg-info/dependency_links.txt
--rw-r--r--   0 gary      (1000) gary      (1000)     7724 2020-10-28 23:46:53.000000 ubiq-security-1.0.7/ubiq_security.egg-info/PKG-INFO
--rw-r--r--   0 gary      (1000) gary      (1000)       26 2020-10-28 23:46:53.000000 ubiq-security-1.0.7/ubiq_security.egg-info/requires.txt
--rw-r--r--   0 gary      (1000) gary      (1000)     5259 2020-09-15 21:53:19.000000 ubiq-security-1.0.7/README.md
-drwxr-xr-x   0 gary      (1000) gary      (1000)        0 2020-10-28 23:46:53.000000 ubiq-security-1.0.7/ubiq_security/
--rw-r--r--   0 gary      (1000) gary      (1000)     5455 2020-10-28 23:43:02.000000 ubiq-security-1.0.7/ubiq_security/auth.py
--rw-r--r--   0 gary      (1000) gary      (1000)     8027 2020-10-28 23:43:02.000000 ubiq-security-1.0.7/ubiq_security/encrypt.py
--rw-r--r--   0 gary      (1000) gary      (1000)     3843 2020-10-28 23:43:02.000000 ubiq-security-1.0.7/ubiq_security/algorithm.py
--rw-r--r--   0 gary      (1000) gary      (1000)       18 2020-10-28 23:44:48.000000 ubiq-security-1.0.7/ubiq_security/version.py
--rw-r--r--   0 gary      (1000) gary      (1000)    13080 2020-10-28 23:43:02.000000 ubiq-security-1.0.7/ubiq_security/decrypt.py
--rw-r--r--   0 gary      (1000) gary      (1000)      226 2020-10-28 23:43:02.000000 ubiq-security-1.0.7/ubiq_security/__init__.py
--rw-r--r--   0 gary      (1000) gary      (1000)     3743 2020-10-28 23:43:02.000000 ubiq-security-1.0.7/ubiq_security/credentials.py
+drwxr-xr-x   0 gary      (1000) gary      (1000)        0 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/
+-rw-r--r--   0 gary      (1000) gary      (1000)       38 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/setup.cfg
+-rw-r--r--   0 gary      (1000) gary      (1000)     1742 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/setup.py
+-rw-r--r--   0 gary      (1000) gary      (1000)       27 2020-08-26 05:35:52.000000 ubiq-security-1.0.8/requirements.txt
+-rw-r--r--   0 gary      (1000) gary      (1000)     7724 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/PKG-INFO
+-rw-r--r--   0 gary      (1000) gary      (1000)      448 2021-01-18 22:11:45.000000 ubiq-security-1.0.8/CHANGELOG.md
+drwxr-xr-x   0 gary      (1000) gary      (1000)        0 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/examples/
+-rw-r--r--   0 gary      (1000) gary      (1000)       77 2021-01-18 22:05:49.000000 ubiq-security-1.0.8/examples/credentials
+-rw-r--r--   0 gary      (1000) gary      (1000)    11701 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/examples/ubiq_sample.py
+-rw-r--r--   0 gary      (1000) gary      (1000)     2575 2020-08-26 05:35:52.000000 ubiq-security-1.0.8/examples/README.md
+-rw-r--r--   0 gary      (1000) gary      (1000)     1104 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/LICENSE
+drwxr-xr-x   0 gary      (1000) gary      (1000)        0 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security.egg-info/
+-rw-r--r--   0 gary      (1000) gary      (1000)      483 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security.egg-info/SOURCES.txt
+-rw-r--r--   0 gary      (1000) gary      (1000)       14 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security.egg-info/top_level.txt
+-rw-r--r--   0 gary      (1000) gary      (1000)        1 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security.egg-info/dependency_links.txt
+-rw-r--r--   0 gary      (1000) gary      (1000)     7724 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security.egg-info/PKG-INFO
+-rw-r--r--   0 gary      (1000) gary      (1000)       26 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security.egg-info/requires.txt
+-rw-r--r--   0 gary      (1000) gary      (1000)     5259 2020-09-18 18:46:45.000000 ubiq-security-1.0.8/README.md
+drwxr-xr-x   0 gary      (1000) gary      (1000)        0 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security/
+-rw-r--r--   0 gary      (1000) gary      (1000)     5455 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/ubiq_security/auth.py
+-rw-r--r--   0 gary      (1000) gary      (1000)     8027 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/ubiq_security/encrypt.py
+-rw-r--r--   0 gary      (1000) gary      (1000)     3843 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/ubiq_security/algorithm.py
+-rw-r--r--   0 gary      (1000) gary      (1000)       18 2021-01-18 22:10:59.000000 ubiq-security-1.0.8/ubiq_security/version.py
+-rw-r--r--   0 gary      (1000) gary      (1000)    13080 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/ubiq_security/decrypt.py
+-rw-r--r--   0 gary      (1000) gary      (1000)      226 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/ubiq_security/__init__.py
+-rw-r--r--   0 gary      (1000) gary      (1000)     4750 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/ubiq_security/credentials.py
```

### Comparing `ubiq-security-1.0.7/setup.py` & `ubiq-security-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-1.0.7/PKG-INFO` & `ubiq-security-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiq-security
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python client library for accessing Ubiq Platform
 Home-page: https://gitlab.com/ubiqsecurity/ubiq-python
 Author: Ubiq Security, Inc.
 Author-email: support@ubiqsecurity.com
 License: Free To Use But Restricted
 Description: # Ubiq Security Python Library
```

### Comparing `ubiq-security-1.0.7/examples/ubiq_sample.py` & `ubiq-security-1.0.8/examples/ubiq_sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,16 +162,16 @@
     except KeyboardInterrupt:
         ### handle keyboard interrupt ###
         return False
     except Exception as e:
         if DEBUG or TESTRUN:
             raise(e)
         indent = len(program_name) * " "
-        sys.stderr.write(program_name + ": " + repr(e) + "\n")
-        sys.stderr.write(indent + "  for help use --help")
+        sys.stderr.write(program_name + ": {0}\n".format(e))
+        sys.stderr.write(indent + "  For help use --help\n")
         return False
 
 def simple_encryption(infile, outfile, creds):
     ''' Sample of the Ubiq Platform using the simple encryption API.'''
     data = infile.read()
     try:
        ct = ubiq.encrypt(creds,
@@ -261,29 +261,32 @@
         except:
            pass
         print("Error performing decryption: ", msg )
 
 # Main For the application
 if __name__ == "__main__":
 
-    # Parse the args and return the necessary information.  An error during
-    # parsing or testing the input / output files will result in valid_args
-    # being false which will prevent commands from being executed.        
-    valid_args, encryption, simple, infile, outfile, creds = parse_args()
-    
-    # If the arguments were valid, then process the encrypt or decrypt and 
-    # use either the simple or piecewise APIs
-    if valid_args:
-        if simple:
-            if encryption:
-                status = simple_encryption(infile, outfile, creds) 
-            else:
-                status = simple_decryption(infile, outfile, creds)
-        else:
-            if encryption:
-                status = piecewise_encryption(infile, outfile, creds) 
+    try:
+        # Parse the args and return the necessary information.  An error during
+        # parsing or testing the input / output files will result in valid_args
+        # being false which will prevent commands from being executed.
+        valid_args, encryption, simple, infile, outfile, creds = parse_args()
+
+        # If the arguments were valid, then process the encrypt or decrypt and
+        # use either the simple or piecewise APIs
+        if valid_args:
+            if simple:
+                if encryption:
+                    status = simple_encryption(infile, outfile, creds)
+                else:
+                    status = simple_decryption(infile, outfile, creds)
             else:
-                status = piecewise_decryption(infile, outfile, creds)
-        infile.close()
-        outfile.close()
-        
+                if encryption:
+                    status = piecewise_encryption(infile, outfile, creds)
+                else:
+                    status = piecewise_decryption(infile, outfile, creds)
+            infile.close()
+            outfile.close()
+    except Exception as inst:
+        valid_args = False
+
     sys.exit(valid_args == True)
```

### Comparing `ubiq-security-1.0.7/examples/README.md` & `ubiq-security-1.0.8/examples/README.md`

 * *Files identical despite different names*

### Comparing `ubiq-security-1.0.7/LICENSE` & `ubiq-security-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ubiq-security-1.0.7/ubiq_security.egg-info/PKG-INFO` & `ubiq-security-1.0.8/ubiq_security.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiq-security
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python client library for accessing Ubiq Platform
 Home-page: https://gitlab.com/ubiqsecurity/ubiq-python
 Author: Ubiq Security, Inc.
 Author-email: support@ubiqsecurity.com
 License: Free To Use But Restricted
 Description: # Ubiq Security Python Library
```

### Comparing `ubiq-security-1.0.7/README.md` & `ubiq-security-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ubiq-security-1.0.7/ubiq_security/auth.py` & `ubiq-security-1.0.8/ubiq_security/auth.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-1.0.7/ubiq_security/encrypt.py` & `ubiq-security-1.0.8/ubiq_security/encrypt.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-1.0.7/ubiq_security/algorithm.py` & `ubiq-security-1.0.8/ubiq_security/algorithm.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-1.0.7/ubiq_security/decrypt.py` & `ubiq-security-1.0.8/ubiq_security/decrypt.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-1.0.7/ubiq_security/credentials.py` & `ubiq-security-1.0.8/ubiq_security/credentials.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     secret_crypto_access_key = property(get_secret_crypto_access_key)
 
     def get_host(self):
         return self.__host
     host = property(get_host)
 
     def set(self):
-        return (self.__access_key_id != None and self.__secret_signing_key != None and self.__secret_crypto_access_key != None)
+        return (self.__access_key_id != None and self.__secret_signing_key != None and self.__secret_crypto_access_key != None and 
+            self.__access_key_id.strip() != "" and self.__secret_signing_key.strip() != "" and self.__secret_crypto_access_key.strip() != "")
 
 class configCredentials(credentialsInfo):
 
     def load_config_file(self, config_file, profile):
         config = configparser.ConfigParser()
         config.read(config_file)
 
@@ -70,15 +71,20 @@
 
         if os.path.exists(config_file):
             self.load_config_file(config_file, profile)
 
         credentialsInfo.__init__(self, self.__access_key_id , self.__secret_signing_key, self.__secret_crypto_access_key, self.__host)
 
         if (not self.set()):
-            raise RuntimeError("Unable to open config file '{0}' or contains missing values.  ".format(config_file))
+            if (self.__access_key_id == None or self.__access_key_id.strip() == ""):
+               raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'acess_key_id' value in profile '{1}' or through environment variable for 'UBIQ_ACCESS_KEY_ID'.".format(config_file, profile))
+            elif (self.__secret_signing_key == None or self.__secret_signing_key.strip() == ""):
+               raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'secret_signing_key' value in profile '{1}' or through environment variable for 'UBIQ_SECRET_SIGNING_KEY'.".format(config_file, profile))
+            elif(self.__secret_crypto_access_key == None or self.__secret_crypto_access_key.strip() == ""):
+               raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'secret_crypto_access_key' value in profile '{1}' or through environment variable for 'UBIQ_SECRET_CRYPTO_ACCESS_KEY'.".format(config_file, profile))
 
 
 class credentials(credentialsInfo):
 
     def __init__(self, access_key_id = None, secret_signing_key = None, secret_crypto_access_key = None, host = UBIQ_HOST):
         # If supplied value is None, use ENV variable, otherwise use supplied value.
         # If env value isn't set, use the supplied value anyways (None) but prevent an exception
```

