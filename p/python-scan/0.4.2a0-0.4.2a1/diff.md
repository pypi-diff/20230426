# Comparing `tmp/python_scan-0.4.2a0-py3-none-any.whl.zip` & `tmp/python_scan-0.4.2a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 9627 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    28928 b- defN 23-Apr-25 21:17 python_scan-0.4.2a0.data/scripts/PORT_SCAN.py
--rw-rw-rw-  2.0 fat     1684 b- defN 23-Apr-25 21:26 python_scan-0.4.2a0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 21:26 python_scan-0.4.2a0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-25 21:26 python_scan-0.4.2a0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      424 b- defN 23-Apr-25 21:26 python_scan-0.4.2a0.dist-info/RECORD
-5 files, 31129 bytes uncompressed, 8831 bytes compressed:  71.6%
+Zip file size: 9659 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    29334 b- defN 23-Apr-26 08:10 python_scan-0.4.2a1.data/scripts/PORT_SCAN.py
+-rw-rw-rw-  2.0 fat     1684 b- defN 23-Apr-26 08:24 python_scan-0.4.2a1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-26 08:24 python_scan-0.4.2a1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-26 08:24 python_scan-0.4.2a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      424 b- defN 23-Apr-26 08:24 python_scan-0.4.2a1.dist-info/RECORD
+5 files, 31535 bytes uncompressed, 8863 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: python_scan-0.4.2a0.data/scripts/PORT_SCAN.py
+Filename: python_scan-0.4.2a1.data/scripts/PORT_SCAN.py
 Comment: 
 
-Filename: python_scan-0.4.2a0.dist-info/METADATA
+Filename: python_scan-0.4.2a1.dist-info/METADATA
 Comment: 
 
-Filename: python_scan-0.4.2a0.dist-info/WHEEL
+Filename: python_scan-0.4.2a1.dist-info/WHEEL
 Comment: 
 
-Filename: python_scan-0.4.2a0.dist-info/top_level.txt
+Filename: python_scan-0.4.2a1.dist-info/top_level.txt
 Comment: 
 
-Filename: python_scan-0.4.2a0.dist-info/RECORD
+Filename: python_scan-0.4.2a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `python_scan-0.4.2a0.data/scripts/PORT_SCAN.py` & `python_scan-0.4.2a1.data/scripts/PORT_SCAN.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,31 +13,42 @@
     import os
     import nmap
     from pathlib import Path
     from pyExploitDb import PyExploitDb
     import colorama
     from colorama import Fore
     colorama.init()
+
     print(Fore.BLUE + "\n[♦]" +
           Fore.YELLOW + " Modulos importados correctamente, procediendo con la ejecución del programa")
     time.sleep(1)
+    modules = True
 except Exception as e:
     # If there are any errors encountered during the importing of the modules,
     # then we display the error message on the console screen
-    print('Existen modulos necesario que no tiene instalado... \n{}'.format(e))
-    print("Para instalar los modulos necesarios ejecte el siguente comando \n 'pip install -r requirements.txt'")
-
-
-nm = nmap.PortScanner()
-open_ports = []
+    print('Existen modulos necesarios que no tiene instalado... \n\n')
+    time.sleep(2)
+    exit()
+
+if modules:
+    nm = nmap.PortScanner()
+    open_ports = []
 
 
 def verifi_tools():
-    pass
-
+    print(Fore.BLUE + "\n[♦]" +
+          Fore.YELLOW + " Verificando herramientas necesarias...")
+    time.sleep(2)
+    if os.name == "posix":
+        if os.system('command -v nmap > /dev/null') != 0:
+            print(Fore.RED + "\n[♦] No tienes NMAP instalado...")
+    else:
+        if os.system("where nmap") != 0:
+            print(Fore.RED + "\n[♦] No tienes NMAP instalado...")
+            exit()
 
 def clean():
     if os.name == "posix":
         os.system("clear")
     else:
         os.system("cls")
 
@@ -701,15 +712,17 @@
 
 
 def main():
     try:
         # Empezamos código limpiando pantalla
         clean()
         # Miramos si eres admin / root
-        # is_admin()
+        is_admin()
+        # Verificamos NMAP
+        verifi_tools()
         # Iniciamos la herramienta
         enter_arguments()
 
     # Salida con CTRL + C
     except KeyboardInterrupt:
         print("\n\nSaliendo del programa...")
         exit()
```

## Comparing `python_scan-0.4.2a0.dist-info/METADATA` & `python_scan-0.4.2a1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-scan
-Version: 0.4.2a0
+Version: 0.4.2a1
 Summary: Herramienta para escaneo de puertos/vulners/explits en una IP
 Home-page: https://github.com/TownPablo/PORT_SCANNER
 Author: __TownPablo__
 Author-email: pablodiez024@proton.me
 License: MIT
 Keywords: port scan,seguridad,redes
 Description-Content-Type: text/markdown
```

