# Comparing `tmp/eda_report-2.7.3.tar.gz` & `tmp/eda_report-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eda_report-2.7.3.tar", last modified: Mon Dec  5 18:22:44 2022, max compression
+gzip compressed data, was "eda_report-2.8.0.tar", last modified: Wed Apr 26 08:26:11 2023, max compression
```

## Comparing `eda_report-2.7.3.tar` & `eda_report-2.8.0.tar`

### file list

```diff
@@ -1,30 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 18:22:44.767342 eda_report-2.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2022-12-05 18:22:32.000000 eda_report-2.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-05 18:22:32.000000 eda_report-2.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2022-12-05 18:22:44.767342 eda_report-2.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2022-12-05 18:22:32.000000 eda_report-2.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 18:22:44.763342 eda_report-2.7.3/eda_report/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/content.py
--rw-r--r--   0 runner    (1001) docker     (123)    13138 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 18:22:44.767342 eda_report-2.7.3/eda_report/images/
--rw-r--r--   0 runner    (1001) docker     (123)    12572 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/images/background.png
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14490 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/univariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2022-12-05 18:22:32.000000 eda_report-2.7.3/eda_report/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 18:22:44.763342 eda_report-2.7.3/eda_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2022-12-05 18:22:44.000000 eda_report-2.7.3/eda_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2022-12-05 18:22:44.000000 eda_report-2.7.3/eda_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 18:22:44.000000 eda_report-2.7.3/eda_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-05 18:22:44.000000 eda_report-2.7.3/eda_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2022-12-05 18:22:44.000000 eda_report-2.7.3/eda_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-05 18:22:44.000000 eda_report-2.7.3/eda_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-05 18:22:32.000000 eda_report-2.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2022-12-05 18:22:44.767342 eda_report-2.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:26:11.889951 eda_report-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-26 08:26:00.000000 eda_report-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 08:26:00.000000 eda_report-2.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-26 08:26:11.889951 eda_report-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-04-26 08:26:00.000000 eda_report-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:26:11.885951 eda_report-2.8.0/eda_report/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/_read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/bivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12557 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:26:11.889951 eda_report-2.8.0/eda_report/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/images/background.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16174 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-04-26 08:26:00.000000 eda_report-2.8.0/eda_report/univariate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:26:11.885951 eda_report-2.8.0/eda_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-26 08:26:11.000000 eda_report-2.8.0/eda_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-26 08:26:11.000000 eda_report-2.8.0/eda_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:26:11.000000 eda_report-2.8.0/eda_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 08:26:11.000000 eda_report-2.8.0/eda_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-26 08:26:11.000000 eda_report-2.8.0/eda_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 08:26:11.000000 eda_report-2.8.0/eda_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-26 08:26:00.000000 eda_report-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-26 08:26:11.893951 eda_report-2.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:26:11.889951 eda_report-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-26 08:26:00.000000 eda_report-2.8.0/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-26 08:26:00.000000 eda_report-2.8.0/tests/test_bivariate_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-26 08:26:00.000000 eda_report-2.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-26 08:26:00.000000 eda_report-2.8.0/tests/test_content_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-26 08:26:00.000000 eda_report-2.8.0/tests/test_data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-26 08:26:00.000000 eda_report-2.8.0/tests/test_document_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-26 08:26:00.000000 eda_report-2.8.0/tests/test_file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-26 08:26:00.000000 eda_report-2.8.0/tests/test_main_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-26 08:26:00.000000 eda_report-2.8.0/tests/test_plotting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-26 08:26:00.000000 eda_report-2.8.0/tests/test_univariate_analysis.py
```

### Comparing `eda_report-2.7.3/LICENSE` & `eda_report-2.8.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021-2022 Abwao
+Copyright (c) 2021-2023 Abwao
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `eda_report-2.7.3/PKG-INFO` & `eda_report-2.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eda_report
-Version: 2.7.3
+Version: 2.8.0
 Summary: A simple program to automate exploratory data analysis and reporting.
 Home-page: https://eda-report.readthedocs.io/
 Author: Abwao
 Author-email: abwaomusungu@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Tim-Abwao/eda-report
 Keywords: eda report
@@ -27,61 +27,52 @@
 [![codecov](https://codecov.io/gh/Tim-Abwao/eda-report/branch/main/graph/badge.svg?token=KNQD8XZCWG)](https://codecov.io/gh/Tim-Abwao/eda-report)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A Python program to help automate the exploratory data analysis and reporting process.
 
 Input data is analyzed using [pandas][pandas] and [SciPy][scipy]. Graphs are plotted using [matplotlib][matplotlib]. The results are then nicely packaged as a *Word (.docx)* document using [python-docx][python-docx].
 
+![screencast of report document from iris dataset][report-screencast]
+
 ## Installation
 
 You can install the package from [PyPI][eda-report-pypi] using:
 
 ```bash
 pip install eda-report
 ```
 
 ## Basic Usage
 
 ### 1. Graphical User Interface
 
-The `eda-report` command launches a graphical window to help select and analyze a `csv`/`excel` file:
+The `eda-report` command launches a graphical window to help select a `csv`/`excel` file to analyze:
 
 ```bash
 eda-report
 ```
 
-![screencast of the gui][screencast]
+![screencast of the gui][gui-screencast]
 
-You will be prompted to set a *report title*, *group-by variable (optional)*, *graph color* and *output filename*, after which the contents of the input file will be analyzed, and the results will be saved in a *Word (.docx)* document.
+You'll be prompted to set a *report title*, *group-by/target variable (optional)*, *graph color* and *output filename*; after which the contents of the input file are analyzed, and the results saved in a *Word (.docx)* document.
 
 >**NOTE:** For help with `Tk` - related issues, consider visiting [TkDocs][tkdocs].
 
 ### 2. Command Line Interface
 
-To analyze a file named `input.csv`, just supply its path to the `eda-report` command:
-
 ```bash
-eda-report -i input.csv
-```
-
-Or even:
-
-```bash
-eda-report -i input.csv -o output.docx -c cyan --title 'EDA Report'
-```
-
-For more details on the optional arguments, pass the `-h` or `--help` flag to view the *help message*:
-
-```bash
-eda-report -h
+$ eda-report -i iris.csv -o iris-report.docx
+Analyze variables:  100%|███████████████████████████████████| 5/5
+Plot variables:     100%|███████████████████████████████████| 5/5
+Bivariate analysis: 100%|███████████████████████████████████| 6/6 pairs.
+[INFO 02:12:22.146] Done. Results saved as 'iris-report.docx'
 ```
 
-<details>
-
 ```bash
+$ eda-report -h
 usage: eda-report [-h] [-i INFILE] [-o OUTFILE] [-t TITLE] [-c COLOR]
                   [-g GROUPBY]
 
 Automatically analyze data and generate reports. A graphical user interface
 will be launched if none of the optional arguments is specified.
 
 optional arguments:
@@ -100,72 +91,47 @@
                         The variable to use for grouping plotted values. An
                         integer value is treated as a column index, whereas a
                         string is treated as a column label.
 ```
 
 </details>
 
-### 3. Interactive Mode
-
-#### 3.1 Analyze data
+### 3. Interpreter Session
 
 ```python
 >>> eda_report.summarize(iris_data)
-                        OVERVIEW
-                        ========
-Numeric features: sepal_length, sepal_width, petal_length, petal_width
-Categorical features: species
-
-          Summary Statistics (Numeric features)
-          -------------------------------------
-              count    mean     std  min  25%   50%  75%  max  skewness  kurtosis
-sepal_length  150.0  5.8433  0.8281  4.3  5.1  5.80  6.4  7.9    0.3149   -0.5521
-sepal_width   150.0  3.0573  0.4359  2.0  2.8  3.00  3.3  4.4    0.3190    0.2282
-petal_length  150.0  3.7580  1.7653  1.0  1.6  4.35  5.1  6.9   -0.2749   -1.4021
-petal_width   150.0  1.1993  0.7622  0.1  0.3  1.30  1.8  2.5   -0.1030   -1.3406
-
-          Summary Statistics (Categorical features)
-          -----------------------------------------
-        count unique     top freq relative freq
-species   150      3  setosa   50        33.33%
-
-          Pearson's Correlation (Top 20)
-          ------------------------------
-petal_length & petal_width --> very strong positive correlation (0.96)
-sepal_length & petal_length --> very strong positive correlation (0.87)
-sepal_length & petal_width --> very strong positive correlation (0.82)
-sepal_width & petal_length --> moderate negative correlation (-0.43)
-sepal_width & petal_width --> weak negative correlation (-0.37)
-sepal_length & sepal_width --> very weak negative correlation (-0.12)
-```
-
-#### 3.2 Plot statistical graphs
-
-```python
->>> fig = ep.regression_plot(mpg_data["acceleration"], mpg_data["horsepower"],
-...                          labels=("Acceleration", "Horsepower"))
->>> fig.savefig("regression-plot.png")
-```
 
-<img src="https://raw.githubusercontent.com/Tim-Abwao/eda-report/dev/docs/source/_static/regression-plot.png" width=400px style="display: block; margin: auto;">
-
-#### 3.3 Generate a report
-
-```python
->>> eda_report.get_word_report(iris_data)
-Analyze variables:  100%|███████████████████████████████████| 5/5
-Plot variables:     100%|███████████████████████████████████| 5/5
-Bivariate analysis: 100%|███████████████████████████████████| 6/6 pairs.
-[INFO 16:14:53.648] Done. Results saved as 'eda-report.docx'
-<eda_report.document.ReportDocument object at 0x7f196753bd60>
+                  Summary Statistics for Numeric features (4)
+                  -------------------------------------------
+                count     avg  stddev  min  25%   50%  75%  max  skewness  kurtosis
+  sepal_length    150  5.8433  0.8281  4.3  5.1  5.80  6.4  7.9    0.3149   -0.5521
+  sepal_width     150  3.0573  0.4359  2.0  2.8  3.00  3.3  4.4    0.3190    0.2282
+  petal_length    150  3.7580  1.7653  1.0  1.6  4.35  5.1  6.9   -0.2749   -1.4021
+  petal_width     150  1.1993  0.7622  0.1  0.3  1.30  1.8  2.5   -0.1030   -1.3406
+
+                Summary Statistics for Categorical features (1)
+                -----------------------------------------------
+                    count unique     top freq relative freq
+            species   150      3  setosa   50        33.33%
+
+
+                        Pearson's Correlation (Top 20)
+                        ------------------------------
+      petal_length & petal_width -> very strong positive correlation (0.96)
+     sepal_length & petal_length -> very strong positive correlation (0.87)
+      sepal_length & petal_width -> very strong positive correlation (0.82)
+      sepal_width & petal_length -> moderate negative correlation (-0.43)
+       sepal_width & petal_width -> weak negative correlation (-0.37)
+      sepal_length & sepal_width -> very weak negative correlation (-0.12)
 ```
 
-Visit the [official documentation][docs] for more info.
+Check out the [documentation][docs] for more features and details.
 
 [docs]: https://eda-report.readthedocs.io/
 [eda-report-pypi]: https://pypi.org/project/eda-report/
 [matplotlib]: https://matplotlib.org/
 [pandas]: https://pandas.pydata.org/
 [python-docx]: https://python-docx.readthedocs.io/
 [scipy]: https://scipy.org/
-[screencast]: https://raw.githubusercontent.com/Tim-Abwao/eda-report/dev/docs/source/_static/screencast.gif
+[gui-screencast]: https://raw.githubusercontent.com/Tim-Abwao/eda-report/dev/docs/source/_static/screencast.gif
+[report-screencast]: https://raw.githubusercontent.com/Tim-Abwao/eda-report/dev/docs/source/_static/report.gif
 [tkdocs]: https://tkdocs.com/index.html
```

### Comparing `eda_report-2.7.3/README.md` & `eda_report-2.8.0/eda_report.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,78 @@
+Metadata-Version: 2.1
+Name: eda-report
+Version: 2.8.0
+Summary: A simple program to automate exploratory data analysis and reporting.
+Home-page: https://eda-report.readthedocs.io/
+Author: Abwao
+Author-email: abwaomusungu@gmail.com
+License: MIT
+Project-URL: Source Code, https://github.com/Tim-Abwao/eda-report
+Keywords: eda report
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # `eda-report` - Automated Exploratory Data Analysis
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Tim-Abwao/eda-report/HEAD?filepath=eda-report-basics.ipynb)
 [![PyPI version](https://badge.fury.io/py/eda-report.svg)](https://badge.fury.io/py/eda-report)
 [![Python 3.8 - 3.11](https://github.com/Tim-Abwao/eda-report/actions/workflows/test-python3.8-3.11.yml/badge.svg)](https://github.com/Tim-Abwao/eda-report/actions/workflows/test-python3.8-3.11.yml)
 [![Documentation Status](https://readthedocs.org/projects/eda-report/badge/?version=latest)](https://eda-report.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/Tim-Abwao/eda-report/branch/main/graph/badge.svg?token=KNQD8XZCWG)](https://codecov.io/gh/Tim-Abwao/eda-report)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A Python program to help automate the exploratory data analysis and reporting process.
 
 Input data is analyzed using [pandas][pandas] and [SciPy][scipy]. Graphs are plotted using [matplotlib][matplotlib]. The results are then nicely packaged as a *Word (.docx)* document using [python-docx][python-docx].
 
+![screencast of report document from iris dataset][report-screencast]
+
 ## Installation
 
 You can install the package from [PyPI][eda-report-pypi] using:
 
 ```bash
 pip install eda-report
 ```
 
 ## Basic Usage
 
 ### 1. Graphical User Interface
 
-The `eda-report` command launches a graphical window to help select and analyze a `csv`/`excel` file:
+The `eda-report` command launches a graphical window to help select a `csv`/`excel` file to analyze:
 
 ```bash
 eda-report
 ```
 
-![screencast of the gui][screencast]
+![screencast of the gui][gui-screencast]
 
-You will be prompted to set a *report title*, *group-by variable (optional)*, *graph color* and *output filename*, after which the contents of the input file will be analyzed, and the results will be saved in a *Word (.docx)* document.
+You'll be prompted to set a *report title*, *group-by/target variable (optional)*, *graph color* and *output filename*; after which the contents of the input file are analyzed, and the results saved in a *Word (.docx)* document.
 
 >**NOTE:** For help with `Tk` - related issues, consider visiting [TkDocs][tkdocs].
 
 ### 2. Command Line Interface
 
-To analyze a file named `input.csv`, just supply its path to the `eda-report` command:
-
-```bash
-eda-report -i input.csv
-```
-
-Or even:
-
 ```bash
-eda-report -i input.csv -o output.docx -c cyan --title 'EDA Report'
+$ eda-report -i iris.csv -o iris-report.docx
+Analyze variables:  100%|███████████████████████████████████| 5/5
+Plot variables:     100%|███████████████████████████████████| 5/5
+Bivariate analysis: 100%|███████████████████████████████████| 6/6 pairs.
+[INFO 02:12:22.146] Done. Results saved as 'iris-report.docx'
 ```
 
-For more details on the optional arguments, pass the `-h` or `--help` flag to view the *help message*:
-
-```bash
-eda-report -h
-```
-
-<details>
-
 ```bash
+$ eda-report -h
 usage: eda-report [-h] [-i INFILE] [-o OUTFILE] [-t TITLE] [-c COLOR]
                   [-g GROUPBY]
 
 Automatically analyze data and generate reports. A graphical user interface
 will be launched if none of the optional arguments is specified.
 
 optional arguments:
@@ -80,72 +91,47 @@
                         The variable to use for grouping plotted values. An
                         integer value is treated as a column index, whereas a
                         string is treated as a column label.
 ```
 
 </details>
 
-### 3. Interactive Mode
-
-#### 3.1 Analyze data
+### 3. Interpreter Session
 
 ```python
 >>> eda_report.summarize(iris_data)
-                        OVERVIEW
-                        ========
-Numeric features: sepal_length, sepal_width, petal_length, petal_width
-Categorical features: species
-
-          Summary Statistics (Numeric features)
-          -------------------------------------
-              count    mean     std  min  25%   50%  75%  max  skewness  kurtosis
-sepal_length  150.0  5.8433  0.8281  4.3  5.1  5.80  6.4  7.9    0.3149   -0.5521
-sepal_width   150.0  3.0573  0.4359  2.0  2.8  3.00  3.3  4.4    0.3190    0.2282
-petal_length  150.0  3.7580  1.7653  1.0  1.6  4.35  5.1  6.9   -0.2749   -1.4021
-petal_width   150.0  1.1993  0.7622  0.1  0.3  1.30  1.8  2.5   -0.1030   -1.3406
-
-          Summary Statistics (Categorical features)
-          -----------------------------------------
-        count unique     top freq relative freq
-species   150      3  setosa   50        33.33%
-
-          Pearson's Correlation (Top 20)
-          ------------------------------
-petal_length & petal_width --> very strong positive correlation (0.96)
-sepal_length & petal_length --> very strong positive correlation (0.87)
-sepal_length & petal_width --> very strong positive correlation (0.82)
-sepal_width & petal_length --> moderate negative correlation (-0.43)
-sepal_width & petal_width --> weak negative correlation (-0.37)
-sepal_length & sepal_width --> very weak negative correlation (-0.12)
-```
-
-#### 3.2 Plot statistical graphs
-
-```python
->>> fig = ep.regression_plot(mpg_data["acceleration"], mpg_data["horsepower"],
-...                          labels=("Acceleration", "Horsepower"))
->>> fig.savefig("regression-plot.png")
-```
 
-<img src="https://raw.githubusercontent.com/Tim-Abwao/eda-report/dev/docs/source/_static/regression-plot.png" width=400px style="display: block; margin: auto;">
-
-#### 3.3 Generate a report
-
-```python
->>> eda_report.get_word_report(iris_data)
-Analyze variables:  100%|███████████████████████████████████| 5/5
-Plot variables:     100%|███████████████████████████████████| 5/5
-Bivariate analysis: 100%|███████████████████████████████████| 6/6 pairs.
-[INFO 16:14:53.648] Done. Results saved as 'eda-report.docx'
-<eda_report.document.ReportDocument object at 0x7f196753bd60>
+                  Summary Statistics for Numeric features (4)
+                  -------------------------------------------
+                count     avg  stddev  min  25%   50%  75%  max  skewness  kurtosis
+  sepal_length    150  5.8433  0.8281  4.3  5.1  5.80  6.4  7.9    0.3149   -0.5521
+  sepal_width     150  3.0573  0.4359  2.0  2.8  3.00  3.3  4.4    0.3190    0.2282
+  petal_length    150  3.7580  1.7653  1.0  1.6  4.35  5.1  6.9   -0.2749   -1.4021
+  petal_width     150  1.1993  0.7622  0.1  0.3  1.30  1.8  2.5   -0.1030   -1.3406
+
+                Summary Statistics for Categorical features (1)
+                -----------------------------------------------
+                    count unique     top freq relative freq
+            species   150      3  setosa   50        33.33%
+
+
+                        Pearson's Correlation (Top 20)
+                        ------------------------------
+      petal_length & petal_width -> very strong positive correlation (0.96)
+     sepal_length & petal_length -> very strong positive correlation (0.87)
+      sepal_length & petal_width -> very strong positive correlation (0.82)
+      sepal_width & petal_length -> moderate negative correlation (-0.43)
+       sepal_width & petal_width -> weak negative correlation (-0.37)
+      sepal_length & sepal_width -> very weak negative correlation (-0.12)
 ```
 
-Visit the [official documentation][docs] for more info.
+Check out the [documentation][docs] for more features and details.
 
 [docs]: https://eda-report.readthedocs.io/
 [eda-report-pypi]: https://pypi.org/project/eda-report/
 [matplotlib]: https://matplotlib.org/
 [pandas]: https://pandas.pydata.org/
 [python-docx]: https://python-docx.readthedocs.io/
 [scipy]: https://scipy.org/
-[screencast]: https://raw.githubusercontent.com/Tim-Abwao/eda-report/dev/docs/source/_static/screencast.gif
+[gui-screencast]: https://raw.githubusercontent.com/Tim-Abwao/eda-report/dev/docs/source/_static/screencast.gif
+[report-screencast]: https://raw.githubusercontent.com/Tim-Abwao/eda-report/dev/docs/source/_static/report.gif
 [tkdocs]: https://tkdocs.com/index.html
```

### Comparing `eda_report-2.7.3/eda_report/__init__.py` & `eda_report-2.8.0/eda_report/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,71 @@
 from collections.abc import Iterable
 from typing import Union
 
+from eda_report._validate import _validate_dataset
+from eda_report.bivariate import Dataset
 from eda_report.document import ReportDocument
-from eda_report.multivariate import MultiVariable
+from eda_report.univariate import Variable
 
-__version__ = "2.7.3"
+__version__ = "2.8.0"
 
 
 def get_word_report(
     data: Iterable,
     *,
     title: str = "Exploratory Data Analysis Report",
     graph_color: str = "cyan",
-    groupby_data: Union[str, int] = None,
+    groupby_variable: Union[str, int] = None,
     output_filename: str = "eda-report.docx",
     table_style: str = "Table Grid",
 ) -> ReportDocument:
-    """Analyzes data, and generates a report in *Word* (*.docx*) format.
+    """Analyze `data`, and generate a report document in *Word* (*.docx*)
+    format.
 
     Args:
         data (Iterable): The data to analyze.
         title (str, optional): The title to assign the report. Defaults to
             "Exploratory Data Analysis Report".
         graph_color (str, optional): The color to apply to the graphs.
             Defaults to "cyan".
-        groupby_data (Union[str, int], optional): The label/index for the
+        groupby_variable (Union[str, int], optional): The label/index for the
             column to use to group values. Defaults to None.
-        output_filename (str, optional): The name and path to save the report
+        output_filename (str, optional): The name/path to save the report
             document. Defaults to "eda-report.docx".
         table_style (str, optional): The style to apply to the tables created.
             Defaults to "Table Grid".
 
     Returns:
         ReportDocument: Document object with analysis results.
 
     Example:
         .. literalinclude:: examples.txt
-           :lines: 145-151
-
+           :lines: 135-141
     """
     return ReportDocument(
         data,
         title=title,
         graph_color=graph_color,
         output_filename=output_filename,
-        groupby_data=groupby_data,
+        groupby_variable=groupby_variable,
         table_style=table_style,
     )
 
 
-def summarize(data: Iterable) -> MultiVariable:
+def summarize(data: Iterable) -> Union[Variable, Dataset]:
     """Get summary statistics for the supplied data.
 
     Args:
         data (Iterable): The data to analyze.
 
     Returns:
-        MultiVariable: Analysis results.
+        Union[Variable, Dataset]: Analysis results.
 
-    Examples:
+    Example:
         .. literalinclude:: examples.txt
-           :lines: 155-212
-
+           :lines: 171-194
     """
-    return MultiVariable(data)
+    data = _validate_dataset(data)
+    if data.shape[1] == 1:
+        return Variable(data.squeeze())
+    else:
+        return Dataset(data)
```

### Comparing `eda_report-2.7.3/eda_report/cli.py` & `eda_report-2.8.0/eda_report/_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 from typing import Optional
 
+from eda_report._read_file import df_from_file
 from eda_report.document import ReportDocument
-from eda_report.read_file import df_from_file
 
 
 def process_cli_args() -> argparse.Namespace:
     """Captures and parses input from the command line interface using the
     :mod:`argparse` module from the Python standard library.
 
     Returns:
@@ -20,76 +20,67 @@
         prog="eda-report",
         description=(
             "Automatically analyze data and generate reports. A graphical user"
             " interface will be launched if none of the optional arguments is "
             "specified."
         ),
     )
-
     parser.add_argument(
         "-i",
         "--infile",
         type=df_from_file,
         help="A .csv or .xlsx file to analyze.",
     )
-
     parser.add_argument(
         "-o",
         "--outfile",
         default="eda-report.docx",
         help="The output name for analysis results (default: %(default)s)",
     )
-
     parser.add_argument(
         "-t",
         "--title",
         default="Exploratory Data Analysis Report",
         help="The top level heading for the report (default: %(default)s)",
     )
-
     parser.add_argument(
         "-c",
         "--color",
         default="cyan",
         help="The color to apply to graphs (default: %(default)s)",
     )
-
     parser.add_argument(
         "-g",
         "-T",
         "--groupby",
         "--target",
         help=(
             "The variable to use for grouping plotted values. An integer value"
             " is treated as a column index, whereas a string is treated as a"
             " column label."
         ),
     )
-
     return parser.parse_args()
 
 
 def run_from_cli() -> Optional[ReportDocument]:
     """Creates an exploratory data analysis report in *Word* format using input
     from the command line interface.
 
     This is the function executed when the package is run as a script (using
     ``python -m eda_report``). It is also the entry point for the
     ``eda-report`` command (console script).
     """
     args = process_cli_args()
-
     if args.infile is None:
         from eda_report.gui import EDAGUI
-
         # Launch graphical user interface to select and analyze a file
         app = EDAGUI()
         app.mainloop()
-
     else:
         ReportDocument(
             args.infile,
             title=args.title,
             graph_color=args.color,
             output_filename=args.outfile,
-            groupby_data=args.groupby,
+            groupby_variable=args.groupby,
         )
```

### Comparing `eda_report-2.7.3/eda_report/content.py` & `eda_report-2.8.0/eda_report/univariate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,268 +1,299 @@
-from multiprocessing import Pool
-from typing import Any, Dict, Iterable, Optional, Union
+from collections.abc import Iterable
+from textwrap import shorten
+from typing import Dict, Optional, Tuple
 
-import pandas as pd
-from tqdm import tqdm
+from pandas import DataFrame, Series
+from pandas.api.types import (
+    is_bool_dtype,
+    is_datetime64_any_dtype,
+    is_numeric_dtype,
+)
+from scipy import stats
 
-from eda_report.multivariate import MultiVariable, _select_dtypes
-from eda_report.plotting import _plot_multivariable, _plot_variable
-from eda_report.univariate import Variable, _analyze_univariate
-from eda_report.validate import validate_groupby_data
-
-
-def _get_contingency_tables(
-    categorical_df: pd.DataFrame, groupby_data: pd.Series
-) -> Dict[str, pd.DataFrame]:
-    """Get contingency tables for categorical variables.
+from eda_report._validate import _validate_univariate_input
 
-    Args:
-        categorical_df (pandas.DataFrame): Categorical data.
-        groupby_data (pandas.Series): Values to group by.
 
-    Returns:
-        Dict[str, pd.DataFrame]: Contingency tables for each column.
-    """
-    if (categorical_df.shape[1] == 0) or (groupby_data is None):
-        return {}
-
-    contingency_tables = {
-        col: pd.crosstab(
-            index=categorical_df[col],
-            columns=groupby_data,
-            margins=True,
-            margins_name="Total",
-        )
-        for col in categorical_df
-        # Only include columns with upto 20 unique values to cut clutter
-        if categorical_df[col].nunique() <= 20
-    }
-    # Exclude groupby_data in case it is among the categorical cols
-    contingency_tables.pop(groupby_data.name, None)
-    return contingency_tables
+class Variable:
 
-
-class _AnalysisResult:
-    """Analyzes data, and stores the resultant summary statistics and graphs.
+    """Obtain summary statistics and properties such as data type, missing
+    value info, ..., from one-dimensional datasets.
 
     Args:
-        data (Iterable): The data to analyse.
-        graph_color (str, optional): The color to apply to the graphs.
-            Defaults to "cyan".
-        groupby_data (Union[str, int], optional): The column to
-            use to group values. Defaults to None.
+        data (Iterable): The data to analyze.
+        name (str, optional): The name to assign the variable. Defaults to
+            None.
 
+    Examples:
+        .. literalinclude:: examples.txt
+           :lines: 6-31
+        .. literalinclude:: examples.txt
+           :lines: 35-49
+        .. literalinclude:: examples.txt
+           :lines: 53-70
     """
 
-    def __init__(
-        self,
-        data: Iterable,
-        graph_color: str = "cyan",
-        groupby_data: Union[str, int] = None,
-    ) -> None:
-        self.GRAPH_COLOR = graph_color
-        self.multivariable = MultiVariable(data)
-        self.GROUPBY_DATA = validate_groupby_data(
-            data=self.multivariable.data, groupby_data=groupby_data
-        )
-        self.analyzed_variables = self._analyze_variables()
-        self.univariate_stats = self._get_univariate_statistics()
-        self.normality_tests = self._test_for_normality()
-        self.univariate_graphs = self._get_univariate_graphs()
-        self.bivariate_graphs = _plot_multivariable(
-            self.multivariable, color=graph_color
-        )
-        self.bivariate_summaries = self._get_bivariate_summaries()
+    def __init__(self, data: Iterable, *, name: str = None) -> None:
+        data = _validate_univariate_input(data, name=name)
 
-    def _analyze_variables(self) -> Dict[str, Variable]:
-        """Compute summary statistics and assess variable properties.
+        #: str: The variable's *name*. If no name is specified
+        #: during instantiation, the name will be equal to the value of the
+        #: ``name`` attribute of the input data (if present), or None.
+        self.name = data.name
+
+        #: str: The variable's *type* — one of *"boolean"*, *"categorical"*,
+        #: *"datetime"*, *"numeric"* or *"numeric (<=10 levels)"*.
+        self.var_type = self._get_variable_type(data)
+
+        #: int: The *number of unique values* present in the variable.
+        self.num_unique = data.nunique()
+
+        #: list: The *unique values* present in the variable.
+        self.unique_values = sorted(data.dropna().unique())
+
+        #: str: The number of *missing values* in the form
+        #: ``number (percentage%)`` e.g "4 (16.67%)".
+        self.missing = self._get_missing_values_info(data)
+        self._num_non_null = len(data.dropna())
+
+        #: dict: Descriptive statistics
+        self.summary_stats = self._get_summary_statistics(data)
+        self._normality_test_results = self._test_for_normality(data)
+        self._most_common_categories = self._get_most_common_categories(data)
+
+    def __repr__(self) -> str:
+        """Define the string representation of a `Variable`.
 
         Returns:
-            Dict[str, Variable]: Univariate analysis results.
+            str: Variable summary.
         """
-        data = self.multivariable.data
-        with Pool() as p:
-            univariate_stats = dict(
-                tqdm(
-                    # Analyze variables concurrently
-                    p.imap(_analyze_univariate, data.items()),
-                    # Progress-bar options
-                    total=data.shape[1],
-                    bar_format=(
-                        "{desc} {percentage:3.0f}%|{bar:35}| "
-                        "{n_fmt}/{total_fmt}"
-                    ),
-                    desc="Analyze variables: ",
-                    dynamic_ncols=True,
-                )
-            )
-        # Create contingency tables
-        categorical_cols = [
-            col_name
-            for col_name, var in univariate_stats.items()
-            if var.var_type != "numeric"
-        ]
-        self.contingency_tables = _get_contingency_tables(
-            data[categorical_cols], self.GROUPBY_DATA
+        sample_values = shorten(
+            f"{self.num_unique} -> {self.unique_values}", 60
         )
+        basic_details = "\n".join(
+            [
+                f"\nName: {self.name}",
+                f"Type: {self.var_type}",
+                f"Non-null Observations: {self._num_non_null}",
+                f"Unique Values: {sample_values}",
+                f"Missing Values: {self.missing}",
+            ]
+        )
+        if self.var_type == "numeric":
+            summary_stats = "\n".join(
+                [
+                    f"\t{key + ':':21} {value :>15.4f}"
+                    for key, value in self.summary_stats.items()
+                ],
+            )
+            return "\n".join(
+                [
+                    f"{basic_details}\n",
+                    "\t\t  Summary Statistics",
+                    "\t\t  ------------------",
+                    summary_stats,
+                    "\n\t\t  Tests for Normality",
+                    "\t\t  -------------------",
+                    f"{self._normality_test_results}",
+                ]
+            )
+        elif self.var_type == "datetime":
+            summary_stats = "\n".join(
+                [
+                    f"\t{key + ':':18} {str(value):>22}"
+                    for key, value in self.summary_stats.items()
+                ],
+            )
+            return "\n".join(
+                [
+                    f"{basic_details}\n",
+                    "\t\t  Summary Statistics",
+                    "\t\t  ------------------",
+                    summary_stats,
+                ]
+            )
+        else:
+            summary_stats = "\n".join(
+                [
+                    f"{key}: {value}"
+                    for key, value in self.summary_stats.items()
+                ]
+            )
+            most_common = "\n".join(
+                [
+                    f"{str(key):>24}: {value:}"
+                    for key, value in self._most_common_categories.items()
+                ]
+            )
+            return "\n".join(
+                [
+                    basic_details,
+                    summary_stats,
+                    "\n\t\tMost Common Items",
+                    "\t\t-----------------",
+                    most_common,
+                ]
+            )
 
-        return univariate_stats
+    def _get_variable_type(self, data: Series) -> str:
+        """Determine the variable type.
 
-    def _get_univariate_statistics(self) -> Dict[str, pd.DataFrame]:
-        """Get a dataframe of summary statistics for all variables.
+        Args:
+            data (pandas.Series): The data to analyze.
 
         Returns:
-            Dict[str, pandas.DataFrame]: Summary statistics.
+            str: The variable type: `boolean`, `categorical`, `datetime`,
+            `numeric` or `numeric (<10 levels)`.
         """
-        return {
-            name: variable.summary_statistics._get_summary_statistics()
-            .to_frame()
-            .round(4)
-            for name, variable in self.analyzed_variables.items()
-        }
-
-    def _test_for_normality(self) -> Dict[str, pd.DataFrame]:
-        """Perform tests for normality.
+        if is_numeric_dtype(data):
+            if is_bool_dtype(data) or set(data.dropna()) == {0, 1}:
+                # Consider boolean data as categorical
+                return "boolean"
+            elif data.nunique() <= 10:
+                # Consider numeric data with <= 10 unique values categorical
+                return "numeric (<=10 levels)"
+            else:
+                return "numeric"
+        elif set(data.dropna()) in [{False, True}, {"No", "Yes"}, {"N", "Y"}]:
+            return "boolean"
+        elif is_datetime64_any_dtype(data):
+            return "datetime"
+        else:
+            return "categorical"
 
-        Returns:
-            Dict[str, pandas.DataFrame]: Normality test results.
-        """
-        return {
-            name: variable.summary_statistics._test_for_normality()
-            for name, variable in self.analyzed_variables.items()
-            if variable.var_type == "numeric"
-        }
+    def _get_missing_values_info(self, data: Series) -> Optional[str]:
+        """Get the number of missing values.
 
-    def _get_univariate_graphs(self) -> Dict[str, Dict]:
-        """Plot graphs for all variables present.
+        Args:
+            data (pandas.Series): The data to analyze.
 
         Returns:
-            Dict[str, Dict]: Univariate graphs.
+            Optional[str]: Details about the number of missing values.
         """
-        with Pool() as p:
-            variables_hue_and_color = [
-                (variable, self.GROUPBY_DATA, self.GRAPH_COLOR)
-                for variable in self.analyzed_variables.values()
-            ]
-            univariate_graphs = dict(
-                tqdm(
-                    # Plot variables in parallel processes
-                    p.imap(_plot_variable, variables_hue_and_color),
-                    # Progress-bar options
-                    total=len(self.analyzed_variables),
-                    bar_format=(
-                        "{desc} {percentage:3.0f}%|{bar:35}| "
-                        "{n_fmt}/{total_fmt}"
-                    ),
-                    desc="Plot variables:    ",
-                    dynamic_ncols=True,
-                )
-            )
-        return univariate_graphs
+        missing_values = data.isna().sum()
+        if missing_values == 0:
+            return None
+        else:
+            return f"{missing_values:,} ({missing_values / len(data):.2%})"
 
-    def _get_bivariate_summaries(self) -> Optional[Dict[str, str]]:
-        """Get descriptions of the nature of correlation between numeric
-        column pairs.
+    def _get_summary_statistics(self, data: Series) -> Dict:
+        """Compute summary statistics for the variable based on data type.
+
+        Args:
+            data (pandas.Series): The data to analyze.
 
         Returns:
-            Optional[Dict[str, str]]: Correlation info.
+            Dict: Summary statistics.
         """
-        if self.multivariable._correlation_values is None:
-            return None
+        if self.var_type == "numeric":
+            stats = data.describe()
+            return {
+                "Average": stats["mean"],
+                "Standard Deviation": stats["std"],
+                "Minimum": stats["min"],
+                "Lower Quartile": stats["25%"],
+                "Median": stats["50%"],
+                "Upper Quartile": stats["75%"],
+                "Maximum": stats["max"],
+                "Skewness": data.skew(),
+                "Kurtosis": data.kurt(),
+            }
+        elif self.var_type == "datetime":
+            stats = data.describe()
+            return {
+                "Average": stats["mean"],
+                "Minimum": stats["min"],
+                "Lower Quartile": stats["25%"],
+                "Median": stats["50%"],
+                "Upper Quartile": stats["75%"],
+                "Maximum": stats["max"],
+            }
         else:
-            # Take the top 20 pairs by magnitude of correlation.
-            # 20 var_pairs ≈ 10+ pages
-            # 20 numeric columns == 190 var_pairs ≈ 95+ pages.
-            pairs_to_include = [
-                pair for pair, _ in self.multivariable._correlation_values[:20]
-            ]
-            correlation_descriptions = (
-                self.multivariable._correlation_descriptions
-            )
+            data = data.copy().astype("category")
+            stats = data.describe()
             return {
-                var_pair: (
-                    f"{var_pair[0].title()} and {var_pair[1].title()} have "
-                    f"{correlation_descriptions[var_pair]}."
-                )
-                for var_pair in pairs_to_include
+                "Mode (Most frequent)": stats["top"],
+                "Maximum frequency": stats["freq"],
             }
 
+    def _test_for_normality(
+        self, data: Series, alpha: float = 0.05
+    ) -> DataFrame:
+        """Perform the "D'Agostino's K-squared", "Kolmogorov-Smirnov" and
+        "Shapiro-Wilk" tests for normality.
 
-class _ReportContent(_AnalysisResult):
-    """Prepares textual summaries of analysis results.
+        Args:
+            data (pandas.Series): The data to analyze.
+            alpha (float, optional): The level of significance. Defaults to
+                0.05.
 
-    Args:
-        data (Iterable): The data to analyze.
-        title (str, optional): The title to assign the report. Defaults to
-            "Exploratory Data Analysis Report".
-        graph_color (str, optional): The color to apply to the graphs.
-            Defaults to "cyan".
-        groupby_data (Union[str, int], optional): The column to
-            use to group values. Defaults to None.
-    """
+        Returns:
+            pandas.DataFrame: Table of results.
+        """
+        data = data.dropna()
+        if self.var_type == "numeric":
+            # The scipy implementation of the Shapiro-Wilk test reports:
+            # "For N > 5000 the W test statistic is accurate but the p-value
+            # may not be."
+            shapiro_sample = data.sample(5000) if len(data) > 5000 else data
+            tests = [
+                "D'Agostino's K-squared test",
+                "Kolmogorov-Smirnov test",
+                "Shapiro-Wilk test",
+            ]
+            p_values = [
+                stats.normaltest(data).pvalue,
+                stats.kstest(data, "norm", N=200).pvalue,
+                stats.shapiro(shapiro_sample).pvalue,
+            ]
+            results = DataFrame(index=tests)
+            results["p-value"] = [f"{x:.7f}" for x in p_values]
+            results[f"Conclusion at α = {alpha}"] = [
+                "Possibly normal"
+                if p_value > alpha
+                else "Unlikely to be normal"
+                for p_value in p_values
+            ]
+            return results
+        else:
+            return None
 
-    def __init__(
-        self,
-        data: Iterable,
-        *,
-        title: str = "Exploratory Data Analysis Report",
-        graph_color: str = "cyan",
-        groupby_data: Union[str, int] = None,
-    ) -> None:
-        super().__init__(
-            data, graph_color=graph_color, groupby_data=groupby_data
-        )
-        self.TITLE = title
-        self.intro_text = self._get_introductory_summary()
-        self.variable_descriptions = self._describe_variables()
+    def _get_most_common_categories(self, data: Series) -> Dict:
+        """Get the top 10 frequently occuring categories.
 
-    def _get_introductory_summary(self) -> str:
-        """Get an overview of the number of rows and the nature of columns.
+        Args:
+            data (pandas.Series): The data to analyze.
 
         Returns:
-            str: Introduction.
+            Dict: Top 10 categories and their frequency info.
         """
-        num_rows, num_cols = self.multivariable.data.shape
-
-        if num_rows == 1:
-            rows = "1 row (observation)"
+        data = data.dropna()
+        if self.var_type in {"numeric", "datetime"}:
+            return None
         else:
-            rows = f"{num_rows:,} rows (observations)"
+            top_10 = data.value_counts().nlargest(10)
+            return {
+                key: f"{val} ({val/len(data):.2%})"
+                for key, val in top_10.items()
+            }
 
-        if num_cols == 1:
-            cols = "1 column (feature)"
-        else:
-            cols = f"{num_cols:,} columns (features)"
+    def rename(self, name: str) -> None:
+        """Update the variable's name.
 
-        # Get numeric column info
-        numeric_cols = _select_dtypes(self.multivariable.data, "number")
-        if numeric_cols is None:
-            numeric = ""
-        elif numeric_cols.shape[1] == 1:
-            numeric = ", 1 of which is numeric"
-        else:
-            numeric = f", {numeric_cols.shape[1]} of which are numeric"
+        Args:
+            name (str): New name.
+        """
+        self.name = name
 
-        return f"The dataset consists of {rows} and {cols}{numeric}."
 
-    def _describe_variables(self) -> Dict[str, Any]:
-        """Get summary statistics for a variable.
+def _analyze_univariate(name_and_data: Tuple) -> Variable:
+    """Helper function to concurrently analyze data with multiprocessing.
 
-        Args:
-            univariate_stats (Variable): The data to analyze.
-
-        Returns:
-            Dict[str, Any]: Summary statistics.
-        """
-        descriptions = {}
-        for name, variable in self.analyzed_variables.items():
-            if variable.num_unique == 1:
-                unique_vals = "1 unique value"
-            else:
-                unique_vals = f"{variable.num_unique:,} unique values"
+    Args:
+        name_and_data (Tuple): Name and data.
 
-            descriptions[name] = (
-                f"{variable.name.capitalize()} is a {variable.var_type} "
-                f"variable with {unique_vals}. {variable.missing} of its "
-                "values are missing."
-            )
-        return descriptions
+    Returns:
+        Variable: `Variable` instance.
+    """
+    name, data = name_and_data
+    var = Variable(data, name=name)
+    return name, var
```

### Comparing `eda_report-2.7.3/eda_report/document.py` & `eda_report-2.8.0/eda_report/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,226 +1,185 @@
 import logging
 from typing import Iterable, Sequence, Union
 
 from docx import Document
 from docx.enum.text import WD_ALIGN_PARAGRAPH
 from docx.shared import Inches, Pt
-from docx.text.parfmt import ParagraphFormat
-from pandas.core.frame import DataFrame
+from docx.text.paragraph import Paragraph
+from pandas import DataFrame, Series
 
-from eda_report.content import _ReportContent
-from eda_report.multivariate import _select_dtypes
+from eda_report._content import _ReportContent
 
 logging.basicConfig(
     format="[%(levelname)s %(asctime)s.%(msecs)03d] %(message)s",
     level=logging.INFO,
     datefmt="%H:%M:%S",
 )
 # Set matplotlib logging level to WARNING.
 mpl_logger = logging.getLogger("matplotlib")
 mpl_logger.setLevel(logging.WARNING)
 
 
 class ReportDocument(_ReportContent):
-    """Creates a :class:`~docx.document.Document` with analysis results
-    using `python-docx`_.
+    """Creates a report :class:`~docx.document.Document` with analysis results.
 
     The report consists of 3 main sections:
 
     #. An **Overview** of the data and its features.
     #. **Univariate Analysis**: Summary statistics and graphs for each feature.
     #. **Bivariate Analysis**: Pair-wise comparisons of numerical features.
 
-    .. _python-docx: https://python-docx.readthedocs.io/en/latest/
-
     Args:
         data (Iterable): The data to analyze.
         title (str, optional): The title to assign the report. Defaults to
             "Exploratory Data Analysis Report".
         graph_color (str, optional): The color to apply to the graphs.
             Defaults to "cyan".
-        groupby_data (Union[str, int], optional): The column to
+        groupby_variable (Union[str, int], optional): The column to
             use to group values. Defaults to None.
-        output_filename (str, optional): The file name or path to save the
-            document to. Defaults to "eda-report.docx".
+        output_filename (str, optional): The name/path to save the document
+            to. Defaults to "eda-report.docx".
         table_style (str, optional): The style to apply to the tables created.
             Defaults to "Table Grid".
     """
 
     def __init__(
         self,
         data: Iterable,
         *,
         title: str = "Exploratory Data Analysis Report",
         graph_color: str = "cyan",
-        groupby_data: Union[str, int] = None,
+        groupby_variable: Union[str, int] = None,
         output_filename: str = "eda-report.docx",
         table_style: str = "Table Grid",
     ) -> None:
         super().__init__(
             data,
             title=title,
             graph_color=graph_color,
-            groupby_data=groupby_data,
+            groupby_variable=groupby_variable,
         )
         self.OUTPUT_FILENAME = output_filename
         self.TABLE_STYLE = table_style
-        self.document = Document()
-        self._get_report()
-
-    def _get_report(self) -> None:
-        """Calculate summary statistics, plot graphs, and save the results as
-        a .docx file.
-        """
-        self._create_title_page()
+        self.document = Document()  # Initialize report document
+        self._create_cover_page()
         self._get_univariate_analysis()
 
-        if self.multivariable._correlation_values is not None:
+        if self.dataset._correlation_values is not None:
             self._get_bivariate_analysis()
 
         self._to_file()
         logging.info(f"Done. Results saved as {self.OUTPUT_FILENAME!r}")
 
-    def _create_title_page(self) -> None:
-        """Add a title and a brief summary of the data."""
+    def _create_cover_page(self) -> None:
+        """Add a title and overview of the data."""
         self.document.add_heading(self.TITLE, level=0)
-
         self.document.add_paragraph(self.intro_text)
-
         self._get_numeric_overview_table()
         self._get_categorical_overview_table()
         self.document.add_page_break()
 
-    def _format_heading_spacing(
-        self, format: ParagraphFormat, before: int = 15, after: int = 7
-    ) -> None:
-        """Set the spacing above or below a heading.
-
-        Args:
-            format (ParagraphFormat): The heading's format.
-            before (int, optional): Size of spacing above the heading in pt.
-                Defaults to 15.
-            after (int, optional): Size of spacing below the heading in pt.
-                Defaults to 7.
-        """
-        format.space_before = Pt(before)
-        format.space_after = Pt(after)
-
     def _get_numeric_overview_table(self) -> None:
         """Create a table with an overview of the numeric features present."""
-        numeric_cols = _select_dtypes(self.multivariable.data, "number")
-        if numeric_cols is None:
+        if self.dataset._numeric_stats is None:
             return None
         else:
             heading = self.document.add_heading(
                 "Overview of Numeric Features", level=1
             )
-            self._format_heading_spacing(heading.paragraph_format)
-            # count | mean | std | min | 25% | 50% | 75% | max
+            self._format_paragraph_spacing(heading)
+            # count | avg | stddev | min | 25% | 50% | 75% | max
             self._create_table(
-                data=self.multivariable._numeric_stats,
+                data=self.dataset._numeric_stats,
                 header=True,
                 column_widths=(1.2,) + (0.7,) * 8,
                 font_size=8.5,
                 style="Normal Table",
             )
 
     def _get_categorical_overview_table(self) -> None:
         """Create a table with an overview of the categorical features
         present.
         """
-        categorical_cols = _select_dtypes(
-            self.multivariable.data, "bool", "category", "object"
-        )
-        if categorical_cols is None:
+        if self.dataset._categorical_stats is None:
             return None
         else:
             heading = self.document.add_heading(
                 "Overview of Categorical Features", level=1
             )
-            self._format_heading_spacing(heading.paragraph_format)
+            self._format_paragraph_spacing(heading)
             # column-name | count | unique | top | freq | relative freq
             self._create_table(
-                data=self.multivariable._categorical_stats,
+                data=self.dataset._categorical_stats,
                 header=True,
                 column_widths=(1.2,) + (0.9,) * 5,
                 font_size=8.5,
                 style="Normal Table",
             )
 
     def _get_univariate_analysis(self) -> None:
         """Get a brief introduction, summary statistics, and graphs for each
         individual variable.
         """
         univariate_heading = self.document.add_heading(
             "1. Univariate Analysis", level=1
         )
-        self._format_heading_spacing(
-            univariate_heading.paragraph_format, before=0, after=0
-        )
-        for idx, variable in enumerate(
-            self.analyzed_variables.values(), start=1
-        ):
+        self._format_paragraph_spacing(univariate_heading, before=0, after=0)
+        for idx, variable in enumerate(self.variables.values(), start=1):
             var_name = variable.name
             description = self.variable_descriptions[var_name]
-            summary_stats = self.univariate_stats[var_name]
+            summary_stats = Series(self.univariate_stats[var_name]).to_frame()
             graphs = self.univariate_graphs[var_name]
             contingency_table = self.contingency_tables.get(var_name)
             normality_tests = self.normality_tests.get(var_name)
-
+            # Variable's title and brief description
             heading = self.document.add_heading(
                 f"1.{idx} {var_name}".title(), level=2
             )
-            self._format_heading_spacing(
-                heading.paragraph_format, before=12, after=5
-            )
+            self._format_paragraph_spacing(heading, before=12, after=5)
             self.document.add_paragraph(description)
-
+            # Summary statistics table
             stats_heading = self.document.add_heading(
                 "Summary Statistics", level=4
             )
             stats_heading.alignment = WD_ALIGN_PARAGRAPH.CENTER
-
             self._create_table(summary_stats, column_widths=[2.5, 2])
-
-            for graph in (graphs).values():
-                self.document.add_picture(graph, width=Inches(4.4))
+            # Images of plotted graphs
+            for name, image in graphs.items():
+                width = 3.3 if name == "prob_plot" else 4.2
+                self.document.add_picture(image, width=Inches(width))
                 picture_paragraph = self.document.paragraphs[-1]
                 picture_paragraph.alignment = WD_ALIGN_PARAGRAPH.CENTER
 
             if contingency_table is not None:
                 contingency_table_heading = self.document.add_heading(
                     "Contingency table", level=4
                 )
                 contingency_table_heading.alignment = WD_ALIGN_PARAGRAPH.CENTER
-                subtext = self.document.add_paragraph(
-                    f"Index = '{var_name}' "
-                    f"(missing: {variable.data.isna().sum()}). "
+                context = self.document.add_paragraph(
+                    f"Index = '{var_name}', "
                     f"Columns = '{self.GROUPBY_DATA.name}' "
-                    f"(missing: {self.GROUPBY_DATA.isna().sum()})"
                 )
-                subtext.alignment = WD_ALIGN_PARAGRAPH.CENTER
-                subtext.runs[0].font.size = Pt(8)
-
+                context.alignment = WD_ALIGN_PARAGRAPH.CENTER
+                context.runs[0].font.size = Pt(8)
                 n_cols = contingency_table.shape[1]
-                max_width = 5 if n_cols > 5.2 else 3.2
+                max_width = 5.2 if n_cols > 5 else 3.2
                 col_width = max_width / n_cols
                 self._create_table(
                     data=contingency_table,
                     header=True,
                     column_widths=(1.2,) + (col_width,) * n_cols,
                     font_size=8.5,
                 )
 
             if normality_tests is not None:
                 norm_test_heading = self.document.add_heading(
                     "Tests for Normality", level=4
                 )
                 norm_test_heading.alignment = WD_ALIGN_PARAGRAPH.CENTER
-
                 # type | p-value | conclusion
                 self._create_table(
                     data=normality_tests,
                     header=True,
                     column_widths=(2.2, 1, 2),
                     font_size=8.5,
                     style="Normal Table",
@@ -231,118 +190,122 @@
     def _get_bivariate_analysis(self) -> None:
         """Get comparisons and regression-plots for pairs of numeric
         variables.
         """
         bivariate_heading = self.document.add_heading(
             "2. Bivariate Analysis", level=1
         )
-        self._format_heading_spacing(
-            bivariate_heading.paragraph_format, before=0
-        )
-
+        self._format_paragraph_spacing(bivariate_heading, before=0)
         overview_heading = self.document.add_heading("2.1 Overview", level=2)
-        self._format_heading_spacing(overview_heading.paragraph_format)
+        self._format_paragraph_spacing(overview_heading)
         self.document.add_picture(
             self.bivariate_graphs["correlation_plot"],
-            width=Inches(6.7),
+            width=Inches(6.4),
         )
         picture_paragraph = self.document.paragraphs[-1]
         picture_paragraph.alignment = WD_ALIGN_PARAGRAPH.CENTER
         self.document.add_page_break()
 
         pairwise_heading = self.document.add_heading(
             "2.2 Regression Plots (Top 20)", level=2
         )
-        self._format_heading_spacing(
-            pairwise_heading.paragraph_format, before=0
-        )
+        self._format_paragraph_spacing(pairwise_heading, before=0)
         for idx, var_pair in enumerate(self.bivariate_summaries, start=1):
             heading = self.document.add_heading(
                 f"2.2.{idx} {var_pair[0]} vs {var_pair[1]}".title(), level=3
             )
-            self._format_heading_spacing(
-                heading.paragraph_format, before=16, after=5
-            )
+            self._format_paragraph_spacing(heading, before=16, after=5)
             self.document.add_paragraph(self.bivariate_summaries[var_pair])
             self.document.add_picture(
                 self.bivariate_graphs["regression_plots"][var_pair],
-                width=Inches(3.5),
+                width=Inches(3.3),
             )
             picture_paragraph = self.document.paragraphs[-1]
             picture_paragraph.alignment = WD_ALIGN_PARAGRAPH.CENTER
 
+    def _format_paragraph_spacing(
+        self, paragraph: Paragraph, before: int = 15, after: int = 7
+    ) -> None:
+        """Set the spacing above or below a paragraph.
+
+        Args:
+            paragraph (docx.text.paragraph.Paragraph): A paragraph.
+            before (int, optional): Size of spacing above the paragraph in pt.
+                Defaults to 15.
+            after (int, optional): Size of spacing below the paragraph in pt.
+                Defaults to 7.
+        """
+        paragraph.paragraph_format.space_before = Pt(before)
+        paragraph.paragraph_format.space_after = Pt(after)
+
     def _create_table(
         self,
         data: DataFrame,
         column_widths: Sequence = (),
         font_face: str = "Courier New",
         font_size: float = 10,
         style: str = None,
         header: bool = False,
     ) -> None:
         """Generates a table for the supplied ``data``.
 
         Args:
             data (DataFrame): The data to tabulate.
-            column_widths (Sequence, optional): Column specifications.
+            column_widths (Sequence, optional): Column dimensions in inches.
                 Defaults to ().
-            font_face (str, optional): Font typeface for cell text. Defaults
-                to "Courier New".
+            font_face (str, optional): Font for cell text. Defaults to
+                "Courier New".
             font_size (float, optional): Font size. Defaults to 10.
             style (str, optional): A `Word` table style. Defaults to
                 None.
             header (bool, optional): Whether or not to include column names.
                 Defaults to False.
         """
-        n_cols = len(column_widths)
         table = self.document.add_table(
             rows=0,
-            cols=n_cols,
+            cols=len(column_widths),
             style=style or self.document.styles[self.TABLE_STYLE],
         )
         table.alignment = WD_ALIGN_PARAGRAPH.CENTER
-
-        # Set column dimensions
         for idx, width in enumerate(column_widths):
             table.columns[idx].width = Inches(width)
 
         if header:
             cells = table.add_row().cells
             header_labels = [""] + list(data.columns)
             for cell, value in zip(cells, header_labels):
                 cell.text = f"{value}"
-
                 # Font size and type-face have to be set at `run` level
                 run = cell.paragraphs[0].runs[0]
                 run.bold = True
                 run.font.size = Pt(font_size)
                 run.font.name = font_face
 
-        # Populate the rows
+        # Sequentially add and populate rows
         for row_data in data.itertuples():
             cells = table.add_row().cells
             for idx, (cell, value) in enumerate(zip(cells, row_data)):
-                text = f"{value}"
-                # Strip trailing zeros, if text is not all zeros.
-                if set(text) != {"0"}:
-                    text = text.rstrip("0").rstrip(".")
+                try:
+                    # Strip trailing zeros from float values
+                    text = f"{value:.4f}".rstrip("0").rstrip(".")
+                except ValueError:
+                    text = f"{value}"
 
                 cell.text = text
-
                 # Font size and type-face have to be set at `run` level
                 run = cell.paragraphs[0].runs[0]
                 run.font.size = Pt(font_size)
                 run.font.name = font_face
                 # Make first column values bold if header is True
                 if idx == 0 and header:
                     run.bold = True
 
+        # Add empty paragraph. "Spacing" for docx Table isn't yet implemented
         self.document.add_paragraph()
 
     def _to_file(self) -> None:
         """Save the report as a file."""
-        # Set page margins
         for section in self.document.sections:
             section.left_margin = Inches(1.2)
             section.right_margin = Inches(1.2)
 
         self.document.save(self.OUTPUT_FILENAME)
```

### Comparing `eda_report-2.7.3/eda_report/exceptions.py` & `eda_report-2.8.0/eda_report/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 class Error(Exception):
     """The base class for exceptions in this package."""
 
     pass
 
 
 class InputError(Error):
-    """The *Exception* raised when a given input object is *not of the
-    expected type* or is otherwise *invalid*.
+    """*Exception* raised when a given input object is *not of the expected
+    type* or is otherwise *invalid*.
 
     In most cases, an attempt is made to cast the erroneous input into the
     proper type, and this *Exception* is raised if it fails.
 
     Args:
         message (str): A brief description of the mishap detected.
     """
 
     def __init__(self, message: str) -> None:
         self.message = message
 
 
 class EmptyDataError(InputError):
-    """The *Exception* raised when an iterable input object has length zero
-    or has no items to yield.
+    """*Exception* raised when an iterable input object has length zero or has
+    no more items to yield.
     """
 
     pass
 
 
 class GroupbyVariableError(InputError):
-    """The *Exception* raised when the specified group-by variable is invalid.
-    """
+    """*Exception* raised when the specified group-by variable is invalid."""
 
     pass
```

### Comparing `eda_report-2.7.3/eda_report/gui.py` & `eda_report-2.8.0/eda_report/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,23 @@
         showinfo,
         showwarning,
     )
     from tkinter.simpledialog import askstring
 except (ImportError, ModuleNotFoundError) as error:
     print(
         f"{error}.\nPlease visit https://tkdocs.com/tutorial/install.html for"
-        " help installing it.\n\n"
-        "Or just specify an input file to by-pass the GUI.\n"
-        "Use eda-report -h for more details.",
+        " help installing it.\n\nOr just specify CLI args. Try eda-report -h "
+        "for more details."
     )
     exit()
 
+from eda_report._read_file import df_from_file
+from eda_report._validate import _validate_groupby_variable
 from eda_report.document import ReportDocument
 from eda_report.exceptions import GroupbyVariableError
-from eda_report.read_file import df_from_file
-from eda_report.validate import validate_groupby_data
 
 background_image = pkgutil.get_data(__name__, "images/background.png")
 icon = pkgutil.get_data(__name__, "images/icon.png")
 
 description = (
     "Speed up exploratory data analysis & reporting.\n\n"
     "Automatically analyze files, and get a Word report complete with "
@@ -35,25 +34,25 @@
 )
 
 
 class EDAGUI(Frame):  # pragma: no cover
     """The blueprint for the :mod:`tkinter` - based *graphical user
     interface* to the application.
 
-    The "Select a file" button launches a *file-dialog* to navigate to and
-    select a file to analyze.
-
     .. figure:: _static/screencast.*
        :alt: an image of the graphical user interface
 
+    The "Select a file" button launches a *file-dialog* to navigate to and
+    select a file to analyze.
+
     If a valid file is selected, *text-input widgets* and a *color-picker
     tool* pop up to help set the report's *title*,
-    *groupby variable(optional)* and *graph color*.
+    *target/groupby variable(optional)* and *graph color*.
 
-    Afterwards, a final file-dialog appears to help select the destination
+    Afterwards, a final file-dialog appears to help set the destination
     for the generated report.
 
     .. hint::
         For help with `Tk` - related issues, consider visiting `TkDocs`_.
 
     .. _`TkDocs`: https://tkdocs.com/index.html
     """
@@ -69,67 +68,61 @@
 
     def _create_widgets(self) -> None:
         """Creates the widgets for the graphical user interface: A Tk *Frame*
         with the *canvas(background image)*, *introductory text*, and a
         *button* to select files to analyze.
         """
         self.canvas = Canvas(self, width=560, height=320)
-
         # Set background image
         self.bg_image = PhotoImage(data=background_image)
         self.canvas.create_image((0, 0), image=self.bg_image, anchor="nw")
-
         # Add title
         self.canvas.create_text(
             (70, 30),
             anchor="nw",
             fill="black",
             font=("Courier", 28, "bold"),
             text="eda-report",
         )
-
-        # Add introductory text
+        # Add description
         self.canvas.create_text(
             (40, 90),
             anchor="nw",
             fill="black",
             font=("Courier", 12),
             text=description,
             width=480,
         )
-
         # Add a button to select input file
         self.button = Button(
             self,
             bg="#204060",
             command=self._create_report,
             default="active",
             fg="white",
             font=("Courier", 11),
             relief="flat",
             text="Select a file",
         )
         self.canvas.create_window(
             (180, 220), anchor="nw", height=40, width=200, window=self.button
         )
-
-        # Show current action
+        # Display current action
         self.current_action = StringVar()
         self.display_current_action = Label(
             self,
             bg="#c0d6e3",
             font=("Courier", 10, "italic"),
             textvariable=self.current_action,
         )
         self.canvas.create_window(
             (140, 280),
             anchor="nw",
             window=self.display_current_action,
         )
-
         self.canvas.pack()
 
     def _create_report(self) -> None:
         """Collects input from the graphical user interface, and uses the
         :class:`~eda_report.document.ReportDocument` object to generate a
         report.
         """
@@ -137,42 +130,43 @@
         self._get_data_from_file()
 
         if self.data is not None:
             self.current_action.set("Waiting for report title...")
             self._get_report_title()
 
             self.current_action.set("Waiting for group-by variable...")
-            self._get_groupby_data()
+            self._get_groupby_variable()
 
             self.current_action.set("Waiting for graph color...")
             self._get_graph_color()
 
             self.current_action.set("Analysing data & compiling the report...")
             self._get_save_as_name()
 
             # Generate and save the report using the collected arguments
             ReportDocument(
                 self.data,
                 title=self.report_title,
                 graph_color=self.graph_color,
                 output_filename=self.save_name,
-                groupby_data=self.groupby_data,
+                groupby_variable=self.groupby_variable,
             )
             self.current_action.set("")
             showinfo(message=f"Done! Report saved as {self.save_name!r}.")
 
-            # Clear stale data to free up memory
+            # Clear data to free up memory
             del self.data
 
     def _get_data_from_file(self, retries: int = 1) -> None:
         """Creates a file dialog to help navigate to and select a file to
         analyze.
 
         Args:
-            retries (int): Number of additional prompts, if input is invalid.
+            retries (int, optional): Number of additional prompts, if input is
+                invalid.
         """
         file_name = askopenfilename(
             title="Select a file to analyze",
             filetypes=(
                 ("All supported formats", ("*.csv", "*.xlsx")),
                 ("csv", "*.csv"),
                 ("excel", "*.xlsx"),
@@ -187,63 +181,58 @@
                 # No data if retry prompt is cancelled
                 self.data = None
         else:
             # No data if no file is selected and retry has been used up
             self.data = None
 
     def _get_report_title(self) -> None:
-        """Creates a simple dialog to capture text input for the desired
-        report title.
-        """
+        """Capture text input for the desired report title."""
         report_title = askstring(
             title="Report Title",
             prompt="Please enter your preferred title for the report:",
             initialvalue="Exploratory Data Analysis Report",
         )
-
         self.report_title = report_title or "Exploratory Data Analysis Report"
 
-    def _get_groupby_data(self) -> None:
+    def _get_groupby_variable(self) -> None:
         """Inquire about the groupby variable, and create a text box to
         collect input.
         """
         if askyesno(
             message="Would you like to specify a variable to group by?"
         ):
-            self.groupby_data = askstring(
+            self.groupby_variable = askstring(
                 title="Select Group-by Variable",
-                prompt="Please enter the name of the group-by variable:",
+                prompt="Please enter the name/index of the group-by variable:",
             )
             try:
-                validate_groupby_data(
-                    data=self.data, groupby_data=self.groupby_data
+                _validate_groupby_variable(
+                    data=self.data, groupby_variable=self.groupby_variable
                 )
             except GroupbyVariableError as error:
-                self.groupby_data = None
+                self.groupby_variable = None
                 showwarning(
                     title="Invalid Group-By Variable", message=error.message
                 )
         else:
-            self.groupby_data = None
+            self.groupby_variable = None
 
     def _get_graph_color(self) -> None:
         """Creates a graphical color picking tool to help set the desired
         color for the generated graphs.
         """
         color = askcolor(
             color="cyan", title="Please select a color for the graphs"
         )
         # Pick the hexadecimal color format. `askcolor` returns a tuple e.g
         # ((255.99609375, 69.26953125, 0.0), '#ff4500').
         self.graph_color = color[-1] or "cyan"
 
     def _get_save_as_name(self) -> None:
-        """Create a file dialog to help select a destination folder and file
-        name for the generated report.
-        """
+        """Create a file dialog to set destination of the generated report."""
         save_name = asksaveasfilename(
             initialdir=".",
             initialfile="eda-report.docx",
             filetypes=(("Word document", "*.docx"),),
             title="Please select Save As file name",
         )
         self.save_name = save_name or "eda-report.docx"
```

### Comparing `eda_report-2.7.3/eda_report/images/background.png` & `eda_report-2.8.0/eda_report/images/background.png`

 * *Files identical despite different names*

### Comparing `eda_report-2.7.3/eda_report/images/icon.png` & `eda_report-2.8.0/eda_report/images/icon.png`

 * *Files identical despite different names*

### Comparing `eda_report-2.7.3/eda_report/multivariate.py` & `eda_report-2.8.0/eda_report/bivariate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from collections.abc import Iterable
 from itertools import combinations
-from typing import List, Optional, Sequence
+from textwrap import indent
+from typing import List
 
-from pandas.core.frame import DataFrame
+from pandas import DataFrame
 
-from eda_report.univariate import Variable
-from eda_report.validate import validate_multivariate_input
+from eda_report._validate import _validate_dataset
 
 
 def _compute_correlation(dataframe: DataFrame) -> List:
     """Get the Pearson correlation coefficients for numeric variables.
 
     Args:
         dataframe (pandas.DataFrame): A 2D array of numeric data.
@@ -40,177 +40,172 @@
     Args:
         corr_value (str): Pearson's correlation coefficient.
 
     Returns:
         str: Brief description of correlation type.
     """
     nature = " positive" if corr_value > 0 else " negative"
-
     value = abs(corr_value)
     if value >= 0.8:
         strength = "very strong"
     elif value >= 0.6:
         strength = "strong"
     elif value >= 0.4:
         strength = "moderate"
     elif value >= 0.2:
         strength = "weak"
     elif value >= 0.05:
         strength = "very weak"
     else:
         strength = "virtually no"
         nature = ""
-
     return f"{strength}{ nature} correlation ({corr_value:.2f})"
 
 
-def _select_dtypes(
-    dataframe: DataFrame, *dtypes: Sequence[str]
-) -> Optional[DataFrame]:
-    """Get a DataFrame including only the specified `dtypes`.
+class Dataset:
+    """Analyze two-dimensional datasets to obtain descriptive statistics
+    and correlation information.
 
-    Args:
-        dataframe (pandas.DataFrame): A 2D array of numeric data.
-        *dtypes (str): Data types to include e.g. "bool", "number", etc.
-
-    Returns:
-        Optional[DataFrame]: Subset with the desired data types.
-    """
-    selected_cols = dataframe.select_dtypes(include=dtypes)
-    return selected_cols if selected_cols.shape[1] > 0 else None
-
-
-class MultiVariable:
-    """Defines objects that analyze two-dimensional datasets.
-
-    Input data is held as a :class:`pandas.DataFrame` in order to leverage
-    pandas_ built-in statistical methods, as well as functions
-    from the `SciPy ecosystem`_.
+    Input data is stored as a :class:`pandas.DataFrame` in order to leverage
+    pandas_' built-in statistical methods.
 
     .. _pandas: https://pandas.pydata.org/
-    .. _SciPy ecosystem: https://www.scipy.org/
-
-    .. note::
-       Not meant to be used directly: use the :func:`eda_report.summarize`
-       function instead.
 
     Args:
         data (Iterable): The data to analyze.
 
     Example:
         .. literalinclude:: examples.txt
-           :lines: 84-110
+           :lines: 78-100
     """
 
     def __init__(self, data: Iterable) -> None:
-
-        self.data = validate_multivariate_input(data)
+        self.data = _validate_dataset(data)
         self._get_summary_statistics()
         self._get_bivariate_analysis()
 
     def __repr__(self) -> str:
-        """Get the string representation for a ``Multivariable``.
+        """Get the string representation for a `Dataset`.
 
         Returns:
-            str: The string representation of the ``MultiVariable`` instance.
+            str: The string representation of the `Dataset` instance.
         """
-        if self.data.shape[1] == 1:
-            return str(
-                Variable(self.data.squeeze(), name=self.data.columns[0])
-            )
-
-        numeric_data = _select_dtypes(self.data, "number")
-        if numeric_data is None:
-            numeric_info = numeric_stats = ""
+        if self._numeric_stats is None:
+            numeric_stats = ""
         else:
-            numeric_info = f"Numeric features: {', '.join(numeric_data)}"
-            numeric_stats = (
-                "\n\t  Summary Statistics (Numeric features)\n"
-                "\t  -------------------------------------\n"
-                f"{self._numeric_stats}"
+            numeric_stats_title = (
+                "Summary Statistics for Numeric features "
+                f"({self._numeric_stats.shape[0]})"
+            )
+            numeric_stats = "\n".join(
+                [
+                    f"\n\t\t  {numeric_stats_title}",
+                    f"\t\t  {'-' * len(numeric_stats_title)}",
+                    indent(f"{self._numeric_stats}\n", "  "),
+                ]
             )
 
-        categorical_data = _select_dtypes(
-            self.data, "bool", "category", "object"
-        )
-        if categorical_data is None:
-            categorical_info = categorical_stats = ""
+        if self._categorical_stats is None:
+            categorical_stats = ""
         else:
-            categorical_info = (
-                f"Categorical features: {', '.join(categorical_data)}"
+            categorical_stats_title = (
+                "Summary Statistics for Categorical features "
+                f"({self._categorical_stats.shape[0]})"
             )
-            categorical_stats = (
-                "\n\t  Summary Statistics (Categorical features)\n"
-                "\t  -----------------------------------------\n"
-                f"{self._categorical_stats}"
+            categorical_stats = "\n".join(
+                [
+                    f"\t{categorical_stats_title}",
+                    f"\t{'-' * len(categorical_stats_title)}",
+                    indent(f"{self._categorical_stats}\n", " " * 4),
+                ]
             )
         if hasattr(self, "_correlation_descriptions"):
             max_pairs = min(20, len(self._correlation_descriptions))
             top_20 = list(self._correlation_descriptions.items())[:max_pairs]
             corr_repr = "\n".join(
                 [
-                    f"{var_pair[0]} & {var_pair[1]} --> {corr_description}"
+                    f"{var_pair[0] + ' & ' + var_pair[1]:>32} -> "
+                    f"{corr_description}"
                     for var_pair, corr_description in top_20
                 ]
             )
-            correlation_description = (
-                f"\n\t  Pearson's Correlation (Top 20)"
-                "\n\t  ------------------------------\n"
-                f"{corr_repr}"
+            correlation_description = "\n".join(
+                [
+                    "\n\t\t\tPearson's Correlation (Top 20)",
+                    f"\t\t\t{'-' * 30}",
+                    f"{corr_repr}",
+                ]
             )
         else:
             correlation_description = ""
 
         return "\n".join(
             [
-                "\t\t\tOVERVIEW",
-                "\t\t\t========",
-                f"{numeric_info}",
-                f"{categorical_info}",
                 f"{numeric_stats}",
-                f"{categorical_stats}",
+                indent(f"{categorical_stats}", "\t"),
                 f"{correlation_description}",
+                "\t",
             ]
         )
 
     def _get_summary_statistics(self) -> None:
         """Compute descriptive statistics."""
-        numeric_data = _select_dtypes(self.data, "number")
-        if numeric_data is None:
+        data = self.data.copy()
+        numeric_data = data.select_dtypes("number")
+        # Consider numeric columns with < 11 unique values as categorical
+        categorical_with_numbers = [
+            col for col in numeric_data if numeric_data[col].nunique() < 11
+        ]
+        numeric_data = numeric_data.drop(columns=categorical_with_numbers)
+        if numeric_data.shape[1] < 1:
             self._numeric_stats = None
         else:
             numeric_stats = numeric_data.describe().T
+            numeric_stats["count"] = numeric_stats["count"].astype("int")
+            numeric_stats = numeric_stats.rename(
+                columns={"mean": "avg", "std": "stddev"}
+            )
             numeric_stats["skewness"] = numeric_data.skew(numeric_only=True)
             numeric_stats["kurtosis"] = numeric_data.kurt(numeric_only=True)
             self._numeric_stats = numeric_stats.round(4)
 
-        categorical_data = _select_dtypes(
-            self.data, "category", "object", "bool"
-        )
-        if categorical_data is None:
+        categorical_data = data.drop(columns=numeric_data.columns).copy()
+        if categorical_data.shape[1] < 1:
             self._categorical_stats = None
         else:
+            for col in categorical_data:
+                # Convert categorical columns with "unique ratio" < 0.3 to
+                # categorical dtype, reducing memory usage.
+                if (
+                    categorical_data[col].nunique() / len(categorical_data)
+                ) < 0.3:
+                    categorical_data[col] = categorical_data[col].astype(
+                        "category"
+                    )
+                else:
+                    categorical_data[col] = categorical_data[col].astype(
+                        "string"
+                    )
             categorical_stats = categorical_data.describe().T
             categorical_stats["relative freq"] = (
                 categorical_stats["freq"] / len(self.data)
             ).apply(lambda x: f"{x :.2%}")
             self._categorical_stats = categorical_stats
 
-    def _get_correlation_descriptions(self) -> None:
-        """Get brief descriptions of the nature of correlation between numeric
-        column pairs."""
-        self._correlation_descriptions = {
-            pair: _describe_correlation(corr_value)
-            for pair, corr_value in self._correlation_values
-        }
-
     def _get_bivariate_analysis(self) -> None:
         """Compare numeric column pairs."""
         self._correlation_values = _compute_correlation(self.data)
-
         if self._correlation_values is None:
             logging.warning(
                 "Skipped Bivariate Analysis: There are less than 2 numeric "
                 "variables."
             )
         else:
             self._get_correlation_descriptions()
+
+    def _get_correlation_descriptions(self) -> None:
+        """Get brief descriptions of the nature of correlation between numeric
+        column pairs."""
+        self._correlation_descriptions = {
+            pair: _describe_correlation(corr_value)
+            for pair, corr_value in self._correlation_values
+        }
```

### Comparing `eda_report-2.7.3/eda_report/plotting.py` & `eda_report-2.8.0/eda_report/plotting.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 from io import BytesIO
 from multiprocessing import Pool
 from typing import Dict, Iterable, Optional, Sequence, Tuple, Union
 
 import matplotlib as mpl
 import numpy as np
+from matplotlib.axes import Axes
 from matplotlib.colors import to_rgb
 from matplotlib.figure import Figure
 from scipy.stats import gaussian_kde, probplot
 from tqdm import tqdm
 
-from eda_report.multivariate import MultiVariable
-from eda_report.validate import (
-    validate_multivariate_input,
-    validate_univariate_input,
-)
+from eda_report._validate import _validate_dataset, _validate_univariate_input
+from eda_report.bivariate import Dataset
 
 # Matplotlib configuration
-mpl.rc("figure", autolayout=True, dpi=150, figsize=(6.5, 4))
-mpl.rc("font", family="serif")
-mpl.rc("axes.spines", top=False, right=False)
-mpl.rc("axes", titlesize=12, titleweight=500)
-mpl.use("agg")  # use non-interactive matplotlib back-end
-
-# Customize boxplots
-mpl.rc("boxplot", patchartist=True, vertical=False)
-mpl.rc("boxplot.medianprops", color="black")
+GENERAL_RC_PARAMS = {
+    "axes.spines.top": False,
+    "axes.spines.right": False,
+    "axes.titlesize": 12,
+    "axes.titleweight": 500,
+    "figure.autolayout": True,
+    "figure.figsize": (5.6, 3.5),
+    "font.family": "serif",
+    "savefig.dpi": 120,
+}
+# Customize box-plots
+BOXPLOT_RC_PARAMS = {
+    **GENERAL_RC_PARAMS,
+    "boxplot.medianprops.color": "black",
+    "boxplot.patchartist": True,
+    "boxplot.vertical": False,
+}
+# Customize correlation-plots
+CORRPLOT_RC_PARAMS = {**GENERAL_RC_PARAMS, "figure.figsize": (7, 6.3)}
+# Customize regression-plots
+REGPLOT_RC_PARAMS = {**GENERAL_RC_PARAMS, "figure.figsize": (5.2, 5)}
 
 
+@mpl.rc_context(GENERAL_RC_PARAMS)
 def _savefig(figure: Figure) -> BytesIO:
     """Saves the contents of a :class:`~matplotlib.figure.Figure` in PNG
     format, as bytes in a file-like object.
 
     This is a utility function helpful in by-passing the *filesystem*. Graphs
     are stored in :class:`~io.BytesIO` objects, and can then be read
     directly as *attributes*, thus allowing rapid in-memory access when
@@ -40,302 +51,308 @@
         figure (matplotlib.figure.Figure): Graph content.
 
     Returns:
         io.BytesIO: A graph in PNG format as bytes.
     """
     graph = BytesIO()
     figure.savefig(graph, format="png")
-
     return graph
 
 
+def _get_axes(ax: Axes = None) -> Axes:
+    """Validate or create an Axes instance.
+
+    Args:
+        ax (matplotlib.axes.Axes, optional): Axes instance. Defaults to None.
+
+    Raises:
+        TypeError: If `ax` is not an Axes instance.
+
+    Returns:
+        Axes: Axes instance.
+    """
+    if ax is None:
+        return Figure().subplots()
+    elif isinstance(ax, Axes):
+        return ax
+    else:
+        raise TypeError(f"Invalid input for 'ax': {type(ax)}")
+
+
 def _get_color_shades_of(color: str, num: int = None) -> Sequence:
-    """Obtain an array of `num` shades of the specified `color`.
+    """Obtain an array with `num` shades of the specified `color`.
 
     Args:
         color (str): The desired color.
         num (int): Desired number of color shades.
+
+    Returns:
+        Sequence: Array of RGB colors.
     """
     color_rgb = to_rgb(color)
     return np.linspace(color_rgb, (0.25, 0.25, 0.25), num=num)
 
 
+@mpl.rc_context(BOXPLOT_RC_PARAMS)
 def box_plot(
     data: Iterable,
     *,
     label: str,
     hue: Iterable = None,
     color: Union[str, Sequence] = None,
-) -> Figure:
+    ax: Axes = None,
+) -> Axes:
     """Get a box-plot from numeric values.
 
     Args:
         data (Iterable): Values to plot.
-        label (str): A name for the `data`, shown in the title.
-        hue (Iterable, optional): Values for grouping the `data`. Defaults to
+        label (str): A name for the ``data``, shown in the title.
+        hue (Iterable, optional): Values for grouping the ``data``. Defaults to
             None.
         color (Union[str, Sequence]): A valid matplotlib color specifier.
+        ax (matplotlib.axes.Axes, optional): Axes instance. Defaults to None.
 
     Returns:
-        matplotlib.figure.Figure: Matplotlib figure with the box-plot.
+        matplotlib.axes.Axes: Matplotlib axes with the box-plot.
     """
-    original_data = validate_univariate_input(data)
+    original_data = _validate_univariate_input(data)
     data = original_data.dropna()
-
-    fig = Figure()
-    ax = fig.subplots()
-
+    ax = _get_axes(ax)
     if hue is None:
         bxplot = ax.boxplot(
             data,
             labels=[label],
             sym=".",
             boxprops=dict(facecolor=color, alpha=0.75),
         )
         ax.set_yticklabels("")
     else:
-        hue = validate_univariate_input(hue)[original_data.notna()]
-        groups = {key: series for key, series in data.groupby(hue)}
+        hue = _validate_univariate_input(hue)[original_data.notna()]
+        groups = {key: sub_series for key, sub_series in data.groupby(hue)}
         bxplot = ax.boxplot(groups.values(), labels=groups.keys(), sym=".")
 
         if color is None:
             colors = [f"C{idx}" for idx in range(hue.nunique())]
         else:
             colors = _get_color_shades_of(color, hue.nunique())
 
         for patch, color in zip(bxplot["boxes"], reversed(colors)):
             patch.set_facecolor(color)
             patch.set_alpha(0.75)
 
-    ax.set_title(f"Box-plot of {label}")
+        if hue.name is not None:
+            ax.set_ylabel(f"{hue.name}".title())
 
-    return fig
+    ax.set_title(f"Box-plot of {label}")
+    return ax
 
 
+@mpl.rc_context(GENERAL_RC_PARAMS)
 def kde_plot(
     data: Iterable,
     *,
     label: str,
     hue: Iterable = None,
     color: Union[str, Sequence] = None,
-) -> Figure:
+    ax: Axes = None,
+) -> Axes:
     """Get a kde-plot from numeric values.
 
     Args:
         data (Iterable): Values to plot.
-        label (str): A name for the `data`, shown in the title.
-        hue (Iterable, optional): Values for grouping the `data`. Defaults to
+        label (str): A name for the ``data``, shown in the title.
+        hue (Iterable, optional): Values for grouping the ``data``. Defaults to
             None.
         color (Union[str, Sequence]): A valid matplotlib color specifier.
+        ax (matplotlib.axes.Axes, optional): Axes instance. Defaults to None.
 
     Returns:
-        matplotlib.figure.Figure: Matplotlib figure with the kde-plot.
+        matplotlib.axes.Axes: Matplotlib axes with the kde-plot.
     """
-    original_data = validate_univariate_input(data)
+    original_data = _validate_univariate_input(data)
     data = original_data.dropna()
-
-    fig = Figure()
-    ax = fig.subplots()
-
+    ax = _get_axes(ax)
     if len(data) < 2 or np.isclose(data.std(), 0):
-        ax.text(
-            x=0.08,
-            y=0.45,
-            s=(
-                "[Could not plot kernel density estimate.\n "
-                "Data is singular.]"
-            ),
-            color="#f72",
-            size=14,
-            weight=600,
-        )
-        return fig
+        msg = "[Could not plot kernel density estimate.\n Data is singular.]"
+        ax.text(x=0.08, y=0.45, s=msg, color="#f72", size=14, weight=600)
+        return ax
 
     eval_points = np.linspace(data.min(), data.max(), num=len(data))
     if hue is None:
         kernel = gaussian_kde(data)
         density = kernel(eval_points)
         ax.plot(eval_points, density, label=label, color=color)
         ax.fill_between(eval_points, density, alpha=0.3, color=color)
     else:
-        hue = validate_univariate_input(hue)[original_data.notna()]
+        hue = _validate_univariate_input(hue)[original_data.notna()]
         if color is None:
             colors = [f"C{idx}" for idx in range(hue.nunique())]
         else:
             colors = _get_color_shades_of(color, hue.nunique())
 
         for color, (key, series) in zip(colors, data.groupby(hue)):
             kernel = gaussian_kde(series)
             density = kernel(eval_points)
             ax.plot(eval_points, density, label=key, alpha=0.75, color=color)
             ax.fill_between(eval_points, density, alpha=0.25, color=color)
 
+        if hue.name is not None:
+            ax.legend(title=f"{hue.name}".title())
+
+    ax.set_xlabel(label)
     ax.set_ylim(0)
-    ax.legend()
     ax.set_title(f"Density plot of {label}")
-
-    return fig
+    return ax
 
 
+@mpl.rc_context(REGPLOT_RC_PARAMS)
 def prob_plot(
     data: Iterable,
     *,
     label: str,
     marker_color: Union[str, Sequence] = "C0",
     line_color: Union[str, Sequence] = "#222",
-) -> Figure:
+    ax: Axes = None,
+) -> Axes:
     """Get a probability-plot from numeric values.
 
     Args:
         data (Iterable): Values to plot.
-        label (str): A name for the `data`, shown in the title.
+        label (str): A name for the ``data``, shown in the title.
         marker_color (Union[str, Sequence]): Color for the plotted points.
             Defaults to "C0".
         line_color (Union[str, Sequence]): Color for the line of best fit.
             Defaults to "#222".
+        ax (matplotlib.axes.Axes, optional): Axes instance. Defaults to None.
 
     Returns:
-        matplotlib.figure.Figure: Matplotlib figure with the probability-plot.
+        matplotlib.axes.Axes: Matplotlib axes with the probability-plot.
     """
-    original_data = validate_univariate_input(data)
+    original_data = _validate_univariate_input(data)
     data = original_data.dropna()
-
-    fig = Figure(figsize=(6.5, 4.5))
-    ax = fig.subplots()
+    ax = _get_axes(ax)
     probplot(data, fit=True, plot=ax)
     ax.lines[0].set_color(marker_color)
     ax.lines[1].set_color(line_color)
+    ax.set_xlabel("Theoretical Quantiles (Normal)")
     ax.set_title(f"Probability plot of {label}")
-
-    return fig
+    return ax
 
 
+@mpl.rc_context(GENERAL_RC_PARAMS)
 def bar_plot(
-    data: Iterable, *, label: str, color: Union[str, Sequence] = None
-) -> Figure:
+    data: Iterable,
+    *,
+    label: str,
+    color: Union[str, Sequence] = None,
+    ax: Axes = None,
+) -> Axes:
     """Get a bar-plot from a sequence of values.
 
     Args:
         data (Iterable): Values to plot.
-        label (str): A name for the `data`, shown in the title.
+        label (str): A name for the ``data``, shown in the title.
         color (Union[str, Sequence]): A valid matplotlib color specifier.
+        ax (matplotlib.axes.Axes, optional): Axes instance. Defaults to None.
 
     Returns:
-        matplotlib.figure.Figure: Matplotlib figure with the bar-plot.
+        matplotlib.axes.Axes: Matplotlib axes with the bar-plot.
     """
-    original_data = validate_univariate_input(data)
+    original_data = _validate_univariate_input(data)
     data = original_data.dropna()
-
-    fig = Figure()
-    ax = fig.subplots()
-
+    ax = _get_axes(ax)
     # Include no more than 10 of the most common values
     top_10 = data.value_counts().nlargest(10)
     bars = ax.bar(top_10.index.map(str), top_10, alpha=0.8, color=color)
     ax.bar_label(bars, labels=[f"{x:,.0f}" for x in top_10], padding=2)
-
     if (num_unique := data.nunique()) > 10:
         title = f"Bar-plot of {label} (Top 10 of {num_unique})"
     else:
         title = f"Bar-plot of {label}"
     ax.set_title(title)
-    ax.tick_params(axis="x", rotation=90)  # Improve visibility of long labels
-
-    return fig
+    ax.set_ylabel("Count")
+    ax.tick_params(axis="x", rotation=90)  # Improve visibility for long labels
+    return ax
 
 
-def _plot_variable(variables_hue_and_color: Tuple) -> Tuple:
+def _plot_variable(variable_data_hue_and_color: Tuple) -> Tuple:
     """Helper function to concurrently plot variables in a multiprocessing
     Pool.
 
     Args:
-        variables_hue_and_color (Tuple): A variable, hue data and the desired
-            theme.
+        variable_data_hue_and_color (Tuple): A variable, plot data, hue data
+            and the desired plot color.
 
     Returns:
         Tuple: `variable`s name, and graphs in a dict.
     """
-    variable, hue, color = variables_hue_and_color
+    variable, data, hue, color = variable_data_hue_and_color
     if variable.var_type == "numeric":
-        graphs = {
-            "box_plot": _savefig(
-                box_plot(
-                    data=variable.data,
-                    hue=hue,
-                    label=variable.name,
-                    color=color,
-                )
+        plots = {
+            "box_plot": box_plot(
+                data=data, hue=hue, label=variable.name, color=color
             ),
-            "kde_plot": _savefig(
-                kde_plot(
-                    data=variable.data,
-                    hue=hue,
-                    label=variable.name,
-                    color=color,
-                )
+            "kde_plot": kde_plot(
+                data=data, hue=hue, label=variable.name, color=color
             ),
-            "prob_plot": _savefig(
-                prob_plot(
-                    data=variable.data, label=variable.name, marker_color=color
-                )
+            "prob_plot": prob_plot(
+                data, label=variable.name, marker_color=color
             ),
         }
-    else:  # {"boolean", "categorical", "datetime"}:
-        graphs = {
-            "bar_plot": _savefig(
-                bar_plot(data=variable.data, label=variable.name, color=color)
-            )
-        }
+    else:  # {"boolean", "categorical", "datetime", "numeric (<=10 levels)"}
+        plots = {"bar_plot": bar_plot(data, label=variable.name, color=color)}
 
-    return variable.name, graphs
+    graph_images = {name: _savefig(ax.figure) for name, ax in plots.items()}
+    return variable.name, graph_images
 
 
+@mpl.rc_context(CORRPLOT_RC_PARAMS)
 def plot_correlation(
     variables: Iterable,
     max_pairs: int = 20,
     color_pos: Union[str, Sequence] = "orangered",
     color_neg: Union[str, Sequence] = "steelblue",
-) -> Figure:
+    ax: Axes = None,
+) -> Axes:
     """Create a bar chart showing the top ``max_pairs`` most correlated
-    variables.
+    variables. Bars are annotated with variable pairs and their respective
+    Pearson correlation coefficients.
 
     Args:
-        variables (Iterable): 2-dimensional data.
+        variables (Iterable): 2-dimensional numeric data.
         max_pairs (int): The maximum number of numeric pairs to include in the
             plot. Defaults to 20.
         color_pos (Union[str, Sequence]): Color for positive correlation bars.
             Defaults to "orangered".
         color_neg (Union[str, Sequence]): Color for negative correlation bars.
             Defaults to "steelblue".
+        ax (matplotlib.axes.Axes, optional): Axes instance. Defaults to None.
 
     Returns:
-        matplotlib.figure.Figure: A bar-plot of correlation data.
+        matplotlib.axes.Axes: A bar-plot of correlation data.
     """
-    if not isinstance(variables, MultiVariable):
-        variables = MultiVariable(variables)
+    if not isinstance(variables, Dataset):
+        variables = Dataset(variables)
 
     if variables._correlation_values is None:
         return None
 
     # Show at most `max_pairs` numeric pairs.
     pairs_to_show = variables._correlation_values[:max_pairs]
     # Reverse items so largest values appear at the top.
     corr_data = dict(reversed(pairs_to_show))
     labels = [" vs ".join(pair) for pair in corr_data.keys()]
-
-    fig = Figure(figsize=(7, 6.3))
-    ax = fig.subplots()
+    ax = _get_axes(ax)
     ax.barh(labels, corr_data.values(), edgecolor="#222", linewidth=0.5)
     ax.set_xlim(-1.1, 1.1)
-    ax.spines["left"].set_position("zero")
-    ax.yaxis.set_visible(False)  # hide y-axis labels
+    ax.spines["left"].set_position("zero")  # Place y-axis spine at x=0
+    ax.yaxis.set_visible(False)  # Hide y-axis labels
 
     for p, label in zip(ax.patches, labels):
         p.set_alpha(min(1, abs(p.get_width()) + 0.1))
-
         if p.get_width() < 0:
             p.set_facecolor(color_neg)
             ax.text(
                 p.get_x(),
                 p.get_y() + p.get_height() / 2,
                 f"{p.get_width():,.2f} ({label})  ",
                 size=8,
@@ -350,123 +367,122 @@
                 f"  {p.get_width():,.2}  ({label})",
                 size=8,
                 ha="left",
                 va="center",
             )
 
     ax.set_title(f"Pearson Correlation (Top {len(corr_data)})")
-
-    return fig
+    return ax
 
 
+@mpl.rc_context(REGPLOT_RC_PARAMS)
 def regression_plot(
     x: Iterable,
     y: Iterable,
     labels: Tuple[str, str],
-    color: Union[str, Sequence] = None,
-) -> Figure:
+    marker_color: Union[str, Sequence] = "C0",
+    line_color: Union[str, Sequence] = "#444",
+    ax: Axes = None,
+) -> Axes:
     """Get a regression-plot from the provided pair of values.
 
     Args:
         x (Iterable): Numeric values.
         y (Iterable): Numeric values.
         labels (Tuple[str, str]): Names for `x` and `y` respectively, shown in
             axis labels.
-        color (Union[str, Sequence]): A valid matplotlib color specifier.
+        marker_color (Union[str, Sequence]): Color for the plotted points.
+            Defaults to "C0".
+        line_color (Union[str, Sequence]): Color for the line of best fit.
+            Defaults to "#444".
+        ax (matplotlib.axes.Axes, optional): Axes instance. Defaults to None.
 
     Returns:
-        matplotlib.figure.Figure: Matplotlib figure with the regression-plot.
+        matplotlib.axes.Axes: Matplotlib axes with the regression-plot.
     """
     var1, var2 = labels
-    # Convert to DataFrame
-    data = validate_multivariate_input({var1: x, var2: y}).dropna()
-
+    data = _validate_dataset({var1: x, var2: y}).dropna()
     if len(data) > 50000:
         data = data.sample(50000)
 
-    fig = Figure(figsize=(5, 5))
-    ax = fig.subplots()
+    ax = _get_axes(ax)
     x = data[var1]
     y = data[var2]
     slope, intercept = np.polyfit(x, y, deg=1)
-    line_x = np.linspace(x.min(), x.max(), num=100)
-
-    ax.scatter(x, y, s=40, alpha=0.7, color=color, edgecolors="#444")
-    ax.plot(line_x, slope * line_x + intercept, color="#444", lw=2)
+    ax.scatter(x, y, s=40, alpha=0.7, color=marker_color, edgecolors="#444")
+    reg_line_x = np.linspace(x.min(), x.max(), num=100)
+    reg_line_y = slope * reg_line_x + intercept
+    ax.plot(reg_line_x, reg_line_y, color=line_color, lw=2)
     ax.set_title(
         f"Slope: {slope:,.4f}\nIntercept: {intercept:,.4f}\n"
         + f"Correlation: {x.corr(y):.4f}",
         size=11,
     )
     ax.set_xlabel(var1)
     ax.set_ylabel(var2)
-
-    return fig
+    return ax
 
 
 def _plot_regression(data_and_color: Tuple) -> Tuple:
-    """Helper function to plot regression plots concurrently.
+    """Helper function to plot regression-plots concurrently.
 
     Args:
-        data_and_color (Tuple): A pair of numeric values.
+        data_and_color (Tuple): Dataframe, and desired marker-color.
 
     Returns:
-        Tuple: Names for the pair of values, and a figure with the regression
+        Tuple: Names for the variable pair, and axes with the regression
         plot.
     """
     data, color = data_and_color
     var1, var2 = data.columns
-    fig = regression_plot(
-        x=data[var1], y=data[var2], labels=(var1, var2), color=color
+    ax = regression_plot(
+        x=data[var1], y=data[var2], labels=(var1, var2), marker_color=color
     )
-    return (var1, var2), fig
+    return (var1, var2), ax
 
 
-def _plot_multivariable(
-    variables: MultiVariable, color: str = None
-) -> Optional[Dict]:
-    """Concurrently plot regression plots in a multiprocessing Pool.
+def _plot_dataset(variables: Dataset, color: str = None) -> Optional[Dict]:
+    """Concurrently plot regression-plots in a multiprocessing Pool.
 
     Args:
-        variables (MultiVariable): Bi-variate analysis results.
+        variables (Dataset): Bi-variate analysis results.
         color (str, optional): The color to apply to the graphs.
 
     Returns:
         Optional[Dict]: A dictionary with a correlation plot and regression
         plots.
     """
     if variables._correlation_values is None:
         return None
     else:
         # Take the top 20 pairs by magnitude of correlation.
-        # 20 var_pairs ≈ 10+ pages
+        # 20 var_pairs ≈ 10+ pages in report document
         # 20 numeric columns == 190 var_pairs ≈ 95+ pages.
         pairs_to_include = [
             pair for pair, _ in variables._correlation_values[:20]
         ]
         with Pool() as p:
-            paired_data_gen = [
+            paired_data = [
                 (variables.data.loc[:, pair], color)
                 for pair in pairs_to_include
             ]
             bivariate_regression_plots = dict(
                 tqdm(
                     # Plot in parallel processes
-                    p.imap(_plot_regression, paired_data_gen),
+                    p.imap(_plot_regression, paired_data),
                     # Progress-bar options
                     total=len(pairs_to_include),
                     bar_format=(
                         "{desc} {percentage:3.0f}%|{bar:35}| "
                         "{n_fmt}/{total_fmt} pairs."
                     ),
                     desc="Bivariate analysis:",
                     dynamic_ncols=True,
                 )
             )
-
         return {
-            "correlation_plot": _savefig(plot_correlation(variables)),
+            "correlation_plot": _savefig(plot_correlation(variables).figure),
             "regression_plots": {
-                var_pair: _savefig(plot)
+                var_pair: _savefig(plot.figure)
                 for var_pair, plot in bivariate_regression_plots.items()
             },
         }
```

### Comparing `eda_report-2.7.3/eda_report/read_file.py` & `eda_report-2.8.0/eda_report/_read_file.py`

 * *Files identical despite different names*

### Comparing `eda_report-2.7.3/eda_report/validate.py` & `eda_report-2.8.0/eda_report/_validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from eda_report.exceptions import (
     EmptyDataError,
     GroupbyVariableError,
     InputError,
 )
 
 
-def clean_column_labels(data: DataFrame) -> DataFrame:
+def _clean_column_labels(data: DataFrame) -> DataFrame:
     """Makes sure that columns have *meaningful* names.
 
     When creating a ``DataFrame`` from an ``Iterable``, if no column names
     are provided, the columns are set as a :class:`~pandas.RangeIndex` —
     [0, 1, 2, ...] (default).
 
     This function renames such columns to ['var_1', 'var_2, 'var_3', ...],
@@ -25,28 +25,27 @@
     It also ensures that column labels are all of similar type (``str``) to
     allow sorting and the use of string methods.
 
     Args:
         data (pandas.DataFrame): Data to inspect and perhaps edit.
 
     Returns:
-        pandas.DataFrame: The ``data``, with reader-friendly column
+        pandas.DataFrame: The ``data``, with human-friendly column
         names.
     """
     if isinstance(data.columns, RangeIndex):
         data.columns = [f"var_{i+1}" for i in data.columns]
     elif is_numeric_dtype(data.columns):
         data.columns = [f"var_{i}" for i in data.columns]
-        return data
     else:
         data.columns = data.columns.map(str)
     return data
 
 
-def check_cardinality(groupby_data: Series, *, threshold: int = 10) -> None:
+def _check_cardinality(groupby_data: Series, *, threshold: int = 10) -> None:
     """Assesses whether the ``groupby_data`` has too many unique values
     (> ``threshold``, default 10).
 
     Args:
         groupby_data (pandas.Series): The data intended to group values.
         threshold (int, optional): Maximum allowable cardinality. Defaults to
             10.
@@ -61,17 +60,16 @@
             f"values. It has high cardinality ({groupby_data.nunique()}) "
             f"and would clutter graphs."
         )
         logging.warning(message)
         raise GroupbyVariableError(message)
 
 
-def validate_multivariate_input(data: Iterable) -> DataFrame:
-    """Ensures that *multivariate input data* is of type
-    :class:`pandas.DataFrame`.
+def _validate_dataset(data: Iterable) -> DataFrame:
+    """Ensures that input data is of type :class:`pandas.DataFrame`.
 
     If it isn't, this attempts to explicitly cast it as a ``DataFrame``.
 
     Columns in the data that are completely empty will be dropped.
 
     Args:
         data (Iterable): The data to analyze.
@@ -96,18 +94,18 @@
 
     data_frame = (
         # Attempt to infer better dtypes for columns.
         data_frame.infer_objects()
         # Drop completely empty columns.
         .dropna(axis=1, how="all")
     )
-    return clean_column_labels(data_frame)
+    return _clean_column_labels(data_frame)
 
 
-def validate_univariate_input(
+def _validate_univariate_input(
     data: Iterable, *, name: str = None
 ) -> Optional[Series]:
     """Ensures that *univariate input data* is of type :class:`pandas.Series`.
 
     If it isn't, this attempts to explicitly cast it as a ``Series``.
 
     Args:
@@ -134,53 +132,53 @@
             )
     if series.shape[0] == 0:
         raise EmptyDataError("No data to process.")
     else:
         return series
 
 
-def validate_groupby_data(
-    *, data: DataFrame, groupby_data: Union[int, str]
+def _validate_groupby_variable(
+    *, data: DataFrame, groupby_variable: Union[int, str]
 ) -> Optional[Series]:
     """Ensures that the specified column label/index for grouping values is
     present in the data.
 
     Args:
         data (DataFrame): The data being analyzed.
-        groupby_data (Union[int, str]): A column label or index.
+        groupby_variable (Union[int, str]): A column label or index.
 
     Raises:
         GroupbyVariableError: If the supplied column label does not exist, or
             the supplied column index is out of bounds.
 
     Returns:
         Optional[pandas.Series]: The groupby variable's data.
     """
-    if groupby_data is None:
+    if groupby_variable is None:
         return None
-    elif f"{groupby_data}".isdecimal():
-        idx = int(groupby_data)
+    elif f"{groupby_variable}".isdecimal():
+        idx = int(groupby_variable)
         try:
             groupby_data = data.iloc[:, idx]
         except IndexError:
             raise GroupbyVariableError(
-                f"Column index {groupby_data} is not in the range"
+                f"Column index {groupby_variable} is not in the range"
                 f" [0, {data.columns.size}]."
             )
-        check_cardinality(groupby_data)
+        _check_cardinality(groupby_data)
         return groupby_data
-    elif isinstance(groupby_data, str):
+    elif isinstance(groupby_variable, str):
         try:
-            groupby_data = data[groupby_data]
+            groupby_data = data[groupby_variable]
         except KeyError:
             raise GroupbyVariableError(
-                f"{groupby_data!r} is not in {data.columns.to_list()}"
+                f"{groupby_variable!r} is not in {data.columns.to_list()}"
             )
-        check_cardinality(groupby_data)
+        _check_cardinality(groupby_data)
         return groupby_data
     else:
         # If groupby_data is neither an index(int) or label(str)
         logging.warning(
-            f"Group-by variable '{groupby_data}' ignored."
+            f"Group-by variable '{groupby_variable}' ignored."
             " Not a valid column index or label."
         )
         return None
```

### Comparing `eda_report-2.7.3/setup.cfg` & `eda_report-2.8.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -17,32 +17,32 @@
 	Programming Language :: Python :: 3.8
 project_urls = 
 	Source Code = https://github.com/Tim-Abwao/eda-report
 
 [options]
 packages = find:
 install_requires = 
-	matplotlib>=3.6.0
-	openpyxl>=3.0.10
-	pandas>=1.5.0
+	matplotlib>=3.7.0
+	openpyxl>=3.1.2
+	pandas>=2.0.0
 	python-docx>=0.8.11
-	scipy>=1.9.1
-	tqdm>=4.64.1
+	scipy>=1.10.1
+	tqdm>=4.65.0
 include_package_data = True
 python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
-	eda-report = eda_report.cli:run_from_cli
+	eda-report = eda_report._cli:run_from_cli
 
 [options.extras_require]
 dev = 
-	black>=22.8.0
-	coverage>=6.5.0
-	flake8>=5.0.4
+	black>=23.3.0
+	coverage>=7.2.3
+	flake8>=6.0.0
 
 [options.package_data]
 eda_report = */*.png
 
 [options.packages.find]
 exclude = tests, tests.*
```

