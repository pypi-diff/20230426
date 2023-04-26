# Comparing `tmp/RaphaelSomaDIT-2.3-py3-none-any.whl.zip` & `tmp/RaphaelSomaDIT-2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5068 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    10536 b- defN 23-Apr-25 13:06 RaphaelSomaDIT/__init__.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Apr-25 14:08 RaphaelSomaDIT-2.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Apr-25 14:08 RaphaelSomaDIT-2.3.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      434 b- defN 23-Apr-25 14:08 RaphaelSomaDIT-2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 14:08 RaphaelSomaDIT-2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Apr-25 14:08 RaphaelSomaDIT-2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      591 b- defN 23-Apr-25 14:08 RaphaelSomaDIT-2.3.dist-info/RECORD
-7 files, 13821 bytes uncompressed, 4014 bytes compressed:  71.0%
+Zip file size: 5049 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    10577 b- defN 23-Apr-25 16:37 RaphaelSomaDIT/__init__.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Apr-25 16:38 RaphaelSomaDIT-2.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Apr-25 16:38 RaphaelSomaDIT-2.4.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      434 b- defN 23-Apr-25 16:38 RaphaelSomaDIT-2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 16:38 RaphaelSomaDIT-2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Apr-25 16:38 RaphaelSomaDIT-2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      591 b- defN 23-Apr-25 16:38 RaphaelSomaDIT-2.4.dist-info/RECORD
+7 files, 13862 bytes uncompressed, 3995 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: RaphaelSomaDIT/__init__.py
 Comment: 
 
-Filename: RaphaelSomaDIT-2.3.dist-info/LICENSE
+Filename: RaphaelSomaDIT-2.4.dist-info/LICENSE
 Comment: 
 
-Filename: RaphaelSomaDIT-2.3.dist-info/LICENSE.txt
+Filename: RaphaelSomaDIT-2.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: RaphaelSomaDIT-2.3.dist-info/METADATA
+Filename: RaphaelSomaDIT-2.4.dist-info/METADATA
 Comment: 
 
-Filename: RaphaelSomaDIT-2.3.dist-info/WHEEL
+Filename: RaphaelSomaDIT-2.4.dist-info/WHEEL
 Comment: 
 
-Filename: RaphaelSomaDIT-2.3.dist-info/top_level.txt
+Filename: RaphaelSomaDIT-2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: RaphaelSomaDIT-2.3.dist-info/RECORD
+Filename: RaphaelSomaDIT-2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RaphaelSomaDIT/__init__.py

```diff
@@ -227,22 +227,26 @@
                 module = session.get(module).text
                 # soup = bs(module,'html.parser')
                 soup = pd.read_html(module)
                 modules = soup[0]['Code'][0][-4]
                 # soup = soup.find('table').find_all('td')[1].text
                 # modules = soup[-4]
                 self.NTA_level = modules
-                print(self.NTA_level)
+                
                 sems = list(soup[0]['Semester'])
+                
                 if datetime.datetime.now().month>=4 and datetime.datetime.now().month<=10:
                     self.sem = sems[-1]
+                    return self.sem
                     
                 else:
                     self.sem = sems[0]
                     
+                    return self.sem
+                    
                     
                 
                 
             elif 'invalid' in p.text:
                self.error = 'Login Failed: invalid credentials'
             else:
                 self.error = 'invalid status code' 
@@ -307,9 +311,9 @@
                self.error = 'Login Failed: invalid credentials'
             else:
                 self.error = 'invalid status code' 
         except:
             self.error = 'no internet connection'
                 
 rex=raphael()
-rex.studentInfo('rsiphael@gmail.com','#Raphael1996')
+
```

## Comparing `RaphaelSomaDIT-2.3.dist-info/LICENSE` & `RaphaelSomaDIT-2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `RaphaelSomaDIT-2.3.dist-info/LICENSE.txt` & `RaphaelSomaDIT-2.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

