# Comparing `tmp/discco-0.2.3.tar.gz` & `tmp/discco-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discco-0.2.3.tar", last modified: Fri Jan 27 10:45:21 2023, max compression
+gzip compressed data, was "discco-0.2.4.tar", last modified: Wed Apr 26 14:34:11 2023, max compression
```

## Comparing `discco-0.2.3.tar` & `discco-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-27 10:45:21.679791 discco-0.2.3/
--rw-r--r--   0 blandt   (743162876) 1934034978    18650 2021-09-23 09:56:26.000000 discco-0.2.3/LICENSE
--rw-r--r--   0 blandt   (743162876) 1934034978     3661 2023-01-27 10:45:21.680025 discco-0.2.3/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978     2865 2023-01-25 17:52:17.000000 discco-0.2.3/README.md
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-27 10:45:21.666127 discco-0.2.3/discco/
--rw-r--r--   0 blandt   (743162876) 1934034978       22 2023-01-24 10:52:48.000000 discco-0.2.3/discco/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978    21243 2023-01-27 10:43:33.000000 discco-0.2.3/discco/discco.py
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-27 10:45:21.678755 discco-0.2.3/discco.egg-info/
--rw-r--r--   0 blandt   (743162876) 1934034978     3661 2023-01-27 10:45:19.000000 discco-0.2.3/discco.egg-info/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      221 2023-01-27 10:45:20.000000 discco-0.2.3/discco.egg-info/SOURCES.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-01-27 10:45:19.000000 discco-0.2.3/discco.egg-info/dependency_links.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       69 2023-01-27 10:45:19.000000 discco-0.2.3/discco.egg-info/requires.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        7 2023-01-27 10:45:19.000000 discco-0.2.3/discco.egg-info/top_level.txt
--rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-01-27 10:45:21.682628 discco-0.2.3/setup.cfg
--rw-r--r--   0 blandt   (743162876) 1934034978      837 2023-01-27 10:44:43.000000 discco-0.2.3/setup.py
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:34:11.505150 discco-0.2.4/
+-rw-r--r--   0 blandt   (743162876) 1934034978    18650 2021-09-23 09:56:26.000000 discco-0.2.4/LICENSE
+-rw-r--r--   0 blandt   (743162876) 1934034978     3776 2023-04-26 14:34:11.505403 discco-0.2.4/PKG-INFO
+-rw-r--r--   0 blandt   (743162876) 1934034978     2927 2023-01-31 12:49:19.000000 discco-0.2.4/README.md
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:34:11.489488 discco-0.2.4/discco/
+-rw-r--r--   0 blandt   (743162876) 1934034978       22 2023-01-24 10:52:48.000000 discco-0.2.4/discco/__init__.py
+-rw-r--r--   0 blandt   (743162876) 1934034978    21470 2023-01-27 22:05:05.000000 discco-0.2.4/discco/discco.py
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:34:11.504119 discco-0.2.4/discco.egg-info/
+-rw-r--r--   0 blandt   (743162876) 1934034978     3776 2023-04-26 14:34:11.000000 discco-0.2.4/discco.egg-info/PKG-INFO
+-rw-r--r--   0 blandt   (743162876) 1934034978      221 2023-04-26 14:34:11.000000 discco-0.2.4/discco.egg-info/SOURCES.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-04-26 14:34:11.000000 discco-0.2.4/discco.egg-info/dependency_links.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978       69 2023-04-26 14:34:11.000000 discco-0.2.4/discco.egg-info/requires.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978        7 2023-04-26 14:34:11.000000 discco-0.2.4/discco.egg-info/top_level.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-04-26 14:34:11.508332 discco-0.2.4/setup.cfg
+-rw-r--r--   0 blandt   (743162876) 1934034978      924 2023-04-26 14:34:03.000000 discco-0.2.4/setup.py
```

### Comparing `discco-0.2.3/LICENSE` & `discco-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `discco-0.2.3/PKG-INFO` & `discco-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: discco
-Version: 0.2.3
+Version: 0.2.4
 Summary: Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images
 Home-page: UNKNOWN
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/discco
 Description: # DISCCo: Differentiable Image Simulation of the Cell Cortex
         
         [![CC BY 4.0][cc-by-shield]][cc-by]
         [![PyPi version](https://badgen.net/pypi/v/discco/)](https://pypi.org/project/discco)
         
         Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images.
         Designed for use on images of PAR proteins in C. elegans zygotes.
         
-        This extends on the segmentation and straightening algorithm described [here](https://github.com/tsmbland/par-segmentation), and uses similar underlying methods.
+        This extends on the segmentation and straightening algorithm described [here](https://github.com/tsmbland/par-segmentation), and uses straightened cortices obtained by that method as input.
         
         ## Methods
         
         Our method is adapted from previous methods that model cross-cortex intensity profiles at each position around the cortex as the sum of distinct cytoplasmic and membrane signal components (Gross et al., 2018; Reich et al., 2019). 
         Typically, these two components are modelled as an error function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension. 
-        In our model we relax these assumptions to account for the possibility of a non-Gaussian PSF and complex light-scattering properties which cannot be captured with these simplistic descriptions. 
+        In our model we relax these assumptions to account for the possibility of a non-Gaussian PSF and complex light-scattering behaviours which cannot be captured with these simplistic descriptions. 
         Instead, cytoplasmic and membrane signal profiles are modelled as arbitrary vectors of length 50 pixels which can take on any shape (s<sub>mem</sub> and s<sub>cyt</sub>). 
         Full straightened images can then be simulated as the addition of two tensor products:
         
         sim = c<sub>cyt</sub> ⊗ s<sub>cyt</sub> + c<sub>mem</sub> ⊗ s<sub>mem</sub>
         
         where c<sub>cyt</sub> and c<sub>mem</sub> are cytoplasmic and membrane concentration profiles.
         Building the model using the differentiable programming language JAX allows input parameters to be iteratively adjusted by backpropagation to minimise the mean squared error between simulated images and ground truth images: 
@@ -35,26 +36,25 @@
         
         In doing so, both the image-specific concentration parameters and the underlying quantification model (i.e. s<sub>mem</sub> and s<sub>cyt</sub>) can be optimised, allowing for closer simulations and more accurate quantification:
         
         <p align="center">
             <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/simulation comparison.png" width="100%" height="100%"/>
         </p>
         
-        For full details of the method, see
+        For full details of the model and training procedures, see
         
         PAPER IN PREP
         
-        ## Installation
-        
-            pip install discco
+        And the accompanying GitHub repository:
         
-        ## Instructions
+        IN PREP
         
-        Binder link (TO DO)
+        ## Installation
         
+            pip install discco
         
         ## License
         
         This work is licensed under a
         [Creative Commons Attribution 4.0 International License][cc-by].
         
         [![CC BY 4.0][cc-by-image]][cc-by]
```

### Comparing `discco-0.2.3/README.md` & `discco-0.2.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 [![PyPi version](https://badgen.net/pypi/v/discco/)](https://pypi.org/project/discco)
 
 Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images.
 Designed for use on images of PAR proteins in C. elegans zygotes.
 
-This extends on the segmentation and straightening algorithm described [here](https://github.com/tsmbland/par-segmentation), and uses similar underlying methods.
+This extends on the segmentation and straightening algorithm described [here](https://github.com/tsmbland/par-segmentation), and uses straightened cortices obtained by that method as input.
 
 ## Methods
 
 Our method is adapted from previous methods that model cross-cortex intensity profiles at each position around the cortex as the sum of distinct cytoplasmic and membrane signal components (Gross et al., 2018; Reich et al., 2019). 
 Typically, these two components are modelled as an error function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension. 
-In our model we relax these assumptions to account for the possibility of a non-Gaussian PSF and complex light-scattering properties which cannot be captured with these simplistic descriptions. 
+In our model we relax these assumptions to account for the possibility of a non-Gaussian PSF and complex light-scattering behaviours which cannot be captured with these simplistic descriptions. 
 Instead, cytoplasmic and membrane signal profiles are modelled as arbitrary vectors of length 50 pixels which can take on any shape (s<sub>mem</sub> and s<sub>cyt</sub>). 
 Full straightened images can then be simulated as the addition of two tensor products:
 
 sim = c<sub>cyt</sub> ⊗ s<sub>cyt</sub> + c<sub>mem</sub> ⊗ s<sub>mem</sub>
 
 where c<sub>cyt</sub> and c<sub>mem</sub> are cytoplasmic and membrane concentration profiles.
 Building the model using the differentiable programming language JAX allows input parameters to be iteratively adjusted by backpropagation to minimise the mean squared error between simulated images and ground truth images: 
@@ -27,26 +27,25 @@
 
 In doing so, both the image-specific concentration parameters and the underlying quantification model (i.e. s<sub>mem</sub> and s<sub>cyt</sub>) can be optimised, allowing for closer simulations and more accurate quantification:
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/simulation comparison.png" width="100%" height="100%"/>
 </p>
 
-For full details of the method, see
+For full details of the model and training procedures, see
 
 PAPER IN PREP
 
-## Installation
-
-    pip install discco
+And the accompanying GitHub repository:
 
-## Instructions
+IN PREP
 
-Binder link (TO DO)
+## Installation
 
+    pip install discco
 
 ## License
 
 This work is licensed under a
 [Creative Commons Attribution 4.0 International License][cc-by].
 
 [![CC BY 4.0][cc-by-image]][cc-by]
```

### Comparing `discco-0.2.3/discco/discco.py` & `discco-0.2.4/discco/discco.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         self.norm_factor = norm_factor
         self.downsampling_rate = pooling_rate
         self.rol_ave = rol_ave
         self.nfits = nfits
 
         # Fitting parameters
         self.zerocap = zerocap
+        self.swish_factor = 30
 
         # Membrane/cytoplasmic reference profile
         self.cytbg = cytbg
         self.membg = membg
         self.sigma = 1.5
 
         # Internal variables for simulations (numpy arrays and tensors)
@@ -88,19 +89,19 @@
     Run
 
     """
 
     def segment(self, freedom=10, roi_knots=20, lr=0.01, descent_steps=500):
 
         # Set up segmenter class
-        iq = ImageQuant(img=self.img, roi=self.roi, periodic=True, thickness=self.thickness, rol_ave=10, rotate=False,
+        iq = ImageQuant(img=self.img, roi=self.roi, periodic=True, thickness=self.thickness, rol_ave=5, rotate=False,
                         nfits=100, iterations=1, lr=lr, descent_steps=descent_steps, adaptive_sigma=False,
                         batch_norm=False, freedom=freedom, roi_knots=roi_knots, fit_outer=True, save_training=False,
                         save_sims=False, method='GD', itp=10, parallel=False, zerocap=False, cores=None,
-                        bg_subtract=False, interp='cubic')
+                        bg_subtract=False, interp='cubic', sigma=3.5)
 
         # Run segmentation
         iq.run()
 
         # Save loss curves
         self.losses = iq.iq.losses
 
@@ -183,15 +184,15 @@
         if save_interim:
             params_interim = {'cyts': [params['cyts_opt'], ], 'mems': [params['mems_opt'], ]}
 
         # Define loss function
         @jax.jit
         def loss_function(_params):
             sim = sim_img_batch(_params['cyts_opt'], _params['mems_opt'], self.cytbg_opt,
-                                self.membg_opt, self.zerocap)
+                                self.membg_opt, self.zerocap, self.swish_factor)
             loss_full = masked_loss_function(sim, self.target, self.masks)
             return jnp.mean(loss_full), loss_full
 
         # Descent steps
         func_grad = jax.grad(loss_function, has_aux=True)
         for e in tqdm(range(descent_steps)):
             # Calculate gradients
@@ -236,15 +237,15 @@
             params_interim = {'cyts': [params['cyts_opt'], ], 'mems': [params['mems_opt'], ],
                               'membg': [params['membg_opt'], ]}
 
         # Define loss function
         @jax.jit
         def loss_function(params):
             sim = sim_img_batch(params['cyts_opt'], params['mems_opt'], self.cytbg_opt,
-                                params['membg_opt'], self.zerocap)
+                                params['membg_opt'], self.zerocap, self.swish_factor)
             loss_full = masked_loss_function(sim, self.target, self.masks)
             return jnp.mean(loss_full), loss_full
 
         # Descent steps
         func_grad = jax.grad(loss_function, has_aux=True)
         for e in tqdm(range(descent_steps)):
             # Calculate gradients
@@ -287,15 +288,15 @@
         if save_interim:
             params_interim = {'cyts': [params['cyts_opt'], ], 'cytbg': [params['cytbg_opt'], ]}
 
         # Define loss function
         @jax.jit
         def loss_function(_params):
             sim = sim_img_batch(_params['cyts_opt'], self.mems_opt, _params['cytbg_opt'],
-                                self.membg_opt, self.zerocap)
+                                self.membg_opt, self.zerocap, self.swish_factor)
             loss_full = masked_loss_function(sim, self.target, self.masks)
             return jnp.mean(loss_full), loss_full
 
         # Descent steps
         func_grad = jax.grad(loss_function, has_aux=True)
         for e in tqdm(range(descent_steps)):
             # Calculate gradients
@@ -423,26 +424,27 @@
     """
     Misc
     
     """
 
     def _store(self):
         # Final simulation
-        self.sim = sim_img_batch(self.cyts_opt, self.mems_opt, self.cytbg_opt, self.membg_opt, zerocap=self.zerocap)
+        self.sim = sim_img_batch(self.cyts_opt, self.mems_opt, self.cytbg_opt, self.membg_opt, zerocap=self.zerocap,
+                                 swish_factor=self.swish_factor)
 
         # Images: remove padded regions and rescale
         self.straight_images = [img.T[mask == 1].T * norm for img, mask, norm in
                                 zip(self.target, self.masks, self.norms)]
         self.straight_images_sim = [img.T[mask == 1].T * norm for img, mask, norm in
                                     zip(self.sim, self.masks, self.norms)]
 
         # Save and rescale quantification results
         if self.zerocap:
-            _m = self.mems_opt * sigmoid(30 * self.mems_opt)
-            _c = self.cyts_opt * sigmoid(30 * self.cyts_opt)
+            _m = self.mems_opt * sigmoid(self.swish_factor * self.mems_opt)
+            _c = self.cyts_opt * sigmoid(self.swish_factor * self.cyts_opt)
             self.mems = [m[mask == 1] * norm for m, mask, norm in zip(_m, self.masks, self.norms)]
             self.cyts = [c * norm * np.ones(int(np.sum(mask))) for c, mask, norm in
                          zip(_c, self.masks, self.norms)]
         else:
             self.mems = [m[mask == 1] * norm for m, mask, norm in zip(self.mems_opt, self.masks, self.norms)]
             self.cyts = [c * norm * np.ones(int(np.sum(mask))) for c, mask, norm in
                          zip(self.cyts_opt, self.masks, self.norms)]
@@ -564,43 +566,43 @@
         else:
             ax.plot(np.log10(self.losses.T))
             ax.set_xlabel('Descent step')
             ax.set_ylabel('log10(Mean square error)')
         return fig, ax
 
 
-def sim_img_batch(cyts, mems, cytbg, membg, zerocap):
+def sim_img_batch(cyts, mems, cytbg, membg, zerocap, swish_factor):
     """
     [nimgs, thickness, nfits]
 
     """
 
     # Cytbg: expand dimensions
     _cytbg = jnp.expand_dims(jnp.expand_dims(cytbg, axis=0), axis=-1)
 
     # Cyts: expand dimensions
     _cyt = jnp.expand_dims(jnp.expand_dims(cyts, axis=-1), axis=-1) * jnp.expand_dims(
         jnp.expand_dims(jnp.ones(mems.shape[1], dtype=jnp.float32), axis=0), axis=0)
 
     # Cytoplasm zerocap
     if zerocap:
-        _cyt *= sigmoid(30 * _cyt)
+        _cyt *= sigmoid(swish_factor * _cyt)
 
     # Cytoplasmic signal contribution
     cyt_total = _cytbg * _cyt
 
     # Membg: expand dimensions
     _membg = jnp.expand_dims(jnp.expand_dims(membg, axis=0), axis=-1)
 
     # Membrane: expand dimensions
     _mem = jnp.expand_dims(mems, axis=1)
 
     # Membrane zerocap
     if zerocap:
-        _mem = _mem * sigmoid(30 * _mem)
+        _mem = _mem * sigmoid(swish_factor * _mem)
 
     # Membrane signal contribution
     mem_total = _membg * _mem
 
     # Sum membrane and cytoplasmic contributions
     return jnp.add(cyt_total, mem_total)
```

### Comparing `discco-0.2.3/discco.egg-info/PKG-INFO` & `discco-0.2.4/discco.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: discco
-Version: 0.2.3
+Version: 0.2.4
 Summary: Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images
 Home-page: UNKNOWN
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/discco
 Description: # DISCCo: Differentiable Image Simulation of the Cell Cortex
         
         [![CC BY 4.0][cc-by-shield]][cc-by]
         [![PyPi version](https://badgen.net/pypi/v/discco/)](https://pypi.org/project/discco)
         
         Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images.
         Designed for use on images of PAR proteins in C. elegans zygotes.
         
-        This extends on the segmentation and straightening algorithm described [here](https://github.com/tsmbland/par-segmentation), and uses similar underlying methods.
+        This extends on the segmentation and straightening algorithm described [here](https://github.com/tsmbland/par-segmentation), and uses straightened cortices obtained by that method as input.
         
         ## Methods
         
         Our method is adapted from previous methods that model cross-cortex intensity profiles at each position around the cortex as the sum of distinct cytoplasmic and membrane signal components (Gross et al., 2018; Reich et al., 2019). 
         Typically, these two components are modelled as an error function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension. 
-        In our model we relax these assumptions to account for the possibility of a non-Gaussian PSF and complex light-scattering properties which cannot be captured with these simplistic descriptions. 
+        In our model we relax these assumptions to account for the possibility of a non-Gaussian PSF and complex light-scattering behaviours which cannot be captured with these simplistic descriptions. 
         Instead, cytoplasmic and membrane signal profiles are modelled as arbitrary vectors of length 50 pixels which can take on any shape (s<sub>mem</sub> and s<sub>cyt</sub>). 
         Full straightened images can then be simulated as the addition of two tensor products:
         
         sim = c<sub>cyt</sub> ⊗ s<sub>cyt</sub> + c<sub>mem</sub> ⊗ s<sub>mem</sub>
         
         where c<sub>cyt</sub> and c<sub>mem</sub> are cytoplasmic and membrane concentration profiles.
         Building the model using the differentiable programming language JAX allows input parameters to be iteratively adjusted by backpropagation to minimise the mean squared error between simulated images and ground truth images: 
@@ -35,26 +36,25 @@
         
         In doing so, both the image-specific concentration parameters and the underlying quantification model (i.e. s<sub>mem</sub> and s<sub>cyt</sub>) can be optimised, allowing for closer simulations and more accurate quantification:
         
         <p align="center">
             <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/simulation comparison.png" width="100%" height="100%"/>
         </p>
         
-        For full details of the method, see
+        For full details of the model and training procedures, see
         
         PAPER IN PREP
         
-        ## Installation
-        
-            pip install discco
+        And the accompanying GitHub repository:
         
-        ## Instructions
+        IN PREP
         
-        Binder link (TO DO)
+        ## Installation
         
+            pip install discco
         
         ## License
         
         This work is licensed under a
         [Creative Commons Attribution 4.0 International License][cc-by].
         
         [![CC BY 4.0][cc-by-image]][cc-by]
```

### Comparing `discco-0.2.3/setup.py` & `discco-0.2.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='discco',
-    version='0.2.3',
+    version='0.2.4',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     install_requires=['numpy',
                       'matplotlib',
                       'pandas',
                       'tqdm',
                       'jax',
                       'optax',
                       'scikit-image',
                       'par-segmentation'],
     description='Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images',
     long_description=long_description,
-    long_description_content_type='text/markdown'
+    long_description_content_type='text/markdown',
+    project_urls={
+        "Source Code": "https://github.com/tsmbland/discco",
+    }
 )
```

