# Comparing `tmp/pyspellchecker-0.7.1.tar.gz` & `tmp/pyspellchecker-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspellchecker-0.7.1.tar", last modified: Thu Dec 15 03:39:25 2022, max compression
+gzip compressed data, was "pyspellchecker-0.7.2.tar", last modified: Wed Apr 26 01:48:57 2023, max compression
```

## Comparing `pyspellchecker-0.7.1.tar` & `pyspellchecker-0.7.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 03:39:25.560541 pyspellchecker-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2022-12-15 03:39:25.560541 pyspellchecker-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 03:39:25.556542 pyspellchecker-0.7.1/pyspellchecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2022-12-15 03:39:25.000000 pyspellchecker-0.7.1/pyspellchecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-15 03:39:25.000000 pyspellchecker-0.7.1/pyspellchecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 03:39:25.000000 pyspellchecker-0.7.1/pyspellchecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-15 03:39:25.000000 pyspellchecker-0.7.1/pyspellchecker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 03:39:25.560541 pyspellchecker-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 03:39:25.556542 pyspellchecker-0.7.1/spellchecker/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/spellchecker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/spellchecker/info.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/spellchecker/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 03:39:25.560541 pyspellchecker-0.7.1/spellchecker/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   782672 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/spellchecker/resources/ar.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)   104116 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/spellchecker/resources/de.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)   363978 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/spellchecker/resources/en.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)   563595 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/spellchecker/resources/es.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)   259206 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/spellchecker/resources/fr.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)   262502 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/spellchecker/resources/pt.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)   107969 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/spellchecker/resources/ru.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)    19861 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/spellchecker/spellchecker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2022-12-15 03:39:11.000000 pyspellchecker-0.7.1/spellchecker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:48:57.879889 pyspellchecker-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-26 01:48:57.879889 pyspellchecker-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:48:57.875889 pyspellchecker-0.7.2/pyspellchecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-26 01:48:57.000000 pyspellchecker-0.7.2/pyspellchecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-26 01:48:57.000000 pyspellchecker-0.7.2/pyspellchecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 01:48:57.000000 pyspellchecker-0.7.2/pyspellchecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 01:48:57.000000 pyspellchecker-0.7.2/pyspellchecker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 01:48:57.879889 pyspellchecker-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:48:57.875889 pyspellchecker-0.7.2/spellchecker/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:48:57.879889 pyspellchecker-0.7.2/spellchecker/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   782672 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/resources/ar.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   104116 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/resources/de.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   363978 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/resources/en.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   563595 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/resources/es.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   349118 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/resources/eu.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   259206 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/resources/fr.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   615891 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/resources/lv.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   262502 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/resources/pt.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   107969 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/resources/ru.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/spellchecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-26 01:48:41.000000 pyspellchecker-0.7.2/spellchecker/utils.py
```

### Comparing `pyspellchecker-0.7.1/LICENSE` & `pyspellchecker-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspellchecker-0.7.1/PKG-INFO` & `pyspellchecker-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyspellchecker
-Version: 0.7.1
+Version: 0.7.2
 Summary: Pure python spell checker based on work by Peter Norvig
 Author-email: Tyler Barrus <barrust@gmail.com>
 License: MIT
-Project-URL: homepage, https://github.com/barrust/pyprobables
-Project-URL: bug-tracker, https://github.com/barrust/pyprobables/issues
-Project-URL: documentation, https://pyprobables.readthedocs.io/
+Project-URL: homepage, https://github.com/barrust/pyspellchecker
+Project-URL: bug-tracker, https://github.com/barrust/pyspellchecker/issues
+Project-URL: documentation, https://pyspellchecker.readthedocs.io/
 Keywords: python,spelling,natural language processing,nlp,typo,checker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
@@ -59,15 +59,15 @@
 algorithm to find permutations within an edit distance of 2 from the
 original word. It then compares all permutations (insertions, deletions,
 replacements, and transpositions) to known words in a word frequency
 list. Those words that are found more often in the frequency list are
 **more likely** the correct results.
 
 ``pyspellchecker`` supports multiple languages including English, Spanish,
-German, French, and Portuguese. For information on how the dictionaries were
+German, French, Portuguese, Arabic and Basque. For information on how the dictionaries were
 created and how they can be updated and improved, please see the
 **Dictionary Creation and Updating** section of the readme!
 
 ``pyspellchecker`` supports **Python 3**
 
 ``pyspellchecker`` allows for the setting of the Levenshtein Distance (up to two) to check.
 For longer words, it is highly recommended to use a distance of 1 and not the
@@ -173,14 +173,16 @@
 * English       - 'en'
 * Spanish       - 'es'
 * French        - 'fr'
 * Portuguese    - 'pt'
 * German        - 'de'
 * Russian       - 'ru'
 * Arabic        - 'ar'
+* Basque        - 'eu'
+* Latvian       - 'lv'
 
 Dictionary Creation and Updating
 -------------------------------------------------------------------------------
 
 The creation of the dictionaries is, unfortunately, not an exact science. I have provided a script that, given a text file of sentences (in this case from
 `OpenSubtitles <http://opus.nlpl.eu/OpenSubtitles2018.php>`__) it will generate a word frequency list based on the words found within the text. The script then attempts to ***clean up*** the word frequency by, for example, removing words with invalid characters (usually from other languages), removing low count terms (misspellings?) and attempts to enforce rules as available (no more than one accent per word in Spanish). Then it removes words from a list of known words that are to be removed. It then adds words into the dictionary that are known to be missing or were removed for being too low frequency.
```

### Comparing `pyspellchecker-0.7.1/README.rst` & `pyspellchecker-0.7.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 algorithm to find permutations within an edit distance of 2 from the
 original word. It then compares all permutations (insertions, deletions,
 replacements, and transpositions) to known words in a word frequency
 list. Those words that are found more often in the frequency list are
 **more likely** the correct results.
 
 ``pyspellchecker`` supports multiple languages including English, Spanish,
-German, French, and Portuguese. For information on how the dictionaries were
+German, French, Portuguese, Arabic and Basque. For information on how the dictionaries were
 created and how they can be updated and improved, please see the
 **Dictionary Creation and Updating** section of the readme!
 
 ``pyspellchecker`` supports **Python 3**
 
 ``pyspellchecker`` allows for the setting of the Levenshtein Distance (up to two) to check.
 For longer words, it is highly recommended to use a distance of 1 and not the
@@ -143,14 +143,16 @@
 * English       - 'en'
 * Spanish       - 'es'
 * French        - 'fr'
 * Portuguese    - 'pt'
 * German        - 'de'
 * Russian       - 'ru'
 * Arabic        - 'ar'
+* Basque        - 'eu'
+* Latvian       - 'lv'
 
 Dictionary Creation and Updating
 -------------------------------------------------------------------------------
 
 The creation of the dictionaries is, unfortunately, not an exact science. I have provided a script that, given a text file of sentences (in this case from
 `OpenSubtitles <http://opus.nlpl.eu/OpenSubtitles2018.php>`__) it will generate a word frequency list based on the words found within the text. The script then attempts to ***clean up*** the word frequency by, for example, removing words with invalid characters (usually from other languages), removing low count terms (misspellings?) and attempts to enforce rules as available (no more than one accent per word in Spanish). Then it removes words from a list of known words that are to be removed. It then adds words into the dictionary that are known to be missing or were removed for being too low frequency.
```

### Comparing `pyspellchecker-0.7.1/pyproject.toml` & `pyspellchecker-0.7.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -35,17 +35,17 @@
 
 
 [tool.setuptools.dynamic]
 version = {attr = "spellchecker.__version__"}
 
 
 [project.urls]
-homepage = "https://github.com/barrust/pyprobables"
-bug-tracker = "https://github.com/barrust/pyprobables/issues"
-documentation = "https://pyprobables.readthedocs.io/"
+homepage = "https://github.com/barrust/pyspellchecker"
+bug-tracker = "https://github.com/barrust/pyspellchecker/issues"
+documentation = "https://pyspellchecker.readthedocs.io/"
 
 
 [tool.poetry]
 packages = [
         {include = "spellchecker"},
 ]
```

### Comparing `pyspellchecker-0.7.1/pyspellchecker.egg-info/PKG-INFO` & `pyspellchecker-0.7.2/pyspellchecker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyspellchecker
-Version: 0.7.1
+Version: 0.7.2
 Summary: Pure python spell checker based on work by Peter Norvig
 Author-email: Tyler Barrus <barrust@gmail.com>
 License: MIT
-Project-URL: homepage, https://github.com/barrust/pyprobables
-Project-URL: bug-tracker, https://github.com/barrust/pyprobables/issues
-Project-URL: documentation, https://pyprobables.readthedocs.io/
+Project-URL: homepage, https://github.com/barrust/pyspellchecker
+Project-URL: bug-tracker, https://github.com/barrust/pyspellchecker/issues
+Project-URL: documentation, https://pyspellchecker.readthedocs.io/
 Keywords: python,spelling,natural language processing,nlp,typo,checker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
@@ -59,15 +59,15 @@
 algorithm to find permutations within an edit distance of 2 from the
 original word. It then compares all permutations (insertions, deletions,
 replacements, and transpositions) to known words in a word frequency
 list. Those words that are found more often in the frequency list are
 **more likely** the correct results.
 
 ``pyspellchecker`` supports multiple languages including English, Spanish,
-German, French, and Portuguese. For information on how the dictionaries were
+German, French, Portuguese, Arabic and Basque. For information on how the dictionaries were
 created and how they can be updated and improved, please see the
 **Dictionary Creation and Updating** section of the readme!
 
 ``pyspellchecker`` supports **Python 3**
 
 ``pyspellchecker`` allows for the setting of the Levenshtein Distance (up to two) to check.
 For longer words, it is highly recommended to use a distance of 1 and not the
@@ -173,14 +173,16 @@
 * English       - 'en'
 * Spanish       - 'es'
 * French        - 'fr'
 * Portuguese    - 'pt'
 * German        - 'de'
 * Russian       - 'ru'
 * Arabic        - 'ar'
+* Basque        - 'eu'
+* Latvian       - 'lv'
 
 Dictionary Creation and Updating
 -------------------------------------------------------------------------------
 
 The creation of the dictionaries is, unfortunately, not an exact science. I have provided a script that, given a text file of sentences (in this case from
 `OpenSubtitles <http://opus.nlpl.eu/OpenSubtitles2018.php>`__) it will generate a word frequency list based on the words found within the text. The script then attempts to ***clean up*** the word frequency by, for example, removing words with invalid characters (usually from other languages), removing low count terms (misspellings?) and attempts to enforce rules as available (no more than one accent per word in Spanish). Then it removes words from a list of known words that are to be removed. It then adds words into the dictionary that are known to be missing or were removed for being too low frequency.
```

### Comparing `pyspellchecker-0.7.1/pyspellchecker.egg-info/SOURCES.txt` & `pyspellchecker-0.7.2/pyspellchecker.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,10 +11,12 @@
 spellchecker/py.typed
 spellchecker/spellchecker.py
 spellchecker/utils.py
 spellchecker/resources/ar.json.gz
 spellchecker/resources/de.json.gz
 spellchecker/resources/en.json.gz
 spellchecker/resources/es.json.gz
+spellchecker/resources/eu.json.gz
 spellchecker/resources/fr.json.gz
+spellchecker/resources/lv.json.gz
 spellchecker/resources/pt.json.gz
 spellchecker/resources/ru.json.gz
```

### Comparing `pyspellchecker-0.7.1/spellchecker/resources/ar.json.gz` & `pyspellchecker-0.7.2/spellchecker/resources/ar.json.gz`

 * *Files identical despite different names*

### Comparing `pyspellchecker-0.7.1/spellchecker/resources/de.json.gz` & `pyspellchecker-0.7.2/spellchecker/resources/de.json.gz`

 * *Files identical despite different names*

### Comparing `pyspellchecker-0.7.1/spellchecker/resources/en.json.gz` & `pyspellchecker-0.7.2/spellchecker/resources/en.json.gz`

 * *Files identical despite different names*

### Comparing `pyspellchecker-0.7.1/spellchecker/resources/es.json.gz` & `pyspellchecker-0.7.2/spellchecker/resources/es.json.gz`

 * *Files identical despite different names*

### Comparing `pyspellchecker-0.7.1/spellchecker/resources/fr.json.gz` & `pyspellchecker-0.7.2/spellchecker/resources/fr.json.gz`

 * *Files identical despite different names*

### Comparing `pyspellchecker-0.7.1/spellchecker/resources/pt.json.gz` & `pyspellchecker-0.7.2/spellchecker/resources/pt.json.gz`

 * *Files identical despite different names*

### Comparing `pyspellchecker-0.7.1/spellchecker/resources/ru.json.gz` & `pyspellchecker-0.7.2/spellchecker/resources/ru.json.gz`

 * *Files identical despite different names*

### Comparing `pyspellchecker-0.7.1/spellchecker/spellchecker.py` & `pyspellchecker-0.7.2/spellchecker/spellchecker.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class SpellChecker:
     """The SpellChecker class encapsulates the basics needed to accomplish a
     simple spell checking algorithm. It is based on the work by
     Peter Norvig (https://norvig.com/spell-correct.html)
 
     Args:
         language (str): The language of the dictionary to load or None for no dictionary. Supported languages are \
-            `en`, `es`, `de`, `fr`, `pt` and `ru`. Defaults to `en`. A list of languages may be provided and all \
+            `en`, `es`, `de`, `fr`, `pt`, `ru`, `lv`, and `eu`. Defaults to `en`. A list of languages may be provided and all \
                 languages will be loaded.
         local_dictionary (str): The path to a locally stored word frequency dictionary; if provided, no language \
             will be loaded
         distance (int): The edit distance to use. Defaults to 2.
         case_sensitive (bool): Flag to use a case sensitive dictionary or not, only available when not using a \
             language dictionary.
     Note:
@@ -78,15 +78,15 @@
     def __iter__(self) -> typing.Generator[str, None, None]:
         """setup iter support"""
         yield from self._word_frequency.dictionary
 
     @classmethod
     def languages(cls) -> typing.Iterable[str]:
         """list: A list of all official languages supported by the library"""
-        return ["de", "en", "es", "fr", "pt", "ru", "ar"]
+        return ["de", "en", "es", "fr", "pt", "ru", "ar", "lv", "eu"]
 
     @property
     def word_frequency(self) -> "WordFrequency":
         """WordFrequency: An encapsulation of the word frequency `dictionary`
 
         Note:
             Not settable"""
@@ -252,15 +252,15 @@
         return [e2 for e1 in tmp for e2 in self.known(self.edit_distance_1(e1))]
 
     def _check_if_should_check(self, word: str) -> bool:
         if len(word) == 1 and word in string.punctuation:
             return False
         if len(word) > self._word_frequency.longest_word_length + 3:  # allow removal of up to 2 letters
             return False
-        if word.lower() == 'nan':  # nan passes the float(word) so this will bypass that issue (#125)
+        if word.lower() == "nan":  # nan passes the float(word) so this will bypass that issue (#125)
             return True
         try:  # check if it is a number (int, float, etc)
             float(word)
             return False
         except ValueError:
             pass
```

### Comparing `pyspellchecker-0.7.1/spellchecker/utils.py` & `pyspellchecker-0.7.2/spellchecker/utils.py`

 * *Files identical despite different names*

