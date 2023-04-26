# Comparing `tmp/h3ppy-0.3.2.tar.gz` & `tmp/h3ppy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h3ppy-0.3.2.tar", last modified: Wed Mar 22 16:09:31 2023, max compression
+gzip compressed data, was "h3ppy-0.4.0.tar", last modified: Wed Apr 26 11:22:08 2023, max compression
```

## Comparing `h3ppy-0.3.2.tar` & `h3ppy-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,18 @@
-drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-03-22 16:09:31.097947 h3ppy-0.3.2/
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)    35149 2023-02-20 18:17:05.000000 h3ppy-0.3.2/LICENSE
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)       75 2023-02-20 18:17:05.000000 h3ppy-0.3.2/MANIFEST.in
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)      776 2023-03-22 16:09:31.097094 h3ppy-0.3.2/PKG-INFO
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)    17017 2023-02-20 18:17:05.000000 h3ppy-0.3.2/README.md
-drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-03-22 16:09:31.076187 h3ppy-0.3.2/h3ppy/
--rwx------   0 hpm5     (18177) _lpoperator   (100)    28048 2023-03-22 15:41:01.000000 h3ppy-0.3.2/h3ppy/__init__.py
-drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-03-22 16:09:31.087185 h3ppy-0.3.2/h3ppy/data/
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)     4367 2023-03-22 15:34:04.000000 h3ppy-0.3.2/h3ppy/data/h2_line_list_roueff_2019_subset.txt
--rwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)   107921 2023-02-20 18:17:05.000000 h3ppy-0.3.2/h3ppy/data/h3p_line_list_neale_1996_subset.txt
-drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-03-22 16:09:31.095424 h3ppy-0.3.2/h3ppy/h3ppy.egg-info/
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        0 2023-03-22 15:52:11.000000 h3ppy-0.3.2/h3ppy/h3ppy.egg-info/SOURCES.txt
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        1 2023-03-22 15:52:11.000000 h3ppy-0.3.2/h3ppy/h3ppy.egg-info/dependency_links.txt
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        6 2023-03-22 15:52:11.000000 h3ppy-0.3.2/h3ppy/h3ppy.egg-info/requires.txt
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        6 2023-03-22 15:52:11.000000 h3ppy-0.3.2/h3ppy/h3ppy.egg-info/top_level.txt
-drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-03-22 16:09:31.083209 h3ppy-0.3.2/h3ppy.egg-info/
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)      776 2023-03-22 16:09:30.000000 h3ppy-0.3.2/h3ppy.egg-info/PKG-INFO
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)      458 2023-03-22 16:09:30.000000 h3ppy-0.3.2/h3ppy.egg-info/SOURCES.txt
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        1 2023-03-22 16:09:30.000000 h3ppy-0.3.2/h3ppy.egg-info/dependency_links.txt
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        6 2023-03-22 16:09:30.000000 h3ppy-0.3.2/h3ppy.egg-info/requires.txt
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        6 2023-03-22 16:09:30.000000 h3ppy-0.3.2/h3ppy.egg-info/top_level.txt
--rw-r--r--   0 hpm5     (18177) _lpoperator   (100)       38 2023-03-22 16:09:31.098196 h3ppy-0.3.2/setup.cfg
--rwx------   0 hpm5     (18177) _lpoperator   (100)     2319 2023-03-22 15:58:14.000000 h3ppy-0.3.2/setup.py
+drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-04-26 11:22:08.951875 h3ppy-0.4.0/
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)    35149 2023-04-26 11:15:41.000000 h3ppy-0.4.0/LICENSE
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)       75 2023-04-26 11:15:41.000000 h3ppy-0.4.0/MANIFEST.in
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)      812 2023-04-26 11:22:08.950665 h3ppy-0.4.0/PKG-INFO
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)    17036 2023-04-26 11:15:41.000000 h3ppy-0.4.0/README.md
+drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-04-26 11:22:08.932927 h3ppy-0.4.0/h3ppy/
+-rwx------   0 hpm5     (18177) _lpoperator   (100)    29332 2023-04-26 10:44:15.000000 h3ppy-0.4.0/h3ppy/__init__.py
+drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-04-26 11:22:08.948377 h3ppy-0.4.0/h3ppy/data/
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)     4367 2023-04-26 11:15:41.000000 h3ppy-0.4.0/h3ppy/data/h2_line_list_roueff_2019_subset.txt
+-rwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)   107921 2023-04-26 11:15:41.000000 h3ppy-0.4.0/h3ppy/data/h3p_line_list_neale_1996_subset.txt
+drwxr-xr-x   0 hpm5     (18177) _lpoperator   (100)        0 2023-04-26 11:22:08.943767 h3ppy-0.4.0/h3ppy.egg-info/
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)      812 2023-04-26 11:22:07.000000 h3ppy-0.4.0/h3ppy.egg-info/PKG-INFO
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)      314 2023-04-26 11:22:08.000000 h3ppy-0.4.0/h3ppy.egg-info/SOURCES.txt
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        1 2023-04-26 11:22:07.000000 h3ppy-0.4.0/h3ppy.egg-info/dependency_links.txt
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        6 2023-04-26 11:22:08.000000 h3ppy-0.4.0/h3ppy.egg-info/requires.txt
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)        6 2023-04-26 11:22:08.000000 h3ppy-0.4.0/h3ppy.egg-info/top_level.txt
+-rw-r--r--   0 hpm5     (18177) _lpoperator   (100)       38 2023-04-26 11:22:08.952210 h3ppy-0.4.0/setup.cfg
+-rwx------   0 hpm5     (18177) _lpoperator   (100)     2319 2023-04-26 08:25:09.000000 h3ppy-0.4.0/setup.py
```

### Comparing `h3ppy-0.3.2/LICENSE` & `h3ppy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `h3ppy-0.3.2/PKG-INFO` & `h3ppy-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: h3ppy
-Version: 0.3.2
+Version: 0.4.0
 Summary: Model and fit H3+ and H2 spectra
 Home-page: https://github.com/henrikmelin/h3ppy
 Author: Henrik Melin
 Author-email: h.melin@gmail.com
+License: UNKNOWN
 Keywords: infrared spectroscopy H3+ modelling
+Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,7 +23,8 @@
 ## Install via pip
 ```
 pip3 install h3ppy
 ```
 
 Full [documentation on Github](https://github.com/henrikmelin/h3ppy).
     
+
```

### Comparing `h3ppy-0.3.2/README.md` & `h3ppy-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # h3ppy 😁
 
-A python package for modelling and fitting H<sub>3</sub><sup>+</sup> and H<sub>2</sub> spectra, pronounced heppy (perhaps). Great! 
+A python package for modelling and fitting H<sub>3</sub><sup>+</sup> and H<sub>2</sub> spectra, pronounced "happy". Great! 
 
 ## Install via pip
 ```
 pip3 install h3ppy
 ```
 Or to upgrade to the latest greatest version: 
 ```
@@ -352,18 +352,18 @@
 
 
 # Input parameters
 
 The `set()`, `model()`, and `fit()` methods accepts the following inputs:
 
 
-* `wavelength` - the wavelength scale on which to produce the model
+* `wavelength`, `wave`, `w` - the wavelength scale on which to produce the model.  
 * `data` - the observed H<sub>3</sub><sup>+</sup> spectrum
-* `temperature` - the intensity of the H<sub>3</sub><sup>+</sup> spectral lines are an exponential function of the temperature. Typical ranges for the ionosphere's of the giant planets are 400 (Saturn) to 1500 K (Jupiter).
-* `density` - the column integrated H<sub>3</sub><sup>+</sup> density, this is the number of ions along the line of sight vector.
+* `temperature`, `T` - the intensity of the H<sub>3</sub><sup>+</sup> spectral lines are an exponential function of the temperature. Typical ranges for the ionosphere's of the giant planets are 400 (Saturn) to 1500 K (Jupiter). 
+* `density`, `N` - the column integrated H<sub>3</sub><sup>+</sup> density, this is the number of ions along the line of sight vector.
 * `sigma_n` - the _n_th polynomial constant of the spectral line width (sigma)
 * `offset_n` - the _n_th polynomial constant of the wavelength offset from the rest wavelength. Doppler shift and wavelength calibration errors can offset the wavelength scale. 
 * `background_n` - he _n_th polynomial constant of the displacement from the zero intensity level of the spectrum
 * `nsigma` - the number of polynomial constant used for the sigma.
 * `noffset` - the number of polynomial constant used for the offset.
 * `nbackground` - the number of polynomial constant used for the background.
```

### Comparing `h3ppy-0.3.2/h3ppy/__init__.py` & `h3ppy-0.4.0/h3ppy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 import numpy as np
 import logging
 
 class h3p :
 
     def __init__(self, line_list_file = '', **kwargs):
 
-
         # Provide the opportunity to use another line list
         if (line_list_file == '') :
             self.line_list_file = os.path.join(os.path.dirname(__file__), 'data/h3p_line_list_neale_1996_subset.txt')
         else : self.line_list_file = line_list_file
 
         # Set up required parameters
         self.startup()
 
         # Parse any potential input
         self.parse_kwargs(kwargs)
 
-
     def startup(self) : 
 
         # We'll work with double precision
         self.dtype = 'double'
 
         # Configure logging
         logging.basicConfig(format='[h3ppy] %(message)s', datefmt='%m/%d/%Y %I:%M:%S %p', level=logging.INFO)
@@ -75,23 +73,26 @@
         ret = np.zeros(len(self.wavelength))
         for k in range(nbr) :
             key = pname + '_' + str(k)
             ret += self.vars[key] * np.power(self.wavelength, k)
         return ret
 
 
-    def calculate_line_intensities(self) :
+    def calculate_line_intensities(self, **kwargs) :
         '''
             Calculate the individual line intensities at a particlar temperature.
 
                   g*(2J'+1)*hcw*exp(-hcw'/kT)*A(if)
             E(w)= --------------------------------
                                  4Pi*Q
 
         '''
+        
+        self.parse_kwargs(kwargs)
+
         # Don't recalculate if we've just done it
         if (self._last_temperature == self.vars['temperature']) :
             return self.line_intensity
 
         Q = self.Q()
 
         exponent   = ( -1.0 * self.line_data['wu'] *  self.h *  self.c * 100.0 ) / ( self.k * self.vars['temperature'])
@@ -102,15 +103,15 @@
         self.line_intensity = intensity
         self._last_temperature = self.vars['temperature']
 
         return self.line_intensity
 
     def model(self, **kwargs) :
         '''
-            Generate a H3+ spectral model based on the provided parameters.
+            Generate a spectral model based on the provided parameters.
 
         '''
         self.parse_kwargs(kwargs)
 
         line_intensity = self.calculate_line_intensities()
 
         self.background = self.poly_fn('background', self.nbackground)
@@ -124,14 +125,31 @@
 
         spectrum   = np.zeros(len(self.wavelength), dtype = self.dtype)
 
         self.sigma      = self.poly_fn('sigma', self.nsigma)
         self.offset     = self.poly_fn('offset', self.noffset)
         self.background = self.poly_fn('background', self.nbackground)
 
+        # Calculate the contribution for all lines in the line-list at each wavelength
+        for i, w in enumerate(self.wavelength) : 
+            exponent     = -1.0 * np.power(self.wavelength[i] - ( 1e4/self.line_data['wl'] + self.offset[i]), 2) / (2.0 * np.power(self.sigma[i], 2))
+            self.line_contributions = line_intensity / ( self.sigma[i] * np.sqrt(2 * np.pi) ) * np.exp(exponent)
+
+            # The sum of all the individual contributions is the spectrun at each spectral pixel
+
+            # We can process the spectrum by adding additional terms,
+            # used mainly for the derivaties of the spectral function.
+            if (process_fn == '') : spectrum[i] = np.sum(self.line_contributions)
+            else : spectrum[i] = np.sum(getattr(self, process_fn)(i))
+
+        return spectrum
+
+        # How does this change the derivatives? 
+
+
         relevant_range = np.max(self.sigma) * self.sigma_limit
 
         # Iterate over the H3+ spectral lines
         for k in np.arange(len(self.line_data['wl'])) :
 
             # Only calculate over the wavelength range appropriate for this line
             relevant_waves = np.argwhere(np.abs(self.wavelength - (1e4/self.line_data['wl'][k] + np.mean(self.offset))) < relevant_range)
@@ -192,63 +210,61 @@
             vardQdT += float(i) * const * np.power(self.vars['temperature'], float(i - 1))
         return vardQdT
 
     # The tempoerature derivative of the spectral function
     def dIdT(self) :
 
         line_intensity = self.calculate_line_intensities()
-        dIidT          = np.zeros(len(self.line_data['wl']))
 
         const1 =  self.h *  self.c * 100 / ( np.power(self.vars['temperature'], 2) *  self.k )
         Q      = self.Q()
         dQdT   = self.dQdT()
 
-        # Iterate over the H3+ spectral lines
-        for k in np.arange(len(self.line_data['wl'])) :
-            dIidT[k]  = line_intensity[k] * const1 * self.line_data['wu'][k]
-            dIidT[k] -= line_intensity[k] * dQdT     / Q
+        # Caulcate the derivative for each transtion in the line-list
+        dIidT  = line_intensity * const1 * self.line_data['wu']
+        dIidT -= line_intensity * dQdT / Q
 
         return self.render_spectrum(dIidT) * self.vars['density']
 
     # The wavelength polynomial constants derivative of the spectral function I
     def dIdo(self, index) :
 
         line_intensity = self.calculate_line_intensities()
 
         self.offset_index = index
         return self.render_spectrum(line_intensity, process_fn = 'dIdo_process') * self.vars['density']
 
     # Alter the spectral function for dIdo()
-    def dIdo_process(self, i, k) :
+    def dIdo_process(self, i) :
 
-        numerator_deriv = 2.0 * ( self.wavelength[i] - (1e4/self.line_data['wl'][k] + self.offset[i]) )
+        numerator_deriv = 2.0 * ( self.wavelength[i] - (1e4/self.line_data['wl'] + self.offset[i]) )
         dIdc            = 1.0 * np.power(self.wavelength[i], self.offset_index)
 
-        return self.intensity_ik * numerator_deriv / (2.0 * np.power(self.sigma[i], 2)) * dIdc
+        return self.line_contributions * numerator_deriv / (2.0 * np.power(self.sigma[i], 2)) * dIdc
 
     # The line width derivative of the spectral function I
     def dIds(self, index) :
         line_intensity = self.calculate_line_intensities()
 
         self.sigma_index = index
         return  self.render_spectrum(line_intensity, process_fn = 'dIds_process') * self.vars['density']
 
     # Alter the spectral function for dIds()
-    def dIds_process(self, i, k) :
+    def dIds_process(self, i) :
 
         # The exponent in the spectral function
-        exponent_numerator  = -1.0 * np.power(self.wavelength[i] - ( 1e4/self.line_data['wl'][k] + self.offset[i]), 2)
+        exponent_numerator  = -1.0 * np.power(self.wavelength[i] - ( 1e4/self.line_data['wl'] + self.offset[i]), 2)
 
         # The derivative of the exponent denominator
         dIds = -2.0 * exponent_numerator / (2.0 * np.power(self.sigma[i], 3))
 
         # The derivative of the sigma function polynmomial functions
         dsdc = np.power(self.wavelength[i], self.sigma_index)
 
-        return ( self.intensity_ik * dIds - 1.0 * self.intensity_ik / self.sigma[i]) * dsdc
+        return ( self.line_contributions * dIds - 1.0 * self.line_contributions / self.sigma[i]) * dsdc
 
     # The derivative of the background polynomial constants
     def dIdb(self, index) :
         return np.power(self.wavelength, index)
 
     # The partial derivative of the column density
     def dIdN(self) :
@@ -275,15 +291,15 @@
 
         # Add polynomial terms, and set them to zero
         elif (nnew > nold) :
             for i in range(nold, nnew) :
                 key = var + '_' + str(i)
                 self.vars[key] = 0.0
 
-    # Parse the kewyord input
+    # Parse the keyword input
     def parse_kwargs(self, kwargs) :
 
         # Prioritise processing the n variables, that deterime the number of
         # polynomial terms to use for sigma, offset, and backround.
         for key, value in kwargs.items() :
 
             if (key == 'nsigma') :
@@ -456,14 +472,26 @@
         for p, param in enumerate(self.params_to_fit) :
             Zpp = np.delete(np.delete(Z, p, 0), p, 1)
             self.errors[param] = mu / np.sqrt(np.linalg.det(Z)  / np.linalg.det(Zpp) )
 
         return self.model()
 
 
+    def reset_params(self) : 
+        '''
+        Reset all the parameters to sensible values. 
+        '''
+        for key in self.vars.keys() : 
+            self.var[key] = 0.0
+
+        self.vars['temperature']   = 1000
+        self.vars['density']       = 1.0
+
+
+
     def wavegen(self, wstart, wend, wnbr) :
         '''
         Generate a wavelength scale using start and end wavelengths and the number of wavelength elements.
         '''
         res = (wend - wstart) / float(wnbr)
         self.wavelength = np.arange(wstart, wend, res)
         return self.wavelength
@@ -619,20 +647,20 @@
         self.set(offset = offset_guess)
 
         return self.model()
 
     def check_inputs(self) :
 
         # We need to have some data to guess on
-        if (len(self.data) == 1) :
+        if (self.data.shape[0] < 2) :
             logging.error('ERROR - Data array is required at this stage! E.g. h3p.fit(data = uranus)')
             return False
 
         # Santiy check the inputs
-        if (len(self.data) != len(self.wavelength)) :
+        if (self.data.shape[0] != self.wavelength.shape[0]) :
             logging.error('ERROR - The wavelength array has a different length to the data array! ({nd} and {nw})').format(nd = len(self.data), nw = len(self.wavelength))
             return False
 
 
         return True
 
     def get_rest_wavelength(self) :
@@ -653,24 +681,24 @@
             * percent  - The percentage of the maximum model value of the noise           
         '''    
 
         # Generate a model
         model = self.model()
 
         # Calculate the noise scaling depending on the input
-        if (snr > 0) : scale = np.max(self.model) / snr
+        if (snr > 0) : scale = np.max(model) / snr / 2.0
         elif (absolute > 0) : scale = absolute
         elif (percent > 0) : scale = np.max(model) * percent / 100.0
         else : scale = 0.1 * np.max(model)
 
         # Generate the noise        
-        noise = np.random.normal(size = self.wavelength.size, scale = scale) 
+        noise = np.random.normal(size = self.wavelength.size, scale = scale).flatten()
 
         # Add the noise to the model
-        return ( model + noise )
+        return model + noise 
     
     
     
     
 class h2(h3p) : 
 
     def __init__(self, line_list_file = '', **kwargs):
@@ -685,23 +713,26 @@
 
         # Parse any potential input
         self.parse_kwargs(kwargs)
 
 
     # Simple polynomial fit to the Roueff 2019 partiation function on ExoMol
     def Q_constants(self) :
-        return [1.8141538490481226e-06, 0.021686851296966323, 1.0748323788171947]
+        return [ 9.97306739e-10, -1.28235186e-06,  2.43332479e-02,  5.47921938e-01]
     
     def Q(self, **kwargs) :
         self.parse_kwargs(kwargs)
 
         consts = self.Q_constants() 
         Q = consts[0] * self.vars['temperature']**2 + consts[1] * self.vars['temperature'] + consts[2]
         return Q
 
     def dQdT(self) : 
         consts = self.Q_constants() 
         dQdT = 0.5 * consts[0] * self.vars['temperature'] + consts[1]  # * self.vars['temperature'] + consts[2]
         return dQdT    
     
-    
-        
+    def total_emission(self, **kwargs) : 
+        self.parse_kwargs(kwargs)
+
+        # Return the wavelength integrated radiance
+        return np.sum(self.calculate_line_intensities()) * self.vars['density']
```

### Comparing `h3ppy-0.3.2/h3ppy/data/h2_line_list_roueff_2019_subset.txt` & `h3ppy-0.4.0/h3ppy/data/h2_line_list_roueff_2019_subset.txt`

 * *Files identical despite different names*

### Comparing `h3ppy-0.3.2/h3ppy/data/h3p_line_list_neale_1996_subset.txt` & `h3ppy-0.4.0/h3ppy/data/h3p_line_list_neale_1996_subset.txt`

 * *Files identical despite different names*

### Comparing `h3ppy-0.3.2/h3ppy.egg-info/PKG-INFO` & `h3ppy-0.4.0/h3ppy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: h3ppy
-Version: 0.3.2
+Version: 0.4.0
 Summary: Model and fit H3+ and H2 spectra
 Home-page: https://github.com/henrikmelin/h3ppy
 Author: Henrik Melin
 Author-email: h.melin@gmail.com
+License: UNKNOWN
 Keywords: infrared spectroscopy H3+ modelling
+Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,7 +23,8 @@
 ## Install via pip
 ```
 pip3 install h3ppy
 ```
 
 Full [documentation on Github](https://github.com/henrikmelin/h3ppy).
     
+
```

### Comparing `h3ppy-0.3.2/setup.py` & `h3ppy-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 SOFTWARE.
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name             = 'h3ppy',
-    version          = '0.3.2',
+    version          = '0.4.0',
     author           = 'Henrik Melin',
     author_email     = 'h.melin@gmail.com',
     description      = 'Model and fit H3+ and H2 spectra',
     url              = 'https://github.com/henrikmelin/h3ppy',
     keywords         = 'infrared spectroscopy H3+ modelling',
     packages         = find_packages(),
     install_requires = ['numpy'],
```

