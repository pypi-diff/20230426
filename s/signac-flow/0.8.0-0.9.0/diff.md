# Comparing `tmp/signac_flow-0.8.0-py2.py3-none-any.whl.zip` & `tmp/signac_flow-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,73 +1,69 @@
-Zip file size: 109989 bytes, number of entries: 71
--rw-r--r--  2.0 unx     1439 b- defN 19-Sep-01 14:44 flow/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 19-Sep-01 14:44 flow/__main__.py
--rw-r--r--  2.0 unx    14203 b- defN 19-Sep-01 14:44 flow/environment.py
--rw-r--r--  2.0 unx     1314 b- defN 19-Sep-01 14:44 flow/errors.py
--rw-r--r--  2.0 unx     1411 b- defN 19-Sep-01 14:44 flow/labels.py
--rw-r--r--  2.0 unx     1023 b- defN 19-Sep-01 14:44 flow/legacy.py
--rw-r--r--  2.0 unx    11301 b- defN 19-Sep-01 14:44 flow/legacy_templating.py
--rw-r--r--  2.0 unx     8087 b- defN 19-Sep-01 14:44 flow/operations.py
--rw-r--r--  2.0 unx   119281 b- defN 19-Sep-01 14:44 flow/project.py
--rw-r--r--  2.0 unx     3642 b- defN 19-Sep-01 14:44 flow/template.py
--rw-r--r--  2.0 unx      667 b- defN 19-Sep-01 14:44 flow/testing.py
--rw-r--r--  2.0 unx      475 b- defN 19-Sep-01 14:44 flow/environments/__init__.py
--rw-r--r--  2.0 unx     3607 b- defN 19-Sep-01 14:44 flow/environments/incite.py
--rw-r--r--  2.0 unx     1077 b- defN 19-Sep-01 14:44 flow/environments/umich.py
--rw-r--r--  2.0 unx     2880 b- defN 19-Sep-01 14:44 flow/environments/xsede.py
--rw-r--r--  2.0 unx      392 b- defN 19-Sep-01 14:44 flow/scheduling/__init__.py
--rw-r--r--  2.0 unx     1994 b- defN 19-Sep-01 14:44 flow/scheduling/base.py
--rw-r--r--  2.0 unx      997 b- defN 19-Sep-01 14:44 flow/scheduling/fakescheduler.py
--rw-r--r--  2.0 unx     4662 b- defN 19-Sep-01 14:44 flow/scheduling/lsf.py
--rw-r--r--  2.0 unx     1258 b- defN 19-Sep-01 14:44 flow/scheduling/simple_scheduler.py
--rw-r--r--  2.0 unx     4806 b- defN 19-Sep-01 14:44 flow/scheduling/slurm.py
--rw-r--r--  2.0 unx     1514 b- defN 19-Sep-01 14:44 flow/scheduling/status.py
--rw-r--r--  2.0 unx     5522 b- defN 19-Sep-01 14:44 flow/scheduling/torque.py
--rw-r--r--  2.0 unx      979 b- defN 19-Sep-01 14:44 flow/templates/base_script.sh
--rw-r--r--  2.0 unx     2926 b- defN 19-Sep-01 14:44 flow/templates/base_status.jinja
--rw-r--r--  2.0 unx     1857 b- defN 19-Sep-01 14:44 flow/templates/base_status_compact.jinja
--rw-r--r--  2.0 unx     1116 b- defN 19-Sep-01 14:44 flow/templates/base_status_expand.jinja
--rw-r--r--  2.0 unx      814 b- defN 19-Sep-01 14:44 flow/templates/base_status_stack.jinja
--rw-r--r--  2.0 unx     1902 b- defN 19-Sep-01 14:44 flow/templates/bridges.sh
--rw-r--r--  2.0 unx     1671 b- defN 19-Sep-01 14:44 flow/templates/comet.sh
--rw-r--r--  2.0 unx      752 b- defN 19-Sep-01 14:44 flow/templates/eos.sh
--rw-r--r--  2.0 unx      389 b- defN 19-Sep-01 14:44 flow/templates/lsf.sh
--rw-r--r--  2.0 unx      412 b- defN 19-Sep-01 14:44 flow/templates/project_example.pyt
--rw-r--r--  2.0 unx      152 b- defN 19-Sep-01 14:44 flow/templates/project_minimal.pyt
--rw-r--r--  2.0 unx     1235 b- defN 19-Sep-01 14:44 flow/templates/project_testing.pyt
--rw-r--r--  2.0 unx       26 b- defN 19-Sep-01 14:44 flow/templates/script.sh
--rw-r--r--  2.0 unx      218 b- defN 19-Sep-01 14:44 flow/templates/simple_scheduler.sh
--rw-r--r--  2.0 unx      447 b- defN 19-Sep-01 14:44 flow/templates/slurm.sh
--rw-r--r--  2.0 unx     2737 b- defN 19-Sep-01 14:44 flow/templates/stampede2.sh
--rw-r--r--  2.0 unx       34 b- defN 19-Sep-01 14:44 flow/templates/status.jinja
--rw-r--r--  2.0 unx       42 b- defN 19-Sep-01 14:44 flow/templates/status_compact.jinja
--rw-r--r--  2.0 unx       41 b- defN 19-Sep-01 14:44 flow/templates/status_expand.jinja
--rw-r--r--  2.0 unx       40 b- defN 19-Sep-01 14:44 flow/templates/status_stack.jinja
--rw-r--r--  2.0 unx     1224 b- defN 19-Sep-01 14:44 flow/templates/summit.sh
--rw-r--r--  2.0 unx      770 b- defN 19-Sep-01 14:44 flow/templates/titan.sh
--rw-r--r--  2.0 unx      801 b- defN 19-Sep-01 14:44 flow/templates/torque.sh
--rw-r--r--  2.0 unx     1226 b- defN 19-Sep-01 14:44 flow/templates/umich-flux.sh
--rw-r--r--  2.0 unx      305 b- defN 19-Sep-01 14:44 flow/util/__init__.py
--rw-r--r--  2.0 unx     2249 b- defN 19-Sep-01 14:44 flow/util/config.py
--rw-r--r--  2.0 unx      792 b- defN 19-Sep-01 14:44 flow/util/execution.py
--rw-r--r--  2.0 unx     6936 b- defN 19-Sep-01 14:44 flow/util/misc.py
--rw-r--r--  2.0 unx     1088 b- defN 19-Sep-01 14:44 flow/util/progressbar.py
--rw-r--r--  2.0 unx     8110 b- defN 19-Sep-01 14:44 flow/util/template_filters.py
--rw-r--r--  2.0 unx      630 b- defN 19-Sep-01 14:44 flow/util/translate.py
--rw-r--r--  2.0 unx     1000 b- defN 19-Sep-01 14:44 flow/util/tqdm/__init__.py
--rw-r--r--  2.0 unx       31 b- defN 19-Sep-01 14:44 flow/util/tqdm/__main__.py
--rw-r--r--  2.0 unx     4933 b- defN 19-Sep-01 14:44 flow/util/tqdm/_main.py
--rw-r--r--  2.0 unx    41319 b- defN 19-Sep-01 14:44 flow/util/tqdm/_tqdm.py
--rw-r--r--  2.0 unx    13461 b- defN 19-Sep-01 14:44 flow/util/tqdm/_tqdm_gui.py
--rw-r--r--  2.0 unx     8282 b- defN 19-Sep-01 14:44 flow/util/tqdm/_tqdm_notebook.py
--rw-r--r--  2.0 unx     1608 b- defN 19-Sep-01 14:44 flow/util/tqdm/_tqdm_pandas.py
--rw-r--r--  2.0 unx     3436 b- defN 19-Sep-01 14:44 flow/util/tqdm/_utils.py
--rw-r--r--  2.0 unx      925 b- defN 19-Sep-01 14:44 flow/util/tqdm/_version.py
--rwxr-xr-x  2.0 unx     7523 b- defN 19-Sep-01 14:44 signac_flow-0.8.0.data/scripts/simple-scheduler
--rw-r--r--  2.0 unx     1587 b- defN 19-Sep-01 14:44 signac_flow-0.8.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4158 b- defN 19-Sep-01 14:44 signac_flow-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 19-Sep-01 14:44 signac_flow-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 19-Sep-01 14:44 signac_flow-0.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 19-Sep-01 14:44 signac_flow-0.8.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 19-Sep-01 14:44 signac_flow-0.8.0.dist-info/zip-safe
-?rw-rw-r--  2.0 unx     5870 b- defN 19-Sep-01 14:44 signac_flow-0.8.0.dist-info/RECORD
-71 files, 331500 bytes uncompressed, 100751 bytes compressed:  69.6%
+Zip file size: 105167 bytes, number of entries: 67
+-rw-rw----  2.0 unx     1408 b- defN 20-Jan-19 18:22 flow/__init__.py
+-rw-rw----  2.0 unx     3558 b- defN 20-Jan-19 18:22 flow/__main__.py
+-rw-rw----  2.0 unx    13479 b- defN 20-Jan-26 19:30 flow/environment.py
+-rw-rw----  2.0 unx     1314 b- defN 20-Jan-19 18:22 flow/errors.py
+-rw-rw----  2.0 unx     1411 b- defN 20-Jan-19 18:22 flow/labels.py
+-rw-rw----  2.0 unx     7869 b- defN 20-Jan-26 19:30 flow/operations.py
+-rw-rw----  2.0 unx   125434 b- defN 20-Jan-26 19:30 flow/project.py
+-rw-rw----  2.0 unx     2809 b- defN 20-Jan-19 18:22 flow/template.py
+-rw-rw----  2.0 unx      648 b- defN 20-Jan-19 18:22 flow/testing.py
+-rw-rw----  2.0 unx      196 b- defN 20-Jan-19 18:22 flow/version.py
+-rw-rw----  2.0 unx      617 b- defN 20-Jan-09 16:13 flow/environments/__init__.py
+-rw-rw----  2.0 unx     3195 b- defN 20-Jan-26 19:30 flow/environments/incite.py
+-rw-rw----  2.0 unx     1077 b- defN 20-Jan-26 19:30 flow/environments/umich.py
+-rw-rw----  2.0 unx     2842 b- defN 20-Jan-26 19:30 flow/environments/xsede.py
+-rw-rw----  2.0 unx      442 b- defN 20-Jan-09 16:13 flow/scheduling/__init__.py
+-rw-rw----  2.0 unx     1994 b- defN 19-Aug-17 03:30 flow/scheduling/base.py
+-rw-rw----  2.0 unx      959 b- defN 20-Jan-09 16:13 flow/scheduling/fakescheduler.py
+-rw-rw----  2.0 unx     4624 b- defN 20-Jan-09 16:13 flow/scheduling/lsf.py
+-rw-rw----  2.0 unx     1258 b- defN 19-Feb-13 17:56 flow/scheduling/simple_scheduler.py
+-rw-rw----  2.0 unx     4768 b- defN 20-Jan-09 16:13 flow/scheduling/slurm.py
+-rw-rw----  2.0 unx     1514 b- defN 19-Feb-13 17:56 flow/scheduling/status.py
+-rw-rw----  2.0 unx     5484 b- defN 20-Jan-09 16:13 flow/scheduling/torque.py
+-rw-rw----  2.0 unx      979 b- defN 20-Jan-26 19:30 flow/templates/base_script.sh
+-rw-rw----  2.0 unx     2926 b- defN 19-Oct-06 04:03 flow/templates/base_status.jinja
+-rw-rw----  2.0 unx     1857 b- defN 19-Jul-22 02:34 flow/templates/base_status_compact.jinja
+-rw-rw----  2.0 unx     1116 b- defN 19-Jul-22 02:34 flow/templates/base_status_expand.jinja
+-rw-rw----  2.0 unx      814 b- defN 19-Jul-22 02:34 flow/templates/base_status_stack.jinja
+-rw-rw----  2.0 unx     1902 b- defN 20-Jan-26 19:30 flow/templates/bridges.sh
+-rw-rw----  2.0 unx     1671 b- defN 20-Jan-26 19:30 flow/templates/comet.sh
+-rw-rw----  2.0 unx      389 b- defN 19-Feb-13 17:56 flow/templates/lsf.sh
+-rw-rw----  2.0 unx      412 b- defN 19-Feb-13 17:56 flow/templates/project_example.pyt
+-rw-rw----  2.0 unx      152 b- defN 19-Feb-13 17:56 flow/templates/project_minimal.pyt
+-rw-rw----  2.0 unx     1235 b- defN 19-Aug-17 03:30 flow/templates/project_testing.pyt
+-rw-rw----  2.0 unx       26 b- defN 19-Feb-13 17:56 flow/templates/script.sh
+-rw-rw----  2.0 unx      218 b- defN 19-Feb-13 17:56 flow/templates/simple_scheduler.sh
+-rw-rw----  2.0 unx      447 b- defN 19-Feb-13 17:56 flow/templates/slurm.sh
+-rw-rw----  2.0 unx     2737 b- defN 20-Jan-26 19:30 flow/templates/stampede2.sh
+-rw-rw----  2.0 unx       34 b- defN 19-Jul-22 02:34 flow/templates/status.jinja
+-rw-rw----  2.0 unx       42 b- defN 19-Jul-22 02:34 flow/templates/status_compact.jinja
+-rw-rw----  2.0 unx       41 b- defN 19-Jul-22 02:34 flow/templates/status_expand.jinja
+-rw-rw----  2.0 unx       40 b- defN 19-Jul-22 02:34 flow/templates/status_stack.jinja
+-rw-rw----  2.0 unx     1224 b- defN 20-Jan-26 19:30 flow/templates/summit.sh
+-rw-rw----  2.0 unx      801 b- defN 19-Jul-22 02:34 flow/templates/torque.sh
+-rw-rw----  2.0 unx     1226 b- defN 20-Jan-26 19:30 flow/templates/umich-flux.sh
+-rw-rw----  2.0 unx      305 b- defN 19-Oct-06 04:03 flow/util/__init__.py
+-rw-rw----  2.0 unx     2112 b- defN 20-Jan-09 16:13 flow/util/config.py
+-rw-rw----  2.0 unx     5868 b- defN 20-Jan-19 18:22 flow/util/misc.py
+-rw-rw----  2.0 unx     1152 b- defN 20-Jan-19 18:22 flow/util/progressbar.py
+-rw-rw----  2.0 unx     8041 b- defN 20-Jan-19 18:22 flow/util/template_filters.py
+-rw-rw----  2.0 unx      638 b- defN 20-Jan-19 18:22 flow/util/translate.py
+-rw-rw----  2.0 unx     1000 b- defN 19-Feb-13 17:56 flow/util/tqdm/__init__.py
+-rw-rw----  2.0 unx       31 b- defN 19-Feb-13 17:56 flow/util/tqdm/__main__.py
+-rw-rw----  2.0 unx     4933 b- defN 19-Feb-13 17:56 flow/util/tqdm/_main.py
+-rw-rw----  2.0 unx    41319 b- defN 19-Feb-13 17:56 flow/util/tqdm/_tqdm.py
+-rw-rw----  2.0 unx    13461 b- defN 19-Feb-13 17:56 flow/util/tqdm/_tqdm_gui.py
+-rw-rw----  2.0 unx     8282 b- defN 19-Feb-13 17:56 flow/util/tqdm/_tqdm_notebook.py
+-rw-rw----  2.0 unx     1608 b- defN 19-Feb-13 17:56 flow/util/tqdm/_tqdm_pandas.py
+-rw-rw----  2.0 unx     3436 b- defN 19-Feb-13 17:56 flow/util/tqdm/_utils.py
+-rw-rw----  2.0 unx      925 b- defN 19-Feb-13 17:56 flow/util/tqdm/_version.py
+-rwxrwxr-x  2.0 unx     7514 b- defN 20-Jan-26 19:31 signac_flow-0.9.0.data/scripts/simple-scheduler
+-rw-rw----  2.0 unx     1587 b- defN 20-Jan-26 19:31 signac_flow-0.9.0.dist-info/LICENSE.txt
+-rw-rw----  2.0 unx     4218 b- defN 20-Jan-26 19:31 signac_flow-0.9.0.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 20-Jan-26 19:31 signac_flow-0.9.0.dist-info/WHEEL
+-rw-rw----  2.0 unx       45 b- defN 20-Jan-26 19:31 signac_flow-0.9.0.dist-info/entry_points.txt
+-rw-rw----  2.0 unx        5 b- defN 20-Jan-26 19:31 signac_flow-0.9.0.dist-info/top_level.txt
+-rw-rw----  2.0 unx        1 b- defN 19-Apr-14 13:19 signac_flow-0.9.0.dist-info/zip-safe
+?rw-rw-r--  2.0 unx     5552 b- defN 20-Jan-26 19:31 signac_flow-0.9.0.dist-info/RECORD
+67 files, 319314 bytes uncompressed, 96413 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -9,32 +9,29 @@
 
 Filename: flow/errors.py
 Comment: 
 
 Filename: flow/labels.py
 Comment: 
 
-Filename: flow/legacy.py
-Comment: 
-
-Filename: flow/legacy_templating.py
-Comment: 
-
 Filename: flow/operations.py
 Comment: 
 
 Filename: flow/project.py
 Comment: 
 
 Filename: flow/template.py
 Comment: 
 
 Filename: flow/testing.py
 Comment: 
 
+Filename: flow/version.py
+Comment: 
+
 Filename: flow/environments/__init__.py
 Comment: 
 
 Filename: flow/environments/incite.py
 Comment: 
 
 Filename: flow/environments/umich.py
@@ -84,17 +81,14 @@
 
 Filename: flow/templates/bridges.sh
 Comment: 
 
 Filename: flow/templates/comet.sh
 Comment: 
 
-Filename: flow/templates/eos.sh
-Comment: 
-
 Filename: flow/templates/lsf.sh
 Comment: 
 
 Filename: flow/templates/project_example.pyt
 Comment: 
 
 Filename: flow/templates/project_minimal.pyt
@@ -126,32 +120,26 @@
 
 Filename: flow/templates/status_stack.jinja
 Comment: 
 
 Filename: flow/templates/summit.sh
 Comment: 
 
-Filename: flow/templates/titan.sh
-Comment: 
-
 Filename: flow/templates/torque.sh
 Comment: 
 
 Filename: flow/templates/umich-flux.sh
 Comment: 
 
 Filename: flow/util/__init__.py
 Comment: 
 
 Filename: flow/util/config.py
 Comment: 
 
-Filename: flow/util/execution.py
-Comment: 
-
 Filename: flow/util/misc.py
 Comment: 
 
 Filename: flow/util/progressbar.py
 Comment: 
 
 Filename: flow/util/template_filters.py
@@ -183,32 +171,32 @@
 
 Filename: flow/util/tqdm/_utils.py
 Comment: 
 
 Filename: flow/util/tqdm/_version.py
 Comment: 
 
-Filename: signac_flow-0.8.0.data/scripts/simple-scheduler
+Filename: signac_flow-0.9.0.data/scripts/simple-scheduler
 Comment: 
 
-Filename: signac_flow-0.8.0.dist-info/LICENSE.txt
+Filename: signac_flow-0.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: signac_flow-0.8.0.dist-info/METADATA
+Filename: signac_flow-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: signac_flow-0.8.0.dist-info/WHEEL
+Filename: signac_flow-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: signac_flow-0.8.0.dist-info/entry_points.txt
+Filename: signac_flow-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: signac_flow-0.8.0.dist-info/top_level.txt
+Filename: signac_flow-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: signac_flow-0.8.0.dist-info/zip-safe
+Filename: signac_flow-0.9.0.dist-info/zip-safe
 Comment: 
 
-Filename: signac_flow-0.8.0.dist-info/RECORD
+Filename: signac_flow-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flow/__init__.py

```diff
@@ -2,17 +2,16 @@
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """Workflow management based on the signac framework.
 
 The signac-flow package provides the basic infrastructure to easily
 configure and implement a workflow to operate on a signac_ data space.
 
-.. _signac: https://glotzerlab.engin.umich.edu/signac
+.. _signac: https://signac.io/
 """
-from __future__ import absolute_import
 from . import environment
 from . import scheduling
 from . import errors
 from . import testing
 from .project import FlowProject
 from .project import JobOperation
 from .project import label
@@ -21,34 +20,34 @@
 from .operations import cmd
 from .operations import directives
 from .operations import run
 from .environment import get_environment
 from .template import init
 from .util.misc import redirect_log
 from .operations import with_job
+from .version import __version__
 
 # Import packaged environments unless disabled in config:
 from .util.config import get_config_value
 if get_config_value('import_packaged_environments', default=True):
-    from . import environments  # noqa:F401
+    from . import environments  # noqa: F401
 
 
-__version__ = '0.8.0'
-
 __all__ = [
     'environment',
     'scheduling',
     'errors',
+    'testing',
     'FlowProject',
     'JobOperation',
     'label',
     'classlabel',
     'staticlabel',
     'cmd',
     'directives',
     'run',
+    'get_environment',
     'init',
     'redirect_log',
-    'get_environment',
     'with_job',
-    'testing'
+    '__version__',
     ]
```

## flow/__main__.py

```diff
@@ -4,48 +4,45 @@
 """This module defines the main command line interface for signac-flow.
 
 The interface is accessible via the `flow` command and allows users to
 initialize FlowProject class definitions directly from the command line.
 
 Execute `flow --help` for more information.
 """
-from __future__ import print_function
 import argparse
 import logging
 import sys
 
-from signac.common import six
 from signac import init_project
 from signac import get_project
 
 from . import __version__
 from . import template
-from .util.misc import _is_identifier
 
 
 logger = logging.getLogger(__name__)
 
 
 def main_init(args):
     "Initialize a FlowProject from one of the templates defined in the template module."
-    if not _is_identifier(args.alias):
+    if not args.alias.isidentifier():
         raise ValueError(
             "The alias '{}' is not a valid Python identifier and can therefore "
             "not be used as a FlowProject alias.".format(args.alias))
     try:
         get_project()
     except LookupError:
         init_project(name=args.alias)
         print("Initialized signac project with name '{}' in "
               "current directory.".format(args.alias), file=sys.stderr)
     try:
         return template.init(alias=args.alias, template=args.template)
     except OSError as e:
         raise RuntimeError(
-            "Error occured while trying to initialize a flow project: {}".format(e))
+            "Error occurred while trying to initialize a flow project: {}".format(e))
 
 
 def main():
     """Main entry function for the 'flow' command line tool.
 
     This function defines the main 'flow' command line interface which can be used
     to initialize FlowProject modules from different templates as well as print the
@@ -87,16 +84,14 @@
         print('signac-flow', __version__)
         sys.exit(0)
 
     args = parser.parse_args()
 
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
-    elif six.PY2:
-        logging.basicConfig(level=logging.WARNING)
     if not hasattr(args, 'func'):
         parser.print_usage()
         sys.exit(2)
     try:
         args.func(args)
     except KeyboardInterrupt:
         sys.stderr.write("\n")
```

## flow/environment.py

```diff
@@ -3,59 +3,50 @@
 # This software is licensed under the BSD 3-Clause License.
 """Detection of compute environments.
 
 This module provides the ComputeEnvironment class, which can be
 subclassed to automatically detect specific computational environments.
 
 This enables the user to adjust their workflow based on the present
-environment, e.g. for the adjustemt of scheduler submission scripts.
+environment, e.g. for the adjustment of scheduler submission scripts.
 """
-from __future__ import print_function
-from __future__ import division
 import os
 import re
 import socket
 import logging
 import importlib
 from collections import OrderedDict
+import importlib.machinery
 
 from signac.common import config
-from signac.common import six
-from signac.common.six import with_metaclass
 
 from .scheduling.base import JobStatus
 from .scheduling.lsf import LSFScheduler
 from .scheduling.slurm import SlurmScheduler
 from .scheduling.torque import TorqueScheduler
 from .scheduling.simple_scheduler import SimpleScheduler
 from .scheduling.fakescheduler import FakeScheduler
 from .util import config as flow_config
 from .errors import NoSchedulerError
 
-if six.PY2:
-    import imp
-else:
-    import importlib.machinery
 
 logger = logging.getLogger(__name__)
-if six.PY2:
-    logger.addHandler(logging.NullHandler())
 
 
 # Global variable can be used to override detected environment
 ENVIRONMENT = None
 
 
 def setup(py_modules, **attrs):
     """Setup function for environment modules.
 
     Use this function in place of setuptools.setup to not only install
-    a environments module, but also register it with the global signac
-    configuration. Once registered, is automatically imported when the
-    get_environment() function is called.
+    an environment's module, but also register it with the global signac
+    configuration. Once registered, the environment is automatically
+    imported when the :py:meth:`~.get_environment` function is called.
     """
     import setuptools
     from setuptools.command.install import install
 
     class InstallAndConfig(install):
 
         def run(self):
@@ -78,39 +69,39 @@
     return setuptools.setup(
         py_modules=py_modules,
         cmdclass={'install': InstallAndConfig},
         **attrs)
 
 
 class ComputeEnvironmentType(type):
-    """Meta class for the definition of ComputeEnvironments.
+    """Metaclass for the definition of ComputeEnvironments.
 
-    This meta class automatically registers ComputeEnvironment definitions,
+    This metaclass automatically registers ComputeEnvironment definitions,
     which enables the automatic determination of the present environment.
     """
 
     def __init__(cls, name, bases, dct):
         if not hasattr(cls, 'registry'):
             cls.registry = OrderedDict()
         else:
             cls.registry[name] = cls
         return super(ComputeEnvironmentType, cls).__init__(name, bases, dct)
 
 
-class ComputeEnvironment(with_metaclass(ComputeEnvironmentType)):
+class ComputeEnvironment(metaclass=ComputeEnvironmentType):
     """Define computational environments.
 
     The ComputeEnvironment class allows us to automatically determine
-    specific environments in order to programatically adjust workflows
+    specific environments in order to programmatically adjust workflows
     in different environments.
 
-    The default method for the detection of a specific environemnt is to
+    The default method for the detection of a specific environment is to
     provide a regular expression matching the environment's hostname.
-    For example, if the hostname is my_server.com, one could identify the
-    environment by setting the hostname_pattern to 'my_server'.
+    For example, if the hostname is my-server.com, one could identify the
+    environment by setting the hostname_pattern to 'my-server'.
     """
     scheduler_type = None
     hostname_pattern = None
     submit_flags = None
     template = 'base_script.sh'
 
     @classmethod
@@ -128,15 +119,15 @@
                 return cls.scheduler_type.is_present()
         else:
             return re.match(
                 cls.hostname_pattern, socket.getfqdn()) is not None
 
     @classmethod
     def get_scheduler(cls):
-        """Return a environment specific scheduler driver.
+        """Return an environment-specific scheduler driver.
 
         The returned scheduler class provides a standardized interface to
         different scheduler implementations.
         """
         try:
             return getattr(cls, 'scheduler_type')()
         except (AttributeError, TypeError):
@@ -172,57 +163,43 @@
         return
 
     @classmethod
     def get_config_value(cls, key, default=flow_config._GET_CONFIG_VALUE_NONE):
         """Request a value from the user's configuration.
 
         This method should be used whenever values need to be provided
-        that are specific to a users's environment. A good example are
-        account names.
+        that are specific to a user's environment, e.g. account names.
 
         When a key is not configured and no default value is provided,
         a :py:class:`~.errors.SubmitError` will be raised and the user will
         be prompted to add the missing key to their configuration.
 
         Please note, that the key will be automatically expanded to
         be specific to this environment definition. For example, a
-        key should be 'account', not 'MyEnvironment.account`.
+        key should be ``'account'``, not ``'MyEnvironment.account'``.
 
         :param key: The environment specific configuration key.
         :type key: str
         :param default: A default value in case the key cannot be found
             within the user's configuration.
-        :type key: str
+        :type default: str
         :return: The value or default value.
         :raises SubmitError: If the key is not in the user's configuration
             and no default value is provided.
         """
         return flow_config.require_config_value(key, ns=cls.__name__, default=default)
 
 
 class StandardEnvironment(ComputeEnvironment):
     "This is a default environment, which is always present."
 
     @classmethod
     def is_present(cls):
         return True
 
-    @classmethod
-    def mpi_cmd(cls, cmd, np):
-        return 'mpirun -np {np} {cmd}'.format(np=np, cmd=cmd)
-
-
-class UnknownEnvironment(StandardEnvironment):
-    "Deprecated 'standard' environment, replaced by 'StandardEnvironment.'"
-
-    def __init__(self, *args, **kwargs):
-        raise RuntimeError(
-            "The 'flow.environment.UnknownEnvironment' class has been replaced by the "
-            "'flow.environment.StandardEnvironment' class.")
-
 
 class TestEnvironment(ComputeEnvironment):
     """This is a test environment.
 
     The test environment will print a mocked submission script
     and submission commands to screen. This enables testing of
     the job submission script generation in environments without
@@ -338,18 +315,15 @@
 
 class GPUEnvironment(ComputeEnvironment):
     "An environment with GPUs."
     pass
 
 
 def _import_module(fn):
-    if six.PY2:
-        return imp.load_source(os.path.splitext(fn)[0], fn)
-    else:
-        return importlib.machinery.SourceFileLoader(fn, fn).load_module()
+    return importlib.machinery.SourceFileLoader(fn, fn).load_module()
 
 
 def _import_modules(prefix):
     for fn in os.path.listdir(prefix):
         if os.path.isfile(fn) and os.path.splitext(fn)[1] == '.py':
             _import_module(os.path.join(prefix, fn))
 
@@ -371,21 +345,21 @@
         _import_configured_environments()
     return list(ComputeEnvironment.registry.values())
 
 
 def get_environment(test=False, import_configured=True):
     """Attempt to detect the present environment.
 
-    This function iterates through all defined ComputeEnvironment
-    classes in reversed order of definition and and returns the
-    first EnvironmentClass where the is_present() method returns
-    True.
+    This function iterates through all defined :py:class:`~.ComputeEnvironment`
+    classes in reversed order of definition and returns the first
+    environment where the :py:meth:`~.ComputeEnvironment.is_present` method
+    returns True.
 
     :param test:
-        Return the TestEnvironment
+        Whether to return the TestEnvironment.
     :type test:
         bool
     :returns:
         The detected environment class.
     """
     if test:
         return TestEnvironment
```

## flow/errors.py

```diff
@@ -1,19 +1,14 @@
 # Copyright (c) 2018 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """Definitions of Exception classes used in this package."""
 
-try:
-    import jinja2
-    from jinja2.ext import Extension as Jinja2Extension
-except ImportError:
-    JINJA2 = False
-else:
-    JINJA2 = True
+import jinja2
+from jinja2.ext import Extension as Jinja2Extension
 
 
 class ConfigKeyError(KeyError):
     "Indicates that a config key was not found."
     pass
 
 
@@ -23,26 +18,30 @@
 
 
 class NoSchedulerError(AttributeError):
     "Indicates that there is no scheduler type defined for an environment class."
     pass
 
 
-if JINJA2:
+class UserConditionError(RuntimeError):
+    "Indicates an error during evaluation of a FlowCondition."
+    pass
+
+
+class UserOperationError(RuntimeError):
+    "Indicates an error during execution of a FlowOperation."
+    pass
+
+
+class TemplateError(Jinja2Extension):
+    """Indicates errors in jinja2 templates"""
+    # ref:http://jinja.pocoo.org/docs/2.10/extensions/#jinja-extensions
+    tags = set(['raise'])
+
+    def parse(self, parser):
+        lineno = next(parser.stream).lineno
+        args = [parser.parse_expression()]
+        return jinja2.nodes.CallBlock(
+            self.call_method('err', args), [], [], []).set_lineno(lineno)
 
-    class TemplateError(Jinja2Extension):
-        """Indicates errors in jinja2 templates"""
-        # ref:http://jinja.pocoo.org/docs/2.10/extensions/#jinja-extensions
-        tags = set(['raise'])
-
-        def parse(self, parser):
-            lineno = next(parser.stream).lineno
-            args = [parser.parse_expression()]
-            return jinja2.nodes.CallBlock(
-                self.call_method('err', args), [], [], []).set_lineno(lineno)
-
-        def err(self, msg, caller):
-            raise jinja2.TemplateError(msg)
-
-else:
-    class TemplateError(Exception):     # mock class, should never be used
-        pass
+    def err(self, msg, caller):
+        raise jinja2.TemplateError(msg)
```

## flow/labels.py

 * *Ordering differences only*

```diff
@@ -7,19 +7,19 @@
 functions which can be used to decorate label functions which are part
 of a FlowProject class definition.
 """
 
 
 class label(object):
     """Decorate a :class:`~.FlowProject` class function as a label function.
+
     For example:
 
     .. code-block:: python
 
-
         class MyProject(FlowProject):
 
             @label()
             def foo(self, job):
                 return True
     """
```

## flow/operations.py

```diff
@@ -2,27 +2,25 @@
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """This module implements the run() function, which when called equips
 a regular Python module with a command line interface, which can be used
 to execute functions defined within the same module, that operate on a
 signac data space.
 """
-from __future__ import print_function
 import sys
 import argparse
 import logging
 import inspect
+import subprocess
 from multiprocessing import Pool
 from functools import wraps
 
 from signac import get_project
-from signac.common import six
 
 from .util.tqdm import tqdm
-from .util.execution import fork
 
 
 logger = logging.getLogger(__name__)
 
 
 def cmd(func):
     """Specifies that ``func`` returns a shell command.
@@ -101,14 +99,22 @@
 
 
 class directives(object):
     """Decorator for operation functions to provide additional execution directives.
 
     Directives can for example be used to provide information about required resources
     such as the number of processes required for execution of parallelized operations.
+
+    In addition, you can use the `@directives(fork=True)` directive to enforce that a
+    particular operation is always executed within a subprocess and not within the
+    Python interpreter's process even if there are no other reasons that would prevent that.
+    .. note::
+
+        Setting `fork=False` will not prevent forking if there are other reasons for forking,
+        such as a timeout.
     """
 
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     @classmethod
     def copy_from(cls, func):
@@ -130,28 +136,25 @@
     are ignored.
     """
     module = inspect.getmodule(inspect.currentframe().f_back.f_back)
     for name, obj in inspect.getmembers(module):
         if not include_private and name.startswith('_'):
             continue
         if inspect.isfunction(obj):
-            if six.PY2:
-                signature = inspect.getargspec(obj)
-            else:
-                signature = inspect.getfullargspec(obj)
+            signature = inspect.getfullargspec(obj)
             if len(signature.args) == 1:
                 yield name
 
 
 def run(parser=None):
     """Access to the "run" interface of an operations module.
 
     Executing this function within a module will start a command line interface,
     that can be used to execute operations defined within the same module.
-    All **top-level unary functions** will be intepreted as executable operation functions.
+    All **top-level unary functions** will be interpreted as executable operation functions.
 
     For example, if we have a module as such:
 
     .. code-block:: python
 
         # operations.py
 
@@ -236,35 +239,24 @@
     except AttributeError:
         raise KeyError("Unknown operation '{}'.".format(args.operation))
 
     if getattr(operation_func, '_flow_cmd', False):
 
         def operation(job):
             cmd = operation_func(job).format(job=job)
-            fork(cmd=cmd, timeout=args.timeout)
+            subprocess.run(cmd, shell=True, timeout=args.timeout, check=True)
     else:
         operation = operation_func
 
     # Serial execution
     if args.np == 1 or len(jobs) < 2:
         if args.timeout is not None:
             logger.warning("A timeout has no effect in serial execution!")
         for job in tqdm(jobs) if args.progress else jobs:
             operation(job)
-
-    # Parallel execution
-    elif six.PY2:
-        # Due to Python 2.7 issue #8296 (http://bugs.python.org/issue8296) we
-        # always need to provide a timeout to avoid issues with "hanging"
-        # processing pools.
-        timeout = sys.maxint if args.timeout is None else args.timeout
-        pool = Pool(args.np)
-        result = pool.imap_unordered(operation, jobs)
-        for _ in tqdm(jobs) if args.progress else jobs:
-            result.next(timeout)
     else:
         with Pool(args.np) as pool:
             result = pool.imap_unordered(operation, jobs)
             for _ in tqdm(jobs) if args.progress else jobs:
                 result.next(args.timeout)
```

## flow/project.py

```diff
@@ -1,27 +1,28 @@
 # Copyright (c) 2019 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """Workflow definition with the FlowProject.
 
 The FlowProject is a signac Project that allows the user to define a workflow.
 """
-from __future__ import print_function
 import sys
 import os
 import re
 import logging
 import argparse
 import time
 import datetime
 import json
 import inspect
 import functools
 import contextlib
 import random
+import subprocess
+import traceback
 from deprecation import deprecated
 from collections import defaultdict
 from collections import OrderedDict
 from collections import Counter
 from itertools import islice
 from itertools import count
 from itertools import groupby
@@ -29,146 +30,168 @@
 import multiprocessing
 import threading
 from multiprocessing import Pool
 from multiprocessing import cpu_count
 from multiprocessing import TimeoutError
 from multiprocessing.pool import ThreadPool
 from multiprocessing import Event
+import jinja2
+from jinja2 import TemplateNotFound as Jinja2TemplateNotFound
 
 import signac
-from signac.common import six
 from signac.contrib.hashing import calc_id
 from signac.contrib.filterparse import parse_filter_arg
-
-import jinja2
-from jinja2 import TemplateNotFound as Jinja2TemplateNotFound
+from signac.contrib.project import JobsCursor
 
 from .environment import get_environment
 from .scheduling.base import ClusterJob
 from .scheduling.base import JobStatus
 from .scheduling.status import update_status
 from .errors import SubmitError
 from .errors import ConfigKeyError
 from .errors import NoSchedulerError
+from .errors import UserConditionError
+from .errors import UserOperationError
 from .errors import TemplateError
 from .util.tqdm import tqdm
 from .util.misc import _positive_int
-from .util.misc import _mkdir_p
 from .util.misc import roundrobin
 from .util.misc import to_hashable
 from .util import template_filters as tf
 from .util.misc import add_cwd_to_environment_pythonpath
 from .util.misc import switch_to_directory
 from .util.misc import TrackGetItemDict
-from .util.misc import fullmatch
 from .util.translate import abbreviate
 from .util.translate import shorten
-from .util.execution import fork
-from .util.execution import TimeoutExpired
 from .labels import label
 from .labels import staticlabel
 from .labels import classlabel
 from .labels import _is_label_func
-from . import legacy
 from .util import config as flow_config
+from .version import __version__
 
 
 logger = logging.getLogger(__name__)
-if six.PY2:
-    logger.addHandler(logging.NullHandler())
 
 
 # The TEMPLATE_HELP can be shown with the --template-help option available to all
 # command line sub commands that use the templating system.
 TEMPLATE_HELP = """Execution and submission scripts are generated with the jinja2 template files.
 Standard files are shipped with the package, but maybe replaced or extended with
 custom templates provided within a project.
 The default template directory can be configured with the 'template_dir' configuration
 variable, for example in the project configuration file. The current template directory is:
 {template_dir}
 
 All template variables can be placed within a template using the standard jinja2
-syntax, e.g., the project root directory can be written like this: {{ project._rd }}.
+syntax, e.g., the project root directory can be written like this: {{{{ project._rd }}}}.
 The available template variables are:
 {template_vars}
 
 Filter functions can be used to format template variables in a specific way.
-For example: {{ project.get_id() | captialize }}.
+For example: {{{{ project.get_id() | capitalize }}}}.
 
 The available filters are:
 {filters}"""
 
 
 class _condition(object):
+    # This counter should be incremented each time an "always" or "never"
+    # condition is created, and the value should be used as the tag for that
+    # condition to ensure that no pair of "always" and "never" conditions
+    # are found to be equal by the graph detection algorithm.
+    current_arbitrary_tag = 0
+
+    def __init__(self, condition, tag=None):
+        """Add tag to differentiate built-in conditions during graph detection."""
 
-    def __init__(self, condition):
+        if tag is None:
+            try:
+                tag = condition.__code__.co_code
+            except AttributeError:
+                logger.warning("Condition {} could not autogenerate tag.".format(condition))
+        condition._flow_tag = tag
         self.condition = condition
 
     @classmethod
     def isfile(cls, filename):
         "True if the specified file exists for this job."
-        return cls(lambda job: job.isfile(filename))
+        return cls(lambda job: job.isfile(filename), 'isfile_' + filename)
 
     @classmethod
     def true(cls, key):
         """True if the specified key is present in the job document and
         evaluates to True."""
-        return cls(lambda job: job.document.get(key, False))
+        return cls(lambda job: job.document.get(key, False), 'true_' + key)
 
     @classmethod
     def false(cls, key):
         """True if the specified key is present in the job document and
         evaluates to False."""
-        return cls(lambda job: not job.document.get(key, False))
+        return cls(lambda job: not job.document.get(key, False), 'false_' + key)
 
     @classmethod
+    @deprecated(
+        deprecated_in="0.9", removed_in="0.11", current_version=__version__,
+        details="This condition decorator is obsolete.")
     def always(cls, func):
         "Returns True."
-        return cls(lambda _: True)(func)
+        cls.current_arbitrary_tag += 1
+        return cls(lambda _: True, str(cls.current_arbitrary_tag))(func)
 
     @classmethod
     def never(cls, func):
         "Returns False."
-        return cls(lambda _: False)(func)
+        cls.current_arbitrary_tag += 1
+        return cls(lambda _: False, str(cls.current_arbitrary_tag))(func)
 
     @classmethod
     def not_(cls, condition):
         "Returns ``not condition(job)`` for the provided condition function."
-        return cls(lambda job: not condition(job))
+        return cls(lambda job: not condition(job),
+                   'not_'.encode() + condition.__code__.co_code)
 
 
-def make_bundles(operations, size=None):
+def _make_bundles(operations, size=None):
     """Utility function for the generation of bundles.
 
-    This function splits an iterable of operations into  equally
+    This function splits an iterable of operations into equally
     sized bundles and a possibly smaller final bundle.
     """
     n = None if size == 0 else size
     operations = iter(operations)
     while True:
         b = list(islice(operations, n))
         if b:
             yield b
         else:
             break
 
 
+@deprecated(deprecated_in="0.9", removed_in="0.11", current_version=__version__)
+def make_bundles(operations, size=None):
+    """Utility function for the generation of bundles.
+
+    This function splits an iterable of operations into equally
+    sized bundles and a possibly smaller final bundle.
+    """
+    return _make_bundles(operations, size)
+
+
 class JobOperation(object):
     """This class represents the information needed to execute one operation for one job.
 
     An operation function in this context is a shell command, which should be a function
     of one and only one signac job.
 
     .. note::
 
         This class is used by the :class:`~.FlowProject` class for the execution and
         submission process and should not be instantiated by users themselves.
 
-    .. versionchanged:: 0.6
-
     :param name:
         The name of this JobOperation instance. The name is arbitrary,
         but helps to concisely identify the operation in various contexts.
     :type name:
         str
     :param job:
         The job instance associated with this operation.
@@ -220,15 +243,15 @@
         directives.setdefault('omp_num_threads', 0)
         directives.setdefault('processor_fraction', 1)
 
         # Evaluate strings and callables for job:
         def evaluate(value):
             if value and callable(value):
                 return value(job)
-            elif isinstance(value, six.string_types):
+            elif isinstance(value, str):
                 return value.format(job=job)
             else:
                 return value
 
         # We use a special dictionary that allows us to track all keys that have been
         # evaluated by the template engine and compare them to those explicitly set
         # by the user. See also comment above.
@@ -255,18 +278,18 @@
         full_name = '{}%{}%{}%{}'.format(
             project.root_directory(), self.job.get_id(), self.name, index)
 
         # The job_op_id is a hash computed from the unique full name.
         job_op_id = calc_id(full_name)
 
         # The actual job id is then constructed from a readable part and the job_op_id,
-        # ensuring that the job-op is still somewhat identifiable, but guarantueed to
+        # ensuring that the job-op is still somewhat identifiable, but guaranteed to
         # be unique. The readable name is based on the project id, job id, operation name,
         # and the index number. All names and the id itself are restricted in length
-        # to guarantuee that the id does not get too long.
+        # to guarantee that the id does not get too long.
         max_len = self.MAX_LEN_ID - len(job_op_id)
         if max_len < len(job_op_id):
             raise ValueError("Value for MAX_LEN_ID is too small ({}).".format(self.MAX_LEN_ID))
 
         readable_name = '{}/{}/{}/{:04d}/'.format(
             str(project)[:12], str(self.job)[:8], self.name[:12], index)[:max_len]
 
@@ -296,53 +319,60 @@
     """A FlowCondition represents a condition as a function of a signac job.
 
     The __call__() function of a FlowCondition object may return either True
     or False, representing whether the condition is met or not.
     This can be used to build a graph of conditions and operations.
 
     :param callback:
-        A function with one positional argument (the job)
+        A callable with one positional argument (the job).
     :type callback:
-        :py:class:`~signac.contrib.job.Job`
+        callable
     """
 
     def __init__(self, callback):
         self._callback = callback
 
     def __call__(self, job):
         if self._callback is None:
             return True
-        return self._callback(job)
+        try:
+            return self._callback(job)
+        except Exception as e:
+            raise UserConditionError(
+                'An exception was raised while evaluating the condition {name} '
+                'for job {job}.'.format(name=self._callback.__name__, job=job)) from e
 
     def __hash__(self):
         return hash(self._callback)
 
     def __eq__(self, other):
         return self._callback == other._callback
 
 
 class FlowOperation(object):
     """A FlowOperation represents a data space operation, operating on any job.
 
-    Any FlowOperation is associated with a specific command, which should be
-    a function of :py:class:`~signac.contrib.job.Job`. The command (cmd) can
-    be stated as function, either by using str-substitution based on a job's
-    attributes, or by providing a unary callable, which expects an instance
-    of job as its first and only positional argument.
+    Every FlowOperation is associated with a specific command which should be
+    a function of :py:class:`~signac.contrib.job.Job`. The command (cmd) may
+    either be a unary callable that expects an instance of
+    :class:`~signac.contrib.job.Job` as its only positional argument and returns
+    a string containing valid shell commands, or the string of commands itself.
+    In either case, the resulting string may contain any attributes of the job placed
+    in curly braces, which will then be substituted by Python string formatting.
 
     For example, if we wanted to define a command for a program called 'hello',
-    which expects a job id as its first argument, we could contruct the following
+    which expects a job id as its first argument, we could construct the following
     two equivalent operations:
 
     .. code-block:: python
 
         op = FlowOperation('hello', cmd='hello {job._id}')
-        op = FlowOperation('hello', cmd=lambda 'hello {}'.format(job._id))
+         op = FlowOperation('hello', cmd=lambda job: 'hello {}'.format(job._id))
 
-    Here is another example for possible str-substitutions:
+    Here is another example of a possible string substitution:
 
     .. code-block:: python
 
         # Substitute job state point parameters:
         op = FlowOperation('hello', cmd='cd {job.ws}; hello {job.sp.a}')
 
     Pre-requirements (pre) and post-conditions (post) can be used to
@@ -407,14 +437,27 @@
     def __call__(self, job=None):
         if callable(self._cmd):
             return self._cmd(job).format(job=job)
         else:
             return self._cmd.format(job=job)
 
 
+def _create_all_metacondition(condition_dict, *other_funcs):
+    """Standard function for generating aggregate metaconditions that require
+    *all* provided conditions to be met. The resulting metacondition is
+    constructed with appropriate information for graph detection."""
+    condition_list = [c for f in other_funcs for c in condition_dict[f]]
+
+    def _flow_metacondition(job):
+        return all(c(job) for c in condition_list)
+
+    _flow_metacondition._composed_of = condition_list
+    return _flow_metacondition
+
+
 class _FlowProjectClass(type):
     """Metaclass for the FlowProject class."""
     def __new__(metacls, name, bases, namespace, **kwargs):
         cls = type.__new__(metacls, name, bases, dict(namespace))
 
         # All operation functions are registered with the operation() classmethod, which is
         # intended to be used as decorator function. The _OPERATION_FUNCTIONS dict maps the
@@ -424,15 +467,15 @@
         cls._OPERATION_FUNCTIONS = list()
         cls._OPERATION_PRE_CONDITIONS = defaultdict(list)
         cls._OPERATION_POST_CONDITIONS = defaultdict(list)
 
         cls._OPERATION_FUNCTIONS = list()
         cls._OPERATION_PRECONDITIONS = dict()
         cls._OPERATION_POSTCONDITIONS = dict()
-        # All label functions are registered with the label() classmethod, which is intendeded
+        # All label functions are registered with the label() classmethod, which is intended
         # to be used as decorator function. The _LABEL_FUNCTIONS dict contains the function as
         # key and the label name as value, or None to use the default label name.
         cls._LABEL_FUNCTIONS = OrderedDict()
 
         # Give the class a pre and post class that are aware of the class they
         # are in.
         cls.pre = cls._setup_pre_conditions_class(parent_class=cls)
@@ -452,42 +495,42 @@
                 @Project.pre(lambda job: not job.doc.get('hello'))
                 def hello(job):
                     print('hello', job)
                     job.doc.hello = True
 
             The *hello*-operation would only execute if the 'hello' key in the job
             document does not evaluate to True.
+
+            An optional tag may be associated with the condition. These tags
+            are used by :meth:`~.detect_operation_graph` when comparing
+            conditions for equality. The tag defaults to the bytecode of the
+            function.
             """
 
             _parent_class = parent_class
 
-            def __init__(self, condition):
-                self.condition = condition
+            def __init__(self, condition, tag=None):
+                super(pre, self).__init__(condition, tag)
 
             def __call__(self, func):
                 self._parent_class._OPERATION_PRE_CONDITIONS[func].insert(0, self.condition)
                 return func
 
             @classmethod
             def copy_from(cls, *other_funcs):
                 "True if and only if all pre conditions of other operation-function(s) are met."
-                def metacondition(job):
-                    return all(c(job)
-                               for other_func in other_funcs
-                               for c in cls._parent_class._collect_pre_conditions()[other_func])
-                return cls(metacondition)
+                return cls(_create_all_metacondition(cls._parent_class._collect_pre_conditions(),
+                                                     *other_funcs))
 
             @classmethod
             def after(cls, *other_funcs):
                 "True if and only if all post conditions of other operation-function(s) are met."
-                def metacondition(job):
-                    return all(c(job)
-                               for other_func in other_funcs
-                               for c in cls._parent_class._collect_post_conditions()[other_func])
-                return cls(metacondition)
+                return cls(_create_all_metacondition(cls._parent_class._collect_post_conditions(),
+                                                     *other_funcs))
+
         return pre
 
     @staticmethod
     def _setup_post_conditions_class(parent_class):
 
         class post(_condition):
             """Specify a function of job that must evaluate to True for this operation
@@ -499,37 +542,39 @@
                 @Project.post(lambda job: job.doc.get('bye'))
                 def bye(job):
                     print('bye' job)
                     job.doc.bye = True
 
             The *bye*-operation would be considered complete and therefore no longer
             eligible for execution once the 'bye' key in the job document evaluates to True.
+
+            An optional tag may be associated with the condition. These tags
+            are used by :meth:`~.detect_operation_graph` when comparing
+            conditions for equality. The tag defaults to the bytecode of the
+            function.
             """
             _parent_class = parent_class
 
-            def __init__(self, condition):
-                self.condition = condition
+            def __init__(self, condition, tag=None):
+                super(post, self).__init__(condition, tag)
 
             def __call__(self, func):
                 self._parent_class._OPERATION_POST_CONDITIONS[func].insert(0, self.condition)
                 return func
 
             @classmethod
             def copy_from(cls, *other_funcs):
                 "True if and only if all post conditions of other operation-function(s) are met."
-                def metacondition(job):
-                    return all(c(job)
-                               for other_func in other_funcs
-                               for c in cls._parent_class._collect_post_conditions()[other_func])
-                return cls(metacondition)
+                return cls(_create_all_metacondition(cls._parent_class._collect_post_conditions(),
+                                                     *other_funcs))
+
         return post
 
 
-class FlowProject(six.with_metaclass(_FlowProjectClass,
-                                     signac.contrib.Project)):
+class FlowProject(signac.contrib.Project, metaclass=_FlowProjectClass):
     """A signac project class specialized for workflow management.
 
     This class provides a command line interface for the definition, execution, and
     submission of workflows based on condition and operation functions.
 
     This is a typical example on how to use this class:
 
@@ -538,15 +583,15 @@
         @FlowProject.operation
         def hello(job):
             print('hello', job)
 
         FlowProject().main()
 
     :param config:
-        A signac configuaration, defaults to the configuration loaded
+        A signac configuration, defaults to the configuration loaded
         from the environment.
     :type config:
         A signac config object.
     """
 
     def __init__(self, config=None, environment=None):
         super(FlowProject, self).__init__(config=config)
@@ -573,34 +618,33 @@
         # Enable the use of buffered mode for certain functions
         try:
             self._use_buffered_mode = self.config['flow'].as_bool('use_buffered_mode')
         except KeyError:
             self._use_buffered_mode = False
 
     def _setup_template_environment(self):
-        """Setup the jinja2 template environemnt.
+        """Setup the jinja2 template environment.
 
         The templating system is used to generate templated scripts for the script()
         and submit_operations() / submit() function and the corresponding command line
-        sub commands.
+        subcommands.
         """
         if self._config.get('flow') and self._config['flow'].get('environment_modules'):
             envs = self._config['flow'].as_list('environment_modules')
         else:
             envs = []
 
         # Templates are searched in the local template directory first, then in additionally
         # installed packages, then in the main package 'templates' directory.
         extra_packages = []
         for env in envs:
             try:
                 extra_packages.append(jinja2.PackageLoader(env, 'templates'))
             except ImportError as error:
-                name = str(error) if six.PY2 else error.name
-                logger.warning("Unable to load template from package '{}'.".format(name))
+                logger.warning("Unable to load template from package '{}'.".format(error.name))
 
         load_envs = ([jinja2.FileSystemLoader(self._template_dir)] +
                      extra_packages +
                      [jinja2.PackageLoader('flow', 'templates')])
 
         template_environment = jinja2.Environment(
             loader=jinja2.ChoiceLoader(load_envs),
@@ -666,39 +710,141 @@
             def foo_label(job):
                 if job.document.get('foo', False):
                     return 'foo-label-text'
 
         The ``foo-label-text`` label will now show up in the status view for each job,
         where the ``foo`` key evaluates true.
 
-        If instead of a ``str``, the label functions returns any other type, the label
-        name will be the name of the function if and only if the return value evaluates
-        to ``True``, for example:
+        If the label functions returns any type other than ``str``, the label
+        name will be the name of the function if and only if the return value
+        evaluates to ``True``, for example:
 
         .. code-block:: python
 
             @FlowProject.label
             def foo_label(job):
                 return job.document.get('foo', False)
 
         Finally, you can specify a different default label name by providing it as the first
         argument to the ``label()`` decorator.
 
-        .. versionadded:: 0.6
+        :param label_name_or_func:
+            A label name or callable.
+        :type label_name_or_func:
+            str or callable
         """
         if callable(label_name_or_func):
             cls._LABEL_FUNCTIONS[label_name_or_func] = None
             return label_name_or_func
 
         def label_func(func):
             cls._LABEL_FUNCTIONS[func] = label_name_or_func
             return func
 
         return label_func
 
+    def detect_operation_graph(self):
+        """Determine the directed acyclic graph defined by operation pre- and
+        post-conditions.
+
+        In general, executing a given operation registered with a FlowProject
+        just involves checking the operation's pre- and post-conditions to
+        determine eligibility. More generally, however, the pre- and
+        post-conditions define a directed acyclic graph that governs the
+        execution of all operations. Visualizing this graph can be useful for
+        finding logic errors in the specified conditions, and having this graph
+        computed also enables additional execution modes. For example, using
+        this graph it is possible to determine exactly what operations need to
+        be executed in order to make the operation eligible so that the task of
+        executing all necessary operations can be automated.
+
+        The graph is determined by iterating over all pairs of operations and
+        checking for equality of pre- and post-conditions. The algorithm builds
+        an adjacency matrix based on whether the pre-conditions for one
+        operation match the post-conditions for another. The comparison of
+        operations is conservative; by default, conditions must be composed of
+        identical code to be identified as equal (technically, they must be
+        bytecode equivalent, i.e. ``cond1.__code__.co_code ==
+        cond2.__code__.co_code``). Users can specify that conditions should be
+        treated as equal by providing tags to the operations.
+
+        Given a FlowProject subclass defined in a module ``project.py``, the
+        output graph could be visualized using Matplotlib and NetworkX with the
+        following code:
+
+        .. code-block:: python
+
+            import numpy as np
+            import networkx as nx
+            from matplotlib import pyplot as plt
+
+            from project import Project
+
+            project = Project()
+            ops = project.operations.keys()
+            adj = np.asarray(project.detect_operation_graph())
+
+            plt.figure()
+            g = nx.DiGraph(adj)
+            pos = nx.spring_layout(g)
+            nx.draw(g, pos)
+            nx.draw_networkx_labels(
+                g, pos,
+                labels={key: name for (key, name) in
+                        zip(range(len(ops)), [o for o in ops])})
+
+            plt.show()
+
+        Raises a ``RuntimeError`` if a condition does not have a tag. This can
+        occur when using ``functools.partial``, and a manually specified
+        condition tag has not been set.
+
+        :raises: RuntimeError
+
+        """
+
+        def to_callbacks(conditions):
+            """Get the actual callables associated with FlowConditions."""
+            return [condition._callback for condition in conditions]
+
+        def unpack_conditions(condition_functions):
+            """Identify any metaconditions in the list and reduce them to the
+            functions that they are composed of. The callbacks argument is used
+            in recursive calls to the function and appended to directly, but
+            only returned at the end."""
+            callbacks = set()
+            for cf in condition_functions:
+                # condition may not have __name__ attribute in cases where functools is used
+                # for condition creation
+                if hasattr(cf, '__name__') and cf.__name__ == "_flow_metacondition":
+                    callbacks = callbacks.union(unpack_conditions(cf._composed_of))
+                else:
+                    if cf._flow_tag is None:
+                        raise RuntimeError("Condition {} was not tagged. To create a graph, ensure "
+                                           "each base condition has a ``__code__`` attribute or "
+                                           "manually specified tag.".format(cf))
+                    callbacks.add(cf._flow_tag)
+
+            return callbacks
+
+        ops = list(self.operations.items())
+        mat = [[0 for _ in range(len(ops))] for _ in range(len(ops))]
+
+        for i, (name1, op1) in enumerate(ops):
+            for j, (name2, op2) in enumerate(ops[i:]):
+                postconds1 = unpack_conditions(to_callbacks(op1._postconds))
+                postconds2 = unpack_conditions(to_callbacks(op2._postconds))
+                prereqs1 = unpack_conditions(to_callbacks(op1._prereqs))
+                prereqs2 = unpack_conditions(to_callbacks(op2._prereqs))
+                if postconds1.intersection(prereqs2):
+                    mat[i][j+i] = 1
+                elif prereqs1.intersection(postconds2):
+                    mat[j+i][i] = 1
+        return mat
+
     def _register_class_labels(self):
         """This function registers all label functions, which are part of the class definition.
 
         To register a class method or function as label function, use the generalized label()
         function.
         """
         def predicate(m):
@@ -715,78 +861,14 @@
     def _register_labels(self):
         "Register all label functions registered with this class and its parent classes."
         self._register_class_labels()
 
         for cls in type(self).__mro__:
             self._label_functions.update(getattr(cls, '_LABEL_FUNCTIONS', dict()))
 
-    """Decorator to add a pre-condition function for an operation function.
-
-    Use a label function (or any function of :code:`job`) as a condition:
-
-    .. code-block:: python
-
-        @FlowProject.label
-        def some_label(job):
-            return job.doc.ready == True
-
-        @FlowProject.operation
-        @FlowProject.pre(some_label)
-        def some_operation(job):
-            pass
-
-    Use a :code:`lambda` function of :code:`job` to create custom conditions:
-
-    .. code-block:: python
-
-        @FlowProject.operation
-        @FlowProject.pre(lambda job: job.doc.ready == True)
-        def some_operation(job):
-            pass
-
-    Use the post-conditions of an operation as a pre-condition for another operation:
-
-    .. code-block:: python
-
-        @FlowProject.operation
-        @FlowProject.post(lambda job: job.isfile('output.txt'))
-        def previous_operation(job):
-            pass
-
-        @FlowProject.operation
-        @FlowProject.pre.after(previous_operation)
-        def some_operation(job):
-            pass
-    """
-
-    """Decorator to add a post-condition function for an operation function.
-
-    Use a label function (or any function of :code:`job`) as a condition:
-
-    .. code-block:: python
-
-        @FlowProject.label
-        def some_label(job):
-            return job.doc.finished == True
-
-        @FlowProject.operation
-        @FlowProject.post(some_label)
-        def some_operation(job):
-            pass
-
-    Use a :code:`lambda` function of :code:`job` to create custom conditions:
-
-    .. code-block:: python
-
-        @FlowProject.operation
-        @FlowProject.post(lambda job: job.doc.finished == True)
-        def some_operation(job):
-            pass
-    """
-
     ALIASES = dict(
         unknown='U',
         registered='R',
         queued='Q',
         active='A',
         inactive='I',
         requires_attention='!'
@@ -798,51 +880,50 @@
         "Use alias if specified."
         try:
             return abbreviate(x, cls.ALIASES.get(x, x))
         except TypeError:
             return x
 
     @classmethod
-    @deprecated(deprecated_in="0.8", removed_in="1.0")
+    @deprecated(
+        deprecated_in="0.8", removed_in="0.10",
+        current_version=__version__)
     def update_aliases(cls, aliases):
         "Update the ALIASES table for this class."
         cls.ALIASES.update(aliases)
 
     def _fn_bundle(self, bundle_id):
         "Return the canonical name to store bundle information."
         return os.path.join(self.root_directory(), '.bundles', bundle_id)
 
     def _store_bundled(self, operations):
         """Store operation-ids as part of a bundle and return bundle id.
 
-        The operation identifiers are stored in a  text within a file
-        determined by the _fn_bundle() method.
-
-        This may be used to idenfity the status of individual operations
-        root directory. This is necessary to be able to identify each
-
-        A single operation will not be stored, but instead the operation's
-        id is directly returned.
+        The operation identifiers are stored in a text file whose name is
+        determined by the _fn_bundle() method. This may be used to identify
+        the status of individual operations from the bundle id. A single
+        operation will not be stored, but instead the operation's id is
+        directly returned.
 
         :param operations:
             The operations to bundle.
         :type operations:
             A sequence of instances of :py:class:`.JobOperation`
         :return:
-            The  bundle id
+            The bundle id.
         :rtype:
             str
         """
         if len(operations) == 1:
             return operations[0].get_id()
         else:
             h = '.'.join(op.get_id() for op in operations)
             bid = '{}/bundle/{}'.format(self, sha1(h.encode('utf-8')).hexdigest())
             fn_bundle = self._fn_bundle(bid)
-            _mkdir_p(os.path.dirname(fn_bundle))
+            os.makedirs(os.path.dirname(fn_bundle), exist_ok=True)
             with open(fn_bundle, 'w') as file:
                 for operation in operations:
                     file.write(operation.get_id() + '\n')
             return bid
 
     def _expand_bundled_jobs(self, scheduler_jobs):
         "Expand jobs which were submitted as part of a bundle."
@@ -1015,16 +1096,14 @@
                      expand=False, all_ops=False, only_incomplete=False, dump_json=False,
                      unroll=True, compact=False, pretty=False,
                      file=None, err=None, ignore_errors=False,
                      no_parallelize=False, template=None, profile=False,
                      eligible_jobs_max_lines=None):
         """Print the status of the project.
 
-        .. versionchanged:: 0.6
-
         :param jobs:
             Only execute operations for the given jobs, or all if the argument is omitted.
         :type jobs:
             Sequence of instances :class:`.Job`.
         :param overview:
             Aggregate an overview of the project' status.
         :type overview:
@@ -1091,15 +1170,15 @@
         :type ignore_errors:
             bool
         :param no_parallelize:
             Do not parallelize the status update.
         :type no_parallelize:
             bool
         :param template:
-            user provided Jinja2 template file.
+            User provided Jinja2 template file.
         :type template:
             str
         """
         if file is None:
             file = sys.stdout
         if err is None:
             err = sys.stderr
@@ -1116,15 +1195,15 @@
                 template = 'status_compact.jinja'
             else:
                 template = 'status.jinja'
 
         if eligible_jobs_max_lines is None:
             eligible_jobs_max_lines = flow_config.get_config_value('eligible_jobs_max_lines')
 
-        # initialize jinja2 template evnronment and necessary filters
+        # initialize jinja2 template environment and necessary filters
         template_environment = self._template_environment()
 
         def draw_progressbar(value, total, width=40):
             """Visualize progess with a progress bar.
 
             :param value:
                 The current progress as a fraction of total.
@@ -1151,65 +1230,65 @@
             :param job_ops:
                 Operations information for a job.
             :type job_ops:
                 OrderedDict
             :param scheduler_status_code:
                 Dictionary information for status code
             :type scheduler_status_code:
-                Dictionary
+                dict
             :param all_ops:
                 Boolean value indicate if all operations should be displayed
             :type all_ops:
-                Boolean
+                bool
             """
 
             if scheduler_status_code[job_op['scheduler_status']] != 'U' or \
                job_op['eligible'] or all_ops:
                 return True
             else:
                 return False
 
         def get_operation_status(operation_info, symbols):
             """Determine the status of an operation.
 
             :param operation_info:
-                Dicionary containing operation information
+                Dictionary containing operation information.
             :type operation_info:
-                Dictionary
+                dict
             :param symbols:
-                Dicionary containing code for different job status
+                Dictionary containing code for different job status.
             :type symbols:
-                Dictionary
+                dict
             """
 
             if operation_info['scheduler_status'] >= JobStatus.active:
-                op_status = u'running'
+                op_status = 'running'
             elif operation_info['scheduler_status'] > JobStatus.inactive:
-                op_status = u'active'
+                op_status = 'active'
             elif operation_info['completed']:
-                op_status = u'completed'
+                op_status = 'completed'
             elif operation_info['eligible']:
-                op_status = u'eligible'
+                op_status = 'eligible'
             else:
-                op_status = u'ineligible'
+                op_status = 'ineligible'
 
             return symbols[op_status]
 
         if pretty:
             def highlight(s, eligible):
                 """Change font to bold within jinja2 template
 
                 :param s:
                     The string to be printed
                 :type s:
                     str
                 :param eligible:
                     Boolean value for job eligibility
                 :type eligible:
-                    Boolean
+                    bool
                 """
                 if eligible:
                     return '\033[1m' + s + '\033[0m'
                 else:
                     return s
         else:
             def highlight(s, eligible):
@@ -1218,15 +1297,15 @@
                 :param s:
                     The string to be printed
                 :type s:
                     str
                 :param eligible:
                     Boolean value for job eligibility
                 :type eligible:
-                    boolean
+                    bool
                 """
                 return s
 
         template_environment.filters['highlight'] = highlight
         template_environment.filters['draw_progressbar'] = draw_progressbar
         template_environment.filters['get_operation_status'] = get_operation_status
         template_environment.filters['job_filter'] = job_filter
@@ -1410,28 +1489,28 @@
                     column_width_total_label, len(', '.join(job['labels'])))
             if compact:
                 num_operations = len(self._operations)
                 column_width_operations_count = len(str(max(num_operations-1, 0))) + 3
 
             if pretty:
                 OPERATION_STATUS_SYMBOLS = OrderedDict([
-                    ('ineligible', u'\u25cb'),   # open circle
-                    ('eligible', u'\u25cf'),     # black circle
-                    ('active', u'\u25b9'),       # open triangle
-                    ('running', u'\u25b8'),      # black triangle
-                    ('completed', u'\u2714'),    # check mark
+                    ('ineligible', '\u25cb'),   # open circle
+                    ('eligible', '\u25cf'),     # black circle
+                    ('active', '\u25b9'),       # open triangle
+                    ('running', '\u25b8'),      # black triangle
+                    ('completed', '\u2714'),    # check mark
                 ])
                 "Pretty (unicode) symbols denoting the execution status of operations."
             else:
                 OPERATION_STATUS_SYMBOLS = OrderedDict([
-                    ('ineligible', u'-'),
-                    ('eligible', u'+'),
-                    ('active', u'*'),
-                    ('running', u'>'),
-                    ('completed', u'X')
+                    ('ineligible', '-'),
+                    ('eligible', '+'),
+                    ('active', '*'),
+                    ('running', '>'),
+                    ('completed', 'X')
                 ])
                 "Symbols denoting the execution status of operations."
             operation_status_legend = ' '.join('[{}]:{}'.format(v, k)
                                                for k, v in OPERATION_STATUS_SYMBOLS.items())
 
         context['jobs'] = list(statuses.values())
         context['overview'] = overview
@@ -1489,16 +1568,14 @@
             print('\n' + '\n'.join(profiling_results), file=file)
 
     def run_operations(self, operations=None, pretend=False, np=None, timeout=None, progress=False):
         """Execute the next operations as specified by the project's workflow.
 
         See also: :meth:`~.run`
 
-        .. versionadded:: 0.6
-
         :param operations:
             The operations to execute (optional).
         :type operations:
             Sequence of instances of :class:`.JobOperation`
         :param pretend:
             Do not actually execute the operations, but show which command would have been used.
         :type pretend:
@@ -1513,39 +1590,35 @@
         :type timeout:
             int
         :param progress:
             Show a progress bar during execution.
         :type progess:
             bool
         """
-        if six.PY2 and timeout is not None:
-            logger.warning(
-                "The timeout argument for run() is not supported for "
-                "Python 2.7 and will be ignored!")
         if timeout is not None and timeout < 0:
             timeout = None
         if operations is None:
             operations = list(self._get_pending_operations(self))
         else:
             operations = list(operations)   # ensure list
 
         if np is None or np == 1 or pretend:
             if progress:
                 operations = tqdm(operations)
             for operation in operations:
                 if pretend:
                     print(operation.cmd)
                 else:
-                    self._fork(operation, timeout)
+                    self._execute_operation(operation, timeout)
         else:
             logger.debug("Parallelized execution of {} operation(s).".format(len(operations)))
             with contextlib.closing(Pool(processes=cpu_count() if np < 0 else np)) as pool:
                 logger.debug("Parallelized execution of {} operation(s).".format(len(operations)))
                 try:
-                    from six.moves import cPickle as pickle
+                    import pickle
                     self._run_operations_in_parallel(pool, pickle, operations, progress, timeout)
                     logger.debug("Used cPickle module for serialization.")
                 except Exception as error:
                     if not isinstance(error, (pickle.PickleError, self._PickleError)) and\
                             'pickle' not in str(error).lower():
                         raise    # most likely not a pickle related error...
 
@@ -1589,46 +1662,64 @@
         try:
             s_project = pickle.dumps(self)
             s_tasks = [(pickle.loads, s_project, self._dumps_op(op))
                        for op in tqdm(operations, desc='Serialize tasks', file=sys.stderr)]
         except Exception as error:  # Masking all errors since they must be pickling related.
             raise self._PickleError(error)
 
-        results = [pool.apply_async(_fork_with_serialization, task) for task in s_tasks]
+        results = [pool.apply_async(_execute_serialized_operation, task) for task in s_tasks]
 
         for result in tqdm(results) if progress else results:
             result.get(timeout=timeout)
 
-    def _fork(self, operation, timeout=None):
+    def _execute_operation(self, operation, timeout=None):
         logger.info("Execute operation '{}'...".format(operation))
 
-        # Execute without forking if possible...
-        if timeout is None and operation.name in self._operation_functions and \
-                operation.directives.get('executable', sys.executable) == sys.executable:
-            logger.debug("Able to optimize execution of operation '{}'.".format(operation))
-            self._operation_functions[operation.name](operation.job)
-        else:   # need to fork
-            fork(cmd=operation.cmd, timeout=timeout)
+        # Check if we need to fork for operation execution...
+        if (
+            # The 'fork' directive was provided and evaluates to True:
+            operation.directives.get('fork', False)
+            # Separate process needed to cancel with timeout:
+            or timeout is not None
+            # The operation function is not registered with the class:
+            or operation.name not in self._operation_functions
+            # The specified executable is not the same as the interpreter instance:
+            or operation.directives.get('executable', sys.executable) != sys.executable
+        ):
+            # ... need to fork:
+            logger.debug(
+                "Forking to execute operation '{}' with "
+                "cmd '{}'.".format(operation, operation.cmd))
+            subprocess.run(operation.cmd, shell=True, timeout=timeout, check=True)
+        else:
+            # ... executing operation in interpreter process as function:
+            logger.debug(
+                "Executing operation '{}' with current interpreter "
+                "process ({}).".format(operation, os.getpid()))
+            try:
+                self._operation_functions[operation.name](operation.job)
+            except Exception as e:
+                raise UserOperationError(
+                    'An exception was raised during operation {operation.name} '
+                    'for job {operation.job}.'.format(operation=operation)) from e
 
     def run(self, jobs=None, names=None, pretend=False, np=None, timeout=None, num=None,
             num_passes=1, progress=False, order=None):
         """Execute all pending operations for the given selection.
 
         This function will run in an infinite loop until all pending operations
-        have been executed or the total number of passes per operation or the total
-        number of exeutions have been reached.
+        are executed, unless it reaches the maximum number of passes per
+        operation or the maximum number of executions.
 
         By default there is no limit on the total number of executions, but a specific
         operation will only be executed once per job. This is to avoid accidental
         infinite loops when no or faulty post conditions are provided.
 
         See also: :meth:`~.run_operations`
 
-        .. versionchanged:: 0.6
-
         :param jobs:
             Only execute operations for the given jobs, or all if the argument is omitted.
         :type jobs:
             Sequence of instances :class:`.Job`.
         :param names:
             Only execute operations that are in the provided set of names, or all, if the
             argument is omitted.
@@ -1691,15 +1782,15 @@
         # Negative values for the execution limits, means 'no limit'.
         if num_passes and num_passes < 0:
             num_passes = None
         if num and num < 0:
             num = None
 
         # The 'names' argument must be a sequence, not a string.
-        if isinstance(names, six.string_types):
+        if isinstance(names, str):
             raise ValueError(
                 "The names argument of FlowProject.run() must be a sequence of strings, "
                 "not a string.")
 
         messages = list()
 
         def log(msg, lvl=logging.INFO):
@@ -1786,17 +1877,17 @@
             if requires and requires.difference(self.labels(job)):
                 continue
             cmd_ = cmd.format(job=job)
             yield JobOperation(name=cmd_.replace(' ', '-'), cmd=cmd_, job=job)
 
     def _get_pending_operations(self, jobs, operation_names=None):
         "Get all pending operations for the given selection."
-        assert not isinstance(operation_names, six.string_types)
+        assert not isinstance(operation_names, str)
         for op in self.next_operations(* jobs):
-            if operation_names is None or any(fullmatch(n, op.name) for n in operation_names):
+            if operation_names is None or any(re.fullmatch(n, op.name) for n in operation_names):
                 yield op
 
     @contextlib.contextmanager
     def _potentially_buffered(self):
         if self._use_buffered_mode:
             logger.debug("Entering buffered mode...")
             with signac.buffered():
@@ -1810,15 +1901,15 @@
 
         :param operations:
             The operations to execute.
         :type operations:
             Sequence of instances of :class:`.JobOperation`
         :param parallel:
             Execute all operations in parallel (default is False).
-        :param parallel:
+        :type parallel:
             bool
         :param template:
             The name of the template to use to generate the script.
         :type template:
             str
         :param show_template_help:
             Show help related to the templating system and then exit.
@@ -1862,17 +1953,15 @@
         if show_template_help:
             self._show_template_help_and_exit(template_environment, context)
         return template.render(** context)
 
     def submit_operations(self, operations, _id=None, env=None, parallel=False, flags=None,
                           force=False, template='script.sh', pretend=False,
                           show_template_help=False, **kwargs):
-        """Submit a sequence of operations to the scheduler.
-
-        .. versionchanged:: 0.6
+        r"""Submit a sequence of operations to the scheduler.
 
         :param operations:
             The operations to submit.
         :type operations:
             A sequence of instances of :py:class:`.JobOperation`
         :param _id:
             The _id to be used for this submission.
@@ -1899,18 +1988,18 @@
             for testing the submission workflow.
         :type pretend:
             bool
         :param show_template_help:
             Show information about available template variables and filters and exit.
         :type show_template_help:
             bool
-        :param kwargs:
+        :param \*\*kwargs:
             Additional keyword arguments to be forwarded to the scheduler.
         :return:
-            Return the submission status after successful submission or None.
+            Returns the submission status after successful submission or None.
         """
         if _id is None:
             _id = self._store_bundled(operations)
         if env is None:
             env = self._environment
 
         print("Submitting cluster job '{}':".format(_id), file=sys.stderr)
@@ -1940,31 +2029,31 @@
             # Keys which were explicitly set by the user, but are not evaluated by the
             # template engine are cause for concern and might hint at a bug in the template
             # script or ill-defined directives. Here we check whether all directive keys that
             # have been explicitly set by the user were actually evaluated by the template
             # engine and warn about those that have not been.
             keys_unused = {
                 key for op in operations for key in
-                op.directives._keys_set_by_user.difference(op.directives.keys_used)}
+                op.directives._keys_set_by_user.difference(op.directives.keys_used)
+                if key not in ('fork', )  # whitelist
+            }
             if keys_unused:
                 logger.warning(
                     "Some of the keys provided as part of the directives were not used by "
                     "the template script, including: {}".format(
                         ', '.join(sorted(keys_unused))))
             if pretend:
                 print(script)
             else:
                 return env.submit(_id=_id, script=script, flags=flags, **kwargs)
 
     def submit(self, bundle_size=1, jobs=None, names=None, num=None, parallel=False,
                force=False, walltime=None, env=None, **kwargs):
         """Submit function for the project's main submit interface.
 
-        .. versionchanged:: 0.6
-
         :param bundle_size:
             Specify the number of operations to be bundled into one submission, defaults to 1.
         :type bundle_size:
             int
         :param jobs:
             Only submit operations associated with the provided jobs. Defaults to all jobs.
         :type jobs:
@@ -1983,20 +2072,20 @@
         :type parallel:
             bool
         :param force:
             Ignore all warnings or checks during submission, just submit.
         :type force:
             bool
         :param walltime:
-            Specify the walltime in hours or as instance of datetime.timedelta.
+            Specify the walltime in hours or as instance of :py:class:`datetime.timedelta`.
         """
         # Regular argument checks and expansion
         if jobs is None:
             jobs = self  # select all jobs
-        if isinstance(names, six.string_types):
+        if isinstance(names, str):
             raise ValueError(
                 "The 'names' argument must be a sequence of strings, however you "
                 "provided a single string: {}.".format(names))
         if env is None:
             env = self._environment
         if walltime is not None:
             try:
@@ -2010,15 +2099,15 @@
         with self._potentially_buffered():
             operations = (op for op in self._get_pending_operations(jobs, names)
                           if self._eligible_for_submission(op))
             if num is not None:
                 operations = list(islice(operations, num))
 
         # Bundle them up and submit.
-        for bundle in make_bundles(operations, bundle_size):
+        for bundle in _make_bundles(operations, bundle_size):
             status = self.submit_operations(
                 operations=bundle, env=env, parallel=parallel,
                 force=force, walltime=walltime, **kwargs)
 
             if status is not None:  # operations were submitted, store status
                 for op in bundle:
                     op.set_status(status)
@@ -2080,15 +2169,15 @@
                  "can be configured with the 'template_dir' configuration variable. "
                  "Default: '{}'.".format(default))
         template_group.add_argument(
             '--template-help',
             dest='show_template_help',
             action='store_true',
             help="Show information about the template context, including available variables "
-                 "and filter funtions; then exit.")
+                 "and filter functions; then exit.")
 
     @classmethod
     def _add_job_selection_args(cls, parser):
         parser.add_argument(
             '-j', '--job-id',
             type=str,
             nargs='+',
@@ -2124,15 +2213,15 @@
 
     @classmethod
     def _add_operation_bundling_arg_group(cls, parser):
         """Add argument group to parser for operation bundling."""
 
         bundling_group = parser.add_argument_group(
             'bundling',
-            "Bundle mutiple operations for execution, e.g., to submit them "
+            "Bundle multiple operations for execution, e.g., to submit them "
             "all together to a cluster job, or execute them in parallel within "
             "an execution script.")
         bundling_group.add_argument(
             '-b', '--bundle',
             type=int,
             nargs='?',
             const=0,
@@ -2157,15 +2246,18 @@
         direct_cmd_group.add_argument(
             '--requires',
             type=str,
             nargs='+',
             help="Manually specify all labels that are required for the direct command "
                  "to be considered eligible for execution.")
 
-    @deprecated(deprecated_in="0.8", removed_in="1.0", details="Use export_job_statuses() instead.")
+    @deprecated(
+        deprecated_in="0.8", removed_in="0.10",
+        current_version=__version__,
+        details="Use export_job_statuses() instead.")
     def export_job_stati(self, collection, stati):
         "Export the job stati to a database collection."
         self.export_job_statuses(self, collection, stati)
 
     def export_job_statuses(self, collection, statuses):
         "Export the job statuses to a database collection."
         for status in statuses:
@@ -2269,15 +2361,15 @@
                     label_value = label_func(self, job)
                 except Exception:
                     label_func = getattr(self, label.__func__.__name__)
                     label_value = label_func(job)
 
             label_name = getattr(label_func, '_label_name', label_func.__name__)
             assert label_name is not None
-            if isinstance(label_value, six.string_types):
+            if isinstance(label_value, str):
                 yield label_value
             elif bool(label_value) is True:
                 yield label_name
 
     def add_operation(self, name, cmd, pre=None, post=None, **kwargs):
         """
         Add an operation to the workflow.
@@ -2293,15 +2385,15 @@
         Any FlowOperation is associated with a specific command, which should be
         a function of :py:class:`~signac.contrib.job.Job`. The command (cmd) can
         be stated as function, either by using str-substitution based on a job's
         attributes, or by providing a unary callable, which expects an instance
         of job as its first and only positional argument.
 
         For example, if we wanted to define a command for a program called 'hello',
-        which expects a job id as its first argument, we could contruct the following
+        which expects a job id as its first argument, we could construct the following
         two equivalent operations:
 
         .. code-block:: python
 
             op = FlowOperation('hello', cmd='hello {job._id}')
             op = FlowOperation('hello', cmd=lambda 'hello {}'.format(job._id))
 
@@ -2318,40 +2410,43 @@
         argument and return either True or False.
 
         An operation is considered "eligible" for execution when all pre-requirements
         are met and when at least one of the post-conditions is not met.
         Requirements are always met when the list of requirements is empty and
         post-conditions are never met when the list of post-conditions is empty.
 
-        Please note, eligibility in this contexts refers only to the workflow pipline
+        Please note, eligibility in this contexts refers only to the workflow pipeline
         and not to other contributing factors, such as whether the job-operation is currently
         running or queued.
 
         :param name:
-            A unique identifier for this operation, may be freely choosen.
+            A unique identifier for this operation, which may be freely chosen.
         :type name:
             str
         :param cmd:
             The command to execute operation; should be a function of job.
         :type cmd:
             str or callable
         :param pre:
-            required conditions
+            Required conditions.
         :type pre:
             sequence of callables
         :param post:
-            post-conditions to determine completion
+            Post-conditions to determine completion.
         :type pre:
             sequence of callables
         """
         if name in self.operations:
             raise KeyError("An operation with this identifier is already added.")
         self.operations[name] = FlowOperation(cmd=cmd, pre=pre, post=post, directives=kwargs)
 
-    @deprecated(deprecated_in="0.8", removed_in="1.0", details="Use labels() instead.")
+    @deprecated(
+        deprecated_in="0.8", removed_in="0.10",
+        current_version=__version__,
+        details="Use labels() instead.")
     def classify(self, job):
         """Generator function which yields labels for job.
 
         By default, this method yields from the project's labels() method.
 
         :param job:
             The signac job handle.
@@ -2398,15 +2493,18 @@
         :yield:
             All instances of :class:`~.JobOperation` jobs are eligible for.
         """
         for job in jobs:
             for op in self._job_operations(job, True):
                 yield op
 
-    @deprecated(deprecated_in="0.8", removed_in="1.0", details="Use next_operations() instead.")
+    @deprecated(
+        deprecated_in="0.8", removed_in="0.10",
+        current_version=__version__,
+        details="Use next_operations() instead.")
     def next_operation(self, job):
         """Determine the next operation for this job.
 
         :param job:
             The signac job handle.
         :type job:
             :class:`~signac.contrib.job.Job`
@@ -2427,41 +2525,31 @@
         .. code-block:: python
 
             @FlowProject.operation
             def hello(job):
                 print('Hello', job)
 
         See also: :meth:`~.flow.FlowProject.add_operation`.
-
-        .. versionadded:: 0.6
         """
-        if isinstance(func, six.string_types):
+        if isinstance(func, str):
             return lambda op: cls.operation(op, name=func)
 
         if name is None:
             name = func.__name__
 
         if (name, func) in cls._OPERATION_FUNCTIONS:
             raise ValueError(
                 "An operation with name '{}' is already registered.".format(name))
 
-        if six.PY2:
-            signature = inspect.getargspec(func)
-            if len(signature.args) > 1:
-                if signature.defaults is None or len(signature.defaults) + 1 < len(signature.args):
-                    raise ValueError(
-                        "Only the first argument in an operation argument may not have "
-                        "a default value! ({})".format(name))
-        else:
-            signature = inspect.signature(func)
-            for i, (k, v) in enumerate(signature.parameters.items()):
-                if i and v.default is inspect.Parameter.empty:
-                    raise ValueError(
-                        "Only the first argument in an operation argument may not have "
-                        "a default value! ({})".format(name))
+        signature = inspect.signature(func)
+        for i, (k, v) in enumerate(signature.parameters.items()):
+            if i and v.default is inspect.Parameter.empty:
+                raise ValueError(
+                    "Only the first argument in an operation argument may not have "
+                    "a default value! ({})".format(name))
 
         # Append the name and function to the class registry
         cls._OPERATION_FUNCTIONS.append((name, func))
         return func
 
     @classmethod
     def _collect_operations(cls):
@@ -2478,20 +2566,20 @@
         for parent_class in cls.__mro__:
             for func, conds in getattr(parent_class, attr, dict()).items():
                 ret[func].extend(conds)
         return ret
 
     @classmethod
     def _collect_pre_conditions(cls):
-        "Collect all pre-conditions that were add via decorator."
+        "Collect all pre-conditions that were added via decorator."
         return cls._collect_conditions('_OPERATION_PRE_CONDITIONS')
 
     @classmethod
     def _collect_post_conditions(cls):
-        "Collect all post-conditions that were add via decorator."
+        "Collect all post-conditions that were added via decorator."
         return cls._collect_conditions('_OPERATION_POST_CONDITIONS')
 
     def _register_operations(self):
         "Register all operation functions registered with this class and its parent classes."
         operations = self._collect_operations()
         pre_conditions = self._collect_pre_conditions()
         post_conditions = self._collect_post_conditions()
@@ -2542,15 +2630,17 @@
         """
         if job_operation is None:
             return False
         if job_operation.get_status() >= JobStatus.submitted:
             return False
         return True
 
-    @deprecated(deprecated_in="0.8", removed_in="1.0")
+    @deprecated(
+        deprecated_in="0.8", removed_in="0.10",
+        current_version=__version__)
     def eligible_for_submission(self, job_operation):
         return self._eligible_for_submission(self, job_operation)
 
     def _main_status(self, args):
         "Print status overview."
         jobs = self._select_jobs_from_args(args)
         if args.compact and not args.unroll:
@@ -2564,57 +2654,50 @@
             args['detailed'] = args['all_ops'] = True
 
         start = time.time()
         try:
             self.print_status(jobs=jobs, **args)
         except NoSchedulerError:
             self.print_status(jobs=jobs, **args)
-        except Exception:
-            logger.error(
-                "Error occured during status update. Use '--show-traceback' to "
-                "show the full traceback or '--ignore-errors' to complete the "
-                "update anyways.")
+        except Exception as error:
             if show_traceback:
-                raise
+                logger.error(
+                    "Error during status update: {}\nUse '--ignore-errors' to "
+                    "complete the update anyways.".format(str(error)))
+            else:
+                logger.error(
+                    "Error during status update: {}\nUse '--ignore-errors' to "
+                    "complete the update anyways or '--show-traceback' to show "
+                    "the full traceback.".format(str(error)))
+                error = error.__cause__  # Always show the user traceback cause.
+            traceback.print_exception(type(error), error, error.__traceback__)
         else:
             # Use small offset to account for overhead with few jobs
             delta_t = (time.time() - start - 0.5) / max(len(jobs), 1)
             config_key = 'status_performance_warn_threshold'
             warn_threshold = flow_config.get_config_value(config_key)
             if not args['profile'] and delta_t > warn_threshold >= 0:
                 print(
                     "WARNING: "
-                    "The status compilation took more than {}s per job. Consider to "
-                    "use `--profile` to determine bottlenecks within your project "
+                    "The status compilation took more than {}s per job. Consider "
+                    "using `--profile` to determine bottlenecks within your project "
                     "workflow definition.\n"
                     "Execute `signac config set flow.{} VALUE` to specify the "
                     "warning threshold in seconds. Use -1 to completely suppress this "
                     "warning."
                     .format(warn_threshold, config_key), file=sys.stderr)
 
     def _main_next(self, args):
         "Determine the jobs that are eligible for a specific operation."
         for job in self:
             if args.name in {op.name for op in self.next_operations(job)}:
                 print(job)
 
     def _main_run(self, args):
         "Run all (or select) job operations."
-        if args.hidden_operation_name:
-            print(
-                "WARNING: "
-                "The run command expects operation names under the -o/--operation argument "
-                "as of version 0.6.\n         Positional arguments will no longer be "
-                "accepted beginning with version 0.7.",
-                file=sys.stderr)
-            if args.operation_name:
-                args.operation_name.extend(args.hidden_operation_name)
-            else:
-                args.operation_name = args.hidden_operation_name
-
         # Select jobs:
         jobs = self._select_jobs_from_args(args)
 
         # Setup partial run function, because we need to call this either
         # inside some context managers or not based on whether we need
         # to switch to the project root directory or not.
         run = functools.partial(self.run,
@@ -2670,15 +2753,15 @@
         # Gather all pending operations ...
         with self._potentially_buffered():
             ops = (op for op in self._get_pending_operations(jobs, args.operation_name)
                    if self._eligible_for_submission(op))
             ops = list(islice(ops, args.num))
 
         # Bundle operations up, generate the script, and submit to scheduler.
-        for bundle in make_bundles(ops, args.bundle_size):
+        for bundle in _make_bundles(ops, args.bundle_size):
             status = self.submit_operations(operations=bundle, **kwargs)
             if status is not None:
                 for op in bundle:
                     op.set_status(status)
 
     def _main_exec(self, args):
         if len(args.jobid):
@@ -2689,15 +2772,15 @@
             try:
                 operation_function = self._operation_functions[args.operation]
             except KeyError:
                 operation = self._operations[args.operation]
 
                 def operation_function(job):
                     cmd = operation(job).format(job=job)
-                    fork(cmd=cmd)
+                    subprocess.run(cmd, shell=True, check=True)
 
         except KeyError:
             raise KeyError("Unknown operation '{}'.".format(args.operation))
 
         if getattr(operation_function, '_flow_aggregate', False):
             operation_function(jobs)
         else:
@@ -2714,15 +2797,15 @@
             try:
                 return [self.open_job(id=job_id) for job_id in args.job_id]
             except KeyError as error:
                 raise LookupError("Did not find job with id {}.".format(error))
         else:
             filter_ = parse_filter_arg(args.filter)
             doc_filter = parse_filter_arg(args.doc_filter)
-            return legacy.JobsCursorWrapper(self, filter_, doc_filter)
+            return JobsCursor(self, filter_, doc_filter)
 
     def main(self, parser=None):
         """Call this function to use the main command line interface.
 
         In most cases one would want to call this function as part of the
         class definition, e.g.:
 
@@ -2796,19 +2879,14 @@
             help="The name of the operation.")
         parser_next.set_defaults(func=self._main_next)
 
         parser_run = subparsers.add_parser(
             'run',
             parents=[base_parser],
         )
-        parser_run.add_argument(          # Hidden positional arguments for backwards-compatibility.
-            'hidden_operation_name',
-            type=str,
-            nargs='*',
-            help=argparse.SUPPRESS)
         self._add_operation_selection_arg_group(parser_run, list(sorted(self._operations)))
 
         execution_group = parser_run.add_argument_group('execution')
         execution_group.add_argument(
             '--pretend',
             action='store_true',
             help="Do not actually execute commands, just show them.")
@@ -2911,63 +2989,73 @@
         if hasattr(args, 'parameters'):
             if args.parameters is not None and len(args.parameters) == 0:
                 args.parameters = self.PRINT_STATUS_ALL_VARYING_PARAMETERS
 
         # Set verbosity level according to the `-v` argument.
         logging.basicConfig(level=max(0, logging.WARNING - 10 * args.verbose))
 
-        def _exit_or_raise():
+        def _show_traceback_and_exit(error):
             if args.show_traceback:
-                raise
+                traceback.print_exception(type(error), error, error.__traceback__)
+            elif isinstance(error, (UserOperationError, UserConditionError)):
+                # Always show the user traceback cause.
+                error = error.__cause__
+                traceback.print_exception(type(error), error, error.__traceback__)
+                print("Execute with '--show-traceback' or '--debug' to show the "
+                      "full traceback.", file=sys.stderr)
             else:
-                sys.exit(1)
+                print("Execute with '--show-traceback' or '--debug' to get more "
+                      "information.", file=sys.stderr)
+            sys.exit(1)
 
         try:
             args.func(args)
         except NoSchedulerError as error:
             print("ERROR: {}".format(error),
                   "Consider to use the 'script' command to generate an execution script instead.",
                   file=sys.stderr)
-            _exit_or_raise()
+            _show_traceback_and_exit(error)
         except SubmitError as error:
             print("Submission error:", error, file=sys.stderr)
-            _exit_or_raise()
-        except (TimeoutError, TimeoutExpired):
+            _show_traceback_and_exit(error)
+        except (TimeoutError, subprocess.TimeoutExpired) as error:
             print("Error: Failed to complete execution due to "
                   "timeout ({}s).".format(args.timeout), file=sys.stderr)
-            _exit_or_raise()
+            _show_traceback_and_exit(error)
         except Jinja2TemplateNotFound as error:
             print("Did not find template script '{}'.".format(error), file=sys.stderr)
-            _exit_or_raise()
-        except AssertionError:
+            _show_traceback_and_exit(error)
+        except AssertionError as error:
             if not args.show_traceback:
-                print("ERROR: Encountered internal error during program execution. "
-                      "Execute with '--show-traceback' or '--debug' to get more "
-                      "information.", file=sys.stderr)
-            _exit_or_raise()
+                print("ERROR: Encountered internal error during program execution.",
+                      file=sys.stderr)
+            _show_traceback_and_exit(error)
+        except (UserOperationError, UserConditionError) as error:
+            if str(error):
+                print("ERROR: {}\n".format(error), file=sys.stderr)
+            else:
+                print("ERROR: Encountered error during program execution.\n",
+                      file=sys.stderr)
+            _show_traceback_and_exit(error)
         except Exception as error:
-            if not args.debug:
-                if str(error):
-                    print("ERROR: Encountered error during program execution: '{}'\n"
-                          "Execute with '--show-traceback' or '--debug' to get "
-                          "more information.".format(error), file=sys.stderr)
-                else:
-                    print("ERROR: Encountered error during program execution.\n"
-                          "Execute with '--show-traceback' or '--debug' to get "
-                          "more information.", file=sys.stderr)
-            _exit_or_raise()
+            if str(error):
+                print("ERROR: Encountered error during program execution: "
+                      "'{}'\n".format(error), file=sys.stderr)
+            else:
+                print("ERROR: Encountered error during program execution.\n",
+                      file=sys.stderr)
+            _show_traceback_and_exit(error)
 
 
-def _fork_with_serialization(loads, project, operation):
-    """Invoke the _fork() method on a serialized project instance."""
+def _execute_serialized_operation(loads, project, operation):
+    """Invoke the _execute_operation() method on a serialized project instance."""
     project = loads(project)
-    project._fork(project._loads_op(operation))
+    project._execute_operation(project._loads_op(operation))
 
 
-###
 # Status-related helper functions
 
 
 _FMT_SCHEDULER_STATUS = {
     JobStatus.unknown: 'U',
     JobStatus.registered: 'R',
     JobStatus.inactive: 'I',
```

## flow/template.py

```diff
@@ -2,56 +2,36 @@
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """This module contains the FlowProject module templates.
 
 These templates can be initialized via the init() function defined
 in this module and the main 'flow' command line interface.
 """
-from __future__ import print_function
 import os
 import sys
 import errno
 import logging
-
-from signac.common import six
-try:
-    import jinja2
-    from jinja2 import TemplateNotFound as Jinja2TemplateNotFound
-except ImportError:
-    # Mock exception, which will never be raised.
-    class Jinja2TemplateNotFound(Exception):
-        pass
-
-    JINJA2 = False
-else:
-    JINJA2 = True
-
-from .util.misc import _is_identifier
+import jinja2
 
 
 logger = logging.getLogger(__name__)
-if six.PY2:
-    logger.addHandler(logging.NullHandler())
 
 
 TEMPLATES = {
     'minimal': [('{alias}.py', 'project_minimal.pyt'), ],
     'example': [('{alias}.py', 'project_example.pyt'), ],
     'testing': [('{alias}.py', 'project_testing.pyt'), ],
 }
 
 
 def init(alias=None, template=None, root=None, out=None):
     "Initialize a templated FlowProject module."
-    if not JINJA2:
-        raise ValueError("The init() function requires the 'jinja2' package.")
-
     if alias is None:
         alias = 'project'
-    elif not _is_identifier(alias):
+    elif not alias.isidentifier():
         raise ValueError(
             "The alias '{}' is not a valid Python identifier and therefore "
             "not be used as a FlowProject alias.".format(alias))
     if template is None:
         template = 'minimal'
     if out is None:
         out = sys.stderr
@@ -83,23 +63,16 @@
 
     # create files
     files_created = []
     for fn, code in codes.items():
         try:
             if root is not None:
                 fn = os.path.join(root, fn)
-            if six.PY2:
-                # Adapted from: http://stackoverflow.com/questions/10978869/
-                flags = os.O_CREAT | os.O_WRONLY | os.O_EXCL
-                fd = os.open(fn, flags)
-                with os.fdopen(fd, 'w') as file:
-                    file.write(code + '\n')
-            else:
-                with open(fn, 'x') as fw:
-                    fw.write(code + '\n')
+            with open(fn, 'x') as fw:
+                fw.write(code + '\n')
         except OSError as e:
             if e.errno == errno.EEXIST:
                 logger.error(
                     "Error while trying to initialize flow project with alias '{alias}', "
                     "a file named '{fn}' already exists!".format(alias=alias, fn=fn))
             else:
                 logger.error(
```

## flow/testing.py

```diff
@@ -1,22 +1,19 @@
 # Copyright (c) 2018 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
-"""Initialize a project for testing purposes
-
-"""
+"""Initialize a project for testing."""
 import signac
 
 from .template import init
 
 
 def make_project(alias='project', root=None, **kwargs):
-    """Initialize a project for testing purposes
+    """Initialize a project for testing.
 
     The initialized project has a few operations and a few jobs that are in
     various points in the workflow defined by the project.
-
     """
     init(alias=alias, root=root, template='testing')
     project = signac.init_project(name=alias, root=root)
     signac.testing.init_jobs(project, **kwargs)
     return project
```

## flow/environments/__init__.py

```diff
@@ -1,17 +1,19 @@
 # Copyright (c) 2017 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
-"""The environments module contains additional *opt-in* environment profiles.
+"""The environments module contains a set of provided environment profiles.
 
-Add the following line to your project modules, to use these profiles:
+These environments are imported by default. This can be disabled by setting
+the configuration key 'flow.import_packaged_environments' to 'off' with the
+following shell command:
 
-.. code-block:: python
+.. code-block:: bash
 
-    import flow.environments
+    signac config --global set flow.import_packaged_environments off
 
 """
 from . import incite
 from . import xsede
 from . import umich
 
 __all__ = [
```

## flow/environments/incite.py

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2018 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """Environments for INCITE supercomputers.
 
 http://www.doeleadershipcomputing.org/
 """
-from ..environment import DefaultLSFEnvironment, DefaultTorqueEnvironment
+from ..environment import DefaultLSFEnvironment
 
 from fractions import gcd
 
 
 class SummitEnvironment(DefaultLSFEnvironment):
     """Environment profile for the Summit supercomputer.
 
@@ -68,40 +68,21 @@
         cpus_per_set = tasks_per_set*cpus_per_task*np_per_task
 
         return nsets, tasks_per_set, cpus_per_set, gpus_per_set
 
     @staticmethod
     def jsrun_options(resource_set):
         nsets, tasks, cpus, gpus = resource_set
-        return '-n {} -a {} -c {} -g {}'.format(nsets, tasks, cpus, gpus)
+        cuda_aware_mpi = "--smpiargs='-gpu'" if (nsets > 0 or tasks > 0) and gpus > 0 else ""
+        return '-n {} -a {} -c {} -g {} {}'.format(nsets, tasks, cpus, gpus, cuda_aware_mpi)
 
     @staticmethod
     def jsrun_extra_args(operation):
         return str(operation.directives.get('extra_jsrun_args', ''))
 
     filters = {'calc_num_nodes': calc_num_nodes.__func__,
                'guess_resource_sets': guess_resource_sets.__func__,
                'jsrun_options': jsrun_options.__func__,
                'jsrun_extra_args': jsrun_extra_args.__func__}
 
 
-class TitanEnvironment(DefaultTorqueEnvironment):
-    """Environment profile for the titan super computer.
-
-    https://www.olcf.ornl.gov/titan/
-    """
-    hostname_pattern = 'titan'
-    template = 'titan.sh'
-    cores_per_node = 16
-
-
-class EosEnvironment(DefaultTorqueEnvironment):
-    """Environment profile for the eos super computer.
-
-    https://www.olcf.ornl.gov/computing-resources/eos/
-    """
-    hostname_pattern = 'eos'
-    template = 'eos.sh'
-    cores_per_node = 32
-
-
-__all__ = ['TitanEnvironment', 'EosEnvironment']
+__all__ = ['SummitEnvironment']
```

## flow/environments/xsede.py

```diff
@@ -1,12 +1,11 @@
 # Copyright (c) 2017 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """Environments for XSEDE supercomputers."""
-from __future__ import print_function
 import logging
 
 from ..environment import DefaultSlurmEnvironment
 
 
 logger = logging.getLogger(__name__)
```

## flow/scheduling/__init__.py

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) 2018 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """Defines the API for the scheduling system."""
 from .fakescheduler import FakeScheduler
-from .torque import TorqueScheduler
+from .lsf import LSFScheduler
 from .slurm import SlurmScheduler
+from .torque import TorqueScheduler
 
 
 __all__ = [
     'FakeScheduler',
-    'TorqueScheduler',
+    'LSFScheduler',
     'SlurmScheduler',
+    'TorqueScheduler',
     ]
```

## flow/scheduling/fakescheduler.py

```diff
@@ -2,15 +2,14 @@
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """Implementation of the scheduling system for a fake scheduler.
 
 The FakeScheduler class can be used in place of a real scheduler to test
 the cluster job submission workflow.
 """
-from __future__ import print_function
 import logging
 
 from .base import Scheduler
 
 logger = logging.getLogger(__name__)
```

## flow/scheduling/lsf.py

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2018 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """Implementation of the scheduling system for LSF schedulers.
 
 This module implements the Scheduler and ClusterJob classes for LSF.
 """
-from __future__ import print_function
 import getpass
 import subprocess
 import tempfile
 import json
 import logging
 import errno
```

## flow/scheduling/slurm.py

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2018 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """Implementation of the scheduling system for SLURM schedulers.
 
 This module implements the Scheduler and ClusterJob classes for SLURM.
 """
-from __future__ import print_function
 import getpass
 import subprocess
 import tempfile
 import logging
 import errno
 
 from .base import Scheduler
```

## flow/scheduling/torque.py

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2018 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """Implementation of the scheduling system for TORQUE schedulers.
 
 This module implements the Scheduler and ClusterJob classes for TORQUE.
 """
-from __future__ import print_function
 import io
 import errno
 import getpass
 import subprocess
 import tempfile
 import logging
 import xml.etree.ElementTree as ET
```

## flow/util/config.py

```diff
@@ -27,15 +27,15 @@
 
 def require_config_value(key, ns=None, default=_GET_CONFIG_VALUE_NONE):
     """Request a value from the user's configuration, fail if not available.
 
     :param key: The environment specific configuration key.
     :type key: str
     :param ns: The namespace in which to look for the key.
-    :type key: str
+    :type ns: str
     :param default: A default value in case the key cannot be found
         within the user's configuration.
     :return: The value or default value.
     :raises ConfigKeyError: If the key is not in the user's configuration
         and no default value is provided.
     """
     try:
@@ -53,19 +53,13 @@
 
 def get_config_value(key, ns=None, default=None):
     """Request a value from the user's configuration.
 
     :param key: The configuration key.
     :type key: str
     :param ns: The namespace in which to look for the key.
-    :type key: str
+    :type ns: str
     :param default: A default value in case the key cannot be found
         within the user's configuration.
     :return: The value if found, None if not found.
     """
-    try:
-        if ns is None:
-            return config.load_config()['flow'][key]
-        else:
-            return config.load_config()['flow'][ns][key]
-    except KeyError:
-        return default
+    return require_config_value(key=key, ns=ns, default=default)
```

## flow/util/misc.py

```diff
@@ -1,33 +1,17 @@
 # Copyright (c) 2018 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 import os
-import re
-import errno
 import json
 import argparse
 import logging
 from contextlib import contextmanager
 from itertools import cycle, islice
 
-from signac.common import six
-
-
-def _mkdir_p(path):
-    """"Create a directory at 'path', ignore if the directory already exists.
-
-    Needed, because the 'ignore_exists' is not available in Python 2.7.
-    """
-    try:
-        os.makedirs(path)
-    except OSError as error:
-        if not (error.errno == errno.EEXIST and os.path.isdir(path)):
-            raise
-
 
 def _positive_int(value):
     """Expect a command line argument to be a positive integer.
 
     Designed to be used in conjunction with an argparse.ArgumentParser.
 
     :param value:
@@ -58,15 +42,14 @@
     :type total:
         int
     :param width:
         The character width of the drawn progress bar.
     :type width:
         int
     """
-    "Helper function for the visualization of progress."
     assert value >= 0 and total > 0
     n = int(value / total * width)
     return '|' + ''.join(['#'] * n) + ''.join(['-'] * (width - n)) + '|'
 
 
 def write_human_readable_statepoint(script, job):
     """Human-readable representation of a signac state point."""
@@ -155,30 +138,14 @@
         try:
             os.chdir(root)
             yield
         finally:
             os.chdir(cwd)
 
 
-def _is_identifier(name):
-    """Check if 'name' is a valid Python identifier.
-
-    Source: https://stackoverflow.com/a/2545164
-    """
-    if name:
-        if six.PY2:
-            import re
-            import keyword
-            return re.match(r'^[a-z_][a-z0-9_]*$', name, re.I) and not keyword.iskeyword(name)
-        else:
-            return name.isidentifier()
-    else:
-        return False    # empty string or None
-
-
 class TrackGetItemDict(dict):
     "A dict that keeps track of which keys were accessed via __getitem__."
 
     def __init__(self, *args, **kwargs):
         self._keys_used = set()
         super(TrackGetItemDict, self).__init__(*args, **kwargs)
 
@@ -192,20 +159,14 @@
 
     @property
     def keys_used(self):
         "Return all keys that have been accessed."
         return self._keys_used.copy()
 
 
-# Remove this after we drop Python 2.7 support:
-def fullmatch(regex, string, flags=0):
-    """Emulate python-3.4 re.fullmatch()."""
-    return re.match("(?:" + regex + r")\Z", string, flags=flags)
-
-
 def roundrobin(*iterables):
     # From: https://docs.python.org/3/library/itertools.html#itertools-recipes
     # roundrobin('ABC', 'D', 'EF') --> A D E B F C
     # Recipe credited to George Sakkis
     num_active = len(iterables)
     nexts = cycle(iter(it).__next__ for it in iterables)
     while num_active:
```

## flow/util/progressbar.py

```diff
@@ -1,16 +1,18 @@
 # Copyright (c) 2018 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 "Simple progressbar formatting."
 import sys
 from deprecation import deprecated
 
+from .version import __version__
 
-@deprecated(deprecated_in="0.8", removed_in="1.0")
+
+@deprecated(deprecated_in="0.8", removed_in="0.10", current_version=__version__)
 def with_progressbar(iterable, total=None, width=120, desc='',
                      percentage=True, file=None):
     if file is None:
         file = sys.stderr
     if total is None:
         total = len(iterable)
     n = max(1, total // width)
```

## flow/util/template_filters.py

```diff
@@ -1,27 +1,26 @@
 # Copyright (c) 2018 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """Provide jinja2 template environment filter functions."""
-from __future__ import division, print_function
 import sys
 from math import ceil
 
 from .config import require_config_value
 from ..errors import ConfigKeyError
 from ..errors import SubmitError
 
 
 def identical(iterable):
-    """Check that all elements of an iterator are identical"""
+    """Check that all elements of an iterable are identical."""
     return len(set(iterable)) <= 1
 
 
 def format_timedelta(delta, style='HH:MM:SS'):
-    "Format a time delta for interpretation by schedulers."
+    """Format a time delta for interpretation by schedulers."""
     if isinstance(delta, int) or isinstance(delta, float):
         import datetime
         delta = datetime.timedelta(hours=delta)
     hours, r = divmod(delta.seconds, 3600)
     minutes, seconds = divmod(r, 60)
     hours += delta.days * 24
     if style == 'HH:MM:SS':
@@ -71,17 +70,16 @@
         Raises a RuntimeError if the required processing units across operations
         is not identical unless the allow_mixed parameter is set to True.
     """
     processing_units = [op.directives[name] *
                         op.directives.get('processor_fraction', 1) for op in operations]
     if identical(processing_units) or allow_mixed:
         if len(processing_units) > 0:
-            # need to cast int for python2
-            sum_processing_units = int(round(sum(processing_units)))
-            max_processing_units = int(round(max(processing_units)))
+            sum_processing_units = round(sum(processing_units))
+            max_processing_units = round(max(processing_units))
             return sum_processing_units if parallel else max_processing_units
         else:
             return 0    # empty set
     else:
         raise RuntimeError(
             "The number of required processing units ({}) differs between "
             "different operations.".format(name))
@@ -93,15 +91,15 @@
     This function raises a :class:`RuntimeError` if the calculated
     node utilization is below the given threshold or if the number
     of calculated required nodes is zero.
 
     :param nn:
         Number of requested nodes.
     :param np:
-        Number of required processing units (CPU/GPUs etc.).
+        Number of required processing units (e.g. CPUs, GPUs).
     :param ppn:
         Number of processing units available per node.
     :param threshold:
         The minimally required node utilization.
     :param name:
         A human-friendly name for the tested processing unit
         to be used in the error message, for example: CPU or GPU.
@@ -109,21 +107,22 @@
         The number of calculated nodes.
     :raises RuntimeError:
         Raised if the node utilization is below the given threshold.
     """
     if not (0 <= threshold <= 1.0):
         raise ValueError("The value for 'threshold' must be between 0 and 1.")
 
-    # Zero nodes are just returned and possible utilization or validiation checks
-    # must be performed elswhere.
+    # Zero nodes are just returned and possible utilization or validation checks
+    # must be performed elsewhere.
     if nn == 0:
         return 0
 
-    # The utilization is the number of processing units (np) required divided by the
-    # number of nodes (nn) multiplied with the number of processing units per node (ppn).
+    # The utilization is the number of processing units (np) required divided
+    # by the product of the number of nodes (nn) and the number of processing
+    # units per node (ppn).
     utilization = np / (nn * ppn)
 
     # Raise RuntimeError if the utilization is below the specified threshold.
     if utilization < threshold:
         raise RuntimeError(
             "Low{name} utilization warning: {util:.0%}\n"
             "Total resources requested would require {nn} node(s), "
@@ -137,15 +136,15 @@
     return nn
 
 
 def calc_num_nodes(np, ppn=1, threshold=0, name=None):
     """Calculate the number of required nodes with optional utilization check.
 
     :param np:
-        Number of required processing units (CPU/GPU etc.).
+        Number of required processing units (e.g. CPUs, GPUs).
     :param ppn:
         Number of processing units available per node.
     :param threshold:
         (optional) The required node utilization.
         The default is 0, which means no check.
     :param name:
         (optional) A human-friendly name for the tested processing unit
@@ -157,15 +156,15 @@
         If the calculated node utilization is below the given threshold.
     """
     nn = int(ceil(np / ppn))
     return check_utilization(nn, np, ppn, threshold, name)
 
 
 def print_warning(msg):
-    """Print warning message within jinja2 template
+    """Print warning message within jinja2 template.
 
     :param:
         The warning message as a string
     """
     import logging
     logger = logging.getLogger(__name__)
     logger.warn(msg)
@@ -174,15 +173,15 @@
 
 _GET_ACCOUNT_NAME_MESSAGES_SHOWN = set()
 
 
 def get_account_name(environment, required=False):
     """Get account name for environment with user-friendly messages on failure.
 
-    :param:
+    :param environment:
         The environment for which to obtain the account variable.
     :param required:
         Specify whether the account name is required instead of optional.
     :returns:
         The account name for the given environment or None if missing and not required.
     :raises SubmitError:
         Raised if 'required' is True and the account name is missing.
```

## flow/util/translate.py

```diff
@@ -1,23 +1,23 @@
 # Copyright (c) 2018 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 "Helper functions to keep track of abbreviations meant for output on screen."
 
 
 def abbreviate(x, a):
-    "Abbreviate x with a and add to the abbreviation table."
+    """Abbreviate x with a and add to the abbreviation table."""
     if x == a:
         return x
     else:
         abbreviate.table[a] = x
         return a
 
 abbreviate.table = dict()  # noqa
 
 
 def shorten(x, max_length=None):
-    "Shorten x to max_length and add to abbreviation table."
+    """Shorten x to max_length and add to abbreviation table."""
     if max_length is None:
         return x
     else:
         return abbreviate(x, x[:max_length])
```

## Comparing `signac_flow-0.8.0.data/scripts/simple-scheduler` & `signac_flow-0.9.0.data/scripts/simple-scheduler`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     for line in script.readlines():
         if line.startswith('#SSCHED'):
             for token in line[8:].split():
                 yield token
 
 
 def main_submit(args):
-    # Try to parse args, should raise error if anytyhing is wrong or missing
+    # Try to parse args, should raise error if anything is wrong or missing
     with open(args.filename) as script:
         _get_submit_parser().parse_args(list(_get_args(script)))
     dst = os.path.join(args.inbox, str(uuid.uuid4()) + '.sh')
     shutil.copyfile(args.filename, dst)
 
 
 @contextmanager
@@ -138,15 +138,15 @@
             assert 0
 
         cmd = '/bin/bash ' + doc['script']
 
         with open(fn_out, 'w') as outfile:
             with open(fn_err, 'w') as errfile:
                 check_call(cmd, shell=True, stdout=outfile, stderr=errfile)
-    except CalledProcessError as error:
+    except CalledProcessError:
         logger.warning("Error while executing job '{}'.".format(doc['_id']))
     finally:
         os.chdir(cwd)
         os.remove(doc['script'])
         doc['status'] = int(JobStatus.inactive)
         doc['_delete_after'] = time.time() + 2 * 60     # remove after 2 mins
         db[doc['_id']] = doc
@@ -219,19 +219,19 @@
         'status',
         description="Display the status of jobs submitted to the scheduler.")
     parser_status.add_argument('--json', action='store_true')
     parser_status.set_defaults(func=main_status)
 
     parser_run = subparsers.add_parser(
         'run',
-        description="Execute jobs subitted to the schduler.")
+        description="Execute jobs submitted to the scheduler.")
     parser.add_argument(
         '--polling-period',
         default=10,
-        help="Check the database for new entryies every given seconds.")
+        help="Check the database for new entries every given seconds.")
     parser_run.set_defaults(func=main_run)
 
     args = parser.parse_args()
     if not hasattr(args, 'func'):
         parser.print_usage()
         sys.exit(2)
```

## Comparing `signac_flow-0.8.0.dist-info/LICENSE.txt` & `signac_flow-0.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `signac_flow-0.8.0.dist-info/METADATA` & `signac_flow-0.9.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: signac-flow
-Version: 0.8.0
+Version: 0.9.0
 Summary: Simple workflow management for signac projects.
 Home-page: https://signac.io
-Author: Carl Simon Adorf
+Author: Carl Simon Adorf et al.
 Author-email: csadorf@umich.edu
+Maintainer: signac Developers
+Maintainer-email: signac-support@umich.edu
 License: UNKNOWN
+Download-URL: https://pypi.org/project/signac-flow/
 Keywords: workflow management signac framework database
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, <4
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.5, <4
 Description-Content-Type: text/markdown
 Requires-Dist: signac (>=1.0.0)
 Requires-Dist: jinja2 (>=2.8)
 Requires-Dist: cloudpickle
 Requires-Dist: deprecation (>=2)
-Requires-Dist: enum34 ; python_version < "3.4"
 
-# <img src="https://raw.githubusercontent.com/glotzerlab/signac-flow/master/doc/images/logo.png" width="75" height="75"> signac-flow - manage workflows with signac
+# <img src="https://raw.githubusercontent.com/glotzerlab/signac-flow/master/doc/images/palette-header.png" width="75" height="58"> signac-flow - manage workflows with signac
 
 [![Affiliated with NumFOCUS](https://img.shields.io/badge/NumFOCUS-affiliated%20project-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org/sponsored-projects/affiliated-projects)
 [![PyPI](https://img.shields.io/pypi/v/signac-flow.svg)](https://pypi.org/project/signac-flow/)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/signac-flow.svg?style=flat)](https://anaconda.org/conda-forge/signac-flow)
 ![CircleCI](https://img.shields.io/circleci/project/github/glotzerlab/signac-flow/master.svg)
 [![RTD](https://img.shields.io/readthedocs/signac.svg?style=flat)](https://docs.signac.io)
 [![License](https://img.shields.io/github/license/glotzerlab/signac-flow.svg)](https://github.com/glotzerlab/signac-flow/blob/master/LICENSE.txt)
@@ -52,15 +54,15 @@
 - [**signac** website](https://signac.io/):
   Framework overview and news.
 
 
 ## Installation
 
 The recommended installation method for **signac-flow** is through **conda** or **pip**.
-The software is tested for Python versions 2.7 and 3.5+ and is built for all major platforms.
+The software is tested for Python versions 3.5+ and is built for all major platforms.
 
 To install **signac-flow** *via* the [conda-forge](https://conda-forge.github.io/) channel, execute:
 
 ```bash
 conda install -c conda-forge signac-flow
 ```
```

## Comparing `signac_flow-0.8.0.dist-info/RECORD` & `signac_flow-0.9.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,67 @@
-flow/__init__.py,sha256=ChyuALK5yH5r8dJE9q4F3QQV0IaG3pGKvEUIO6SPKTQ,1439
-flow/__main__.py,sha256=Pt-WeOSEezzaHuxt8zmI5dwmkiJFlNIJQdbya0JNjNY,3733
-flow/environment.py,sha256=tJEmu3nQsdgfHks3LWrtfLqKF7KMAwX28PTE7gtAK50,14203
-flow/errors.py,sha256=pHABw80KowPi3GZ4luqa0EKf-KtS7pU_xgn1QluOe4c,1314
-flow/labels.py,sha256=7XZArf9lu05eCnkzFj7KMjb8G3eDn2jyculYhUGRLL0,1411
-flow/legacy.py,sha256=dNvw0RCuiYHace0IO1orXb6cNfK42sCa40cyeLNG2pk,1023
-flow/legacy_templating.py,sha256=bLPPPoWIKb16tfzeiM1_FV2KtQuJ8ISJBAfUTgvqypM,11301
-flow/operations.py,sha256=yMwM-yeyBUN6nsarhCkrGi_5e3lXlLYVW46Sqhqax7I,8087
-flow/project.py,sha256=q0Wkbw1Ia8BCKMfBjt_aI9XGHGg2R3EIigCZ5EJZqOA,119281
-flow/template.py,sha256=r4faA42MxBdkLMntLB2v_Lmu0_KVaWPQZRo1txYZ9xE,3642
-flow/testing.py,sha256=lUrQUstO_jxVgU7mLyw8dINp-sB6qJuxkBGFsEa4a9E,667
-flow/environments/__init__.py,sha256=p16bWLfScEzVnXT9_YmtYGcogb4pwBTwO3f5W3JMKB0,475
-flow/environments/incite.py,sha256=8OAf1TXhChkVLErjF_a0PwcjE7wp-xorqZ_YY8ui_h0,3607
+flow/__init__.py,sha256=tHkfn4M1DetvJjpvZQ-aEC6JSn9eZ2IkPZ6RTiPnXKc,1408
+flow/__main__.py,sha256=2UCn0vTCFuQ2VyaL360MoilslWBtblwt-wZme3RZYeA,3558
+flow/environment.py,sha256=TZgQdp_hlrU0gqqDI54eT3s2_daErop6DobBjQYxEB8,13479
+flow/errors.py,sha256=yziJOd250phKFQWIBigpjvKomHsdDf6AgjRmM8vbgKo,1314
+flow/labels.py,sha256=sG8v0aMgYGJ5u1rO4C4Wb-Xk9XEbMFAykoG4tNQ-nBw,1411
+flow/operations.py,sha256=Wds6hVyroj4yWzta3Vq7OgKq80esvAh4d1E7a6cglJg,7869
+flow/project.py,sha256=-9atQPuJ_mbuIOMZ0W-LiZWYMgGY9sr20IE4a5p-GKU,125434
+flow/template.py,sha256=6OHbrgRnoJRoKGGMfRJCeWLxvTKWyQx2vA9KfMhG484,2809
+flow/testing.py,sha256=2k5VGFUQmjzeMqashbAX5Tf9pAvB29-1sF1Nyu5gWDw,648
+flow/version.py,sha256=J9h7nWDTlkvvfc79an8uazEv5TT_33ou1NhjAnCoXsQ,196
+flow/environments/__init__.py,sha256=66w-ZRhEdHEgO2wGFQ-yKczjtlF7rF7mf5sqy3R7nZU,617
+flow/environments/incite.py,sha256=rCva9gZAiUYsfeFBvuATUFmED5E-42Z3Laazm7lN8pI,3195
 flow/environments/umich.py,sha256=oWssrbrAiDq1EUQnd3Ai0J6d0zBC0P48l_b-eG9Xgy8,1077
-flow/environments/xsede.py,sha256=AE3OZe0MsWwQzrWarIK3lwv3GKhFdEmB8Jhq3JiHouY,2880
-flow/scheduling/__init__.py,sha256=hLtykOa1AbMdoCjiqjIK1-pAY3RLyUcTjk-bwvXnzqs,392
+flow/environments/xsede.py,sha256=J_NvX6keDWQ_pd7BPGMszyPqnonG1rSH46dIaT6p62s,2842
+flow/scheduling/__init__.py,sha256=ztMX9IEoib5Gi9L_cA3wCo5GUnWcEs-CnXbuWh-ZjDY,442
 flow/scheduling/base.py,sha256=iFPj0ub3RGe-vzmPdG0r7QjsaL96LKGCsNxN6LHVMe4,1994
-flow/scheduling/fakescheduler.py,sha256=726_9ePtBmW5RQuhIurhEGKIZWjTY_lMiYH4jvQzSlY,997
-flow/scheduling/lsf.py,sha256=jjxe_W21lmDVf2JgOoSj3O8HI-roVpBx_eGRd_hnBDE,4662
+flow/scheduling/fakescheduler.py,sha256=bAd90rmWDZrSCczv1xUGZHld3yLAfJ7z9qFAG7ARB4o,959
+flow/scheduling/lsf.py,sha256=-poZJNyOA6fwdGtsNef1vDCSa3wVaKuQbN5pyZ5ZhnA,4624
 flow/scheduling/simple_scheduler.py,sha256=fMoGSy7sKecRjzteJOIKfgpvKeJw8sDIGDrR7Nlg96c,1258
-flow/scheduling/slurm.py,sha256=HAIqrr2Pa7RJlE46ibXaHAav7i_YENWXD18akqNABV0,4806
+flow/scheduling/slurm.py,sha256=l3ADAXbV9D8fE26yIzokQgl4nG4mtVAqjtnvG1CNIrQ,4768
 flow/scheduling/status.py,sha256=zxIsGkyHcOd_XeTSk2ZWochQuxm7H9_msMXv-cJzOZQ,1514
-flow/scheduling/torque.py,sha256=o1QwdRZJZ3gtlcViOceHZdg5s0r1D5AA91KGuxV0ZLs,5522
+flow/scheduling/torque.py,sha256=Ar6wEZfNHOBUcR8pvH1S7iWZhNYWuEzftH5yTbAD77E,5484
 flow/templates/base_script.sh,sha256=SRFi8-uv6B5ME_4u-xSyaKzPJv2LEp9GCRGl83GgRtc,979
 flow/templates/base_status.jinja,sha256=NVKiqZqaIwn-PB6DFf6hJ2esCSbtMozi-Gkb5ElOfTI,2926
 flow/templates/base_status_compact.jinja,sha256=GYoK_zCC1GGW25s4Wp-YP_RAmVp0emvKHF9EoIIT28Y,1857
 flow/templates/base_status_expand.jinja,sha256=wjM35iTcZPUKDbW_Ds49LCgqM5DZDlMpZirH7bw3eCk,1116
 flow/templates/base_status_stack.jinja,sha256=8CKCQio8Nr2qmIOSw58yK_qZ2gbmaO0v59NARQGxRBA,814
 flow/templates/bridges.sh,sha256=VJW6R9E1SbxiIzpS6nP0L-E7bRvr4ZJoDE7ou6uUIPE,1902
 flow/templates/comet.sh,sha256=TcgvtOlwzoupHmTEY5HFOLFEZrl6MWXBgD-SWwERUEE,1671
-flow/templates/eos.sh,sha256=51IP2qPrD5kK55od6xdQVzESV6H3F5LEQ0uoxGnWcN8,752
 flow/templates/lsf.sh,sha256=3eDQF6xzcRsvQfVg-Um41wCIzbh-dm15CsxJOhyjJHc,389
 flow/templates/project_example.pyt,sha256=hmL8uD2IPIWXd8q10aPjoO8hRAx7EdNYgbOJ8-ZslaI,412
 flow/templates/project_minimal.pyt,sha256=udhwEOqGI6xtOiH1dIany4VNS8_3S9nQixo8G5kBU80,152
 flow/templates/project_testing.pyt,sha256=Jd-djNq-R6CGOVdRwax9XQJgO8WKvRwZnfiLlfpO3_o,1235
 flow/templates/script.sh,sha256=QQxCqDUbo3_yfXdZaUI9uU6cZ0c3IJvQyEywSHj4j7E,26
 flow/templates/simple_scheduler.sh,sha256=Andn4I783ABVFePZV1beq-2GVJcvniuup96w4cCEwwI,218
 flow/templates/slurm.sh,sha256=Qp3VQGV1nOa1Mfk1MpPEc94EjX-HX0DcIpfSb8JcGhg,447
 flow/templates/stampede2.sh,sha256=TH37ct9HTEU1IPuQP3VwBHNzjXoNOHkWF5DoGEqzYVw,2737
 flow/templates/status.jinja,sha256=fCbcVVcls_PbdYQ5socAjWMparZgz2v2Ri43dd5Tmk0,34
 flow/templates/status_compact.jinja,sha256=XuJjDc0brddbVKMK2y5A4hBDZUprH626UTYTq5DHM38,42
 flow/templates/status_expand.jinja,sha256=NDLv_APnTFYZQO4EJEn2t2Fdfwca-a30f4fLlJF19CU,41
 flow/templates/status_stack.jinja,sha256=KlHugMVnneLs3XHc8WshnrfCAPKMcei95x7UzKpQzrI,40
 flow/templates/summit.sh,sha256=1G_NEW5p9S7jmk5Bn8XWz2jO1rWNL5M8y2u4PIsCEbA,1224
-flow/templates/titan.sh,sha256=e83pCNWyE858ID9q6ZgGODq-scKPhCH-xW32MfU163M,770
 flow/templates/torque.sh,sha256=-MdPwbCiRWzYc0D4iM4y9Qf2ygSDbLrU8XFwrdCt0ZI,801
 flow/templates/umich-flux.sh,sha256=70G8ATTVu10iRPeskahbhNmxv1dZzgLRbEwQ4D_dPW4,1226
 flow/util/__init__.py,sha256=HPHqVUBJqCtnFQR9SWbcabqEAsCKgI29AuTvz6gcDhM,305
-flow/util/config.py,sha256=1fTFS-SYvHybCKy0GiUpoiNEFaxu4OPw-KrDMwPejtQ,2249
-flow/util/execution.py,sha256=I6Nxw1Tn-SDveT9CRfnO3nQPMfz3-WiG1YGtc74Yt0I,792
-flow/util/misc.py,sha256=H7iPOkNLUh1xvrlDiiiGfDFTtSpn6E9469Pt_ru0KMU,6936
-flow/util/progressbar.py,sha256=aTA0yMI4TKl1mZAshE67Esh02V14JKZEoGy9XNBk_eA,1088
-flow/util/template_filters.py,sha256=I9BeCsvupW_oAjm8yIN3dUTpVM-W3If5bhYsACEOvV8,8110
-flow/util/translate.py,sha256=KUTtInrE5jCzOTPTsz9hmc3JBbsz0m3gU2VXWZDSmwY,630
+flow/util/config.py,sha256=tR2O5BalSUrbYz7RQ2h4rkMvuDJT1nQJNaXf3aYG0jg,2112
+flow/util/misc.py,sha256=uEGiaInui6kbKQihiUNfOlUI9-I6TvhHiYa8uJR8m8w,5868
+flow/util/progressbar.py,sha256=1S_FrnwqB_QDis-eg23h4JEFcB_dEPzFIQ2HFlmasDQ,1152
+flow/util/template_filters.py,sha256=KQthpKasuhiEilw7WAGmW4K9DY7vJceb_shJ3ybZ37I,8041
+flow/util/translate.py,sha256=8aanjSdR-1l1SOvf2SDTPiRJ1xSTGz289P6OsAzPRTQ,638
 flow/util/tqdm/__init__.py,sha256=27Cfpptq2y44-g0wg9PQXwIUImNUyjF1f9CSXJb2P7c,1000
 flow/util/tqdm/__main__.py,sha256=JPNIwI-Qb_VQERows-n4R2XzcY8rGCt5FR8kUiKD1J4,31
 flow/util/tqdm/_main.py,sha256=PKOF_OBlPfh9CdqlRKYVNvKzZxJUQte2KnRXWfXOn3A,4933
 flow/util/tqdm/_tqdm.py,sha256=EVV6oQX5r1Lyq3wSQOxiiM9G7ZY3q9iTPyqcZqr5exc,41319
 flow/util/tqdm/_tqdm_gui.py,sha256=yEa6K6weD-Xqankn58KUMhH7UyRnf5Tr7QUkPAIWREw,13461
 flow/util/tqdm/_tqdm_notebook.py,sha256=hqcB50c2CtrIE1YWg-H1osgKBcFUmIzWFrOiaklUgWc,8282
 flow/util/tqdm/_tqdm_pandas.py,sha256=4RjSpzbHLgfuRLJQPbDf9_LT-f_0db2gaAB6nOJ4dYA,1608
 flow/util/tqdm/_utils.py,sha256=JNa0QZIZIcgGmUXIDKbSdoFqQZTTQuB7785Y8PleePo,3436
 flow/util/tqdm/_version.py,sha256=8D0Qc3n-T7u5YrWoes49oe_D3rezR_Rded0ZOJedc_A,925
-signac_flow-0.8.0.data/scripts/simple-scheduler,sha256=QeyxDKVajcBEZsCJKlod8bMyEbMUziVlmm_IJ2FKXuk,7523
-signac_flow-0.8.0.dist-info/LICENSE.txt,sha256=m3oc8WW0Nh_WDJPO8LtuPOEfj2XdloUE69ggSw_LXu8,1587
-signac_flow-0.8.0.dist-info/METADATA,sha256=mqa95Z-WP3L6jB4CGAp36NLb_iBDiIC528XCo8o6Ao0,4158
-signac_flow-0.8.0.dist-info/WHEEL,sha256=8zNYZbwQSXoB9IfXOjPfeNwvAsALAjffgk27FqvCWbo,110
-signac_flow-0.8.0.dist-info/entry_points.txt,sha256=5cu19ZN7yBI8Q9TrLrW-ZfUixQ0G31rseKJjU69Y2u4,45
-signac_flow-0.8.0.dist-info/top_level.txt,sha256=mZX7nA6le1XNJV9ujgVL0yyesYwj3fMwHSm3zGwjNbU,5
-signac_flow-0.8.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-signac_flow-0.8.0.dist-info/RECORD,,
+signac_flow-0.9.0.data/scripts/simple-scheduler,sha256=bxDwBnFpiaePpE7hFrCfz3My6rPeSCi2vBiy6z-5NgM,7514
+signac_flow-0.9.0.dist-info/LICENSE.txt,sha256=m3oc8WW0Nh_WDJPO8LtuPOEfj2XdloUE69ggSw_LXu8,1587
+signac_flow-0.9.0.dist-info/METADATA,sha256=SpDUSQdFiVyOl11jV3iF6hMjYw58ZOxkx7nlwzKnfk4,4218
+signac_flow-0.9.0.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
+signac_flow-0.9.0.dist-info/entry_points.txt,sha256=5cu19ZN7yBI8Q9TrLrW-ZfUixQ0G31rseKJjU69Y2u4,45
+signac_flow-0.9.0.dist-info/top_level.txt,sha256=mZX7nA6le1XNJV9ujgVL0yyesYwj3fMwHSm3zGwjNbU,5
+signac_flow-0.9.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+signac_flow-0.9.0.dist-info/RECORD,,
```

