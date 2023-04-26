# Comparing `tmp/shipmmg-0.0.8.tar.gz` & `tmp/shipmmg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipmmg-0.0.8.tar", last modified: Sat Jan  1 12:40:46 2022, max compression
+gzip compressed data, was "shipmmg-0.0.9.tar", max compression
```

## Comparing `shipmmg-0.0.8.tar` & `shipmmg-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2021-01-09 09:21:13.038804 shipmmg-0.0.8/LICENSE
--rw-r--r--   0        0        0     1633 2021-04-10 07:47:02.162827 shipmmg-0.0.8/README.md
--rw-r--r--   0        0        0      576 2022-01-01 12:40:25.750560 shipmmg-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       22 2022-01-01 12:40:25.750560 shipmmg-0.0.8/shipmmg/__init__.py
--rw-r--r--   0        0        0     6345 2022-01-01 12:40:25.750560 shipmmg-0.0.8/shipmmg/draw_obj.py
--rw-r--r--   0        0        0    23214 2022-01-01 12:40:25.750560 shipmmg-0.0.8/shipmmg/kt.py
--rw-r--r--   0        0        0    55376 2022-01-01 12:40:25.754560 shipmmg-0.0.8/shipmmg/mmg_3dof.py
--rw-r--r--   0        0        0    41409 2022-01-01 12:40:25.754560 shipmmg-0.0.8/shipmmg/ship_obj_3dof.py
--rw-r--r--   0        0        0     2420 2022-01-01 12:40:46.979976 shipmmg-0.0.8/setup.py
--rw-r--r--   0        0        0     2423 2022-01-01 12:40:46.980260 shipmmg-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2021-01-09 09:21:13.038804 shipmmg-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2207 2022-05-17 10:15:07.000000 shipmmg-0.0.9/README.md
+-rw-r--r--   0        0        0      594 2022-05-17 10:16:02.000000 shipmmg-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-05-17 10:15:55.000000 shipmmg-0.0.9/shipmmg/__init__.py
+-rw-r--r--   0        0        0     6345 2022-01-01 12:40:25.750560 shipmmg-0.0.9/shipmmg/draw_obj.py
+-rw-r--r--   0        0        0    23214 2022-01-01 12:40:25.750560 shipmmg-0.0.9/shipmmg/kt.py
+-rw-r--r--   0        0        0    55718 2022-05-17 10:15:07.000000 shipmmg-0.0.9/shipmmg/mmg_3dof.py
+-rw-r--r--   0        0        0    41409 2022-01-01 12:40:25.754560 shipmmg-0.0.9/shipmmg/ship_obj_3dof.py
+-rw-r--r--   0        0        0     3050 2022-05-17 10:28:00.933485 shipmmg-0.0.9/setup.py
+-rw-r--r--   0        0        0     3088 2022-05-17 10:28:00.933955 shipmmg-0.0.9/PKG-INFO
```

### Comparing `shipmmg-0.0.8/LICENSE` & `shipmmg-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shipmmg-0.0.8/pyproject.toml` & `shipmmg-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "shipmmg"
-version = "0.0.8"
+version = "0.0.9"
 description = "A Python package of ship maneuvering simulation"
 readme = "README.md"
 authors = ["Taiga MITSUYUKI <mitsuyuki-taiga-my@ynu.ac.jp>"]
 repository="https://github.com/ShipMMG/shipmmg"
 documentation = "https://shipmmg.github.io/shipmmg/"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.19.5"
 scipy = "^1.6.0"
 pytest-cov = "^2.10.1"
 matplotlib = "^3.3.3"
+Pillow = "^9.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shipmmg-0.0.8/shipmmg/draw_obj.py` & `shipmmg-0.0.9/shipmmg/draw_obj.py`

 * *Files identical despite different names*

### Comparing `shipmmg-0.0.8/shipmmg/kt.py` & `shipmmg-0.0.9/shipmmg/kt.py`

 * *Files identical despite different names*

### Comparing `shipmmg-0.0.8/shipmmg/mmg_3dof.py` & `shipmmg-0.0.9/shipmmg/mmg_3dof.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
             Added moment of inertia
         f_α (float):
             Rudder lift gradient coefficient
         ϵ (float):
             Ratio of wake fraction at propeller and rudder positions
         t_R (float):
             Steering resistance deduction factor
+        x_R (float):
+            Longitudinal coordinate of rudder position.
         a_H (float):
             Rudder force increase factor
         x_H (float):
             Longitudinal coordinate of acting point of the additional lateral force component induced by steering
         γ_R_minus (float):
             Flow straightening coefficient if βR < 0
         γ_R_plus (float):
@@ -98,14 +100,15 @@
     η: float
     m_x: float
     m_y: float
     J_z: float
     f_α: float
     ϵ: float
     t_R: float
+    x_R: float
     a_H: float
     x_H: float
     γ_R_minus: float
     γ_R_plus: float
     l_R: float
     κ: float
     t_P: float
@@ -329,14 +332,15 @@
         >>>                     η=D_p/0.345,
         >>>                     m_x=0.022*(0.5 * ρ * (L_pp ** 2) * d),
         >>>                     m_y=0.223*(0.5 * ρ * (L_pp ** 2) * d),
         >>>                     J_z=0.011*(0.5 * ρ * (L_pp ** 4) * d),
         >>>                     f_α=2.747,
         >>>                     ϵ=1.09,
         >>>                     t_R=0.387,
+        >>>                     x_R=-0.500*L_pp,
         >>>                     a_H=0.312,
         >>>                     x_H=-0.464*L_pp,
         >>>                     γ_R_minus=0.395,
         >>>                     γ_R_plus=0.640,
         >>>                     l_R=-0.710,
         >>>                     κ=0.50,
         >>>                     t_P=0.220,
@@ -395,14 +399,15 @@
         η=basic_params.η,
         m_x=basic_params.m_x,
         m_y=basic_params.m_y,
         J_z=basic_params.J_z,
         f_α=basic_params.f_α,
         ϵ=basic_params.ϵ,
         t_R=basic_params.t_R,
+        x_R=basic_params.x_R,
         a_H=basic_params.a_H,
         x_H=basic_params.x_H,
         γ_R_minus=basic_params.γ_R_minus,
         γ_R_plus=basic_params.γ_R_plus,
         l_R=basic_params.l_R,
         κ=basic_params.κ,
         t_P=basic_params.t_P,
@@ -455,14 +460,15 @@
     η: float,
     m_x: float,
     m_y: float,
     J_z: float,
     f_α: float,
     ϵ: float,
     t_R: float,
+    x_R: float,
     a_H: float,
     x_H: float,
     γ_R_minus: float,
     γ_R_plus: float,
     l_R: float,
     κ: float,
     t_P: float,
@@ -540,14 +546,16 @@
             Added moment of inertia
         f_α (float):
             Rudder lift gradient coefficient
         ϵ (float):
             Ratio of wake fraction at propeller and rudder positions
         t_R (float):
             Steering resistance deduction factor
+        x_R (float):
+            Longitudinal coordinate of rudder position
         a_H (float):
             Rudder force increase factor
         x_H (float):
             Longitudinal coordinate of acting point of the additional lateral force component induced by steering
         γ_R_minus (float):
             Flow straightening coefficient if βR < 0
         γ_R_plus (float):
@@ -729,14 +737,15 @@
         >>> η=D_p/0.345
         >>> m_x=0.022*(0.5 * ρ * (L_pp ** 2) * d)
         >>> m_y=0.223*(0.5 * ρ * (L_pp ** 2) * d)
         >>> J_z=0.011*(0.5 * ρ * (L_pp ** 4) * d)
         >>> f_α=2.747
         >>> ϵ=1.09
         >>> t_R=0.387
+        >>> x_R=-0.500*L_pp
         >>> a_H=0.312
         >>> x_H=-0.464*L_pp
         >>> γ_R=0.395
         >>> l_R=-0.710
         >>> κ=0.50
         >>> t_P=0.220
         >>> w_P0=0.40
@@ -773,14 +782,15 @@
         >>>                    η=η,
         >>>                    m_x=m_x,
         >>>                    m_y=m_y,
         >>>                    J_z=J_z,
         >>>                    f_α=f_α,
         >>>                    ϵ=ϵ,
         >>>                    t_R=t_R,
+        >>>                    x_R=x_R,
         >>>                    a_H=a_H,
         >>>                    x_H=x_H,
         >>>                    γ_R=γ_R,
         >>>                    l_R=l_R,
         >>>                    κ=κ,
         >>>                    t_P=t_P,
         >>>                    w_P0=w_P0,
@@ -898,15 +908,15 @@
                 + N_r_dash * r_dash
                 + N_vvv_dash * (v_dash ** 3)
                 + N_vvr_dash * (v_dash ** 2) * r_dash
                 + N_vrr_dash * v_dash * (r_dash ** 2)
                 + N_rrr_dash * (r_dash ** 3)
             )
         )
-        N_R = -(-0.5 + a_H * x_H) * F_N * np.cos(δ)
+        N_R = -(x_R + a_H * x_H) * F_N * np.cos(δ)
         d_u = ((X_H + X_R + X_P) + (m + m_y) * v * r + x_G * m * (r ** 2)) / (m + m_x)
         d_v = (
             (x_G ** 2) * (m ** 2) * u * r
             - (N_H + N_R) * x_G * m
             + ((Y_H + Y_R) - (m + m_x) * u * r) * (I_zG + J_z + (x_G ** 2) * m)
         ) / ((I_zG + J_z + (x_G ** 2) * m) * (m + m_y) - (x_G ** 2) * (m ** 2))
         d_r = (N_H + N_R - x_G * m * (d_v + u * r)) / (I_zG + J_z + (x_G ** 2) * m)
@@ -1182,15 +1192,15 @@
             U_list,
             v_dash_list,
             r_dash_list,
         )
     )
     N_R_list = list(
         map(
-            lambda F_N, δ: -(-0.5 + basic_params.a_H * basic_params.x_H)
+            lambda F_N, δ: -(basic_params.x_R + basic_params.a_H * basic_params.x_H)
             * F_N
             * np.cos(δ),
             F_N_list,
             δ_list,
         )
     )
     if return_all_vals:
```

### Comparing `shipmmg-0.0.8/shipmmg/ship_obj_3dof.py` & `shipmmg-0.0.9/shipmmg/ship_obj_3dof.py`

 * *Files identical despite different names*

### Comparing `shipmmg-0.0.8/setup.py` & `shipmmg-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 packages = \
 ['shipmmg']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['matplotlib>=3.3.3,<4.0.0',
+['Pillow>=9.0.0,<10.0.0',
+ 'matplotlib>=3.3.3,<4.0.0',
  'numpy>=1.19.5,<2.0.0',
  'pytest-cov>=2.10.1,<3.0.0',
  'scipy>=1.6.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'shipmmg',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'A Python package of ship maneuvering simulation',
-    'long_description': "# ShipMMG: Ship Maneuvering Simulation Model\n\n[![PyPi version](https://pypip.in/v/shipmmg/badge.png)](https://pypi.org/project/shipmmg/)\n[![Anaconda-Server Badge](https://anaconda.org/taiga4112/shipmmg/badges/version.svg)](https://anaconda.org/taiga4112/shipmmg)\n![codecov](https://github.com/ShipMMG/shipmmg/workflows/codecov/badge.svg)\n[![codecov](https://codecov.io/gh/ShipMMG/shipmmg/branch/main/graph/badge.svg?token=VQ1J2RTC7X)](https://codecov.io/gh/ShipMMG/shipmmg)\n\n## What is it?\n\n**ShipMMG** is a unofficial Python package of ship maneuvering simulation with respect to the research committee on “standardization of mathematical model for ship maneuvering predictions” was organized by the JASNAOE.\n\n## Where to get it\nThe source code is currently hosted on GitHub at: [https://github.com/ShipMMG/shipmmg](https://github.com/ShipMMG/shipmmg)\n\nBinary installers for the latest released version will be available at the Python package index. Now, please install pDESy as following.\n\n```sh\npip install shipmmg\n# pip install git+ssh://git@github.com/ShipMMG/shipmmg.git # Install from GitHub\n# conda install -c conda-forge -c taiga4112 shipmmg # Install from Anaconda\n```\n\n## License\n[MIT](https://github.com/ShipMMG/shipmmg/blob/master/LICENSE)\n\n## Contribution\n1. Fork it ( http://github.com/ShipMMG/shipmmg/fork )\n2. Create your feature branch (git checkout -b my-new-feature)\n3. Commit your changes (git commit -am 'Add some feature')\n4. Push to the branch (git push origin my-new-feature)\n5. Create new Pull Request\n\nIf you want to join this project as a researcher, please contact [me](https://github.com/taiga4112).",
+    'long_description': "# ShipMMG: Ship Maneuvering Simulation Model\n\n[![PyPi version](https://pypip.in/v/shipmmg/badge.png)](https://pypi.org/project/shipmmg/)\n[![Anaconda-Server Badge](https://anaconda.org/taiga4112/shipmmg/badges/version.svg)](https://anaconda.org/taiga4112/shipmmg)\n![codecov](https://github.com/ShipMMG/shipmmg/workflows/codecov/badge.svg)\n[![codecov](https://codecov.io/gh/ShipMMG/shipmmg/branch/main/graph/badge.svg?token=VQ1J2RTC7X)](https://codecov.io/gh/ShipMMG/shipmmg)\n\n## What is it?\n\n**ShipMMG** is a unofficial Python package of ship maneuvering simulation with respect to the research committee on “standardization of mathematical model for ship maneuvering predictions” was organized by the JASNAOE.\n\n## Where to get it\n\nThe source code is currently hosted on GitHub at: [https://github.com/ShipMMG/shipmmg](https://github.com/ShipMMG/shipmmg)\n\nBinary installers for the latest released version will be available at the Python package index. Now, please install pDESy as following.\n\n```sh\npip install shipmmg\n# pip install git+ssh://git@github.com/ShipMMG/shipmmg.git # Install from GitHub\n# conda install -c conda-forge -c taiga4112 shipmmg # Install from Anaconda\n```\n\n## License\n\n[MIT](https://github.com/ShipMMG/shipmmg/blob/master/LICENSE)\n\n## For developers\n\n### Developing shipmmg API\n\nHere is an example of constructing a developing environment.\n\n```sh\ndocker build -t shipmmg-dev-env .\ndocker run --rm --name shipmmg-dev -v `pwd`:/code -w /code -it shipmmg-dev-env /bin/bash\n```\n\nIn this docker container, we can run `pytest` for checking this library.\n\n### Checking shipmmg API\n\nHere is an example of checking the shipmmg developing version using JupyterLab.\n\n```sh\ndocker-compose build\ndocker-compose up\n```\n\nAfter that, access [http://localhost:8888](http://localhost:8888).\n\n- Password is `shipmmg`.\n\n## Contribution\n\n1. Fork it ( <http://github.com/ShipMMG/shipmmg/fork> )\n2. Create your feature branch (git checkout -b my-new-feature)\n3. Commit your changes (git commit -am 'Add some feature')\n4. Push to the branch (git push origin my-new-feature)\n5. Create new Pull Request\n\nIf you want to join this project as a researcher, please contact [me](https://github.com/taiga4112).\n",
     'author': 'Taiga MITSUYUKI',
     'author_email': 'mitsuyuki-taiga-my@ynu.ac.jp',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ShipMMG/shipmmg',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `shipmmg-0.0.8/PKG-INFO` & `shipmmg-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: shipmmg
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package of ship maneuvering simulation
 Home-page: https://github.com/ShipMMG/shipmmg
 License: MIT
 Author: Taiga MITSUYUKI
 Author-email: mitsuyuki-taiga-my@ynu.ac.jp
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: Pillow (>=9.0.0,<10.0.0)
 Requires-Dist: matplotlib (>=3.3.3,<4.0.0)
 Requires-Dist: numpy (>=1.19.5,<2.0.0)
 Requires-Dist: pytest-cov (>=2.10.1,<3.0.0)
 Requires-Dist: scipy (>=1.6.0,<2.0.0)
 Project-URL: Documentation, https://shipmmg.github.io/shipmmg/
 Project-URL: Repository, https://github.com/ShipMMG/shipmmg
 Description-Content-Type: text/markdown
@@ -27,28 +29,58 @@
 [![codecov](https://codecov.io/gh/ShipMMG/shipmmg/branch/main/graph/badge.svg?token=VQ1J2RTC7X)](https://codecov.io/gh/ShipMMG/shipmmg)
 
 ## What is it?
 
 **ShipMMG** is a unofficial Python package of ship maneuvering simulation with respect to the research committee on “standardization of mathematical model for ship maneuvering predictions” was organized by the JASNAOE.
 
 ## Where to get it
+
 The source code is currently hosted on GitHub at: [https://github.com/ShipMMG/shipmmg](https://github.com/ShipMMG/shipmmg)
 
 Binary installers for the latest released version will be available at the Python package index. Now, please install pDESy as following.
 
 ```sh
 pip install shipmmg
 # pip install git+ssh://git@github.com/ShipMMG/shipmmg.git # Install from GitHub
 # conda install -c conda-forge -c taiga4112 shipmmg # Install from Anaconda
 ```
 
 ## License
+
 [MIT](https://github.com/ShipMMG/shipmmg/blob/master/LICENSE)
 
+## For developers
+
+### Developing shipmmg API
+
+Here is an example of constructing a developing environment.
+
+```sh
+docker build -t shipmmg-dev-env .
+docker run --rm --name shipmmg-dev -v `pwd`:/code -w /code -it shipmmg-dev-env /bin/bash
+```
+
+In this docker container, we can run `pytest` for checking this library.
+
+### Checking shipmmg API
+
+Here is an example of checking the shipmmg developing version using JupyterLab.
+
+```sh
+docker-compose build
+docker-compose up
+```
+
+After that, access [http://localhost:8888](http://localhost:8888).
+
+- Password is `shipmmg`.
+
 ## Contribution
-1. Fork it ( http://github.com/ShipMMG/shipmmg/fork )
+
+1. Fork it ( <http://github.com/ShipMMG/shipmmg/fork> )
 2. Create your feature branch (git checkout -b my-new-feature)
 3. Commit your changes (git commit -am 'Add some feature')
 4. Push to the branch (git push origin my-new-feature)
 5. Create new Pull Request
 
 If you want to join this project as a researcher, please contact [me](https://github.com/taiga4112).
+
```

