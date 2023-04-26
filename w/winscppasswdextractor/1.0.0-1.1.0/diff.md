# Comparing `tmp/winscppasswdextractor-1.0.0.tar.gz` & `tmp/winscppasswdextractor-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winscppasswdextractor-1.0.0.tar", max compression
+gzip compressed data, was "winscppasswdextractor-1.1.0.tar", max compression
```

## Comparing `winscppasswdextractor-1.0.0.tar` & `winscppasswdextractor-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      900 2023-03-30 14:51:48.354102 winscppasswdextractor-1.0.0/README.md
--rw-r--r--   0        0        0     6219 2023-03-30 15:47:05.638171 winscppasswdextractor-1.0.0/WinSCPPasswdExtractor/WinSCPPasswdExtractor.py
--rw-r--r--   0        0        0      525 2023-03-30 15:49:09.866173 winscppasswdextractor-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1695 1970-01-01 00:00:00.000000 winscppasswdextractor-1.0.0/setup.py
--rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 winscppasswdextractor-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1685 2023-04-25 09:52:01.446000 winscppasswdextractor-1.1.0/README.md
+-rw-r--r--   0        0        0     8186 2023-04-25 12:21:08.307000 winscppasswdextractor-1.1.0/WinSCPPasswdExtractor/WinSCPPasswdExtractor.py
+-rw-r--r--   0        0        0      524 2023-04-25 12:13:16.866000 winscppasswdextractor-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2322 1970-01-01 00:00:00.000000 winscppasswdextractor-1.1.0/PKG-INFO
```

### Comparing `winscppasswdextractor-1.0.0/pyproject.toml` & `winscppasswdextractor-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "WinSCPPasswdExtractor"
-version = "1.0.0"
+version = "1.1.0"
 description = "Extract WinSCP Credentials from any Windows System or winscp config file"
 authors = ["Alexander Neff <alex99.neff@gmx.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "WinSCPPasswdExtractor" },
 ]
 
 [tool.poetry.scripts]
 WinSCPPasswdExtractor = "WinSCPPasswdExtractor.WinSCPPasswdExtractor:run"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.7"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `winscppasswdextractor-1.0.0/PKG-INFO` & `winscppasswdextractor-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-Metadata-Version: 2.1
-Name: winscppasswdextractor
-Version: 1.0.0
-Summary: Extract WinSCP Credentials from any Windows System or winscp config file
-License: MIT
-Author: Alexander Neff
-Author-email: alex99.neff@gmx.de
-Requires-Python: >=3.11,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
 # WinSCP Password Extractor
-WinSCP stores ssh session passwords in an encoded format in either the registry or a file called WinSCP.ini.
-This python script searches in the winscp default locations to extract stored credentials.
+WinSCP stores ssh session passwords in an encoded format in either the registry or a config file called WinSCP.ini.
+
+This python script searches in the WinSCP default locations to extract stored credentials for the current user, when executed locally on the target. If a WinSCP.ini config file is already present the script can decode stored credentials as seen below. To gather WinSCP credentials from a remote target or a range of targets there is a module present for the pentesting Tool [CrackMapExec](https://github.com/Porchetta-Industries/CrackMapExec) called "winscp_dump".
 
-These default file locations are:
+These default locations are:
+- registry
 - %APPDATA%\WinSCP.ini
 - %USER%\Documents\WinSCP.ini
 
+## Installation
+WinSCPPasswdExtractor is available on pypi.org. Therefore it is recommended to install this tool with pipx:
+```python3
+pipx install WinSCPPasswdExtractor
+```
+Alternatively you could install it with pip or simply download the file and run it.
+
 ## Usage
 You can either specify a file path if you know the exact path to an existing WinSCP.ini file or you let the tool itself look if any credentials are stored in the default locations.
+
+With pipx:
 ```python3
-python WinSCPPwdDump.py
-python WinSCPPwdDump.py <path-to-file>
+WinSCPPasswdExtractor
+WinSCPPasswdExtractor <path-to-winscp-file>
+```
+
+Manually downloaded:
+```python3
+python WinSCPPasswdExtractor.py
+python WinSCPPasswdExtractor.py <path-to-winscp-file>
 ```
 
 ## About
 This Tool is based on the work of [winscppasswd](https://github.com/anoopengineer/winscppasswd), the ruby winscp parser from [Metasploit-Framework](https://github.com/rapid7/metasploit-framework) and the awesome work from [winscppassword](https://github.com/dzxs/winscppassword).
 
 They did the hard stuff
-
```

