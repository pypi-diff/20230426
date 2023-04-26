# Comparing `tmp/mythic_container-0.2.1.tar.gz` & `tmp/mythic_container-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic_container-0.2.1.tar", last modified: Tue Apr 25 19:38:55 2023, max compression
+gzip compressed data, was "mythic_container-0.2.2.tar", last modified: Wed Apr 26 17:35:56 2023, max compression
```

## Comparing `mythic_container-0.2.1.tar` & `mythic_container-0.2.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 19:38:55.566430 mythic_container-0.2.1/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.2.1/LICENSE.md
--rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2023-04-25 19:38:55.566192 mythic_container-0.2.1/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      993 2023-04-25 19:15:08.000000 mythic_container-0.2.1/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 19:38:55.538044 mythic_container-0.2.1/mythic_container/
--rw-r--r--   0 itsafeature   (501) staff       (20)    29960 2023-04-19 16:52:07.000000 mythic_container-0.2.1/mythic_container/C2ProfileBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    26032 2023-04-20 01:54:22.000000 mythic_container-0.2.1/mythic_container/LoggingBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    77811 2023-04-20 00:07:13.000000 mythic_container-0.2.1/mythic_container/MythicCommandBase.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 19:38:55.564539 mythic_container-0.2.1/mythic_container/MythicGoRPC/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2482 2023-04-01 06:52:48.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7424 2023-03-23 13:36:37.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2273 2023-04-04 02:07:20.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3182 2023-03-13 17:15:03.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-04-01 06:52:13.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2767 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1785 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4453 2023-04-13 18:13:16.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2216 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     6013 2023-04-01 05:24:39.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1748 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1327 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1318 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2072 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2659 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.2.1/mythic_container/MythicRPC.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    22324 2023-04-21 19:16:23.000000 mythic_container-0.2.1/mythic_container/PayloadBuilder.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7251 2023-04-19 16:38:54.000000 mythic_container-0.2.1/mythic_container/TranslationBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    13910 2023-04-25 19:08:24.000000 mythic_container-0.2.1/mythic_container/WebhookBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2577 2023-04-25 19:38:46.000000 mythic_container-0.2.1/mythic_container/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    36785 2023-04-21 19:16:40.000000 mythic_container-0.2.1/mythic_container/agent_utils.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    27738 2023-04-24 22:49:45.000000 mythic_container-0.2.1/mythic_container/c2_utils.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.2.1/mythic_container/config.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 19:38:55.565768 mythic_container-0.2.1/mythic_container/grpc/
--rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.2.1/mythic_container/grpc/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-02-21 13:59:33.000000 mythic_container-0.2.1/mythic_container/grpc/translationContainerGRPC_pb2.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-02-21 17:37:56.000000 mythic_container-0.2.1/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.2.1/mythic_container/logging.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4025 2023-04-19 23:39:10.000000 mythic_container-0.2.1/mythic_container/logging_utils.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)    28650 2023-04-25 19:14:22.000000 mythic_container-0.2.1/mythic_container/mythic_service.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    14498 2023-04-10 15:53:13.000000 mythic_container-0.2.1/mythic_container/rabbitmq.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.2.1/mythic_container/utils_mythic_file_transfer.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2821 2023-04-20 15:20:17.000000 mythic_container-0.2.1/mythic_container/webhook_utils.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 19:38:55.540162 mythic_container-0.2.1/mythic_container.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2023-04-25 19:38:55.000000 mythic_container-0.2.1/mythic_container.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)     4375 2023-04-25 19:38:55.000000 mythic_container-0.2.1/mythic_container.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-25 19:38:55.000000 mythic_container-0.2.1/mythic_container.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       95 2023-04-25 19:38:55.000000 mythic_container-0.2.1/mythic_container.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       17 2023-04-25 19:38:55.000000 mythic_container-0.2.1/mythic_container.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-25 19:38:55.566528 mythic_container-0.2.1/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1088 2023-04-25 19:38:30.000000 mythic_container-0.2.1/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-26 17:35:56.817836 mythic_container-0.2.2/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.2.2/LICENSE.md
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2023-04-26 17:35:56.817477 mythic_container-0.2.2/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      993 2023-04-25 19:15:08.000000 mythic_container-0.2.2/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-26 17:35:56.766323 mythic_container-0.2.2/mythic_container/
+-rw-r--r--   0 itsafeature   (501) staff       (20)    29960 2023-04-19 16:52:07.000000 mythic_container-0.2.2/mythic_container/C2ProfileBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    26032 2023-04-20 01:54:22.000000 mythic_container-0.2.2/mythic_container/LoggingBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    77811 2023-04-20 00:07:13.000000 mythic_container-0.2.2/mythic_container/MythicCommandBase.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-26 17:35:56.813747 mythic_container-0.2.2/mythic_container/MythicGoRPC/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2482 2023-04-01 06:52:48.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7424 2023-03-23 13:36:37.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2273 2023-04-04 02:07:20.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3309 2023-04-26 14:57:11.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-04-01 06:52:13.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2767 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1785 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4453 2023-04-13 18:13:16.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2216 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     6013 2023-04-01 05:24:39.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1748 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1327 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1318 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2072 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2659 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.2.2/mythic_container/MythicRPC.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    22324 2023-04-21 19:16:23.000000 mythic_container-0.2.2/mythic_container/PayloadBuilder.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7251 2023-04-19 16:38:54.000000 mythic_container-0.2.2/mythic_container/TranslationBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    13910 2023-04-25 19:08:24.000000 mythic_container-0.2.2/mythic_container/WebhookBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2573 2023-04-26 14:59:14.000000 mythic_container-0.2.2/mythic_container/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    36785 2023-04-21 19:16:40.000000 mythic_container-0.2.2/mythic_container/agent_utils.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    27738 2023-04-24 22:49:45.000000 mythic_container-0.2.2/mythic_container/c2_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.2.2/mythic_container/config.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-26 17:35:56.816068 mythic_container-0.2.2/mythic_container/grpc/
+-rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.2.2/mythic_container/grpc/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-02-21 13:59:33.000000 mythic_container-0.2.2/mythic_container/grpc/translationContainerGRPC_pb2.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-02-21 17:37:56.000000 mythic_container-0.2.2/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.2.2/mythic_container/logging.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4025 2023-04-19 23:39:10.000000 mythic_container-0.2.2/mythic_container/logging_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)    29459 2023-04-26 12:59:18.000000 mythic_container-0.2.2/mythic_container/mythic_service.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    14498 2023-04-10 15:53:13.000000 mythic_container-0.2.2/mythic_container/rabbitmq.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.2.2/mythic_container/utils_mythic_file_transfer.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2821 2023-04-20 15:20:17.000000 mythic_container-0.2.2/mythic_container/webhook_utils.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-26 17:35:56.768614 mythic_container-0.2.2/mythic_container.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2023-04-26 17:35:56.000000 mythic_container-0.2.2/mythic_container.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4375 2023-04-26 17:35:56.000000 mythic_container-0.2.2/mythic_container.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-26 17:35:56.000000 mythic_container-0.2.2/mythic_container.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       95 2023-04-26 17:35:56.000000 mythic_container-0.2.2/mythic_container.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       17 2023-04-26 17:35:56.000000 mythic_container-0.2.2/mythic_container.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-26 17:35:56.817989 mythic_container-0.2.2/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1088 2023-04-26 14:59:01.000000 mythic_container-0.2.2/setup.py
```

### Comparing `mythic_container-0.2.1/LICENSE.md` & `mythic_container-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/PKG-INFO` & `mythic_container-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic_container
-Version: 0.2.1
+Version: 0.2.2
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mythic_container-0.2.1/README.md` & `mythic_container-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/C2ProfileBase.py` & `mythic_container-0.2.2/mythic_container/C2ProfileBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/LoggingBase.py` & `mythic_container-0.2.2/mythic_container/LoggingBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicCommandBase.py` & `mythic_container-0.2.2/mythic_container/MythicCommandBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/__init__.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/__init__.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
                  IP: str = None,
                  ExternalIP: str = None,
                  IntegrityLevel: int = None,
                  OS: str = None,
                  Domain: str = None,
                  Architecture: str = None,
                  Description: str = None,
+                 ProcessName: str = None,
                  **kwargs):
         self.AgentCallbackUUID = AgentCallbackUUID
         self.CallbackID = CallbackID
         self.TaskID = TaskID
         self.EncryptionKeyBase64 = EncryptionKeyBase64
         self.DecryptionKeyBase64 = DecryptionKeyBase64
         self.CryptoType = CryptoType
@@ -39,14 +40,15 @@
         self.Ip = IP
         self.ExternalIP = ExternalIP
         self.IntegrityLevel = IntegrityLevel
         self.Os = OS
         self.Domain = Domain
         self.Architecture = Architecture
         self.Description = Description
+        self.ProcessName = ProcessName
         for k, v in kwargs.items():
             logger.info(f"Unknown kwarg {k} - {v}")
 
     def to_json(self):
         return {
             "agent_callback_id": self.AgentCallbackUUID,
             "callback_id": self.CallbackID,
@@ -61,15 +63,16 @@
             "sleep_info": self.SleepInfo,
             "ip": self.Ip,
             "external_ip": self.ExternalIP,
             "integrity_level": self.IntegrityLevel,
             "os": self.Os,
             "domain": self.Domain,
             "architecture": self.Architecture,
-            "description": self.Description
+            "description": self.Description,
+            "process_name": self.ProcessName
         }
 
 
 class MythicRPCCallbackUpdateMessageResponse:
     def __init__(self,
                  success: bool = False,
                  error: str = "",
```

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py` & `mythic_container-0.2.2/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/MythicRPC.py` & `mythic_container-0.2.2/mythic_container/MythicRPC.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/PayloadBuilder.py` & `mythic_container-0.2.2/mythic_container/PayloadBuilder.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/TranslationBase.py` & `mythic_container-0.2.2/mythic_container/TranslationBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/WebhookBase.py` & `mythic_container-0.2.2/mythic_container/WebhookBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/__init__.py` & `mythic_container-0.2.2/mythic_container/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .rabbitmq import rabbitmqConnectionClass
 from .mythic_service import start_and_run_forever, test_command
 
-containerVersion = "v1.0.0-rc9"
+containerVersion = "v1.0.0"
 
-PyPi_version = "0.2.1"
+PyPi_version = "0.2.2"
 
 RabbitmqConnection = rabbitmqConnectionClass()
 
 MYTHIC_RPC_OTHER_SERVICES_RPC = "mythic_rpc_other_service_rpc"
 PAYLOAD_BUILD_C2_ROUTING_KEY = "payload_c2_build"
 # payload routes
 PT_SYNC_ROUTING_KEY = "pt_sync"
```

### Comparing `mythic_container-0.2.1/mythic_container/agent_utils.py` & `mythic_container-0.2.2/mythic_container/agent_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/c2_utils.py` & `mythic_container-0.2.2/mythic_container/c2_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/grpc/translationContainerGRPC_pb2.py` & `mythic_container-0.2.2/mythic_container/grpc/translationContainerGRPC_pb2.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py` & `mythic_container-0.2.2/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/logging.py` & `mythic_container-0.2.2/mythic_container/logging.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/logging_utils.py` & `mythic_container-0.2.2/mythic_container/logging_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/mythic_service.py` & `mythic_container-0.2.2/mythic_container/mythic_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from . import TranslationBase
 from . import WebhookBase
 from . import LoggingBase
 from . import webhook_utils
 from . import logging_utils
 from .rabbitmq import failedConnectRetryDelay
 
-
 # set the global hostname variable
 output = ""
 
 
 # start our service
 def start_and_run_forever():
     try:
@@ -106,16 +105,18 @@
     modulePieces = pt.__module__.split(".")
     modulePrefix = ".".join(modulePieces[:-1])
     for cls in MythicCommandBase.CommandBase.__subclasses__():
         if cls.__module__.startswith(modulePrefix):
             logger.info(f"[*] Processing command {cls.cmd}")
             if pt.name not in MythicCommandBase.commands:
                 MythicCommandBase.commands[pt.name] = []
-            MythicCommandBase.commands[pt.name].append(cls(pt.agent_path, pt.agent_code_path, pt.agent_browserscript_path))
-            syncMessage["commands"].append(cls(pt.agent_path, pt.agent_code_path, pt.agent_browserscript_path).to_json())
+            MythicCommandBase.commands[pt.name].append(
+                cls(pt.agent_path, pt.agent_code_path, pt.agent_browserscript_path))
+            syncMessage["commands"].append(
+                cls(pt.agent_path, pt.agent_code_path, pt.agent_browserscript_path).to_json())
     while True:
         response = await mythic_container.RabbitmqConnection.SendRPCDictMessage(
             queue=mythic_container.PT_SYNC_ROUTING_KEY,
             body=syncMessage)
         if response is None:
             logger.error("[-] Failed to get a response back from syncing RPC message, trying again...")
             await asyncio.sleep(failedConnectRetryDelay)
@@ -243,97 +244,113 @@
         else:
             logger.info(f"[+] Successfully synced {tr.name}")
             return
 
 
 async def syncWebhookData(wb: WebhookBase.Webhook) -> None:
     if wb.new_startup is not None and callable(wb.new_startup):
-        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
-            queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_STARTUP),
-            routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_STARTUP),
-            handler=webhook_utils.new_startup
-        )))
+        payloadQueueTasks.append(
+            asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+                queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_STARTUP),
+                routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_STARTUP),
+                handler=webhook_utils.new_startup
+            )))
     if wb.new_callback is not None and callable(wb.new_callback):
-        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
-            queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_CALLBACK),
-            routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_CALLBACK),
-            handler=webhook_utils.new_callback
-        )))
+        payloadQueueTasks.append(
+            asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+                queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_CALLBACK),
+                routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_CALLBACK),
+                handler=webhook_utils.new_callback
+            )))
     if wb.new_feedback is not None and callable(wb.new_feedback):
-        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
-            queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_FEEDBACK),
-            routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_FEEDBACK),
-            handler=webhook_utils.new_feedback
-        )))
+        payloadQueueTasks.append(
+            asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+                queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_FEEDBACK),
+                routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_FEEDBACK),
+                handler=webhook_utils.new_feedback
+            )))
     if wb.new_alert is not None and callable(wb.new_alert):
-        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
-            queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_ALERT),
-            routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_ALERT),
-            handler=webhook_utils.new_alert
-        )))
+        payloadQueueTasks.append(
+            asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+                queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_ALERT),
+                routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_ALERT),
+                handler=webhook_utils.new_alert
+            )))
     if wb.new_custom is not None and callable(wb.new_custom):
-        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
-            queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_CUSTOM),
-            routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_CUSTOM),
-            handler=webhook_utils.new_custom
-        )))
+        payloadQueueTasks.append(
+            asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+                queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_CUSTOM),
+                routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_CUSTOM),
+                handler=webhook_utils.new_custom
+            )))
     logger.info(f"Successfully started webhook service")
 
 
 async def syncLoggingData(wb: LoggingBase.Log) -> None:
     if wb.new_callback is not None and callable(wb.new_callback):
-        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
-            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_CALLBACK),
-            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_CALLBACK),
-            handler=logging_utils.new_callback
-        )))
+        payloadQueueTasks.append(
+            asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+                queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_CALLBACK),
+                routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_CALLBACK),
+                handler=logging_utils.new_callback
+            )))
     if wb.new_credential is not None and callable(wb.new_credential):
-        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
-            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_CREDENTIAL),
-            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_CREDENTIAL),
-            handler=logging_utils.new_credential
-        )))
+        payloadQueueTasks.append(
+            asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+                queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_CREDENTIAL),
+                routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_CREDENTIAL),
+                handler=logging_utils.new_credential
+            )))
     if wb.new_keylog is not None and callable(wb.new_keylog):
-        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
-            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_KEYLOG),
-            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_KEYLOG),
-            handler=logging_utils.new_keylog
-        )))
+        payloadQueueTasks.append(
+            asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+                queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_KEYLOG),
+                routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_KEYLOG),
+                handler=logging_utils.new_keylog
+            )))
     if wb.new_file is not None and callable(wb.new_file):
-        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
-            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_FILE),
-            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_FILE),
-            handler=logging_utils.new_file
-        )))
+        payloadQueueTasks.append(
+            asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+                queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_FILE),
+                routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_FILE),
+                handler=logging_utils.new_file
+            )))
     if wb.new_payload is not None and callable(wb.new_payload):
-        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
-            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_PAYLOAD),
-            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_PAYLOAD),
-            handler=logging_utils.new_payload
-        )))
+        payloadQueueTasks.append(
+            asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+                queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_PAYLOAD),
+                routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_PAYLOAD),
+                handler=logging_utils.new_payload
+            )))
     if wb.new_artifact is not None and callable(wb.new_artifact):
-        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
-            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_ARTIFACT),
-            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_ARTIFACT),
-            handler=logging_utils.new_artifact
-        )))
+        payloadQueueTasks.append(
+            asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+                queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_ARTIFACT),
+                routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_ARTIFACT),
+                handler=logging_utils.new_artifact
+            )))
     if wb.new_task is not None and callable(wb.new_task):
-        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
-            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_TASK),
-            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_TASK),
-            handler=logging_utils.new_task
-        )))
+        payloadQueueTasks.append(
+            asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+                queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_TASK),
+                routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_TASK),
+                handler=logging_utils.new_task
+            )))
 
     logger.info(f"Successfully started logging service")
 
+
 consumingServices = []
+
+
 async def start_services():
     initialize()
 
-    logger.info(f"[+] Starting Services with version {mythic_container.containerVersion} and PyPi version {mythic_container.PyPi_version}\n")
+    logger.info(
+        f"[+] Starting Services with version {mythic_container.containerVersion} and PyPi version {mythic_container.PyPi_version}\n")
     webhook_services = WebhookBase.Webhook.__subclasses__()
     for cls in webhook_services:
         logger.info(f"[*] Processing webhook service")
         webhook = cls()
         consumingServices.append(webhook)
         await syncWebhookData(webhook)
     logging_services = LoggingBase.Log.__subclasses__()
@@ -384,29 +401,30 @@
                        task_id: int = None,
                        tasking_location: str = "command_line",
                        parameters_string: str = None,
                        parameters_dictionary: dict = None):
     logger.info(f"[*] Started testing {payload_type_name}'s {command_name} command")
     if operation_name is None or task_id is None:
         logger.info(f"[*] Specify an operation_name and task_id to get real data for testing."
-                     f"\nThis does not adjust your specified command/parameters, but allows MythicRPC calls to work properly")
+                    f"\nThis does not adjust your specified command/parameters, but allows MythicRPC calls to work properly")
     params = parameters_string
     if parameters_dictionary is not None:
         params = json.dumps(parameters_dictionary)
     payloadTypes = PayloadBuilder.PayloadType.__subclasses__()
     for cls in payloadTypes:
         payload_type = cls()
         if payload_type.name == payload_type_name:
             logger.info(f"[+] Found payload type: {payload_type.name}")
             modulePieces = payload_type.__module__.split(".")
             modulePrefix = ".".join(modulePieces[:-1])
             for cmdcls in MythicCommandBase.CommandBase.__subclasses__():
                 if cmdcls.__module__.startswith(modulePrefix):
                     if cmdcls.cmd == command_name:
-                        commandInstance = cmdcls(payload_type.agent_path, payload_type.agent_code_path, payload_type.agent_browserscript_path)
+                        commandInstance = cmdcls(payload_type.agent_path, payload_type.agent_code_path,
+                                                 payload_type.agent_browserscript_path)
                         logger.info(f"[+] Found command: {commandInstance.cmd}")
                         opsecPre = MythicCommandBase.PTTaskMessageAllData(
                             task={
                                 "tasking_location": tasking_location,
                                 "params": params,
                                 "original_params": params
                             },
@@ -426,46 +444,52 @@
                                 "tasking_location": tasking_location,
                                 "params": params,
                                 "original_params": params
                             },
                             args=cmdcls.argument_class
                         )
                         if operation_name is None or task_id is None:
-                            logger.info(f"[*] operation_name is None, testing with fake data. Some MythicRPC functions might not work")
+                            logger.info(
+                                f"[*] operation_name is None, testing with fake data. Some MythicRPC functions might not work")
                         else:
                             logger.info(f"[*] Fetching information for task {task_id} of operation {operation_name}")
-                            fetchResp = await MythicGoRPC.SendMythicRPCTaskDisplayToRealIdSearch(MythicGoRPC.MythicRPCTaskDisplayToRealIdSearchMessage(
-                                TaskDisplayID=task_id,
-                                OperationName=operation_name
-                            ))
+                            fetchResp = await MythicGoRPC.SendMythicRPCTaskDisplayToRealIdSearch(
+                                MythicGoRPC.MythicRPCTaskDisplayToRealIdSearchMessage(
+                                    TaskDisplayID=task_id,
+                                    OperationName=operation_name
+                                ))
                             if not fetchResp.Success:
                                 logger.error(f"[-] Failed to find task: {fetchResp.Error}")
                                 sys.exit(1)
                             else:
-                                taskResp = await MythicGoRPC.SendMythicRPCTaskSearch(MythicGoRPC.MythicRPCTaskSearchMessage(
-                                    TaskID=fetchResp.TaskID,
-                                ))
+                                taskResp = await MythicGoRPC.SendMythicRPCTaskSearch(
+                                    MythicGoRPC.MythicRPCTaskSearchMessage(
+                                        TaskID=fetchResp.TaskID,
+                                    ))
                                 if not taskResp.Success:
                                     logger.error(f"[-] Failed to get task information: {taskResp.Error}")
                                     sys.exit(1)
                                 elif len(taskResp.Tasks) == 0:
                                     logger.error(f"[-] Failed to search for task information")
                                     sys.exit(1)
                                 else:
-                                    opsecPre.Task = MythicCommandBase.PTTaskMessageTaskData(**taskResp.Tasks[0].to_json())
+                                    opsecPre.Task = MythicCommandBase.PTTaskMessageTaskData(
+                                        **taskResp.Tasks[0].to_json())
                                     opsecPre.Task.CommandName = command_name
                                     opsecPre.Task.Params = params
                                     opsecPre.Task.OriginalParams = params
                                     opsecPre.Task.TaskingLocation = tasking_location
-                                    opsecPost.Task = MythicCommandBase.PTTaskMessageTaskData(**taskResp.Tasks[0].to_json())
+                                    opsecPost.Task = MythicCommandBase.PTTaskMessageTaskData(
+                                        **taskResp.Tasks[0].to_json())
                                     opsecPost.Task.CommandName = command_name
                                     opsecPost.Task.Params = params
                                     opsecPost.Task.OriginalParams = params
                                     opsecPost.Task.TaskingLocation = tasking_location
-                                    createTasking.Task = MythicCommandBase.PTTaskMessageTaskData(**taskResp.Tasks[0].to_json())
+                                    createTasking.Task = MythicCommandBase.PTTaskMessageTaskData(
+                                        **taskResp.Tasks[0].to_json())
                                     createTasking.Task.CommandName = command_name
                                     createTasking.Task.Params = params
                                     createTasking.Task.OriginalParams = params
                                     createTasking.Task.TaskingLocation = tasking_location
                         logger.info(f"[*] Testing OPSEC PRE")
                         if not await agent_utils.verifyTaskArgs(opsecPre, ""):
                             return
@@ -473,33 +497,36 @@
                             try:
                                 response = await commandInstance.opsec_pre(taskData=opsecPre)
                                 logger.info(f"[+] Finished OPSEC PRE:\n{json.dumps(response.to_json(), indent=4)}")
                             except Exception as e:
                                 logger.exception(f"[*] Hit exception: {e}")
                         logger.info(f"[*] Testing Create Tasking")
                         task = await agent_utils.initialize_task(commandInstance, {
-                            "task":  createTasking.Task.to_json(),
+                            "task": createTasking.Task.to_json(),
                             "callback": createTasking.Callback.to_json()
                         }, "")
                         if task is None:
                             # we hit an error and already sent the response, just return
                             return
                         else:
                             try:
                                 if hasattr(commandInstance, "create_go_tasking"):
                                     if not await agent_utils.verifyTaskArgs(createTasking, ""):
                                         return
-                                    createTaskingResponse = await commandInstance.create_go_tasking(taskData=createTasking)
+                                    createTaskingResponse = await commandInstance.create_go_tasking(
+                                        taskData=createTasking)
                                     if createTaskingResponse.Params is None:
                                         # no manual args were set, so parse them from the task.args
                                         createTaskingResponse.Params = str(task.args)
-                                    logger.info(f"[+] Finished Create Tasking (new):\n{json.dumps(createTaskingResponse.to_json(), indent=4)}")
+                                    logger.info(
+                                        f"[+] Finished Create Tasking (new):\n{json.dumps(createTaskingResponse.to_json(), indent=4)}")
                                 else:
                                     createTaskingResponse = await commandInstance.create_tasking(task=task)
-                                    logger.info(f"[+] Finished Create Tasking (legacy):\n{json.dumps(createTaskingResponse.to_json(), indent=4)}")
+                                    logger.info(
+                                        f"[+] Finished Create Tasking (legacy):\n{json.dumps(createTaskingResponse.to_json(), indent=4)}")
                             except Exception as createTaskingException:
                                 logger.exception(f"[*] Hit exception: {createTaskingException}")
                         logger.info(f"[*] Testing OPSEC Post")
                         if not await agent_utils.verifyTaskArgs(opsecPost, ""):
                             return
                         else:
                             try:
```

### Comparing `mythic_container-0.2.1/mythic_container/rabbitmq.py` & `mythic_container-0.2.2/mythic_container/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/utils_mythic_file_transfer.py` & `mythic_container-0.2.2/mythic_container/utils_mythic_file_transfer.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container/webhook_utils.py` & `mythic_container-0.2.2/mythic_container/webhook_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/mythic_container.egg-info/PKG-INFO` & `mythic_container-0.2.2/mythic_container.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic-container
-Version: 0.2.1
+Version: 0.2.2
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mythic_container-0.2.1/mythic_container.egg-info/SOURCES.txt` & `mythic_container-0.2.2/mythic_container.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.1/setup.py` & `mythic_container-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic_container",
-    version="0.2.1",
+    version="0.2.2",
     description="Functionality for Mythic Services",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/customizing/payload-type-development",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

