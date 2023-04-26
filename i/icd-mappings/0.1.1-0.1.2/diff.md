# Comparing `tmp/icd_mappings-0.1.1.tar.gz` & `tmp/icd_mappings-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icd_mappings-0.1.1.tar", max compression
+gzip compressed data, was "icd_mappings-0.1.2.tar", max compression
```

## Comparing `icd_mappings-0.1.1.tar` & `icd_mappings-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1959 2023-03-15 14:59:53.227631 icd_mappings-0.1.1/README.md
--rw-r--r--   0        0        0       31 2023-03-15 14:37:28.554849 icd_mappings-0.1.1/icdmappings/__init__.py
--rw-r--r--   0        0        0     2092 2023-03-15 14:48:19.512378 icd_mappings-0.1.1/icdmappings/icdmappings.py
--rw-r--r--   0        0        0      382 2023-03-15 14:37:12.884893 icd_mappings-0.1.1/icdmappings/mappers/__init__.py
--rw-r--r--   0        0        0     1885 2023-03-15 14:45:53.879281 icd_mappings-0.1.1/icdmappings/mappers/icd10_to_icd9.py
--rw-r--r--   0        0        0     2452 2023-03-15 14:45:53.879689 icd_mappings-0.1.1/icdmappings/mappers/icd9_to_cci.py
--rw-r--r--   0        0        0     4780 2023-03-15 14:45:53.880197 icd_mappings-0.1.1/icdmappings/mappers/icd9_to_ccs.py
--rw-r--r--   0        0        0     3333 2023-03-15 14:45:53.881086 icd_mappings-0.1.1/icdmappings/mappers/icd9_to_chapters.py
--rw-r--r--   0        0        0     1956 2023-03-15 14:45:53.881708 icd_mappings-0.1.1/icdmappings/mappers/icd9_to_icd10.py
--rw-r--r--   0        0        0      729 2023-03-15 14:45:53.882241 icd_mappings-0.1.1/icdmappings/mappers/icd9_to_level3.py
--rw-r--r--   0        0        0     1096 2023-03-15 14:45:47.834508 icd_mappings-0.1.1/icdmappings/mappers/lol.ipynb
--rw-r--r--   0        0        0      472 2023-03-15 14:45:53.882877 icd_mappings-0.1.1/icdmappings/mappers/mapper_interface.py
--rw-r--r--   0        0        0      100 2023-03-14 10:04:00.087660 icd_mappings-0.1.1/icdmappings/validators/__init__.py
--rw-r--r--   0        0        0     3233 2023-03-15 14:45:53.883649 icd_mappings-0.1.1/icdmappings/validators/icd9_validator.py
--rw-r--r--   0        0        0      686 2023-03-15 14:45:53.884114 icd_mappings-0.1.1/icdmappings/validators/icd_validator_interface.py
--rw-r--r--   0        0        0      601 2023-03-15 15:21:35.550466 icd_mappings-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 icd_mappings-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1992 2023-04-26 11:33:59.681730 icd_mappings-0.1.2/README.md
+-rw-r--r--   0        0        0       31 2023-03-15 14:37:28.554849 icd_mappings-0.1.2/icdmappings/__init__.py
+-rw-r--r--   0        0        0     2092 2023-04-26 11:39:27.537862 icd_mappings-0.1.2/icdmappings/icdmappings.py
+-rw-r--r--   0        0        0      382 2023-03-15 14:37:12.884893 icd_mappings-0.1.2/icdmappings/mappers/__init__.py
+-rw-r--r--   0        0        0     1885 2023-03-15 14:45:53.879281 icd_mappings-0.1.2/icdmappings/mappers/icd10_to_icd9.py
+-rw-r--r--   0        0        0     2452 2023-03-15 14:45:53.879689 icd_mappings-0.1.2/icdmappings/mappers/icd9_to_cci.py
+-rw-r--r--   0        0        0     4780 2023-03-15 14:45:53.880197 icd_mappings-0.1.2/icdmappings/mappers/icd9_to_ccs.py
+-rw-r--r--   0        0        0     3333 2023-03-15 14:45:53.881086 icd_mappings-0.1.2/icdmappings/mappers/icd9_to_chapters.py
+-rw-r--r--   0        0        0     1956 2023-03-15 14:45:53.881708 icd_mappings-0.1.2/icdmappings/mappers/icd9_to_icd10.py
+-rw-r--r--   0        0        0      729 2023-03-15 14:45:53.882241 icd_mappings-0.1.2/icdmappings/mappers/icd9_to_level3.py
+-rw-r--r--   0        0        0     1096 2023-03-15 14:45:47.834508 icd_mappings-0.1.2/icdmappings/mappers/lol.ipynb
+-rw-r--r--   0        0        0      472 2023-03-15 14:45:53.882877 icd_mappings-0.1.2/icdmappings/mappers/mapper_interface.py
+-rw-r--r--   0        0        0      100 2023-03-14 10:04:00.087660 icd_mappings-0.1.2/icdmappings/validators/__init__.py
+-rw-r--r--   0        0        0     3233 2023-03-15 14:45:53.883649 icd_mappings-0.1.2/icdmappings/validators/icd9_validator.py
+-rw-r--r--   0        0        0      686 2023-03-15 14:45:53.884114 icd_mappings-0.1.2/icdmappings/validators/icd_validator_interface.py
+-rw-r--r--   0        0        0      600 2023-04-26 11:41:06.374754 icd_mappings-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 icd_mappings-0.1.2/PKG-INFO
```

### Comparing `icd_mappings-0.1.1/README.md` & `icd_mappings-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 - [ICD9->ICD9Chapters](https://icd.codes/icd9cm): ICD9-CM diagnostic codes to the 19 Chapters;
 - [ICD9->CCI](https://www.hcup-us.ahrq.gov/toolssoftware/chronic/chronic.jsp) ICD9-CM diagnostics to CCI (Chronic Condition Indicator). True of False depending on whether a diagnostic is chronic or not;
 - ICD9->Level3: Gets the 3rd level of an ICD9-CM diagnostic code;
 
 
 Supports mapping either a `single code` at a time, or an `iterable of codes` (range, list, np.array, pd.Series, etc...).
 
-----
 
-> :warning: **Warning:** When ICD9 or ICD10 is mentioned, it refers to the American version aka ICD9-CM / ICD10-CM.
+> :warning: When ICD9 or ICD10 is mentioned, it always refers to the American version aka ICD9-CM / ICD10-CM.
+
+# Installation
+
+`pip install icd-mappings`
 
 # Usage
 
 ```python
 from icdmappings import Mapper
 
 mapper = Mapper()
```

### Comparing `icd_mappings-0.1.1/icdmappings/icdmappings.py` & `icd_mappings-0.1.2/icdmappings/icdmappings.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,21 +33,21 @@
 
     def show_mappers(self):
         return list(self._internal_mapping.keys())
     
     def show_validators(self):
         return list(self._internal_validators.keys())
     
-    def validate_diagnostics(self, category : str, codes : str | Iterable):
+    def validate_diagnostics(self, codes : str | Iterable, category : str):
 
         validator = self._get_validator(category)
         
         return validator.validate_diagnostics(codes)
     
-    def validate_procedures(self, category : str, codes : str | Iterable):
+    def validate_procedures(self, codes : str | Iterable, category : str):
 
         validator = self._get_validator(category)
         
         return validator.validate_procedures(codes)
 
     def _get_validator(self, category : str):
         validator = self._internal_validators.get(category)
```

### Comparing `icd_mappings-0.1.1/icdmappings/mappers/icd10_to_icd9.py` & `icd_mappings-0.1.2/icdmappings/mappers/icd10_to_icd9.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.1/icdmappings/mappers/icd9_to_cci.py` & `icd_mappings-0.1.2/icdmappings/mappers/icd9_to_cci.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.1/icdmappings/mappers/icd9_to_ccs.py` & `icd_mappings-0.1.2/icdmappings/mappers/icd9_to_ccs.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.1/icdmappings/mappers/icd9_to_chapters.py` & `icd_mappings-0.1.2/icdmappings/mappers/icd9_to_chapters.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.1/icdmappings/mappers/icd9_to_icd10.py` & `icd_mappings-0.1.2/icdmappings/mappers/icd9_to_icd10.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.1/icdmappings/mappers/icd9_to_level3.py` & `icd_mappings-0.1.2/icdmappings/mappers/icd9_to_level3.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.1/icdmappings/mappers/lol.ipynb` & `icd_mappings-0.1.2/icdmappings/mappers/lol.ipynb`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.1/icdmappings/validators/icd9_validator.py` & `icd_mappings-0.1.2/icdmappings/validators/icd9_validator.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.1/icdmappings/validators/icd_validator_interface.py` & `icd_mappings-0.1.2/icdmappings/validators/icd_validator_interface.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.1/pyproject.toml` & `icd_mappings-0.1.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "icd-mappings"
-version = "0.1.1"
+version = "0.1.2"
 description = "This python tools allows you to map icd codes between versions (9 and 10) and also to other coding schemas such as CCS (Clinical Classification Software))"
 authors = ["Simao Novais <snovaisg.97@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/snovaisg/ICDMappings"
 packages = [{include = "icdmappings"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `icd_mappings-0.1.1/PKG-INFO` & `icd_mappings-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: icd-mappings
-Version: 0.1.1
+Version: 0.1.2
 Summary: This python tools allows you to map icd codes between versions (9 and 10) and also to other coding schemas such as CCS (Clinical Classification Software))
 Home-page: https://github.com/snovaisg/ICDMappings
 License: MIT
 Author: Simao Novais
 Author-email: snovaisg.97@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/snovaisg/ICDMappings
 Description-Content-Type: text/markdown
 
 # ICDMappings
 
@@ -24,17 +26,20 @@
 - [ICD9->ICD9Chapters](https://icd.codes/icd9cm): ICD9-CM diagnostic codes to the 19 Chapters;
 - [ICD9->CCI](https://www.hcup-us.ahrq.gov/toolssoftware/chronic/chronic.jsp) ICD9-CM diagnostics to CCI (Chronic Condition Indicator). True of False depending on whether a diagnostic is chronic or not;
 - ICD9->Level3: Gets the 3rd level of an ICD9-CM diagnostic code;
 
 
 Supports mapping either a `single code` at a time, or an `iterable of codes` (range, list, np.array, pd.Series, etc...).
 
-----
 
-> :warning: **Warning:** When ICD9 or ICD10 is mentioned, it refers to the American version aka ICD9-CM / ICD10-CM.
+> :warning: When ICD9 or ICD10 is mentioned, it always refers to the American version aka ICD9-CM / ICD10-CM.
+
+# Installation
+
+`pip install icd-mappings`
 
 # Usage
 
 ```python
 from icdmappings import Mapper
 
 mapper = Mapper()
```

