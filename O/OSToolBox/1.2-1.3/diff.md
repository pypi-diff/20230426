# Comparing `tmp/OSToolBox-1.2.tar.gz` & `tmp/OSToolBox-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OSToolBox-1.2.tar", last modified: Tue Jan 31 21:44:04 2023, max compression
+gzip compressed data, was "dist/OSToolBox-1.3.tar", last modified: Tue Apr 25 19:40:03 2023, max compression
```

## Comparing `OSToolBox-1.2.tar` & `OSToolBox-1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ostocker  (1000) ostocker  (1000)        0 2023-01-31 21:44:04.844627 OSToolBox-1.2/
-drwxrwxr-x   0 ostocker  (1000) ostocker  (1000)        0 2023-01-31 21:44:04.844627 OSToolBox-1.2/GDALToolBox/
--rwxr-xr-x   0 ostocker  (1000) ostocker  (1000)      206 2023-01-30 21:18:02.000000 OSToolBox-1.2/GDALToolBox/__init__.py
--rwxr-xr-x   0 ostocker  (1000) ostocker  (1000)     6223 2023-01-30 21:19:55.000000 OSToolBox-1.2/GDALToolBox/gdaltools.py
-drwxrwxr-x   0 ostocker  (1000) ostocker  (1000)        0 2023-01-31 21:44:04.844627 OSToolBox-1.2/OSToolBox/
--rwxr-xr-x   0 ostocker  (1000) ostocker  (1000)      202 2021-04-20 19:35:41.000000 OSToolBox-1.2/OSToolBox/__init__.py
--rwxr-xr-x   0 ostocker  (1000) ostocker  (1000)    23683 2023-01-30 21:26:36.000000 OSToolBox-1.2/OSToolBox/tools.py
-drwxrwxr-x   0 ostocker  (1000) ostocker  (1000)        0 2023-01-31 21:44:04.844627 OSToolBox-1.2/OSToolBox.egg-info/
--rw-rw-r--   0 ostocker  (1000) ostocker  (1000)      240 2023-01-31 21:44:04.000000 OSToolBox-1.2/OSToolBox.egg-info/PKG-INFO
--rw-rw-r--   0 ostocker  (1000) ostocker  (1000)      304 2023-01-31 21:44:04.000000 OSToolBox-1.2/OSToolBox.egg-info/SOURCES.txt
--rw-rw-r--   0 ostocker  (1000) ostocker  (1000)        1 2023-01-31 21:44:04.000000 OSToolBox-1.2/OSToolBox.egg-info/dependency_links.txt
--rw-rw-r--   0 ostocker  (1000) ostocker  (1000)        1 2023-01-31 21:44:04.000000 OSToolBox-1.2/OSToolBox.egg-info/not-zip-safe
--rw-rw-r--   0 ostocker  (1000) ostocker  (1000)       17 2023-01-31 21:44:04.000000 OSToolBox-1.2/OSToolBox.egg-info/requires.txt
--rw-rw-r--   0 ostocker  (1000) ostocker  (1000)       22 2023-01-31 21:44:04.000000 OSToolBox-1.2/OSToolBox.egg-info/top_level.txt
--rw-rw-r--   0 ostocker  (1000) ostocker  (1000)      240 2023-01-31 21:44:04.844627 OSToolBox-1.2/PKG-INFO
--rwxr-xr-x   0 ostocker  (1000) ostocker  (1000)      367 2023-01-30 21:26:38.000000 OSToolBox-1.2/README.md
--rw-rw-r--   0 ostocker  (1000) ostocker  (1000)       38 2023-01-31 21:44:04.844627 OSToolBox-1.2/setup.cfg
--rwxr-xr-x   0 ostocker  (1000) ostocker  (1000)      574 2023-01-31 21:43:58.000000 OSToolBox-1.2/setup.py
+drwxrwxr-x   0 ostocker  (1000) ostocker  (1000)        0 2023-04-25 19:40:03.000000 OSToolBox-1.3/
+drwxrwxr-x   0 ostocker  (1000) ostocker  (1000)        0 2023-04-25 19:40:03.000000 OSToolBox-1.3/GDALToolBox/
+-rwxr-xr-x   0 ostocker  (1000) ostocker  (1000)      206 2023-01-30 21:18:02.000000 OSToolBox-1.3/GDALToolBox/__init__.py
+-rwxr-xr-x   0 ostocker  (1000) ostocker  (1000)     6223 2023-01-30 21:19:55.000000 OSToolBox-1.3/GDALToolBox/gdaltools.py
+drwxrwxr-x   0 ostocker  (1000) ostocker  (1000)        0 2023-04-25 19:40:03.000000 OSToolBox-1.3/OSToolBox/
+-rwxr-xr-x   0 ostocker  (1000) ostocker  (1000)      202 2021-04-20 19:35:41.000000 OSToolBox-1.3/OSToolBox/__init__.py
+-rwxr-xr-x   0 ostocker  (1000) ostocker  (1000)    24695 2023-04-18 15:55:45.000000 OSToolBox-1.3/OSToolBox/tools.py
+drwxrwxr-x   0 ostocker  (1000) ostocker  (1000)        0 2023-04-25 19:40:03.000000 OSToolBox-1.3/OSToolBox.egg-info/
+-rw-rw-r--   0 ostocker  (1000) ostocker  (1000)      240 2023-04-25 19:40:03.000000 OSToolBox-1.3/OSToolBox.egg-info/PKG-INFO
+-rw-rw-r--   0 ostocker  (1000) ostocker  (1000)      304 2023-04-25 19:40:03.000000 OSToolBox-1.3/OSToolBox.egg-info/SOURCES.txt
+-rw-rw-r--   0 ostocker  (1000) ostocker  (1000)        1 2023-04-25 19:40:03.000000 OSToolBox-1.3/OSToolBox.egg-info/dependency_links.txt
+-rw-rw-r--   0 ostocker  (1000) ostocker  (1000)        1 2023-04-25 19:40:03.000000 OSToolBox-1.3/OSToolBox.egg-info/not-zip-safe
+-rw-rw-r--   0 ostocker  (1000) ostocker  (1000)       17 2023-04-25 19:40:03.000000 OSToolBox-1.3/OSToolBox.egg-info/requires.txt
+-rw-rw-r--   0 ostocker  (1000) ostocker  (1000)       22 2023-04-25 19:40:03.000000 OSToolBox-1.3/OSToolBox.egg-info/top_level.txt
+-rw-rw-r--   0 ostocker  (1000) ostocker  (1000)      240 2023-04-25 19:40:03.000000 OSToolBox-1.3/PKG-INFO
+-rwxr-xr-x   0 ostocker  (1000) ostocker  (1000)      367 2023-01-30 21:26:38.000000 OSToolBox-1.3/README.md
+-rw-rw-r--   0 ostocker  (1000) ostocker  (1000)       38 2023-04-25 19:40:03.000000 OSToolBox-1.3/setup.cfg
+-rwxr-xr-x   0 ostocker  (1000) ostocker  (1000)      672 2023-04-25 19:37:41.000000 OSToolBox-1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `OSToolBox-1.2/GDALToolBox/gdaltools.py` & `OSToolBox-1.3/GDALToolBox/gdaltools.py`

 * *Files identical despite different names*

### Comparing `OSToolBox-1.2/OSToolBox/tools.py` & `OSToolBox-1.3/OSToolBox/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,28 +68,46 @@
     cax1 = ax1_divider.append_axes("right", size=0.1, pad="2%")
     plt.colorbar(orientation='vertical', cax=cax1)
     if save is not None :
         plt.savefig(save)
     if show : 
         plt.show()
 
-def plotLogGraph(x,y,datalabel,xlabel,ylabel,title,save=None,show=1):
+def plotGraph(x,array_y,datalabel="",xlabel="",ylabel="",xlimit=None,ylimit=None,title="",fontsize=10,log=False,save=None,grid=True,dpi=600,show=1):
+    #array_y can be y data or an array of y datas to plot together
     #datalabel=name of data
     #xlabel & ylabel = name of x and Y data
     #save : path to save
     #show = true to display it
+    plt.rcParams.update({'font.size': fontsize})
     fig,ax=plt.subplots()
-    ax.semilogy(x, y,label=datalabel)
+    array_y=np.asarray(array_y)#cast as np array
+    if len(array_y.shape)>1:
+        for i,y in enumerate(array_y):
+            if log:
+                ax.semilogy(x, y,label=datalabel[i])
+            else:
+                ax.plot(x, y,label=datalabel[i])
+    else :
+        if log:
+            ax.semilogy(x, array_y,label=datalabel)
+        else:
+            ax.plot(x, array_y,label=datalabel)
+    if xlimit is not None : 
+        plt.xlim(xlimit)
+    if ylimit is not None :
+        plt.ylim(ylimit)
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
     plt.title(title)
     ax.legend()
-    plt.grid(True)
+    plt.grid(grid)
+    plt.tight_layout()
     if save is not None :
-        plt.savefig(save)
+        plt.savefig(save,dpi=dpi)
     if show : 
         plt.show()
 
 
 """TIMER"""
 def chrono(tps=-1):
     #tps = reference time
@@ -205,18 +223,21 @@
     if nat:
         list_dir.sort(key=natural_keys)
     else :
         list_dir.sort()
 #    print(list_file)
     return list_dir
 
-def pathBranch(path):
+def pathBranch(path,n=1):
     #return root of file name
     #ex : pathBranch("media/ostocker/ilove.you") return "media/ostocker"
-    return os.path.abspath(os.path.join(path, os.pardir))
+    #n : number of back setps : pathBranch("media/ostocker/ilove.you",2) return "media"
+    for i in range(n):
+        path=os.path.abspath(os.path.join(path, os.pardir))
+    return path
 
 def pathRelative(path,n):
     #return rrelative path give certain depth n
     #ex : pathBranch("media/ostocker/ilove.you",1) return "ostocker/ilove.you"
     leafed_branch=pathLeafExt(path)
     rooted_branch=pathBranch(path)
     for i in range(n):
@@ -428,14 +449,19 @@
     #Force = True skip border finding and use mini and max values
     
     if not force:
         maxi=a.max()
         mini=a.min()
     return (a-mini)/(maxi-mini)
 
+def movingAverage(x, window_size):
+    #For smoothing curve, it does loop around, so return a vector of the same size
+    window= np.ones(int(window_size))/float(window_size)
+    return np.convolve(x, window, 'same')
+
 """ STRING"""
 def find_nth(string, substring, n):
     if (n == 1):
         return string.find(substring)
     else:
         return string.find(substring, find_nth(string, substring, n - 1) + 1)
    
@@ -678,15 +704,14 @@
     field_list = list(field_list) if (type(field_list) == list or type(field_list) == tuple) else list((field_list,))
     for i, field in enumerate(field_list):
         if field.ndim < 2:
             field_list[i] = field.reshape(-1, 1)
         if field.ndim > 2:
             print('fields have more than 2 dimensions')
             return False    
-    print("aaaaaa", field_list)
     # check all fields have the same number of data
     n_points = [field.shape[0] for field in field_list]
     if not np.all(np.equal(n_points, n_points[0])):
         print('wrong field dimensions')
         return False    
 
     # Check if field_names and field_list have same nb of column
```

