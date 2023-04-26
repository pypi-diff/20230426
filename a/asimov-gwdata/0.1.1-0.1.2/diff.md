# Comparing `tmp/asimov-gwdata-0.1.1.tar.gz` & `tmp/asimov-gwdata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asimov-gwdata-0.1.1.tar", last modified: Wed Apr 19 17:28:08 2023, max compression
+gzip compressed data, was "asimov-gwdata-0.1.2.tar", last modified: Wed Apr 26 09:16:39 2023, max compression
```

## Comparing `asimov-gwdata-0.1.1.tar` & `asimov-gwdata-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      148 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-19 17:28:08.000000 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      452 2023-04-19 17:28:08.000000 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-19 17:28:08.000000 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      104 2023-04-19 17:28:08.000000 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       45 2023-04-19 17:28:08.000000 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-04-19 17:28:08.000000 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/blueprints/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      168 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/blueprints/asimov-analysis.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/datafind/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-02-19 16:31:31.000000 asimov-gwdata-0.1.1/datafind/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5650 2023-04-19 17:27:01.000000 asimov-gwdata-0.1.1/datafind/asimov.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1273 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/datafind/datafind_template.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3349 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/datafind/main.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1037 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/pyproject.toml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/scripts/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      251 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/scripts/asimov-test-script.sh
--rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/scripts/test-calibration-dump.yaml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)      122 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/test_settings.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      148 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-26 09:16:39.000000 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      452 2023-04-26 09:16:39.000000 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-26 09:16:39.000000 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      104 2023-04-26 09:16:39.000000 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       45 2023-04-26 09:16:39.000000 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-04-26 09:16:39.000000 asimov-gwdata-0.1.2/asimov_gwdata.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/blueprints/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      168 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/blueprints/asimov-analysis.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/datafind/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-02-19 16:31:31.000000 asimov-gwdata-0.1.2/datafind/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5590 2023-04-26 06:19:27.000000 asimov-gwdata-0.1.2/datafind/asimov.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1273 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/datafind/datafind_template.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3349 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/datafind/main.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1037 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/pyproject.toml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/scripts/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      251 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/scripts/asimov-test-script.sh
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/scripts/test-calibration-dump.yaml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-26 09:16:39.242146 asimov-gwdata-0.1.2/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      122 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.2/test_settings.yaml
```

### Comparing `asimov-gwdata-0.1.1/PKG-INFO` & `asimov-gwdata-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asimov-gwdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: An asimov plugin to make downloading gravitational wave data easier
 Author-email: Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/asimov/asimov-gwdatahelp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asimov-gwdata-0.1.1/asimov_gwdata.egg-info/PKG-INFO` & `asimov-gwdata-0.1.2/asimov_gwdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asimov-gwdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: An asimov plugin to make downloading gravitational wave data easier
 Author-email: Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/asimov/asimov-gwdatahelp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asimov-gwdata-0.1.1/datafind/asimov.py` & `asimov-gwdata-0.1.2/datafind/asimov.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import importlib
 import os
 import configparser
 import glob
 
 import asimov.pipeline
+
 from asimov import config
 import htcondor
 from asimov.utils import set_directory
 
 
 class Pipeline(asimov.pipeline.Pipeline):
     """
     An asimov pipeline for datafind.
     """
-    
+
     name = "gwdata"
     with importlib.resources.path("datafind", "datafind_template.yml") as template_file:
         config_template = template_file
     _pipeline_command = "gwdata"
 
     def _substitute_locations_in_config(self):
         """
@@ -30,42 +31,41 @@
         """
         name = self.production.name
         ini = self.production.event.repository.find_prods(name, self.category)[0]
         with open(ini, "r") as config_file:
             data = config_file.read()
         data = data.replace("<event>", self.production.event.name)
         data = data.replace("<gid>", self.production.event.meta['ligo']['preferred event'])
-        print(data)
+        self.logger.info(data)
         with open(ini, "w") as config_file:
             config_file.write(data)
         
     def build_dag(self, dryrun=False):
         """
         Create a condor submission description.
         """
         name = self.production.name  # meta['name']
         ini = self.production.event.repository.find_prods(name, self.category)[0]
         self._substitute_locations_in_config()
         executable = os.path.join(config.get('pipelines', 'environment'), 'bin', self._pipeline_command)
-        command  = ["--settings", ini]
+        command = ["--settings", ini]
         full_command = executable + " " + " ".join(command)
         self.logger.info(full_command)
 
         description = {
             "executable": f"{executable}",
             "arguments": f"{' '.join(command)}",
             "output": f"{name}.out",
             "error": f"{name}.err",
             "log": f"{name}.log",
             "request_disk": "1024",
             "request_memory": "1024",
             "batch_name": f"gwdata/{name}",
             "accounting_group_user": config.get('condor', 'user'),
             "accounting_group": self.production.meta['scheduler']["accounting group"],
-
         }
 
         job = htcondor.Submit(description)
         os.makedirs(self.production.rundir, exist_ok=True)
         with set_directory(self.production.rundir):
             with open(f"{name}.sub", "w") as subfile:
                 subfile.write(job.__str__())
@@ -79,17 +79,17 @@
                     htcondor.DaemonTypes.Schedd, config.get("condor", "scheduler")
                 )
             except configparser.NoOptionError:
                 schedulers = htcondor.Collector().locate(htcondor.DaemonTypes.Schedd)
             schedd = htcondor.Schedd(schedulers)
             with schedd.transaction() as txn:
                 cluster_id = job.queue(txn)
+                self.logger.info("Submitted to htcondor job queue.")
 
         self.production.job_id = int(cluster_id)
-        print(cluster_id)
         self.clusterid = cluster_id
 
     def submit_dag(self, dryrun=False):
         self.production.status = "running"
         self.production.job_id = int(self.clusterid)
         return self.clusterid
 
@@ -101,15 +101,16 @@
             return True
         else:
             self.logger.info("Datafind job completion was not detected.")
             return False
 
     def after_completion(self):
         self.production.status = "uploaded"
-    
+        self.production.event.update_data()
+
     def collect_assets(self):
         """
         Collect the assets for this job.
         """
         outputs = {}
         if os.path.exists(f"{self.production.rundir}/frames/"):
             results_dir = glob.glob(f"{self.production.rundir}/frames/*")
@@ -118,43 +119,39 @@
             for frame in results_dir:
                 ifo = frame.split("/")[-1].split("_")[0].split("-")[1]
                 frames[ifo] = frame
 
             outputs["frames"] = frames
 
             self.production.event.meta['data']['data files'] = frames
-            self.production.event.update_data()
 
         if os.path.exists(f"{self.production.rundir}/psds/"):
             results_dir = glob.glob(f"{self.production.rundir}/psds/*")
             psds = {}
 
             for psd in results_dir:
                 ifo = psds.split(".")[0]
                 psds[ifo] = psd
 
             outputs["psds"] = psds
 
         # TODO: Need to have this check the sample rate before it saves to ledger
         # self.production.event.meta['data']['data files'] = frames
-        self.production.event.update_data()
 
         if os.path.exists(f"{self.production.rundir}/calibration/"):
             results_dir = glob.glob(f"{self.production.rundir}/calibration/*")
             calibration = {}
 
             for cal in results_dir:
                 ifo = cal.split(".")[0]
                 calibration[ifo] = cal
 
             outputs["calibration"] = calibration
 
             self.production.event.meta['data']['calibration'] = calibration
-            self.production.event.update_data()
 
         if os.path.exists(f"{self.production.rundir}/posterior/"):
             results = glob.glob(f"{self.production.rundir}/posterior/*")
 
             outputs["samples"] = results[0]
 
-        
         return outputs
```

### Comparing `asimov-gwdata-0.1.1/datafind/datafind_template.yml` & `asimov-gwdata-0.1.2/datafind/datafind_template.yml`

 * *Files identical despite different names*

### Comparing `asimov-gwdata-0.1.1/datafind/main.py` & `asimov-gwdata-0.1.2/datafind/main.py`

 * *Files identical despite different names*

### Comparing `asimov-gwdata-0.1.1/pyproject.toml` & `asimov-gwdata-0.1.2/pyproject.toml`

 * *Files identical despite different names*

