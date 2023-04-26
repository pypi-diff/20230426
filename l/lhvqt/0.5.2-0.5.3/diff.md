# Comparing `tmp/lhvqt-0.5.2.tar.gz` & `tmp/lhvqt-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lhvqt-0.5.2.tar", last modified: Fri Nov  5 02:17:52 2021, max compression
+gzip compressed data, was "lhvqt-0.5.3.tar", last modified: Wed Apr 26 14:26:13 2023, max compression
```

## Comparing `lhvqt-0.5.2.tar` & `lhvqt-0.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2021-11-05 02:17:52.062142 lhvqt-0.5.2/
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1072 2021-09-14 12:18:55.000000 lhvqt-0.5.2/LICENSE.txt
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     2374 2021-11-05 02:17:52.062142 lhvqt-0.5.2/PKG-INFO
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     2007 2021-09-14 12:18:55.000000 lhvqt-0.5.2/README.md
-drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2021-11-05 02:17:52.062142 lhvqt-0.5.2/lhvqt/
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      190 2021-09-14 12:18:55.000000 lhvqt-0.5.2/lhvqt/__init__.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     6119 2021-09-14 12:18:55.000000 lhvqt-0.5.2/lhvqt/lhvqt.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     4528 2021-10-29 17:06:39.000000 lhvqt-0.5.2/lhvqt/lhvqt_comb.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    32761 2021-11-05 02:05:13.000000 lhvqt-0.5.2/lhvqt/lvqt.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     3631 2021-09-14 12:18:55.000000 lhvqt-0.5.2/lhvqt/lvqt_hilb.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     4646 2021-09-14 12:18:55.000000 lhvqt-0.5.2/lhvqt/lvqt_orig.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     3401 2021-09-14 12:18:55.000000 lhvqt-0.5.2/lhvqt/lvqt_real.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     7801 2021-09-14 12:18:55.000000 lhvqt-0.5.2/lhvqt/utils.py
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     4997 2021-09-14 12:34:37.000000 lhvqt-0.5.2/lhvqt/variational.py
-drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2021-11-05 02:17:52.062142 lhvqt-0.5.2/lhvqt.egg-info/
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     2374 2021-11-05 02:17:52.000000 lhvqt-0.5.2/lhvqt.egg-info/PKG-INFO
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      334 2021-11-05 02:17:52.000000 lhvqt-0.5.2/lhvqt.egg-info/SOURCES.txt
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)        1 2021-11-05 02:17:52.000000 lhvqt-0.5.2/lhvqt.egg-info/dependency_links.txt
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)       41 2021-11-05 02:17:52.000000 lhvqt-0.5.2/lhvqt.egg-info/requires.txt
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)        6 2021-11-05 02:17:52.000000 lhvqt-0.5.2/lhvqt.egg-info/top_level.txt
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)       38 2021-11-05 02:17:52.062142 lhvqt-0.5.2/setup.cfg
--rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      648 2021-11-05 02:12:14.000000 lhvqt-0.5.2/setup.py
+drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2023-04-26 14:26:13.272448 lhvqt-0.5.3/
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     1072 2023-03-18 15:35:41.000000 lhvqt-0.5.3/LICENSE.txt
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     2393 2023-04-26 14:26:13.272448 lhvqt-0.5.3/PKG-INFO
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     2046 2023-03-18 15:35:41.000000 lhvqt-0.5.3/README.md
+drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2023-04-26 14:26:13.268448 lhvqt-0.5.3/lhvqt/
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      190 2023-03-18 15:35:41.000000 lhvqt-0.5.3/lhvqt/__init__.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     6119 2023-03-18 15:35:41.000000 lhvqt-0.5.3/lhvqt/lhvqt.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     4528 2023-03-18 15:35:41.000000 lhvqt-0.5.3/lhvqt/lhvqt_comb.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)    32761 2023-03-18 15:35:41.000000 lhvqt-0.5.3/lhvqt/lvqt.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     3631 2023-03-18 15:35:41.000000 lhvqt-0.5.3/lhvqt/lvqt_hilb.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     4646 2023-03-18 15:35:41.000000 lhvqt-0.5.3/lhvqt/lvqt_orig.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     3401 2023-03-18 15:35:41.000000 lhvqt-0.5.3/lhvqt/lvqt_real.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     7115 2023-04-25 16:53:24.000000 lhvqt-0.5.3/lhvqt/utils.py
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     4997 2023-03-18 15:35:41.000000 lhvqt-0.5.3/lhvqt/variational.py
+drwxrwxr-x   0 rockstar  (1000) rockstar  (1000)        0 2023-04-26 14:26:13.272448 lhvqt-0.5.3/lhvqt.egg-info/
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)     2393 2023-04-26 14:26:13.000000 lhvqt-0.5.3/lhvqt.egg-info/PKG-INFO
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      334 2023-04-26 14:26:13.000000 lhvqt-0.5.3/lhvqt.egg-info/SOURCES.txt
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)        1 2023-04-26 14:26:13.000000 lhvqt-0.5.3/lhvqt.egg-info/dependency_links.txt
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)       41 2023-04-26 14:26:13.000000 lhvqt-0.5.3/lhvqt.egg-info/requires.txt
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)        6 2023-04-26 14:26:13.000000 lhvqt-0.5.3/lhvqt.egg-info/top_level.txt
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)       38 2023-04-26 14:26:13.272448 lhvqt-0.5.3/setup.cfg
+-rw-rw-r--   0 rockstar  (1000) rockstar  (1000)      648 2023-04-26 14:08:03.000000 lhvqt-0.5.3/setup.py
```

### Comparing `lhvqt-0.5.2/LICENSE.txt` & `lhvqt-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lhvqt-0.5.2/PKG-INFO` & `lhvqt-0.5.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: lhvqt
-Version: 0.5.2
+Version: 0.5.3
 Summary: Frontend filterbank learning module with HVQT initialization capabilities
 Home-page: https://github.com/cwitkowitz/LHVQT
 Author: Frank Cwitkowitz
 Author-email: fcwitkow@ur.rochester.edu
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Learnable Harmonic Variable-Q Transform (LHVQT)
 Implements a frontend filterbank learning module which can be initialized with complex weights for a Variable-Q Transform (lvqt_orig.py). Several techniques and variations of the module are also implemented, including:
  - Multi-channel (harmonic) structure (lhvqt.py)
@@ -38,28 +37,26 @@
 
 # Usage
 Several examples of instantiation, inference, and visualization are provided under the ```examples``` sub-directory. A full-blown training, visualization, and evaluation example for piano transcription can be found at https://github.com/cwitkowitz/sparse-analytic-filters.
 
 ## Cite
 Please cite whichever is more relevant to your usage.
 
-##### arXiv Paper
+##### SMC 2022 Paper
 ```
-@article{cwitkowitz2021learning,
-  author  = {Frank Cwitkowitz and Mojtaba Heydari and Zhiyao Duan},
-  title   = {Learning Sparse Analytic Filters for Piano Transcription},
-  journal = {arXiv preprint arXiv:2108.10382},
-  year    = {2021}
+@inproceedings{cwitkowitz2022learning,
+  title     = {Learning Sparse Analytic Filters for Piano Transcription},
+  author    = {Frank Cwitkowitz and Mojtaba Heydari and Zhiyao Duan},
+  year      = 2022,
+  booktitle = {Proceedings of Sound and Music Computing Conference (SMC)}
 }
 ```
 
 ##### Master's Thesis
 ```
 @mastersthesis{cwitkowitz2019end,
-  author  = {Cwitkowitz, Frank},
   title   = {End-to-End Music Transcription Using Fine-Tuned Variable-{Q} Filterbanks},
-  school  = {Rochester Institute of Technology},
-  year    = {2019}
+  author  = {Cwitkowitz, Frank},
+  year    = 2019,
+  school  = {Rochester Institute of Technology}
 }
 ```
-
-
```

### Comparing `lhvqt-0.5.2/README.md` & `lhvqt-0.5.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,26 +25,26 @@
 
 # Usage
 Several examples of instantiation, inference, and visualization are provided under the ```examples``` sub-directory. A full-blown training, visualization, and evaluation example for piano transcription can be found at https://github.com/cwitkowitz/sparse-analytic-filters.
 
 ## Cite
 Please cite whichever is more relevant to your usage.
 
-##### arXiv Paper
+##### SMC 2022 Paper
 ```
-@article{cwitkowitz2021learning,
-  author  = {Frank Cwitkowitz and Mojtaba Heydari and Zhiyao Duan},
-  title   = {Learning Sparse Analytic Filters for Piano Transcription},
-  journal = {arXiv preprint arXiv:2108.10382},
-  year    = {2021}
+@inproceedings{cwitkowitz2022learning,
+  title     = {Learning Sparse Analytic Filters for Piano Transcription},
+  author    = {Frank Cwitkowitz and Mojtaba Heydari and Zhiyao Duan},
+  year      = 2022,
+  booktitle = {Proceedings of Sound and Music Computing Conference (SMC)}
 }
 ```
 
 ##### Master's Thesis
 ```
 @mastersthesis{cwitkowitz2019end,
-  author  = {Cwitkowitz, Frank},
   title   = {End-to-End Music Transcription Using Fine-Tuned Variable-{Q} Filterbanks},
-  school  = {Rochester Institute of Technology},
-  year    = {2019}
+  author  = {Cwitkowitz, Frank},
+  year    = 2019,
+  school  = {Rochester Institute of Technology}
 }
 ```
```

### Comparing `lhvqt-0.5.2/lhvqt/lhvqt.py` & `lhvqt-0.5.3/lhvqt/lhvqt.py`

 * *Files identical despite different names*

### Comparing `lhvqt-0.5.2/lhvqt/lhvqt_comb.py` & `lhvqt-0.5.3/lhvqt/lhvqt_comb.py`

 * *Files identical despite different names*

### Comparing `lhvqt-0.5.2/lhvqt/lvqt.py` & `lhvqt-0.5.3/lhvqt/lvqt.py`

 * *Files identical despite different names*

### Comparing `lhvqt-0.5.2/lhvqt/lvqt_hilb.py` & `lhvqt-0.5.3/lhvqt/lvqt_hilb.py`

 * *Files identical despite different names*

### Comparing `lhvqt-0.5.2/lhvqt/lvqt_orig.py` & `lhvqt-0.5.3/lhvqt/lvqt_orig.py`

 * *Files identical despite different names*

### Comparing `lhvqt-0.5.2/lhvqt/lvqt_real.py` & `lhvqt-0.5.3/lhvqt/lvqt_real.py`

 * *Files identical despite different names*

### Comparing `lhvqt-0.5.2/lhvqt/utils.py` & `lhvqt-0.5.3/lhvqt/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,91 +4,77 @@
 import numpy as np
 import librosa
 import torch
 
 EPSILON = torch.finfo(torch.float32).eps
 
 
-def torch_amplitude_to_db(feats, amin=1e-10, top_db=80.0, to_prob=False):
+def torch_amplitude_to_db(feats, amin=1e-5, top_db=80.0, to_prob=False):
     """
-    Take the log of a time-frequency representation with differentiable
-    PyTorch functions, scaling values to be between 0 and 1. Adapted from
-    the Librosa amplitude_to_db function.
+    Convert amplitude features to decibels or probability-like
+    values sample-wise with differentiable PyTorch functions.
+
+    Adapted from the Librosa amplitude_to_db function.
 
     Parameters
     ----------
     feats : Tensor (B x H x F x T) or (B x F x T)
-      Set of amplitude features,
+      Set of magnitude of amplitude features,
       B - batch size
       H - number of harmonics (a.k.a. channels)
       F - dimensionality of features
       T - number of time steps (frames)
     amin : float
-      Minimum amplitude possible within a time-frequency bin
+      Threshold for minimum amplitude
     top_db : float
-      Maximum difference from dB ceiling (defines dB floor)
+      Maximum difference from dB ceiling
     to_prob : bool
-      Scale decibel values to be between 0 and 1
+      Convert decibels to probability-like features
 
     Returns
     ----------
-    log_feats : Tensor (B x H x F x T) or (B x F x T)
-      Set of dB or probability features
+    decibels : Tensor (B x H x F x T) or (B x F x T)
+      Set of decibel or probability-like features
     """
 
-    # Perform processing on a copy of original features
-    feats_copy = feats.clone()
+    # Determine the number of samples in the batch
+    B = feats.size(0)
+
+    # Make sure the features represent magnitude
+    magnitude = torch.abs(feats.clone())
+
+    # Convert magnitude to power
+    power = torch.square(magnitude)
+
+    # Get reference values for each sample in the batch
+    ref_values = power.reshape(B, -1).max(dim=-1)[0]
+
+    # Add dimensions to reference values for broadcasting
+    ref_values = ref_values.view((-1,) + tuple([1] * (len(feats.shape) - 1)))
 
-    # Get handles for the feature dimensionality
-    B, H, F, T = feats.size(0), 1, feats.size(-2), feats.size(-1)
+    # Convert threshold to power
+    amin = torch.tensor(amin) ** 2
 
-    # Collapse the channel dimension if it exists
-    if len(feats.size()) > 3:
-        H = feats.size(1)
-        feats_copy = feats_copy.view(B * H, F, T)
-
-    # Get handle for pseudo batch size
-    PB = B * H
-
-    # Convert amplitude features to power
-    power = torch.abs(feats_copy) ** 2
-
-    # Get reference values (maximums) from power spectrogram for each 2D transform
-    ref_value = torch.max(power.view(PB, -1), dim=-1)[0]
-
-    # Clamp power spectrogram at specified minimum - effectively max(amin, power)
-    power[power < amin] = amin
-
-    # Convert power to dB
-    log_feats = 10.0 * torch.log10(power)
-
-    # Make sure reference values are above minimum amplitude
-    amin = torch.Tensor([amin] * PB).to(power.device)
-    amin[amin < ref_value] = ref_value[amin < ref_value]
-    # Add dimensions for broadcasting
-    amin = amin.unsqueeze(-1).unsqueeze(-1)
-
-    # Combined with previous log, we are performing 10 * log10(power / ref)
-    log_feats = log_feats - 10.0 * torch.log10(amin)
-
-    # Collapse the last two dimensions temporarily to make the following easier
-    log_feats = log_feats.view(PB, -1)
-    # Determine the dB floor for each 2D transform
-    dB_floor = (torch.max(log_feats, dim=-1)[0] - top_db).unsqueeze(-1)
-    # Clamp the values at the specified dB floor
-    log_feats[log_feats < dB_floor] = dB_floor.repeat(1, F * T)[log_feats < dB_floor]
+    # Convert power to dB, clamping power at specified threshold
+    log_feats = 10.0 * torch.log10(torch.maximum(amin, power))
+
+    # Combine with previous operation to perform 10 * log10(power / ref)
+    log_feats -= 10.0 * torch.log10(torch.maximum(amin, ref_values))
+
+    # Clamp all decibels at the corresponding floor
+    decibels = torch.maximum(log_feats, -torch.tensor(top_db))
+
+    # Make sure features for silence are at decibel floor
+    decibels[ref_values.squeeze() == 0.] = -top_db
 
     if to_prob:
         # Scale values and offset to be between 0 and 1
-        log_feats = (log_feats / top_db) + 1.0
-
-    # Reshape the log-scaled features using the original feature dimensions
-    log_feats = log_feats.view(feats.size())
+        decibels = (decibels / top_db) + 1.0
 
-    return log_feats
+    return decibels
 
 
 def torch_hilbert(x_real, n_fft=None):
     """
     Obtain imaginary counterpart to a real signal such that there are no negative frequency
     components when represented as a complex signal. This is done by using the Hilbert transform.
     We end up with an analytic signal and return only the imaginary part. Most importantly,
```

### Comparing `lhvqt-0.5.2/lhvqt/variational.py` & `lhvqt-0.5.3/lhvqt/variational.py`

 * *Files identical despite different names*

### Comparing `lhvqt-0.5.2/lhvqt.egg-info/PKG-INFO` & `lhvqt-0.5.3/lhvqt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: lhvqt
-Version: 0.5.2
+Version: 0.5.3
 Summary: Frontend filterbank learning module with HVQT initialization capabilities
 Home-page: https://github.com/cwitkowitz/LHVQT
 Author: Frank Cwitkowitz
 Author-email: fcwitkow@ur.rochester.edu
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Learnable Harmonic Variable-Q Transform (LHVQT)
 Implements a frontend filterbank learning module which can be initialized with complex weights for a Variable-Q Transform (lvqt_orig.py). Several techniques and variations of the module are also implemented, including:
  - Multi-channel (harmonic) structure (lhvqt.py)
@@ -38,28 +37,26 @@
 
 # Usage
 Several examples of instantiation, inference, and visualization are provided under the ```examples``` sub-directory. A full-blown training, visualization, and evaluation example for piano transcription can be found at https://github.com/cwitkowitz/sparse-analytic-filters.
 
 ## Cite
 Please cite whichever is more relevant to your usage.
 
-##### arXiv Paper
+##### SMC 2022 Paper
 ```
-@article{cwitkowitz2021learning,
-  author  = {Frank Cwitkowitz and Mojtaba Heydari and Zhiyao Duan},
-  title   = {Learning Sparse Analytic Filters for Piano Transcription},
-  journal = {arXiv preprint arXiv:2108.10382},
-  year    = {2021}
+@inproceedings{cwitkowitz2022learning,
+  title     = {Learning Sparse Analytic Filters for Piano Transcription},
+  author    = {Frank Cwitkowitz and Mojtaba Heydari and Zhiyao Duan},
+  year      = 2022,
+  booktitle = {Proceedings of Sound and Music Computing Conference (SMC)}
 }
 ```
 
 ##### Master's Thesis
 ```
 @mastersthesis{cwitkowitz2019end,
-  author  = {Cwitkowitz, Frank},
   title   = {End-to-End Music Transcription Using Fine-Tuned Variable-{Q} Filterbanks},
-  school  = {Rochester Institute of Technology},
-  year    = {2019}
+  author  = {Cwitkowitz, Frank},
+  year    = 2019,
+  school  = {Rochester Institute of Technology}
 }
 ```
-
-
```

### Comparing `lhvqt-0.5.2/setup.py` & `lhvqt-0.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,13 +7,13 @@
     name='lhvqt',
     url='https://github.com/cwitkowitz/LHVQT',
     author='Frank Cwitkowitz',
     author_email='fcwitkow@ur.rochester.edu',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=['numpy', 'librosa', 'torch', 'matplotlib', 'soundfile'],
-    version='0.5.2',
+    version='0.5.3',
     license='MIT',
     description='Frontend filterbank learning module with HVQT initialization capabilities',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown'
 )
```

