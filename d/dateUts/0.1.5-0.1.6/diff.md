# Comparing `tmp/dateUts-0.1.5.tar.gz` & `tmp/dateUts-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dateUts-0.1.5.tar", last modified: Thu Apr 20 20:15:56 2023, max compression
+gzip compressed data, was "dateUts-0.1.6.tar", last modified: Wed Apr 26 21:24:11 2023, max compression
```

## Comparing `dateUts-0.1.5.tar` & `dateUts-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 20:15:56.494061 dateUts-0.1.5/
--rw-rw-rw-   0        0        0      583 2023-04-20 19:55:45.000000 dateUts-0.1.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2022-05-25 14:00:44.000000 dateUts-0.1.5/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2022-05-25 22:21:08.000000 dateUts-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6136 2023-04-20 20:15:56.493061 dateUts-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3159 2023-04-20 19:57:17.000000 dateUts-0.1.5/README.md
--rw-rw-rw-   0        0        0      122 2022-10-03 19:44:47.000000 dateUts-0.1.5/commands.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 20:15:56.481069 dateUts-0.1.5/dateUts/
--rw-rw-rw-   0        0        0     4751 2023-04-20 19:55:03.000000 dateUts-0.1.5/dateUts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:15:56.491063 dateUts-0.1.5/dateUts.egg-info/
--rw-rw-rw-   0        0        0     6136 2023-04-20 20:15:56.000000 dateUts-0.1.5/dateUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-04-20 20:15:56.000000 dateUts-0.1.5/dateUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 20:15:56.000000 dateUts-0.1.5/dateUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-20 20:15:56.000000 dateUts-0.1.5/dateUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 20:15:56.495061 dateUts-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-04-20 20:03:43.000000 dateUts-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:24:11.822960 dateUts-0.1.6/
+-rw-rw-rw-   0        0        0      644 2023-04-26 21:23:08.000000 dateUts-0.1.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 dateUts-0.1.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 dateUts-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4331 2023-04-26 21:24:11.821963 dateUts-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3159 2023-04-26 21:06:44.000000 dateUts-0.1.6/README.md
+-rw-rw-rw-   0        0        0      122 2023-04-26 21:06:44.000000 dateUts-0.1.6/commands.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 21:24:11.790048 dateUts-0.1.6/dateUts/
+-rw-rw-rw-   0        0        0     4964 2023-04-26 21:20:07.000000 dateUts-0.1.6/dateUts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:24:11.820966 dateUts-0.1.6/dateUts.egg-info/
+-rw-rw-rw-   0        0        0     4331 2023-04-26 21:24:11.000000 dateUts-0.1.6/dateUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-04-26 21:24:11.000000 dateUts-0.1.6/dateUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 21:24:11.000000 dateUts-0.1.6/dateUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 21:24:11.000000 dateUts-0.1.6/dateUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 21:24:11.822960 dateUts-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-04-26 21:22:35.000000 dateUts-0.1.6/setup.py
```

### Comparing `dateUts-0.1.5/LICENCE.txt` & `dateUts-0.1.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.5/README.md` & `dateUts-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dateUts-0.1.5/dateUts/__init__.py` & `dateUts-0.1.6/dateUts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
     date = None
 
     def __init__(self,date):
         self.date = date
 
     def is_weekend(self):
         return self.date.weekday() in [5, 6]
+    
+    def weekday(self):
+        self.date.weekday()
 
     def __repr__(self):
         return f"<DateUts {self.date.strftime('%Y-%m-%d %H:%M:%S')}>"
 
 
 # output: True (2023-04-22 is a Saturday)
 
@@ -44,29 +47,29 @@
 
 #========= USAGE ============
 #Ex1:
 # > today()  ,  today(fmt='%Y-%m-%d')   ,   today(fmt='sql')
 # > <datetime>, 'yyyy-MM-dd',  'yyyy-MM-dd'
 
 def today(fmt=None,addDays=0):
-    v =  dt.now() 
+    v =  dt.now().date()
     v =  v if not addDays else dateAdd(today(),addDays,'day')
     return fmtDate(v,fmt)
 
 #========= USAGE ============
 #Ex1:
 # > yesterday()  ,  yesterday(fmt='%Y-%m-%d')   ,   yesterday(fmt='sql')
 # > <datetime>, 'yyyy-MM-dd',  'yyyy-MM-dd'
 
 def yesterday(fmt=None):
-    v = dt.now() - td(1)
+    v = today().date - td(1)
     return fmtDate(v,fmt)
 
 def tomorrow(fmt=None):
-    v = dt.now() + td(1)
+    v = today().date + td(1)
     return fmtDate(v,fmt)
 
 #========= USAGE ============
 #Ex1:
 # > start,end = <date:2022-05-23>,<date:2022-05-24>
 # > dateRange(start,end) ,  dateRange('2022-05-23',1,'day',fmt='%Y-%m-%d')   ,   dateRange('2022-05-23',1,'day',fmt='sql')
 # > [<datetime>,<datetime>], ['2022-05-23','2022-05-24'],  ['2022-05-23','2022-05-24']
@@ -89,14 +92,15 @@
 # > dateAdd('2022-05-23',1,'day') ,  dateAdd('2022-05-23',1,'day',fmt='%Y-%m-%d')   ,   dateAdd('2022-05-23',1,'day',fmt='sql')
 # > <datetime>, '2022-05-24',  '2022-05-24'
 #Ex2:
 # > dateAdd('2022-05-23',-1,'day') ,  dateAdd('2022-05-23',-1,'day',fmt='%Y-%m-%d')   ,   dateAdd('2022-05-23',-1,'day',fmt='sql')
 # > <datetime>, '2022-05-22',  '2022-05-22'
 
 def dateAdd(date:date,qtd:int,unit:str="day",fmt=None):
+    date = date.date if isinstance(date,DateUts) else date
     if unit == 'day':
         v = date + td(qtd) if qtd > 0 else date - td(abs(qtd))
     elif unit == 'year':
         v = date.replace(year = date.year + qtd)
     elif unit == 'hours':
         v = date + td(hours=qtd)
     elif unit == 'minutes':
@@ -133,26 +137,29 @@
 #========= USAGE ============
 #Ex1:
 # > today()  ,  today(fmt='%Y-%m-%d')   ,   today(fmt='sql')
 # > <datetime>, 'yyyy-MM-dd',  'yyyy-MM-dd'
 
 def fmtDate(dt:date,fmt:str):
     fmt= fmt if not fmt else ("%Y-%m-%d" if fmt == "sql" else fmt)
-    return DateUts(dt if not fmt else dt.strftime(fmt))
+    dt = dt.date if isinstance(dt,DateUts) else dt
+
+    return DateUts(dt) if not fmt else dt.strftime(fmt)
 
 def dateMatch(dt:str,fmt:str):
     fmt = "%Y-%m-%d" if fmt == "sql" else fmt
 
     try:
         dt = datetime.strptime(dt,fmt)
     except ValueError:
         return False
 
     return True
 
+lastWorkingDate(today())
 
 Fnc_noWeekends = lambda dt:dt.weekday() not in [5,6]
 
 # a = DateUts(dt.now())
 # print(a)
 # a = lastWorkingDate(fmt="%Y-%m-%d")
 # rng = dateRange(sqlToDate("2022-05-01"),sqlToDate("2022-05-10"))
```

### Comparing `dateUts-0.1.5/setup.py` & `dateUts-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='dateUts',
-  version='0.1.5',
+  version='0.1.6',
   description='Date package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

