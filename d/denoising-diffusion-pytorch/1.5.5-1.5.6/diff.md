# Comparing `tmp/denoising-diffusion-pytorch-1.5.5.tar.gz` & `tmp/denoising-diffusion-pytorch-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.5.5.tar", last modified: Wed Apr 19 18:17:48 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.5.6.tar", last modified: Tue Apr 25 16:09:24 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.5.5.tar` & `denoising-diffusion-pytorch-1.5.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:17:48.389421 denoising-diffusion-pytorch-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-19 18:17:48.389421 denoising-diffusion-pytorch-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:17:48.385420 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30767 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:17:48.389421 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-19 18:17:48.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-19 18:17:48.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:17:48.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 18:17:48.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 18:17:48.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:17:48.389421 denoising-diffusion-pytorch-1.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:09:24.816532 denoising-diffusion-pytorch-1.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-25 16:09:24.816532 denoising-diffusion-pytorch-1.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:09:24.812532 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30767 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:09:24.816532 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-25 16:09:24.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-25 16:09:24.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:09:24.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-25 16:09:24.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-25 16:09:24.000000 denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:09:24.816532 denoising-diffusion-pytorch-1.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-25 16:09:11.000000 denoising-diffusion-pytorch-1.5.6/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.5.5/LICENSE` & `denoising-diffusion-pytorch-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/PKG-INFO` & `denoising-diffusion-pytorch-1.5.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.5.5
+Version: 1.5.6
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.5.5/README.md` & `denoising-diffusion-pytorch-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,29 +77,33 @@
     ):
         super().__init__(model, *args, **kwargs)
         assert model.out_dim == (model.channels * 2), 'dimension out of unet must be twice the number of channels for learned variance - you can also set the `learned_variance` keyword argument on the Unet to be `True`'
         assert not model.self_condition, 'not supported yet'
 
         self.vb_loss_weight = vb_loss_weight
 
-    def model_predictions(self, x, t):
+    def model_predictions(self, x, t, clip_x_start = False):
         model_output = self.model(x, t)
         model_output, pred_variance = model_output.chunk(2, dim = 1)
 
+        maybe_clip = partial(torch.clamp, min = -1., max = 1.) if clip_x_start else identity
+
         if self.objective == 'pred_noise':
             pred_noise = model_output
             x_start = self.predict_start_from_noise(x, t, model_output)
 
         elif self.objective == 'pred_x0':
             pred_noise = self.predict_noise_from_start(x, t, model_output)
             x_start = model_output
 
+        x_start = maybe_clip(x_start)
+
         return ModelPrediction(pred_noise, x_start, pred_variance)
 
-    def p_mean_variance(self, *, x, t, clip_denoised, model_output = None):
+    def p_mean_variance(self, *, x, t, clip_denoised, model_output = None, **kwargs):
         model_output = default(model_output, lambda: self.model(x, t))
         pred_noise, var_interp_frac_unnormalized = model_output.chunk(2, dim = 1)
 
         min_log = extract(self.posterior_log_variance_clipped, t, x.shape)
         max_log = extract(torch.log(self.betas), t, x.shape)
         var_interp_frac = unnormalize_to_zero_to_one(var_interp_frac_unnormalized)
 
@@ -109,28 +113,28 @@
         x_start = self.predict_start_from_noise(x, t, pred_noise)
 
         if clip_denoised:
             x_start.clamp_(-1., 1.)
 
         model_mean, _, _ = self.q_posterior(x_start, x, t)
 
-        return model_mean, model_variance, model_log_variance
+        return model_mean, model_variance, model_log_variance, x_start
 
     def p_losses(self, x_start, t, noise = None, clip_denoised = False):
         noise = default(noise, lambda: torch.randn_like(x_start))
         x_t = self.q_sample(x_start = x_start, t = t, noise = noise)
 
         # model output
 
         model_output = self.model(x_t, t)
 
         # calculating kl loss for learned variance (interpolation)
 
         true_mean, _, true_log_variance_clipped = self.q_posterior(x_start = x_start, x_t = x_t, t = t)
-        model_mean, _, model_log_variance = self.p_mean_variance(x = x_t, t = t, clip_denoised = clip_denoised, model_output = model_output)
+        model_mean, _, model_log_variance, _ = self.p_mean_variance(x = x_t, t = t, clip_denoised = clip_denoised, model_output = model_output)
 
         # kl loss with detached model predicted mean, for stability reasons as in paper
 
         detached_model_mean = model_mean.detach()
 
         kl = normal_kl(true_mean, true_log_variance_clipped, detached_model_mean, model_log_variance)
         kl = meanflat(kl) * NAT
```

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.5.5
+Version: 1.5.6
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.5.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.5/setup.py` & `denoising-diffusion-pytorch-1.5.6/setup.py`

 * *Files identical despite different names*

