# Comparing `tmp/pulumi_equinix-0.1.1.tar.gz` & `tmp/pulumi_equinix-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_equinix-0.1.1.tar", last modified: Fri Mar 31 19:37:01 2023, max compression
+gzip compressed data, was "pulumi_equinix-0.2.0.tar", last modified: Tue Apr 25 14:50:03 2023, max compression
```

## Comparing `pulumi_equinix-0.1.1.tar` & `pulumi_equinix-0.2.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:37:01.791347 pulumi_equinix-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-31 19:37:01.791347 pulumi_equinix-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:37:01.779347 pulumi_equinix-0.1.1/pulumi_equinix/
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:37:01.779347 pulumi_equinix-0.1.1/pulumi_equinix/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:37:01.783347 pulumi_equinix-0.1.1/pulumi_equinix/fabric/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/fabric/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)   153150 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/fabric/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40569 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/fabric/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/fabric/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/fabric/get_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/fabric/get_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/fabric/get_service_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/fabric/get_service_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)   278984 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/fabric/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49961 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/fabric/service_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:37:01.787347 pulumi_equinix-0.1.1/pulumi_equinix/metal/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    36924 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/bgp_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    98205 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/device_network_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_device_bgp_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_hardware_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_interconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_ip_block_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_operating_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_plans.py
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_port.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_precreated_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_project_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_reserved_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_spot_market_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/get_vrf.py
--rw-r--r--   0 runner    (1001) docker     (123)    40307 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/interconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/ip_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    22562 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/organization_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    53545 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27669 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    20194 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/port_vlan_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/project_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/project_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    47883 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/reserved_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/user_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    42418 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/metal/vrf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:37:01.791347 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    65598 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/acl_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    92184 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/device_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    23682 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/get_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/get_device_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/get_device_software.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/get_device_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    23195 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/network_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    85384 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/networkedge/ssh_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:37:01.779347 pulumi_equinix-0.1.1/pulumi_equinix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/pulumi_equinix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 19:37:01.791347 pulumi_equinix-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-31 19:37:01.000000 pulumi_equinix-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.819202 pulumi_equinix-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-25 14:50:03.819202 pulumi_equinix-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.803201 pulumi_equinix-0.2.0/pulumi_equinix/
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.803201 pulumi_equinix-0.2.0/pulumi_equinix/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.807201 pulumi_equinix-0.2.0/pulumi_equinix/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153044 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40569 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_service_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_service_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)   278947 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49961 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/fabric/service_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.815201 pulumi_equinix-0.2.0/pulumi_equinix/metal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36916 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/bgp_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100333 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/device_network_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_device_bgp_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_hardware_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_ip_block_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_plans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_precreated_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_project_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_reserved_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_spot_market_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/get_vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41964 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20819 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/ip_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22562 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/organization_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53563 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27669 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/port_vlan_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/project_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/project_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47745 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/reserved_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28278 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/user_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42418 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/metal/vrf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.819202 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65598 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/acl_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92184 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/device_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23682 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device_software.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23195 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/network_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85384 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/networkedge/ssh_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:50:03.803201 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/pulumi_equinix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:50:03.819202 pulumi_equinix-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 14:50:03.000000 pulumi_equinix-0.2.0/setup.py
```

### Comparing `pulumi_equinix-0.1.1/PKG-INFO` & `pulumi_equinix-0.2.0/pulumi_equinix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_equinix
-Version: 0.1.1
+Name: pulumi-equinix
+Version: 0.2.0
 Summary: A Pulumi package for creating and managing equinix cloud resources.
 Home-page: https://deploy.equinix.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/equinix/pulumi-equinix
 Keywords: pulumi equinix category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_equinix-0.1.1/README.md` & `pulumi_equinix-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/__init__.py` & `pulumi_equinix-0.2.0/pulumi_equinix/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/_enums.py` & `pulumi_equinix-0.2.0/pulumi_equinix/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/_utilities.py` & `pulumi_equinix-0.2.0/pulumi_equinix/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/config/vars.py` & `pulumi_equinix-0.2.0/pulumi_equinix/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/fabric/__init__.py` & `pulumi_equinix-0.2.0/pulumi_equinix/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/fabric/_enums.py` & `pulumi_equinix-0.2.0/pulumi_equinix/fabric/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/fabric/_inputs.py` & `pulumi_equinix-0.2.0/pulumi_equinix/fabric/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3643,31 +3643,31 @@
 
 @pulumi.input_type
 class ServiceProfilePortArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  uuid: pulumi.Input[str],
                  cross_connect_id: Optional[pulumi.Input[str]] = None,
-                 locations: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfilePortLocationArgs']]]] = None,
+                 location: Optional[pulumi.Input['ServiceProfilePortLocationArgs']] = None,
                  seller_region: Optional[pulumi.Input[str]] = None,
                  seller_region_description: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] type: Colo/Port Type
         :param pulumi.Input[str] uuid: Colo/Port Uuid
         :param pulumi.Input[str] cross_connect_id: Cross Connect Id
-        :param pulumi.Input[Sequence[pulumi.Input['ServiceProfilePortLocationArgs']]] locations: Colo/Port Location
+        :param pulumi.Input['ServiceProfilePortLocationArgs'] location: Colo/Port Location
         :param pulumi.Input[str] seller_region: Seller Region
         :param pulumi.Input[str] seller_region_description: Seller Region details
         """
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "uuid", uuid)
         if cross_connect_id is not None:
             pulumi.set(__self__, "cross_connect_id", cross_connect_id)
-        if locations is not None:
-            pulumi.set(__self__, "locations", locations)
+        if location is not None:
+            pulumi.set(__self__, "location", location)
         if seller_region is not None:
             pulumi.set(__self__, "seller_region", seller_region)
         if seller_region_description is not None:
             pulumi.set(__self__, "seller_region_description", seller_region_description)
 
     @property
     @pulumi.getter
@@ -3703,23 +3703,23 @@
 
     @cross_connect_id.setter
     def cross_connect_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cross_connect_id", value)
 
     @property
     @pulumi.getter
-    def locations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfilePortLocationArgs']]]]:
+    def location(self) -> Optional[pulumi.Input['ServiceProfilePortLocationArgs']]:
         """
         Colo/Port Location
         """
-        return pulumi.get(self, "locations")
+        return pulumi.get(self, "location")
 
-    @locations.setter
-    def locations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfilePortLocationArgs']]]]):
-        pulumi.set(self, "locations", value)
+    @location.setter
+    def location(self, value: Optional[pulumi.Input['ServiceProfilePortLocationArgs']]):
+        pulumi.set(self, "location", value)
 
     @property
     @pulumi.getter(name="sellerRegion")
     def seller_region(self) -> Optional[pulumi.Input[str]]:
         """
         Seller Region
         """
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/fabric/connection.py` & `pulumi_equinix-0.2.0/pulumi_equinix/fabric/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/fabric/get_connection.py` & `pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/fabric/get_port.py` & `pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_port.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/fabric/get_ports.py` & `pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_ports.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/fabric/get_service_profile.py` & `pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_service_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/fabric/get_service_profiles.py` & `pulumi_equinix-0.2.0/pulumi_equinix/fabric/get_service_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/fabric/outputs.py` & `pulumi_equinix-0.2.0/pulumi_equinix/fabric/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3501,31 +3501,31 @@
         ServiceProfilePort.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  type: str,
                  uuid: str,
                  cross_connect_id: Optional[str] = None,
-                 locations: Optional[Sequence['outputs.ServiceProfilePortLocation']] = None,
+                 location: Optional['outputs.ServiceProfilePortLocation'] = None,
                  seller_region: Optional[str] = None,
                  seller_region_description: Optional[str] = None):
         """
         :param str type: Colo/Port Type
         :param str uuid: Colo/Port Uuid
         :param str cross_connect_id: Cross Connect Id
-        :param Sequence['ServiceProfilePortLocationArgs'] locations: Colo/Port Location
+        :param 'ServiceProfilePortLocationArgs' location: Colo/Port Location
         :param str seller_region: Seller Region
         :param str seller_region_description: Seller Region details
         """
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "uuid", uuid)
         if cross_connect_id is not None:
             pulumi.set(__self__, "cross_connect_id", cross_connect_id)
-        if locations is not None:
-            pulumi.set(__self__, "locations", locations)
+        if location is not None:
+            pulumi.set(__self__, "location", location)
         if seller_region is not None:
             pulumi.set(__self__, "seller_region", seller_region)
         if seller_region_description is not None:
             pulumi.set(__self__, "seller_region_description", seller_region_description)
 
     @property
     @pulumi.getter
@@ -3549,19 +3549,19 @@
         """
         Cross Connect Id
         """
         return pulumi.get(self, "cross_connect_id")
 
     @property
     @pulumi.getter
-    def locations(self) -> Optional[Sequence['outputs.ServiceProfilePortLocation']]:
+    def location(self) -> Optional['outputs.ServiceProfilePortLocation']:
         """
         Colo/Port Location
         """
-        return pulumi.get(self, "locations")
+        return pulumi.get(self, "location")
 
     @property
     @pulumi.getter(name="sellerRegion")
     def seller_region(self) -> Optional[str]:
         """
         Seller Region
         """
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/fabric/service_profile.py` & `pulumi_equinix-0.2.0/pulumi_equinix/fabric/service_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/__init__.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/_enums.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/_inputs.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -616,16 +616,16 @@
                  asn: pulumi.Input[int],
                  deployment_type: pulumi.Input[str],
                  max_prefix: Optional[pulumi.Input[int]] = None,
                  md5: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[int] asn: Autonomous System Number for local BGP deployment.
-        :param pulumi.Input[str] deployment_type: `private` or `public`, the `private` is likely to be usable immediately, the
-               `public` will need to be reviewed by Equinix Metal engineers.
+        :param pulumi.Input[str] deployment_type: `local` or `global`, the `local` is likely to be usable immediately, the
+               `global` will need to be reviewed by Equinix Metal engineers.
         :param pulumi.Input[int] max_prefix: The maximum number of route filters allowed per server.
         :param pulumi.Input[str] md5: Password for BGP session in plaintext (not a checksum).
         :param pulumi.Input[str] status: status of BGP configuration in the project.
         """
         pulumi.set(__self__, "asn", asn)
         pulumi.set(__self__, "deployment_type", deployment_type)
         if max_prefix is not None:
@@ -647,16 +647,16 @@
     def asn(self, value: pulumi.Input[int]):
         pulumi.set(self, "asn", value)
 
     @property
     @pulumi.getter(name="deploymentType")
     def deployment_type(self) -> pulumi.Input[str]:
         """
-        `private` or `public`, the `private` is likely to be usable immediately, the
-        `public` will need to be reviewed by Equinix Metal engineers.
+        `local` or `global`, the `local` is likely to be usable immediately, the
+        `global` will need to be reviewed by Equinix Metal engineers.
         """
         return pulumi.get(self, "deployment_type")
 
     @deployment_type.setter
     def deployment_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "deployment_type", value)
 
@@ -927,15 +927,15 @@
 @pulumi.input_type
 class GetMetroCapacityArgs:
     def __init__(__self__, *,
                  plan: str,
                  quantity: Optional[int] = None):
         """
         :param str plan: Device plan that must be available in selected location.
-        :param int quantity: Minimun number of devices that must be available in selected location.
+        :param int quantity: Minimum number of devices that must be available in selected location.
                Default is `1`.
         """
         pulumi.set(__self__, "plan", plan)
         if quantity is not None:
             pulumi.set(__self__, "quantity", quantity)
 
     @property
@@ -950,15 +950,15 @@
     def plan(self, value: str):
         pulumi.set(self, "plan", value)
 
     @property
     @pulumi.getter
     def quantity(self) -> Optional[int]:
         """
-        Minimun number of devices that must be available in selected location.
+        Minimum number of devices that must be available in selected location.
         Default is `1`.
         """
         return pulumi.get(self, "quantity")
 
     @quantity.setter
     def quantity(self, value: Optional[int]):
         pulumi.set(self, "quantity", value)
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/bgp_session.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/bgp_session.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/device.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,18 @@
         :param pulumi.Input[str] project_id: The ID of the project in which to create the device
         :param pulumi.Input[bool] always_pxe: If true, a device with OS `custom_ipxe` will continue to boot via iPXE
                on reboots.
         :param pulumi.Input['DeviceBehaviorArgs'] behavior: Behavioral overrides that change how the resource handles certain attribute updates. See Behavior below for more details.
         :param pulumi.Input[Union[str, 'BillingCycle']] billing_cycle: monthly or hourly
         :param pulumi.Input[str] custom_data: A string of the desired Custom Data for the device.  By default, changing this attribute will cause the provider to destroy and recreate your device.  If `reinstall` is specified or `behavior.allow_changes` includes `"custom_data"`, the device will be updated in-place instead of recreated.
         :param pulumi.Input[str] description: The device description.
-        :param pulumi.Input[Sequence[pulumi.Input[Union[str, 'Facility']]]] facilities: List of facility codes with deployment preferences. Equinix Metal API will go
-               through the list and will deploy your device to first facility with free capacity. List items must
-               be facility codes or `any` (a wildcard). To find the facility code, visit
-               [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth
-               token in the top of the page and see JSON from the API response. Conflicts with `metro`.
+        :param pulumi.Input[Sequence[pulumi.Input[Union[str, 'Facility']]]] facilities: List of facility codes with deployment preferences. Equinix Metal API will go through the list and will deploy your
+               device to first facility with free capacity. List items must be facility codes or any (a wildcard). To find the facility
+               code, visit [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth token in the
+               top of the page and see JSON from the API response. Conflicts with metro
         :param pulumi.Input[bool] force_detach_volumes: Delete device even if it has volumes attached. Only applies
                for destroy action.
         :param pulumi.Input[str] hardware_reservation_id: The UUID of the hardware reservation where you want this device deployed, or next-available if you want to pick your
                next available reservation automatically
         :param pulumi.Input[str] hostname: The device hostname used in deployments taking advantage of Layer3 DHCP
                or metadata service configuration.
         :param pulumi.Input[Sequence[pulumi.Input['DeviceIpAddressArgs']]] ip_addresses: A list of IP address types for the device. See
@@ -102,14 +101,17 @@
         if billing_cycle is not None:
             pulumi.set(__self__, "billing_cycle", billing_cycle)
         if custom_data is not None:
             pulumi.set(__self__, "custom_data", custom_data)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if facilities is not None:
+            warnings.warn("""Use metro instead of facilities.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facilities is deprecated: Use metro instead of facilities.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+        if facilities is not None:
             pulumi.set(__self__, "facilities", facilities)
         if force_detach_volumes is not None:
             pulumi.set(__self__, "force_detach_volumes", force_detach_volumes)
         if hardware_reservation_id is not None:
             pulumi.set(__self__, "hardware_reservation_id", hardware_reservation_id)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -237,19 +239,18 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def facilities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Union[str, 'Facility']]]]]:
         """
-        List of facility codes with deployment preferences. Equinix Metal API will go
-        through the list and will deploy your device to first facility with free capacity. List items must
-        be facility codes or `any` (a wildcard). To find the facility code, visit
-        [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth
-        token in the top of the page and see JSON from the API response. Conflicts with `metro`.
+        List of facility codes with deployment preferences. Equinix Metal API will go through the list and will deploy your
+        device to first facility with free capacity. List items must be facility codes or any (a wildcard). To find the facility
+        code, visit [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth token in the
+        top of the page and see JSON from the API response. Conflicts with metro
         """
         return pulumi.get(self, "facilities")
 
     @facilities.setter
     def facilities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Union[str, 'Facility']]]]]):
         pulumi.set(self, "facilities", value)
 
@@ -486,23 +487,22 @@
         :param pulumi.Input[str] access_public_ipv6: The ipv6 maintenance IP assigned to the device.
         :param pulumi.Input[bool] always_pxe: If true, a device with OS `custom_ipxe` will continue to boot via iPXE
                on reboots.
         :param pulumi.Input['DeviceBehaviorArgs'] behavior: Behavioral overrides that change how the resource handles certain attribute updates. See Behavior below for more details.
         :param pulumi.Input[Union[str, 'BillingCycle']] billing_cycle: monthly or hourly
         :param pulumi.Input[str] created: The timestamp for when the device was created.
         :param pulumi.Input[str] custom_data: A string of the desired Custom Data for the device.  By default, changing this attribute will cause the provider to destroy and recreate your device.  If `reinstall` is specified or `behavior.allow_changes` includes `"custom_data"`, the device will be updated in-place instead of recreated.
-        :param pulumi.Input[str] deployed_facility: The facility where the device is deployed.
+        :param pulumi.Input[str] deployed_facility: The facility where the device is deployed
         :param pulumi.Input[str] deployed_hardware_reservation_id: ID of hardware reservation where this device was deployed.
                It is useful when using the `next-available` hardware reservation.
         :param pulumi.Input[str] description: The device description.
-        :param pulumi.Input[Sequence[pulumi.Input[Union[str, 'Facility']]]] facilities: List of facility codes with deployment preferences. Equinix Metal API will go
-               through the list and will deploy your device to first facility with free capacity. List items must
-               be facility codes or `any` (a wildcard). To find the facility code, visit
-               [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth
-               token in the top of the page and see JSON from the API response. Conflicts with `metro`.
+        :param pulumi.Input[Sequence[pulumi.Input[Union[str, 'Facility']]]] facilities: List of facility codes with deployment preferences. Equinix Metal API will go through the list and will deploy your
+               device to first facility with free capacity. List items must be facility codes or any (a wildcard). To find the facility
+               code, visit [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth token in the
+               top of the page and see JSON from the API response. Conflicts with metro
         :param pulumi.Input[bool] force_detach_volumes: Delete device even if it has volumes attached. Only applies
                for destroy action.
         :param pulumi.Input[str] hardware_reservation_id: The UUID of the hardware reservation where you want this device deployed, or next-available if you want to pick your
                next available reservation automatically
         :param pulumi.Input[str] hostname: The device hostname used in deployments taking advantage of Layer3 DHCP
                or metadata service configuration.
         :param pulumi.Input[Sequence[pulumi.Input['DeviceIpAddressArgs']]] ip_addresses: A list of IP address types for the device. See
@@ -567,20 +567,26 @@
         if billing_cycle is not None:
             pulumi.set(__self__, "billing_cycle", billing_cycle)
         if created is not None:
             pulumi.set(__self__, "created", created)
         if custom_data is not None:
             pulumi.set(__self__, "custom_data", custom_data)
         if deployed_facility is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""deployed_facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+        if deployed_facility is not None:
             pulumi.set(__self__, "deployed_facility", deployed_facility)
         if deployed_hardware_reservation_id is not None:
             pulumi.set(__self__, "deployed_hardware_reservation_id", deployed_hardware_reservation_id)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if facilities is not None:
+            warnings.warn("""Use metro instead of facilities.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facilities is deprecated: Use metro instead of facilities.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+        if facilities is not None:
             pulumi.set(__self__, "facilities", facilities)
         if force_detach_volumes is not None:
             pulumi.set(__self__, "force_detach_volumes", force_detach_volumes)
         if hardware_reservation_id is not None:
             pulumi.set(__self__, "hardware_reservation_id", hardware_reservation_id)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -729,15 +735,15 @@
     def custom_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_data", value)
 
     @property
     @pulumi.getter(name="deployedFacility")
     def deployed_facility(self) -> Optional[pulumi.Input[str]]:
         """
-        The facility where the device is deployed.
+        The facility where the device is deployed
         """
         return pulumi.get(self, "deployed_facility")
 
     @deployed_facility.setter
     def deployed_facility(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "deployed_facility", value)
 
@@ -766,19 +772,18 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def facilities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Union[str, 'Facility']]]]]:
         """
-        List of facility codes with deployment preferences. Equinix Metal API will go
-        through the list and will deploy your device to first facility with free capacity. List items must
-        be facility codes or `any` (a wildcard). To find the facility code, visit
-        [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth
-        token in the top of the page and see JSON from the API response. Conflicts with `metro`.
+        List of facility codes with deployment preferences. Equinix Metal API will go through the list and will deploy your
+        device to first facility with free capacity. List items must be facility codes or any (a wildcard). To find the facility
+        code, visit [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth token in the
+        top of the page and see JSON from the API response. Conflicts with metro
         """
         return pulumi.get(self, "facilities")
 
     @facilities.setter
     def facilities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Union[str, 'Facility']]]]]):
         pulumi.set(self, "facilities", value)
 
@@ -1174,19 +1179,18 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] always_pxe: If true, a device with OS `custom_ipxe` will continue to boot via iPXE
                on reboots.
         :param pulumi.Input[pulumi.InputType['DeviceBehaviorArgs']] behavior: Behavioral overrides that change how the resource handles certain attribute updates. See Behavior below for more details.
         :param pulumi.Input[Union[str, 'BillingCycle']] billing_cycle: monthly or hourly
         :param pulumi.Input[str] custom_data: A string of the desired Custom Data for the device.  By default, changing this attribute will cause the provider to destroy and recreate your device.  If `reinstall` is specified or `behavior.allow_changes` includes `"custom_data"`, the device will be updated in-place instead of recreated.
         :param pulumi.Input[str] description: The device description.
-        :param pulumi.Input[Sequence[pulumi.Input[Union[str, 'Facility']]]] facilities: List of facility codes with deployment preferences. Equinix Metal API will go
-               through the list and will deploy your device to first facility with free capacity. List items must
-               be facility codes or `any` (a wildcard). To find the facility code, visit
-               [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth
-               token in the top of the page and see JSON from the API response. Conflicts with `metro`.
+        :param pulumi.Input[Sequence[pulumi.Input[Union[str, 'Facility']]]] facilities: List of facility codes with deployment preferences. Equinix Metal API will go through the list and will deploy your
+               device to first facility with free capacity. List items must be facility codes or any (a wildcard). To find the facility
+               code, visit [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth token in the
+               top of the page and see JSON from the API response. Conflicts with metro
         :param pulumi.Input[bool] force_detach_volumes: Delete device even if it has volumes attached. Only applies
                for destroy action.
         :param pulumi.Input[str] hardware_reservation_id: The UUID of the hardware reservation where you want this device deployed, or next-available if you want to pick your
                next available reservation automatically
         :param pulumi.Input[str] hostname: The device hostname used in deployments taking advantage of Layer3 DHCP
                or metadata service configuration.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceIpAddressArgs']]]] ip_addresses: A list of IP address types for the device. See
@@ -1305,14 +1309,17 @@
             __props__ = DeviceArgs.__new__(DeviceArgs)
 
             __props__.__dict__["always_pxe"] = always_pxe
             __props__.__dict__["behavior"] = behavior
             __props__.__dict__["billing_cycle"] = billing_cycle
             __props__.__dict__["custom_data"] = None if custom_data is None else pulumi.Output.secret(custom_data)
             __props__.__dict__["description"] = description
+            if facilities is not None and not opts.urn:
+                warnings.warn("""Use metro instead of facilities.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+                pulumi.log.warn("""facilities is deprecated: Use metro instead of facilities.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
             __props__.__dict__["facilities"] = facilities
             __props__.__dict__["force_detach_volumes"] = force_detach_volumes
             __props__.__dict__["hardware_reservation_id"] = hardware_reservation_id
             __props__.__dict__["hostname"] = hostname
             __props__.__dict__["ip_addresses"] = ip_addresses
             __props__.__dict__["ipxe_script_url"] = ipxe_script_url
             __props__.__dict__["metro"] = metro
@@ -1408,23 +1415,22 @@
         :param pulumi.Input[str] access_public_ipv6: The ipv6 maintenance IP assigned to the device.
         :param pulumi.Input[bool] always_pxe: If true, a device with OS `custom_ipxe` will continue to boot via iPXE
                on reboots.
         :param pulumi.Input[pulumi.InputType['DeviceBehaviorArgs']] behavior: Behavioral overrides that change how the resource handles certain attribute updates. See Behavior below for more details.
         :param pulumi.Input[Union[str, 'BillingCycle']] billing_cycle: monthly or hourly
         :param pulumi.Input[str] created: The timestamp for when the device was created.
         :param pulumi.Input[str] custom_data: A string of the desired Custom Data for the device.  By default, changing this attribute will cause the provider to destroy and recreate your device.  If `reinstall` is specified or `behavior.allow_changes` includes `"custom_data"`, the device will be updated in-place instead of recreated.
-        :param pulumi.Input[str] deployed_facility: The facility where the device is deployed.
+        :param pulumi.Input[str] deployed_facility: The facility where the device is deployed
         :param pulumi.Input[str] deployed_hardware_reservation_id: ID of hardware reservation where this device was deployed.
                It is useful when using the `next-available` hardware reservation.
         :param pulumi.Input[str] description: The device description.
-        :param pulumi.Input[Sequence[pulumi.Input[Union[str, 'Facility']]]] facilities: List of facility codes with deployment preferences. Equinix Metal API will go
-               through the list and will deploy your device to first facility with free capacity. List items must
-               be facility codes or `any` (a wildcard). To find the facility code, visit
-               [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth
-               token in the top of the page and see JSON from the API response. Conflicts with `metro`.
+        :param pulumi.Input[Sequence[pulumi.Input[Union[str, 'Facility']]]] facilities: List of facility codes with deployment preferences. Equinix Metal API will go through the list and will deploy your
+               device to first facility with free capacity. List items must be facility codes or any (a wildcard). To find the facility
+               code, visit [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth token in the
+               top of the page and see JSON from the API response. Conflicts with metro
         :param pulumi.Input[bool] force_detach_volumes: Delete device even if it has volumes attached. Only applies
                for destroy action.
         :param pulumi.Input[str] hardware_reservation_id: The UUID of the hardware reservation where you want this device deployed, or next-available if you want to pick your
                next available reservation automatically
         :param pulumi.Input[str] hostname: The device hostname used in deployments taking advantage of Layer3 DHCP
                or metadata service configuration.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceIpAddressArgs']]]] ip_addresses: A list of IP address types for the device. See
@@ -1584,15 +1590,15 @@
         """
         return pulumi.get(self, "custom_data")
 
     @property
     @pulumi.getter(name="deployedFacility")
     def deployed_facility(self) -> pulumi.Output[str]:
         """
-        The facility where the device is deployed.
+        The facility where the device is deployed
         """
         return pulumi.get(self, "deployed_facility")
 
     @property
     @pulumi.getter(name="deployedHardwareReservationId")
     def deployed_hardware_reservation_id(self) -> pulumi.Output[str]:
         """
@@ -1609,19 +1615,18 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def facilities(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of facility codes with deployment preferences. Equinix Metal API will go
-        through the list and will deploy your device to first facility with free capacity. List items must
-        be facility codes or `any` (a wildcard). To find the facility code, visit
-        [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth
-        token in the top of the page and see JSON from the API response. Conflicts with `metro`.
+        List of facility codes with deployment preferences. Equinix Metal API will go through the list and will deploy your
+        device to first facility with free capacity. List items must be facility codes or any (a wildcard). To find the facility
+        code, visit [Facilities API docs](https://metal.equinix.com/developers/api/facilities/), set your API auth token in the
+        top of the page and see JSON from the API response. Conflicts with metro
         """
         return pulumi.get(self, "facilities")
 
     @property
     @pulumi.getter(name="forceDetachVolumes")
     def force_detach_volumes(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/device_network_type.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/device_network_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/gateway.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_device.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_device.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
         if device_id and not isinstance(device_id, str):
             raise TypeError("Expected argument 'device_id' to be a str")
         pulumi.set(__self__, "device_id", device_id)
         if facility and not isinstance(facility, str):
             raise TypeError("Expected argument 'facility' to be a str")
+        if facility is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+
         pulumi.set(__self__, "facility", facility)
         if hardware_reservation_id and not isinstance(hardware_reservation_id, str):
             raise TypeError("Expected argument 'hardware_reservation_id' to be a str")
         pulumi.set(__self__, "hardware_reservation_id", hardware_reservation_id)
         if hostname and not isinstance(hostname, str):
             raise TypeError("Expected argument 'hostname' to be a str")
         pulumi.set(__self__, "hostname", hostname)
@@ -145,17 +149,14 @@
     @pulumi.getter(name="deviceId")
     def device_id(self) -> str:
         return pulumi.get(self, "device_id")
 
     @property
     @pulumi.getter
     def facility(self) -> str:
-        """
-        The facility where the device is deployed.
-        """
         return pulumi.get(self, "facility")
 
     @property
     @pulumi.getter(name="hardwareReservationId")
     def hardware_reservation_id(self) -> str:
         """
         The id of hardware reservation which this device occupies.
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_device_bgp_neighbors.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_device_bgp_neighbors.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_facility.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_facility.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,16 +110,15 @@
 
 
 def get_facility(capacities: Optional[Sequence[pulumi.InputType['GetFacilityCapacityArgs']]] = None,
                  code: Optional[str] = None,
                  features_requireds: Optional[Sequence[str]] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFacilityResult:
     """
-    Provides an Equinix Metal facility datasource.
-
+    Use this data source to access information about an existing resource.
 
     :param Sequence[pulumi.InputType['GetFacilityCapacityArgs']] capacities: One or more device plans for which the facility must have capacity.
     :param str code: The facility code to search for facilities.
     :param Sequence[str] features_requireds: Set of feature strings that the facility must have. Some
            possible values are `baremetal`, `ibx`, `storage`, `global_ipv4`, `backend_transfer`, `layer_2`.
     """
     __args__ = dict()
@@ -141,16 +140,15 @@
 
 @_utilities.lift_output_func(get_facility)
 def get_facility_output(capacities: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetFacilityCapacityArgs']]]]] = None,
                         code: Optional[pulumi.Input[str]] = None,
                         features_requireds: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFacilityResult]:
     """
-    Provides an Equinix Metal facility datasource.
-
+    Use this data source to access information about an existing resource.
 
     :param Sequence[pulumi.InputType['GetFacilityCapacityArgs']] capacities: One or more device plans for which the facility must have capacity.
     :param str code: The facility code to search for facilities.
     :param Sequence[str] features_requireds: Set of feature strings that the facility must have. Some
            possible values are `baremetal`, `ibx`, `storage`, `global_ipv4`, `backend_transfer`, `layer_2`.
     """
     ...
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_gateway.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_hardware_reservation.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_hardware_reservation.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     """
     def __init__(__self__, device_id=None, facility=None, id=None, plan=None, project_id=None, provisionable=None, short_id=None, spare=None, switch_uuid=None):
         if device_id and not isinstance(device_id, str):
             raise TypeError("Expected argument 'device_id' to be a str")
         pulumi.set(__self__, "device_id", device_id)
         if facility and not isinstance(facility, str):
             raise TypeError("Expected argument 'facility' to be a str")
+        if facility is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+
         pulumi.set(__self__, "facility", facility)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if plan and not isinstance(plan, str):
             raise TypeError("Expected argument 'plan' to be a str")
         pulumi.set(__self__, "plan", plan)
@@ -57,17 +61,14 @@
         UUID of device occupying the reservation.
         """
         return pulumi.get(self, "device_id")
 
     @property
     @pulumi.getter
     def facility(self) -> str:
-        """
-        Plan type for the reservation.
-        """
         return pulumi.get(self, "facility")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         ID of the hardware reservation to look up.
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_interconnection.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_interconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,18 @@
             raise TypeError("Expected argument 'connection_id' to be a str")
         pulumi.set(__self__, "connection_id", connection_id)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
         if facility and not isinstance(facility, str):
             raise TypeError("Expected argument 'facility' to be a str")
+        if facility is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+
         pulumi.set(__self__, "facility", facility)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if metro and not isinstance(metro, str):
             raise TypeError("Expected argument 'metro' to be a str")
         pulumi.set(__self__, "metro", metro)
@@ -97,17 +101,14 @@
         Description of the connection resource.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def facility(self) -> str:
-        """
-        Slug of a facility to which the connection belongs.
-        """
         return pulumi.get(self, "facility")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_ip_block_ranges.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_ip_block_ranges.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 class GetIpBlockRangesResult:
     """
     A collection of values returned by getIpBlockRanges.
     """
     def __init__(__self__, facility=None, global_ipv4s=None, id=None, ipv6s=None, metro=None, private_ipv4s=None, project_id=None, public_ipv4s=None):
         if facility and not isinstance(facility, str):
             raise TypeError("Expected argument 'facility' to be a str")
+        if facility is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+
         pulumi.set(__self__, "facility", facility)
         if global_ipv4s and not isinstance(global_ipv4s, list):
             raise TypeError("Expected argument 'global_ipv4s' to be a list")
         pulumi.set(__self__, "global_ipv4s", global_ipv4s)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
@@ -138,16 +142,14 @@
 
     project_id = "<UUID_of_your_project>"
     test = equinix.metal.get_ip_block_ranges(project_id=project_id)
     pulumi.export("out", test)
     ```
 
 
-    :param str facility: Facility code filtering the IP blocks. Global IPv4 blocks will be listed
-           anyway. If you omit this and metro, all the block from the project will be listed.
     :param str metro: Metro code filtering the IP blocks. Global IPv4 blocks will be listed
            anyway. If you omit this and facility, all the block from the project will be listed.
     :param str project_id: ID of the project from which to list the blocks.
     """
     __args__ = dict()
     __args__['facility'] = facility
     __args__['metro'] = metro
@@ -186,14 +188,12 @@
 
     project_id = "<UUID_of_your_project>"
     test = equinix.metal.get_ip_block_ranges(project_id=project_id)
     pulumi.export("out", test)
     ```
 
 
-    :param str facility: Facility code filtering the IP blocks. Global IPv4 blocks will be listed
-           anyway. If you omit this and metro, all the block from the project will be listed.
     :param str metro: Metro code filtering the IP blocks. Global IPv4 blocks will be listed
            anyway. If you omit this and facility, all the block from the project will be listed.
     :param str project_id: ID of the project from which to list the blocks.
     """
     ...
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_metro.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_metro.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,16 +91,16 @@
 def get_metro(capacities: Optional[Sequence[pulumi.InputType['GetMetroCapacityArgs']]] = None,
               code: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMetroResult:
     """
     Provides an Equinix Metal metro datasource.
 
 
-    :param Sequence[pulumi.InputType['GetMetroCapacityArgs']] capacities: One or more device plans for which the facility must have capacity.
-    :param str code: The facility code to search for facilities.
+    :param Sequence[pulumi.InputType['GetMetroCapacityArgs']] capacities: One or more device plans for which the metro must have capacity.
+    :param str code: The metro code to search for.
     """
     __args__ = dict()
     __args__['capacities'] = capacities
     __args__['code'] = code
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('equinix:metal/getMetro:getMetro', __args__, opts=opts, typ=GetMetroResult).value
 
@@ -116,11 +116,11 @@
 def get_metro_output(capacities: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetMetroCapacityArgs']]]]] = None,
                      code: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMetroResult]:
     """
     Provides an Equinix Metal metro datasource.
 
 
-    :param Sequence[pulumi.InputType['GetMetroCapacityArgs']] capacities: One or more device plans for which the facility must have capacity.
-    :param str code: The facility code to search for facilities.
+    :param Sequence[pulumi.InputType['GetMetroCapacityArgs']] capacities: One or more device plans for which the metro must have capacity.
+    :param str code: The metro code to search for.
     """
     ...
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_operating_system.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_operating_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     example = equinix.metal.get_operating_system(distro="ubuntu",
         version="20.04",
         provisionable_on="c3.medium.x86")
     server = equinix.metal.Device("server",
         hostname="tf.ubuntu",
         plan="c3.medium.x86",
-        facilities=["ny5"],
+        metro="ny",
         operating_system=example.id.apply(lambda x: equinix.metal/operatingsystem.OperatingSystem(x)),
         billing_cycle="hourly",
         project_id=local["project_id"])
     ```
 
 
     :param str distro: Name of the OS distribution.
@@ -158,15 +158,15 @@
 
     example = equinix.metal.get_operating_system(distro="ubuntu",
         version="20.04",
         provisionable_on="c3.medium.x86")
     server = equinix.metal.Device("server",
         hostname="tf.ubuntu",
         plan="c3.medium.x86",
-        facilities=["ny5"],
+        metro="ny",
         operating_system=example.id.apply(lambda x: equinix.metal/operatingsystem.OperatingSystem(x)),
         billing_cycle="hourly",
         project_id=local["project_id"])
     ```
 
 
     :param str distro: Name of the OS distribution.
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_organization.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_plans.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_plans.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,17 +49,14 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def plans(self) -> Sequence['outputs.GetPlansPlanResult']:
-        """
-        The ID of the facility
-        """
         return pulumi.get(self, "plans")
 
     @property
     @pulumi.getter
     def sorts(self) -> Optional[Sequence['outputs.GetPlansSortResult']]:
         return pulumi.get(self, "sorts")
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_port.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_port.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
     import pulumi
     import pulumi_equinix as equinix
 
     project_id = "<UUID_of_your_project>"
     test_device = equinix.metal.Device("testDevice",
         hostname="tfacc-test-device-port",
         plan="c3.medium.x86",
-        facilities=["sv15"],
+        metro="sv",
         operating_system="ubuntu_20_04",
         billing_cycle="hourly",
         project_id=project_id)
     test_port = equinix.metal.get_port_output(device_id=test_device.id,
         name="eth0")
     ```
 
@@ -275,15 +275,15 @@
     import pulumi
     import pulumi_equinix as equinix
 
     project_id = "<UUID_of_your_project>"
     test_device = equinix.metal.Device("testDevice",
         hostname="tfacc-test-device-port",
         plan="c3.medium.x86",
-        facilities=["sv15"],
+        metro="sv",
         operating_system="ubuntu_20_04",
         billing_cycle="hourly",
         project_id=project_id)
     test_port = equinix.metal.get_port_output(device_id=test_device.id,
         name="eth0")
     ```
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_precreated_ip_block.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_precreated_ip_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,14 @@
 
     > Precreated (management) IP blocks for a metro will not be available until first device is created in that metro.
 
     > Public IPv4 blocks auto-assigned (management) to a device cannot be retrieved. If you need that information, consider using the metal.Device data source instead.
 
 
     :param int address_family: 4 or 6, depending on which block you are looking for.
-    :param str facility: Facility of the searched block. (for non-global blocks).
     :param bool global_: Whether to look for global block. Default is false for backward compatibility.
     :param str metro: Metro of the searched block (for non-global blocks).
     :param str project_id: ID of the project where the searched block should be.
     :param bool public: Whether to look for public or private block.
     """
     __args__ = dict()
     __args__['addressFamily'] = address_family
@@ -272,14 +271,13 @@
 
     > Precreated (management) IP blocks for a metro will not be available until first device is created in that metro.
 
     > Public IPv4 blocks auto-assigned (management) to a device cannot be retrieved. If you need that information, consider using the metal.Device data source instead.
 
 
     :param int address_family: 4 or 6, depending on which block you are looking for.
-    :param str facility: Facility of the searched block. (for non-global blocks).
     :param bool global_: Whether to look for global block. Default is false for backward compatibility.
     :param str metro: Metro of the searched block (for non-global blocks).
     :param str project_id: ID of the project where the searched block should be.
     :param bool public: Whether to look for public or private block.
     """
     ...
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_project.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_project_ssh_key.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_project_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_reserved_ip_block.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_reserved_ip_block.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,18 @@
             raise TypeError("Expected argument 'cidr' to be a int")
         pulumi.set(__self__, "cidr", cidr)
         if cidr_notation and not isinstance(cidr_notation, str):
             raise TypeError("Expected argument 'cidr_notation' to be a str")
         pulumi.set(__self__, "cidr_notation", cidr_notation)
         if facility and not isinstance(facility, str):
             raise TypeError("Expected argument 'facility' to be a str")
+        if facility is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+
         pulumi.set(__self__, "facility", facility)
         if gateway and not isinstance(gateway, str):
             raise TypeError("Expected argument 'gateway' to be a str")
         pulumi.set(__self__, "gateway", gateway)
         if global_ and not isinstance(global_, bool):
             raise TypeError("Expected argument 'global_' to be a bool")
         pulumi.set(__self__, "global_", global_)
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_spot_market_price.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_spot_market_price.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 class GetSpotMarketPriceResult:
     """
     A collection of values returned by getSpotMarketPrice.
     """
     def __init__(__self__, facility=None, id=None, metro=None, plan=None, price=None):
         if facility and not isinstance(facility, str):
             raise TypeError("Expected argument 'facility' to be a str")
+        if facility is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+
         pulumi.set(__self__, "facility", facility)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if metro and not isinstance(metro, str):
             raise TypeError("Expected argument 'metro' to be a str")
         pulumi.set(__self__, "metro", metro)
@@ -88,36 +92,25 @@
                           plan: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSpotMarketPriceResult:
     """
     Use this data source to get Equinix Metal Spot Market Price for a plan.
 
     ## Example Usage
 
-    Lookup by facility:
-
-    ```python
-    import pulumi
-    import pulumi_equinix as equinix
-
-    example = equinix.metal.get_spot_market_price(facility="ny5",
-        plan="c3.small.x86")
-    ```
-
     Lookup by metro:
 
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_spot_market_price(metro="sv",
         plan="c3.small.x86")
     ```
 
 
-    :param str facility: Name of the facility.
     :param str metro: Name of the metro.
     :param str plan: Name of the plan.
     """
     __args__ = dict()
     __args__['facility'] = facility
     __args__['metro'] = metro
     __args__['plan'] = plan
@@ -138,33 +131,22 @@
                                  plan: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSpotMarketPriceResult]:
     """
     Use this data source to get Equinix Metal Spot Market Price for a plan.
 
     ## Example Usage
 
-    Lookup by facility:
-
-    ```python
-    import pulumi
-    import pulumi_equinix as equinix
-
-    example = equinix.metal.get_spot_market_price(facility="ny5",
-        plan="c3.small.x86")
-    ```
-
     Lookup by metro:
 
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_spot_market_price(metro="sv",
         plan="c3.small.x86")
     ```
 
 
-    :param str facility: Name of the facility.
     :param str metro: Name of the metro.
     :param str plan: Name of the plan.
     """
     ...
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_spot_market_request.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_spot_market_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,18 @@
             raise TypeError("Expected argument 'devices_min' to be a int")
         pulumi.set(__self__, "devices_min", devices_min)
         if end_at and not isinstance(end_at, str):
             raise TypeError("Expected argument 'end_at' to be a str")
         pulumi.set(__self__, "end_at", end_at)
         if facilities and not isinstance(facilities, list):
             raise TypeError("Expected argument 'facilities' to be a list")
+        if facilities is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facilities is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+
         pulumi.set(__self__, "facilities", facilities)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if max_bid_price and not isinstance(max_bid_price, float):
             raise TypeError("Expected argument 'max_bid_price' to be a float")
         pulumi.set(__self__, "max_bid_price", max_bid_price)
@@ -87,17 +91,14 @@
         Date and time When the spot market request will be ended.
         """
         return pulumi.get(self, "end_at")
 
     @property
     @pulumi.getter
     def facilities(self) -> Sequence[str]:
-        """
-        Facility IDs where devices should be created.
-        """
         return pulumi.get(self, "facilities")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_virtual_circuit.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_vlan.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_vlan.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,14 +26,18 @@
             raise TypeError("Expected argument 'assigned_devices_ids' to be a list")
         pulumi.set(__self__, "assigned_devices_ids", assigned_devices_ids)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
         if facility and not isinstance(facility, str):
             raise TypeError("Expected argument 'facility' to be a str")
+        if facility is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+
         pulumi.set(__self__, "facility", facility)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if metro and not isinstance(metro, str):
             raise TypeError("Expected argument 'metro' to be a str")
         pulumi.set(__self__, "metro", metro)
@@ -146,15 +150,15 @@
 
     dsvlan = equinix.metal.get_vlan(project_id=local["project_id"],
         vxlan=5,
         metro="sv")
     ```
 
 
-    :param str facility: Facility where the VLAN is deployed.
+    :param str facility: Facility where the VLAN is deployed. Deprecated, see https://feedback.equinixmetal.com/changelog/bye-facilities-hello-again-metros
     :param str metro: Metro where the VLAN is deployed.
     :param str project_id: UUID of parent project of the VLAN. Use together with the vxlan number and metro or facility.
     :param str vlan_id: Metal UUID of the VLAN resource to look up.
     :param int vxlan: vxlan number of the VLAN to look up. Use together with the project_id and metro or facility.
     """
     __args__ = dict()
     __args__['facility'] = facility
@@ -210,14 +214,14 @@
 
     dsvlan = equinix.metal.get_vlan(project_id=local["project_id"],
         vxlan=5,
         metro="sv")
     ```
 
 
-    :param str facility: Facility where the VLAN is deployed.
+    :param str facility: Facility where the VLAN is deployed. Deprecated, see https://feedback.equinixmetal.com/changelog/bye-facilities-hello-again-metros
     :param str metro: Metro where the VLAN is deployed.
     :param str project_id: UUID of parent project of the VLAN. Use together with the vxlan number and metro or facility.
     :param str vlan_id: Metal UUID of the VLAN resource to look up.
     :param int vxlan: vxlan number of the VLAN to look up. Use together with the project_id and metro or facility.
     """
     ...
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/get_vrf.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/get_vrf.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/interconnection.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/interconnection.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                  vlans: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None):
         """
         The set of arguments for constructing a Interconnection resource.
         :param pulumi.Input[str] redundancy: Connection redundancy - redundant or primary.
         :param pulumi.Input[str] speed: Connection speed - one of 50Mbps, 200Mbps, 500Mbps, 1Gbps, 2Gbps, 5Gbps, 10Gbps.
         :param pulumi.Input[str] type: Connection type - dedicated or shared.
         :param pulumi.Input[str] description: Description for the connection resource.
-        :param pulumi.Input[str] facility: Facility where the connection will be created.
+        :param pulumi.Input[str] facility: Facility where the connection will be created
         :param pulumi.Input[str] metro: Metro where the connection will be created.
         :param pulumi.Input[str] mode: Mode for connections in IBX facilities with the dedicated type - standard or tunnel. Default is standard.
         :param pulumi.Input[str] name: Name of the connection resource
         :param pulumi.Input[str] organization_id: ID of the organization where the connection is scoped to.
         :param pulumi.Input[str] project_id: ID of the project where the connection is scoped to, must be set for.
         :param pulumi.Input[str] service_token_type: Only used with shared connection. Type of service token to use for the connection, a_side or z_side
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: String list of tags.
@@ -47,14 +47,17 @@
         """
         pulumi.set(__self__, "redundancy", redundancy)
         pulumi.set(__self__, "speed", speed)
         pulumi.set(__self__, "type", type)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if facility is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+        if facility is not None:
             pulumi.set(__self__, "facility", facility)
         if metro is not None:
             pulumi.set(__self__, "metro", metro)
         if mode is not None:
             pulumi.set(__self__, "mode", mode)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -117,15 +120,15 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def facility(self) -> Optional[pulumi.Input[str]]:
         """
-        Facility where the connection will be created.
+        Facility where the connection will be created
         """
         return pulumi.get(self, "facility")
 
     @facility.setter
     def facility(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "facility", value)
 
@@ -245,15 +248,15 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  token: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  vlans: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None):
         """
         Input properties used for looking up and filtering Interconnection resources.
         :param pulumi.Input[str] description: Description for the connection resource.
-        :param pulumi.Input[str] facility: Facility where the connection will be created.
+        :param pulumi.Input[str] facility: Facility where the connection will be created
         :param pulumi.Input[str] metro: Metro where the connection will be created.
         :param pulumi.Input[str] mode: Mode for connections in IBX facilities with the dedicated type - standard or tunnel. Default is standard.
         :param pulumi.Input[str] name: Name of the connection resource
         :param pulumi.Input[str] organization_id: ID of the organization where the connection is scoped to.
         :param pulumi.Input[Sequence[pulumi.Input['InterconnectionPortArgs']]] ports: List of connection ports - primary (`ports[0]`) and secondary (`ports[1]`). Schema of
                port is described in documentation of the
                metal.Interconnection datasource.
@@ -267,14 +270,17 @@
         :param pulumi.Input[str] token: (Deprecated) Fabric Token required to configure the connection in Equinix Fabric with the equinix_ecx_l2_connection resource or from the [Equinix Fabric Portal](https://ecxfabric.equinix.com/dashboard). If your organization already has connection service tokens enabled, use `service_tokens` instead.
         :param pulumi.Input[str] type: Connection type - dedicated or shared.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] vlans: Only used with shared connection. Vlans to attach. Pass one vlan for Primary/Single connection and two vlans for Redundant connection.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if facility is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+        if facility is not None:
             pulumi.set(__self__, "facility", facility)
         if metro is not None:
             pulumi.set(__self__, "metro", metro)
         if mode is not None:
             pulumi.set(__self__, "mode", mode)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -318,15 +324,15 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def facility(self) -> Optional[pulumi.Input[str]]:
         """
-        Facility where the connection will be created.
+        Facility where the connection will be created
         """
         return pulumi.get(self, "facility")
 
     @facility.setter
     def facility(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "facility", value)
 
@@ -561,15 +567,15 @@
         pulumi.export("connectionStatus", connection.status)
         pulumi.export("connectionTokens", connection.service_tokens)
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description for the connection resource.
-        :param pulumi.Input[str] facility: Facility where the connection will be created.
+        :param pulumi.Input[str] facility: Facility where the connection will be created
         :param pulumi.Input[str] metro: Metro where the connection will be created.
         :param pulumi.Input[str] mode: Mode for connections in IBX facilities with the dedicated type - standard or tunnel. Default is standard.
         :param pulumi.Input[str] name: Name of the connection resource
         :param pulumi.Input[str] organization_id: ID of the organization where the connection is scoped to.
         :param pulumi.Input[str] project_id: ID of the project where the connection is scoped to, must be set for.
         :param pulumi.Input[str] redundancy: Connection redundancy - redundant or primary.
         :param pulumi.Input[str] service_token_type: Only used with shared connection. Type of service token to use for the connection, a_side or z_side
@@ -648,14 +654,17 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InterconnectionArgs.__new__(InterconnectionArgs)
 
             __props__.__dict__["description"] = description
+            if facility is not None and not opts.urn:
+                warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+                pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
             __props__.__dict__["facility"] = facility
             __props__.__dict__["metro"] = metro
             __props__.__dict__["mode"] = mode
             __props__.__dict__["name"] = name
             __props__.__dict__["organization_id"] = organization_id
             __props__.__dict__["project_id"] = project_id
             if redundancy is None and not opts.urn:
@@ -705,15 +714,15 @@
         Get an existing Interconnection resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description for the connection resource.
-        :param pulumi.Input[str] facility: Facility where the connection will be created.
+        :param pulumi.Input[str] facility: Facility where the connection will be created
         :param pulumi.Input[str] metro: Metro where the connection will be created.
         :param pulumi.Input[str] mode: Mode for connections in IBX facilities with the dedicated type - standard or tunnel. Default is standard.
         :param pulumi.Input[str] name: Name of the connection resource
         :param pulumi.Input[str] organization_id: ID of the organization where the connection is scoped to.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InterconnectionPortArgs']]]] ports: List of connection ports - primary (`ports[0]`) and secondary (`ports[1]`). Schema of
                port is described in documentation of the
                metal.Interconnection datasource.
@@ -759,15 +768,15 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def facility(self) -> pulumi.Output[str]:
         """
-        Facility where the connection will be created.
+        Facility where the connection will be created
         """
         return pulumi.get(self, "facility")
 
     @property
     @pulumi.getter
     def metro(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/ip_attachment.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/ip_attachment.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 class IpAttachmentArgs:
     def __init__(__self__, *,
                  cidr_notation: pulumi.Input[str],
                  device_id: pulumi.Input[str]):
         """
         The set of arguments for constructing a IpAttachment resource.
         :param pulumi.Input[str] cidr_notation: CIDR notation of subnet from block reserved in the same project
-               and facility as the device.
+               and metro as the device.
         :param pulumi.Input[str] device_id: ID of device to which to assign the subnet.
         """
         pulumi.set(__self__, "cidr_notation", cidr_notation)
         pulumi.set(__self__, "device_id", device_id)
 
     @property
     @pulumi.getter(name="cidrNotation")
     def cidr_notation(self) -> pulumi.Input[str]:
         """
         CIDR notation of subnet from block reserved in the same project
-        and facility as the device.
+        and metro as the device.
         """
         return pulumi.get(self, "cidr_notation")
 
     @cidr_notation.setter
     def cidr_notation(self, value: pulumi.Input[str]):
         pulumi.set(self, "cidr_notation", value)
 
@@ -68,15 +68,15 @@
                  public: Optional[pulumi.Input[bool]] = None,
                  vrf_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering IpAttachment resources.
         :param pulumi.Input[int] address_family: Address family as integer. One of `4` or `6`.
         :param pulumi.Input[int] cidr: Length of CIDR prefix of the subnet as integer.
         :param pulumi.Input[str] cidr_notation: CIDR notation of subnet from block reserved in the same project
-               and facility as the device.
+               and metro as the device.
         :param pulumi.Input[str] device_id: ID of device to which to assign the subnet.
         :param pulumi.Input[str] gateway: IP address of gateway for the subnet.
         :param pulumi.Input[bool] global_: Flag indicating whether IP block is global, i.e. assignable in any location
         :param pulumi.Input[str] netmask: Subnet mask in decimal notation, e.g., `255.255.255.0`.
         :param pulumi.Input[str] network: Subnet network address.
         :param pulumi.Input[bool] public: Boolean flag whether subnet is reachable from the Internet.
         """
@@ -141,15 +141,15 @@
         pulumi.set(self, "cidr", value)
 
     @property
     @pulumi.getter(name="cidrNotation")
     def cidr_notation(self) -> Optional[pulumi.Input[str]]:
         """
         CIDR notation of subnet from block reserved in the same project
-        and facility as the device.
+        and metro as the device.
         """
         return pulumi.get(self, "cidr_notation")
 
     @cidr_notation.setter
     def cidr_notation(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cidr_notation", value)
 
@@ -261,22 +261,22 @@
                  cidr_notation: Optional[pulumi.Input[str]] = None,
                  device_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a resource to attach elastic IP subnets to devices.
 
         To attach an IP subnet from a reserved block to a provisioned device, you must derive a subnet CIDR
-        belonging to one of your reserved blocks in the same project and facility as the target device.
+        belonging to one of your reserved blocks in the same project and metro as the target device.
 
         For example, you have reserved IPv4 address block `147.229.10.152/30`, you can choose to assign
         either the whole block as one subnet to a device; or 2 subnets with CIDRs `147.229.10.152/31` and
         `147.229.10.154/31`; or 4 subnets with mask prefix length `32`. More about the elastic IP subnets
         is [here](https://metal.equinix.com/developers/docs/networking/elastic-ips/).
 
-        Device and reserved block must be in the same facility.
+        Device and reserved block must be in the same metro.
 
         ## Example Usage
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         config = pulumi.Config()
@@ -290,35 +290,35 @@
         pulumi.export("ipAttach", ip_attach_resource.id)
         pulumi.export("ipNetmask", ip_attach_resource.netmask)
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cidr_notation: CIDR notation of subnet from block reserved in the same project
-               and facility as the device.
+               and metro as the device.
         :param pulumi.Input[str] device_id: ID of device to which to assign the subnet.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IpAttachmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a resource to attach elastic IP subnets to devices.
 
         To attach an IP subnet from a reserved block to a provisioned device, you must derive a subnet CIDR
-        belonging to one of your reserved blocks in the same project and facility as the target device.
+        belonging to one of your reserved blocks in the same project and metro as the target device.
 
         For example, you have reserved IPv4 address block `147.229.10.152/30`, you can choose to assign
         either the whole block as one subnet to a device; or 2 subnets with CIDRs `147.229.10.152/31` and
         `147.229.10.154/31`; or 4 subnets with mask prefix length `32`. More about the elastic IP subnets
         is [here](https://metal.equinix.com/developers/docs/networking/elastic-ips/).
 
-        Device and reserved block must be in the same facility.
+        Device and reserved block must be in the same metro.
 
         ## Example Usage
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         config = pulumi.Config()
@@ -405,15 +405,15 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] address_family: Address family as integer. One of `4` or `6`.
         :param pulumi.Input[int] cidr: Length of CIDR prefix of the subnet as integer.
         :param pulumi.Input[str] cidr_notation: CIDR notation of subnet from block reserved in the same project
-               and facility as the device.
+               and metro as the device.
         :param pulumi.Input[str] device_id: ID of device to which to assign the subnet.
         :param pulumi.Input[str] gateway: IP address of gateway for the subnet.
         :param pulumi.Input[bool] global_: Flag indicating whether IP block is global, i.e. assignable in any location
         :param pulumi.Input[str] netmask: Subnet mask in decimal notation, e.g., `255.255.255.0`.
         :param pulumi.Input[str] network: Subnet network address.
         :param pulumi.Input[bool] public: Boolean flag whether subnet is reachable from the Internet.
         """
@@ -458,15 +458,15 @@
         return pulumi.get(self, "cidr")
 
     @property
     @pulumi.getter(name="cidrNotation")
     def cidr_notation(self) -> pulumi.Output[str]:
         """
         CIDR notation of subnet from block reserved in the same project
-        and facility as the device.
+        and metro as the device.
         """
         return pulumi.get(self, "cidr_notation")
 
     @property
     @pulumi.getter(name="deviceId")
     def device_id(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/organization.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/organization_member.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/organization_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/outputs.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -614,16 +614,16 @@
                  asn: int,
                  deployment_type: str,
                  max_prefix: Optional[int] = None,
                  md5: Optional[str] = None,
                  status: Optional[str] = None):
         """
         :param int asn: Autonomous System Number for local BGP deployment.
-        :param str deployment_type: `private` or `public`, the `private` is likely to be usable immediately, the
-               `public` will need to be reviewed by Equinix Metal engineers.
+        :param str deployment_type: `local` or `global`, the `local` is likely to be usable immediately, the
+               `global` will need to be reviewed by Equinix Metal engineers.
         :param int max_prefix: The maximum number of route filters allowed per server.
         :param str md5: Password for BGP session in plaintext (not a checksum).
         :param str status: status of BGP configuration in the project.
         """
         pulumi.set(__self__, "asn", asn)
         pulumi.set(__self__, "deployment_type", deployment_type)
         if max_prefix is not None:
@@ -641,16 +641,16 @@
         """
         return pulumi.get(self, "asn")
 
     @property
     @pulumi.getter(name="deploymentType")
     def deployment_type(self) -> str:
         """
-        `private` or `public`, the `private` is likely to be usable immediately, the
-        `public` will need to be reviewed by Equinix Metal engineers.
+        `local` or `global`, the `local` is likely to be usable immediately, the
+        `global` will need to be reviewed by Equinix Metal engineers.
         """
         return pulumi.get(self, "deployment_type")
 
     @property
     @pulumi.getter(name="maxPrefix")
     def max_prefix(self) -> Optional[int]:
         """
@@ -1319,15 +1319,15 @@
 @pulumi.output_type
 class GetMetroCapacityResult(dict):
     def __init__(__self__, *,
                  plan: str,
                  quantity: Optional[int] = None):
         """
         :param str plan: Device plan that must be available in selected location.
-        :param int quantity: Minimun number of devices that must be available in selected location.
+        :param int quantity: Minimum number of devices that must be available in selected location.
                Default is `1`.
         """
         pulumi.set(__self__, "plan", plan)
         if quantity is not None:
             pulumi.set(__self__, "quantity", quantity)
 
     @property
@@ -1338,15 +1338,15 @@
         """
         return pulumi.get(self, "plan")
 
     @property
     @pulumi.getter
     def quantity(self) -> Optional[int]:
         """
-        Minimun number of devices that must be available in selected location.
+        Minimum number of devices that must be available in selected location.
         Default is `1`.
         """
         return pulumi.get(self, "quantity")
 
 
 @pulumi.output_type
 class GetOrganizationAddressResult(dict):
@@ -1475,16 +1475,16 @@
                  legacy: bool,
                  line: str,
                  name: str,
                  pricing_hour: float,
                  pricing_month: float,
                  slug: str):
         """
-        :param Sequence[str] available_in_metros: list of facilities where the plan is available
-        :param Sequence[str] available_ins: list of facilities where the plan is available
+        :param Sequence[str] available_in_metros: list of metros where the plan is available
+        :param Sequence[str] available_ins: (**Deprecated**) list of facilities where the plan is available
         :param str class_: plan class
         :param Sequence[str] deployment_types: list of deployment types, e.g. on_demand, spot_market
         :param str description: description of the plan
         :param str id: id of the plan
         :param bool legacy: flag showing if it's a legacy plan
         :param str line: plan line, e.g. baremetal
         :param str name: name of the plan
@@ -1505,23 +1505,23 @@
         pulumi.set(__self__, "pricing_month", pricing_month)
         pulumi.set(__self__, "slug", slug)
 
     @property
     @pulumi.getter(name="availableInMetros")
     def available_in_metros(self) -> Sequence[str]:
         """
-        list of facilities where the plan is available
+        list of metros where the plan is available
         """
         return pulumi.get(self, "available_in_metros")
 
     @property
     @pulumi.getter(name="availableIns")
     def available_ins(self) -> Sequence[str]:
         """
-        list of facilities where the plan is available
+        (**Deprecated**) list of facilities where the plan is available
         """
         return pulumi.get(self, "available_ins")
 
     @property
     @pulumi.getter(name="class")
     def class_(self) -> str:
         """
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/port.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/port.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/port_vlan_attachment.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/port_vlan_attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
                  native: Optional[pulumi.Input[bool]] = None,
                  port_name: Optional[pulumi.Input[str]] = None,
                  vlan_vnid: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Provides a resource to attach device ports to VLANs.
 
-        Device and VLAN must be in the same facility.
+        Device and VLAN must be in the same metro.
 
         If you need this resource to add the port back to bond on removal, set `force_bond = true`.
 
         To learn more about Layer 2 networking in Equinix Metal, refer to
 
         * <https://metal.equinix.com/developers/docs/networking/layer2/>
         * <https://metal.equinix.com/developers/docs/networking/layer2-configs/>
@@ -301,15 +301,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: PortVlanAttachmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a resource to attach device ports to VLANs.
 
-        Device and VLAN must be in the same facility.
+        Device and VLAN must be in the same metro.
 
         If you need this resource to add the port back to bond on removal, set `force_bond = true`.
 
         To learn more about Layer 2 networking in Equinix Metal, refer to
 
         * <https://metal.equinix.com/developers/docs/networking/layer2/>
         * <https://metal.equinix.com/developers/docs/networking/layer2-configs/>
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/project.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/project_api_key.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/project_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/project_ssh_key.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/project_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/reserved_ip_block.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/reserved_ip_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         """
         The set of arguments for constructing a ReservedIpBlock resource.
         :param pulumi.Input[str] project_id: The metal project ID where to allocate the address block.
         :param pulumi.Input[int] cidr: Only valid as an argument and required when `type` is `vrf`. The size of the network to reserve from an existing VRF ip_range. `cidr` can only be specified with `vrf_id`. Range is 22-31. Virtual Circuits require 30-31. Other VRF resources must use a CIDR in the 22-29 range.
         :param pulumi.Input[str] custom_data: Custom Data is an arbitrary object (submitted in Terraform as serialized JSON) to assign to the IP Reservation. This may
                be helpful for self-managed IPAM. The object must be valid JSON.
         :param pulumi.Input[str] description: Arbitrary description.
-        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to allocate the public IP address block, makes sense only
-               if type is `public_ipv4` and must be empty if type is `global_ipv4`. Conflicts with `metro`.
+        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to allocate the public IP address block, makes sense only for type==public_ipv4, must be empty for
+               type==global_ipv4, conflicts with metro
         :param pulumi.Input[str] metro: Metro where to allocate the public IP address block, makes sense only
                if type is `public_ipv4` and must be empty if type is `global_ipv4`. Conflicts with `facility`.
         :param pulumi.Input[str] network: Only valid as an argument and required when `type` is `vrf`. An unreserved network address from an existing `ip_range` in the specified VRF.
         :param pulumi.Input[int] quantity: The number of allocated `/32` addresses, a power of 2. Required when `type` is not `vrf`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: String list of tags.
         :param pulumi.Input[Union[str, 'IpBlockType']] type: One of `global_ipv4`, `public_ipv4`, or `vrf`. Defaults to `public_ipv4` for backward
                compatibility.
@@ -119,16 +119,16 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def facility(self) -> Optional[pulumi.Input[Union[str, 'Facility']]]:
         """
-        Facility where to allocate the public IP address block, makes sense only
-        if type is `public_ipv4` and must be empty if type is `global_ipv4`. Conflicts with `metro`.
+        Facility where to allocate the public IP address block, makes sense only for type==public_ipv4, must be empty for
+        type==global_ipv4, conflicts with metro
         """
         return pulumi.get(self, "facility")
 
     @facility.setter
     def facility(self, value: Optional[pulumi.Input[Union[str, 'Facility']]]):
         pulumi.set(self, "facility", value)
 
@@ -247,18 +247,18 @@
         Input properties used for looking up and filtering ReservedIpBlock resources.
         :param pulumi.Input[int] address_family: Address family as integer. One of `4` or `6`.
         :param pulumi.Input[int] cidr: Only valid as an argument and required when `type` is `vrf`. The size of the network to reserve from an existing VRF ip_range. `cidr` can only be specified with `vrf_id`. Range is 22-31. Virtual Circuits require 30-31. Other VRF resources must use a CIDR in the 22-29 range.
         :param pulumi.Input[str] cidr_notation: Address and mask in CIDR notation, e.g. `147.229.15.30/31`.
         :param pulumi.Input[str] custom_data: Custom Data is an arbitrary object (submitted in Terraform as serialized JSON) to assign to the IP Reservation. This may
                be helpful for self-managed IPAM. The object must be valid JSON.
         :param pulumi.Input[str] description: Arbitrary description.
-        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to allocate the public IP address block, makes sense only
-               if type is `public_ipv4` and must be empty if type is `global_ipv4`. Conflicts with `metro`.
+        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to allocate the public IP address block, makes sense only for type==public_ipv4, must be empty for
+               type==global_ipv4, conflicts with metro
         :param pulumi.Input[bool] global_: Boolean flag whether addresses from a block are global (i.e. can be assigned in any
-               facility).
+               metro).
         :param pulumi.Input[str] metro: Metro where to allocate the public IP address block, makes sense only
                if type is `public_ipv4` and must be empty if type is `global_ipv4`. Conflicts with `facility`.
         :param pulumi.Input[str] netmask: Mask in decimal notation, e.g. `255.255.255.0`.
         :param pulumi.Input[str] network: Only valid as an argument and required when `type` is `vrf`. An unreserved network address from an existing `ip_range` in the specified VRF.
         :param pulumi.Input[str] project_id: The metal project ID where to allocate the address block.
         :param pulumi.Input[bool] public: Boolean flag whether addresses from a block are public.
         :param pulumi.Input[int] quantity: The number of allocated `/32` addresses, a power of 2. Required when `type` is not `vrf`.
@@ -381,16 +381,16 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def facility(self) -> Optional[pulumi.Input[Union[str, 'Facility']]]:
         """
-        Facility where to allocate the public IP address block, makes sense only
-        if type is `public_ipv4` and must be empty if type is `global_ipv4`. Conflicts with `metro`.
+        Facility where to allocate the public IP address block, makes sense only for type==public_ipv4, must be empty for
+        type==global_ipv4, conflicts with metro
         """
         return pulumi.get(self, "facility")
 
     @facility.setter
     def facility(self, value: Optional[pulumi.Input[Union[str, 'Facility']]]):
         pulumi.set(self, "facility", value)
 
@@ -404,15 +404,15 @@
         pulumi.set(self, "gateway", value)
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> Optional[pulumi.Input[bool]]:
         """
         Boolean flag whether addresses from a block are global (i.e. can be assigned in any
-        facility).
+        metro).
         """
         return pulumi.get(self, "global_")
 
     @global_.setter
     def global_(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "global_", value)
 
@@ -574,22 +574,22 @@
                  type: Optional[pulumi.Input[Union[str, 'IpBlockType']]] = None,
                  vrf_id: Optional[pulumi.Input[str]] = None,
                  wait_for_state: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a resource to create and manage blocks of reserved IP addresses in a project.
 
-        When a user provisions first device in a facility, Equinix Metal API automatically allocates IPv6/56 and private IPv4/25 blocks.
+        When a user provisions first device in a metro, Equinix Metal API automatically allocates IPv6/56 and private IPv4/25 blocks.
         The new device then gets IPv6 and private IPv4 addresses from those block. It also gets a public IPv4/31 address.
-        Every new device in the project and facility will automatically get IPv6 and private IPv4 addresses from these pre-allocated blocks.
+        Every new device in the project and metro will automatically get IPv6 and private IPv4 addresses from these pre-allocated blocks.
         The IPv6 and private IPv4 blocks can't be created, only imported. With this resource, it's possible to create either public IPv4 blocks or global IPv4 blocks.
 
-        Public blocks are allocated in a facility. Addresses from public blocks can only be assigned to devices in the facility. Public blocks can have mask from /24 (256 addresses) to /32 (1 address). If you create public block with this resource, you must fill the facility argument.
+        Public blocks are allocated in a metro. Addresses from public blocks can only be assigned to devices in the metro. Public blocks can have mask from /24 (256 addresses) to /32 (1 address). If you create public block with this resource, you must fill the metro argument.
 
-        Addresses from global blocks can be assigned in any facility. Global blocks can have mask from /30 (4 addresses), to /32 (1 address). If you create global block with this resource, you must specify type = "global_ipv4" and you must omit the facility argument.
+        Addresses from global blocks can be assigned in any metro. Global blocks can have mask from /30 (4 addresses), to /32 (1 address). If you create global block with this resource, you must specify type = "global_ipv4" and you must omit the metro argument.
 
         Once IP block is allocated or imported, an address from it can be assigned to device with the `metal.IpAttachment` resource.
 
         > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
 
         ## Example Usage
         ```python
@@ -622,16 +622,16 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] cidr: Only valid as an argument and required when `type` is `vrf`. The size of the network to reserve from an existing VRF ip_range. `cidr` can only be specified with `vrf_id`. Range is 22-31. Virtual Circuits require 30-31. Other VRF resources must use a CIDR in the 22-29 range.
         :param pulumi.Input[str] custom_data: Custom Data is an arbitrary object (submitted in Terraform as serialized JSON) to assign to the IP Reservation. This may
                be helpful for self-managed IPAM. The object must be valid JSON.
         :param pulumi.Input[str] description: Arbitrary description.
-        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to allocate the public IP address block, makes sense only
-               if type is `public_ipv4` and must be empty if type is `global_ipv4`. Conflicts with `metro`.
+        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to allocate the public IP address block, makes sense only for type==public_ipv4, must be empty for
+               type==global_ipv4, conflicts with metro
         :param pulumi.Input[str] metro: Metro where to allocate the public IP address block, makes sense only
                if type is `public_ipv4` and must be empty if type is `global_ipv4`. Conflicts with `facility`.
         :param pulumi.Input[str] network: Only valid as an argument and required when `type` is `vrf`. An unreserved network address from an existing `ip_range` in the specified VRF.
         :param pulumi.Input[str] project_id: The metal project ID where to allocate the address block.
         :param pulumi.Input[int] quantity: The number of allocated `/32` addresses, a power of 2. Required when `type` is not `vrf`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: String list of tags.
         :param pulumi.Input[Union[str, 'IpBlockType']] type: One of `global_ipv4`, `public_ipv4`, or `vrf`. Defaults to `public_ipv4` for backward
@@ -644,22 +644,22 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ReservedIpBlockArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a resource to create and manage blocks of reserved IP addresses in a project.
 
-        When a user provisions first device in a facility, Equinix Metal API automatically allocates IPv6/56 and private IPv4/25 blocks.
+        When a user provisions first device in a metro, Equinix Metal API automatically allocates IPv6/56 and private IPv4/25 blocks.
         The new device then gets IPv6 and private IPv4 addresses from those block. It also gets a public IPv4/31 address.
-        Every new device in the project and facility will automatically get IPv6 and private IPv4 addresses from these pre-allocated blocks.
+        Every new device in the project and metro will automatically get IPv6 and private IPv4 addresses from these pre-allocated blocks.
         The IPv6 and private IPv4 blocks can't be created, only imported. With this resource, it's possible to create either public IPv4 blocks or global IPv4 blocks.
 
-        Public blocks are allocated in a facility. Addresses from public blocks can only be assigned to devices in the facility. Public blocks can have mask from /24 (256 addresses) to /32 (1 address). If you create public block with this resource, you must fill the facility argument.
+        Public blocks are allocated in a metro. Addresses from public blocks can only be assigned to devices in the metro. Public blocks can have mask from /24 (256 addresses) to /32 (1 address). If you create public block with this resource, you must fill the metro argument.
 
-        Addresses from global blocks can be assigned in any facility. Global blocks can have mask from /30 (4 addresses), to /32 (1 address). If you create global block with this resource, you must specify type = "global_ipv4" and you must omit the facility argument.
+        Addresses from global blocks can be assigned in any metro. Global blocks can have mask from /30 (4 addresses), to /32 (1 address). If you create global block with this resource, you must specify type = "global_ipv4" and you must omit the metro argument.
 
         Once IP block is allocated or imported, an address from it can be assigned to device with the `metal.IpAttachment` resource.
 
         > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
 
         ## Example Usage
         ```python
@@ -789,18 +789,18 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] address_family: Address family as integer. One of `4` or `6`.
         :param pulumi.Input[int] cidr: Only valid as an argument and required when `type` is `vrf`. The size of the network to reserve from an existing VRF ip_range. `cidr` can only be specified with `vrf_id`. Range is 22-31. Virtual Circuits require 30-31. Other VRF resources must use a CIDR in the 22-29 range.
         :param pulumi.Input[str] cidr_notation: Address and mask in CIDR notation, e.g. `147.229.15.30/31`.
         :param pulumi.Input[str] custom_data: Custom Data is an arbitrary object (submitted in Terraform as serialized JSON) to assign to the IP Reservation. This may
                be helpful for self-managed IPAM. The object must be valid JSON.
         :param pulumi.Input[str] description: Arbitrary description.
-        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to allocate the public IP address block, makes sense only
-               if type is `public_ipv4` and must be empty if type is `global_ipv4`. Conflicts with `metro`.
+        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to allocate the public IP address block, makes sense only for type==public_ipv4, must be empty for
+               type==global_ipv4, conflicts with metro
         :param pulumi.Input[bool] global_: Boolean flag whether addresses from a block are global (i.e. can be assigned in any
-               facility).
+               metro).
         :param pulumi.Input[str] metro: Metro where to allocate the public IP address block, makes sense only
                if type is `public_ipv4` and must be empty if type is `global_ipv4`. Conflicts with `facility`.
         :param pulumi.Input[str] netmask: Mask in decimal notation, e.g. `255.255.255.0`.
         :param pulumi.Input[str] network: Only valid as an argument and required when `type` is `vrf`. An unreserved network address from an existing `ip_range` in the specified VRF.
         :param pulumi.Input[str] project_id: The metal project ID where to allocate the address block.
         :param pulumi.Input[bool] public: Boolean flag whether addresses from a block are public.
         :param pulumi.Input[int] quantity: The number of allocated `/32` addresses, a power of 2. Required when `type` is not `vrf`.
@@ -883,30 +883,30 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def facility(self) -> pulumi.Output[Optional[str]]:
         """
-        Facility where to allocate the public IP address block, makes sense only
-        if type is `public_ipv4` and must be empty if type is `global_ipv4`. Conflicts with `metro`.
+        Facility where to allocate the public IP address block, makes sense only for type==public_ipv4, must be empty for
+        type==global_ipv4, conflicts with metro
         """
         return pulumi.get(self, "facility")
 
     @property
     @pulumi.getter
     def gateway(self) -> pulumi.Output[str]:
         return pulumi.get(self, "gateway")
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> pulumi.Output[bool]:
         """
         Boolean flag whether addresses from a block are global (i.e. can be assigned in any
-        facility).
+        metro).
         """
         return pulumi.get(self, "global_")
 
     @property
     @pulumi.getter
     def manageable(self) -> pulumi.Output[bool]:
         return pulumi.get(self, "manageable")
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/spot_market_request.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/spot_market_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,25 +31,28 @@
         :param pulumi.Input['SpotMarketRequestInstanceParametersArgs'] instance_parameters: Key/Value pairs of parameters for devices provisioned from
                this request. Valid keys are: `billing_cycle`, `plan`, `operating_system`, `hostname`,
                `termintation_time`, `always_pxe`, `description`, `features`, `locked`, `project_ssh_keys`,
                `user_ssh_keys`, `userdata`, `customdata`, `ipxe_script_url`, `tags`. You can find each parameter
                description in metal.Device docs.
         :param pulumi.Input[float] max_bid_price: Maximum price user is willing to pay per hour per device.
         :param pulumi.Input[str] project_id: Project ID.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] facilities: Facility IDs where devices should be created.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] facilities: Facility IDs where devices should be created
         :param pulumi.Input[str] metro: Metro where devices should be created.
         :param pulumi.Input[bool] wait_for_devices: On resource creation wait until all desired devices are active.
                On resource destruction wait until devices are removed.
         """
         pulumi.set(__self__, "devices_max", devices_max)
         pulumi.set(__self__, "devices_min", devices_min)
         pulumi.set(__self__, "instance_parameters", instance_parameters)
         pulumi.set(__self__, "max_bid_price", max_bid_price)
         pulumi.set(__self__, "project_id", project_id)
         if facilities is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facilities is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+        if facilities is not None:
             pulumi.set(__self__, "facilities", facilities)
         if metro is not None:
             pulumi.set(__self__, "metro", metro)
         if wait_for_devices is not None:
             pulumi.set(__self__, "wait_for_devices", wait_for_devices)
 
     @property
@@ -116,15 +119,15 @@
     def project_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "project_id", value)
 
     @property
     @pulumi.getter
     def facilities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Facility IDs where devices should be created.
+        Facility IDs where devices should be created
         """
         return pulumi.get(self, "facilities")
 
     @facilities.setter
     def facilities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "facilities", value)
 
@@ -165,15 +168,15 @@
                  metro: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  wait_for_devices: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering SpotMarketRequest resources.
         :param pulumi.Input[int] devices_max: Maximum number devices to be created.
         :param pulumi.Input[int] devices_min: Miniumum number devices to be created.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] facilities: Facility IDs where devices should be created.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] facilities: Facility IDs where devices should be created
         :param pulumi.Input['SpotMarketRequestInstanceParametersArgs'] instance_parameters: Key/Value pairs of parameters for devices provisioned from
                this request. Valid keys are: `billing_cycle`, `plan`, `operating_system`, `hostname`,
                `termintation_time`, `always_pxe`, `description`, `features`, `locked`, `project_ssh_keys`,
                `user_ssh_keys`, `userdata`, `customdata`, `ipxe_script_url`, `tags`. You can find each parameter
                description in metal.Device docs.
         :param pulumi.Input[float] max_bid_price: Maximum price user is willing to pay per hour per device.
         :param pulumi.Input[str] metro: Metro where devices should be created.
@@ -182,14 +185,17 @@
                On resource destruction wait until devices are removed.
         """
         if devices_max is not None:
             pulumi.set(__self__, "devices_max", devices_max)
         if devices_min is not None:
             pulumi.set(__self__, "devices_min", devices_min)
         if facilities is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facilities is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+        if facilities is not None:
             pulumi.set(__self__, "facilities", facilities)
         if instance_parameters is not None:
             pulumi.set(__self__, "instance_parameters", instance_parameters)
         if max_bid_price is not None:
             pulumi.set(__self__, "max_bid_price", max_bid_price)
         if metro is not None:
             pulumi.set(__self__, "metro", metro)
@@ -222,15 +228,15 @@
     def devices_min(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "devices_min", value)
 
     @property
     @pulumi.getter
     def facilities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Facility IDs where devices should be created.
+        Facility IDs where devices should be created
         """
         return pulumi.get(self, "facilities")
 
     @facilities.setter
     def facilities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "facilities", value)
 
@@ -348,15 +354,15 @@
 
         This resource can be imported using an existing spot market request ID: <break><break>```sh<break> $ pulumi import equinix:metal/spotMarketRequest:SpotMarketRequest equinix_metal_spot_market_request {existing_spot_market_request_id} <break>```<break><break>
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] devices_max: Maximum number devices to be created.
         :param pulumi.Input[int] devices_min: Miniumum number devices to be created.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] facilities: Facility IDs where devices should be created.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] facilities: Facility IDs where devices should be created
         :param pulumi.Input[pulumi.InputType['SpotMarketRequestInstanceParametersArgs']] instance_parameters: Key/Value pairs of parameters for devices provisioned from
                this request. Valid keys are: `billing_cycle`, `plan`, `operating_system`, `hostname`,
                `termintation_time`, `always_pxe`, `description`, `features`, `locked`, `project_ssh_keys`,
                `user_ssh_keys`, `userdata`, `customdata`, `ipxe_script_url`, `tags`. You can find each parameter
                description in metal.Device docs.
         :param pulumi.Input[float] max_bid_price: Maximum price user is willing to pay per hour per device.
         :param pulumi.Input[str] metro: Metro where devices should be created.
@@ -438,14 +444,17 @@
 
             if devices_max is None and not opts.urn:
                 raise TypeError("Missing required property 'devices_max'")
             __props__.__dict__["devices_max"] = devices_max
             if devices_min is None and not opts.urn:
                 raise TypeError("Missing required property 'devices_min'")
             __props__.__dict__["devices_min"] = devices_min
+            if facilities is not None and not opts.urn:
+                warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+                pulumi.log.warn("""facilities is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
             __props__.__dict__["facilities"] = facilities
             if instance_parameters is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_parameters'")
             __props__.__dict__["instance_parameters"] = instance_parameters
             if max_bid_price is None and not opts.urn:
                 raise TypeError("Missing required property 'max_bid_price'")
             __props__.__dict__["max_bid_price"] = max_bid_price
@@ -477,15 +486,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] devices_max: Maximum number devices to be created.
         :param pulumi.Input[int] devices_min: Miniumum number devices to be created.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] facilities: Facility IDs where devices should be created.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] facilities: Facility IDs where devices should be created
         :param pulumi.Input[pulumi.InputType['SpotMarketRequestInstanceParametersArgs']] instance_parameters: Key/Value pairs of parameters for devices provisioned from
                this request. Valid keys are: `billing_cycle`, `plan`, `operating_system`, `hostname`,
                `termintation_time`, `always_pxe`, `description`, `features`, `locked`, `project_ssh_keys`,
                `user_ssh_keys`, `userdata`, `customdata`, `ipxe_script_url`, `tags`. You can find each parameter
                description in metal.Device docs.
         :param pulumi.Input[float] max_bid_price: Maximum price user is willing to pay per hour per device.
         :param pulumi.Input[str] metro: Metro where devices should be created.
@@ -523,15 +532,15 @@
         """
         return pulumi.get(self, "devices_min")
 
     @property
     @pulumi.getter
     def facilities(self) -> pulumi.Output[Sequence[str]]:
         """
-        Facility IDs where devices should be created.
+        Facility IDs where devices should be created
         """
         return pulumi.get(self, "facilities")
 
     @property
     @pulumi.getter(name="instanceParameters")
     def instance_parameters(self) -> pulumi.Output['outputs.SpotMarketRequestInstanceParameters']:
         """
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/ssh_key.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/user_api_key.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/user_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/virtual_circuit.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/vlan.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/vlan.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,21 +20,25 @@
                  facility: Optional[pulumi.Input[Union[str, 'Facility']]] = None,
                  metro: Optional[pulumi.Input[str]] = None,
                  vxlan: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a Vlan resource.
         :param pulumi.Input[str] project_id: ID of parent project.
         :param pulumi.Input[str] description: Description string.
-        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to create the VLAN.
+        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to create the VLAN
+        :param pulumi.Input[str] metro: Metro in which to create the VLAN
         :param pulumi.Input[int] vxlan: VLAN ID, must be unique in metro.
         """
         pulumi.set(__self__, "project_id", project_id)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if facility is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+        if facility is not None:
             pulumi.set(__self__, "facility", facility)
         if metro is not None:
             pulumi.set(__self__, "metro", metro)
         if vxlan is not None:
             pulumi.set(__self__, "vxlan", vxlan)
 
     @property
@@ -61,25 +65,28 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def facility(self) -> Optional[pulumi.Input[Union[str, 'Facility']]]:
         """
-        Facility where to create the VLAN.
+        Facility where to create the VLAN
         """
         return pulumi.get(self, "facility")
 
     @facility.setter
     def facility(self, value: Optional[pulumi.Input[Union[str, 'Facility']]]):
         pulumi.set(self, "facility", value)
 
     @property
     @pulumi.getter
     def metro(self) -> Optional[pulumi.Input[str]]:
+        """
+        Metro in which to create the VLAN
+        """
         return pulumi.get(self, "metro")
 
     @metro.setter
     def metro(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "metro", value)
 
     @property
@@ -102,21 +109,25 @@
                  facility: Optional[pulumi.Input[Union[str, 'Facility']]] = None,
                  metro: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  vxlan: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering Vlan resources.
         :param pulumi.Input[str] description: Description string.
-        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to create the VLAN.
+        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to create the VLAN
+        :param pulumi.Input[str] metro: Metro in which to create the VLAN
         :param pulumi.Input[str] project_id: ID of parent project.
         :param pulumi.Input[int] vxlan: VLAN ID, must be unique in metro.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if facility is not None:
+            warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+            pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+        if facility is not None:
             pulumi.set(__self__, "facility", facility)
         if metro is not None:
             pulumi.set(__self__, "metro", metro)
         if project_id is not None:
             pulumi.set(__self__, "project_id", project_id)
         if vxlan is not None:
             pulumi.set(__self__, "vxlan", vxlan)
@@ -133,25 +144,28 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def facility(self) -> Optional[pulumi.Input[Union[str, 'Facility']]]:
         """
-        Facility where to create the VLAN.
+        Facility where to create the VLAN
         """
         return pulumi.get(self, "facility")
 
     @facility.setter
     def facility(self, value: Optional[pulumi.Input[Union[str, 'Facility']]]):
         pulumi.set(self, "facility", value)
 
     @property
     @pulumi.getter
     def metro(self) -> Optional[pulumi.Input[str]]:
+        """
+        Metro in which to create the VLAN
+        """
         return pulumi.get(self, "metro")
 
     @metro.setter
     def metro(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "metro", value)
 
     @property
@@ -220,15 +234,16 @@
         ## Import
 
         This resource can be imported using an existing VLAN ID (UUID): <break><break>```sh<break> $ pulumi import equinix:metal/vlan:Vlan equinix_metal_vlan {existing_vlan_id} <break>```<break><break>
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description string.
-        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to create the VLAN.
+        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to create the VLAN
+        :param pulumi.Input[str] metro: Metro in which to create the VLAN
         :param pulumi.Input[str] project_id: ID of parent project.
         :param pulumi.Input[int] vxlan: VLAN ID, must be unique in metro.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -291,14 +306,17 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VlanArgs.__new__(VlanArgs)
 
             __props__.__dict__["description"] = description
+            if facility is not None and not opts.urn:
+                warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+                pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
             __props__.__dict__["facility"] = facility
             __props__.__dict__["metro"] = metro
             if project_id is None and not opts.urn:
                 raise TypeError("Missing required property 'project_id'")
             __props__.__dict__["project_id"] = project_id
             __props__.__dict__["vxlan"] = vxlan
         super(Vlan, __self__).__init__(
@@ -320,15 +338,16 @@
         Get an existing Vlan resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description string.
-        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to create the VLAN.
+        :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to create the VLAN
+        :param pulumi.Input[str] metro: Metro in which to create the VLAN
         :param pulumi.Input[str] project_id: ID of parent project.
         :param pulumi.Input[int] vxlan: VLAN ID, must be unique in metro.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _VlanState.__new__(_VlanState)
 
@@ -347,21 +366,24 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def facility(self) -> pulumi.Output[Optional[str]]:
         """
-        Facility where to create the VLAN.
+        Facility where to create the VLAN
         """
         return pulumi.get(self, "facility")
 
     @property
     @pulumi.getter
     def metro(self) -> pulumi.Output[Optional[str]]:
+        """
+        Metro in which to create the VLAN
+        """
         return pulumi.get(self, "metro")
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> pulumi.Output[str]:
         """
         ID of parent project.
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/metal/vrf.py` & `pulumi_equinix-0.2.0/pulumi_equinix/metal/vrf.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/__init__.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/_enums.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/_inputs.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/acl_template.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/acl_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/bgp.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/bgp.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/device.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/device_link.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/device_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/get_account.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/get_device.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/get_device_platform.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device_platform.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/get_device_software.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device_software.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/get_device_type.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/get_device_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/network_file.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/network_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/outputs.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/ssh_key.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/ssh_key.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,24 +11,28 @@
 
 __all__ = ['SshKeyArgs', 'SshKey']
 
 @pulumi.input_type
 class SshKeyArgs:
     def __init__(__self__, *,
                  public_key: pulumi.Input[str],
-                 name: Optional[pulumi.Input[str]] = None):
+                 name: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SshKey resource.
         :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
                interpolation function.
         :param pulumi.Input[str] name: The name of SSH key used for identification.
+        :param pulumi.Input[str] type: The type of SSH key: `RSA` (default) or `DSA`.
         """
         pulumi.set(__self__, "public_key", public_key)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> pulumi.Input[str]:
         """
         The SSH public key. If this is a file, it can be read using the file
         interpolation function.
@@ -47,32 +51,48 @@
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        """
+        The type of SSH key: `RSA` (default) or `DSA`.
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
+
 
 @pulumi.input_type
 class _SshKeyState:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SshKey resources.
         :param pulumi.Input[str] name: The name of SSH key used for identification.
         :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
                interpolation function.
+        :param pulumi.Input[str] type: The type of SSH key: `RSA` (default) or `DSA`.
         :param pulumi.Input[str] uuid: The unique identifier of the key
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if public_key is not None:
             pulumi.set(__self__, "public_key", public_key)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
@@ -95,14 +115,26 @@
 
     @public_key.setter
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
     @property
     @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        """
+        The type of SSH key: `RSA` (default) or `DSA`.
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
+
+    @property
+    @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
         The unique identifier of the key
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
@@ -113,14 +145,15 @@
 class SshKey(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Resource `networkedge.SshKey` allows creation and management of Equinix Network Edge SSH keys.
 
         ## Example Usage
         ```python
         import pulumi
@@ -137,14 +170,15 @@
         This resource can be imported using an existing ID: <break><break>```sh<break> $ pulumi import equinix:networkedge/sshKey:SshKey example {existing_id} <break>```<break><break>
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of SSH key used for identification.
         :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
                interpolation function.
+        :param pulumi.Input[str] type: The type of SSH key: `RSA` (default) or `DSA`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SshKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -179,59 +213,64 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SshKeyArgs.__new__(SshKeyArgs)
 
             __props__.__dict__["name"] = name
             if public_key is None and not opts.urn:
                 raise TypeError("Missing required property 'public_key'")
             __props__.__dict__["public_key"] = public_key
+            __props__.__dict__["type"] = type
             __props__.__dict__["uuid"] = None
         super(SshKey, __self__).__init__(
             'equinix:networkedge/sshKey:SshKey',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             name: Optional[pulumi.Input[str]] = None,
             public_key: Optional[pulumi.Input[str]] = None,
+            type: Optional[pulumi.Input[str]] = None,
             uuid: Optional[pulumi.Input[str]] = None) -> 'SshKey':
         """
         Get an existing SshKey resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of SSH key used for identification.
         :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
                interpolation function.
+        :param pulumi.Input[str] type: The type of SSH key: `RSA` (default) or `DSA`.
         :param pulumi.Input[str] uuid: The unique identifier of the key
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SshKeyState.__new__(_SshKeyState)
 
         __props__.__dict__["name"] = name
         __props__.__dict__["public_key"] = public_key
+        __props__.__dict__["type"] = type
         __props__.__dict__["uuid"] = uuid
         return SshKey(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -246,13 +285,21 @@
         The SSH public key. If this is a file, it can be read using the file
         interpolation function.
         """
         return pulumi.get(self, "public_key")
 
     @property
     @pulumi.getter
+    def type(self) -> pulumi.Output[Optional[str]]:
+        """
+        The type of SSH key: `RSA` (default) or `DSA`.
+        """
+        return pulumi.get(self, "type")
+
+    @property
+    @pulumi.getter
     def uuid(self) -> pulumi.Output[str]:
         """
         The unique identifier of the key
         """
         return pulumi.get(self, "uuid")
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/networkedge/ssh_user.py` & `pulumi_equinix-0.2.0/pulumi_equinix/networkedge/ssh_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix/provider.py` & `pulumi_equinix-0.2.0/pulumi_equinix/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix.egg-info/PKG-INFO` & `pulumi_equinix-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-equinix
-Version: 0.1.1
+Name: pulumi_equinix
+Version: 0.2.0
 Summary: A Pulumi package for creating and managing equinix cloud resources.
 Home-page: https://deploy.equinix.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/equinix/pulumi-equinix
 Keywords: pulumi equinix category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_equinix-0.1.1/pulumi_equinix.egg-info/SOURCES.txt` & `pulumi_equinix-0.2.0/pulumi_equinix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.1.1/setup.py` & `pulumi_equinix-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.1"
-PLUGIN_VERSION = "0.1.1"
+VERSION = "0.2.0"
+PLUGIN_VERSION = "0.2.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'equinix', PLUGIN_VERSION, '--server', 'github://api.github.com/equinix'])
         except OSError as error:
```

