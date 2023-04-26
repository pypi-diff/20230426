# Comparing `tmp/phaseaug-1.0.0.tar.gz` & `tmp/phaseaug-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phaseaug-1.0.0.tar", last modified: Thu Apr 20 04:22:58 2023, max compression
+gzip compressed data, was "phaseaug-1.0.1.tar", last modified: Tue Apr 25 23:13:19 2023, max compression
```

## Comparing `phaseaug-1.0.0.tar` & `phaseaug-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-20 04:22:58.574484 phaseaug-1.0.0/
--rw-r--r--   0 jun        (501) staff       (20)     1516 2022-10-07 01:16:31.000000 phaseaug-1.0.0/LICENSE
--rw-r--r--   0 jun        (501) staff       (20)     6650 2023-04-20 04:22:58.574362 phaseaug-1.0.0/PKG-INFO
--rw-r--r--   0 jun        (501) staff       (20)     6196 2023-04-20 04:21:40.000000 phaseaug-1.0.0/README.md
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-20 04:22:58.572986 phaseaug-1.0.0/phaseaug/
--rw-r--r--   0 jun        (501) staff       (20)       23 2022-11-21 06:11:54.000000 phaseaug-1.0.0/phaseaug/__init__.py
--rw-r--r--   0 jun        (501) staff       (20)     4555 2023-04-20 04:16:20.000000 phaseaug-1.0.0/phaseaug/phaseaug.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-20 04:22:58.573933 phaseaug-1.0.0/phaseaug.egg-info/
--rw-r--r--   0 jun        (501) staff       (20)     6650 2023-04-20 04:22:58.000000 phaseaug-1.0.0/phaseaug.egg-info/PKG-INFO
--rw-r--r--   0 jun        (501) staff       (20)      506 2023-04-20 04:22:58.000000 phaseaug-1.0.0/phaseaug.egg-info/SOURCES.txt
--rw-r--r--   0 jun        (501) staff       (20)        1 2023-04-20 04:22:58.000000 phaseaug-1.0.0/phaseaug.egg-info/dependency_links.txt
--rw-r--r--   0 jun        (501) staff       (20)        1 2022-11-21 06:00:26.000000 phaseaug-1.0.0/phaseaug.egg-info/not-zip-safe
--rw-r--r--   0 jun        (501) staff       (20)       23 2023-04-20 04:22:58.000000 phaseaug-1.0.0/phaseaug.egg-info/requires.txt
--rw-r--r--   0 jun        (501) staff       (20)        9 2023-04-20 04:22:58.000000 phaseaug-1.0.0/phaseaug.egg-info/top_level.txt
--rw-r--r--   0 jun        (501) staff       (20)       38 2023-04-20 04:22:58.574529 phaseaug-1.0.0/setup.cfg
--rw-r--r--   0 jun        (501) staff       (20)      857 2023-04-20 04:18:16.000000 phaseaug-1.0.0/setup.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-25 23:13:19.788671 phaseaug-1.0.1/
+-rw-r--r--   0 jun        (501) staff       (20)     1516 2022-10-07 01:16:31.000000 phaseaug-1.0.1/LICENSE
+-rw-r--r--   0 jun        (501) staff       (20)     6650 2023-04-25 23:13:19.788521 phaseaug-1.0.1/PKG-INFO
+-rw-r--r--   0 jun        (501) staff       (20)     6196 2023-04-20 04:21:40.000000 phaseaug-1.0.1/README.md
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-25 23:13:19.786720 phaseaug-1.0.1/phaseaug/
+-rw-r--r--   0 jun        (501) staff       (20)       23 2022-11-21 06:11:54.000000 phaseaug-1.0.1/phaseaug/__init__.py
+-rw-r--r--   0 jun        (501) staff       (20)     4555 2023-04-25 23:05:24.000000 phaseaug-1.0.1/phaseaug/phaseaug.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-25 23:13:19.787970 phaseaug-1.0.1/phaseaug.egg-info/
+-rw-r--r--   0 jun        (501) staff       (20)     6650 2023-04-25 23:13:19.000000 phaseaug-1.0.1/phaseaug.egg-info/PKG-INFO
+-rw-r--r--   0 jun        (501) staff       (20)      506 2023-04-25 23:13:19.000000 phaseaug-1.0.1/phaseaug.egg-info/SOURCES.txt
+-rw-r--r--   0 jun        (501) staff       (20)        1 2023-04-25 23:13:19.000000 phaseaug-1.0.1/phaseaug.egg-info/dependency_links.txt
+-rw-r--r--   0 jun        (501) staff       (20)        1 2022-11-21 06:00:26.000000 phaseaug-1.0.1/phaseaug.egg-info/not-zip-safe
+-rw-r--r--   0 jun        (501) staff       (20)       23 2023-04-25 23:13:19.000000 phaseaug-1.0.1/phaseaug.egg-info/requires.txt
+-rw-r--r--   0 jun        (501) staff       (20)        9 2023-04-25 23:13:19.000000 phaseaug-1.0.1/phaseaug.egg-info/top_level.txt
+-rw-r--r--   0 jun        (501) staff       (20)       38 2023-04-25 23:13:19.788734 phaseaug-1.0.1/setup.cfg
+-rw-r--r--   0 jun        (501) staff       (20)      857 2023-04-25 23:11:39.000000 phaseaug-1.0.1/setup.py
```

### Comparing `phaseaug-1.0.0/LICENSE` & `phaseaug-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phaseaug-1.0.0/PKG-INFO` & `phaseaug-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phaseaug
-Version: 1.0.0
+Version: 1.0.1
 Summary: PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping
 Home-page: https://github.com/mindslab-ai/phaseaug
 Author: junjun3518
 Author-email: junjun3518@gmail.com
 License: UNKNOWN
 Keywords: torch,pytorch,augmentation,diffaugment,speech synthesis,vocoder
 Platform: UNKNOWN
```

### Comparing `phaseaug-1.0.0/README.md` & `phaseaug-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `phaseaug-1.0.0/phaseaug/phaseaug.py` & `phaseaug-1.0.1/phaseaug/phaseaug.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,25 +96,26 @@
                 return x_aug
         self.stft_rot_istft = stft_rot_istft
         
     # x: audio [B,1,T] -> [B,1,T]
     # phi: [B,nfft//2+1]
     # also possible for x :[B,C,T] but we did not generalize it.
     def forward(self, x, phi=None):
+        B = x.shape[0]
         x = x.squeeze(1)  #[B,t]
         if phi is None:
-            phi = self.sample_phi(self, X.shape[0])
+            phi = self.sample_phi(self, B)
         phi[:, 0] = 0. # we are multiplying phi_ref to mu, so it is always zero in our scheme
         phi = phi.unsqueeze(-1)  #[B,F,1]
         x_aug = self.stft_rot_istft(self, x, phi)
         return x_aug  #[B,1,t]
 
     # x: audio [B,1,T] -> [B,1,T]
     # phi: [B,nfft//2+1]
     def forward_sync(self, x, x_hat, phi=None):
         B = x.shape[0]
         x = torch.cat([x, x_hat], dim=0) #[2B,1,t]
         if phi is None:
-            phi = self.sample_phi(self, X.shape[0] // 2) #[2B, nfft//2+1]
+            phi = self.sample_phi(self, B) #[2B, nfft//2+1]
         phi = torch.cat([phi, phi], dim=0)
         x_augs = self.forward(x, phi).split(B, dim=0)
         return x_augs
```

### Comparing `phaseaug-1.0.0/phaseaug.egg-info/PKG-INFO` & `phaseaug-1.0.1/phaseaug.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phaseaug
-Version: 1.0.0
+Version: 1.0.1
 Summary: PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping
 Home-page: https://github.com/mindslab-ai/phaseaug
 Author: junjun3518
 Author-email: junjun3518@gmail.com
 License: UNKNOWN
 Keywords: torch,pytorch,augmentation,diffaugment,speech synthesis,vocoder
 Platform: UNKNOWN
```

### Comparing `phaseaug-1.0.0/setup.py` & `phaseaug-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name                = 'phaseaug',
-    version             = '1.0.0',
+    version             = '1.0.1',
     description         = 'PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author              = 'junjun3518',
     author_email        = 'junjun3518@gmail.com',
     url                 = 'https://github.com/mindslab-ai/phaseaug',
     install_requires    = ['torch', 'alias-free-torch'],
```

