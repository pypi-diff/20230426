# Comparing `tmp/diff_binom_confint-0.0.8.tar.gz` & `tmp/diff_binom_confint-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/diff_binom_confint-0.0.8.tar", last modified: Sun Sep 18 03:36:42 2022, max compression
+gzip compressed data, was "dist/diff_binom_confint-0.0.9.tar", last modified: Sun Sep 18 18:04:31 2022, max compression
```

## Comparing `diff_binom_confint-0.0.8.tar` & `diff_binom_confint-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-09-18 03:36:42.000000 diff_binom_confint-0.0.8/
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-09-18 03:36:42.000000 diff_binom_confint-0.0.8/diff_binom_confint/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3256 2022-09-16 03:09:56.000000 diff_binom_confint-0.0.8/diff_binom_confint/_confint.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      482 2022-09-10 17:13:59.000000 diff_binom_confint-0.0.8/diff_binom_confint/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    19030 2022-09-18 03:22:01.000000 diff_binom_confint-0.0.8/diff_binom_confint/_diff_binom_confint.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4624 2022-09-08 03:15:48.000000 diff_binom_confint-0.0.8/diff_binom_confint/_utils.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       22 2022-09-18 03:35:08.000000 diff_binom_confint-0.0.8/diff_binom_confint/version.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    17889 2022-09-18 03:18:14.000000 diff_binom_confint-0.0.8/diff_binom_confint/_binom_confint.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5886 2022-09-16 06:27:33.000000 diff_binom_confint-0.0.8/README.md
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1517 2022-09-07 02:51:44.000000 diff_binom_confint-0.0.8/setup.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       38 2022-09-18 03:36:42.000000 diff_binom_confint-0.0.8/setup.cfg
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-09-18 03:36:42.000000 diff_binom_confint-0.0.8/diff_binom_confint.egg-info/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       19 2022-09-18 03:36:42.000000 diff_binom_confint-0.0.8/diff_binom_confint.egg-info/top_level.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      462 2022-09-18 03:36:42.000000 diff_binom_confint-0.0.8/diff_binom_confint.egg-info/SOURCES.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        1 2022-09-18 03:36:42.000000 diff_binom_confint-0.0.8/diff_binom_confint.egg-info/dependency_links.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     7973 2022-09-18 03:36:42.000000 diff_binom_confint-0.0.8/diff_binom_confint.egg-info/PKG-INFO
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      181 2022-09-18 03:36:42.000000 diff_binom_confint-0.0.8/diff_binom_confint.egg-info/requires.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     7973 2022-09-18 03:36:42.000000 diff_binom_confint-0.0.8/PKG-INFO
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-09-18 03:36:42.000000 diff_binom_confint-0.0.8/test/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    13339 2022-09-18 03:12:08.000000 diff_binom_confint-0.0.8/test/test_dbci.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5281 2022-09-16 04:17:55.000000 diff_binom_confint-0.0.8/test/test_bci.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-09-18 18:04:31.000000 diff_binom_confint-0.0.9/
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-09-18 18:04:31.000000 diff_binom_confint-0.0.9/diff_binom_confint/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3256 2022-09-16 03:09:56.000000 diff_binom_confint-0.0.9/diff_binom_confint/_confint.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      482 2022-09-10 17:13:59.000000 diff_binom_confint-0.0.9/diff_binom_confint/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    20135 2022-09-18 17:53:47.000000 diff_binom_confint-0.0.9/diff_binom_confint/_diff_binom_confint.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6145 2022-09-18 17:21:01.000000 diff_binom_confint-0.0.9/diff_binom_confint/_utils.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       22 2022-09-18 17:24:05.000000 diff_binom_confint-0.0.9/diff_binom_confint/version.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    17889 2022-09-18 13:07:56.000000 diff_binom_confint-0.0.9/diff_binom_confint/_binom_confint.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6348 2022-09-18 18:02:48.000000 diff_binom_confint-0.0.9/README.md
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1559 2022-09-18 17:14:23.000000 diff_binom_confint-0.0.9/setup.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       38 2022-09-18 18:04:31.000000 diff_binom_confint-0.0.9/setup.cfg
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-09-18 18:04:31.000000 diff_binom_confint-0.0.9/diff_binom_confint.egg-info/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       19 2022-09-18 18:04:31.000000 diff_binom_confint-0.0.9/diff_binom_confint.egg-info/top_level.txt
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      462 2022-09-18 18:04:31.000000 diff_binom_confint-0.0.9/diff_binom_confint.egg-info/SOURCES.txt
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        1 2022-09-18 18:04:31.000000 diff_binom_confint-0.0.9/diff_binom_confint.egg-info/dependency_links.txt
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8591 2022-09-18 18:04:31.000000 diff_binom_confint-0.0.9/diff_binom_confint.egg-info/PKG-INFO
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      200 2022-09-18 18:04:31.000000 diff_binom_confint-0.0.9/diff_binom_confint.egg-info/requires.txt
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8591 2022-09-18 18:04:31.000000 diff_binom_confint-0.0.9/PKG-INFO
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-09-18 18:04:31.000000 diff_binom_confint-0.0.9/test/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    13339 2022-09-18 17:55:58.000000 diff_binom_confint-0.0.9/test/test_dbci.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5281 2022-09-16 04:17:55.000000 diff_binom_confint-0.0.9/test/test_bci.py
```

### Comparing `diff_binom_confint-0.0.8/diff_binom_confint/_confint.py` & `diff_binom_confint-0.0.9/diff_binom_confint/_confint.py`

 * *Files identical despite different names*

### Comparing `diff_binom_confint-0.0.8/diff_binom_confint/_diff_binom_confint.py` & `diff_binom_confint-0.0.9/diff_binom_confint/_diff_binom_confint.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 from scipy.stats import norm
 from scipy.optimize import brentq
 from deprecate_kwargs import deprecate_kwargs
 from deprecated import deprecated
 
 from ._confint import ConfidenceInterval, _SIDE_NAME_MAP, ConfidenceIntervalSides
-from ._utils import add_docstring, remove_parameters_returns_from_docstring
+from ._utils import add_docstring, remove_parameters_returns_from_docstring, accelerator
 
 
 __all__ = [
     "compute_difference_confidence_interval",
     "list_difference_confidence_interval_methods",
 ]
 
@@ -264,108 +264,52 @@
             theta_star + w,
             delta_ratio,
             conf_level,
             confint_type.lower(),
             str(sides),
         )
     elif confint_type.lower() in ["mee", "miettinen-nurminen"]:
+        if confint_type.lower() == "mee":
+            lamb = 1
+        else:  # "miettinen-nurminen"
+            lamb = (n_total + ref_total) / (n_total + ref_total - 1)
         if n_positive == ref_positive == 0:
             # R implementation from https://github.com/AndriSignorell/DescTools/blob/master/R/StatsAndCIs.r
             # `uniroot` unstable for some cases (e.g. 10/10 vs 0/20)
             tol = 1e-6
             lower = uniroot(
                 lambda j: _mee_mn_score_func(
-                    j, ratio, ref_ratio, n_total, ref_total, confint_type.lower()
+                    j, ratio, ref_ratio, n_total, ref_total, lamb
                 )
                 - (1 - _conf_level),
                 -1 + tol,
                 delta_ratio - tol,
                 full_output=False,
             )
             upper = uniroot(
                 lambda j: _mee_mn_score_func(
-                    j, ratio, ref_ratio, n_total, ref_total, confint_type.lower()
+                    j, ratio, ref_ratio, n_total, ref_total, lamb
                 )
                 - (1 - _conf_level),
                 delta_ratio + tol,
                 1 - tol,
                 full_output=False,
             )
         else:  # failed in the case of n_positive == ref_positive == 0
-            theta = ref_total / n_total
-            a = 1 + theta
-            increment = 1e-5
-            itv = []
-            flag = None
-            for j in np.arange(-1, 1 + increment, increment):
-                b = -(1 + theta + ratio + theta * ref_ratio + j * (theta + 2))
-                c = j * (j + 2 * ratio + theta + 1) + ratio + theta * ref_ratio
-                d = -ratio * j * (1 + j)
-                tmp_b = b / 3 / a
-                tmp_c = c / 3 / a
-                v = tmp_b**3 - tmp_b * tmp_c * 3 / 2 + d / 2 / a
-                # https://github.com/AndriSignorell/DescTools/blob/de9731c7d5640deff425e08e63e3aed2c5dc65aa/R/StatsAndCIs.r#L2509
-                # u = np.sign(v) * np.sqrt(tmp_b**2 - tmp_c)
-                if np.abs(v) < np.finfo(np.float64).eps:
-                    v = 0
-                u = np.sqrt(tmp_b**2 - tmp_c)
-                if v < 0:
-                    u = -u
-                w = (np.pi + np.arccos(v / u**3)) / 3
-                ratio_mle = 2 * u * np.cos(w) - tmp_b
-                ref_ratio_mle = ratio_mle - j
-                if confint_type.lower() == "mee":
-                    lamb = 1
-                else:  # "miettinen-nurminen"
-                    lamb = (n_total + ref_total) / (n_total + ref_total - 1)
-                var = np.sqrt(
-                    lamb
-                    * (
-                        ratio_mle * (1 - ratio_mle) / n_total
-                        + ref_ratio_mle * (1 - ref_ratio_mle) / ref_total
-                    )
-                )
-                var = (delta_ratio - j) / var
-                if -z < var < z:
-                    flag = True
-                    itv.append(j)
-                elif flag:
-                    break
+            itv = _mee_mn_lower_upper_bounds(
+                ratio, ref_ratio, n_total, ref_total, lamb, z
+            )
             lower, upper = np.min(itv), np.max(itv)
         return ConfidenceInterval(
             lower, upper, delta_ratio, conf_level, confint_type.lower(), str(sides)
         )
     elif confint_type.lower() == "true-profile":
-        theta = ref_total / n_total
-        a = 1 + theta
-        increment = 1e-5
-        itv = []
-        flag = None
-        for j in np.arange(-1, 1 + increment, increment):
-            b = -(1 + theta + ratio + theta * ref_ratio + j * (theta + 2))
-            c = j * (j + 2 * ratio + theta + 1) + ratio + theta * ref_ratio
-            d = -ratio * j * (1 + j)
-            tmp_b = b / 3 / a
-            tmp_c = c / 3 / a
-            v = tmp_b**3 - tmp_b * tmp_c * 3 / 2 + d / 2 / a
-            u = np.sign(v) * np.sqrt(tmp_b**2 - tmp_c)
-            w = (np.pi + np.arccos(v / u**3)) / 3
-            ratio_mle = 2 * u * np.cos(w) - tmp_b
-            ref_ratio_mle = ratio_mle - j
-            var = (
-                n_positive * np.log(ratio_mle / ratio)
-                + ref_positive * np.log(ref_ratio_mle / ref_ratio)
-                + n_negative * np.log((1 - ratio_mle) / neg_ratio)
-                + ref_negative * np.log((1 - ref_ratio_mle) / ref_neg_ratio)
-            )
-            if var >= -(z**2) / 2:
-                flag = True
-                itv.append(j)
-            elif flag:
-                break
+        itv = _true_profile_lower_upper_bounds(
+            n_positive, n_total, ref_positive, ref_total, z
+        )
         return ConfidenceInterval(
             np.min(itv),
             np.max(itv),
             delta_ratio,
             conf_level,
             confint_type.lower(),
             str(sides),
@@ -514,15 +458,22 @@
 
 def _mee_mn_score_func(
     j: float,
     ratio: float,
     ref_ratio: float,
     n_total: int,
     ref_total: int,
-    method: str,
+    lamb: float,
+) -> float:
+    var = _mee_mn_var_func(j, ratio, ref_ratio, n_total, ref_total, lamb)
+    return 2 * min(pnorm(var), 1 - pnorm(var))
+
+
+def _mee_mn_var_func(
+    j: float, ratio: float, ref_ratio: float, n_total: int, ref_total: int, lamb: float
 ) -> float:
     theta = ref_total / n_total
     delta_ratio = ratio - ref_ratio
     a = a = 1 + theta
     b = -(1 + theta + ratio + theta * ref_ratio + j * (theta + 2))
     c = j * (j + 2 * ratio + theta + 1) + ratio + theta * ref_ratio
     d = -ratio * j * (1 + j)
@@ -535,20 +486,122 @@
         v = 0
     u = np.sqrt(tmp_b**2 - tmp_c)
     if v < 0:
         u = -u
     w = (np.pi + np.arccos(v / u**3)) / 3
     ratio_mle = 2 * u * np.cos(w) - tmp_b
     ref_ratio_mle = ratio_mle - j
-    if method.lower() == "mee":
-        lamb = 1
-    else:  # "miettinen-nurminen"
-        lamb = (n_total + ref_total) / (n_total + ref_total - 1)
     var = np.sqrt(
         lamb
         * (
             ratio_mle * (1 - ratio_mle) / n_total
             + ref_ratio_mle * (1 - ref_ratio_mle) / ref_total
         )
     )
     var = (delta_ratio - j) / var
-    return 2 * min(pnorm(var), 1 - pnorm(var))
+    return var
+
+
+@accelerator.accelerator
+def _mee_mn_lower_upper_bounds(
+    ratio: float,
+    ref_ratio: float,
+    n_total: int,
+    ref_total: int,
+    lamb: float,
+    z: float,
+) -> np.ndarray:
+    theta = ref_total / n_total
+    delta_ratio = ratio - ref_ratio
+    a = 1 + theta
+    increment = 1e-5
+    itv = []
+    # flag = None
+    for j in np.arange(-1, 1 + increment, increment):
+        b = -(1 + theta + ratio + theta * ref_ratio + j * (theta + 2))
+        c = j * (j + 2 * ratio + theta + 1) + ratio + theta * ref_ratio
+        d = -ratio * j * (1 + j)
+        tmp_b = b / 3 / a
+        tmp_c = c / 3 / a
+        v = tmp_b**3 - tmp_b * tmp_c * 3 / 2 + d / 2 / a
+        # https://github.com/AndriSignorell/DescTools/blob/de9731c7d5640deff425e08e63e3aed2c5dc65aa/R/StatsAndCIs.r#L2509
+        # u = np.sign(v) * np.sqrt(tmp_b**2 - tmp_c)
+        if np.abs(v) < np.finfo(np.float64).eps:
+            v = 0
+        u = np.sqrt(tmp_b**2 - tmp_c)
+        if v < 0:
+            u = -u
+        u3 = u**3
+        if u3 == 0:
+            u3 = np.finfo(np.float64).eps
+            continue  # python >= 3.7 would cause ZeroDivisionError
+        w = (np.pi + np.arccos(v / u3)) / 3
+        ratio_mle = 2 * u * np.cos(w) - tmp_b
+        ref_ratio_mle = ratio_mle - j
+        var = np.sqrt(
+            lamb
+            * (
+                ratio_mle * (1 - ratio_mle) / n_total
+                + ref_ratio_mle * (1 - ref_ratio_mle) / ref_total
+            )
+        )
+        var = (delta_ratio - j) / var
+        if -z < var < z:
+            # flag = True
+            itv.append(j)
+        # elif flag:
+        #     break
+    return np.array(itv)
+
+
+@accelerator.accelerator
+def _true_profile_lower_upper_bounds(
+    n_positive: int,
+    n_total: int,
+    ref_positive: int,
+    ref_total: int,
+    z: float,
+) -> np.ndarray:
+    theta = ref_total / n_total
+    ratio = n_positive / n_total
+    ref_ratio = ref_positive / ref_total
+    ref_neg_ratio = 1 - ref_ratio
+    neg_ratio = 1 - ratio
+    n_negative = n_total - n_positive
+    ref_negative = ref_total - ref_positive
+    a = 1 + theta
+    increment = 1e-5
+    itv = []
+    # flag = None
+    for j in np.arange(-1, 1 + increment, increment):
+        b = -(1 + theta + ratio + theta * ref_ratio + j * (theta + 2))
+        c = j * (j + 2 * ratio + theta + 1) + ratio + theta * ref_ratio
+        d = -ratio * j * (1 + j)
+        tmp_b = b / 3 / a
+        tmp_c = c / 3 / a
+        v = tmp_b**3 - tmp_b * tmp_c * 3 / 2 + d / 2 / a
+        # https://github.com/AndriSignorell/DescTools/blob/de9731c7d5640deff425e08e63e3aed2c5dc65aa/R/StatsAndCIs.r#L2509
+        # u = np.sign(v) * np.sqrt(tmp_b**2 - tmp_c)
+        if np.abs(v) < np.finfo(np.float64).eps:
+            v = 0
+        u = np.sqrt(tmp_b**2 - tmp_c)
+        if v < 0:
+            u = -u
+        u3 = u**3
+        if u3 == 0:
+            u3 = np.finfo(np.float64).eps
+            continue  # python >= 3.7 would cause ZeroDivisionError
+        w = (np.pi + np.arccos(v / u3)) / 3
+        ratio_mle = 2 * u * np.cos(w) - tmp_b
+        ref_ratio_mle = ratio_mle - j
+        var = (
+            n_positive * np.log(ratio_mle / ratio)
+            + ref_positive * np.log(ref_ratio_mle / ref_ratio)
+            + n_negative * np.log((1 - ratio_mle) / neg_ratio)
+            + ref_negative * np.log((1 - ref_ratio_mle) / ref_neg_ratio)
+        )
+        if var >= -(z**2) / 2:
+            # flag = True
+            itv.append(j)
+        # elif flag:
+        #     break
+    return np.array(itv)
```

### Comparing `diff_binom_confint-0.0.8/diff_binom_confint/_binom_confint.py` & `diff_binom_confint-0.0.9/diff_binom_confint/_binom_confint.py`

 * *Files identical despite different names*

### Comparing `diff_binom_confint-0.0.8/README.md` & `diff_binom_confint-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 or git clone this repository and install locally via
 
 ```bash
 cd DBCI
 python -m pip install .
 ```
 
+## `Numba` accelerated version
+
+Install using
+
+```bash
+python -m pip install diff-binom-confint[acc]
+```
+
 ## Usage examples
 
 ```python
 from diff_binom_confint import compute_difference_confidence_interval
 
 n_positive, n_total = 84, 101
 ref_positive, ref_total = 89, 105
@@ -109,14 +117,15 @@
 
 1. <a name="ref1"></a> [SAS](https://www.lexjansen.com/wuss/2016/127_Final_Paper_PDF.pdf)
 2. <a name="ref2"></a> [PASS](https://ncss-wpengine.netdna-ssl.com/wp-content/themes/ncss/pdf/Procedures/PASS/Confidence_Intervals_for_the_Difference_Between_Two_Proportions.pdf)
 3. <a name="ref3"></a> [statsmodels.stats.proportion](https://www.statsmodels.org/devel/_modules/statsmodels/stats/proportion.html)
 4. <a name="ref4"></a> [scipy.stats._binomtest](https://github.com/scipy/scipy/blob/main/scipy/stats/_binomtest.py)
 5. <a name="ref5"></a> [corplingstats](https://corplingstats.wordpress.com/2019/04/27/correcting-for-continuity/)
 6. <a name="ref6"></a> [DescTools.StatsAndCIs](https://github.com/AndriSignorell/DescTools/blob/master/R/StatsAndCIs.r)
+7. <a name="ref7"></a> [Newcombee](https://onlinelibrary.wiley.com/doi/10.1002/(SICI)1097-0258(19980430)17:8%3C873::AID-SIM779%3E3.0.CO;2-I)
 
 ## NOTE
 
 [Reference 1](#ref1) has errors in the description of the methods `Wilson CC`, `Mee`, `Miettinen-Nurminen`.
 The correct computation of `Wilson CC` is given in [Reference 5](#ref5).
 The correct computation of `Mee`, `Miettinen-Nurminen` are given in the **code blocks** in [Reference 1](#ref1)
 
@@ -139,16 +148,24 @@
         ci = BinomCI(84,101,method = m)
         new_row = data.table("method" = m, "ratio"=ci[1], "lower_bound" = ci[2], "upper_bound" = ci[3])
         results = rbindlist(list(results, new_row))
     }
     fwrite(results, "./test/test-data/example-84-101.csv")  # with manual slight adjustment of method names
     ```
 
+3. taken from [Reference 7](#ref7) (Table II).
+
 The filenames has the following pattern:
 
 ```python
 # for computing confidence interval for difference of binomial proportions
 "example-(?P<n_positive>[\\d]+)-(?P<n_total>[\\d]+)-vs-(?P<ref_positive>[\\d]+)-(?P<ref_total>[\\d]+)\\.csv"
 
 # for computing confidence interval for binomial proportions
 "example-(?P<n_positive>[\\d]+)-(?P<n_total>[\\d]+)\\.csv"
 ```
+
+Note that the out-of-range values (e.g. `> 1`) are left as empty values in the `.csv` files.
+
+## Known Issues
+
+1. Edge cases incorrect for the method `true-profile`.
```

### Comparing `diff_binom_confint-0.0.8/setup.py` & `diff_binom_confint-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 extras["test"] = [
     "pandas",
     "black==22.3.0",
     "flake8",
     "pytest",
     "pytest-xdist",
 ]
-extras["dev"] = extras["test"]
+extras["acc"] = ["numba"]
+extras["dev"] = extras["test"] + extras["acc"]
 
 
 setuptools.setup(
     name="diff_binom_confint",
     version=__version__,
     author="DeepPSP",
     author_email="wenh06@gmail.com",
```

### Comparing `diff_binom_confint-0.0.8/diff_binom_confint.egg-info/PKG-INFO` & `diff_binom_confint-0.0.9/diff_binom_confint.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diff-binom-confint
-Version: 0.0.8
+Version: 0.0.9
 Summary: Computation of confidence intervals for binomial proportions and for difference of binomial proportions.
 Home-page: https://github.com/DeepPSP/DBCI
 Author: DeepPSP
 Author-email: wenh06@gmail.com
 License: MIT
 Description: # Confidence Intervals for Difference of Binomial Proportions
         
@@ -32,14 +32,22 @@
         or git clone this repository and install locally via
         
         ```bash
         cd DBCI
         python -m pip install .
         ```
         
+        ## `Numba` accelerated version
+        
+        Install using
+        
+        ```bash
+        python -m pip install diff-binom-confint[acc]
+        ```
+        
         ## Usage examples
         
         ```python
         from diff_binom_confint import compute_difference_confidence_interval
         
         n_positive, n_total = 84, 101
         ref_positive, ref_total = 89, 105
@@ -117,14 +125,15 @@
         
         1. <a name="ref1"></a> [SAS](https://www.lexjansen.com/wuss/2016/127_Final_Paper_PDF.pdf)
         2. <a name="ref2"></a> [PASS](https://ncss-wpengine.netdna-ssl.com/wp-content/themes/ncss/pdf/Procedures/PASS/Confidence_Intervals_for_the_Difference_Between_Two_Proportions.pdf)
         3. <a name="ref3"></a> [statsmodels.stats.proportion](https://www.statsmodels.org/devel/_modules/statsmodels/stats/proportion.html)
         4. <a name="ref4"></a> [scipy.stats._binomtest](https://github.com/scipy/scipy/blob/main/scipy/stats/_binomtest.py)
         5. <a name="ref5"></a> [corplingstats](https://corplingstats.wordpress.com/2019/04/27/correcting-for-continuity/)
         6. <a name="ref6"></a> [DescTools.StatsAndCIs](https://github.com/AndriSignorell/DescTools/blob/master/R/StatsAndCIs.r)
+        7. <a name="ref7"></a> [Newcombee](https://onlinelibrary.wiley.com/doi/10.1002/(SICI)1097-0258(19980430)17:8%3C873::AID-SIM779%3E3.0.CO;2-I)
         
         ## NOTE
         
         [Reference 1](#ref1) has errors in the description of the methods `Wilson CC`, `Mee`, `Miettinen-Nurminen`.
         The correct computation of `Wilson CC` is given in [Reference 5](#ref5).
         The correct computation of `Mee`, `Miettinen-Nurminen` are given in the **code blocks** in [Reference 1](#ref1)
         
@@ -147,31 +156,40 @@
                 ci = BinomCI(84,101,method = m)
                 new_row = data.table("method" = m, "ratio"=ci[1], "lower_bound" = ci[2], "upper_bound" = ci[3])
                 results = rbindlist(list(results, new_row))
             }
             fwrite(results, "./test/test-data/example-84-101.csv")  # with manual slight adjustment of method names
             ```
         
+        3. taken from [Reference 7](#ref7) (Table II).
+        
         The filenames has the following pattern:
         
         ```python
         # for computing confidence interval for difference of binomial proportions
         "example-(?P<n_positive>[\\d]+)-(?P<n_total>[\\d]+)-vs-(?P<ref_positive>[\\d]+)-(?P<ref_total>[\\d]+)\\.csv"
         
         # for computing confidence interval for binomial proportions
         "example-(?P<n_positive>[\\d]+)-(?P<n_total>[\\d]+)\\.csv"
         ```
         
+        Note that the out-of-range values (e.g. `> 1`) are left as empty values in the `.csv` files.
+        
+        ## Known Issues
+        
+        1. Edge cases incorrect for the method `true-profile`.
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: acc
 Provides-Extra: dev
```

### Comparing `diff_binom_confint-0.0.8/PKG-INFO` & `diff_binom_confint-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diff_binom_confint
-Version: 0.0.8
+Version: 0.0.9
 Summary: Computation of confidence intervals for binomial proportions and for difference of binomial proportions.
 Home-page: https://github.com/DeepPSP/DBCI
 Author: DeepPSP
 Author-email: wenh06@gmail.com
 License: MIT
 Description: # Confidence Intervals for Difference of Binomial Proportions
         
@@ -32,14 +32,22 @@
         or git clone this repository and install locally via
         
         ```bash
         cd DBCI
         python -m pip install .
         ```
         
+        ## `Numba` accelerated version
+        
+        Install using
+        
+        ```bash
+        python -m pip install diff-binom-confint[acc]
+        ```
+        
         ## Usage examples
         
         ```python
         from diff_binom_confint import compute_difference_confidence_interval
         
         n_positive, n_total = 84, 101
         ref_positive, ref_total = 89, 105
@@ -117,14 +125,15 @@
         
         1. <a name="ref1"></a> [SAS](https://www.lexjansen.com/wuss/2016/127_Final_Paper_PDF.pdf)
         2. <a name="ref2"></a> [PASS](https://ncss-wpengine.netdna-ssl.com/wp-content/themes/ncss/pdf/Procedures/PASS/Confidence_Intervals_for_the_Difference_Between_Two_Proportions.pdf)
         3. <a name="ref3"></a> [statsmodels.stats.proportion](https://www.statsmodels.org/devel/_modules/statsmodels/stats/proportion.html)
         4. <a name="ref4"></a> [scipy.stats._binomtest](https://github.com/scipy/scipy/blob/main/scipy/stats/_binomtest.py)
         5. <a name="ref5"></a> [corplingstats](https://corplingstats.wordpress.com/2019/04/27/correcting-for-continuity/)
         6. <a name="ref6"></a> [DescTools.StatsAndCIs](https://github.com/AndriSignorell/DescTools/blob/master/R/StatsAndCIs.r)
+        7. <a name="ref7"></a> [Newcombee](https://onlinelibrary.wiley.com/doi/10.1002/(SICI)1097-0258(19980430)17:8%3C873::AID-SIM779%3E3.0.CO;2-I)
         
         ## NOTE
         
         [Reference 1](#ref1) has errors in the description of the methods `Wilson CC`, `Mee`, `Miettinen-Nurminen`.
         The correct computation of `Wilson CC` is given in [Reference 5](#ref5).
         The correct computation of `Mee`, `Miettinen-Nurminen` are given in the **code blocks** in [Reference 1](#ref1)
         
@@ -147,31 +156,40 @@
                 ci = BinomCI(84,101,method = m)
                 new_row = data.table("method" = m, "ratio"=ci[1], "lower_bound" = ci[2], "upper_bound" = ci[3])
                 results = rbindlist(list(results, new_row))
             }
             fwrite(results, "./test/test-data/example-84-101.csv")  # with manual slight adjustment of method names
             ```
         
+        3. taken from [Reference 7](#ref7) (Table II).
+        
         The filenames has the following pattern:
         
         ```python
         # for computing confidence interval for difference of binomial proportions
         "example-(?P<n_positive>[\\d]+)-(?P<n_total>[\\d]+)-vs-(?P<ref_positive>[\\d]+)-(?P<ref_total>[\\d]+)\\.csv"
         
         # for computing confidence interval for binomial proportions
         "example-(?P<n_positive>[\\d]+)-(?P<n_total>[\\d]+)\\.csv"
         ```
         
+        Note that the out-of-range values (e.g. `> 1`) are left as empty values in the `.csv` files.
+        
+        ## Known Issues
+        
+        1. Edge cases incorrect for the method `true-profile`.
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: acc
 Provides-Extra: dev
```

### Comparing `diff_binom_confint-0.0.8/test/test_dbci.py` & `diff_binom_confint-0.0.9/test/test_dbci.py`

 * *Files identical despite different names*

### Comparing `diff_binom_confint-0.0.8/test/test_bci.py` & `diff_binom_confint-0.0.9/test/test_bci.py`

 * *Files identical despite different names*

