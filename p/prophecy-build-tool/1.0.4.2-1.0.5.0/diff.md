# Comparing `tmp/prophecy-build-tool-1.0.4.2.tar.gz` & `tmp/prophecy-build-tool-1.0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-build-tool-1.0.4.2.tar", last modified: Mon Mar  6 14:15:06 2023, max compression
+gzip compressed data, was "prophecy-build-tool-1.0.5.0.tar", last modified: Wed Apr 26 12:33:38 2023, max compression
```

## Comparing `prophecy-build-tool-1.0.4.2.tar` & `prophecy-build-tool-1.0.5.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-03-06 14:15:06.916007 prophecy-build-tool-1.0.4.2/
--rw-r--r--   0 kiran      (501) staff       (20)    11357 2022-08-09 06:53:00.000000 prophecy-build-tool-1.0.4.2/LICENSE
--rw-r--r--   0 kiran      (501) staff       (20)     5931 2023-03-06 14:15:06.915862 prophecy-build-tool-1.0.4.2/PKG-INFO
--rw-r--r--   0 kiran      (501) staff       (20)     5308 2023-03-06 11:00:29.000000 prophecy-build-tool-1.0.4.2/README.md
--rw-r--r--   0 kiran      (501) staff       (20)       38 2023-03-06 14:15:06.916055 prophecy-build-tool-1.0.4.2/setup.cfg
--rw-r--r--   0 kiran      (501) staff       (20)     1148 2023-03-06 14:14:57.000000 prophecy-build-tool-1.0.4.2/setup.py
-drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-03-06 14:15:06.913485 prophecy-build-tool-1.0.4.2/src/
-drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-03-06 14:15:06.914661 prophecy-build-tool-1.0.4.2/src/pbt/
--rw-r--r--   0 kiran      (501) staff       (20)     2143 2023-03-06 14:14:57.000000 prophecy-build-tool-1.0.4.2/src/pbt/__init__.py
--rw-r--r--   0 kiran      (501) staff       (20)     2102 2022-11-15 12:55:24.000000 prophecy-build-tool-1.0.4.2/src/pbt/process.py
--rw-r--r--   0 kiran      (501) staff       (20)    36471 2023-03-06 14:14:57.000000 prophecy-build-tool-1.0.4.2/src/pbt/prophecy_build_tool.py
-drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-03-06 14:15:06.915665 prophecy-build-tool-1.0.4.2/src/prophecy_build_tool.egg-info/
--rw-r--r--   0 kiran      (501) staff       (20)     5931 2023-03-06 14:15:06.000000 prophecy-build-tool-1.0.4.2/src/prophecy_build_tool.egg-info/PKG-INFO
--rw-r--r--   0 kiran      (501) staff       (20)      380 2023-03-06 14:15:06.000000 prophecy-build-tool-1.0.4.2/src/prophecy_build_tool.egg-info/SOURCES.txt
--rw-r--r--   0 kiran      (501) staff       (20)        1 2023-03-06 14:15:06.000000 prophecy-build-tool-1.0.4.2/src/prophecy_build_tool.egg-info/dependency_links.txt
--rw-r--r--   0 kiran      (501) staff       (20)       33 2023-03-06 14:15:06.000000 prophecy-build-tool-1.0.4.2/src/prophecy_build_tool.egg-info/entry_points.txt
--rw-r--r--   0 kiran      (501) staff       (20)       65 2023-03-06 14:15:06.000000 prophecy-build-tool-1.0.4.2/src/prophecy_build_tool.egg-info/requires.txt
--rw-r--r--   0 kiran      (501) staff       (20)        4 2023-03-06 14:15:06.000000 prophecy-build-tool-1.0.4.2/src/prophecy_build_tool.egg-info/top_level.txt
+drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-04-26 12:33:38.272828 prophecy-build-tool-1.0.5.0/
+-rw-r--r--   0 ashishpatel   (501) staff       (20)    11357 2023-02-21 12:57:27.000000 prophecy-build-tool-1.0.5.0/LICENSE
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     5941 2023-04-26 12:33:38.272896 prophecy-build-tool-1.0.5.0/PKG-INFO
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     5318 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/README.md
+-rw-r--r--   0 ashishpatel   (501) staff       (20)      419 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/pyproject.toml
+-rw-r--r--   0 ashishpatel   (501) staff       (20)      239 2023-04-26 12:33:38.273183 prophecy-build-tool-1.0.5.0/setup.cfg
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     1182 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/setup.py
+drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-04-26 12:33:38.270364 prophecy-build-tool-1.0.5.0/src/
+drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-04-26 12:33:38.271749 prophecy-build-tool-1.0.5.0/src/pbt/
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     2283 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/src/pbt/__init__.py
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     1941 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/src/pbt/process.py
+-rw-r--r--   0 ashishpatel   (501) staff       (20)    33775 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/src/pbt/prophecy_build_tool.py
+drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-04-26 12:33:38.272562 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     5941 2023-04-26 12:33:38.000000 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/PKG-INFO
+-rw-r--r--   0 ashishpatel   (501) staff       (20)      424 2023-04-26 12:33:38.000000 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 ashishpatel   (501) staff       (20)        1 2023-04-26 12:33:38.000000 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 ashishpatel   (501) staff       (20)       33 2023-04-26 12:33:38.000000 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/entry_points.txt
+-rw-r--r--   0 ashishpatel   (501) staff       (20)       77 2023-04-26 12:33:38.000000 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/requires.txt
+-rw-r--r--   0 ashishpatel   (501) staff       (20)        4 2023-04-26 12:33:38.000000 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/top_level.txt
+drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-04-26 12:33:38.272709 prophecy-build-tool-1.0.5.0/test/
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     2133 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/test/test_build.py
```

### Comparing `prophecy-build-tool-1.0.4.2/LICENSE` & `prophecy-build-tool-1.0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.0.4.2/PKG-INFO` & `prophecy-build-tool-1.0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.0.4.2
+Version: 1.0.5.0
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prophecy-build-tool
 
 **Prophecy** is designed to enable all users to be productive with data engineering. It also replaces legacy ETL
 products.
@@ -136,15 +136,15 @@
 pbt validate --path /path/to/your/prophecy_project/
 ```
 
 Sample output:
 ```shell
 Prophecy-build-tool v1.0.3.4
 
-Project name: HelloWorld
+Project name: resources.HelloWorld
 Found 1 jobs: default_schedule
 Found 4 pipelines: customers_orders (python), report_top_customers (python), join_agg_sort (python), farmers-markets-irs (python)
 
 Validating 4 pipelines 
 
   Validating pipeline pipelines/customers_orders [1/4]
```

### Comparing `prophecy-build-tool-1.0.4.2/README.md` & `prophecy-build-tool-1.0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 pbt validate --path /path/to/your/prophecy_project/
 ```
 
 Sample output:
 ```shell
 Prophecy-build-tool v1.0.3.4
 
-Project name: HelloWorld
+Project name: resources.HelloWorld
 Found 1 jobs: default_schedule
 Found 4 pipelines: customers_orders (python), report_top_customers (python), join_agg_sort (python), farmers-markets-irs (python)
 
 Validating 4 pipelines 
 
   Validating pipeline pipelines/customers_orders [1/4]
```

### Comparing `prophecy-build-tool-1.0.4.2/setup.py` & `prophecy-build-tool-1.0.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as _in:
     long_description = _in.read()
 
 setuptools.setup(
     name="prophecy-build-tool",
-    version="1.0.4.2",
+    version="1.0.5.0",
     author="Prophecy",
     author_email="maciej@prophecy.io",
     description="Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the "
     "Prophecy IDE.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SimpleDataLabsInc/prophecy-build-tool",
@@ -24,14 +24,16 @@
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "requests>=2.28.0",
         "PyYAML>=6.0",
         "databricks_cli>=0.17.1",
         "rich>=12.5.1",
+        "wheel",
+        "build",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     entry_points="""
         [console_scripts]
         pbt=pbt:main
     """,
 )
```

### Comparing `prophecy-build-tool-1.0.4.2/src/pbt/__init__.py` & `prophecy-build-tool-1.0.5.0/src/pbt/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,17 +15,22 @@
 
 @cli.command()
 @click.option(
     "--path",
     help="Path to the directory containing the pbt_project.yml file",
     required=True,
 )
-def build(path):
+@click.option(
+    "--pipelines",
+    help="Pipeline names(comma separated) which can be used to filter pipelines to be build",
+    default="",
+)
+def build(path, pipelines):
     pbt = ProphecyBuildTool(path)
-    pbt.build(dict())
+    pbt.build(pipelines)
 
 
 @cli.command()
 @click.option(
     "--path",
     help="Path to the directory containing the pbt_project.yml file",
     required=True,
@@ -58,29 +63,25 @@
     default="",
 )
 @click.option(
     "--fabric-ids",
     help="Fabric IDs(comma separated) which can be used to filter jobs for deployments",
     default="",
 )
-@click.option(
-    "--skip-builds", is_flag=True, default=False, help="Flag to skip building Pipelines"
-)
+@click.option("--skip-builds", is_flag=True, default=False, help="Flag to skip building Pipelines")
 def deploy(
     path,
     dependent_projects_path,
     release_version,
     project_id,
     prophecy_url,
     fabric_ids,
     skip_builds,
 ):
-    pbt = ProphecyBuildTool(
-        path, dependent_projects_path, release_version, project_id, prophecy_url
-    )
+    pbt = ProphecyBuildTool(path, dependent_projects_path, release_version, project_id, prophecy_url)
     pbt.deploy(fabric_ids, skip_builds)
 
 
 @cli.command()
 @click.option(
     "--path",
     help="Path to the directory containing the pbt_project.yml file",
```

### Comparing `prophecy-build-tool-1.0.4.2/src/pbt/process.py` & `prophecy-build-tool-1.0.5.0/src/pbt/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     def __init__(
         self,
         process_args,
         current_working_directory,
         std_output=subprocess.PIPE,
         std_err=subprocess.PIPE,
         is_shell=False,
-        running_message=""
+        running_message="",
     ):
         self.process_args = process_args
         self.current_working_directory = current_working_directory
         self.std_output = std_output
         self.std_err = std_err
         self.is_shell = is_shell
         self.running_message = running_message
@@ -38,29 +38,23 @@
                 result.stderr,
             )
 
             if stdout is not None:
                 if stderr is not None and len(stderr) > 0:
                     print(
                         "   ",
-                        "\n    ".join(
-                            [line.decode("utf-8") for line in stdout.splitlines()]
-                        ),
+                        "\n    ".join([line.decode("utf-8") for line in stdout.splitlines()]),
                     )
                     print(
                         "   ",
-                        "\n    ".join(
-                            [line.decode("utf-8") for line in stderr.splitlines()]
-                        ),
+                        "\n    ".join([line.decode("utf-8") for line in stderr.splitlines()]),
                     )
                 else:
                     print(
                         "   ",
-                        "\n    ".join(
-                            [line.decode("utf-8") for line in stdout.splitlines()]
-                        ),
+                        "\n    ".join([line.decode("utf-8") for line in stdout.splitlines()]),
                     )
 
             if return_code != 0:
                 break
             time.sleep(time_between_each_cmd)
         return return_code
```

### Comparing `prophecy-build-tool-1.0.4.2/src/pbt/prophecy_build_tool.py` & `prophecy-build-tool-1.0.5.0/src/pbt/prophecy_build_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         self,
         path_root: str,
         dependent_projects_path: str = "",
         release_version: str = "",
         project_id: str = "",
         prophecy_url: str = "",
     ):
-
         if not path_root:
             self._error("Path of project not passed as argument using --path.")
         self.operating_system = sys.platform
         self.path_root = path_root
         self.path_project = os.path.join(self.path_root, "pbt_project.yml")
 
         self._verify_project()
@@ -41,17 +40,15 @@
         if dependent_projects_path:
             print("\nParsing dependent projects")
             other_pbt_projects = glob(
                 f"{dependent_projects_path}{os.sep}**{os.sep}pbt_project.yml",
                 recursive=True,
             )
             for dependent_project in other_pbt_projects:
-                self.dependent_projects[dirname(dependent_project)] = ProphecyBuildTool(
-                    dirname(dependent_project)
-                )
+                self.dependent_projects[dirname(dependent_project)] = ProphecyBuildTool(dirname(dependent_project))
         self.dbfs_service = None
         self.jobs_service = None
         self.api_client = None
         self.python_cmd, self.pip_cmd = self.get_python_commands(path_root)
         self.pipelines_build_path = {}
         self.dependent_pipelines_build_path = {}
         self.project_release = (
@@ -59,22 +56,18 @@
             if release_version
             else os.getenv(
                 "PROJECT_RELEASE_VERSION_PLACEHOLDER",
                 "__PROJECT_RELEASE_VERSION_PLACEHOLDER__",
             )
         )
         self.project_id = (
-            project_id
-            if project_id
-            else os.getenv("PROJECT_ID_PLACEHOLDER", "__PROJECT_ID_PLACEHOLDER__")
+            project_id if project_id else os.getenv("PROJECT_ID_PLACEHOLDER", "__PROJECT_ID_PLACEHOLDER__")
         )
         self.prophecy_url = (
-            prophecy_url
-            if prophecy_url
-            else os.getenv("PROPHECY_URL_PLACEHOLDER", "__PROPHECY_URL_PLACEHOLDER__")
+            prophecy_url if prophecy_url else os.getenv("PROPHECY_URL_PLACEHOLDER", "__PROPHECY_URL_PLACEHOLDER__")
         )
 
     def get_python_commands(self, cwd):
         if (
             Process.process_sequential(
                 [
                     Process(
@@ -109,61 +102,55 @@
             sys.exit(1)
 
     def validate(self):
         pipelines = self.pipelines
         print("\n[bold blue]Validating %s pipelines [/bold blue]" % len(pipelines))
         overall_validate_status = True
         for pipeline_i, (path_pipeline, pipeline) in enumerate(pipelines.items()):
-            print(
-                "\n  Validating pipeline %s [%s/%s]"
-                % (path_pipeline, pipeline_i + 1, len(pipelines))
-            )
+            print("\n  Validating pipeline %s [%s/%s]" % (path_pipeline, pipeline_i + 1, len(pipelines)))
 
             workflow_json_path_pipeline_absolute = os.path.join(
                 os.path.join(self.path_root, path_pipeline),
                 "code",
                 ".prophecy",
                 "workflow.latest.json",
             )
             if os.path.exists(workflow_json_path_pipeline_absolute):
                 workflow = json.load(open(workflow_json_path_pipeline_absolute, "r"))
                 if "diagnostics" in workflow:
-                    print(
-                        f"\n[bold red]Pipeline is Broken: {pipeline['name']}[/bold red]"
-                    )
+                    print(f"\n[bold red]Pipeline is Broken: {pipeline['name']}[/bold red]")
                     overall_validate_status = False
                 else:
-                    print(
-                        f"\n[bold blue] Pipeline is validated: {pipeline['name']}[/bold blue]"
-                    )
+                    print(f"\n[bold blue] Pipeline is validated: {pipeline['name']}[/bold blue]")
             else:
-                print(
-                    f"\n[bold red] Empty Pipeline Found: {pipeline['name']}![/bold red]"
-                )
+                print(f"\n[bold red] Empty Pipeline Found: {pipeline['name']}![/bold red]")
                 overall_validate_status = False
 
         if not overall_validate_status:
             sys.exit(1)
         else:
             sys.exit(0)
 
     def build(self, pipelines, exit_on_build_failure=True):
-        if not pipelines:
+        if not pipelines:  # if pipelines not provided run for all pipelines
             pipelines = self.pipelines
+        else:  # else filter pipelines
+            pipeline_filter = [x.strip() for x in pipelines.split(",")]
+            print("\n[bold blue]Filtering pipelines: %s [/bold blue]" % str(pipeline_filter))
+            pipelines = {k: v for k, v in self.pipelines.items() if k.split("/")[1] in pipeline_filter}
+            if not pipelines:  # empty no matching pipeline found
+                print("\n[bold yellow]No matching pipelines found for given pipelines names: %s" % (pipeline_filter))
+                raise Exception()
+
         print("\n[bold blue]Building %s pipelines [/bold blue]" % len(pipelines))
         overall_build_status = True
         for pipeline_i, (path_pipeline, pipeline) in enumerate(pipelines.items()):
-            print(
-                "\n  Building pipeline %s [%s/%s]"
-                % (path_pipeline, pipeline_i + 1, len(pipelines))
-            )
+            print("\n  Building pipeline %s [%s/%s]" % (path_pipeline, pipeline_i + 1, len(pipelines)))
 
-            path_pipeline_absolute = os.path.join(
-                os.path.join(self.path_root, path_pipeline), "code"
-            )
+            path_pipeline_absolute = os.path.join(os.path.join(self.path_root, path_pipeline), "code")
             return_code = (
                 self.build_python(path_pipeline_absolute, path_pipeline)
                 if self.project_language == "python"
                 else self.build_scala(path_pipeline_absolute)
             )
 
             self.pipelines_build_path[path_pipeline] = None
@@ -201,93 +188,75 @@
                 else:
                     print(
                         f"\n[bold red] Build completed but built target "
                         f"not found for pipeline: {pipeline['name']}![/bold red]"
                     )
                     overall_build_status = False
             else:
-                print(
-                    f"\n[bold red] Build failed for pipeline: {pipeline['name']}![/bold red]"
-                )
+                print(f"\n[bold red] Build failed for pipeline: {pipeline['name']}![/bold red]")
                 overall_build_status = False
 
         if not overall_build_status and exit_on_build_failure:
             sys.exit(1)
         else:
             return overall_build_status, self.pipelines_build_path
 
     def deploy(self, fabric_ids: str = "", skip_builds: bool = False):
-        fabric_ids = (
-            list(i.strip() for i in fabric_ids.split(r",")) if fabric_ids else list()
-        )
+        fabric_ids = list(i.strip() for i in fabric_ids.split(r",")) if fabric_ids else list()
 
         self._verify_databricks_configs()
         config = EnvironmentVariableConfigProvider().get_config()
 
         self.api_client = _get_api_client(config)
 
         self.dbfs_service = DbfsService(self.api_client)
         self.jobs_service = JobsService(self.api_client)
 
         if not skip_builds:
             self.build(dict())
         else:
-            print(
-                "[SKIP]: Skipping builds for all pipelines as '--skip-builds' flag is passed."
-            )
+            print("[SKIP]: Skipping builds for all pipelines as '--skip-builds' flag is passed.")
 
         print("\n[bold blue] Deploying %s jobs [/bold blue]" % self.jobs_count)
 
         pipelines_upload_failures = collections.defaultdict(list)
         job_update_failures = dict()
 
         if not fabric_ids:
             print("Deploying jobs for all Fabrics")
         else:
             print("Deploying jobs only for given Fabric IDs: %s" % (str(fabric_ids)))
 
         for job_idx, (path_job, job) in enumerate(self.jobs.items()):
             pipelines_upload_failures_job = collections.defaultdict(list)
-            print(
-                "\n[START]:  Deploying job %s [%s/%s]"
-                % (path_job, job_idx + 1, self.jobs_count)
-            )
+            print("\n[START]:  Deploying job %s [%s/%s]" % (path_job, job_idx + 1, self.jobs_count))
 
-            path_job_absolute = os.path.join(
-                os.path.join(self.path_root, path_job), "code"
-            )
+            path_job_absolute = os.path.join(os.path.join(self.path_root, path_job), "code")
             path_job_definition = os.path.join(path_job_absolute, "databricks-job.json")
 
             with open(path_job_definition, "r") as _in:
                 data = _in.read()
                 data = (
-                    data.replace(
-                        "__PROJECT_RELEASE_VERSION_PLACEHOLDER__", self.project_release
-                    )
+                    data.replace("__PROJECT_RELEASE_VERSION_PLACEHOLDER__", self.project_release)
                     .replace("__PROJECT_ID_PLACEHOLDER__", self.project_id)
                     .replace("__PROPHECY_URL_PLACEHOLDER__", self.prophecy_url)
                 )
             with open(path_job_definition, "w") as _out:
                 _out.write(data)
 
             with open(path_job_definition, "r") as _in:
                 job_definition = json.load(_in)
 
             components = job_definition["components"]
             fabric_id = job_definition["fabric_id"]
 
             # if --fabric is passed, then only deploy jobs
             if fabric_ids:
-                if (
-                    fabric_id not in fabric_ids
-                ):  # Jobs for this fabric id should be skipped
-                    print(
-                        "[SKIP]: Job skipped as it belongs to fabric id (not passed): %s"
-                        % fabric_id
-                    )
+                if fabric_id not in fabric_ids:  # Jobs for this fabric id should be skipped
+                    print("[SKIP]: Job skipped as it belongs to fabric id (not passed): %s" % fabric_id)
                     continue
                 else:
                     print("[DEPLOY]: Job being deployed for fabric id: %s" % fabric_id)
 
             generate_pipeline_config_from_pipeline_component = False
 
             for component in components:
@@ -307,140 +276,103 @@
                         # Check if this shared pipelineComponent has configs
                         dependent_pipeline_regex_pattern = (
                             "(^[0-9]+?\/pipelines\/[-_.A-Za-z0-9 \/]+)$"
                             "|^.*projectSubscriptionProjectId=([0-9]+).*path=([-_.A-Za-z0-9 \/]+).*$"
                             "|^.*path=([-_.A-Za-z0-9 \/]+).*projectSubscriptionProjectId=([0-9]+).*$"
                         )
                         print(f"Parsing basepipeline: {pipeline_uri}")
-                        search_regex_id = re.search(
-                            dependent_pipeline_regex_pattern, pipeline_uri
-                        )
-                        if (
-                            bool(search_regex_id)
-                            and "configPath" in component["PipelineComponent"]
-                        ):
+                        search_regex_id = re.search(dependent_pipeline_regex_pattern, pipeline_uri)
+                        if bool(search_regex_id) and "configPath" in component["PipelineComponent"]:
                             generate_pipeline_config_from_pipeline_component = True
                             shared_pipeline_id = ""
                             if bool(search_regex_id.group(1)):
                                 shared_pipeline_id = search_regex_id.group(1)
-                            elif bool(search_regex_id.group(2)) and bool(
-                                search_regex_id.group(3)
-                            ):
+                            elif bool(search_regex_id.group(2)) and bool(search_regex_id.group(3)):
                                 shared_pipeline_id = f"{search_regex_id.group(2)}/{search_regex_id.group(3)}"
-                            elif bool(search_regex_id.group(4)) and bool(
-                                search_regex_id.group(5)
-                            ):
+                            elif bool(search_regex_id.group(4)) and bool(search_regex_id.group(5)):
                                 shared_pipeline_id = f"{search_regex_id.group(5)}/{search_regex_id.group(4)}"
                             else:
                                 generate_pipeline_config_from_pipeline_component = False
-                            self.pipeline_to_dbfs_config_path[
-                                shared_pipeline_id
-                            ] = component["PipelineComponent"]["configPath"]
+                            self.pipeline_to_dbfs_config_path[shared_pipeline_id] = component["PipelineComponent"][
+                                "configPath"
+                            ]
 
-                            print(
-                                f"Shared pipeline id for {pipeline_uri} is {shared_pipeline_id}"
-                            )
+                            print(f"Shared pipeline id for {pipeline_uri} is {shared_pipeline_id}")
 
-                        print(
-                            f"    Pipeline {pipeline_id} might be shared, checking if it exists in DBFS"
-                        )
+                        print(f"    Pipeline {pipeline_id} might be shared, checking if it exists in DBFS")
 
                         # This jar is from a shared pipeline, check if jar exists in DBFS
                         try:
-                            if self.dbfs_service.get_status(
-                                component["PipelineComponent"]["path"]
-                            ):
-                                print(
-                                    "    Dependent package exists on DBFS already, continuing with next pipeline"
-                                )
+                            if self.dbfs_service.get_status(component["PipelineComponent"]["path"]):
+                                print("    Dependent package exists on DBFS already, continuing with next pipeline")
                                 continue
                         except HTTPError as e:
                             dependent_build_jar_found = False
                             if e.response.status_code == 404:
                                 # Pipeline not found on DBFS. Check if it is present in dependency folder
                                 # and try to build it ourselves
                                 print(
                                     f"    Pipeline {pipeline_id} not found in DFBS, "
                                     f"searching in dependent project directory"
                                 )
                                 for project in self.dependent_projects.values():
                                     if (
                                         pipeline_id in project.pipelines
-                                        and self.project_language
-                                        == project.project_language
+                                        and self.project_language == project.project_language
                                     ):
-                                        print(
-                                            "    Building dependent project's pipeline:"
-                                        )
+                                        print("    Building dependent project's pipeline:")
                                         (
                                             dependent_build_status,
                                             dependent_build_paths,
                                         ) = project.build(
                                             {
                                                 k: v
                                                 for (k, v) in project.pipelines.items()
                                                 if pipeline_id in project.pipelines
                                             },
                                             False,
                                         )
                                         if dependent_build_status:
                                             dependent_build_jar_found = True
-                                            self.dependent_pipelines_build_path[
+                                            self.dependent_pipelines_build_path[pipeline_id] = dependent_build_paths[
                                                 pipeline_id
-                                            ] = dependent_build_paths[pipeline_id]
+                                            ]
                             if not dependent_build_jar_found:
-                                pipelines_upload_failures_job[pipeline_id].append(
-                                    e.response.text
-                                )
-                                pipelines_upload_failures[pipeline_id].append(
-                                    e.response.text
-                                )
+                                pipelines_upload_failures_job[pipeline_id].append(e.response.text)
+                                pipelines_upload_failures[pipeline_id].append(e.response.text)
                         except Exception as ex:
                             self.pipelines_build_path[pipeline_id]["uploaded"] = False
                             pipelines_upload_failures_job[pipeline_id].append(str(ex))
                             pipelines_upload_failures[pipeline_id].append(str(ex))
-                    if (
-                        pipeline_id in self.pipelines_build_path
-                        or pipeline_id in self.dependent_pipelines_build_path
-                    ):
+                    if pipeline_id in self.pipelines_build_path or pipeline_id in self.dependent_pipelines_build_path:
                         pipelines_build_path = (
                             self.pipelines_build_path
                             if pipeline_id in self.pipelines_build_path
                             else self.dependent_pipelines_build_path
                         )
-                        source_path = pipelines_build_path[pipeline_id][
-                            "source_absolute"
-                        ]
+                        source_path = pipelines_build_path[pipeline_id]["source_absolute"]
                         target_path = component["PipelineComponent"]["path"]
                         if not pipelines_build_path[pipeline_id]["uploaded"]:
                             print(
                                 "    Uploading %s to %s"
                                 % (
                                     pipelines_build_path[pipeline_id]["source"],
                                     target_path,
                                 )
                             )
 
                             try:
-                                self.dbfs_service.put(
-                                    target_path, overwrite=True, src_path=source_path
-                                )
+                                self.dbfs_service.put(target_path, overwrite=True, src_path=source_path)
                                 pipelines_build_path[pipeline_id]["uploaded"] = True
                             except HTTPError as e:
-                                pipelines_upload_failures_job[pipeline_id].append(
-                                    e.response.text
-                                )
-                                pipelines_upload_failures[pipeline_id].append(
-                                    e.response.text
-                                )
+                                pipelines_upload_failures_job[pipeline_id].append(e.response.text)
+                                pipelines_upload_failures[pipeline_id].append(e.response.text)
                             except Exception as ex:
                                 pipelines_build_path[pipeline_id]["uploaded"] = False
-                                pipelines_upload_failures_job[pipeline_id].append(
-                                    str(ex)
-                                )
+                                pipelines_upload_failures_job[pipeline_id].append(str(ex))
                                 pipelines_upload_failures[pipeline_id].append(str(ex))
 
             job_request = job_definition["request"]
             if "CreateNewJobRequest" in job_request.keys():
                 job_request = job_definition["request"]["CreateNewJobRequest"]
 
             job_request["version"] = "2.1"
@@ -450,76 +382,56 @@
             local_path_dbfs_map = dict()
             if generate_pipeline_config_from_pipeline_component:
                 for (
                     base_pipeline_id,
                     local_config_path,
                 ) in self.pipeline_to_local_config_path.items():
                     if base_pipeline_id in self.pipeline_to_dbfs_config_path:
-                        local_path_dbfs_map[
-                            local_config_path
-                        ] = self.pipeline_to_dbfs_config_path[base_pipeline_id]
+                        local_path_dbfs_map[local_config_path] = self.pipeline_to_dbfs_config_path[base_pipeline_id]
             else:
-                json_configs = self._get_spark_parameter_files(
-                    job_request["tasks"], ".json"
-                )
+                json_configs = self._get_spark_parameter_files(job_request["tasks"], ".json")
 
-                local_path_dbfs_map = self._construct_local_config_to_dbfs_config_path(
-                    json_configs
-                )
+                local_path_dbfs_map = self._construct_local_config_to_dbfs_config_path(json_configs)
 
             for local_json_directory, dbfs_directory in local_path_dbfs_map.items():
                 files = [
                     join(local_json_directory, f)
                     for f in listdir(local_json_directory)
                     if isfile(join(local_json_directory, f))
                 ]
                 for file_path in files:
                     dbfs_file_path = join(dbfs_directory, basename(file_path))
                     try:
                         print(f"    Uploading {file_path} to {dbfs_file_path}")
-                        self.dbfs_service.put(
-                            dbfs_file_path, overwrite=True, src_path=file_path
-                        )
+                        self.dbfs_service.put(dbfs_file_path, overwrite=True, src_path=file_path)
                     except Exception as e:
-                        print(
-                            f"    Failed to upload {file_path} to {dbfs_file_path}. Exception: {e}"
-                        )
+                        print(f"    Failed to upload {file_path} to {dbfs_file_path}. Exception: {e}")
 
             if len(pipelines_upload_failures_job) > 0:
-                print(
-                    "\n[bold red] Package upload failed or doesn't exist for one or more pipelines [/bold red]"
-                )
+                print("\n[bold red] Package upload failed or doesn't exist for one or more pipelines [/bold red]")
                 for pipeline_id, errors in pipelines_upload_failures_job.items():
-                    print(
-                        "\n[bold red] %s: Exceptions: %s [/bold red]"
-                        % (pipeline_id, "\n".join(errors))
-                    )
+                    print("\n[bold red] %s: Exceptions: %s [/bold red]" % (pipeline_id, "\n".join(errors)))
 
                 # Process next job
                 continue
 
             limit = 25
             current_offset = 0
             found_job = None
             try:
                 while found_job is None:
                     print(
                         f"    Querying existing jobs to find current job: Offset: {current_offset}, Pagesize: {limit}"
                     )
-                    response = self.jobs_service.list_jobs(
-                        limit=limit, offset=current_offset, version="2.1"
-                    )
+                    response = self.jobs_service.list_jobs(limit=limit, offset=current_offset, version="2.1")
                     current_offset += limit
 
                     found_jobs = response["jobs"] if "jobs" in response else []
                     for potential_found_job in found_jobs:
-                        if (
-                            potential_found_job["settings"]["name"]
-                            == job_request["name"]
-                        ):
+                        if potential_found_job["settings"]["name"] == job_request["name"]:
                             found_job = potential_found_job
                             break
 
                     if len(found_jobs) <= 0:
                         break
 
                 job_request = job_definition["request"]
@@ -527,79 +439,54 @@
                     job_request = job_definition["request"]["CreateNewJobRequest"]
 
                 if found_job is None:
                     print("    Creating a new job: %s" % (job_request["name"]))
                     self.jobs_service.create_job(**job_request)
                 else:
                     print("    Updating an existing job: %s" % (job_request["name"]))
-                    self.jobs_service.reset_job(
-                        found_job["job_id"], new_settings=job_request, version="2.1"
-                    )
+                    self.jobs_service.reset_job(found_job["job_id"], new_settings=job_request, version="2.1")
             except Exception as e:
                 print(
                     f"\n[bold red] Create/Update for job: {job_request['name']} failed with exception: {e} [/bold red]"
                 )
                 job_update_failures[job_request["name"]] = str(e)
 
         if len(pipelines_upload_failures) == 0 and len(job_update_failures) == 0:
             print("\n[bold blue][DONE]: Deployment completed successfully![/bold blue]")
         else:
             print("\n[bold red] Deployment failed![/bold red]")
             if len(pipelines_upload_failures) > 0:
-                print(
-                    "   Pipeline failures: %s"
-                    % (" ,".join(pipelines_upload_failures.keys()))
-                )
+                print("   Pipeline failures: %s" % (" ,".join(pipelines_upload_failures.keys())))
             if len(job_update_failures) > 0:
-                print(
-                    "   Create/Update failed for jobs: %s"
-                    % (" ,".join(job_update_failures.keys()))
-                )
+                print("   Create/Update failed for jobs: %s" % (" ,".join(job_update_failures.keys())))
             sys.exit(1)
 
     def test(self):
         if self._verify_unit_test_env():
             unit_test_results = {}
 
-            for pipeline_i, (path_pipeline, pipeline) in enumerate(
-                self.pipelines.items()
-            ):
-                print(
-                    "\n  Unit Testing pipeline %s [%s/%s]"
-                    % (path_pipeline, pipeline_i + 1, self.pipelines_count)
-                )
+            for pipeline_i, (path_pipeline, pipeline) in enumerate(self.pipelines.items()):
+                print("\n  Unit Testing pipeline %s [%s/%s]" % (path_pipeline, pipeline_i + 1, self.pipelines_count))
 
-                path_pipeline_absolute = os.path.join(
-                    os.path.join(self.path_root, path_pipeline), "code"
-                )
+                path_pipeline_absolute = os.path.join(os.path.join(self.path_root, path_pipeline), "code")
                 if self.project_language == "python":
-                    if os.path.isfile(
-                        os.path.join(
-                            path_pipeline_absolute, f"test{os.sep}TestSuite.py"
-                        )
-                    ):
-                        unit_test_results[path_pipeline] = self.test_python(
-                            path_pipeline_absolute, path_pipeline
-                        )
+                    if os.path.isfile(os.path.join(path_pipeline_absolute, f"test{os.sep}TestSuite.py")):
+                        unit_test_results[path_pipeline] = self.test_python(path_pipeline_absolute, path_pipeline)
                 elif self.project_language == "scala":
-                    unit_test_results[path_pipeline] = self.test_scala(
-                        path_pipeline_absolute
-                    )
+                    unit_test_results[path_pipeline] = self.test_scala(path_pipeline_absolute)
             is_any_ut_failed = False
             for path_pipeline, return_code in unit_test_results.items():
                 if return_code not in (0, 5):
                     is_any_ut_failed = True
                     print(
                         f"\n[bold red] Unit test for pipeline: {path_pipeline} failed "
                         f"with return code {return_code}![/bold red]"
                     )
                 else:
-                    print(
-                        f"\n[bold blue] Unit test for pipeline: {path_pipeline} succeeded.[/bold blue]"
-                    )
+                    print(f"\n[bold blue] Unit test for pipeline: {path_pipeline} succeeded.[/bold blue]")
 
             if is_any_ut_failed:
                 sys.exit(1)
         else:
             sys.exit(1)
 
     def get_python_dependencies(self, path_pipeline_absolute, path_pipeline):
@@ -614,34 +501,30 @@
                         is_shell=(self.operating_system == "win32"),
                         running_message="    Getting Python dependencies...",
                     )
                 ]
             )
             == 0
         ):
-            egg_info_requires_glob = glob(
-                f"{path_pipeline_absolute}/**/*.egg-info/requires.txt", recursive=True
-            )
+            egg_info_requires_glob = glob(f"{path_pipeline_absolute}/**/*.egg-info/requires.txt", recursive=True)
             if not egg_info_requires_glob:
                 print(f"Failed to get python dependencies for {path_pipeline}")
             else:
                 egg_info_requires = egg_info_requires_glob[0]
                 for line in open(egg_info_requires, "r"):
                     if not line.lstrip().startswith("[") and line.strip():
                         python_dependencies.append(line.strip())
         else:
             print(f"Failed to get python dependencies for {path_pipeline}")
 
         print(f"    Dependencies found for {path_pipeline}: {python_dependencies}")
         return python_dependencies
 
     def build_python(self, path_pipeline_absolute, path_pipeline):
-        python_dependencies = self.get_python_dependencies(
-            path_pipeline_absolute, path_pipeline
-        )
+        python_dependencies = self.get_python_dependencies(path_pipeline_absolute, path_pipeline)
 
         install_python_dependencies_cmd = (
             [self.pip_cmd, "install", "-q"] + python_dependencies
             if python_dependencies
             else [
                 # this is just a fallback in case reading dependencies from setup.py fails
                 self.pip_cmd,
@@ -708,17 +591,15 @@
                     [self.python_cmd, "setup.py", "-q", "egg_info"],
                     path_pipeline_absolute,
                     is_shell=(self.operating_system == "win32"),
                 ),
                 # 2. Extract the install_requires and extra_requires and install them
                 Process(
                     [self.pip_cmd, "install", "-q"]
-                    + self.get_python_dependencies(
-                        path_pipeline_absolute, path_pipeline
-                    ),
+                    + self.get_python_dependencies(path_pipeline_absolute, path_pipeline),
                     path_pipeline_absolute,
                     is_shell=(self.operating_system == "win32"),
                 ),
                 # Run the unit test
                 Process(
                     [
                         self.python_cmd,
@@ -745,30 +626,26 @@
         self.pipelines: Dict = {}
         self.jobs: Dict = {}
         with open(self.path_project, "r") as _in:
             self.project = yaml.safe_load(_in)
             self.jobs = self.project["jobs"]
             self.pipelines = self.project["pipelines"]
             self.project_language = self.project["language"]
-            self.pipeline_configurations = dict(
-                self.project.get("pipelineConfigurations", [])
-            )
+            self.pipeline_configurations = dict(self.project.get("pipelineConfigurations", []))
             self.pipeline_to_local_config_path = {}
             self.pipeline_to_dbfs_config_path = {}
             for (
                 pipeline_config_path,
                 pipeline_config_object,
             ) in self.pipeline_configurations.items():
-                self.pipeline_to_local_config_path[
-                    pipeline_config_object["basePipeline"]
-                ] = os.path.join(self.path_root, pipeline_config_path)
+                self.pipeline_to_local_config_path[pipeline_config_object["basePipeline"]] = os.path.join(
+                    self.path_root, pipeline_config_path
+                )
         if self.project_language not in ("python", "scala"):
-            self._error(
-                f"Language: [i]{self.project_language}[/i] not supported by Prophecy-Build-Tool right now."
-            )
+            self._error(f"Language: [i]{self.project_language}[/i] not supported by Prophecy-Build-Tool right now.")
 
         self.pipelines_count = len(self.pipelines)
         self.jobs_count = len(self.jobs)
 
         jobs_str = ", ".join(map(lambda job: job["name"], self.jobs.values()))
         print(f"Project name: {self.project['name']}")
         print("Found %s jobs: %s" % (self.jobs_count, jobs_str))
@@ -780,48 +657,34 @@
             )
         )
         print("Found %s pipelines: %s" % (self.pipelines_count, pipelines_str))
         self._verify_project_structure()
 
     def _verify_project_structure(self):
         for path_pipeline, pipeline in self.pipelines.items():
-            path_pipeline_absolute = os.path.join(
-                os.path.join(self.path_root, path_pipeline), "code"
-            )
-            pipeline_dependencies_file = (
-                "setup.py" if self.project_language == "python" else "pom.xml"
-            )
+            path_pipeline_absolute = os.path.join(os.path.join(self.path_root, path_pipeline), "code")
+            pipeline_dependencies_file = "setup.py" if self.project_language == "python" else "pom.xml"
 
-            if not os.path.isfile(
-                os.path.join(path_pipeline_absolute, pipeline_dependencies_file)
-            ):
-                print(
-                    f"\n[bold red]Pipeline {path_pipeline} does not exist or is corrupted. [/bold red]"
-                )
+            if not os.path.isfile(os.path.join(path_pipeline_absolute, pipeline_dependencies_file)):
+                print(f"\n[bold red]Pipeline {path_pipeline} does not exist or is corrupted. [/bold red]")
                 sys.exit(1)
 
         for path_job, job in self.jobs.items():
             path_job_definition = os.path.join(
                 os.path.join(self.path_root, path_job),
                 f"code{os.sep}databricks-job.json",
             )
 
             if not os.path.isfile(path_job_definition):
-                print(
-                    f"\n[bold red]Job {path_job} does not exist or is corrupted. [/bold red]"
-                )
+                print(f"\n[bold red]Job {path_job} does not exist or is corrupted. [/bold red]")
                 sys.exit(1)
 
     def _get_spark_parameter_files(self, tasks_list, file_extension):
         result = []
-        package_field = (
-            "spark_jar_task"
-            if self.project_language == "scala"
-            else "python_wheel_task"
-        )
+        package_field = "spark_jar_task" if self.project_language == "scala" else "python_wheel_task"
         for task in tasks_list:
             if package_field in task and "parameters" in task[package_field]:
                 params = [
                     file.replace("/dbfs/", "dbfs:/")
                     for file in list(task[package_field]["parameters"])
                     if file.endswith(file_extension)
                 ]
@@ -832,17 +695,15 @@
         local_config_to_dbfs_config_path_map = {}
         for json_config in json_configs:
             for (
                 pipeline_id,
                 pipeline_config_path,
             ) in self.pipeline_to_local_config_path.items():
                 if pipeline_id in json_config:
-                    local_config_to_dbfs_config_path_map[
-                        pipeline_config_path
-                    ] = os.path.dirname(json_config)
+                    local_config_to_dbfs_config_path_map[pipeline_config_path] = os.path.dirname(json_config)
 
         return local_config_to_dbfs_config_path_map
 
     @classmethod
     def _verify_databricks_configs(cls, exit_on_failure=True):
         host = os.environ.get("DATABRICKS_HOST")
         token = os.environ.get("DATABRICKS_TOKEN")
```

### Comparing `prophecy-build-tool-1.0.4.2/src/prophecy_build_tool.egg-info/PKG-INFO` & `prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.0.4.2
+Version: 1.0.5.0
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prophecy-build-tool
 
 **Prophecy** is designed to enable all users to be productive with data engineering. It also replaces legacy ETL
 products.
@@ -136,15 +136,15 @@
 pbt validate --path /path/to/your/prophecy_project/
 ```
 
 Sample output:
 ```shell
 Prophecy-build-tool v1.0.3.4
 
-Project name: HelloWorld
+Project name: resources.HelloWorld
 Found 1 jobs: default_schedule
 Found 4 pipelines: customers_orders (python), report_top_customers (python), join_agg_sort (python), farmers-markets-irs (python)
 
 Validating 4 pipelines 
 
   Validating pipeline pipelines/customers_orders [1/4]
```

