# Comparing `tmp/types-paramiko-3.0.0.7.tar.gz` & `tmp/types-paramiko-3.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-paramiko-3.0.0.7.tar", last modified: Tue Apr  4 15:16:03 2023, max compression
+gzip compressed data, was "types-paramiko-3.0.0.8.tar", last modified: Tue Apr 25 21:13:14 2023, max compression
```

## Comparing `types-paramiko-3.0.0.7.tar` & `types-paramiko-3.0.0.8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:16:03.658178 types-paramiko-3.0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-04 15:16:03.000000 types-paramiko-3.0.0.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 15:16:03.000000 types-paramiko-3.0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-04 15:16:03.658178 types-paramiko-3.0.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:16:03.658178 types-paramiko-3.0.0.7/paramiko-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-04 15:16:03.000000 types-paramiko-3.0.0.7/paramiko-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/_winapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/agent.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/auth_handler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/ber.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/buffered_pipe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/channel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/common.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/compress.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/dsskey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/ecdsakey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/ed25519key.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/hostkeys.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/kex_curve25519.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/kex_ecdh_nist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/kex_gex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/kex_group1.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/kex_group14.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/kex_group16.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/kex_gss.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/message.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/packet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/pipe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/pkey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/primes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/rsakey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/sftp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/sftp_attr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/sftp_client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/sftp_file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/sftp_handle.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/sftp_server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/sftp_si.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/ssh_exception.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/ssh_gss.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/transport.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/win_openssh.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-04 15:15:34.000000 types-paramiko-3.0.0.7/paramiko-stubs/win_pageant.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:16:03.658178 types-paramiko-3.0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-04 15:16:03.000000 types-paramiko-3.0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:16:03.658178 types-paramiko-3.0.0.7/types_paramiko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-04 15:16:03.000000 types-paramiko-3.0.0.7/types_paramiko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-04 15:16:03.000000 types-paramiko-3.0.0.7/types_paramiko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:16:03.000000 types-paramiko-3.0.0.7/types_paramiko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 15:16:03.000000 types-paramiko-3.0.0.7/types_paramiko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-04 15:16:03.000000 types-paramiko-3.0.0.7/types_paramiko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:14.960519 types-paramiko-3.0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-04-25 21:13:13.000000 types-paramiko-3.0.0.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 21:13:13.000000 types-paramiko-3.0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-25 21:13:14.960519 types-paramiko-3.0.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:14.960519 types-paramiko-3.0.0.8/paramiko-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 21:13:13.000000 types-paramiko-3.0.0.8/paramiko-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/_winapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/agent.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/auth_handler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/ber.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/buffered_pipe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/channel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/compress.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/dsskey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/ecdsakey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/ed25519key.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/hostkeys.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_curve25519.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_ecdh_nist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_gex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_group1.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_group14.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_group16.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/kex_gss.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/packet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/pipe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/pkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/primes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/rsakey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/server.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp_attr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp_file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp_handle.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp_server.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/sftp_si.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/ssh_exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/ssh_gss.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/transport.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/win_openssh.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-25 21:13:01.000000 types-paramiko-3.0.0.8/paramiko-stubs/win_pageant.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 21:13:14.960519 types-paramiko-3.0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-25 21:13:13.000000 types-paramiko-3.0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:14.960519 types-paramiko-3.0.0.8/types_paramiko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-25 21:13:14.000000 types-paramiko-3.0.0.8/types_paramiko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-25 21:13:14.000000 types-paramiko-3.0.0.8/types_paramiko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:13:14.000000 types-paramiko-3.0.0.8/types_paramiko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 21:13:14.000000 types-paramiko-3.0.0.8/types_paramiko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 21:13:14.000000 types-paramiko-3.0.0.8/types_paramiko.egg-info/top_level.txt
```

### Comparing `types-paramiko-3.0.0.7/CHANGELOG.md` & `types-paramiko-3.0.0.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 3.0.0.8 (2023-04-25)
+
+`paramiko`: Be more lenient for client parameter types (#10083)
+
+Use Mapping instead of dict for better covariance
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 3.0.0.7 (2023-04-04)
 
 `google-cloud-ndb`, `paramiko`, `setuptools`: remove unnecessary `= ...`s (#10011)
 
 ## 3.0.0.6 (2023-03-29)
 
 Remove unnecessary ellipsis expressions (#9976)
```

### Comparing `types-paramiko-3.0.0.7/PKG-INFO` & `types-paramiko-3.0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-paramiko
-Version: 3.0.0.7
+Version: 3.0.0.8
 Summary: Typing stubs for paramiko
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `paramiko`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/paramiko. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `60939b00afede13feeec3cee6f6dfe6eb2df1593`.
+This package was generated from typeshed commit `c4b6d635abb881f0a3b0e87d4b4f75933bcde317`.
```

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/__init__.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/_winapi.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/_winapi.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/agent.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/agent.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/auth_handler.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/auth_handler.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/ber.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/ber.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/channel.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/channel.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/client.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 from paramiko.transport import Transport
 from paramiko.util import ClosingContextManager
 
 from .transport import _SocketLike
 
 class _TransportFactory(Protocol):
     def __call__(
-        self, __sock: _SocketLike, *, gss_kex: bool, gss_deleg_creds: bool, disabled_algorithms: dict[str, Iterable[str]] | None
+        self,
+        __sock: _SocketLike,
+        *,
+        gss_kex: bool,
+        gss_deleg_creds: bool,
+        disabled_algorithms: Mapping[str, Iterable[str]] | None,
     ) -> Transport: ...
 
 class SSHClient(ClosingContextManager):
     def __init__(self) -> None: ...
     def load_system_host_keys(self, filename: str | None = None) -> None: ...
     def load_host_keys(self, filename: str) -> None: ...
     def save_host_keys(self, filename: str) -> None: ...
@@ -40,25 +45,25 @@
         gss_kex: bool = False,
         gss_deleg_creds: bool = True,
         gss_host: str | None = None,
         banner_timeout: float | None = None,
         auth_timeout: float | None = None,
         gss_trust_dns: bool = True,
         passphrase: str | None = None,
-        disabled_algorithms: dict[str, Iterable[str]] | None = None,
+        disabled_algorithms: Mapping[str, Iterable[str]] | None = None,
         transport_factory: _TransportFactory | None = None,
     ) -> None: ...
     def close(self) -> None: ...
     def exec_command(
         self,
         command: str,
         bufsize: int = -1,
         timeout: float | None = None,
         get_pty: bool = False,
-        environment: dict[str, str] | None = None,
+        environment: Mapping[str, str] | None = None,
     ) -> tuple[ChannelStdinFile, ChannelFile, ChannelStderrFile]: ...
     def invoke_shell(
         self,
         term: str = "vt100",
         width: int = 80,
         height: int = 24,
         width_pixels: int = 0,
```

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/common.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/common.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/config.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/config.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/dsskey.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/dsskey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/ecdsakey.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/ecdsakey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/ed25519key.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/ed25519key.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/file.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/file.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/hostkeys.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/hostkeys.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/kex_curve25519.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/kex_curve25519.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/kex_ecdh_nist.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/kex_ecdh_nist.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/kex_gex.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/kex_gex.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/kex_group1.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/kex_group1.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/kex_gss.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/kex_gss.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/message.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/message.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/packet.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/packet.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/pipe.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/pipe.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/pkey.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/pkey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/rsakey.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/rsakey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/server.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/server.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/sftp.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/sftp.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/sftp_attr.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/sftp_attr.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/sftp_client.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/sftp_client.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/sftp_file.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/sftp_file.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/sftp_server.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/sftp_server.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/sftp_si.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/sftp_si.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/ssh_exception.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/ssh_exception.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/ssh_gss.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/ssh_gss.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/transport.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/transport.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections.abc import Callable, Iterable, Sequence
+from collections.abc import Callable, Iterable, Mapping, Sequence
 from logging import Logger
 from socket import socket
 from threading import Condition, Event, Lock, Thread
 from types import ModuleType
 from typing import Any, Protocol
 from typing_extensions import TypeAlias
 
@@ -60,30 +60,30 @@
     logger: Logger
     auth_handler: AuthHandler | None
     global_response: Message | None
     completion_event: Event | None
     banner_timeout: float
     handshake_timeout: float
     auth_timeout: float
-    disabled_algorithms: dict[str, Iterable[str]] | None
+    disabled_algorithms: Mapping[str, Iterable[str]] | None
     server_mode: bool
     server_object: ServerInterface | None
     server_key_dict: dict[str, PKey]
     server_accepts: list[Channel]
     server_accept_cv: Condition
     subsystem_table: dict[str, tuple[type[SubsystemHandler], tuple[Any, ...], dict[str, Any]]]
     sys: ModuleType
     def __init__(
         self,
         sock: _SocketLike,
         default_window_size: int = 2097152,
         default_max_packet_size: int = 32768,
         gss_kex: bool = False,
         gss_deleg_creds: bool = True,
-        disabled_algorithms: dict[str, Iterable[str]] | None = None,
+        disabled_algorithms: Mapping[str, Iterable[str]] | None = None,
         server_sig_algs: bool = True,
     ) -> None: ...
     @property
     def preferred_ciphers(self) -> Sequence[str]: ...
     @property
     def preferred_macs(self) -> Sequence[str]: ...
     @property
```

### Comparing `types-paramiko-3.0.0.7/paramiko-stubs/util.pyi` & `types-paramiko-3.0.0.8/paramiko-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.0.0.7/setup.py` & `types-paramiko-3.0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `paramiko`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/paramiko. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `60939b00afede13feeec3cee6f6dfe6eb2df1593`.
+This package was generated from typeshed commit `c4b6d635abb881f0a3b0e87d4b4f75933bcde317`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.0.0.7",
+      version="3.0.0.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md",
```

### Comparing `types-paramiko-3.0.0.7/types_paramiko.egg-info/PKG-INFO` & `types-paramiko-3.0.0.8/types_paramiko.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-paramiko
-Version: 3.0.0.7
+Version: 3.0.0.8
 Summary: Typing stubs for paramiko
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `paramiko`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/paramiko. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `60939b00afede13feeec3cee6f6dfe6eb2df1593`.
+This package was generated from typeshed commit `c4b6d635abb881f0a3b0e87d4b4f75933bcde317`.
```

### Comparing `types-paramiko-3.0.0.7/types_paramiko.egg-info/SOURCES.txt` & `types-paramiko-3.0.0.8/types_paramiko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

