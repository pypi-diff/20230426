# Comparing `tmp/prometheus-pve-exporter-2.2.4.tar.gz` & `tmp/prometheus-pve-exporter-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus-pve-exporter-2.2.4.tar", last modified: Sun Oct 16 11:31:52 2022, max compression
+gzip compressed data, was "prometheus-pve-exporter-2.3.0.tar", last modified: Wed Apr 26 12:22:08 2023, max compression
```

## Comparing `prometheus-pve-exporter-2.2.4.tar` & `prometheus-pve-exporter-2.3.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 11:31:52.088031 prometheus-pve-exporter-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)    14354 2022-10-16 11:31:52.088031 prometheus-pve-exporter-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11253 2022-10-16 11:31:32.000000 prometheus-pve-exporter-2.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-16 11:31:52.088031 prometheus-pve-exporter-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-10-16 11:31:32.000000 prometheus-pve-exporter-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 11:31:52.084031 prometheus-pve-exporter-2.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 11:31:52.084031 prometheus-pve-exporter-2.2.4/src/prometheus_pve_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14354 2022-10-16 11:31:51.000000 prometheus-pve-exporter-2.2.4/src/prometheus_pve_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-10-16 11:31:51.000000 prometheus-pve-exporter-2.2.4/src/prometheus_pve_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-16 11:31:51.000000 prometheus-pve-exporter-2.2.4/src/prometheus_pve_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-16 11:31:51.000000 prometheus-pve-exporter-2.2.4/src/prometheus_pve_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-16 11:31:51.000000 prometheus-pve-exporter-2.2.4/src/prometheus_pve_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-16 11:31:51.000000 prometheus-pve-exporter-2.2.4/src/prometheus_pve_exporter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 11:31:52.088031 prometheus-pve-exporter-2.2.4/src/pve_exporter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-16 11:31:32.000000 prometheus-pve-exporter-2.2.4/src/pve_exporter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4263 2022-10-16 11:31:32.000000 prometheus-pve-exporter-2.2.4/src/pve_exporter/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    11638 2022-10-16 11:31:32.000000 prometheus-pve-exporter-2.2.4/src/pve_exporter/collector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2980 2022-10-16 11:31:32.000000 prometheus-pve-exporter-2.2.4/src/pve_exporter/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4056 2022-10-16 11:31:32.000000 prometheus-pve-exporter-2.2.4/src/pve_exporter/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:22:08.393193 prometheus-pve-exporter-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-04-26 12:22:08.393193 prometheus-pve-exporter-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 12:22:08.397193 prometheus-pve-exporter-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:22:08.389193 prometheus-pve-exporter-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:22:08.393193 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-04-26 12:22:08.000000 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-26 12:22:08.000000 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:22:08.000000 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 12:22:08.000000 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 12:22:08.000000 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 12:22:08.000000 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:22:08.393193 prometheus-pve-exporter-2.3.0/src/pve_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/src/pve_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/src/pve_exporter/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4641 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/src/pve_exporter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/src/pve_exporter/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/src/pve_exporter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/src/pve_exporter/http.py
```

### Comparing `prometheus-pve-exporter-2.2.4/PKG-INFO` & `prometheus-pve-exporter-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,316 +1,319 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 2.2.4
+Version: 2.3.0
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Home-page: https://github.com/prometheus-pve/prometheus-pve-exporter
 Author: Lorenz Schori
 Author-email: lo@znerol.ch
 License: Apache Software License 2.0
-Description: Prometheus Proxmox VE Exporter
-        ==============================
-        
-        |Build Status| |Package Version|
-        
-        This is an exporter that exposes information gathered from Proxmox VE
-        node for use by the Prometheus monitoring system.
-        
-        Installation
-        ------------
-        
-        Note: Python 2 is not supported anymore as of version 2.0.0. Instead use Python 3.6 or better.
-        
-        Using pip:
-        ==========
-        
-        .. code:: shell
-        
-            python3 -m pip install prometheus-pve-exporter
-            pve-exporter --help
-        
-        Using docker:
-        =============
-        
-        .. code:: shell
-        
-           docker pull prompve/prometheus-pve-exporter
-        
-        Example: Display usage message:
-        
-        .. code:: shell
-        
-           docker run -it --rm prompve/prometheus-pve-exporter --help
-        
-        
-        Example: Run the image with a mounted configuration file and published port:
-        
-        .. code:: shell
-        
-           docker run --name prometheus-pve-exporter -d -p 127.0.0.1:9221:9221 -v /path/to/pve.yml:/etc/pve.yml prompve/prometheus-pve-exporter
-        
-        Prometheus PVE Exporter will now be reachable at http://localhost:9221/.
-        
-        Usage
-        -----
-        
-        ::
-        
-            usage: pve_exporter [-h] [--collector.status] [--collector.version]
-                                [--collector.node] [--collector.cluster]
-                                [--collector.resources] [--collector.config]
-                                [config] [port] [address]
-        
-            positional arguments:
-              config                Path to configuration file (pve.yml)
-              port                  Port on which the exporter is listening (9221)
-              address               Address to which the exporter will bind
-        
-            optional arguments:
-              -h, --help            show this help message and exit
-              --collector.status, --no-collector.status
-                                    Exposes Node/VM/CT-Status (default: True)
-              --collector.version, --no-collector.version
-                                    Exposes PVE version info (default: True)
-              --collector.node, --no-collector.node
-                                    Exposes PVE node info (default: True)
-              --collector.cluster, --no-collector.cluster
-                                    Exposes PVE cluster info (default: True)
-              --collector.resources, --no-collector.resources
-                                    Exposes PVE resources info (default: True)
-              --collector.config, --no-collector.config
-                                    Exposes PVE onboot status (default: True)
-        
-        
-        Use `::` for the `address` argument in order to bind to both IPv6 and IPv4
-        sockets on dual stacked machines.
-        
-        Visit http://localhost:9221/pve?target=1.2.3.4 where 1.2.3.4 is the IP
-        of the Proxmox VE node to get metrics from. Specify the ``module``
-        request parameter, to choose which module to use from the config file.
-        
-        The ``target`` request parameter defaults to ``localhost``. Hence if
-        ``pve_exporter`` is deployed directly on the proxmox host, ``target``
-        can be omitted.
-        
-        Use the `--collector.X` / `--no-collector.X` flags to enable disable selected
-        collectors.
-        
-        Note that that the config collector results in one API call per guest VM/CT.
-        It is therefore recommended to disable this collector using the
-        `--no-collector.config` flag on big deployments.
-        
-        See the wiki_  for more examples and docs.
-        
-        Exported Metrics
-        ----------------
-        
-        Here's an example of the metrics exported.
-        
-        ::
-        
-            # HELP pve_up Node/VM/CT-Status is online/running
-            # TYPE pve_up gauge
-            pve_up{id="node/proxmox"} 1.0
-            pve_up{id="qemu/100"} 1.0
-            # HELP pve_disk_size_bytes Size of storage device
-            # TYPE pve_disk_size_bytes gauge
-            pve_disk_size_bytes{id="qemu/100"} 6.8719476736e+010
-            pve_disk_size_bytes{id="node/proxmox"} 3.1044079616e+010
-            pve_disk_size_bytes{id="storage/proxmox/local"} 3.1044079616e+010
-            pve_disk_size_bytes{id="storage/proxmox/local-lvm"} 6.9243764736e+010
-            pve_disk_size_bytes{id="storage/proxmox/vms"} 1.934882766848e+012
-            # HELP pve_disk_usage_bytes Disk usage in bytes
-            # TYPE pve_disk_usage_bytes gauge
-            pve_disk_usage_bytes{id="qemu/100"} 0.0
-            pve_disk_usage_bytes{id="node/proxmox"} 1.7571426304e+010
-            pve_disk_usage_bytes{id="storage/proxmox/local"} 1.7571426304e+010
-            pve_disk_usage_bytes{id="storage/proxmox/local-lvm"} 6.619703908e+09
-            pve_disk_usage_bytes{id="storage/proxmox/vms"} 8.32870981632e+011
-            # HELP pve_memory_size_bytes Size of memory
-            # TYPE pve_memory_size_bytes gauge
-            pve_memory_size_bytes{id="qemu/100"} 1.7179869184e+010
-            pve_memory_size_bytes{id="node/proxmox"} 6.739961856e+010
-            # HELP pve_memory_usage_bytes Memory usage in bytes
-            # TYPE pve_memory_usage_bytes gauge
-            pve_memory_usage_bytes{id="qemu/100"} 1.6573280275e+010
-            pve_memory_usage_bytes{id="node/proxmox"} 5.3907812352e+010
-            # HELP pve_network_transmit_bytes Number of bytes transmitted over the network
-            # TYPE pve_network_transmit_bytes gauge
-            pve_network_transmit_bytes{id="qemu/100"} 7.75070828e+09
-            # HELP pve_network_receive_bytes Number of bytes received over the network
-            # TYPE pve_network_receive_bytes gauge
-            pve_network_receive_bytes{id="qemu/100"} 1.529756162e+09
-            # HELP pve_disk_write_bytes Number of bytes written to storage
-            # TYPE pve_disk_write_bytes gauge
-            pve_disk_write_bytes{id="qemu/100"} 1.50048127488e+011
-            # HELP pve_disk_read_bytes Number of bytes read from storage
-            # TYPE pve_disk_read_bytes gauge
-            pve_disk_read_bytes{id="qemu/100"} 7.473739264e+09
-            # HELP pve_cpu_usage_ratio CPU usage (value between 0.0 and pve_cpu_usage_limit)
-            # TYPE pve_cpu_usage_ratio gauge
-            pve_cpu_usage_ratio{id="qemu/100"} 0.105009724408557
-            pve_cpu_usage_ratio{id="node/proxmox"} 0.984243806697115
-            # HELP pve_cpu_usage_limit Maximum allowed CPU usage
-            # TYPE pve_cpu_usage_limit gauge
-            pve_cpu_usage_limit{id="qemu/100"} 1.0
-            pve_cpu_usage_limit{id="node/proxmox"} 4.0
-            # HELP pve_uptime_seconds Number of seconds since the last boot
-            # TYPE pve_uptime_seconds gauge
-            pve_uptime_seconds{id="qemu/100"} 315039.0
-            pve_uptime_seconds{id="node/proxmox"} 315069.0
-            # HELP pve_storage_shared Whether or not the storage is shared among cluster nodes
-            # TYPE pve_storage_shared gauge
-            pve_storage_shared{id="storage/proxmox/local"} 0.0
-            pve_storage_shared{id="storage/proxmox/local-lvm"} 0.0
-            pve_storage_shared{id="storage/proxmox/vms"} 0.0
-            # HELP pve_guest_info VM/CT info
-            # TYPE pve_guest_info gauge
-            pve_guest_info{id="qemu/100",name="samplevm1",node="proxmox",type="qemu"} 1.0
-            # HELP pve_storage_info Storage info
-            # TYPE pve_storage_info gauge
-            pve_storage_info{id="storage/proxmox/local",node="proxmox",storage="local"} 1.0
-            pve_storage_info{id="storage/proxmox/local-lvm",node="proxmox",storage="local-lvm"} 1.0
-            pve_storage_info{id="storage/proxmox/vms",node="proxmox",storage="vms"} 1.0
-            # HELP pve_node_info Node info
-            # TYPE pve_node_info gauge
-            pve_node_info{id="node/proxmox",level="",name="proxmox",nodeid="0"} 1.0
-            # HELP pve_onboot_status Proxmox vm config onboot value
-            # TYPE pve_onboot_status gauge
-            pve_onboot_status{id="qemu/201",node="proxmox",type="qemu"} 1.0
-            # HELP pve_version_info Proxmox VE version info
-            # TYPE pve_version_info gauge
-            pve_version_info{release="7.1",repoid="6fe299a0",version="7.1-5"} 1.0
-        
-        Authentication
-        --------------
-        
-        **Using pve.yml config file**
-        
-        Example ``pve.yml`` for password authentication:
-        
-        .. code:: yaml
-        
-            default:
-                user: prometheus@pve
-                password: sEcr3T!
-                # Optional: set to false to skip SSL/TLS verification
-                verify_ssl: true
-        
-        Example ``pve.yml`` for `token authentication`_:
-        
-        .. code:: yaml
-        
-           default:
-               user: prometheus@pve
-               token_name: "your-token-id"
-               token_value: "..."
-        
-        **Using environment variables:**
-        
-        If the ``PVE_USER`` environment variable exists, then configuration is taken from
-        the environment instead of from the ``pve.yml`` config file. The following
-        environment variables are respected:
-        
-        * ``PVE_USER``: user name
-        
-        Required for password authentication:
-        
-        * ``PVE_PASSWORD``: user password
-        
-        Required for `token authentication`_:
-        
-        * ``PVE_TOKEN_NAME``: token name
-        * ``PVE_TOKEN_VALUE``: token value
-        
-        Optional:
-        
-        * ``PVE_VERIFY_SSL``: Either ``true`` or ``false``, whether or not to verify PVE tls
-          certificate. Defaults to ``true``.
-        * ``PVE_MODULE``: Name of the configuration module. Defaults to ``default``.
-        
-        The configuration is passed directly into `proxmoxer.ProxmoxAPI()`_.
-        
-        **Note on verify_ssl and certificate trust store:**
-        
-        When operating PVE with self-signed certificates, then it is necessary to
-        either import the certificate into the local trust store (see this `SE answer`_
-        for Debian/Ubuntu) or add ``verify_ssl: false`` to the config dict as a sibling
-        to the credentials. Note that PVE `supports Let's Encrypt`_ out ouf the box. In
-        many cases setting up trusted certificates is the better option than operating
-        with self-signed certs.
-        
-        Proxmox VE Configuration
-        ------------------------
-        
-        For security reasons it is essential to add a user with read-only access
-        (PVEAuditor role) for the purpose of metrics collection.
-        
-        Refer to the  `Proxmox Documentation`_ for the several ways of creating a user. 
-        Once created, assign the user the `/` path permission.
-        
-        Prometheus Configuration
-        ------------------------
-        
-        The PVE exporter can be deployed either directly on a Proxmox VE node or
-        onto a separate machine.
-        
-        Example config for PVE exporter running on PVE node:
-        
-        .. code:: yaml
-        
-            scrape_configs:
-              - job_name: 'pve'
-                static_configs:
-                  - targets:
-                    - 192.168.1.2:9221  # Proxmox VE node with PVE exporter.
-                    - 192.168.1.3:9221  # Proxmox VE node with PVE exporter.
-                metrics_path: /pve
-                params:
-                  module: [default]
-        
-        Example config for PVE exporter running on Prometheus host:
-        
-        .. code:: yaml
-        
-            scrape_configs:
-              - job_name: 'pve'
-                static_configs:
-                  - targets:
-                    - 192.168.1.2  # Proxmox VE node.
-                    - 192.168.1.3  # Proxmox VE node.
-                metrics_path: /pve
-                params:
-                  module: [default]
-                relabel_configs:
-                  - source_labels: [__address__]
-                    target_label: __param_target
-                  - source_labels: [__param_target]
-                    target_label: instance
-                  - target_label: __address__
-                    replacement: 127.0.0.1:9221  # PVE exporter.
-        
-        Grafana Dashboards
-        ------------------
-        
-        * `Proxmox via Prometheus by Pietro Saccardi`_
-        
-        .. |Build Status| image:: https://github.com/prometheus-pve/prometheus-pve-exporter/actions/workflows/ci.yml/badge.svg
-           :target: https://github.com/prometheus-pve/prometheus-pve-exporter/actions/workflows/ci.yml
-        .. |Package Version| image:: https://img.shields.io/pypi/v/prometheus-pve-exporter.svg
-           :target: https://pypi.python.org/pypi/prometheus-pve-exporter
-        .. _wiki: https://github.com/prometheus-pve/prometheus-pve-exporter/wiki
-        .. _`token authentication`: https://pve.proxmox.com/wiki/User_Management#pveum_tokens
-        .. _`proxmoxer.ProxmoxAPI()`: https://pypi.python.org/pypi/proxmoxer
-        .. _`SE answer`: https://askubuntu.com/a/1007236
-        .. _`supports Let's Encrypt`: https://pve.proxmox.com/pve-docs/pve-admin-guide.html#sysadmin_certificate_management
-        .. _`Proxmox Documentation`: https://pve.proxmox.com/pve-docs/pve-admin-guide.html#pveum_permission_management
-        .. _`Proxmox via Prometheus by Pietro Saccardi`: https://grafana.com/dashboards/10347
-        
 Keywords: prometheus exporter network monitoring proxmox
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.4
+License-File: LICENSE
+
+Prometheus Proxmox VE Exporter
+==============================
+
+|Build Status| |Package Version|
+
+This is an exporter that exposes information gathered from Proxmox VE
+node for use by the Prometheus monitoring system.
+
+Installation
+------------
+
+Note: Python 2 is not supported anymore as of version 2.0.0. Instead use Python 3.6 or better.
+
+Using pip:
+==========
+
+.. code:: shell
+
+    python3 -m pip install prometheus-pve-exporter
+    pve_exporter --help
+
+Using docker:
+=============
+
+.. code:: shell
+
+   docker pull prompve/prometheus-pve-exporter
+
+Example: Display usage message:
+
+.. code:: shell
+
+   docker run -it --rm prompve/prometheus-pve-exporter --help
+
+
+Example: Run the image with a mounted configuration file and published port:
+
+.. code:: shell
+
+   docker run --name prometheus-pve-exporter -d -p 127.0.0.1:9221:9221 -v /path/to/pve.yml:/etc/pve.yml prompve/prometheus-pve-exporter
+
+Prometheus PVE Exporter will now be reachable at http://localhost:9221/.
+
+Usage
+-----
+
+::
+
+    usage: pve_exporter [-h] [--collector.status] [--collector.version]
+                        [--collector.node] [--collector.cluster]
+                        [--collector.resources] [--collector.config]
+                        [config] [port] [address]
+
+    positional arguments:
+      config                Path to configuration file (pve.yml)
+      port                  Port on which the exporter is listening (9221)
+      address               Address to which the exporter will bind
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      --collector.status, --no-collector.status
+                            Exposes Node/VM/CT-Status (default: True)
+      --collector.version, --no-collector.version
+                            Exposes PVE version info (default: True)
+      --collector.node, --no-collector.node
+                            Exposes PVE node info (default: True)
+      --collector.cluster, --no-collector.cluster
+                            Exposes PVE cluster info (default: True)
+      --collector.resources, --no-collector.resources
+                            Exposes PVE resources info (default: True)
+      --collector.config, --no-collector.config
+                            Exposes PVE onboot status (default: True)
+
+
+Use `::` for the `address` argument in order to bind to both IPv6 and IPv4
+sockets on dual stacked machines.
+
+Visit http://localhost:9221/pve?target=1.2.3.4 where 1.2.3.4 is the IP
+of the Proxmox VE node to get metrics from. Specify the ``module``
+request parameter, to choose which module to use from the config file.
+
+The ``target`` request parameter defaults to ``localhost``. Hence if
+``pve_exporter`` is deployed directly on the proxmox host, ``target``
+can be omitted.
+
+Use the `--collector.X` / `--no-collector.X` flags to enable disable selected
+collectors.
+
+Note that that the config collector results in one API call per guest VM/CT.
+It is therefore recommended to disable this collector using the
+`--no-collector.config` flag on big deployments.
+
+See the wiki_  for more examples and docs.
+
+Exported Metrics
+----------------
+
+Here's an example of the metrics exported.
+
+::
+
+    # HELP pve_up Node/VM/CT-Status is online/running
+    # TYPE pve_up gauge
+    pve_up{id="node/proxmox"} 1.0
+    pve_up{id="qemu/100"} 1.0
+    # HELP pve_disk_size_bytes Size of storage device
+    # TYPE pve_disk_size_bytes gauge
+    pve_disk_size_bytes{id="qemu/100"} 6.8719476736e+010
+    pve_disk_size_bytes{id="node/proxmox"} 3.1044079616e+010
+    pve_disk_size_bytes{id="storage/proxmox/local"} 3.1044079616e+010
+    pve_disk_size_bytes{id="storage/proxmox/local-lvm"} 6.9243764736e+010
+    pve_disk_size_bytes{id="storage/proxmox/vms"} 1.934882766848e+012
+    # HELP pve_disk_usage_bytes Disk usage in bytes
+    # TYPE pve_disk_usage_bytes gauge
+    pve_disk_usage_bytes{id="qemu/100"} 0.0
+    pve_disk_usage_bytes{id="node/proxmox"} 1.7571426304e+010
+    pve_disk_usage_bytes{id="storage/proxmox/local"} 1.7571426304e+010
+    pve_disk_usage_bytes{id="storage/proxmox/local-lvm"} 6.619703908e+09
+    pve_disk_usage_bytes{id="storage/proxmox/vms"} 8.32870981632e+011
+    # HELP pve_memory_size_bytes Size of memory
+    # TYPE pve_memory_size_bytes gauge
+    pve_memory_size_bytes{id="qemu/100"} 1.7179869184e+010
+    pve_memory_size_bytes{id="node/proxmox"} 6.739961856e+010
+    # HELP pve_memory_usage_bytes Memory usage in bytes
+    # TYPE pve_memory_usage_bytes gauge
+    pve_memory_usage_bytes{id="qemu/100"} 1.6573280275e+010
+    pve_memory_usage_bytes{id="node/proxmox"} 5.3907812352e+010
+    # HELP pve_network_transmit_bytes Number of bytes transmitted over the network
+    # TYPE pve_network_transmit_bytes gauge
+    pve_network_transmit_bytes{id="qemu/100"} 7.75070828e+09
+    # HELP pve_network_receive_bytes Number of bytes received over the network
+    # TYPE pve_network_receive_bytes gauge
+    pve_network_receive_bytes{id="qemu/100"} 1.529756162e+09
+    # HELP pve_disk_write_bytes Number of bytes written to storage
+    # TYPE pve_disk_write_bytes gauge
+    pve_disk_write_bytes{id="qemu/100"} 1.50048127488e+011
+    # HELP pve_disk_read_bytes Number of bytes read from storage
+    # TYPE pve_disk_read_bytes gauge
+    pve_disk_read_bytes{id="qemu/100"} 7.473739264e+09
+    # HELP pve_cpu_usage_ratio CPU usage (value between 0.0 and pve_cpu_usage_limit)
+    # TYPE pve_cpu_usage_ratio gauge
+    pve_cpu_usage_ratio{id="qemu/100"} 0.105009724408557
+    pve_cpu_usage_ratio{id="node/proxmox"} 0.984243806697115
+    # HELP pve_cpu_usage_limit Maximum allowed CPU usage
+    # TYPE pve_cpu_usage_limit gauge
+    pve_cpu_usage_limit{id="qemu/100"} 1.0
+    pve_cpu_usage_limit{id="node/proxmox"} 4.0
+    # HELP pve_uptime_seconds Number of seconds since the last boot
+    # TYPE pve_uptime_seconds gauge
+    pve_uptime_seconds{id="qemu/100"} 315039.0
+    pve_uptime_seconds{id="node/proxmox"} 315069.0
+    # HELP pve_storage_shared Whether or not the storage is shared among cluster nodes
+    # TYPE pve_storage_shared gauge
+    pve_storage_shared{id="storage/proxmox/local"} 0.0
+    pve_storage_shared{id="storage/proxmox/local-lvm"} 0.0
+    pve_storage_shared{id="storage/proxmox/vms"} 0.0
+    # HELP pve_guest_info VM/CT info
+    # TYPE pve_guest_info gauge
+    pve_guest_info{id="qemu/100",name="samplevm1",node="proxmox",type="qemu"} 1.0
+    # HELP pve_storage_info Storage info
+    # TYPE pve_storage_info gauge
+    pve_storage_info{id="storage/proxmox/local",node="proxmox",storage="local"} 1.0
+    pve_storage_info{id="storage/proxmox/local-lvm",node="proxmox",storage="local-lvm"} 1.0
+    pve_storage_info{id="storage/proxmox/vms",node="proxmox",storage="vms"} 1.0
+    # HELP pve_node_info Node info
+    # TYPE pve_node_info gauge
+    pve_node_info{id="node/proxmox",level="",name="proxmox",nodeid="0"} 1.0
+    # HELP pve_onboot_status Proxmox vm config onboot value
+    # TYPE pve_onboot_status gauge
+    pve_onboot_status{id="qemu/201",node="proxmox",type="qemu"} 1.0
+    # HELP pve_version_info Proxmox VE version info
+    # TYPE pve_version_info gauge
+    pve_version_info{release="7.1",repoid="6fe299a0",version="7.1-5"} 1.0
+
+Authentication
+--------------
+
+**Using pve.yml config file**
+
+Example ``pve.yml`` for password authentication:
+
+.. code:: yaml
+
+    default:
+        user: prometheus@pve
+        password: sEcr3T!
+        # Optional: set to false to skip SSL/TLS verification
+        verify_ssl: true
+
+Example ``pve.yml`` for `token authentication`_:
+
+.. code:: yaml
+
+   default:
+       user: prometheus@pve
+       token_name: "your-token-id"
+       token_value: "..."
+
+**Using environment variables:**
+
+If the ``PVE_USER`` environment variable exists, then configuration is taken from
+the environment instead of from the ``pve.yml`` config file. The following
+environment variables are respected:
+
+* ``PVE_USER``: user name
+
+Required for password authentication:
+
+* ``PVE_PASSWORD``: user password
+
+Required for `token authentication`_:
+
+* ``PVE_TOKEN_NAME``: token name
+* ``PVE_TOKEN_VALUE``: token value
+
+Optional:
+
+* ``PVE_VERIFY_SSL``: Either ``true`` or ``false``, whether or not to verify PVE tls
+  certificate. Defaults to ``true``.
+* ``PVE_MODULE``: Name of the configuration module. Defaults to ``default``.
+
+The configuration is passed directly into `proxmoxer.ProxmoxAPI()`_.
+
+**Note on verify_ssl and certificate trust store:**
+
+When operating PVE with self-signed certificates, then it is necessary to
+either import the certificate into the local trust store (see this `SE answer`_
+for Debian/Ubuntu) or add ``verify_ssl: false`` to the config dict as a sibling
+to the credentials. Note that PVE `supports Let's Encrypt`_ out ouf the box. In
+many cases setting up trusted certificates is the better option than operating
+with self-signed certs.
+
+Proxmox VE Configuration
+------------------------
+
+For security reasons it is essential to add a user with read-only access
+(PVEAuditor role) for the purpose of metrics collection.
+
+Refer to the  `Proxmox Documentation`_ for the several ways of creating a user. 
+Once created, assign the user the `/` path permission.
+
+Prometheus Configuration
+------------------------
+
+The PVE exporter can be deployed either directly on a Proxmox VE node or
+onto a separate machine.
+
+Example config for PVE exporter running on PVE node:
+
+.. code:: yaml
+
+    scrape_configs:
+      - job_name: 'pve'
+        static_configs:
+          - targets:
+            - 192.168.1.2:9221  # Proxmox VE node with PVE exporter.
+            - 192.168.1.3:9221  # Proxmox VE node with PVE exporter.
+        metrics_path: /pve
+        params:
+          module: [default]
+
+Example config for PVE exporter running on Prometheus host:
+
+.. code:: yaml
+
+    scrape_configs:
+      - job_name: 'pve'
+        static_configs:
+          - targets:
+            - 192.168.1.2  # Proxmox VE node.
+            - 192.168.1.3  # Proxmox VE node.
+        metrics_path: /pve
+        params:
+          module: [default]
+        relabel_configs:
+          - source_labels: [__address__]
+            target_label: __param_target
+          - source_labels: [__param_target]
+            target_label: instance
+          - target_label: __address__
+            replacement: 127.0.0.1:9221  # PVE exporter.
+
+Grafana Dashboards
+------------------
+
+* `Proxmox via Prometheus by Pietro Saccardi`_
+
+.. |Build Status| image:: https://github.com/prometheus-pve/prometheus-pve-exporter/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/prometheus-pve/prometheus-pve-exporter/actions/workflows/ci.yml
+.. |Package Version| image:: https://img.shields.io/pypi/v/prometheus-pve-exporter.svg
+   :target: https://pypi.python.org/pypi/prometheus-pve-exporter
+.. _wiki: https://github.com/prometheus-pve/prometheus-pve-exporter/wiki
+.. _`token authentication`: https://pve.proxmox.com/wiki/User_Management#pveum_tokens
+.. _`proxmoxer.ProxmoxAPI()`: https://pypi.python.org/pypi/proxmoxer
+.. _`SE answer`: https://askubuntu.com/a/1007236
+.. _`supports Let's Encrypt`: https://pve.proxmox.com/pve-docs/pve-admin-guide.html#sysadmin_certificate_management
+.. _`Proxmox Documentation`: https://pve.proxmox.com/pve-docs/pve-admin-guide.html#pveum_permission_management
+.. _`Proxmox via Prometheus by Pietro Saccardi`: https://grafana.com/grafana/dashboards/10347-proxmox-via-prometheus/
+
+
```

### Comparing `prometheus-pve-exporter-2.2.4/README.rst` & `prometheus-pve-exporter-2.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Using pip:
 ==========
 
 .. code:: shell
 
     python3 -m pip install prometheus-pve-exporter
-    pve-exporter --help
+    pve_exporter --help
 
 Using docker:
 =============
 
 .. code:: shell
 
    docker pull prompve/prometheus-pve-exporter
@@ -291,8 +291,8 @@
    :target: https://pypi.python.org/pypi/prometheus-pve-exporter
 .. _wiki: https://github.com/prometheus-pve/prometheus-pve-exporter/wiki
 .. _`token authentication`: https://pve.proxmox.com/wiki/User_Management#pveum_tokens
 .. _`proxmoxer.ProxmoxAPI()`: https://pypi.python.org/pypi/proxmoxer
 .. _`SE answer`: https://askubuntu.com/a/1007236
 .. _`supports Let's Encrypt`: https://pve.proxmox.com/pve-docs/pve-admin-guide.html#sysadmin_certificate_management
 .. _`Proxmox Documentation`: https://pve.proxmox.com/pve-docs/pve-admin-guide.html#pveum_permission_management
-.. _`Proxmox via Prometheus by Pietro Saccardi`: https://grafana.com/dashboards/10347
+.. _`Proxmox via Prometheus by Pietro Saccardi`: https://grafana.com/grafana/dashboards/10347-proxmox-via-prometheus/
```

### Comparing `prometheus-pve-exporter-2.2.4/setup.py` & `prometheus-pve-exporter-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="prometheus-pve-exporter",
-    version="2.2.4",
+    version="2.3.0",
     author="Lorenz Schori",
     author_email="lo@znerol.ch",
     description=("Proxmox VE exporter for the Prometheus monitoring system."),
     long_description=open('README.rst').read(),
     license="Apache Software License 2.0",
     keywords="prometheus exporter network monitoring proxmox",
     url="https://github.com/prometheus-pve/prometheus-pve-exporter",
@@ -21,14 +21,15 @@
     python_requires=">=3.4",
     install_requires=[
         "prometheus_client>=0.0.11",
         "proxmoxer",
         "pyyaml",
         "requests",
         'Werkzeug',
+        'gunicorn',
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Topic :: System :: Monitoring",
         "Topic :: System :: Networking :: Monitoring",
```

### Comparing `prometheus-pve-exporter-2.2.4/src/prometheus_pve_exporter.egg-info/PKG-INFO` & `prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,316 +1,319 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 2.2.4
+Version: 2.3.0
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Home-page: https://github.com/prometheus-pve/prometheus-pve-exporter
 Author: Lorenz Schori
 Author-email: lo@znerol.ch
 License: Apache Software License 2.0
-Description: Prometheus Proxmox VE Exporter
-        ==============================
-        
-        |Build Status| |Package Version|
-        
-        This is an exporter that exposes information gathered from Proxmox VE
-        node for use by the Prometheus monitoring system.
-        
-        Installation
-        ------------
-        
-        Note: Python 2 is not supported anymore as of version 2.0.0. Instead use Python 3.6 or better.
-        
-        Using pip:
-        ==========
-        
-        .. code:: shell
-        
-            python3 -m pip install prometheus-pve-exporter
-            pve-exporter --help
-        
-        Using docker:
-        =============
-        
-        .. code:: shell
-        
-           docker pull prompve/prometheus-pve-exporter
-        
-        Example: Display usage message:
-        
-        .. code:: shell
-        
-           docker run -it --rm prompve/prometheus-pve-exporter --help
-        
-        
-        Example: Run the image with a mounted configuration file and published port:
-        
-        .. code:: shell
-        
-           docker run --name prometheus-pve-exporter -d -p 127.0.0.1:9221:9221 -v /path/to/pve.yml:/etc/pve.yml prompve/prometheus-pve-exporter
-        
-        Prometheus PVE Exporter will now be reachable at http://localhost:9221/.
-        
-        Usage
-        -----
-        
-        ::
-        
-            usage: pve_exporter [-h] [--collector.status] [--collector.version]
-                                [--collector.node] [--collector.cluster]
-                                [--collector.resources] [--collector.config]
-                                [config] [port] [address]
-        
-            positional arguments:
-              config                Path to configuration file (pve.yml)
-              port                  Port on which the exporter is listening (9221)
-              address               Address to which the exporter will bind
-        
-            optional arguments:
-              -h, --help            show this help message and exit
-              --collector.status, --no-collector.status
-                                    Exposes Node/VM/CT-Status (default: True)
-              --collector.version, --no-collector.version
-                                    Exposes PVE version info (default: True)
-              --collector.node, --no-collector.node
-                                    Exposes PVE node info (default: True)
-              --collector.cluster, --no-collector.cluster
-                                    Exposes PVE cluster info (default: True)
-              --collector.resources, --no-collector.resources
-                                    Exposes PVE resources info (default: True)
-              --collector.config, --no-collector.config
-                                    Exposes PVE onboot status (default: True)
-        
-        
-        Use `::` for the `address` argument in order to bind to both IPv6 and IPv4
-        sockets on dual stacked machines.
-        
-        Visit http://localhost:9221/pve?target=1.2.3.4 where 1.2.3.4 is the IP
-        of the Proxmox VE node to get metrics from. Specify the ``module``
-        request parameter, to choose which module to use from the config file.
-        
-        The ``target`` request parameter defaults to ``localhost``. Hence if
-        ``pve_exporter`` is deployed directly on the proxmox host, ``target``
-        can be omitted.
-        
-        Use the `--collector.X` / `--no-collector.X` flags to enable disable selected
-        collectors.
-        
-        Note that that the config collector results in one API call per guest VM/CT.
-        It is therefore recommended to disable this collector using the
-        `--no-collector.config` flag on big deployments.
-        
-        See the wiki_  for more examples and docs.
-        
-        Exported Metrics
-        ----------------
-        
-        Here's an example of the metrics exported.
-        
-        ::
-        
-            # HELP pve_up Node/VM/CT-Status is online/running
-            # TYPE pve_up gauge
-            pve_up{id="node/proxmox"} 1.0
-            pve_up{id="qemu/100"} 1.0
-            # HELP pve_disk_size_bytes Size of storage device
-            # TYPE pve_disk_size_bytes gauge
-            pve_disk_size_bytes{id="qemu/100"} 6.8719476736e+010
-            pve_disk_size_bytes{id="node/proxmox"} 3.1044079616e+010
-            pve_disk_size_bytes{id="storage/proxmox/local"} 3.1044079616e+010
-            pve_disk_size_bytes{id="storage/proxmox/local-lvm"} 6.9243764736e+010
-            pve_disk_size_bytes{id="storage/proxmox/vms"} 1.934882766848e+012
-            # HELP pve_disk_usage_bytes Disk usage in bytes
-            # TYPE pve_disk_usage_bytes gauge
-            pve_disk_usage_bytes{id="qemu/100"} 0.0
-            pve_disk_usage_bytes{id="node/proxmox"} 1.7571426304e+010
-            pve_disk_usage_bytes{id="storage/proxmox/local"} 1.7571426304e+010
-            pve_disk_usage_bytes{id="storage/proxmox/local-lvm"} 6.619703908e+09
-            pve_disk_usage_bytes{id="storage/proxmox/vms"} 8.32870981632e+011
-            # HELP pve_memory_size_bytes Size of memory
-            # TYPE pve_memory_size_bytes gauge
-            pve_memory_size_bytes{id="qemu/100"} 1.7179869184e+010
-            pve_memory_size_bytes{id="node/proxmox"} 6.739961856e+010
-            # HELP pve_memory_usage_bytes Memory usage in bytes
-            # TYPE pve_memory_usage_bytes gauge
-            pve_memory_usage_bytes{id="qemu/100"} 1.6573280275e+010
-            pve_memory_usage_bytes{id="node/proxmox"} 5.3907812352e+010
-            # HELP pve_network_transmit_bytes Number of bytes transmitted over the network
-            # TYPE pve_network_transmit_bytes gauge
-            pve_network_transmit_bytes{id="qemu/100"} 7.75070828e+09
-            # HELP pve_network_receive_bytes Number of bytes received over the network
-            # TYPE pve_network_receive_bytes gauge
-            pve_network_receive_bytes{id="qemu/100"} 1.529756162e+09
-            # HELP pve_disk_write_bytes Number of bytes written to storage
-            # TYPE pve_disk_write_bytes gauge
-            pve_disk_write_bytes{id="qemu/100"} 1.50048127488e+011
-            # HELP pve_disk_read_bytes Number of bytes read from storage
-            # TYPE pve_disk_read_bytes gauge
-            pve_disk_read_bytes{id="qemu/100"} 7.473739264e+09
-            # HELP pve_cpu_usage_ratio CPU usage (value between 0.0 and pve_cpu_usage_limit)
-            # TYPE pve_cpu_usage_ratio gauge
-            pve_cpu_usage_ratio{id="qemu/100"} 0.105009724408557
-            pve_cpu_usage_ratio{id="node/proxmox"} 0.984243806697115
-            # HELP pve_cpu_usage_limit Maximum allowed CPU usage
-            # TYPE pve_cpu_usage_limit gauge
-            pve_cpu_usage_limit{id="qemu/100"} 1.0
-            pve_cpu_usage_limit{id="node/proxmox"} 4.0
-            # HELP pve_uptime_seconds Number of seconds since the last boot
-            # TYPE pve_uptime_seconds gauge
-            pve_uptime_seconds{id="qemu/100"} 315039.0
-            pve_uptime_seconds{id="node/proxmox"} 315069.0
-            # HELP pve_storage_shared Whether or not the storage is shared among cluster nodes
-            # TYPE pve_storage_shared gauge
-            pve_storage_shared{id="storage/proxmox/local"} 0.0
-            pve_storage_shared{id="storage/proxmox/local-lvm"} 0.0
-            pve_storage_shared{id="storage/proxmox/vms"} 0.0
-            # HELP pve_guest_info VM/CT info
-            # TYPE pve_guest_info gauge
-            pve_guest_info{id="qemu/100",name="samplevm1",node="proxmox",type="qemu"} 1.0
-            # HELP pve_storage_info Storage info
-            # TYPE pve_storage_info gauge
-            pve_storage_info{id="storage/proxmox/local",node="proxmox",storage="local"} 1.0
-            pve_storage_info{id="storage/proxmox/local-lvm",node="proxmox",storage="local-lvm"} 1.0
-            pve_storage_info{id="storage/proxmox/vms",node="proxmox",storage="vms"} 1.0
-            # HELP pve_node_info Node info
-            # TYPE pve_node_info gauge
-            pve_node_info{id="node/proxmox",level="",name="proxmox",nodeid="0"} 1.0
-            # HELP pve_onboot_status Proxmox vm config onboot value
-            # TYPE pve_onboot_status gauge
-            pve_onboot_status{id="qemu/201",node="proxmox",type="qemu"} 1.0
-            # HELP pve_version_info Proxmox VE version info
-            # TYPE pve_version_info gauge
-            pve_version_info{release="7.1",repoid="6fe299a0",version="7.1-5"} 1.0
-        
-        Authentication
-        --------------
-        
-        **Using pve.yml config file**
-        
-        Example ``pve.yml`` for password authentication:
-        
-        .. code:: yaml
-        
-            default:
-                user: prometheus@pve
-                password: sEcr3T!
-                # Optional: set to false to skip SSL/TLS verification
-                verify_ssl: true
-        
-        Example ``pve.yml`` for `token authentication`_:
-        
-        .. code:: yaml
-        
-           default:
-               user: prometheus@pve
-               token_name: "your-token-id"
-               token_value: "..."
-        
-        **Using environment variables:**
-        
-        If the ``PVE_USER`` environment variable exists, then configuration is taken from
-        the environment instead of from the ``pve.yml`` config file. The following
-        environment variables are respected:
-        
-        * ``PVE_USER``: user name
-        
-        Required for password authentication:
-        
-        * ``PVE_PASSWORD``: user password
-        
-        Required for `token authentication`_:
-        
-        * ``PVE_TOKEN_NAME``: token name
-        * ``PVE_TOKEN_VALUE``: token value
-        
-        Optional:
-        
-        * ``PVE_VERIFY_SSL``: Either ``true`` or ``false``, whether or not to verify PVE tls
-          certificate. Defaults to ``true``.
-        * ``PVE_MODULE``: Name of the configuration module. Defaults to ``default``.
-        
-        The configuration is passed directly into `proxmoxer.ProxmoxAPI()`_.
-        
-        **Note on verify_ssl and certificate trust store:**
-        
-        When operating PVE with self-signed certificates, then it is necessary to
-        either import the certificate into the local trust store (see this `SE answer`_
-        for Debian/Ubuntu) or add ``verify_ssl: false`` to the config dict as a sibling
-        to the credentials. Note that PVE `supports Let's Encrypt`_ out ouf the box. In
-        many cases setting up trusted certificates is the better option than operating
-        with self-signed certs.
-        
-        Proxmox VE Configuration
-        ------------------------
-        
-        For security reasons it is essential to add a user with read-only access
-        (PVEAuditor role) for the purpose of metrics collection.
-        
-        Refer to the  `Proxmox Documentation`_ for the several ways of creating a user. 
-        Once created, assign the user the `/` path permission.
-        
-        Prometheus Configuration
-        ------------------------
-        
-        The PVE exporter can be deployed either directly on a Proxmox VE node or
-        onto a separate machine.
-        
-        Example config for PVE exporter running on PVE node:
-        
-        .. code:: yaml
-        
-            scrape_configs:
-              - job_name: 'pve'
-                static_configs:
-                  - targets:
-                    - 192.168.1.2:9221  # Proxmox VE node with PVE exporter.
-                    - 192.168.1.3:9221  # Proxmox VE node with PVE exporter.
-                metrics_path: /pve
-                params:
-                  module: [default]
-        
-        Example config for PVE exporter running on Prometheus host:
-        
-        .. code:: yaml
-        
-            scrape_configs:
-              - job_name: 'pve'
-                static_configs:
-                  - targets:
-                    - 192.168.1.2  # Proxmox VE node.
-                    - 192.168.1.3  # Proxmox VE node.
-                metrics_path: /pve
-                params:
-                  module: [default]
-                relabel_configs:
-                  - source_labels: [__address__]
-                    target_label: __param_target
-                  - source_labels: [__param_target]
-                    target_label: instance
-                  - target_label: __address__
-                    replacement: 127.0.0.1:9221  # PVE exporter.
-        
-        Grafana Dashboards
-        ------------------
-        
-        * `Proxmox via Prometheus by Pietro Saccardi`_
-        
-        .. |Build Status| image:: https://github.com/prometheus-pve/prometheus-pve-exporter/actions/workflows/ci.yml/badge.svg
-           :target: https://github.com/prometheus-pve/prometheus-pve-exporter/actions/workflows/ci.yml
-        .. |Package Version| image:: https://img.shields.io/pypi/v/prometheus-pve-exporter.svg
-           :target: https://pypi.python.org/pypi/prometheus-pve-exporter
-        .. _wiki: https://github.com/prometheus-pve/prometheus-pve-exporter/wiki
-        .. _`token authentication`: https://pve.proxmox.com/wiki/User_Management#pveum_tokens
-        .. _`proxmoxer.ProxmoxAPI()`: https://pypi.python.org/pypi/proxmoxer
-        .. _`SE answer`: https://askubuntu.com/a/1007236
-        .. _`supports Let's Encrypt`: https://pve.proxmox.com/pve-docs/pve-admin-guide.html#sysadmin_certificate_management
-        .. _`Proxmox Documentation`: https://pve.proxmox.com/pve-docs/pve-admin-guide.html#pveum_permission_management
-        .. _`Proxmox via Prometheus by Pietro Saccardi`: https://grafana.com/dashboards/10347
-        
 Keywords: prometheus exporter network monitoring proxmox
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.4
+License-File: LICENSE
+
+Prometheus Proxmox VE Exporter
+==============================
+
+|Build Status| |Package Version|
+
+This is an exporter that exposes information gathered from Proxmox VE
+node for use by the Prometheus monitoring system.
+
+Installation
+------------
+
+Note: Python 2 is not supported anymore as of version 2.0.0. Instead use Python 3.6 or better.
+
+Using pip:
+==========
+
+.. code:: shell
+
+    python3 -m pip install prometheus-pve-exporter
+    pve_exporter --help
+
+Using docker:
+=============
+
+.. code:: shell
+
+   docker pull prompve/prometheus-pve-exporter
+
+Example: Display usage message:
+
+.. code:: shell
+
+   docker run -it --rm prompve/prometheus-pve-exporter --help
+
+
+Example: Run the image with a mounted configuration file and published port:
+
+.. code:: shell
+
+   docker run --name prometheus-pve-exporter -d -p 127.0.0.1:9221:9221 -v /path/to/pve.yml:/etc/pve.yml prompve/prometheus-pve-exporter
+
+Prometheus PVE Exporter will now be reachable at http://localhost:9221/.
+
+Usage
+-----
+
+::
+
+    usage: pve_exporter [-h] [--collector.status] [--collector.version]
+                        [--collector.node] [--collector.cluster]
+                        [--collector.resources] [--collector.config]
+                        [config] [port] [address]
+
+    positional arguments:
+      config                Path to configuration file (pve.yml)
+      port                  Port on which the exporter is listening (9221)
+      address               Address to which the exporter will bind
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      --collector.status, --no-collector.status
+                            Exposes Node/VM/CT-Status (default: True)
+      --collector.version, --no-collector.version
+                            Exposes PVE version info (default: True)
+      --collector.node, --no-collector.node
+                            Exposes PVE node info (default: True)
+      --collector.cluster, --no-collector.cluster
+                            Exposes PVE cluster info (default: True)
+      --collector.resources, --no-collector.resources
+                            Exposes PVE resources info (default: True)
+      --collector.config, --no-collector.config
+                            Exposes PVE onboot status (default: True)
+
+
+Use `::` for the `address` argument in order to bind to both IPv6 and IPv4
+sockets on dual stacked machines.
+
+Visit http://localhost:9221/pve?target=1.2.3.4 where 1.2.3.4 is the IP
+of the Proxmox VE node to get metrics from. Specify the ``module``
+request parameter, to choose which module to use from the config file.
+
+The ``target`` request parameter defaults to ``localhost``. Hence if
+``pve_exporter`` is deployed directly on the proxmox host, ``target``
+can be omitted.
+
+Use the `--collector.X` / `--no-collector.X` flags to enable disable selected
+collectors.
+
+Note that that the config collector results in one API call per guest VM/CT.
+It is therefore recommended to disable this collector using the
+`--no-collector.config` flag on big deployments.
+
+See the wiki_  for more examples and docs.
+
+Exported Metrics
+----------------
+
+Here's an example of the metrics exported.
+
+::
+
+    # HELP pve_up Node/VM/CT-Status is online/running
+    # TYPE pve_up gauge
+    pve_up{id="node/proxmox"} 1.0
+    pve_up{id="qemu/100"} 1.0
+    # HELP pve_disk_size_bytes Size of storage device
+    # TYPE pve_disk_size_bytes gauge
+    pve_disk_size_bytes{id="qemu/100"} 6.8719476736e+010
+    pve_disk_size_bytes{id="node/proxmox"} 3.1044079616e+010
+    pve_disk_size_bytes{id="storage/proxmox/local"} 3.1044079616e+010
+    pve_disk_size_bytes{id="storage/proxmox/local-lvm"} 6.9243764736e+010
+    pve_disk_size_bytes{id="storage/proxmox/vms"} 1.934882766848e+012
+    # HELP pve_disk_usage_bytes Disk usage in bytes
+    # TYPE pve_disk_usage_bytes gauge
+    pve_disk_usage_bytes{id="qemu/100"} 0.0
+    pve_disk_usage_bytes{id="node/proxmox"} 1.7571426304e+010
+    pve_disk_usage_bytes{id="storage/proxmox/local"} 1.7571426304e+010
+    pve_disk_usage_bytes{id="storage/proxmox/local-lvm"} 6.619703908e+09
+    pve_disk_usage_bytes{id="storage/proxmox/vms"} 8.32870981632e+011
+    # HELP pve_memory_size_bytes Size of memory
+    # TYPE pve_memory_size_bytes gauge
+    pve_memory_size_bytes{id="qemu/100"} 1.7179869184e+010
+    pve_memory_size_bytes{id="node/proxmox"} 6.739961856e+010
+    # HELP pve_memory_usage_bytes Memory usage in bytes
+    # TYPE pve_memory_usage_bytes gauge
+    pve_memory_usage_bytes{id="qemu/100"} 1.6573280275e+010
+    pve_memory_usage_bytes{id="node/proxmox"} 5.3907812352e+010
+    # HELP pve_network_transmit_bytes Number of bytes transmitted over the network
+    # TYPE pve_network_transmit_bytes gauge
+    pve_network_transmit_bytes{id="qemu/100"} 7.75070828e+09
+    # HELP pve_network_receive_bytes Number of bytes received over the network
+    # TYPE pve_network_receive_bytes gauge
+    pve_network_receive_bytes{id="qemu/100"} 1.529756162e+09
+    # HELP pve_disk_write_bytes Number of bytes written to storage
+    # TYPE pve_disk_write_bytes gauge
+    pve_disk_write_bytes{id="qemu/100"} 1.50048127488e+011
+    # HELP pve_disk_read_bytes Number of bytes read from storage
+    # TYPE pve_disk_read_bytes gauge
+    pve_disk_read_bytes{id="qemu/100"} 7.473739264e+09
+    # HELP pve_cpu_usage_ratio CPU usage (value between 0.0 and pve_cpu_usage_limit)
+    # TYPE pve_cpu_usage_ratio gauge
+    pve_cpu_usage_ratio{id="qemu/100"} 0.105009724408557
+    pve_cpu_usage_ratio{id="node/proxmox"} 0.984243806697115
+    # HELP pve_cpu_usage_limit Maximum allowed CPU usage
+    # TYPE pve_cpu_usage_limit gauge
+    pve_cpu_usage_limit{id="qemu/100"} 1.0
+    pve_cpu_usage_limit{id="node/proxmox"} 4.0
+    # HELP pve_uptime_seconds Number of seconds since the last boot
+    # TYPE pve_uptime_seconds gauge
+    pve_uptime_seconds{id="qemu/100"} 315039.0
+    pve_uptime_seconds{id="node/proxmox"} 315069.0
+    # HELP pve_storage_shared Whether or not the storage is shared among cluster nodes
+    # TYPE pve_storage_shared gauge
+    pve_storage_shared{id="storage/proxmox/local"} 0.0
+    pve_storage_shared{id="storage/proxmox/local-lvm"} 0.0
+    pve_storage_shared{id="storage/proxmox/vms"} 0.0
+    # HELP pve_guest_info VM/CT info
+    # TYPE pve_guest_info gauge
+    pve_guest_info{id="qemu/100",name="samplevm1",node="proxmox",type="qemu"} 1.0
+    # HELP pve_storage_info Storage info
+    # TYPE pve_storage_info gauge
+    pve_storage_info{id="storage/proxmox/local",node="proxmox",storage="local"} 1.0
+    pve_storage_info{id="storage/proxmox/local-lvm",node="proxmox",storage="local-lvm"} 1.0
+    pve_storage_info{id="storage/proxmox/vms",node="proxmox",storage="vms"} 1.0
+    # HELP pve_node_info Node info
+    # TYPE pve_node_info gauge
+    pve_node_info{id="node/proxmox",level="",name="proxmox",nodeid="0"} 1.0
+    # HELP pve_onboot_status Proxmox vm config onboot value
+    # TYPE pve_onboot_status gauge
+    pve_onboot_status{id="qemu/201",node="proxmox",type="qemu"} 1.0
+    # HELP pve_version_info Proxmox VE version info
+    # TYPE pve_version_info gauge
+    pve_version_info{release="7.1",repoid="6fe299a0",version="7.1-5"} 1.0
+
+Authentication
+--------------
+
+**Using pve.yml config file**
+
+Example ``pve.yml`` for password authentication:
+
+.. code:: yaml
+
+    default:
+        user: prometheus@pve
+        password: sEcr3T!
+        # Optional: set to false to skip SSL/TLS verification
+        verify_ssl: true
+
+Example ``pve.yml`` for `token authentication`_:
+
+.. code:: yaml
+
+   default:
+       user: prometheus@pve
+       token_name: "your-token-id"
+       token_value: "..."
+
+**Using environment variables:**
+
+If the ``PVE_USER`` environment variable exists, then configuration is taken from
+the environment instead of from the ``pve.yml`` config file. The following
+environment variables are respected:
+
+* ``PVE_USER``: user name
+
+Required for password authentication:
+
+* ``PVE_PASSWORD``: user password
+
+Required for `token authentication`_:
+
+* ``PVE_TOKEN_NAME``: token name
+* ``PVE_TOKEN_VALUE``: token value
+
+Optional:
+
+* ``PVE_VERIFY_SSL``: Either ``true`` or ``false``, whether or not to verify PVE tls
+  certificate. Defaults to ``true``.
+* ``PVE_MODULE``: Name of the configuration module. Defaults to ``default``.
+
+The configuration is passed directly into `proxmoxer.ProxmoxAPI()`_.
+
+**Note on verify_ssl and certificate trust store:**
+
+When operating PVE with self-signed certificates, then it is necessary to
+either import the certificate into the local trust store (see this `SE answer`_
+for Debian/Ubuntu) or add ``verify_ssl: false`` to the config dict as a sibling
+to the credentials. Note that PVE `supports Let's Encrypt`_ out ouf the box. In
+many cases setting up trusted certificates is the better option than operating
+with self-signed certs.
+
+Proxmox VE Configuration
+------------------------
+
+For security reasons it is essential to add a user with read-only access
+(PVEAuditor role) for the purpose of metrics collection.
+
+Refer to the  `Proxmox Documentation`_ for the several ways of creating a user. 
+Once created, assign the user the `/` path permission.
+
+Prometheus Configuration
+------------------------
+
+The PVE exporter can be deployed either directly on a Proxmox VE node or
+onto a separate machine.
+
+Example config for PVE exporter running on PVE node:
+
+.. code:: yaml
+
+    scrape_configs:
+      - job_name: 'pve'
+        static_configs:
+          - targets:
+            - 192.168.1.2:9221  # Proxmox VE node with PVE exporter.
+            - 192.168.1.3:9221  # Proxmox VE node with PVE exporter.
+        metrics_path: /pve
+        params:
+          module: [default]
+
+Example config for PVE exporter running on Prometheus host:
+
+.. code:: yaml
+
+    scrape_configs:
+      - job_name: 'pve'
+        static_configs:
+          - targets:
+            - 192.168.1.2  # Proxmox VE node.
+            - 192.168.1.3  # Proxmox VE node.
+        metrics_path: /pve
+        params:
+          module: [default]
+        relabel_configs:
+          - source_labels: [__address__]
+            target_label: __param_target
+          - source_labels: [__param_target]
+            target_label: instance
+          - target_label: __address__
+            replacement: 127.0.0.1:9221  # PVE exporter.
+
+Grafana Dashboards
+------------------
+
+* `Proxmox via Prometheus by Pietro Saccardi`_
+
+.. |Build Status| image:: https://github.com/prometheus-pve/prometheus-pve-exporter/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/prometheus-pve/prometheus-pve-exporter/actions/workflows/ci.yml
+.. |Package Version| image:: https://img.shields.io/pypi/v/prometheus-pve-exporter.svg
+   :target: https://pypi.python.org/pypi/prometheus-pve-exporter
+.. _wiki: https://github.com/prometheus-pve/prometheus-pve-exporter/wiki
+.. _`token authentication`: https://pve.proxmox.com/wiki/User_Management#pveum_tokens
+.. _`proxmoxer.ProxmoxAPI()`: https://pypi.python.org/pypi/proxmoxer
+.. _`SE answer`: https://askubuntu.com/a/1007236
+.. _`supports Let's Encrypt`: https://pve.proxmox.com/pve-docs/pve-admin-guide.html#sysadmin_certificate_management
+.. _`Proxmox Documentation`: https://pve.proxmox.com/pve-docs/pve-admin-guide.html#pveum_permission_management
+.. _`Proxmox via Prometheus by Pietro Saccardi`: https://grafana.com/grafana/dashboards/10347-proxmox-via-prometheus/
+
+
```

### Comparing `prometheus-pve-exporter-2.2.4/src/pve_exporter/cli.py` & `prometheus-pve-exporter-2.3.0/src/pve_exporter/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,14 +84,16 @@
                         help='Exposes PVE onboot status')
     parser.add_argument('config', nargs='?', default='pve.yml',
                         help='Path to configuration file (pve.yml)')
     parser.add_argument('port', nargs='?', type=int, default='9221',
                         help='Port on which the exporter is listening (9221)')
     parser.add_argument('address', nargs='?', default='',
                         help='Address to which the exporter will bind')
+    parser.add_argument('--server.keyfile', dest='server_keyfile', help='SSL key for server')
+    parser.add_argument('--server.certfile', dest='server_certfile', help='SSL certificate for server')
 
     params = parser.parse_args()
 
     collectors = CollectorsOptions(
         status=params.collector_status,
         version=params.collector_version,
         node=params.collector_node,
@@ -103,11 +105,18 @@
     # Load configuration.
     if 'PVE_USER' in os.environ:
         config = config_from_env(os.environ)
     else:
         with open(params.config) as handle:
             config = config_from_yaml(yaml.safe_load(handle))
 
+    gunicorn_options = {
+        'bind': f'{params.address}:{params.port}',
+        'threads': 2,
+        'keyfile': params.server_keyfile,
+        'certfile': params.server_certfile,
+    }
+
     if config.valid:
-        start_http_server(config, params.port, params.address, collectors)
+        start_http_server(config, gunicorn_options, collectors)
     else:
         parser.error(str(config))
```

### Comparing `prometheus-pve-exporter-2.2.4/src/pve_exporter/collector.py` & `prometheus-pve-exporter-2.3.0/src/pve_exporter/collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,18 +43,18 @@
             labels=['id'])
 
         for entry in self._pve.cluster.status.get():
             if entry['type'] == 'node':
                 label_values = [entry['id']]
                 status_metrics.add_metric(label_values, entry['online'])
             elif entry['type'] == 'cluster':
-                label_values = ['cluster/{:s}'.format(entry['name'])]
+                label_values = [f"cluster/{entry['name']}"]
                 status_metrics.add_metric(label_values, entry['quorate'])
             else:
-                raise ValueError('Got unexpected status entry type {:s}'.format(entry['type']))
+                raise ValueError(f"Got unexpected status entry type {entry['type']}")
 
         for resource in self._pve.cluster.resources.get(type='vm'):
             label_values = [resource['id']]
             status_metrics.add_metric(label_values, resource['status'] == 'running')
 
         yield status_metrics
 
@@ -133,15 +133,15 @@
         if clusters:
             # Remove superflous keys.
             for cluster in clusters:
                 del cluster['type']
 
             # Add cluster-prefix to id.
             for cluster in clusters:
-                cluster['id'] = 'cluster/{:s}'.format(cluster['name'])
+                cluster['id'] = f"cluster/{cluster['name']}"
                 del cluster['name']
 
             # Yield remaining data.
             labels = clusters[0].keys()
             info_metrics = GaugeMetricFamily(
                 'pve_cluster_info',
                 'Cluster info',
@@ -285,23 +285,23 @@
             # next one in order to avoid failing the whole scrape.
             try:
                 # Qemu
                 vmtype = 'qemu'
                 for vmdata in self._pve.nodes(node['node']).qemu.get():
                     config = self._pve.nodes(node['node']).qemu(vmdata['vmid']).config.get().items()
                     for key, metric_value in config:
-                        label_values = ["%s/%s" % (vmtype, vmdata['vmid']), node['node'], vmtype]
+                        label_values = [f"{vmtype}/{vmdata['vmid']}", node['node'], vmtype]
                         if key in metrics:
                             metrics[key].add_metric(label_values, metric_value)
                 # LXC
                 vmtype = 'lxc'
                 for vmdata in self._pve.nodes(node['node']).lxc.get():
                     config = self._pve.nodes(node['node']).lxc(vmdata['vmid']).config.get().items()
                     for key, metric_value in config:
-                        label_values = ["%s/%s" % (vmtype, vmdata['vmid']), node['node'], vmtype]
+                        label_values = [f"{vmtype}/{vmdata['vmid']}", node['node'], vmtype]
                         if key in metrics:
                             metrics[key].add_metric(label_values, metric_value)
 
             except ResourceException:
                 self._log.exception(
                     "Exception thrown while scraping quemu/lxc config from %s",
                     node['node']
```

### Comparing `prometheus-pve-exporter-2.2.4/src/pve_exporter/config.py` & `prometheus-pve-exporter-2.3.0/src/pve_exporter/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 """
 Config module for Proxmox VE prometheus collector.
 """
 
-try:
-    from collections.abc import Mapping
-except ImportError:
-    from collections import Mapping
-
+from collections.abc import Mapping
 
 def config_from_yaml(yaml):
     """
     Given a dictionary parsed from a yaml file return a config object.
     """
 
     if not isinstance(yaml, Mapping):
@@ -20,15 +16,15 @@
 
     modules = {
         key: config_module_from_yaml(value) for
         key, value in
         yaml.items()
     }
     invalid = [
-        "  - {0}: {1}".format(key, module) for
+        f"  - {key}: {module}" for
         key, module in
         modules.items() if
         not module.valid
     ]
 
     if invalid:
         return ConfigInvalid("\n".join(
@@ -96,15 +92,15 @@
     def __init__(self, mapping):
         super().__init__()
         self._mapping = mapping
 
     def __str__(self):
         num = len(self._mapping)
         keys = ", ".join(self._mapping.keys())
-        return "Valid config: with {0} keys: {1}".format(num, keys)
+        return f"Valid config: with {num} keys: {keys}"
 
     def __getitem__(self, key):
         return self._mapping[key]
 
     def __iter__(self):
         return iter(self._mapping)
 
@@ -121,8 +117,8 @@
 
     valid = False
 
     def __init__(self, error="Unspecified reason."):
         self._error = error
 
     def __str__(self):
-        return "Invalid config: {0}".format(self._error)
+        return f"Invalid config: {self._error}"
```

### Comparing `prometheus-pve-exporter-2.2.4/src/pve_exporter/http.py` & `prometheus-pve-exporter-2.3.0/src/pve_exporter/http.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 HTTP API for Proxmox VE prometheus collector.
 """
 
 import logging
 import time
 
+import gunicorn.app.base
 from prometheus_client import CONTENT_TYPE_LATEST, Summary, Counter, generate_latest
 from werkzeug.routing import Map, Rule
-from werkzeug.serving import run_simple
 from werkzeug.wrappers import Request, Response
 from werkzeug.exceptions import InternalServerError
 from .collector import collect_pve
 
 
 class PveExporterApplication:
     """
@@ -36,15 +36,15 @@
         if module in self._config:
             start = time.time()
             output = collect_pve(self._config[module], target, self._collectors)
             response = Response(output)
             response.headers['content-type'] = CONTENT_TYPE_LATEST
             self._duration.labels(module).observe(time.time() - start)
         else:
-            response = Response("Module '{0}' not found in config".format(module))
+            response = Response("Module '{module}' not found in config")
             response.status_code = 400
 
         return response
 
     def on_metrics(self):
         """
         Request handler for /metrics route
@@ -108,15 +108,38 @@
         ])
 
         urls = url_map.bind_to_environ(request.environ)
         view_func = lambda endpoint, values: self.view(endpoint, values, request.args)
         return urls.dispatch(view_func, catch_http_exceptions=True)
 
 
-def start_http_server(config, port, address, collectors):
+class StandaloneGunicornApplication(gunicorn.app.base.BaseApplication):
+    """
+    Copy-paste from https://docs.gunicorn.org/en/stable/custom.html
+    """
+
+    # 'init' and 'load' methods are implemented by WSGIApplication.
+    # pylint: disable=abstract-method
+
+    def __init__(self, app, options=None):
+        self.options = options or {}
+        self.application = app
+        super().__init__()
+
+    def load_config(self):
+        config = {key: value for key, value in self.options.items()
+                  if key in self.cfg.settings and value is not None}
+        for key, value in config.items():
+            self.cfg.set(key.lower(), value)
+
+    def load(self):
+        return self.application
+
+
+def start_http_server(config, gunicorn_options, collectors):
     """
     Start a HTTP API server for Proxmox VE prometheus collector.
     """
 
     duration = Summary(
         'pve_collection_duration_seconds',
         'Duration of collections by the PVE exporter',
@@ -132,8 +155,8 @@
     for module in config.keys():
         # pylint: disable=no-member
         errors.labels(module)
         # pylint: disable=no-member
         duration.labels(module)
 
     app = PveExporterApplication(config, duration, errors, collectors)
-    run_simple(address, port, app, threaded=True)
+    StandaloneGunicornApplication(app, gunicorn_options).run()
```

