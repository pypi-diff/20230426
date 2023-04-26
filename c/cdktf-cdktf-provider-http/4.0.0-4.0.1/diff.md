# Comparing `tmp/cdktf-cdktf-provider-http-4.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-http-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-http-4.0.0.tar", last modified: Tue Apr 18 20:44:52 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-http-4.0.1.tar", last modified: Wed Apr 26 03:15:14 2023, max compression
```

## Comparing `cdktf-cdktf-provider-http-4.0.0.tar` & `cdktf-cdktf-provider-http-4.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.244869 cdktf-cdktf-provider-http-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50098 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/_jsii/provider-http@4.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/data_http/
--rw-r--r--   0 runner    (1001) docker     (123)    29953 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/data_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 20:44:52.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-18 20:44:52.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:44:52.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:44:52.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 20:44:52.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:15:14.731841 cdktf-cdktf-provider-http-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-26 03:15:03.000000 cdktf-cdktf-provider-http-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 03:15:03.000000 cdktf-cdktf-provider-http-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-26 03:15:14.731841 cdktf-cdktf-provider-http-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-26 03:15:03.000000 cdktf-cdktf-provider-http-4.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 03:15:03.000000 cdktf-cdktf-provider-http-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 03:15:14.731841 cdktf-cdktf-provider-http-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-26 03:15:03.000000 cdktf-cdktf-provider-http-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:15:14.731841 cdktf-cdktf-provider-http-4.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:15:14.731841 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-26 03:15:03.000000 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:15:14.731841 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-26 03:15:03.000000 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28560 2023-04-26 03:15:03.000000 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/_jsii/provider-http@4.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:15:14.731841 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/data_http/
+-rw-r--r--   0 runner    (1001) docker     (123)    45926 2023-04-26 03:15:03.000000 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/data_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:15:14.731841 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-26 03:15:03.000000 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 03:15:03.000000 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:15:14.731841 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-26 03:15:14.000000 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-26 03:15:14.000000 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 03:15:14.000000 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-26 03:15:14.000000 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 03:15:14.000000 cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-http-4.0.0/LICENSE` & `cdktf-cdktf-provider-http-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-http-4.0.0/PKG-INFO` & `cdktf-cdktf-provider-http-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-http
-Version: 4.0.0
+Version: 4.0.1
 Summary: Prebuilt http Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-http.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-http.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-http-4.0.0/README.md` & `cdktf-cdktf-provider-http-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-http-4.0.0/setup.py` & `cdktf-cdktf-provider-http-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-http",
-    "version": "4.0.0",
+    "version": "4.0.1",
     "description": "Prebuilt http Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-http.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -24,15 +24,15 @@
         "cdktf_cdktf_provider_http",
         "cdktf_cdktf_provider_http._jsii",
         "cdktf_cdktf_provider_http.data_http",
         "cdktf_cdktf_provider_http.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_http._jsii": [
-            "provider-http@4.0.0.jsii.tgz"
+            "provider-http@4.0.1.jsii.tgz"
         ],
         "cdktf_cdktf_provider_http": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/__init__.py` & `cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/data_http/__init__.py` & `cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/data_http/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_http`
 
-Refer to the Terraform Registory for docs: [`data_http`](https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http).
+Refer to the Terraform Registory for docs: [`data_http`](https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,45 +22,49 @@
 
 
 class DataHttp(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-http.dataHttp.DataHttp",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http http}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http http}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         url: builtins.str,
         ca_cert_pem: typing.Optional[builtins.str] = None,
         insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         method: typing.Optional[builtins.str] = None,
         request_body: typing.Optional[builtins.str] = None,
         request_headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        request_timeout_ms: typing.Optional[jsii.Number] = None,
+        retry: typing.Optional[typing.Union["DataHttpRetry", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http http} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http http} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param url: The URL for the request. Supported schemes are ``http`` and ``https``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#url DataHttp#url}
-        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
-        :param insecure: Disables verification of the server's certificate chain and hostname. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#insecure DataHttp#insecure}
-        :param method: The HTTP Method for the request. Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#method DataHttp#method}
-        :param request_body: The request body as a string. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#request_body DataHttp#request_body}
-        :param request_headers: A map of request header field names and values. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#request_headers DataHttp#request_headers}
+        :param url: The URL for the request. Supported schemes are ``http`` and ``https``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#url DataHttp#url}
+        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
+        :param insecure: Disables verification of the server's certificate chain and hostname. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#insecure DataHttp#insecure}
+        :param method: The HTTP Method for the request. Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#method DataHttp#method}
+        :param request_body: The request body as a string. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_body DataHttp#request_body}
+        :param request_headers: A map of request header field names and values. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_headers DataHttp#request_headers}
+        :param request_timeout_ms: The request timeout in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_timeout_ms DataHttp#request_timeout_ms}
+        :param retry: retry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#retry DataHttp#retry}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -72,25 +76,46 @@
         config = DataHttpConfig(
             url=url,
             ca_cert_pem=ca_cert_pem,
             insecure=insecure,
             method=method,
             request_body=request_body,
             request_headers=request_headers,
+            request_timeout_ms=request_timeout_ms,
+            retry=retry,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
         jsii.create(self.__class__, self, [scope, id, config])
 
+    @jsii.member(jsii_name="putRetry")
+    def put_retry(
+        self,
+        *,
+        attempts: typing.Optional[jsii.Number] = None,
+        max_delay_ms: typing.Optional[jsii.Number] = None,
+        min_delay_ms: typing.Optional[jsii.Number] = None,
+    ) -> None:
+        '''
+        :param attempts: The number of times the request is to be retried. For example, if 2 is specified, the request will be tried a maximum of 3 times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#attempts DataHttp#attempts}
+        :param max_delay_ms: The maximum delay between retry requests in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#max_delay_ms DataHttp#max_delay_ms}
+        :param min_delay_ms: The minimum delay between retry requests in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#min_delay_ms DataHttp#min_delay_ms}
+        '''
+        value = DataHttpRetry(
+            attempts=attempts, max_delay_ms=max_delay_ms, min_delay_ms=min_delay_ms
+        )
+
+        return typing.cast(None, jsii.invoke(self, "putRetry", [value]))
+
     @jsii.member(jsii_name="resetCaCertPem")
     def reset_ca_cert_pem(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetCaCertPem", []))
 
     @jsii.member(jsii_name="resetInsecure")
     def reset_insecure(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetInsecure", []))
@@ -103,14 +128,22 @@
     def reset_request_body(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetRequestBody", []))
 
     @jsii.member(jsii_name="resetRequestHeaders")
     def reset_request_headers(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetRequestHeaders", []))
 
+    @jsii.member(jsii_name="resetRequestTimeoutMs")
+    def reset_request_timeout_ms(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetRequestTimeoutMs", []))
+
+    @jsii.member(jsii_name="resetRetry")
+    def reset_retry(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetRetry", []))
+
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
@@ -133,14 +166,19 @@
 
     @builtins.property
     @jsii.member(jsii_name="responseHeaders")
     def response_headers(self) -> _cdktf_9a9027ec.StringMap:
         return typing.cast(_cdktf_9a9027ec.StringMap, jsii.get(self, "responseHeaders"))
 
     @builtins.property
+    @jsii.member(jsii_name="retry")
+    def retry(self) -> "DataHttpRetryOutputReference":
+        return typing.cast("DataHttpRetryOutputReference", jsii.get(self, "retry"))
+
+    @builtins.property
     @jsii.member(jsii_name="statusCode")
     def status_code(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "statusCode"))
 
     @builtins.property
     @jsii.member(jsii_name="caCertPemInput")
     def ca_cert_pem_input(self) -> typing.Optional[builtins.str]:
@@ -167,14 +205,26 @@
     @jsii.member(jsii_name="requestHeadersInput")
     def request_headers_input(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], jsii.get(self, "requestHeadersInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="requestTimeoutMsInput")
+    def request_timeout_ms_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "requestTimeoutMsInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="retryInput")
+    def retry_input(
+        self,
+    ) -> typing.Optional[typing.Union["DataHttpRetry", _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union["DataHttpRetry", _cdktf_9a9027ec.IResolvable]], jsii.get(self, "retryInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="urlInput")
     def url_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "urlInput"))
 
     @builtins.property
     @jsii.member(jsii_name="caCertPem")
     def ca_cert_pem(self) -> builtins.str:
@@ -238,14 +288,26 @@
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1a74bd45d9b8a30578befabcf666ca96bd1f9bef3b6e84638b0934128d782b51)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "requestHeaders", value)
 
     @builtins.property
+    @jsii.member(jsii_name="requestTimeoutMs")
+    def request_timeout_ms(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "requestTimeoutMs"))
+
+    @request_timeout_ms.setter
+    def request_timeout_ms(self, value: jsii.Number) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__56342ca3a5f8a383c7aa7363c40000689eb017e1d4a08f440bf27cac06150376)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "requestTimeoutMs", value)
+
+    @builtins.property
     @jsii.member(jsii_name="url")
     def url(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "url"))
 
     @url.setter
     def url(self, value: builtins.str) -> None:
         if __debug__:
@@ -267,14 +329,16 @@
         "provisioners": "provisioners",
         "url": "url",
         "ca_cert_pem": "caCertPem",
         "insecure": "insecure",
         "method": "method",
         "request_body": "requestBody",
         "request_headers": "requestHeaders",
+        "request_timeout_ms": "requestTimeoutMs",
+        "retry": "retry",
     },
 )
 class DataHttpConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
@@ -286,32 +350,38 @@
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         url: builtins.str,
         ca_cert_pem: typing.Optional[builtins.str] = None,
         insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         method: typing.Optional[builtins.str] = None,
         request_body: typing.Optional[builtins.str] = None,
         request_headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        request_timeout_ms: typing.Optional[jsii.Number] = None,
+        retry: typing.Optional[typing.Union["DataHttpRetry", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param url: The URL for the request. Supported schemes are ``http`` and ``https``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#url DataHttp#url}
-        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
-        :param insecure: Disables verification of the server's certificate chain and hostname. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#insecure DataHttp#insecure}
-        :param method: The HTTP Method for the request. Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#method DataHttp#method}
-        :param request_body: The request body as a string. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#request_body DataHttp#request_body}
-        :param request_headers: A map of request header field names and values. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#request_headers DataHttp#request_headers}
+        :param url: The URL for the request. Supported schemes are ``http`` and ``https``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#url DataHttp#url}
+        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
+        :param insecure: Disables verification of the server's certificate chain and hostname. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#insecure DataHttp#insecure}
+        :param method: The HTTP Method for the request. Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#method DataHttp#method}
+        :param request_body: The request body as a string. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_body DataHttp#request_body}
+        :param request_headers: A map of request header field names and values. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_headers DataHttp#request_headers}
+        :param request_timeout_ms: The request timeout in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_timeout_ms DataHttp#request_timeout_ms}
+        :param retry: retry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#retry DataHttp#retry}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
+        if isinstance(retry, dict):
+            retry = DataHttpRetry(**retry)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ee2b6a3664a80e642a2ef1d255302a3f3dc3d391999cb8f3d6103cac8420d573)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
@@ -319,14 +389,16 @@
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument url", value=url, expected_type=type_hints["url"])
             check_type(argname="argument ca_cert_pem", value=ca_cert_pem, expected_type=type_hints["ca_cert_pem"])
             check_type(argname="argument insecure", value=insecure, expected_type=type_hints["insecure"])
             check_type(argname="argument method", value=method, expected_type=type_hints["method"])
             check_type(argname="argument request_body", value=request_body, expected_type=type_hints["request_body"])
             check_type(argname="argument request_headers", value=request_headers, expected_type=type_hints["request_headers"])
+            check_type(argname="argument request_timeout_ms", value=request_timeout_ms, expected_type=type_hints["request_timeout_ms"])
+            check_type(argname="argument retry", value=retry, expected_type=type_hints["retry"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "url": url,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
@@ -346,14 +418,18 @@
             self._values["insecure"] = insecure
         if method is not None:
             self._values["method"] = method
         if request_body is not None:
             self._values["request_body"] = request_body
         if request_headers is not None:
             self._values["request_headers"] = request_headers
+        if request_timeout_ms is not None:
+            self._values["request_timeout_ms"] = request_timeout_ms
+        if retry is not None:
+            self._values["retry"] = retry
 
     @builtins.property
     def connection(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]]:
         '''
         :stability: experimental
@@ -415,100 +491,299 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def url(self) -> builtins.str:
         '''The URL for the request. Supported schemes are ``http`` and ``https``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#url DataHttp#url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#url DataHttp#url}
         '''
         result = self._values.get("url")
         assert result is not None, "Required property 'url' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def ca_cert_pem(self) -> typing.Optional[builtins.str]:
         '''Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
         '''
         result = self._values.get("ca_cert_pem")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def insecure(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Disables verification of the server's certificate chain and hostname. Defaults to ``false``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#insecure DataHttp#insecure}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#insecure DataHttp#insecure}
         '''
         result = self._values.get("insecure")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def method(self) -> typing.Optional[builtins.str]:
         '''The HTTP Method for the request.
 
         Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#method DataHttp#method}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#method DataHttp#method}
         '''
         result = self._values.get("method")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def request_body(self) -> typing.Optional[builtins.str]:
         '''The request body as a string.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#request_body DataHttp#request_body}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_body DataHttp#request_body}
         '''
         result = self._values.get("request_body")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def request_headers(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''A map of request header field names and values.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#request_headers DataHttp#request_headers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_headers DataHttp#request_headers}
         '''
         result = self._values.get("request_headers")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
+    @builtins.property
+    def request_timeout_ms(self) -> typing.Optional[jsii.Number]:
+        '''The request timeout in milliseconds.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_timeout_ms DataHttp#request_timeout_ms}
+        '''
+        result = self._values.get("request_timeout_ms")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def retry(self) -> typing.Optional["DataHttpRetry"]:
+        '''retry block.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#retry DataHttp#retry}
+        '''
+        result = self._values.get("retry")
+        return typing.cast(typing.Optional["DataHttpRetry"], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
         return "DataHttpConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+@jsii.data_type(
+    jsii_type="@cdktf/provider-http.dataHttp.DataHttpRetry",
+    jsii_struct_bases=[],
+    name_mapping={
+        "attempts": "attempts",
+        "max_delay_ms": "maxDelayMs",
+        "min_delay_ms": "minDelayMs",
+    },
+)
+class DataHttpRetry:
+    def __init__(
+        self,
+        *,
+        attempts: typing.Optional[jsii.Number] = None,
+        max_delay_ms: typing.Optional[jsii.Number] = None,
+        min_delay_ms: typing.Optional[jsii.Number] = None,
+    ) -> None:
+        '''
+        :param attempts: The number of times the request is to be retried. For example, if 2 is specified, the request will be tried a maximum of 3 times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#attempts DataHttp#attempts}
+        :param max_delay_ms: The maximum delay between retry requests in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#max_delay_ms DataHttp#max_delay_ms}
+        :param min_delay_ms: The minimum delay between retry requests in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#min_delay_ms DataHttp#min_delay_ms}
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__5db3ea948028eba5857abc78a333d807c1e084b83b50b80801b01c9a63f2d524)
+            check_type(argname="argument attempts", value=attempts, expected_type=type_hints["attempts"])
+            check_type(argname="argument max_delay_ms", value=max_delay_ms, expected_type=type_hints["max_delay_ms"])
+            check_type(argname="argument min_delay_ms", value=min_delay_ms, expected_type=type_hints["min_delay_ms"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if attempts is not None:
+            self._values["attempts"] = attempts
+        if max_delay_ms is not None:
+            self._values["max_delay_ms"] = max_delay_ms
+        if min_delay_ms is not None:
+            self._values["min_delay_ms"] = min_delay_ms
+
+    @builtins.property
+    def attempts(self) -> typing.Optional[jsii.Number]:
+        '''The number of times the request is to be retried.
+
+        For example, if 2 is specified, the request will be tried a maximum of 3 times.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#attempts DataHttp#attempts}
+        '''
+        result = self._values.get("attempts")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def max_delay_ms(self) -> typing.Optional[jsii.Number]:
+        '''The maximum delay between retry requests in milliseconds.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#max_delay_ms DataHttp#max_delay_ms}
+        '''
+        result = self._values.get("max_delay_ms")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def min_delay_ms(self) -> typing.Optional[jsii.Number]:
+        '''The minimum delay between retry requests in milliseconds.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#min_delay_ms DataHttp#min_delay_ms}
+        '''
+        result = self._values.get("min_delay_ms")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "DataHttpRetry(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class DataHttpRetryOutputReference(
+    _cdktf_9a9027ec.ComplexObject,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdktf/provider-http.dataHttp.DataHttpRetryOutputReference",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__2cf266833e9dd8e06f847ea44a4e068fb0ee801803b7ebef25f70a7de5dfcd02)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
+
+    @jsii.member(jsii_name="resetAttempts")
+    def reset_attempts(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetAttempts", []))
+
+    @jsii.member(jsii_name="resetMaxDelayMs")
+    def reset_max_delay_ms(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetMaxDelayMs", []))
+
+    @jsii.member(jsii_name="resetMinDelayMs")
+    def reset_min_delay_ms(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetMinDelayMs", []))
+
+    @builtins.property
+    @jsii.member(jsii_name="attemptsInput")
+    def attempts_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "attemptsInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="maxDelayMsInput")
+    def max_delay_ms_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "maxDelayMsInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="minDelayMsInput")
+    def min_delay_ms_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "minDelayMsInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attempts")
+    def attempts(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "attempts"))
+
+    @attempts.setter
+    def attempts(self, value: jsii.Number) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ba6ceaf9624235fec7754791a324617747f68d6b3bc1dcfb74de6d279a0aa7ef)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "attempts", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="maxDelayMs")
+    def max_delay_ms(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "maxDelayMs"))
+
+    @max_delay_ms.setter
+    def max_delay_ms(self, value: jsii.Number) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__f5f294fe63a7fd316b6ec5164799a68a0d8639c0e2fc23d8bd552231c0f7d60a)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "maxDelayMs", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="minDelayMs")
+    def min_delay_ms(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "minDelayMs"))
+
+    @min_delay_ms.setter
+    def min_delay_ms(self, value: jsii.Number) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__5d59f2427a3deeb5b67ceab4f858492ff5754a45bc2792465bae30603cbe442f)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "minDelayMs", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="internalValue")
+    def internal_value(
+        self,
+    ) -> typing.Optional[typing.Union[DataHttpRetry, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[DataHttpRetry, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
+
+    @internal_value.setter
+    def internal_value(
+        self,
+        value: typing.Optional[typing.Union[DataHttpRetry, _cdktf_9a9027ec.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8a2d49cc40232891cff2e743c36c379a77b753843ddef54acaa1aa0c95341d88)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "internalValue", value)
+
+
 __all__ = [
     "DataHttp",
     "DataHttpConfig",
+    "DataHttpRetry",
+    "DataHttpRetryOutputReference",
 ]
 
 publication.publish()
 
 def _typecheckingstub__d6cd955bd349cdf3bff4e55c988ca69502aeda8b1ad29c58e5fc66c185056a1f(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     url: builtins.str,
     ca_cert_pem: typing.Optional[builtins.str] = None,
     insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     method: typing.Optional[builtins.str] = None,
     request_body: typing.Optional[builtins.str] = None,
     request_headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    request_timeout_ms: typing.Optional[jsii.Number] = None,
+    retry: typing.Optional[typing.Union[DataHttpRetry, typing.Dict[builtins.str, typing.Any]]] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
@@ -542,14 +817,20 @@
 
 def _typecheckingstub__1a74bd45d9b8a30578befabcf666ca96bd1f9bef3b6e84638b0934128d782b51(
     value: typing.Mapping[builtins.str, builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__56342ca3a5f8a383c7aa7363c40000689eb017e1d4a08f440bf27cac06150376(
+    value: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__63c7570b908cd9916d86ef50e54da516dfc1d30d4f00a51c428bab8efd6bef04(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ee2b6a3664a80e642a2ef1d255302a3f3dc3d391999cb8f3d6103cac8420d573(
@@ -563,10 +844,52 @@
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     url: builtins.str,
     ca_cert_pem: typing.Optional[builtins.str] = None,
     insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     method: typing.Optional[builtins.str] = None,
     request_body: typing.Optional[builtins.str] = None,
     request_headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    request_timeout_ms: typing.Optional[jsii.Number] = None,
+    retry: typing.Optional[typing.Union[DataHttpRetry, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5db3ea948028eba5857abc78a333d807c1e084b83b50b80801b01c9a63f2d524(
+    *,
+    attempts: typing.Optional[jsii.Number] = None,
+    max_delay_ms: typing.Optional[jsii.Number] = None,
+    min_delay_ms: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2cf266833e9dd8e06f847ea44a4e068fb0ee801803b7ebef25f70a7de5dfcd02(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ba6ceaf9624235fec7754791a324617747f68d6b3bc1dcfb74de6d279a0aa7ef(
+    value: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__f5f294fe63a7fd316b6ec5164799a68a0d8639c0e2fc23d8bd552231c0f7d60a(
+    value: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5d59f2427a3deeb5b67ceab4f858492ff5754a45bc2792465bae30603cbe442f(
+    value: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8a2d49cc40232891cff2e743c36c379a77b753843ddef54acaa1aa0c95341d88(
+    value: typing.Optional[typing.Union[DataHttpRetry, _cdktf_9a9027ec.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/provider/__init__.py` & `cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http/provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`http`](https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs).
+Refer to the Terraform Registory for docs: [`http`](https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,28 +22,28 @@
 
 
 class HttpProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-http.provider.HttpProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs http}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs http}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs http} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs http} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs#alias HttpProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs#alias HttpProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ed4656733258f821890abe9b576315755fbb2c26c5225d063440932e3244ec0a)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = HttpProviderConfig(alias=alias)
 
@@ -84,28 +84,28 @@
     jsii_type="@cdktf/provider-http.provider.HttpProviderConfig",
     jsii_struct_bases=[],
     name_mapping={"alias": "alias"},
 )
 class HttpProviderConfig:
     def __init__(self, *, alias: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs#alias HttpProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs#alias HttpProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c5e292f1b2ced23926cb25076c6e327c7591be5943163c3c72b898964467f963)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if alias is not None:
             self._values["alias"] = alias
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs#alias HttpProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs#alias HttpProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO` & `cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-http
-Version: 4.0.0
+Version: 4.0.1
 Summary: Prebuilt http Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-http.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-http.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-http-4.0.1/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 src/cdktf_cdktf_provider_http/py.typed
 src/cdktf_cdktf_provider_http.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_http.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_http.egg-info/requires.txt
 src/cdktf_cdktf_provider_http.egg-info/top_level.txt
 src/cdktf_cdktf_provider_http/_jsii/__init__.py
-src/cdktf_cdktf_provider_http/_jsii/provider-http@4.0.0.jsii.tgz
+src/cdktf_cdktf_provider_http/_jsii/provider-http@4.0.1.jsii.tgz
 src/cdktf_cdktf_provider_http/data_http/__init__.py
 src/cdktf_cdktf_provider_http/provider/__init__.py
```

