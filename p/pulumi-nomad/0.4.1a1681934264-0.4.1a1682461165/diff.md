# Comparing `tmp/pulumi_nomad-0.4.1a1681934264.tar.gz` & `tmp/pulumi_nomad-0.4.1a1682461165.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_nomad-0.4.1a1681934264.tar", last modified: Wed Apr 19 20:06:21 2023, max compression
+gzip compressed data, was "pulumi_nomad-0.4.1a1682461165.tar", last modified: Tue Apr 25 22:23:27 2023, max compression
```

## Comparing `pulumi_nomad-0.4.1a1681934264.tar` & `pulumi_nomad-0.4.1a1682461165.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:06:21.270956 pulumi_nomad-0.4.1a1681934264/
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-19 20:06:21.270956 pulumi_nomad-0.4.1a1681934264/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:06:21.270956 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33737 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/acl_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    27631 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/acl_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:06:21.270956 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    52267 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/external_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_acl_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_acl_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_acl_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_acl_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_acl_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_job_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_scaling_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_scaling_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_scheduler_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)    40679 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    50484 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20563 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/quote_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/scheduler_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/sentinel_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    56839 2023-04-19 20:06:20.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:06:21.270956 pulumi_nomad-0.4.1a1681934264/pulumi_nomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-19 20:06:21.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-19 20:06:21.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:06:21.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:06:21.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 20:06:21.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 20:06:21.000000 pulumi_nomad-0.4.1a1681934264/pulumi_nomad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:06:21.270956 pulumi_nomad-0.4.1a1681934264/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-19 20:06:21.000000 pulumi_nomad-0.4.1a1681934264/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:23:27.787228 pulumi_nomad-0.4.1a1682461165/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-25 22:23:27.783228 pulumi_nomad-0.4.1a1682461165/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:23:27.783228 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/acl_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/acl_binding_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27631 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/acl_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:23:27.783228 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52267 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/external_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_acl_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_acl_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_acl_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_acl_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_job_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_scaling_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_scaling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_scheduler_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40679 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55024 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20563 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/quote_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/scheduler_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/sentinel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56839 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:23:27.783228 pulumi_nomad-0.4.1a1682461165/pulumi_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/pulumi_nomad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 22:23:27.787228 pulumi_nomad-0.4.1a1682461165/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-25 22:23:27.000000 pulumi_nomad-0.4.1a1682461165/setup.py
```

### Comparing `pulumi_nomad-0.4.1a1681934264/PKG-INFO` & `pulumi_nomad-0.4.1a1682461165/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_nomad
-Version: 0.4.1a1681934264
+Version: 0.4.1a1682461165
 Summary: A Pulumi package for creating and managing nomad cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
 Keywords: pulumi nomad
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-nomad/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-nomad/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fnomad.svg)](https://www.npmjs.com/package/@pulumi/nomad)
 [![Python version](https://badge.fury.io/py/pulumi-nomad.svg)](https://pypi.org/project/pulumi-nomad)
 [![NuGet version](https://badge.fury.io/nu/pulumi.nomad.svg)](https://badge.fury.io/nu/pulumi.nomad)
```

### Comparing `pulumi_nomad-0.4.1a1681934264/README.md` & `pulumi_nomad-0.4.1a1682461165/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/__init__.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
+from .acl_auth_method import *
+from .acl_binding_rule import *
 from .acl_policy import *
 from .acl_role import *
 from .acl_token import *
 from .external_volume import *
 from .get_acl_policies import *
 from .get_acl_policy import *
 from .get_acl_role import *
@@ -46,14 +48,30 @@
     config = _utilities.lazy_import('pulumi_nomad.config')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "nomad",
+  "mod": "index/aclAuthMethod",
+  "fqn": "pulumi_nomad",
+  "classes": {
+   "nomad:index/aclAuthMethod:AclAuthMethod": "AclAuthMethod"
+  }
+ },
+ {
+  "pkg": "nomad",
+  "mod": "index/aclBindingRule",
+  "fqn": "pulumi_nomad",
+  "classes": {
+   "nomad:index/aclBindingRule:AclBindingRule": "AclBindingRule"
+  }
+ },
+ {
+  "pkg": "nomad",
   "mod": "index/aclPolicy",
   "fqn": "pulumi_nomad",
   "classes": {
    "nomad:index/aclPolicy:AclPolicy": "AclPolicy"
   }
  },
  {
```

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/_inputs.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/_inputs.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
+    'AclAuthMethodConfigArgs',
     'AclRolePolicyArgs',
     'AclTokenRoleArgs',
     'ExternalVolumeCapabilityArgs',
     'ExternalVolumeMountOptionsArgs',
     'ExternalVolumeTopologyArgs',
     'ExternalVolumeTopologyRequestArgs',
     'ExternalVolumeTopologyRequestPreferredArgs',
@@ -34,14 +35,135 @@
     'VolumeTopologyArgs',
     'VolumeTopologyRequestArgs',
     'VolumeTopologyRequestRequiredArgs',
     'VolumeTopologyRequestRequiredTopologyArgs',
 ]
 
 @pulumi.input_type
+class AclAuthMethodConfigArgs:
+    def __init__(__self__, *,
+                 allowed_redirect_uris: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 oidc_client_id: pulumi.Input[str],
+                 oidc_client_secret: pulumi.Input[str],
+                 oidc_discovery_url: pulumi.Input[str],
+                 bound_audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 claim_mappings: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 discovery_ca_pems: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 list_claim_mappings: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 oidc_scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 signing_algs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        pulumi.set(__self__, "allowed_redirect_uris", allowed_redirect_uris)
+        pulumi.set(__self__, "oidc_client_id", oidc_client_id)
+        pulumi.set(__self__, "oidc_client_secret", oidc_client_secret)
+        pulumi.set(__self__, "oidc_discovery_url", oidc_discovery_url)
+        if bound_audiences is not None:
+            pulumi.set(__self__, "bound_audiences", bound_audiences)
+        if claim_mappings is not None:
+            pulumi.set(__self__, "claim_mappings", claim_mappings)
+        if discovery_ca_pems is not None:
+            pulumi.set(__self__, "discovery_ca_pems", discovery_ca_pems)
+        if list_claim_mappings is not None:
+            pulumi.set(__self__, "list_claim_mappings", list_claim_mappings)
+        if oidc_scopes is not None:
+            pulumi.set(__self__, "oidc_scopes", oidc_scopes)
+        if signing_algs is not None:
+            pulumi.set(__self__, "signing_algs", signing_algs)
+
+    @property
+    @pulumi.getter(name="allowedRedirectUris")
+    def allowed_redirect_uris(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        return pulumi.get(self, "allowed_redirect_uris")
+
+    @allowed_redirect_uris.setter
+    def allowed_redirect_uris(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "allowed_redirect_uris", value)
+
+    @property
+    @pulumi.getter(name="oidcClientId")
+    def oidc_client_id(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "oidc_client_id")
+
+    @oidc_client_id.setter
+    def oidc_client_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "oidc_client_id", value)
+
+    @property
+    @pulumi.getter(name="oidcClientSecret")
+    def oidc_client_secret(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "oidc_client_secret")
+
+    @oidc_client_secret.setter
+    def oidc_client_secret(self, value: pulumi.Input[str]):
+        pulumi.set(self, "oidc_client_secret", value)
+
+    @property
+    @pulumi.getter(name="oidcDiscoveryUrl")
+    def oidc_discovery_url(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "oidc_discovery_url")
+
+    @oidc_discovery_url.setter
+    def oidc_discovery_url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "oidc_discovery_url", value)
+
+    @property
+    @pulumi.getter(name="boundAudiences")
+    def bound_audiences(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "bound_audiences")
+
+    @bound_audiences.setter
+    def bound_audiences(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "bound_audiences", value)
+
+    @property
+    @pulumi.getter(name="claimMappings")
+    def claim_mappings(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        return pulumi.get(self, "claim_mappings")
+
+    @claim_mappings.setter
+    def claim_mappings(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "claim_mappings", value)
+
+    @property
+    @pulumi.getter(name="discoveryCaPems")
+    def discovery_ca_pems(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "discovery_ca_pems")
+
+    @discovery_ca_pems.setter
+    def discovery_ca_pems(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "discovery_ca_pems", value)
+
+    @property
+    @pulumi.getter(name="listClaimMappings")
+    def list_claim_mappings(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        return pulumi.get(self, "list_claim_mappings")
+
+    @list_claim_mappings.setter
+    def list_claim_mappings(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "list_claim_mappings", value)
+
+    @property
+    @pulumi.getter(name="oidcScopes")
+    def oidc_scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "oidc_scopes")
+
+    @oidc_scopes.setter
+    def oidc_scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "oidc_scopes", value)
+
+    @property
+    @pulumi.getter(name="signingAlgs")
+    def signing_algs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "signing_algs")
+
+    @signing_algs.setter
+    def signing_algs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "signing_algs", value)
+
+
+@pulumi.input_type
 class AclRolePolicyArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str]):
         """
         :param pulumi.Input[str] name: `(string: <required>)` - A human-friendly name for this ACL Role.
         """
         pulumi.set(__self__, "name", name)
```

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/_utilities.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/acl_policy.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/acl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/acl_role.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/acl_token.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/acl_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/config/outputs.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/config/vars.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/external_volume.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/external_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_acl_policies.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_acl_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_acl_policy.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_acl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_acl_role.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_acl_roles.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_acl_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_acl_token.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_acl_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_acl_tokens.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_acl_tokens.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_datacenters.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_deployments.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_deployments.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_job.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_job_parser.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_job_parser.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_namespace.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_namespaces.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_namespaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_plugin.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_plugins.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_plugins.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_regions.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_scaling_policies.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_scaling_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_scaling_policy.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_scaling_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_scheduler_policy.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_scheduler_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/get_volumes.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/get_volumes.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/job.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/namespace.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/outputs.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
+    'AclAuthMethodConfig',
     'AclRolePolicy',
     'AclTokenRole',
     'ExternalVolumeCapability',
     'ExternalVolumeMountOptions',
     'ExternalVolumeTopology',
     'ExternalVolumeTopologyRequest',
     'ExternalVolumeTopologyRequestPreferred',
@@ -50,14 +51,130 @@
     'GetJobTaskGroupVolumeResult',
     'GetNamespaceCapabilityResult',
     'GetPluginNodeResult',
     'GetScalingPoliciesPolicyResult',
 ]
 
 @pulumi.output_type
+class AclAuthMethodConfig(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "allowedRedirectUris":
+            suggest = "allowed_redirect_uris"
+        elif key == "oidcClientId":
+            suggest = "oidc_client_id"
+        elif key == "oidcClientSecret":
+            suggest = "oidc_client_secret"
+        elif key == "oidcDiscoveryUrl":
+            suggest = "oidc_discovery_url"
+        elif key == "boundAudiences":
+            suggest = "bound_audiences"
+        elif key == "claimMappings":
+            suggest = "claim_mappings"
+        elif key == "discoveryCaPems":
+            suggest = "discovery_ca_pems"
+        elif key == "listClaimMappings":
+            suggest = "list_claim_mappings"
+        elif key == "oidcScopes":
+            suggest = "oidc_scopes"
+        elif key == "signingAlgs":
+            suggest = "signing_algs"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in AclAuthMethodConfig. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        AclAuthMethodConfig.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        AclAuthMethodConfig.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 allowed_redirect_uris: Sequence[str],
+                 oidc_client_id: str,
+                 oidc_client_secret: str,
+                 oidc_discovery_url: str,
+                 bound_audiences: Optional[Sequence[str]] = None,
+                 claim_mappings: Optional[Mapping[str, str]] = None,
+                 discovery_ca_pems: Optional[Sequence[str]] = None,
+                 list_claim_mappings: Optional[Mapping[str, str]] = None,
+                 oidc_scopes: Optional[Sequence[str]] = None,
+                 signing_algs: Optional[Sequence[str]] = None):
+        pulumi.set(__self__, "allowed_redirect_uris", allowed_redirect_uris)
+        pulumi.set(__self__, "oidc_client_id", oidc_client_id)
+        pulumi.set(__self__, "oidc_client_secret", oidc_client_secret)
+        pulumi.set(__self__, "oidc_discovery_url", oidc_discovery_url)
+        if bound_audiences is not None:
+            pulumi.set(__self__, "bound_audiences", bound_audiences)
+        if claim_mappings is not None:
+            pulumi.set(__self__, "claim_mappings", claim_mappings)
+        if discovery_ca_pems is not None:
+            pulumi.set(__self__, "discovery_ca_pems", discovery_ca_pems)
+        if list_claim_mappings is not None:
+            pulumi.set(__self__, "list_claim_mappings", list_claim_mappings)
+        if oidc_scopes is not None:
+            pulumi.set(__self__, "oidc_scopes", oidc_scopes)
+        if signing_algs is not None:
+            pulumi.set(__self__, "signing_algs", signing_algs)
+
+    @property
+    @pulumi.getter(name="allowedRedirectUris")
+    def allowed_redirect_uris(self) -> Sequence[str]:
+        return pulumi.get(self, "allowed_redirect_uris")
+
+    @property
+    @pulumi.getter(name="oidcClientId")
+    def oidc_client_id(self) -> str:
+        return pulumi.get(self, "oidc_client_id")
+
+    @property
+    @pulumi.getter(name="oidcClientSecret")
+    def oidc_client_secret(self) -> str:
+        return pulumi.get(self, "oidc_client_secret")
+
+    @property
+    @pulumi.getter(name="oidcDiscoveryUrl")
+    def oidc_discovery_url(self) -> str:
+        return pulumi.get(self, "oidc_discovery_url")
+
+    @property
+    @pulumi.getter(name="boundAudiences")
+    def bound_audiences(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "bound_audiences")
+
+    @property
+    @pulumi.getter(name="claimMappings")
+    def claim_mappings(self) -> Optional[Mapping[str, str]]:
+        return pulumi.get(self, "claim_mappings")
+
+    @property
+    @pulumi.getter(name="discoveryCaPems")
+    def discovery_ca_pems(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "discovery_ca_pems")
+
+    @property
+    @pulumi.getter(name="listClaimMappings")
+    def list_claim_mappings(self) -> Optional[Mapping[str, str]]:
+        return pulumi.get(self, "list_claim_mappings")
+
+    @property
+    @pulumi.getter(name="oidcScopes")
+    def oidc_scopes(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "oidc_scopes")
+
+    @property
+    @pulumi.getter(name="signingAlgs")
+    def signing_algs(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "signing_algs")
+
+
+@pulumi.output_type
 class AclRolePolicy(dict):
     def __init__(__self__, *,
                  name: str):
         """
         :param str name: `(string: <required>)` - A human-friendly name for this ACL Role.
         """
         pulumi.set(__self__, "name", name)
```

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/provider.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/quote_specification.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/quote_specification.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/scheduler_config.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/scheduler_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/sentinel_policy.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/sentinel_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad/volume.py` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad.egg-info/PKG-INFO` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-nomad
-Version: 0.4.1a1681934264
+Version: 0.4.1a1682461165
 Summary: A Pulumi package for creating and managing nomad cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
 Keywords: pulumi nomad
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-nomad/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-nomad/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fnomad.svg)](https://www.npmjs.com/package/@pulumi/nomad)
 [![Python version](https://badge.fury.io/py/pulumi-nomad.svg)](https://pypi.org/project/pulumi-nomad)
 [![NuGet version](https://badge.fury.io/nu/pulumi.nomad.svg)](https://badge.fury.io/nu/pulumi.nomad)
```

### Comparing `pulumi_nomad-0.4.1a1681934264/pulumi_nomad.egg-info/SOURCES.txt` & `pulumi_nomad-0.4.1a1682461165/pulumi_nomad.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 README.md
 setup.py
 pulumi_nomad/__init__.py
 pulumi_nomad/_inputs.py
 pulumi_nomad/_utilities.py
+pulumi_nomad/acl_auth_method.py
+pulumi_nomad/acl_binding_rule.py
 pulumi_nomad/acl_policy.py
 pulumi_nomad/acl_role.py
 pulumi_nomad/acl_token.py
 pulumi_nomad/external_volume.py
 pulumi_nomad/get_acl_policies.py
 pulumi_nomad/get_acl_policy.py
 pulumi_nomad/get_acl_role.py
```

### Comparing `pulumi_nomad-0.4.1a1681934264/setup.py` & `pulumi_nomad-0.4.1a1682461165/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.1a1681934264"
-PLUGIN_VERSION = "0.4.1-alpha.1681934264+d734e04a"
+VERSION = "0.4.1a1682461165"
+PLUGIN_VERSION = "0.4.1-alpha.1682461165+56ffa9b0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'nomad', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "nomad Pulumi Package - Development Version"
 
 
 setup(name='pulumi_nomad',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing nomad cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

