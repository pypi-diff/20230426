# Comparing `tmp/matrix_package-22.3.12.tar.gz` & `tmp/matrix_package-23.4.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrix_package-22.3.12.tar", last modified: Thu Mar 10 10:28:16 2022, max compression
+gzip compressed data, was "matrix_package-23.4.29.tar", last modified: Tue Apr 25 16:08:18 2023, max compression
```

## Comparing `matrix_package-22.3.12.tar` & `matrix_package-23.4.29.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-03-10 10:28:16.000000 matrix_package-22.3.12/
--rw-rw-rw-   0        0        0     1073 2022-02-09 11:02:44.000000 matrix_package-22.3.12/LICENCE
--rw-rw-rw-   0        0        0     1272 2022-03-10 10:28:18.000000 matrix_package-22.3.12/PKG-INFO
--rw-rw-rw-   0        0        0      132 2022-02-09 11:02:44.000000 matrix_package-22.3.12/README.md
--rw-rw-rw-   0        0        0      834 2022-02-09 11:02:44.000000 matrix_package-22.3.12/README.txt
-drwxrwxrwx   0        0        0        0 2022-03-10 10:28:16.000000 matrix_package-22.3.12/matrix_package/
--rw-rw-rw-   0        0        0    19382 2022-02-09 11:02:42.000000 matrix_package-22.3.12/matrix_package/Structure_Factor.py
--rw-rw-rw-   0        0        0        0 2022-02-09 11:02:40.000000 matrix_package-22.3.12/matrix_package/__init__.py
--rw-rw-rw-   0        0        0     5543 2022-02-09 11:02:40.000000 matrix_package-22.3.12/matrix_package/bin.py
--rw-rw-rw-   0        0        0    40479 2022-02-09 11:02:40.000000 matrix_package-22.3.12/matrix_package/com.py
--rw-rw-rw-   0        0        0    83898 2022-03-10 09:21:00.000000 matrix_package-22.3.12/matrix_package/control.py
--rw-rw-rw-   0        0        0     6276 2022-02-09 11:02:42.000000 matrix_package-22.3.12/matrix_package/coordinates_transform.py
--rw-rw-rw-   0        0        0    38091 2022-02-09 11:02:42.000000 matrix_package-22.3.12/matrix_package/density.py
--rw-rw-rw-   0        0        0    34852 2022-02-09 11:02:42.000000 matrix_package-22.3.12/matrix_package/density_test.py
--rw-rw-rw-   0        0        0    26620 2022-02-09 11:02:42.000000 matrix_package-22.3.12/matrix_package/gdr.py
--rw-rw-rw-   0        0        0    12433 2022-02-09 11:02:42.000000 matrix_package-22.3.12/matrix_package/get_file.py
--rw-rw-rw-   0        0        0    11077 2022-02-09 11:02:42.000000 matrix_package-22.3.12/matrix_package/molecule.py
--rw-rw-rw-   0        0        0    23753 2022-02-09 11:02:40.000000 matrix_package-22.3.12/matrix_package/params.py
--rw-rw-rw-   0        0        0     6558 2022-02-09 11:02:42.000000 matrix_package-22.3.12/matrix_package/pbc.py
--rw-rw-rw-   0        0        0     1957 2022-02-09 11:02:42.000000 matrix_package-22.3.12/matrix_package/periodic_bc.py
--rw-rw-rw-   0        0        0    21167 2022-02-09 11:02:40.000000 matrix_package-22.3.12/matrix_package/scale.py
-drwxrwxrwx   0        0        0        0 2022-03-10 10:28:16.000000 matrix_package-22.3.12/matrix_package.egg-info/
--rw-rw-rw-   0        0        0     1272 2022-03-10 10:28:14.000000 matrix_package-22.3.12/matrix_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      684 2022-03-10 10:28:16.000000 matrix_package-22.3.12/matrix_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-10 10:28:16.000000 matrix_package-22.3.12/matrix_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2022-02-09 11:02:44.000000 matrix_package-22.3.12/matrix_package.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2022-03-10 10:28:16.000000 matrix_package-22.3.12/matrix_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-03-10 10:28:16.000000 matrix_package-22.3.12/matrix_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2022-02-09 11:02:42.000000 matrix_package-22.3.12/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-03-10 10:28:18.000000 matrix_package-22.3.12/setup.cfg
--rw-rw-rw-   0        0        0      938 2022-03-10 10:19:16.000000 matrix_package-22.3.12/setup.py
+drwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)        0 2023-04-25 16:08:18.134786 matrix_package-23.4.29/
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)     1073 2021-12-08 12:05:16.000000 matrix_package-23.4.29/LICENCE
+-rw-r--r--   0 amiehe   (276822563) groupead-externes (276821974)     1252 2023-04-25 16:08:18.134786 matrix_package-23.4.29/PKG-INFO
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)      132 2021-12-08 12:05:16.000000 matrix_package-23.4.29/README.md
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)      834 2022-02-09 10:46:52.000000 matrix_package-23.4.29/README.txt
+drwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)        0 2023-04-25 16:08:18.134786 matrix_package-23.4.29/matrix_package/
+-rwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)    19382 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/Structure_Factor.py
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)        0 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/__init__.py
+-rwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)     5543 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/bin.py
+-rwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)    40479 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/com.py
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)    83898 2022-03-10 09:53:20.000000 matrix_package-23.4.29/matrix_package/control.py
+-rwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)     6276 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/coordinates_transform.py
+-rwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)    38091 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/density.py
+-rwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)    34852 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/density_test.py
+-rwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)    26620 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/gdr.py
+-rw-r--r--   0 amiehe   (276822563) groupead-externes (276821974)    12433 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/get_file.py
+-rwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)    11077 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/molecule.py
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)    23753 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/params.py
+-rwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)     6558 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/pbc.py
+-rwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)     1957 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/periodic_bc.py
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)    21167 2022-02-09 10:41:46.000000 matrix_package-23.4.29/matrix_package/scale.py
+drwxr-xr-x   0 amiehe   (276822563) groupead-externes (276821974)        0 2023-04-25 16:08:18.134786 matrix_package-23.4.29/matrix_package.egg-info/
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)     1252 2023-04-25 16:08:18.000000 matrix_package-23.4.29/matrix_package.egg-info/PKG-INFO
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)      684 2023-04-25 16:08:18.000000 matrix_package-23.4.29/matrix_package.egg-info/SOURCES.txt
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)        1 2023-04-25 16:08:18.000000 matrix_package-23.4.29/matrix_package.egg-info/dependency_links.txt
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)        1 2021-12-08 12:05:16.000000 matrix_package-23.4.29/matrix_package.egg-info/not-zip-safe
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)        9 2023-04-25 16:08:18.000000 matrix_package-23.4.29/matrix_package.egg-info/requires.txt
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)       15 2023-04-25 16:08:18.000000 matrix_package-23.4.29/matrix_package.egg-info/top_level.txt
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)        0 2021-12-08 12:05:16.000000 matrix_package-23.4.29/pyproject.toml
+-rw-r--r--   0 amiehe   (276822563) groupead-externes (276821974)       38 2023-04-25 16:08:18.138786 matrix_package-23.4.29/setup.cfg
+-rwxrwxrwx   0 amiehe   (276822563) groupead-externes (276821974)      938 2023-04-25 16:06:29.000000 matrix_package-23.4.29/setup.py
```

### Comparing `matrix_package-22.3.12/LICENCE` & `matrix_package-23.4.29/LICENCE`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/PKG-INFO` & `matrix_package-23.4.29/matrix_package.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: matrix_package
-Version: 22.3.12
-Summary: Molecular dynamics code for the analysis of structural, dynamic, thermodynamic and electronic properties of certain 2D materials.
-Home-page: https://github.com/amieheessomba
-Author: Iréné Amiehe-Essomba 
-Author-email: ibamieheessomba@unistra.fr
-License: IPCMS
-Keywords: molecular dynamics matrix package
-Platform: UNKNOWN
-License-File: LICENCE
-
-matrix_package is a molecular dynamics analysis code allowing to calculate several structural, dynamic, thermodynamic properties of amorphous, crystalline or semi-amorphous and electronic systems of certain 2D layered materials of Van Der Waals.
-It is based on powerful solving algorithms, using MACHINE LEARNING to solve certain more or less complex problems such as the computation of the properties of dipole moments from Wanier centers.
-version 22.02.09-alpha offers the possibility of processing six different inputs.
-LAMMPS outputs, DL_POLY outputs, CPMD outputs, GAMESS outputs, Abinit outputs and VASP outputs.
-this version will evolve gradually and will take into account more versions of inputs.
-However, it has a module that allows you to convert an input into an XYZ file that it can then use to do several calculations. 
-
-
+Metadata-Version: 2.1
+Name: matrix-package
+Version: 23.4.29
+Summary: Molecular dynamics code for the analysis of structural, dynamic, thermodynamic and electronic properties of certain 2D materials.
+Home-page: https://github.com/amieheessomba
+Author: Iréné Amiehe-Essomba 
+Author-email: ibamieheessomba@unistra.fr
+License: IPCMS
+Keywords: molecular dynamics matrix package
+Platform: UNKNOWN
+License-File: LICENCE
+
+matrix_package is a molecular dynamics analysis code allowing to calculate several structural, dynamic, thermodynamic properties of amorphous, crystalline or semi-amorphous and electronic systems of certain 2D layered materials of Van Der Waals.
+It is based on powerful solving algorithms, using MACHINE LEARNING to solve certain more or less complex problems such as the computation of the properties of dipole moments from Wanier centers.
+version 22.02.09-alpha offers the possibility of processing six different inputs.
+LAMMPS outputs, DL_POLY outputs, CPMD outputs, GAMESS outputs, Abinit outputs and VASP outputs.
+this version will evolve gradually and will take into account more versions of inputs.
+However, it has a module that allows you to convert an input into an XYZ file that it can then use to do several calculations. 
+
+
```

### Comparing `matrix_package-22.3.12/README.txt` & `matrix_package-23.4.29/README.txt`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/Structure_Factor.py` & `matrix_package-23.4.29/matrix_package/Structure_Factor.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/bin.py` & `matrix_package-23.4.29/matrix_package/bin.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/com.py` & `matrix_package-23.4.29/matrix_package/com.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/control.py` & `matrix_package-23.4.29/matrix_package/control.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/coordinates_transform.py` & `matrix_package-23.4.29/matrix_package/coordinates_transform.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/density.py` & `matrix_package-23.4.29/matrix_package/density.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/density_test.py` & `matrix_package-23.4.29/matrix_package/density_test.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/gdr.py` & `matrix_package-23.4.29/matrix_package/gdr.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/get_file.py` & `matrix_package-23.4.29/matrix_package/get_file.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/molecule.py` & `matrix_package-23.4.29/matrix_package/molecule.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/params.py` & `matrix_package-23.4.29/matrix_package/params.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/pbc.py` & `matrix_package-23.4.29/matrix_package/pbc.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/periodic_bc.py` & `matrix_package-23.4.29/matrix_package/periodic_bc.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package/scale.py` & `matrix_package-23.4.29/matrix_package/scale.py`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/matrix_package.egg-info/PKG-INFO` & `matrix_package-23.4.29/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: matrix-package
-Version: 22.3.12
-Summary: Molecular dynamics code for the analysis of structural, dynamic, thermodynamic and electronic properties of certain 2D materials.
-Home-page: https://github.com/amieheessomba
-Author: Iréné Amiehe-Essomba 
-Author-email: ibamieheessomba@unistra.fr
-License: IPCMS
-Keywords: molecular dynamics matrix package
-Platform: UNKNOWN
-License-File: LICENCE
-
-matrix_package is a molecular dynamics analysis code allowing to calculate several structural, dynamic, thermodynamic properties of amorphous, crystalline or semi-amorphous and electronic systems of certain 2D layered materials of Van Der Waals.
-It is based on powerful solving algorithms, using MACHINE LEARNING to solve certain more or less complex problems such as the computation of the properties of dipole moments from Wanier centers.
-version 22.02.09-alpha offers the possibility of processing six different inputs.
-LAMMPS outputs, DL_POLY outputs, CPMD outputs, GAMESS outputs, Abinit outputs and VASP outputs.
-this version will evolve gradually and will take into account more versions of inputs.
-However, it has a module that allows you to convert an input into an XYZ file that it can then use to do several calculations. 
-
-
+Metadata-Version: 2.1
+Name: matrix_package
+Version: 23.4.29
+Summary: Molecular dynamics code for the analysis of structural, dynamic, thermodynamic and electronic properties of certain 2D materials.
+Home-page: https://github.com/amieheessomba
+Author: Iréné Amiehe-Essomba 
+Author-email: ibamieheessomba@unistra.fr
+License: IPCMS
+Keywords: molecular dynamics matrix package
+Platform: UNKNOWN
+License-File: LICENCE
+
+matrix_package is a molecular dynamics analysis code allowing to calculate several structural, dynamic, thermodynamic properties of amorphous, crystalline or semi-amorphous and electronic systems of certain 2D layered materials of Van Der Waals.
+It is based on powerful solving algorithms, using MACHINE LEARNING to solve certain more or less complex problems such as the computation of the properties of dipole moments from Wanier centers.
+version 22.02.09-alpha offers the possibility of processing six different inputs.
+LAMMPS outputs, DL_POLY outputs, CPMD outputs, GAMESS outputs, Abinit outputs and VASP outputs.
+this version will evolve gradually and will take into account more versions of inputs.
+However, it has a module that allows you to convert an input into an XYZ file that it can then use to do several calculations. 
+
+
```

### Comparing `matrix_package-22.3.12/matrix_package.egg-info/SOURCES.txt` & `matrix_package-23.4.29/matrix_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matrix_package-22.3.12/setup.py` & `matrix_package-23.4.29/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 		return f.read() 
 
 def short_readme():
 	with open('README.md', 'r')  as f1:
 		return f1.read()
     	
 setup(name='matrix_package',
-	version='22.03.12',
+	version='23.04.29',
 	description = short_readme() , 
 	long_description = readme(),
 	url='https://github.com/amieheessomba',
 	author='Iréné Amiehe-Essomba ',
 	keywords = 'molecular dynamics matrix package',
 	install_requires = [
 	'markdown',
```

