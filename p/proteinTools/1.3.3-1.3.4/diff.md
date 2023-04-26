# Comparing `tmp/proteinTools-1.3.3.tar.gz` & `tmp/proteinTools-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.3.3.tar", last modified: Tue Apr 25 04:56:05 2023, max compression
+gzip compressed data, was "proteinTools-1.3.4.tar", last modified: Wed Apr 26 01:41:49 2023, max compression
```

## Comparing `proteinTools-1.3.3.tar` & `proteinTools-1.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-25 04:56:05.948302 proteinTools-1.3.3/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.3.3/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-25 04:56:05.944366 proteinTools-1.3.3/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.3.3/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-25 04:56:05.830642 proteinTools-1.3.3/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    53090 2023-04-25 04:55:56.000000 proteinTools-1.3.3/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.3.3/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-25 04:56:05.924874 proteinTools-1.3.3/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-25 04:56:05.000000 proteinTools-1.3.3/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-25 04:56:05.000000 proteinTools-1.3.3/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-25 04:56:05.000000 proteinTools-1.3.3/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-25 04:56:05.000000 proteinTools-1.3.3/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-25 04:56:05.000000 proteinTools-1.3.3/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-25 04:56:05.953320 proteinTools-1.3.3/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-25 04:55:23.000000 proteinTools-1.3.3/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-26 01:41:49.117251 proteinTools-1.3.4/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.3.4/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-26 01:41:49.113927 proteinTools-1.3.4/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.3.4/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-26 01:41:48.995367 proteinTools-1.3.4/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    53271 2023-04-26 01:32:02.000000 proteinTools-1.3.4/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.3.4/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-26 01:41:49.100507 proteinTools-1.3.4/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-26 01:41:48.000000 proteinTools-1.3.4/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-26 01:41:48.000000 proteinTools-1.3.4/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-26 01:41:48.000000 proteinTools-1.3.4/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-26 01:41:48.000000 proteinTools-1.3.4/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-26 01:41:48.000000 proteinTools-1.3.4/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-26 01:41:49.121290 proteinTools-1.3.4/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-26 01:41:41.000000 proteinTools-1.3.4/setup.py
```

### Comparing `proteinTools-1.3.3/LICENSE` & `proteinTools-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.3.3/proteinTools/PT.py` & `proteinTools-1.3.4/proteinTools/PT.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,24 +31,25 @@
 
 class atom:
     """
     Atom class
 
     This class contains the essential parameters of an individual atom in a protein structural file, including the coordinates, element, atomic mass, parent residue, and line data.
     """
-    def __init__(self, element, x, y, z, data, residue = ''):
+    def __init__(self, element, x, y, z, data, residue = '', number = 0):
         
         self.element = element
         self.x = x
         self.y = y
         self.z = z
         self.residue = residue
         self.data = data
         self.mass = atom_dict[self.element]
         self.radius = element_radii[self.element]
+        self.number = number
         
 class residue:
     """
     Residue class
     
     This class contains the essential parameters of an individual residue in a protein structural file, including the child atoms, protein sidechain, residue index, and type of amino acid.
     """
@@ -437,17 +438,17 @@
                     element = line[76:79].strip()
                     if element not in atom_keys:
                         e = element[:1]
                         if e not in atom_keys:
                             e = element[1:]
                         element = e
                     try:
-                        atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), residue = res.chain + str(resnum), data = line)
+                        atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), residue = res.chain + str(resnum), data = line, number = int(numconv.sub('', line[6:13])))
                     except:
-                        atm = atom(element, float(line[30:37].strip()), float(line[38:46].strip()), float(line[47:55].strip()), residue = res.chain + str(resnum), data = line)
+                        atm = atom(element, float(line[30:37].strip()), float(line[38:46].strip()), float(line[47:55].strip()), residue = res.chain + str(resnum), data = line, number = int(numconv.sub('', line[6:13])))
                     res.atoms.append(atm)
             
             
             if self.ID_type == 'PDB':
                 #Generates ligands if PDB filetype and ligands in file
                 sheet, helix, chainkeys = [], [], list(self.chains.keys())
                 for count, line in enumerate(data):
@@ -467,15 +468,15 @@
                                 current_ligand_index += 1
                         element = line[76:80].strip()
                         if element not in atom_keys:
                             e = element[:1]
                             if e not in atom_keys:
                                 e = element[1:]
                             element = e
-                        atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), data = line)
+                        atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), data = line, number = int(numconv.sub('', line[6:13])))
                         try:
                             self.ligand_list[current_ligand_index].atoms.append(atm)
                         except:
                             try:
                                  self.ligand_list[current_ligand_index + 1].atoms.append(atm)
                             except:
                                  continue
@@ -742,19 +743,18 @@
         -------
         class
             Returns the atom class at the given index.
         """
         ac = 0
         for res in self.residue_list:
             for atom in res.atoms:
-                if ac == atom_index:
-                    atom_items = {'element':atom.element, 'x':atom.x, 'y':atom.y, 'z':atom.z, 'residue':atom.residue, 'data':atom.data}
-                    atm = pd.Series(atom_items, index = ['element', 'x', 'y', 'z', 'residue', 'data'])
+                if atom.number == atom_index:
+                    atom_items = {'element':atom.element, 'x':atom.x, 'y':atom.y, 'z':atom.z, 'residue':atom.residue, 'data':atom.data, 'mass':atom.mass}
+                    atm = pd.Series(atom_items, index = ['element', 'x', 'y', 'z', 'residue', 'data', 'mass'])
                     return atm
-                ac += 1
         return 'Index is larger than total number of atoms!'
     
     def concat(self, start, stop, destination = os.getcwd()):
         """
         Residue Concatenation
     
         This method allows for the concatenation of residues into a sub-structural file containing only the indexed residues.
```

### Comparing `proteinTools-1.3.3/setup.py` & `proteinTools-1.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.3.3",
+    version = "1.3.4",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```

