# Comparing `tmp/bacteria-0.1.5.tar.gz` & `tmp/bacteria-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.1.5.tar", last modified: Mon Apr 24 19:07:53 2023, max compression
+gzip compressed data, was "bacteria-0.1.6.tar", last modified: Tue Apr 25 17:49:31 2023, max compression
```

## Comparing `bacteria-0.1.5.tar` & `bacteria-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 19:07:53.595000 bacteria-0.1.5/
--rw-rw-rw-   0        0        0      593 2023-04-24 19:07:53.479000 bacteria-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2023-04-21 18:30:09.000000 bacteria-0.1.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-24 19:07:53.082000 bacteria-0.1.5/bacteria/
--rw-rw-rw-   0        0        0       67 2023-04-23 10:02:48.000000 bacteria-0.1.5/bacteria/__init__.py
--rw-rw-rw-   0        0        0   148163 2023-04-24 19:07:40.000000 bacteria-0.1.5/bacteria/functions.py
--rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.1.5/bacteria/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-24 19:07:53.439000 bacteria-0.1.5/bacteria.egg-info/
--rw-rw-rw-   0        0        0      593 2023-04-24 19:07:52.000000 bacteria-0.1.5/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-04-24 19:07:52.000000 bacteria-0.1.5/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 19:07:52.000000 bacteria-0.1.5/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-04-24 19:07:52.000000 bacteria-0.1.5/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 19:07:52.000000 bacteria-0.1.5/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 19:07:53.563000 bacteria-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1128 2023-04-24 19:07:47.000000 bacteria-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:49:31.291000 bacteria-0.1.6/
+-rw-rw-rw-   0        0        0      593 2023-04-25 17:49:31.020000 bacteria-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2023-04-21 18:30:09.000000 bacteria-0.1.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-25 17:49:29.257000 bacteria-0.1.6/bacteria/
+-rw-rw-rw-   0        0        0       67 2023-04-23 10:02:48.000000 bacteria-0.1.6/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   149375 2023-04-25 17:48:52.000000 bacteria-0.1.6/bacteria/functions.py
+-rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.1.6/bacteria/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:49:30.640000 bacteria-0.1.6/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-04-25 17:49:24.000000 bacteria-0.1.6/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-04-25 17:49:24.000000 bacteria-0.1.6/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 17:49:24.000000 bacteria-0.1.6/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-04-25 17:49:24.000000 bacteria-0.1.6/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 17:49:24.000000 bacteria-0.1.6/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 17:49:31.275000 bacteria-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2023-04-25 17:49:05.000000 bacteria-0.1.6/setup.py
```

### Comparing `bacteria-0.1.5/PKG-INFO` & `bacteria-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.5
+Version: 0.1.6
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.1.5/README.rst` & `bacteria-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `bacteria-0.1.5/bacteria/functions.py` & `bacteria-0.1.6/bacteria/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,17 @@
     Create a the volume column in 3d DataFrame. 
     v = np.pi*(l-w) * ((w/2)**2) + (4/3) * np.pi * ((w/2)**3)
     
     Parameters
     --------------
     df : DataFrame
         df from 3D data 
+    const : float (optional)
+        parameter extracted from the microscope to transform
+        pixel to micrometers
         
     Returns
     --------------
     df : pandas DataFrame
         df with the Volume column
     """
     vol_temp = []
@@ -152,15 +155,18 @@
     Create a the volume at birth and division column in 2d DataFrame. 
     v = np.pi*(l-w) * ((w/2)**2) + (4/3) * np.pi * ((w/2)**3)
     
     Parameters
     --------------
     df : DataFrame
         df from 2D data 
-        
+    const : float (optional)
+        parameter extracted from the microscope to transform
+        pixel to micrometers
+
     Returns
     --------------
     df : pandas DataFrame
         df with the Volume columns
     """
     vol_b,vol_d = [],[]
     
@@ -234,26 +240,29 @@
         time_frames = df[(df['Cell ID'] == cell) & (df['Time (fps)'])]['Time (fps)'].values
         cell_cycles.extend(pre.MinMaxScaler((0,1)).fit_transform(np.arange(0,len(time_frames),1).reshape(-1, 1)).flatten())
 
     df['Cell Cycle'] = cell_cycles
 
     return df
 
-def df_data3d(data, fps = 3, filters = True, comp = False):
+def df_data3d(data, fps = 3, filters = True, const = 0.1067,comp = False):
     """
     Create a pandas DataFrame of the 2D data using the headers pre-determined. 
     
     Parameters
     --------------
     data : clist.mat
         Supersegger clist already loaded
     fps : int (optional)
         Frames per second used in the experiment, usual 3
     filters : bool (optional)
         Filter data based on data2d['stat0'] = 2 and non NaN's
+    const : float (optional)
+        parameter extracted from the microscope to transform
+        pixel to micrometers
     comp : bool
         Input data are the compiled clists (clist for all xy/fovs)
         
     Returns
     --------------
     df : pandas DataFrame
         3D data in df
@@ -291,28 +300,31 @@
     df = pd.concat(df_temp)
     if filters:
         # remove the NaN values
         df = df[df['Age (Frames)'].isna()== False]
     # remove trailing space
     df.columns = df.columns.str.rstrip()
 
-    df = _volume(df)
+    df = _volume(df,const = const)
     
     return df,gc
 
-def df_data2d(data, fps = 3, comp = False):
+def df_data2d(data, fps = 3,const = 0.1067, comp = False):
     """
     Create a pandas DataFrame of the 2D data using the headers pre-determined. 
     
     Parameters
     --------------
     data: clist.mat
         Supersegger clist already loaded
     fps: int (optional)
         Frames per second used in the experiment, usual 3
+    const : float (optional)
+        parameter extracted from the microscope to transform
+        pixel to micrometers
     comp : bool
         Input data are the compiled clists (clist for all xy/fovs)
         
     Returns
     --------------
     df: pandas DataFrame
     
@@ -335,15 +347,15 @@
     df = pd.DataFrame(df_dict)
 
     # multiply the frame by the fps
     df['Cell birth time'] = df['Cell birth time'] * fps
     df['Cell age'] = df['Cell age'] * fps
 
     # add the volume columns
-    df = _volume2d(df)
+    df = _volume2d(df,const = const)
 
     if comp:
         off_sets , intervals = _off_set(df)
         # **this lasts step are unnecessary because the Cell ID follow the number of points in the data, it is just to assure to find this off sets**
 
         # update the intervals for each fov with the offsets
         for idx in range(len(intervals)):
@@ -376,15 +388,15 @@
     data2d = df_data2d(data,fps,comp)
     
     # vector of good cells
     good_cells = data2d[data2d['stat0']==2]['Cell ID'].values
 
     return good_cells
 
-def concatenate_clist(path, fps = 3, filters = True, save_mat = False, path2save = None , direct = False):
+def concatenate_clist(path, fps = 3, filters = True, save_mat = False, path2save = None , const = 0.1067 , direct = False):
     """
     Concatenate all c_list.mat from one experiment in DataFrames.
     
     Parameters
     --------------
     path : str
         Experiment path
@@ -393,14 +405,17 @@
     filters : bool (optional)
         Filter data based on data2d['stat0'] = 2 and is.nan()
     save_mat : bool (optional)
         save the dataframes in .mat format.
     path2save : str (optional)
         If false, the data will be saved into the current directory
         else, should pass a path to save.
+    const : float (optional)
+        parameter extracted from the microscope to transform
+        pixel to micrometers
     direct : bool
         If you have all the clists in one folder.
         
     Returns
     --------------
     data2D : pandas DataFrame
         with 2D data
@@ -415,16 +430,16 @@
         paths_xy = natsorted([os.path.join(path, files+os.sep+'clist.mat') for files in os.listdir(path) if files.startswith("xy") == True])
 
     df_temp_2 = []
     df_temp_3 = []
 
     for idx,mat in enumerate(paths_xy,1):
         data_temp = scipy.io.loadmat(mat)
-        data2D_temp = df_data2d(data_temp,fps)
-        data3D_temp,_ = df_data3d(data_temp,fps,False)
+        data2D_temp = df_data2d(data_temp,fps=fps, const=const)
+        data3D_temp,_ = df_data3d(data_temp,fps = fps, filter = False, const = const)
 
         if direct:
             data2D_temp['fov'] = 'xy' + str(idx)
             data3D_temp['fov'] = 'xy' + str(idx)
         else:
             data2D_temp['fov'] = mat.split('/')[-2]
             data3D_temp['fov'] = mat.split('/')[-2]
@@ -2759,15 +2774,15 @@
                 filtered_lineage.append(reverse_lineages[cell])
         else:
             if cell in natsorted(set(lineages_corr)):
                 filtered_lineage.append(reverse_lineages[cell])
 
     return filtered_lineage
 
-def plot_lineage_derivative(df_lineage,peaks,column = 'Fluor1 sum',derivative_column = 'Derivative',x_axis = 'Smoothed Volume',ax = None):
+def plot_lineage_derivative(df_lineage,peaks,column = 'Fluor1 sum',derivative_column = 'Derivative/V',x_axis = 'Smoothed Volume',ax = None):
     """
     Plot a single lineages derivative with the
     local minima and local maxmia. The input parameters
     are the output of 'lineage_derivative()'. This 
     function can receive both volume ('Smoothed Volume')
     and time ('Time (fps)') as the X axis.
 
@@ -3141,15 +3156,15 @@
         out.append(ax.set_title('Minima Distance',fontsize = 17))
         out.append(ax.set_xlabel(r'Volume at birth [$\mu m^3$]',fontsize = 15))
         out.append(ax.set_ylabel(r'Volume minima [$\mu m^3$]',fontsize = 15))
         out.append(ax.legend())
 
         return out
 
-def diff_minima(df_3d,df_2d,order = 3,pre = None,pos = None, adjust = False):
+def diff_minima(df_3d,df_2d,derivative_column = 'Derivative/V',order = 3,pre = None,pos = None, adjust = False):
     """
     Function to plot the distance between the minimas of
     the daughter and mother by the mothe volume. The 'pre' 
     and 'pos' to be used, both must be different than 'None'.
     It is possible to use a higher order together with adjust 
     order for each cell, the higher the order, the higher 
     the noise acceptance. Higher orders take longer and can 
@@ -3160,14 +3175,20 @@
 
     Parameters
     --------------
     df_3d : DataFrame
         DataFrame of 3D data
     df_2d : DataFrame
         DataFrame of 2D data
+    derivative_column : str (optional)
+        Derivative column to bin. Columns: 'Derivative',
+        'Derivative/V' is the derivative normalized by 
+        volume, 'Log Derivative' logarithm of the derivative,
+        'Log Derivative/V' logarithm of the derivative
+        normalized by volume. Default is 'Derivative/V'.
     order : int (optional)
         The order of the polynomial used to fit the 
         savgol_filter from scipy in 'lineage_derivative()'
         higher order is better to find more minimas, accept
         more noise. Default is 3.
     pre : int (optional)
         Save the data pre this moment in minutes
@@ -3212,15 +3233,15 @@
         temp_order = order
         daughter_cell1 = df_2d[df_2d['Cell ID']==cell]['Daughter1 ID'].values[0]
         daughter_cell2 = df_2d[df_2d['Cell ID']==cell]['Daughter2 ID'].values[0]
         
         if len(df_3d[df_3d['Cell ID']==daughter_cell1]) > 0:
             for attempt in range(for_range):
                 try:            
-                    df,peaks,_= lineage_derivative(df_3d,[cell,daughter_cell1],order = temp_order)
+                    df,peaks,_= lineage_derivative(df_3d,[cell,daughter_cell1],order = temp_order,derivative_column=derivative_column)
                     vol_dict['order'][cell] = temp_order
                     if 0 not in list(peaks['minima'].values()):
                         temp = df['Smoothed Volume'].values[list(peaks['minima'].values())]
                         time_pre = df_3d[df_3d['Cell ID']==daughter_cell1]['Time (fps)'].values[-1]
                         time_pos = df_3d[df_3d['Cell ID']==cell]['Time (fps)'].values[0]
                         size_birth.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
                         diff_size = temp[1]-temp[0]
@@ -3242,15 +3263,15 @@
                         continue
             # else:
             # 	pass
 
         elif len(df_3d[df_3d['Cell ID']==daughter_cell2]) > 0:
             for attempt in range(for_range):
                 try:
-                    df,peaks,_= lineage_derivative(df_3d,[cell,daughter_cell2],order = temp_order)
+                    df,peaks,_= lineage_derivative(df_3d,[cell,daughter_cell2],order = temp_order,derivative_column=derivative_column)
                     vol_dict['order'][cell] = temp_order
                     if 0 not in list(peaks['minima'].values()):
                         temp = df['Smoothed Volume'].values[list(peaks['minima'].values())]
                         time_pre = df_3d[df_3d['Cell ID']==daughter_cell2]['Time (fps)'].values[-1]
                         time_pos = df_3d[df_3d['Cell ID']==cell]['Time (fps)'].values[0]
                         size_birth.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
                         diff_size = temp[1]-temp[0]
@@ -3296,24 +3317,24 @@
     Parameters
     --------------
     vol_dict : dict
         Dict with the values of the diff minima, output
         of 'diff_minima()'.
     key : str (optional)
         key used to plot just one moment, 'all', 'pre'
-        or 'por'
+        or 'pos'
     color : str (optional)
         color to plot the cloud and the histogram of 
         'all' data
     color_pre : str (optional)
         color to plot the cloud and the histogram of 
-        'pre' data
+        'pre' data, default 'black'
     color_pos : str (optional)
         color to plot the cloud and the histogram of 
-        'pos' data
+        'pos' data, default 'red'
     ax : nd.array (optional)
         the ax position to plot
 
     Returns
     --------------
     None
     """
@@ -3332,14 +3353,15 @@
             ax[0].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
             ax[0].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
             ax[0].set_ylim(0,5)
             ax[0].set_xlim(.5,5.5)
             ax[0].legend()
             
             ax[1].hist(vol_dict[key]['diff'])
+            ax[1].set_xlim(.5,5.5)
             if key == 'all':
                 ax[1].set_title('{} the time'.format(key.capitalize()),fontsize = 17)
             else:
                 ax[1].set_title('{} {} min'.format(key.capitalize(),vol_dict['order'][key]),fontsize = 17)
             ax[1].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
         else:
             out = []
@@ -3382,15 +3404,14 @@
             model.fit(np.asarray(vol_dict['pre']['min']).reshape(len(vol_dict['pre']['min']), 1),
                     np.asarray(vol_dict['pre']['diff']).reshape(len(vol_dict['pre']['diff'])))
 
             ax[0][1].plot(vol_dict['pre']['min'],vol_dict['pre']['diff'],'.',color = color_pre)
             ax[0][1].plot(vol_dict['pre']['min'],model.predict(np.asarray(vol_dict['pre']['min']).reshape(len(vol_dict['pre']['min']), 1)),
                     'gray',label = 'Pre Coef: ' + str(model.coef_[0])[:5])
             ax[0][1].set_title('Pre {} min'.format(vol_dict['order']['pre']),fontsize = 17)
-            ax[0][1].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
             ax[0][1].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
             ax[0][1].set_ylim(0,5)
             ax[0][1].set_xlim(.5,5.5)
             ax[0][1].legend()
 
             ax[1][1].hist(vol_dict['pre']['diff'],color = color_pre)
             ax[1][1].set_title('Pre {} Histogram'.format(vol_dict['order']['pre']),fontsize = 17)
@@ -3421,14 +3442,15 @@
             model.fit(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1),
                     np.asarray(vol_dict['all']['diff']).reshape(len(vol_dict['all']['diff'])))
 
             ax[0][0].plot(vol_dict['all']['min'],vol_dict['all']['diff'],'.',color = color)
             ax[0][0].plot(vol_dict['all']['min'],model.predict(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1)),
                     'gray',label = 'Coef: ' + str(model.coef_[0])[:5])
             ax[0][0].set_title('All the time',fontsize = 17)
+            ax[0][0].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
             ax[0][0].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
             ax[0][0].set_ylim(0,5)
             ax[0][0].set_xlim(.5,5.5)
             ax[0][0].legend()
 
             ax[1][0].hist(vol_dict['all']['diff'],color = color)
             ax[1][0].set_title('All the time Histogram',fontsize = 17)
```

### Comparing `bacteria-0.1.5/bacteria/pipeline.py` & `bacteria-0.1.6/bacteria/pipeline.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.1.5/bacteria.egg-info/PKG-INFO` & `bacteria-0.1.6/bacteria.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.5
+Version: 0.1.6
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.1.5/setup.py` & `bacteria-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.rst", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.1.5',      
+    version = '0.1.6',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/x-rst",
     url = 'https://bacteria.readthedocs.io',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

