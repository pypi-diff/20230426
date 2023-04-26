# Comparing `tmp/qdrant_client-1.1.5.tar.gz` & `tmp/qdrant_client-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_client-1.1.5.tar", max compression
+gzip compressed data, was "qdrant_client-1.1.6.tar", max compression
```

## Comparing `qdrant_client-1.1.5.tar` & `qdrant_client-1.1.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    11357 2023-04-19 14:31:07.696748 qdrant_client-1.1.5/LICENSE
--rw-r--r--   0        0        0     5690 2023-04-19 14:31:07.696748 qdrant_client-1.1.5/README.md
--rw-r--r--   0        0        0     1277 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/pyproject.toml
--rw-r--r--   0        0        0       56 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/__init__.py
--rw-r--r--   0        0        0    25845 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/client_base.py
--rw-r--r--   0        0        0     4459 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/connection.py
--rw-r--r--   0        0        0        0 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/conversions/__init__.py
--rw-r--r--   0        0        0     3231 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/conversions/common_types.py
--rw-r--r--   0        0        0    62445 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/conversions/conversion.py
--rw-r--r--   0        0        0      252 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/__init__.py
--rw-r--r--   0        0        0    28633 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/collections_pb2.py
--rw-r--r--   0        0        0      159 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/collections_pb2_grpc.py
--rw-r--r--   0        0        0     1794 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/collections_service_pb2.py
--rw-r--r--   0        0        0    13456 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/collections_service_pb2_grpc.py
--rw-r--r--   0        0        0     3395 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/json_with_int_pb2.py
--rw-r--r--   0        0        0      159 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/json_with_int_pb2_grpc.py
--rw-r--r--   0        0        0    44493 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/points_pb2.py
--rw-r--r--   0        0        0      159 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/points_pb2_grpc.py
--rw-r--r--   0        0        0     2502 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/points_service_pb2.py
--rw-r--r--   0        0        0    23694 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/points_service_pb2_grpc.py
--rw-r--r--   0        0        0     2254 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/qdrant_pb2.py
--rw-r--r--   0        0        0     2411 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/qdrant_pb2_grpc.py
--rw-r--r--   0        0        0     7768 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/snapshots_service_pb2.py
--rw-r--r--   0        0        0    10406 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/grpc/snapshots_service_pb2_grpc.py
--rw-r--r--   0        0        0      505 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api/__init__.py
--rw-r--r--   0        0        0    10437 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api/cluster_api.py
--rw-r--r--   0        0        0    30407 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api/collections_api.py
--rw-r--r--   0        0        0    30820 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api/points_api.py
--rw-r--r--   0        0        0     9499 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api/service_api.py
--rw-r--r--   0        0        0    18850 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api/snapshots_api.py
--rw-r--r--   0        0        0     7577 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/api_client.py
--rw-r--r--   0        0        0      233 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/configuration.py
--rw-r--r--   0        0        0     1616 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/exceptions.py
--rw-r--r--   0        0        0       22 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/models/__init__.py
--rw-r--r--   0        0        0    60032 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/http/models/models.py
--rw-r--r--   0        0        0        0 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/local/__init__.py
--rw-r--r--   0        0        0     2962 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/local/distances.py
--rw-r--r--   0        0        0     1446 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/local/geo.py
--rw-r--r--   0        0        0    21902 2023-04-19 14:31:07.700748 qdrant_client-1.1.5/qdrant_client/local/local_collection.py
--rw-r--r--   0        0        0     5888 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/local/payload_filters.py
--rw-r--r--   0        0        0     2922 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/local/payload_value_extractor.py
--rw-r--r--   0        0        0     2237 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/local/persistence.py
--rw-r--r--   0        0        0    18939 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/local/qdrant_local.py
--rw-r--r--   0        0        0       40 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/models/__init__.py
--rw-r--r--   0        0        0     7034 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/parallel_processor.py
--rw-r--r--   0        0        0    10979 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/collections.proto
--rw-r--r--   0        0        0     1168 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/collections_service.proto
--rw-r--r--   0        0        0     1936 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/json_with_int.proto
--rw-r--r--   0        0        0    14566 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/points.proto
--rw-r--r--   0        0        0     2196 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/points_service.proto
--rw-r--r--   0        0        0      331 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/qdrant.proto
--rw-r--r--   0        0        0     1895 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/proto/snapshots_service.proto
--rw-r--r--   0        0        0        8 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/py.typed
--rw-r--r--   0        0        0    54281 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/qdrant_client.py
--rw-r--r--   0        0        0    88752 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/qdrant_remote.py
--rw-r--r--   0        0        0        0 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/uploader/__init__.py
--rw-r--r--   0        0        0     2865 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/uploader/grpc_uploader.py
--rw-r--r--   0        0        0     2537 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/uploader/rest_uploader.py
--rw-r--r--   0        0        0     3200 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_client/uploader/uploader.py
--rw-r--r--   0        0        0      267 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/__init__.py
--rw-r--r--   0        0        0       37 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/api/__init__.py
--rw-r--r--   0        0        0       53 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/api/collections_api.py
--rw-r--r--   0        0        0       48 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/api/points_api.py
--rw-r--r--   0        0        0       44 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/exceptions.py
--rw-r--r--   0        0        0       47 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/models/__init__.py
--rw-r--r--   0        0        0       47 2023-04-19 14:31:07.704748 qdrant_client-1.1.5/qdrant_openapi_client/models/models.py
--rw-r--r--   0        0        0     6749 1970-01-01 00:00:00.000000 qdrant_client-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/LICENSE
+-rw-r--r--   0        0        0     6250 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/README.md
+-rw-r--r--   0        0        0     1304 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/qdrant_client/__init__.py
+-rw-r--r--   0        0        0    25845 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/qdrant_client/client_base.py
+-rw-r--r--   0        0        0     9363 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/qdrant_client/connection.py
+-rw-r--r--   0        0        0        0 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/qdrant_client/conversions/__init__.py
+-rw-r--r--   0        0        0     3231 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/qdrant_client/conversions/common_types.py
+-rw-r--r--   0        0        0    62445 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/conversions/conversion.py
+-rw-r--r--   0        0        0      252 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/__init__.py
+-rw-r--r--   0        0        0    28633 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/collections_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/collections_pb2_grpc.py
+-rw-r--r--   0        0        0     1794 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/collections_service_pb2.py
+-rw-r--r--   0        0        0    13456 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/collections_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3395 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/json_with_int_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/json_with_int_pb2_grpc.py
+-rw-r--r--   0        0        0    44493 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/points_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/points_pb2_grpc.py
+-rw-r--r--   0        0        0     2502 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/points_service_pb2.py
+-rw-r--r--   0        0        0    23694 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/points_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2254 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/qdrant_pb2.py
+-rw-r--r--   0        0        0     2411 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/qdrant_pb2_grpc.py
+-rw-r--r--   0        0        0     7768 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/snapshots_service_pb2.py
+-rw-r--r--   0        0        0    10406 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/snapshots_service_pb2_grpc.py
+-rw-r--r--   0        0        0      505 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api/__init__.py
+-rw-r--r--   0        0        0    10437 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api/cluster_api.py
+-rw-r--r--   0        0        0    30407 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api/collections_api.py
+-rw-r--r--   0        0        0    30820 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api/points_api.py
+-rw-r--r--   0        0        0     9499 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api/service_api.py
+-rw-r--r--   0        0        0    18850 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api/snapshots_api.py
+-rw-r--r--   0        0        0     7577 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api_client.py
+-rw-r--r--   0        0        0      233 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/configuration.py
+-rw-r--r--   0        0        0     1616 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/exceptions.py
+-rw-r--r--   0        0        0       22 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/models/__init__.py
+-rw-r--r--   0        0        0    60032 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/models/models.py
+-rw-r--r--   0        0        0        0 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/__init__.py
+-rw-r--r--   0        0        0     2962 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/distances.py
+-rw-r--r--   0        0        0     1446 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/geo.py
+-rw-r--r--   0        0        0    21902 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/local_collection.py
+-rw-r--r--   0        0        0     5888 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/payload_filters.py
+-rw-r--r--   0        0        0     2922 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/payload_value_extractor.py
+-rw-r--r--   0        0        0     2237 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/persistence.py
+-rw-r--r--   0        0        0    18939 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/qdrant_local.py
+-rw-r--r--   0        0        0       40 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/models/__init__.py
+-rw-r--r--   0        0        0     7034 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/parallel_processor.py
+-rw-r--r--   0        0        0    10979 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/collections.proto
+-rw-r--r--   0        0        0     1168 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/collections_service.proto
+-rw-r--r--   0        0        0     1936 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/json_with_int.proto
+-rw-r--r--   0        0        0    14566 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/points.proto
+-rw-r--r--   0        0        0     2196 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/points_service.proto
+-rw-r--r--   0        0        0      331 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/qdrant.proto
+-rw-r--r--   0        0        0     1895 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/snapshots_service.proto
+-rw-r--r--   0        0        0        8 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/py.typed
+-rw-r--r--   0        0        0    55103 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/qdrant_client.py
+-rw-r--r--   0        0        0    90192 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/qdrant_remote.py
+-rw-r--r--   0        0        0        0 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/uploader/__init__.py
+-rw-r--r--   0        0        0     2865 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/uploader/grpc_uploader.py
+-rw-r--r--   0        0        0     2537 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/uploader/rest_uploader.py
+-rw-r--r--   0        0        0     3200 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/uploader/uploader.py
+-rw-r--r--   0        0        0      267 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/api/__init__.py
+-rw-r--r--   0        0        0       53 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/api/collections_api.py
+-rw-r--r--   0        0        0       48 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/api/points_api.py
+-rw-r--r--   0        0        0       44 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/exceptions.py
+-rw-r--r--   0        0        0       47 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/models/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/models/models.py
+-rw-r--r--   0        0        0     7309 1970-01-01 00:00:00.000000 qdrant_client-1.1.6/PKG-INFO
```

### Comparing `qdrant_client-1.1.5/LICENSE` & `qdrant_client-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/README.md` & `qdrant_client-1.1.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -182,14 +182,35 @@
 ```python
 from qdrant_client import QdrantClient
 
 client = QdrantClient(host="localhost", grpc_port=6334, prefer_grpc=True)
 ```
 
 
+## Async client
+
+Async methods are available in raw autogenerated clients.
+Usually, you don't need to use them directly, but if you need extra performance, you can access them directly.
+
+### Async gRPC
+
+Example of using raw async gRPC client:
+
+```python
+from qdrant_client import QdrantClient, grpc
+
+client = QdrantClient(prefer_grpc=True, timeout=3.0)
+
+grpc_collections = client.async_grpc_collections
+
+res = await grpc_collections.List(grpc.ListCollectionsRequest(), timeout=1.0)
+```
+
+More examples can be found [here](./tests/test_async_qdrant_client.py).
+
 ### Development
 
 This project uses git hooks to run code formatters.
 
 Install `pre-commit` with `pip3 install pre-commit` and set up hooks with `pre-commit install`.
 
 > pre-commit requires python>=3.8
```

#### html2text {}

```diff
@@ -51,10 +51,18 @@
 required for search results FieldCondition( key='rand_number', # Condition
 based on values of `rand_number` field. range=Range( gte=3 # Select only those
 results where `rand_number` >= 3 ) ) ] ), limit=5 # Return 5 closest points )
 ``` See more examples in our [Documentation](https://qdrant.tech/documentation/
 )! ### gRPC To enable (typically, much faster) collection uploading with gRPC,
 use the following initialization: ```python from qdrant_client import
 QdrantClient client = QdrantClient(host="localhost", grpc_port=6334,
-prefer_grpc=True) ``` ### Development This project uses git hooks to run code
-formatters. Install `pre-commit` with `pip3 install pre-commit` and set up
-hooks with `pre-commit install`. > pre-commit requires python>=3.8
+prefer_grpc=True) ``` ## Async client Async methods are available in raw
+autogenerated clients. Usually, you don't need to use them directly, but if you
+need extra performance, you can access them directly. ### Async gRPC Example of
+using raw async gRPC client: ```python from qdrant_client import QdrantClient,
+grpc client = QdrantClient(prefer_grpc=True, timeout=3.0) grpc_collections =
+client.async_grpc_collections res = await grpc_collections.List
+(grpc.ListCollectionsRequest(), timeout=1.0) ``` More examples can be found
+[here](./tests/test_async_qdrant_client.py). ### Development This project uses
+git hooks to run code formatters. Install `pre-commit` with `pip3 install pre-
+commit` and set up hooks with `pre-commit install`. > pre-commit requires
+python>=3.8
```

### Comparing `qdrant_client-1.1.5/pyproject.toml` & `qdrant_client-1.1.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qdrant-client"
-version = "1.1.5"
+version = "1.1.6"
 description = "Client library for the Qdrant vector search engine"
 authors = ["Andrey Vasnetsov <andrey@qdrant.tech>"]
 packages = [
     {include = "qdrant_client"},
     {include = "qdrant_openapi_client"}
 ]
 readme = "README.md"
@@ -27,14 +27,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1"
 grpcio-tools = "^1.46.0"
 sphinx = "^4.4.0"
 qdrant-sphinx-theme = { git = "https://github.com/qdrant/qdrant_sphinx_theme.git", branch = "master" }
 coverage = "^6.3.3"
+pytest-asyncio = "^0.21.0"
 
 [tool.poetry.group.types.dependencies]
 pyright = "^1.1.293"
 mypy = "^1.0.0"
 types-protobuf = "^4.21.0.5"
```

### Comparing `qdrant_client-1.1.5/qdrant_client/client_base.py` & `qdrant_client-1.1.6/qdrant_client/client_base.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/conversions/common_types.py` & `qdrant_client-1.1.6/qdrant_client/conversions/common_types.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/conversions/conversion.py` & `qdrant_client-1.1.6/qdrant_client/conversions/conversion.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/grpc/collections_pb2.py` & `qdrant_client-1.1.6/qdrant_client/grpc/collections_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/grpc/collections_service_pb2.py` & `qdrant_client-1.1.6/qdrant_client/grpc/collections_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/grpc/collections_service_pb2_grpc.py` & `qdrant_client-1.1.6/qdrant_client/grpc/collections_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/grpc/json_with_int_pb2.py` & `qdrant_client-1.1.6/qdrant_client/grpc/json_with_int_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/grpc/points_pb2.py` & `qdrant_client-1.1.6/qdrant_client/grpc/points_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/grpc/points_service_pb2.py` & `qdrant_client-1.1.6/qdrant_client/grpc/points_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/grpc/points_service_pb2_grpc.py` & `qdrant_client-1.1.6/qdrant_client/grpc/points_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/grpc/qdrant_pb2.py` & `qdrant_client-1.1.6/qdrant_client/grpc/qdrant_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/grpc/qdrant_pb2_grpc.py` & `qdrant_client-1.1.6/qdrant_client/grpc/qdrant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/grpc/snapshots_service_pb2.py` & `qdrant_client-1.1.6/qdrant_client/grpc/snapshots_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/grpc/snapshots_service_pb2_grpc.py` & `qdrant_client-1.1.6/qdrant_client/grpc/snapshots_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/http/api/cluster_api.py` & `qdrant_client-1.1.6/qdrant_client/http/api/cluster_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/http/api/collections_api.py` & `qdrant_client-1.1.6/qdrant_client/http/api/collections_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/http/api/points_api.py` & `qdrant_client-1.1.6/qdrant_client/http/api/points_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/http/api/service_api.py` & `qdrant_client-1.1.6/qdrant_client/http/api/service_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/http/api/snapshots_api.py` & `qdrant_client-1.1.6/qdrant_client/http/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/http/api_client.py` & `qdrant_client-1.1.6/qdrant_client/http/api_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/http/exceptions.py` & `qdrant_client-1.1.6/qdrant_client/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/http/models/models.py` & `qdrant_client-1.1.6/qdrant_client/http/models/models.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/local/distances.py` & `qdrant_client-1.1.6/qdrant_client/local/distances.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/local/geo.py` & `qdrant_client-1.1.6/qdrant_client/local/geo.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/local/local_collection.py` & `qdrant_client-1.1.6/qdrant_client/local/local_collection.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/local/payload_filters.py` & `qdrant_client-1.1.6/qdrant_client/local/payload_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/local/payload_value_extractor.py` & `qdrant_client-1.1.6/qdrant_client/local/payload_value_extractor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/local/persistence.py` & `qdrant_client-1.1.6/qdrant_client/local/persistence.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/local/qdrant_local.py` & `qdrant_client-1.1.6/qdrant_client/local/qdrant_local.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/parallel_processor.py` & `qdrant_client-1.1.6/qdrant_client/parallel_processor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/proto/collections.proto` & `qdrant_client-1.1.6/qdrant_client/proto/collections.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/proto/collections_service.proto` & `qdrant_client-1.1.6/qdrant_client/proto/collections_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/proto/json_with_int.proto` & `qdrant_client-1.1.6/qdrant_client/proto/json_with_int.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/proto/points.proto` & `qdrant_client-1.1.6/qdrant_client/proto/points.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/proto/points_service.proto` & `qdrant_client-1.1.6/qdrant_client/proto/points_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/proto/snapshots_service.proto` & `qdrant_client-1.1.6/qdrant_client/proto/snapshots_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/qdrant_client.py` & `qdrant_client-1.1.6/qdrant_client/qdrant_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,38 @@
         """
         if isinstance(self._client, QdrantRemote):
             return self._client.grpc_points
 
         raise NotImplementedError(f"gRPC client is not supported for {type(self._client)}")
 
     @property
+    def async_grpc_points(self) -> grpc.PointsStub:
+        """gRPC client for points methods
+
+        Returns:
+            An instance of raw gRPC client, generated from Protobuf
+        """
+        if isinstance(self._client, QdrantRemote):
+            return self._client.async_grpc_points
+
+        raise NotImplementedError(f"gRPC client is not supported for {type(self._client)}")
+
+    @property
+    def async_grpc_collections(self) -> grpc.CollectionsStub:
+        """gRPC client for collections methods
+
+        Returns:
+            An instance of raw gRPC client, generated from Protobuf
+        """
+        if isinstance(self._client, QdrantRemote):
+            return self._client.async_grpc_collections
+
+        raise NotImplementedError(f"gRPC client is not supported for {type(self._client)}")
+
+    @property
     def rest(self) -> SyncApis[ApiClient]:
         """REST Client
 
         Returns:
             An instance of raw REST API client, generated from OpenAPI schema
         """
         if isinstance(self._client, QdrantRemote):
```

### Comparing `qdrant_client-1.1.5/qdrant_client/qdrant_remote.py` & `qdrant_client-1.1.6/qdrant_client/qdrant_remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import httpx
 import numpy as np
 from urllib3.util import Url, parse_url
 
 from qdrant_client import grpc as grpc
 from qdrant_client.client_base import QdrantBase
-from qdrant_client.connection import get_channel
+from qdrant_client.connection import get_async_channel, get_channel
 from qdrant_client.conversions import common_types as types
 from qdrant_client.conversions.conversion import GrpcToRest, RestToGrpc
 from qdrant_client.http import ApiClient, SyncApis
 from qdrant_client.http import models as rest_models
 from qdrant_client.parallel_processor import ParallelWorkerPool
 from qdrant_client.uploader.grpc_uploader import GrpcBatchUploader
 from qdrant_client.uploader.rest_uploader import RestBatchUploader
@@ -119,17 +119,18 @@
             self._rest_args["timeout"] = self._timeout
 
         self.openapi_client: SyncApis[ApiClient] = SyncApis(host=self.rest_uri, **self._rest_args)
 
         self._grpc_channel = None
         self._grpc_points_client: Optional[grpc.PointsStub] = None
         self._grpc_collections_client: Optional[grpc.CollectionsStub] = None
-        if prefer_grpc:
-            self._init_grpc_points_client(self._grpc_headers)
-            self._init_grpc_collections_client(self._grpc_headers)
+
+        self._aio_grpc_channel = None
+        self._aio_grpc_points_client: Optional[grpc.PointsStub] = None
+        self._aio_grpc_collections_client: Optional[grpc.CollectionsStub] = None
 
     def __del__(self) -> None:
         if hasattr(self, "_grpc_channel") and self._grpc_channel is not None:
             self._grpc_channel.close()
 
     @staticmethod
     def _parse_url(url: str) -> Tuple[Optional[str], str, Optional[int], Optional[str]]:
@@ -138,28 +139,64 @@
             parse_result.scheme,
             parse_result.host,
             parse_result.port,
             parse_result.path,
         )
         return scheme, host, port, prefix
 
-    def _init_grpc_points_client(self, metadata: Optional[List[Any]] = None) -> None:
+    def _init_grpc_points_client(self) -> None:
         if self._grpc_channel is None:
             self._grpc_channel = get_channel(
-                host=self._host, port=self._grpc_port, ssl=self._https, metadata=metadata
+                host=self._host, port=self._grpc_port, ssl=self._https, metadata=self._grpc_headers
             )
         self._grpc_points_client = grpc.PointsStub(self._grpc_channel)
 
-    def _init_grpc_collections_client(self, metadata: Optional[List[Any]] = None) -> None:
+    def _init_grpc_collections_client(self) -> None:
         if self._grpc_channel is None:
             self._grpc_channel = get_channel(
-                host=self._host, port=self._grpc_port, ssl=self._https, metadata=metadata
+                host=self._host, port=self._grpc_port, ssl=self._https, metadata=self._grpc_headers
             )
         self._grpc_collections_client = grpc.CollectionsStub(self._grpc_channel)
 
+    def _init_async_grpc_points_client(self) -> None:
+        if self._aio_grpc_channel is None:
+            self._aio_grpc_channel = get_async_channel(
+                host=self._host, port=self._grpc_port, ssl=self._https, metadata=self._grpc_headers
+            )
+        self._aio_grpc_points_client = grpc.PointsStub(self._aio_grpc_channel)
+
+    def _init_async_grpc_collections_client(self) -> None:
+        if self._aio_grpc_channel is None:
+            self._aio_grpc_channel = get_async_channel(
+                host=self._host, port=self._grpc_port, ssl=self._https, metadata=self._grpc_headers
+            )
+        self._aio_grpc_collections_client = grpc.CollectionsStub(self._aio_grpc_channel)
+
+    @property
+    def async_grpc_collections(self) -> grpc.CollectionsStub:
+        """gRPC client for collections methods
+
+        Returns:
+            An instance of raw gRPC client, generated from Protobuf
+        """
+        if self._aio_grpc_collections_client is None:
+            self._init_async_grpc_collections_client()
+        return self._aio_grpc_collections_client
+
+    @property
+    def async_grpc_points(self) -> grpc.PointsStub:
+        """gRPC client for points methods
+
+        Returns:
+            An instance of raw gRPC client, generated from Protobuf
+        """
+        if self._aio_grpc_points_client is None:
+            self._init_async_grpc_points_client()
+        return self._aio_grpc_points_client
+
     @property
     def grpc_collections(self) -> grpc.CollectionsStub:
         """gRPC client for collections methods
 
         Returns:
             An instance of raw gRPC client, generated from Protobuf
         """
```

### Comparing `qdrant_client-1.1.5/qdrant_client/uploader/grpc_uploader.py` & `qdrant_client-1.1.6/qdrant_client/uploader/grpc_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/uploader/rest_uploader.py` & `qdrant_client-1.1.6/qdrant_client/uploader/rest_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/qdrant_client/uploader/uploader.py` & `qdrant_client-1.1.6/qdrant_client/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.5/PKG-INFO` & `qdrant_client-1.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-client
-Version: 1.1.5
+Version: 1.1.6
 Summary: Client library for the Qdrant vector search engine
 Home-page: https://github.com/qdrant/qdrant-client
 Keywords: vector,search,neural,matching,client
 Author: Andrey Vasnetsov
 Author-email: andrey@qdrant.tech
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
@@ -208,14 +208,35 @@
 ```python
 from qdrant_client import QdrantClient
 
 client = QdrantClient(host="localhost", grpc_port=6334, prefer_grpc=True)
 ```
 
 
+## Async client
+
+Async methods are available in raw autogenerated clients.
+Usually, you don't need to use them directly, but if you need extra performance, you can access them directly.
+
+### Async gRPC
+
+Example of using raw async gRPC client:
+
+```python
+from qdrant_client import QdrantClient, grpc
+
+client = QdrantClient(prefer_grpc=True, timeout=3.0)
+
+grpc_collections = client.async_grpc_collections
+
+res = await grpc_collections.List(grpc.ListCollectionsRequest(), timeout=1.0)
+```
+
+More examples can be found [here](./tests/test_async_qdrant_client.py).
+
 ### Development
 
 This project uses git hooks to run code formatters.
 
 Install `pre-commit` with `pip3 install pre-commit` and set up hooks with `pre-commit install`.
 
 > pre-commit requires python>=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qdrant-client Version: 1.1.5 Summary: Client
+Metadata-Version: 2.1 Name: qdrant-client Version: 1.1.6 Summary: Client
 library for the Qdrant vector search engine Home-page: https://github.com/
 qdrant/qdrant-client Keywords: vector,search,neural,matching,client Author:
 Andrey Vasnetsov Author-email: andrey@qdrant.tech Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -66,10 +66,18 @@
 required for search results FieldCondition( key='rand_number', # Condition
 based on values of `rand_number` field. range=Range( gte=3 # Select only those
 results where `rand_number` >= 3 ) ) ] ), limit=5 # Return 5 closest points )
 ``` See more examples in our [Documentation](https://qdrant.tech/documentation/
 )! ### gRPC To enable (typically, much faster) collection uploading with gRPC,
 use the following initialization: ```python from qdrant_client import
 QdrantClient client = QdrantClient(host="localhost", grpc_port=6334,
-prefer_grpc=True) ``` ### Development This project uses git hooks to run code
-formatters. Install `pre-commit` with `pip3 install pre-commit` and set up
-hooks with `pre-commit install`. > pre-commit requires python>=3.8
+prefer_grpc=True) ``` ## Async client Async methods are available in raw
+autogenerated clients. Usually, you don't need to use them directly, but if you
+need extra performance, you can access them directly. ### Async gRPC Example of
+using raw async gRPC client: ```python from qdrant_client import QdrantClient,
+grpc client = QdrantClient(prefer_grpc=True, timeout=3.0) grpc_collections =
+client.async_grpc_collections res = await grpc_collections.List
+(grpc.ListCollectionsRequest(), timeout=1.0) ``` More examples can be found
+[here](./tests/test_async_qdrant_client.py). ### Development This project uses
+git hooks to run code formatters. Install `pre-commit` with `pip3 install pre-
+commit` and set up hooks with `pre-commit install`. > pre-commit requires
+python>=3.8
```

