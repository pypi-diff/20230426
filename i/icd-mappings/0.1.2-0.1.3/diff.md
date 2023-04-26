# Comparing `tmp/icd_mappings-0.1.2.tar.gz` & `tmp/icd_mappings-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icd_mappings-0.1.2.tar", max compression
+gzip compressed data, was "icd_mappings-0.1.3.tar", max compression
```

## Comparing `icd_mappings-0.1.2.tar` & `icd_mappings-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1992 2023-04-26 11:33:59.681730 icd_mappings-0.1.2/README.md
--rw-r--r--   0        0        0       31 2023-03-15 14:37:28.554849 icd_mappings-0.1.2/icdmappings/__init__.py
--rw-r--r--   0        0        0     2092 2023-04-26 11:39:27.537862 icd_mappings-0.1.2/icdmappings/icdmappings.py
--rw-r--r--   0        0        0      382 2023-03-15 14:37:12.884893 icd_mappings-0.1.2/icdmappings/mappers/__init__.py
--rw-r--r--   0        0        0     1885 2023-03-15 14:45:53.879281 icd_mappings-0.1.2/icdmappings/mappers/icd10_to_icd9.py
--rw-r--r--   0        0        0     2452 2023-03-15 14:45:53.879689 icd_mappings-0.1.2/icdmappings/mappers/icd9_to_cci.py
--rw-r--r--   0        0        0     4780 2023-03-15 14:45:53.880197 icd_mappings-0.1.2/icdmappings/mappers/icd9_to_ccs.py
--rw-r--r--   0        0        0     3333 2023-03-15 14:45:53.881086 icd_mappings-0.1.2/icdmappings/mappers/icd9_to_chapters.py
--rw-r--r--   0        0        0     1956 2023-03-15 14:45:53.881708 icd_mappings-0.1.2/icdmappings/mappers/icd9_to_icd10.py
--rw-r--r--   0        0        0      729 2023-03-15 14:45:53.882241 icd_mappings-0.1.2/icdmappings/mappers/icd9_to_level3.py
--rw-r--r--   0        0        0     1096 2023-03-15 14:45:47.834508 icd_mappings-0.1.2/icdmappings/mappers/lol.ipynb
--rw-r--r--   0        0        0      472 2023-03-15 14:45:53.882877 icd_mappings-0.1.2/icdmappings/mappers/mapper_interface.py
--rw-r--r--   0        0        0      100 2023-03-14 10:04:00.087660 icd_mappings-0.1.2/icdmappings/validators/__init__.py
--rw-r--r--   0        0        0     3233 2023-03-15 14:45:53.883649 icd_mappings-0.1.2/icdmappings/validators/icd9_validator.py
--rw-r--r--   0        0        0      686 2023-03-15 14:45:53.884114 icd_mappings-0.1.2/icdmappings/validators/icd_validator_interface.py
--rw-r--r--   0        0        0      600 2023-04-26 11:41:06.374754 icd_mappings-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 icd_mappings-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1992 2023-04-26 11:33:59.681730 icd_mappings-0.1.3/README.md
+-rw-r--r--   0        0        0       31 2023-03-15 14:37:28.554849 icd_mappings-0.1.3/icdmappings/__init__.py
+-rw-r--r--   0        0        0     2132 2023-04-26 14:04:37.870674 icd_mappings-0.1.3/icdmappings/icdmappings.py
+-rw-r--r--   0        0        0      382 2023-03-15 14:37:12.884893 icd_mappings-0.1.3/icdmappings/mappers/__init__.py
+-rw-r--r--   0        0        0     1916 2023-04-26 14:01:46.741546 icd_mappings-0.1.3/icdmappings/mappers/icd10_to_icd9.py
+-rw-r--r--   0        0        0     2465 2023-04-26 14:02:22.394668 icd_mappings-0.1.3/icdmappings/mappers/icd9_to_cci.py
+-rw-r--r--   0        0        0     4793 2023-04-26 14:02:40.764706 icd_mappings-0.1.3/icdmappings/mappers/icd9_to_ccs.py
+-rw-r--r--   0        0        0     3351 2023-04-26 14:00:55.494895 icd_mappings-0.1.3/icdmappings/mappers/icd9_to_chapters.py
+-rw-r--r--   0        0        0     1987 2023-04-26 14:01:15.042461 icd_mappings-0.1.3/icdmappings/mappers/icd9_to_icd10.py
+-rw-r--r--   0        0        0      760 2023-04-26 14:01:27.386173 icd_mappings-0.1.3/icdmappings/mappers/icd9_to_level3.py
+-rw-r--r--   0        0        0     1096 2023-03-15 14:45:47.834508 icd_mappings-0.1.3/icdmappings/mappers/lol.ipynb
+-rw-r--r--   0        0        0      491 2023-04-26 14:00:22.255137 icd_mappings-0.1.3/icdmappings/mappers/mapper_interface.py
+-rw-r--r--   0        0        0      100 2023-03-14 10:04:00.087660 icd_mappings-0.1.3/icdmappings/validators/__init__.py
+-rw-r--r--   0        0        0     3264 2023-04-26 14:04:23.901528 icd_mappings-0.1.3/icdmappings/validators/icd9_validator.py
+-rw-r--r--   0        0        0      729 2023-04-26 14:00:03.363869 icd_mappings-0.1.3/icdmappings/validators/icd_validator_interface.py
+-rw-r--r--   0        0        0      600 2023-04-26 14:06:09.691212 icd_mappings-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 icd_mappings-0.1.3/PKG-INFO
```

### Comparing `icd_mappings-0.1.2/README.md` & `icd_mappings-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.2/icdmappings/icdmappings.py` & `icd_mappings-0.1.3/icdmappings/icdmappings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .mappers import * 
 from .validators import ICD9Validator
 from collections.abc import Iterable
+from typing import Union
 class Mapper():
 
     def __init__(self):
 
         # mappers
         self.icd9_to_cci = ICD9toCCI()
         self.icd9_to_level3 = ICD9toLEVEL3()
@@ -33,35 +34,35 @@
 
     def show_mappers(self):
         return list(self._internal_mapping.keys())
     
     def show_validators(self):
         return list(self._internal_validators.keys())
     
-    def validate_diagnostics(self, codes : str | Iterable, category : str):
+    def validate_diagnostics(self, codes : Union[str,Iterable], category : str):
 
         validator = self._get_validator(category)
         
         return validator.validate_diagnostics(codes)
     
-    def validate_procedures(self, codes : str | Iterable, category : str):
+    def validate_procedures(self, codes : Union[str,Iterable], category : str):
 
         validator = self._get_validator(category)
         
         return validator.validate_procedures(codes)
 
     def _get_validator(self, category : str):
         validator = self._internal_validators.get(category)
 
         if validator is None:
             raise ValueError(f"Category must be one of the following {str(self._internal_validators.keys())}")
         return validator
 
     def map(self, 
-            codes : str | Iterable,
+            codes : Union[str,Iterable],
             mapper : str):
         
         mapper = self._internal_mapping.get(mapper)
 
         if mapper is None:
             raise ValueError(f"Mapper {mapper} not found. Please choose one from: {str(self.show_mappers())}.")
```

### Comparing `icd_mappings-0.1.2/icdmappings/mappers/icd10_to_icd9.py` & `icd_mappings-0.1.3/icdmappings/mappers/icd10_to_icd9.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from collections.abc import Iterable
 from .mapper_interface import MapperInterface
 import csv
+from typing import Union
 
 class ICD10toICD9(MapperInterface):
     """
     Maps icd10 codes to icd9.
     
     Source of mapping: https://www.nber.org/research/data/icd-9-cm-and-icd-10-cm-and-icd-10-pcs-crosswalk-or-general-equivalence-mappings
     """
@@ -28,15 +29,15 @@
             
         try:
             return self.icd10_to_icd9[icd10code]
         except:
             return None
 
     def map(self,
-            icd10code : str | Iterable
+            icd10code : Union[str, Iterable]
             ):
         """
         Given an icd10 code, returns the corresponding icd9 code.
 
         Parameters
         ----------
```

### Comparing `icd_mappings-0.1.2/icdmappings/mappers/icd9_to_cci.py` & `icd_mappings-0.1.3/icdmappings/mappers/icd9_to_cci.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Union
 import os
 from collections.abc import Iterable
 import csv
 
 class ICD9toCCI:
         """
         Maps icd9 diagnostic codes to chronic or not chronic (that is the question).
@@ -25,15 +25,15 @@
             )
 
             # creates self.chapters_num, self.chapters_char, self.bins
             self.icd9_to_cci = self._parse_file(filepath)
 
 
         def map(self,
-                icd9code : str | Iterable
+                icd9code : Union[str, Iterable]
                 ):
                 """
                 Given an icd9 code, returns the corresponding Chronic value (True for chronic, and False for not-chronic)
 
                 Parameters
                 ----------
```

### Comparing `icd_mappings-0.1.2/icdmappings/mappers/icd9_to_ccs.py` & `icd_mappings-0.1.3/icdmappings/mappers/icd9_to_ccs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Union
 import os
 from collections.abc import Iterable
 import re
 
 from .mapper_interface import MapperInterface
 
 class ICD9toCCS(MapperInterface):
@@ -39,15 +39,15 @@
         def _map_single(self, icd9code : str):
             try:
                 return self.icd9_to_ccs[icd9code]
             except:
                 return None
 
         def map(self,
-                icd9code: str | Iterable
+                icd9code: Union[str, Iterable]
                 ):
             """
             Given an icd9 code, returns the corresponding ccs code.
             If input is Iterable returns a list of codes. If np.array or pd.Series, returns in the same format.
             
             Parameters
             ----------
```

### Comparing `icd_mappings-0.1.2/icdmappings/mappers/icd9_to_chapters.py` & `icd_mappings-0.1.3/icdmappings/mappers/icd9_to_chapters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List,Union
 import os
 from collections.abc import Iterable
 from .mapper_interface import MapperInterface
 import bisect
 import csv
 
 class ICD9toChapters(MapperInterface):
@@ -41,15 +41,15 @@
                     if bin is not None:
                         return str(bin)
                     return None
                 except:
                     return None
 
 
-        def map(self, icd9code : str | Iterable):
+        def map(self, icd9code : Union[str, Iterable]):
             """
             Parameters
             ----------
             code : str | Iterable
 
             Returns
             -------
@@ -59,15 +59,15 @@
             if isinstance(icd9code,str):
                 return self._map_single(icd9code)
             elif isinstance(icd9code, Iterable):
                 return [self._map_single(code) for code in icd9code]
             raise TypeError(f'Wrong input type. Expecting str or Iterable. Got {type(icd9code)}')
                     
 
-        def _get_bin(self, number : int | Iterable, bins : List):
+        def _get_bin(self, number : Union[int, Iterable], bins : List):
             if isinstance(number,int):
                 return bisect.bisect(bins, number)
             elif isinstance(number,Iterable):
                 return [bisect.bisect(bins, num) if isinstance(num,int) else None for num in number]
             return None
```

### Comparing `icd_mappings-0.1.2/icdmappings/mappers/icd9_to_icd10.py` & `icd_mappings-0.1.3/icdmappings/mappers/icd9_to_icd10.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from collections.abc import Iterable
 from .mapper_interface import MapperInterface
 import csv
+from typing import Union
 
 
 class ICD9toICD10(MapperInterface):
     """
     Maps icd9 codes into icd10.
     
     
@@ -22,15 +23,15 @@
             os.path.dirname(os.path.abspath(__file__)))),
                 self.path2file
         )
 
         # creates self.chapters_num, self.chapters_char, self.bins
         self.icd9_to_icd10 = self._parse_file(filepath)
 
-    def map(self,icd9code : str | Iterable):
+    def map(self,icd9code : Union[str, Iterable]):
             """
             Given an icd9 code, returns the corresponding icd10 code.
 
             Parameters
             ----------
 
             code : str | pd.Series
```

### Comparing `icd_mappings-0.1.2/icdmappings/mappers/icd9_to_level3.py` & `icd_mappings-0.1.3/icdmappings/mappers/icd9_to_level3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .mapper_interface import MapperInterface
 from collections.abc import Iterable
+from typing import Union
 
 class ICD9toLEVEL3(MapperInterface):
     """
     maps diagnostic icd9 codes to the first 3 levels
     """
     
     def __init__(self):
@@ -12,14 +13,14 @@
 
     def _map_single(self,icd9code : str):
 
         if isinstance(icd9code,str):
             return icd9code[:3]
         return None
 
-    def map(self, icd9code : str | Iterable):
+    def map(self, icd9code : Union[str, Iterable]):
         
         if isinstance(icd9code,str):
             return self._map_single(icd9code)
         elif isinstance(icd9code,Iterable):
             return [ self._map_single(code) for code in icd9code ]
         TypeError(f'Wrong input type. Expecting str or Iterable. Got {type(icd9code)}')
```

### Comparing `icd_mappings-0.1.2/icdmappings/mappers/lol.ipynb` & `icd_mappings-0.1.3/icdmappings/mappers/lol.ipynb`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.1.2/icdmappings/validators/icd9_validator.py` & `icd_mappings-0.1.3/icdmappings/validators/icd9_validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .icd_validator_interface import ICDValidatorInterface
-from typing import List
+from typing import List, Union
 import os
 from collections.abc import Iterable
 
+
 class ICD9Validator(ICDValidatorInterface):
         """
         Checks if a code is icd9-cm version 32 compliant.
         """
         
         def __init__(self):
             self.path2folder = "data_sources/ICD-9-CM-v32-master-descriptions"
@@ -20,16 +21,16 @@
                  ), self.path2folder)
              self.diagnostics = self._parse_diagnostics()
              self.procedures = self._parse_procedures()
              pass
         
 
         def validate_diagnostics(self, 
-                                codes : str | Iterable,
-                                ) -> bool | Iterable:
+                                codes : Union[str,Iterable],
+                                ) -> Union[bool, Iterable]:
             """validates if a code or iterable of codes are valid diagnostics.
             If iterable is numpy or pd.Series, returns the same type. ALl other iterables are returned as List.
 
             Args:
                 codes (str | List | pd.Series | np.ndarray): _description_
 
             Raises:
@@ -44,16 +45,16 @@
                 return codes in self.diagnostics.keys()
             elif isinstance(codes,Iterable):
                 valid = [code in self.diagnostics.keys() if code is not None else None for code in codes]
                 return valid
             raise TypeError('Expects a string or iterable of strings as codes.')
         
         def validate_procedures(self,
-                               codes : str | Iterable,
-                              ) -> bool | Iterable:
+                               codes : Union[str, Iterable],
+                              ) -> Union[bool, Iterable]:
             
             if codes is None:
                 return None
             if isinstance(codes,str):
                 return codes in self.procedures.keys()
             elif isinstance(codes,Iterable):
                 valid = [code in self.procedures.keys() if code is not None else None for code in codes]
```

### Comparing `icd_mappings-0.1.2/icdmappings/validators/icd_validator_interface.py` & `icd_mappings-0.1.3/icdmappings/validators/icd_validator_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from abc import ABC, abstractclassmethod
 from collections.abc import Iterable
+from typing import Union
 
 class ICDValidatorInterface(ABC):
     """
     Abstract class for mapping classes.
     """
 
     def __init__(self):
         pass
     
     @abstractclassmethod
     def validate_diagnostics(self, 
-            codes : str | Iterable,
+            codes : Union[str, Iterable],
             ) -> bool | Iterable:
         """
         Returns True of False if the code is a valid diagnostic code.
         """
         pass
 
     @abstractclassmethod
     def validate_procedures(self, 
-            codes : str | Iterable,
-            ) -> bool | Iterable:
+            codes : Union[str, Iterable],
+            ) -> Union[bool, Iterable]:
         """
         Returns True of False if the code is a valid procedure code.
         """
         pass
```

### Comparing `icd_mappings-0.1.2/pyproject.toml` & `icd_mappings-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "icd-mappings"
-version = "0.1.2"
+version = "0.1.3"
 description = "This python tools allows you to map icd codes between versions (9 and 10) and also to other coding schemas such as CCS (Clinical Classification Software))"
 authors = ["Simao Novais <snovaisg.97@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/snovaisg/ICDMappings"
 packages = [{include = "icdmappings"}]
```

### Comparing `icd_mappings-0.1.2/PKG-INFO` & `icd_mappings-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icd-mappings
-Version: 0.1.2
+Version: 0.1.3
 Summary: This python tools allows you to map icd codes between versions (9 and 10) and also to other coding schemas such as CCS (Clinical Classification Software))
 Home-page: https://github.com/snovaisg/ICDMappings
 License: MIT
 Author: Simao Novais
 Author-email: snovaisg.97@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

