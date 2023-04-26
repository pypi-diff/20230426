# Comparing `tmp/corellium-api-0.3.1.tar.gz` & `tmp/corellium-api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corellium-api-0.3.1.tar", last modified: Fri Apr 21 19:24:27 2023, max compression
+gzip compressed data, was "corellium-api-0.3.2.tar", last modified: Wed Apr 26 00:44:44 2023, max compression
```

## Comparing `corellium-api-0.3.1.tar` & `corellium-api-0.3.2.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-21 19:24:27.562211 corellium-api-0.3.1/
--rw-r--r--   0 sam       (1000) sam       (1000)      319 2023-04-21 19:24:27.562211 corellium-api-0.3.1/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)    27335 2023-04-21 19:24:00.000000 corellium-api-0.3.1/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-21 19:24:27.502213 corellium-api-0.3.1/corellium_api/
--rw-r--r--   0 sam       (1000) sam       (1000)     7269 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/__init__.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-21 19:24:27.502213 corellium-api-0.3.1/corellium_api/api/
--rw-r--r--   0 sam       (1000) sam       (1000)      144 2023-04-21 18:54:11.000000 corellium-api-0.3.1/corellium_api/api/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)   817635 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/api/corellium_api.py
--rw-r--r--   0 sam       (1000) sam       (1000)    27761 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/api_client.py
--rw-r--r--   0 sam       (1000) sam       (1000)    16369 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/configuration.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5077 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/exceptions.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-21 19:24:27.534211 corellium-api-0.3.1/corellium_api/models/
--rw-r--r--   0 sam       (1000) sam       (1000)     6728 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7295 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/address.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7552 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_app.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3856 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_app_ready_response.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4353 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_app_status.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4438 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_apps_list.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4528 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_apps_status_list.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5936 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3596 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_icons.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3648 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_install_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3921 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_profiles_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3683 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_system_adb_auth.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3948 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_system_get_prop_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3662 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agent_value_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3803 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/agreed_ack.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5801 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/api_conflict_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5468 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/api_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5772 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/api_internal_consistency_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6107 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/api_not_found_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3836 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/api_token.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3055 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/bit.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3704 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/btrace_enable_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3369 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/button.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5898 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/coupon_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3761 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/create_team.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5544 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/created_by.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4797 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/credentials.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4661 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/domain_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8135 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)    16317 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/features.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5471 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/file_changes.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13228 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/firmware.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4978 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/gpio_state_definition.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4898 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/gpios_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3712 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/grant_trial_request_response.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9581 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/hook.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9950 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/image.py
--rw-r--r--   0 sam       (1000) sam       (1000)    22839 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4239 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_agent_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8955 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_boot_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3479 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_boot_options_additional_tag.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3682 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_console_endpoint.py
--rw-r--r--   0 sam       (1000) sam       (1000)    14845 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_create_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5707 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4953 2023-04-21 18:54:09.000000 corellium-api-0.3.1/corellium_api/models/instance_netdump_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5049 2023-04-21 19:23:53.000000 corellium-api-0.3.1/corellium_api/models/instance_netmon_proc_map_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4937 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_netmon_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4549 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3600 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_services.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4511 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_start_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3340 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3679 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_stop_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4522 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/instance_upgrade_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5003 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/invitation.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3608 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/invite_revoke_params.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3013 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/invite_revoke_params_ids.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4187 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/kcrange.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5587 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/kernel_task.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4973 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/kernel_thread.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4292 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/media_play_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9967 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/model.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6959 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/model_software.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7408 2023-04-21 19:23:53.000000 corellium-api-0.3.1/corellium_api/models/net_mon_proc_map_filter.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7240 2023-04-21 18:54:09.000000 corellium-api-0.3.1/corellium_api/models/netdump_filter.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5831 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/password_change_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5844 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/password_reset_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6273 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/patch_instance_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9478 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/peripherals_data.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4162 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/plan.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5173 2023-04-21 19:23:53.000000 corellium-api-0.3.1/corellium_api/models/plan_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6358 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/project.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8533 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/project_key.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4880 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/project_quota.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5102 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/project_settings.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5461 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/project_usage.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6326 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/proxy_config.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5033 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/rate_info.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3885 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/reset_link_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5639 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/role.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4297 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/rotate_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8024 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/snapshot.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3873 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/snapshot_creation_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4254 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/snapshot_status.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13441 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/subscriber_invite.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5071 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/team.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3564 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/team_create.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3572 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/text_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4459 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/token.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4351 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/touch_curve_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3714 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/touch_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3829 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/trial.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5945 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/trial_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7578 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/trial_request_metadata.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7298 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/trial_request_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3797 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/update_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6883 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/user.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5655 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/user_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6961 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/v1_create_hook_parameters.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4008 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/v1_load_extension_parameters.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3781 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/v1_set_state_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5757 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/validation_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5174 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/volume_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     4353 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/vpn_definition.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7963 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/web_player_create_session_request.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5867 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/models/web_player_session.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9860 2023-04-21 19:24:00.000000 corellium-api-0.3.1/corellium_api/rest.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-21 19:24:27.502213 corellium-api-0.3.1/corellium_api.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)      319 2023-04-21 19:24:27.000000 corellium-api-0.3.1/corellium_api.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     7690 2023-04-21 19:24:27.000000 corellium-api-0.3.1/corellium_api.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-04-21 19:24:27.000000 corellium-api-0.3.1/corellium_api.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       57 2023-04-21 19:24:27.000000 corellium-api-0.3.1/corellium_api.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       14 2023-04-21 19:24:27.000000 corellium-api-0.3.1/corellium_api.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       69 2023-04-21 19:24:27.562211 corellium-api-0.3.1/setup.cfg
--rw-r--r--   0 sam       (1000) sam       (1000)     1054 2023-04-21 19:24:00.000000 corellium-api-0.3.1/setup.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-21 19:24:27.558211 corellium-api-0.3.1/test/
--rw-r--r--   0 sam       (1000) sam       (1000)     1424 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_address.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1518 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_app.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1458 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_app_ready_response.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1384 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_app_status.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1791 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_apps_list.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1614 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_apps_status_list.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1452 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1304 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_icons.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1368 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_install_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1524 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_profiles_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1397 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_system_adb_auth.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1475 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_system_get_prop_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1369 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agent_value_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1374 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_agreed_ack.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1508 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_api_conflict_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1408 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_api_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1621 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_api_internal_consistency_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1522 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_api_not_found_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1315 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_api_token.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1195 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_bit.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1499 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_btrace_enable_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1228 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_button.py
--rw-r--r--   0 sam       (1000) sam       (1000)    20787 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_corellium_api.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1498 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_coupon_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1327 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_create_team.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1381 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_created_by.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1407 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_credentials.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1584 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_domain_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1532 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1934 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_features.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1402 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_file_changes.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1880 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_firmware.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1691 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_gpio_state_definition.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2097 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_gpios_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1469 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_grant_trial_request_response.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1503 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_hook.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1706 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_image.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3732 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1418 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_agent_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1686 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_boot_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1522 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_boot_options_additional_tag.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1444 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_console_endpoint.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3029 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_create_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)      840 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1473 2023-04-21 18:54:09.000000 corellium-api-0.3.1/test/test_instance_netdump_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1543 2023-04-21 19:23:53.000000 corellium-api-0.3.1/test/test_instance_netmon_proc_map_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1462 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_netmon_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1428 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_return.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1592 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_services.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1449 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_start_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1307 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_state.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1403 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_stop_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1455 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_instance_upgrade_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1367 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_invitation.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1391 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_invite_revoke_params.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1399 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_invite_revoke_params_ids.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1338 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_kcrange.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1655 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_kernel_task.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1427 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_kernel_thread.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1366 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_media_play_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1643 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_model.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2366 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_model_software.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1837 2023-04-21 19:23:53.000000 corellium-api-0.3.1/test/test_net_mon_proc_map_filter.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1765 2023-04-21 18:54:09.000000 corellium-api-0.3.1/test/test_netdump_filter.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1559 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_password_change_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1546 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_password_reset_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2193 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_patch_instance_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1827 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_peripherals_data.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1263 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_plan.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1426 2023-04-21 19:23:53.000000 corellium-api-0.3.1/test/test_plan_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1931 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_project.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1702 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_project_key.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1392 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_project_quota.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1432 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_project_settings.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1422 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_project_usage.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1432 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_proxy_config.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1335 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_rate_info.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1364 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_reset_link_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1385 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_role.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1339 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_rotate_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1607 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_snapshot.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1472 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_snapshot_creation_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1377 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_snapshot_status.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2289 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_subscriber_invite.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1606 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_team.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1298 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_team_create.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1289 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_text_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1380 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_token.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1389 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_touch_curve_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1306 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_touch_input.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1284 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_trial.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1450 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_trial_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1572 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_trial_request_metadata.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2081 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_trial_request_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1360 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_update_extension.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1463 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_user.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1428 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_user_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1662 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_v1_create_hook_parameters.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1504 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_v1_load_extension_parameters.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1381 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_v1_set_state_body.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1506 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_validation_error.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1456 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_volume_options.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1459 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_vpn_definition.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3400 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_web_player_create_session_request.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1537 2023-04-21 19:24:00.000000 corellium-api-0.3.1/test/test_web_player_session.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-26 00:44:44.744490 corellium-api-0.3.2/
+-rw-r--r--   0 sam       (1000) sam       (1000)      319 2023-04-26 00:44:44.744490 corellium-api-0.3.2/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)    27786 2023-04-26 00:41:07.000000 corellium-api-0.3.2/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-26 00:44:44.684491 corellium-api-0.3.2/corellium_api/
+-rw-r--r--   0 sam       (1000) sam       (1000)     7269 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/__init__.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-26 00:44:44.688491 corellium-api-0.3.2/corellium_api/api/
+-rw-r--r--   0 sam       (1000) sam       (1000)      144 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/api/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)   830210 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/api/corellium_api.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    27761 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/api_client.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    16369 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/configuration.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5077 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/exceptions.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-26 00:44:44.720491 corellium-api-0.3.2/corellium_api/models/
+-rw-r--r--   0 sam       (1000) sam       (1000)     6728 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7295 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/address.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7552 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agent_app.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3856 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agent_app_ready_response.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4353 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agent_app_status.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4438 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agent_apps_list.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4528 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agent_apps_status_list.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5936 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agent_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3596 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agent_icons.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3648 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agent_install_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3921 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agent_profiles_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3683 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agent_system_adb_auth.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3948 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agent_system_get_prop_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3662 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agent_value_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3803 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/agreed_ack.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5801 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/api_conflict_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5468 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/api_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5772 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/api_internal_consistency_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6107 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/api_not_found_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3836 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/api_token.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3055 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/bit.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3704 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/btrace_enable_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3369 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/button.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5898 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/coupon_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3761 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/create_team.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5544 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/created_by.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4797 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/credentials.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4661 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/domain_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8135 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    16317 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/features.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5471 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/file_changes.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13228 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/firmware.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4978 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/gpio_state_definition.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4898 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/gpios_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3712 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/grant_trial_request_response.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9581 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/hook.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9950 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/image.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    22839 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4239 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_agent_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8955 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_boot_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3479 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_boot_options_additional_tag.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3682 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_console_endpoint.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    14845 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_create_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5707 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4953 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_netdump_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5049 2023-04-21 19:23:53.000000 corellium-api-0.3.2/corellium_api/models/instance_netmon_proc_map_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4937 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_netmon_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4549 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3600 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_services.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4511 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_start_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3340 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3679 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_stop_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4522 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/instance_upgrade_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5003 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/invitation.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3608 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/invite_revoke_params.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3013 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/invite_revoke_params_ids.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4187 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/kcrange.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5587 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/kernel_task.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4973 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/kernel_thread.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4292 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/media_play_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9967 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/model.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6959 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/model_software.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7408 2023-04-21 19:23:53.000000 corellium-api-0.3.2/corellium_api/models/net_mon_proc_map_filter.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7240 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/netdump_filter.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5831 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/password_change_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5844 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/password_reset_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6273 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/patch_instance_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9478 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/peripherals_data.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4162 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/plan.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5173 2023-04-21 19:23:53.000000 corellium-api-0.3.2/corellium_api/models/plan_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6358 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/project.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8533 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/project_key.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4880 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/project_quota.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5102 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/project_settings.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5461 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/project_usage.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6326 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/proxy_config.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5033 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/rate_info.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3885 2023-04-26 00:41:06.000000 corellium-api-0.3.2/corellium_api/models/reset_link_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5639 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/role.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4297 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/rotate_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8024 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/snapshot.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3873 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/snapshot_creation_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4254 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/snapshot_status.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13441 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/subscriber_invite.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5071 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/team.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3564 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/team_create.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3572 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/text_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4459 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/token.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4351 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/touch_curve_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3714 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/touch_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3829 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/trial.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5945 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/trial_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7578 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/trial_request_metadata.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7298 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/trial_request_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3797 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/update_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6883 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/user.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5655 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/user_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6961 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/v1_create_hook_parameters.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4008 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/v1_load_extension_parameters.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3781 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/v1_set_state_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5757 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/validation_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5174 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/volume_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     4353 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/vpn_definition.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7963 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/web_player_create_session_request.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5867 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/models/web_player_session.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     9860 2023-04-26 00:41:07.000000 corellium-api-0.3.2/corellium_api/rest.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-26 00:44:44.688491 corellium-api-0.3.2/corellium_api.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)      319 2023-04-26 00:44:44.000000 corellium-api-0.3.2/corellium_api.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     7690 2023-04-26 00:44:44.000000 corellium-api-0.3.2/corellium_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-04-26 00:44:44.000000 corellium-api-0.3.2/corellium_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       57 2023-04-26 00:44:44.000000 corellium-api-0.3.2/corellium_api.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       14 2023-04-26 00:44:44.000000 corellium-api-0.3.2/corellium_api.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       69 2023-04-26 00:44:44.744490 corellium-api-0.3.2/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)     1054 2023-04-26 00:44:24.000000 corellium-api-0.3.2/setup.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-04-26 00:44:44.744490 corellium-api-0.3.2/test/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1424 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_address.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1518 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agent_app.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1458 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agent_app_ready_response.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1384 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agent_app_status.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1791 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agent_apps_list.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1614 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agent_apps_status_list.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1452 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agent_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1304 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agent_icons.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1368 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agent_install_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1524 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agent_profiles_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1397 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agent_system_adb_auth.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1475 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agent_system_get_prop_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1369 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agent_value_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1374 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_agreed_ack.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1508 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_api_conflict_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1408 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_api_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1621 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_api_internal_consistency_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1522 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_api_not_found_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1315 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_api_token.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1195 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_bit.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1499 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_btrace_enable_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1228 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_button.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    21225 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_corellium_api.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1498 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_coupon_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1327 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_create_team.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1381 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_created_by.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1407 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_credentials.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1584 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_domain_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1532 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1934 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_features.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1402 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_file_changes.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1880 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_firmware.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1691 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_gpio_state_definition.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2097 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_gpios_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1469 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_grant_trial_request_response.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1503 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_hook.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1706 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_image.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3732 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1418 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_agent_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1686 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_boot_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1522 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_boot_options_additional_tag.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1444 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_console_endpoint.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3029 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_create_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      840 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1473 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_netdump_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1543 2023-04-21 19:23:53.000000 corellium-api-0.3.2/test/test_instance_netmon_proc_map_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1462 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_netmon_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1428 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_return.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1592 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_services.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1449 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_start_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1307 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_state.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1403 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_stop_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1455 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_instance_upgrade_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1367 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_invitation.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1391 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_invite_revoke_params.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1399 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_invite_revoke_params_ids.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1338 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_kcrange.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1655 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_kernel_task.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1427 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_kernel_thread.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1366 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_media_play_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1643 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_model.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2366 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_model_software.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1837 2023-04-21 19:23:53.000000 corellium-api-0.3.2/test/test_net_mon_proc_map_filter.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1765 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_netdump_filter.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1559 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_password_change_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1546 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_password_reset_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2193 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_patch_instance_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1827 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_peripherals_data.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1263 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_plan.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1426 2023-04-21 19:23:53.000000 corellium-api-0.3.2/test/test_plan_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1931 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_project.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1702 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_project_key.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1392 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_project_quota.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1432 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_project_settings.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1422 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_project_usage.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1432 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_proxy_config.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1335 2023-04-26 00:41:06.000000 corellium-api-0.3.2/test/test_rate_info.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1364 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_reset_link_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1385 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_role.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1339 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_rotate_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1607 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_snapshot.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1472 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_snapshot_creation_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1377 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_snapshot_status.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2289 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_subscriber_invite.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1606 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_team.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1298 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_team_create.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1289 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_text_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1380 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_token.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1389 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_touch_curve_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1306 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_touch_input.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1284 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_trial.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1450 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_trial_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1572 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_trial_request_metadata.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2081 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_trial_request_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1360 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_update_extension.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1463 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_user.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1428 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_user_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1662 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_v1_create_hook_parameters.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1504 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_v1_load_extension_parameters.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1381 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_v1_set_state_body.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1506 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_validation_error.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1456 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_volume_options.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1459 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_vpn_definition.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3400 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_web_player_create_session_request.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1537 2023-04-26 00:41:07.000000 corellium-api-0.3.2/test/test_web_player_session.py
```

### Comparing `corellium-api-0.3.1/README.md` & `corellium-api-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # corellium-api
 REST API to manage your virtual devices.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 4.5.0-16757
+- API version: 4.5.0-16775
 - Package version: 0.3.1
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -167,14 +167,16 @@
 *CorelliumApi* | [**v1_get_project_instances**](docs/CorelliumApi.md#v1_get_project_instances) | **GET** /v1/projects/{projectId}/instances | Get Instances in Project
 *CorelliumApi* | [**v1_get_project_keys**](docs/CorelliumApi.md#v1_get_project_keys) | **GET** /v1/projects/{projectId}/keys | Get Project Authorized Keys
 *CorelliumApi* | [**v1_get_project_vpn_config**](docs/CorelliumApi.md#v1_get_project_vpn_config) | **GET** /v1/projects/{projectId}/vpnconfig/{format} | Get Project VPN Configuration
 *CorelliumApi* | [**v1_get_projects**](docs/CorelliumApi.md#v1_get_projects) | **GET** /v1/projects | Get Projects
 *CorelliumApi* | [**v1_get_reset_link_info**](docs/CorelliumApi.md#v1_get_reset_link_info) | **GET** /v1/users/reset-link-info | Send Password Reset Link Info
 *CorelliumApi* | [**v1_get_snapshot**](docs/CorelliumApi.md#v1_get_snapshot) | **GET** /v1/snapshots/{snapshotId} | Get Snapshot
 *CorelliumApi* | [**v1_instances_instance_id_message_post**](docs/CorelliumApi.md#v1_instances_instance_id_message_post) | **POST** /v1/instances/{instanceId}/message | Receive a message on an iOS vm
+*CorelliumApi* | [**v1_instances_instance_id_netdump_pcap_get**](docs/CorelliumApi.md#v1_instances_instance_id_netdump_pcap_get) | **GET** /v1/instances/{instanceId}/netdump.pcap | Download a netdump pcap file
+*CorelliumApi* | [**v1_instances_instance_id_network_monitor_pcap_get**](docs/CorelliumApi.md#v1_instances_instance_id_network_monitor_pcap_get) | **GET** /v1/instances/{instanceId}/networkMonitor.pcap | Download a Network Monitor pcap file
 *CorelliumApi* | [**v1_kcrange**](docs/CorelliumApi.md#v1_kcrange) | **GET** /v1/instances/{instanceId}/btrace-kcrange | Get Kernel extension ranges
 *CorelliumApi* | [**v1_list_threads**](docs/CorelliumApi.md#v1_list_threads) | **GET** /v1/instances/{instanceId}/strace/thread-list | Get Running Threads (CoreTrace)
 *CorelliumApi* | [**v1_media_play**](docs/CorelliumApi.md#v1_media_play) | **POST** /v1/instances/{instanceId}/media/play | Start playing media
 *CorelliumApi* | [**v1_media_stop**](docs/CorelliumApi.md#v1_media_stop) | **POST** /v1/instances/{instanceId}/media/stop | Stop playing media
 *CorelliumApi* | [**v1_patch_instance**](docs/CorelliumApi.md#v1_patch_instance) | **PATCH** /v1/instances/{instanceId} | Update Instance
 *CorelliumApi* | [**v1_pause_instance**](docs/CorelliumApi.md#v1_pause_instance) | **POST** /v1/instances/{instanceId}/pause | Pause an Instance
 *CorelliumApi* | [**v1_post_instance_input**](docs/CorelliumApi.md#v1_post_instance_input) | **POST** /v1/instances/{instanceId}/input | Provide Instance Input
```

### Comparing `corellium-api-0.3.1/corellium_api/__init__.py` & `corellium-api-0.3.2/corellium_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 __version__ = "0.3.1"
```

### Comparing `corellium-api-0.3.1/corellium_api/api/corellium_api.py` & `corellium-api-0.3.2/corellium_api/api/corellium_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -10867,14 +10867,290 @@
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
+    def v1_instances_instance_id_netdump_pcap_get(self, instance_id, **kwargs):  # noqa: E501
+        """Download a netdump pcap file  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_instances_instance_id_netdump_pcap_get(instance_id, async_req=True)
+        >>> result = thread.get()
+
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: file
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.v1_instances_instance_id_netdump_pcap_get_with_http_info(instance_id, **kwargs)  # noqa: E501
+
+    def v1_instances_instance_id_netdump_pcap_get_with_http_info(self, instance_id, **kwargs):  # noqa: E501
+        """Download a netdump pcap file  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_instances_instance_id_netdump_pcap_get_with_http_info(instance_id, async_req=True)
+        >>> result = thread.get()
+
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(file, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'instance_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_instances_instance_id_netdump_pcap_get" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'instance_id' is set
+        if self.api_client.client_side_validation and ('instance_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['instance_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `instance_id` when calling `v1_instances_instance_id_netdump_pcap_get`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'instance_id' in local_var_params:
+            path_params['instanceId'] = local_var_params['instance_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/vnd.tcpdump.pcap', 'application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        response_types_map = {
+            200: "file",
+            400: "UserError",
+            403: "ApiError",
+        }
+
+        return self.api_client.call_api(
+            '/v1/instances/{instanceId}/netdump.pcap', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
+    def v1_instances_instance_id_network_monitor_pcap_get(self, instance_id, **kwargs):  # noqa: E501
+        """Download a Network Monitor pcap file  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_instances_instance_id_network_monitor_pcap_get(instance_id, async_req=True)
+        >>> result = thread.get()
+
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: file
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.v1_instances_instance_id_network_monitor_pcap_get_with_http_info(instance_id, **kwargs)  # noqa: E501
+
+    def v1_instances_instance_id_network_monitor_pcap_get_with_http_info(self, instance_id, **kwargs):  # noqa: E501
+        """Download a Network Monitor pcap file  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_instances_instance_id_network_monitor_pcap_get_with_http_info(instance_id, async_req=True)
+        >>> result = thread.get()
+
+        :param instance_id: Instance ID - uuid (required)
+        :type instance_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(file, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'instance_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_instances_instance_id_network_monitor_pcap_get" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'instance_id' is set
+        if self.api_client.client_side_validation and ('instance_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['instance_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `instance_id` when calling `v1_instances_instance_id_network_monitor_pcap_get`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'instance_id' in local_var_params:
+            path_params['instanceId'] = local_var_params['instance_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/vnd.tcpdump.pcap', 'application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        response_types_map = {
+            200: "file",
+            400: "UserError",
+            403: "ApiError",
+        }
+
+        return self.api_client.call_api(
+            '/v1/instances/{instanceId}/networkMonitor.pcap', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
```

### Comparing `corellium-api-0.3.1/corellium_api/api_client.py` & `corellium-api-0.3.2/corellium_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
```

### Comparing `corellium-api-0.3.1/corellium_api/configuration.py` & `corellium-api-0.3.2/corellium_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -381,15 +381,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 4.5.0-16757\n"\
+               "Version of the API: 4.5.0-16775\n"\
                "SDK Package Version: 0.3.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `corellium-api-0.3.1/corellium_api/exceptions.py` & `corellium-api-0.3.2/corellium_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `corellium-api-0.3.1/corellium_api/models/__init__.py` & `corellium-api-0.3.2/corellium_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
```

### Comparing `corellium-api-0.3.1/corellium_api/models/address.py` & `corellium-api-0.3.2/corellium_api/models/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agent_app.py` & `corellium-api-0.3.2/corellium_api/models/agent_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agent_app_ready_response.py` & `corellium-api-0.3.2/corellium_api/models/agent_app_ready_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agent_app_status.py` & `corellium-api-0.3.2/corellium_api/models/agent_app_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agent_apps_list.py` & `corellium-api-0.3.2/corellium_api/models/agent_apps_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agent_apps_status_list.py` & `corellium-api-0.3.2/corellium_api/models/agent_apps_status_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agent_error.py` & `corellium-api-0.3.2/corellium_api/models/agent_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agent_icons.py` & `corellium-api-0.3.2/corellium_api/models/agent_icons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agent_install_body.py` & `corellium-api-0.3.2/corellium_api/models/agent_install_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agent_profiles_return.py` & `corellium-api-0.3.2/corellium_api/models/agent_profiles_return.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agent_system_adb_auth.py` & `corellium-api-0.3.2/corellium_api/models/agent_system_adb_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agent_system_get_prop_body.py` & `corellium-api-0.3.2/corellium_api/models/agent_system_get_prop_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agent_value_return.py` & `corellium-api-0.3.2/corellium_api/models/agent_value_return.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/agreed_ack.py` & `corellium-api-0.3.2/corellium_api/models/agreed_ack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/api_conflict_error.py` & `corellium-api-0.3.2/corellium_api/models/api_conflict_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/api_error.py` & `corellium-api-0.3.2/corellium_api/models/api_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/api_internal_consistency_error.py` & `corellium-api-0.3.2/corellium_api/models/api_internal_consistency_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/api_not_found_error.py` & `corellium-api-0.3.2/corellium_api/models/api_not_found_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/api_token.py` & `corellium-api-0.3.2/corellium_api/models/api_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/bit.py` & `corellium-api-0.3.2/corellium_api/models/bit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/btrace_enable_options.py` & `corellium-api-0.3.2/corellium_api/models/btrace_enable_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/button.py` & `corellium-api-0.3.2/corellium_api/models/button.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/coupon_options.py` & `corellium-api-0.3.2/corellium_api/models/coupon_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/create_team.py` & `corellium-api-0.3.2/corellium_api/models/create_team.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/created_by.py` & `corellium-api-0.3.2/corellium_api/models/created_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/credentials.py` & `corellium-api-0.3.2/corellium_api/models/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/domain_options.py` & `corellium-api-0.3.2/corellium_api/models/domain_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/extension.py` & `corellium-api-0.3.2/corellium_api/models/extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/features.py` & `corellium-api-0.3.2/corellium_api/models/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/file_changes.py` & `corellium-api-0.3.2/corellium_api/models/file_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/firmware.py` & `corellium-api-0.3.2/corellium_api/models/firmware.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/gpio_state_definition.py` & `corellium-api-0.3.2/corellium_api/models/gpio_state_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/gpios_state.py` & `corellium-api-0.3.2/corellium_api/models/gpios_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/grant_trial_request_response.py` & `corellium-api-0.3.2/corellium_api/models/grant_trial_request_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/hook.py` & `corellium-api-0.3.2/corellium_api/models/hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/image.py` & `corellium-api-0.3.2/corellium_api/models/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance.py` & `corellium-api-0.3.2/corellium_api/models/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_agent_state.py` & `corellium-api-0.3.2/corellium_api/models/instance_agent_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_boot_options.py` & `corellium-api-0.3.2/corellium_api/models/instance_boot_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_boot_options_additional_tag.py` & `corellium-api-0.3.2/corellium_api/models/instance_boot_options_additional_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_console_endpoint.py` & `corellium-api-0.3.2/corellium_api/models/instance_console_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_create_options.py` & `corellium-api-0.3.2/corellium_api/models/instance_create_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_input.py` & `corellium-api-0.3.2/corellium_api/models/instance_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_netdump_state.py` & `corellium-api-0.3.2/corellium_api/models/instance_netdump_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_netmon_proc_map_state.py` & `corellium-api-0.3.2/corellium_api/models/instance_netmon_proc_map_state.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_netmon_state.py` & `corellium-api-0.3.2/corellium_api/models/instance_netmon_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_return.py` & `corellium-api-0.3.2/corellium_api/models/instance_return.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_services.py` & `corellium-api-0.3.2/corellium_api/models/instance_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_start_options.py` & `corellium-api-0.3.2/corellium_api/models/instance_start_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_state.py` & `corellium-api-0.3.2/corellium_api/models/instance_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_stop_options.py` & `corellium-api-0.3.2/corellium_api/models/instance_stop_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/instance_upgrade_body.py` & `corellium-api-0.3.2/corellium_api/models/instance_upgrade_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/invitation.py` & `corellium-api-0.3.2/corellium_api/models/invitation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/invite_revoke_params.py` & `corellium-api-0.3.2/corellium_api/models/invite_revoke_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/invite_revoke_params_ids.py` & `corellium-api-0.3.2/corellium_api/models/invite_revoke_params_ids.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/kcrange.py` & `corellium-api-0.3.2/corellium_api/models/kcrange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/kernel_task.py` & `corellium-api-0.3.2/corellium_api/models/kernel_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/kernel_thread.py` & `corellium-api-0.3.2/corellium_api/models/kernel_thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/media_play_body.py` & `corellium-api-0.3.2/corellium_api/models/media_play_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/model.py` & `corellium-api-0.3.2/corellium_api/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/model_software.py` & `corellium-api-0.3.2/corellium_api/models/model_software.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/net_mon_proc_map_filter.py` & `corellium-api-0.3.2/corellium_api/models/net_mon_proc_map_filter.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.1/corellium_api/models/netdump_filter.py` & `corellium-api-0.3.2/corellium_api/models/netdump_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/password_change_body.py` & `corellium-api-0.3.2/corellium_api/models/password_change_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/password_reset_body.py` & `corellium-api-0.3.2/corellium_api/models/password_reset_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/patch_instance_options.py` & `corellium-api-0.3.2/corellium_api/models/patch_instance_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/peripherals_data.py` & `corellium-api-0.3.2/corellium_api/models/peripherals_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/plan.py` & `corellium-api-0.3.2/corellium_api/models/plan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/plan_options.py` & `corellium-api-0.3.2/corellium_api/models/plan_options.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.1/corellium_api/models/project.py` & `corellium-api-0.3.2/corellium_api/models/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/project_key.py` & `corellium-api-0.3.2/corellium_api/models/project_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/project_quota.py` & `corellium-api-0.3.2/corellium_api/models/project_quota.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/project_settings.py` & `corellium-api-0.3.2/corellium_api/models/project_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/project_usage.py` & `corellium-api-0.3.2/corellium_api/models/project_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/proxy_config.py` & `corellium-api-0.3.2/corellium_api/models/proxy_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/rate_info.py` & `corellium-api-0.3.2/corellium_api/models/rate_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/reset_link_body.py` & `corellium-api-0.3.2/corellium_api/models/reset_link_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/role.py` & `corellium-api-0.3.2/corellium_api/models/role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/rotate_body.py` & `corellium-api-0.3.2/corellium_api/models/rotate_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/snapshot.py` & `corellium-api-0.3.2/corellium_api/models/snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/snapshot_creation_options.py` & `corellium-api-0.3.2/corellium_api/models/snapshot_creation_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/snapshot_status.py` & `corellium-api-0.3.2/corellium_api/models/snapshot_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/subscriber_invite.py` & `corellium-api-0.3.2/corellium_api/models/subscriber_invite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/team.py` & `corellium-api-0.3.2/corellium_api/models/team.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/team_create.py` & `corellium-api-0.3.2/corellium_api/models/team_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/text_input.py` & `corellium-api-0.3.2/corellium_api/models/text_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/token.py` & `corellium-api-0.3.2/corellium_api/models/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/touch_curve_input.py` & `corellium-api-0.3.2/corellium_api/models/touch_curve_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/touch_input.py` & `corellium-api-0.3.2/corellium_api/models/touch_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/trial.py` & `corellium-api-0.3.2/corellium_api/models/trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/trial_extension.py` & `corellium-api-0.3.2/corellium_api/models/trial_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/trial_request_metadata.py` & `corellium-api-0.3.2/corellium_api/models/trial_request_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/trial_request_options.py` & `corellium-api-0.3.2/corellium_api/models/trial_request_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/update_extension.py` & `corellium-api-0.3.2/corellium_api/models/update_extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/user.py` & `corellium-api-0.3.2/corellium_api/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/user_error.py` & `corellium-api-0.3.2/corellium_api/models/user_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/v1_create_hook_parameters.py` & `corellium-api-0.3.2/corellium_api/models/v1_create_hook_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/v1_load_extension_parameters.py` & `corellium-api-0.3.2/corellium_api/models/v1_load_extension_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/v1_set_state_body.py` & `corellium-api-0.3.2/corellium_api/models/v1_set_state_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/validation_error.py` & `corellium-api-0.3.2/corellium_api/models/validation_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/volume_options.py` & `corellium-api-0.3.2/corellium_api/models/volume_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/vpn_definition.py` & `corellium-api-0.3.2/corellium_api/models/vpn_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/web_player_create_session_request.py` & `corellium-api-0.3.2/corellium_api/models/web_player_create_session_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/models/web_player_session.py` & `corellium-api-0.3.2/corellium_api/models/web_player_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `corellium-api-0.3.1/corellium_api/rest.py` & `corellium-api-0.3.2/corellium_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `corellium-api-0.3.1/corellium_api.egg-info/SOURCES.txt` & `corellium-api-0.3.2/corellium_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.1/setup.py` & `corellium-api-0.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "corellium-api"
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `corellium-api-0.3.1/test/test_address.py` & `corellium-api-0.3.2/test/test_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agent_app.py` & `corellium-api-0.3.2/test/test_agent_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agent_app_ready_response.py` & `corellium-api-0.3.2/test/test_agent_app_ready_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agent_app_status.py` & `corellium-api-0.3.2/test/test_agent_app_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agent_apps_list.py` & `corellium-api-0.3.2/test/test_agent_apps_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agent_apps_status_list.py` & `corellium-api-0.3.2/test/test_agent_apps_status_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agent_error.py` & `corellium-api-0.3.2/test/test_agent_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agent_icons.py` & `corellium-api-0.3.2/test/test_agent_icons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agent_install_body.py` & `corellium-api-0.3.2/test/test_agent_install_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agent_profiles_return.py` & `corellium-api-0.3.2/test/test_agent_profiles_return.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agent_system_adb_auth.py` & `corellium-api-0.3.2/test/test_agent_system_adb_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agent_system_get_prop_body.py` & `corellium-api-0.3.2/test/test_agent_system_get_prop_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agent_value_return.py` & `corellium-api-0.3.2/test/test_agent_value_return.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_agreed_ack.py` & `corellium-api-0.3.2/test/test_agreed_ack.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_api_conflict_error.py` & `corellium-api-0.3.2/test/test_api_conflict_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_api_error.py` & `corellium-api-0.3.2/test/test_api_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_api_internal_consistency_error.py` & `corellium-api-0.3.2/test/test_api_internal_consistency_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_api_not_found_error.py` & `corellium-api-0.3.2/test/test_api_not_found_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_api_token.py` & `corellium-api-0.3.2/test/test_api_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_bit.py` & `corellium-api-0.3.2/test/test_bit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_btrace_enable_options.py` & `corellium-api-0.3.2/test/test_btrace_enable_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_button.py` & `corellium-api-0.3.2/test/test_button.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_corellium_api.py` & `corellium-api-0.3.2/test/test_corellium_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -556,14 +556,28 @@
     def test_v1_instances_instance_id_message_post(self):
         """Test case for v1_instances_instance_id_message_post
 
         Receive a message on an iOS vm  # noqa: E501
         """
         pass
 
+    def test_v1_instances_instance_id_netdump_pcap_get(self):
+        """Test case for v1_instances_instance_id_netdump_pcap_get
+
+        Download a netdump pcap file  # noqa: E501
+        """
+        pass
+
+    def test_v1_instances_instance_id_network_monitor_pcap_get(self):
+        """Test case for v1_instances_instance_id_network_monitor_pcap_get
+
+        Download a Network Monitor pcap file  # noqa: E501
+        """
+        pass
+
     def test_v1_kcrange(self):
         """Test case for v1_kcrange
 
         Get Kernel extension ranges  # noqa: E501
         """
         pass
```

### Comparing `corellium-api-0.3.1/test/test_coupon_options.py` & `corellium-api-0.3.2/test/test_coupon_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_create_team.py` & `corellium-api-0.3.2/test/test_create_team.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_created_by.py` & `corellium-api-0.3.2/test/test_created_by.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_credentials.py` & `corellium-api-0.3.2/test/test_credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_domain_options.py` & `corellium-api-0.3.2/test/test_domain_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_extension.py` & `corellium-api-0.3.2/test/test_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_features.py` & `corellium-api-0.3.2/test/test_features.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_file_changes.py` & `corellium-api-0.3.2/test/test_file_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_firmware.py` & `corellium-api-0.3.2/test/test_firmware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_gpio_state_definition.py` & `corellium-api-0.3.2/test/test_gpio_state_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_gpios_state.py` & `corellium-api-0.3.2/test/test_gpios_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_grant_trial_request_response.py` & `corellium-api-0.3.2/test/test_grant_trial_request_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_hook.py` & `corellium-api-0.3.2/test/test_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_image.py` & `corellium-api-0.3.2/test/test_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance.py` & `corellium-api-0.3.2/test/test_instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_agent_state.py` & `corellium-api-0.3.2/test/test_instance_agent_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_boot_options.py` & `corellium-api-0.3.2/test/test_instance_boot_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_boot_options_additional_tag.py` & `corellium-api-0.3.2/test/test_instance_boot_options_additional_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_console_endpoint.py` & `corellium-api-0.3.2/test/test_instance_console_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_create_options.py` & `corellium-api-0.3.2/test/test_instance_create_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_input.py` & `corellium-api-0.3.2/test/test_instance_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_netdump_state.py` & `corellium-api-0.3.2/test/test_instance_netdump_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_netmon_proc_map_state.py` & `corellium-api-0.3.2/test/test_instance_netmon_proc_map_state.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.1/test/test_instance_netmon_state.py` & `corellium-api-0.3.2/test/test_instance_netmon_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_return.py` & `corellium-api-0.3.2/test/test_instance_return.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_services.py` & `corellium-api-0.3.2/test/test_instance_services.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_start_options.py` & `corellium-api-0.3.2/test/test_instance_start_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_state.py` & `corellium-api-0.3.2/test/test_instance_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_stop_options.py` & `corellium-api-0.3.2/test/test_instance_stop_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_instance_upgrade_body.py` & `corellium-api-0.3.2/test/test_instance_upgrade_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_invitation.py` & `corellium-api-0.3.2/test/test_invitation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_invite_revoke_params.py` & `corellium-api-0.3.2/test/test_invite_revoke_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_invite_revoke_params_ids.py` & `corellium-api-0.3.2/test/test_invite_revoke_params_ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_kcrange.py` & `corellium-api-0.3.2/test/test_kcrange.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_kernel_task.py` & `corellium-api-0.3.2/test/test_kernel_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_kernel_thread.py` & `corellium-api-0.3.2/test/test_kernel_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_media_play_body.py` & `corellium-api-0.3.2/test/test_media_play_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_model.py` & `corellium-api-0.3.2/test/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_model_software.py` & `corellium-api-0.3.2/test/test_model_software.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_net_mon_proc_map_filter.py` & `corellium-api-0.3.2/test/test_net_mon_proc_map_filter.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.1/test/test_netdump_filter.py` & `corellium-api-0.3.2/test/test_netdump_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_password_change_body.py` & `corellium-api-0.3.2/test/test_password_change_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_password_reset_body.py` & `corellium-api-0.3.2/test/test_password_reset_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_patch_instance_options.py` & `corellium-api-0.3.2/test/test_patch_instance_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_peripherals_data.py` & `corellium-api-0.3.2/test/test_peripherals_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_plan.py` & `corellium-api-0.3.2/test/test_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_plan_options.py` & `corellium-api-0.3.2/test/test_plan_options.py`

 * *Files identical despite different names*

### Comparing `corellium-api-0.3.1/test/test_project.py` & `corellium-api-0.3.2/test/test_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_project_key.py` & `corellium-api-0.3.2/test/test_project_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_project_quota.py` & `corellium-api-0.3.2/test/test_project_quota.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_project_settings.py` & `corellium-api-0.3.2/test/test_project_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_project_usage.py` & `corellium-api-0.3.2/test/test_project_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_proxy_config.py` & `corellium-api-0.3.2/test/test_proxy_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_rate_info.py` & `corellium-api-0.3.2/test/test_rate_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_reset_link_body.py` & `corellium-api-0.3.2/test/test_reset_link_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_role.py` & `corellium-api-0.3.2/test/test_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_rotate_body.py` & `corellium-api-0.3.2/test/test_rotate_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_snapshot.py` & `corellium-api-0.3.2/test/test_snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_snapshot_creation_options.py` & `corellium-api-0.3.2/test/test_snapshot_creation_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_snapshot_status.py` & `corellium-api-0.3.2/test/test_snapshot_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_subscriber_invite.py` & `corellium-api-0.3.2/test/test_subscriber_invite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_team.py` & `corellium-api-0.3.2/test/test_team.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_team_create.py` & `corellium-api-0.3.2/test/test_team_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_text_input.py` & `corellium-api-0.3.2/test/test_text_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_token.py` & `corellium-api-0.3.2/test/test_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_touch_curve_input.py` & `corellium-api-0.3.2/test/test_touch_curve_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_touch_input.py` & `corellium-api-0.3.2/test/test_touch_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_trial.py` & `corellium-api-0.3.2/test/test_trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_trial_extension.py` & `corellium-api-0.3.2/test/test_trial_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_trial_request_metadata.py` & `corellium-api-0.3.2/test/test_trial_request_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_trial_request_options.py` & `corellium-api-0.3.2/test/test_trial_request_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_update_extension.py` & `corellium-api-0.3.2/test/test_update_extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_user.py` & `corellium-api-0.3.2/test/test_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_user_error.py` & `corellium-api-0.3.2/test/test_user_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_v1_create_hook_parameters.py` & `corellium-api-0.3.2/test/test_v1_create_hook_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_v1_load_extension_parameters.py` & `corellium-api-0.3.2/test/test_v1_load_extension_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_v1_set_state_body.py` & `corellium-api-0.3.2/test/test_v1_set_state_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_validation_error.py` & `corellium-api-0.3.2/test/test_validation_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_volume_options.py` & `corellium-api-0.3.2/test/test_volume_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_vpn_definition.py` & `corellium-api-0.3.2/test/test_vpn_definition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_web_player_create_session_request.py` & `corellium-api-0.3.2/test/test_web_player_create_session_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `corellium-api-0.3.1/test/test_web_player_session.py` & `corellium-api-0.3.2/test/test_web_player_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Corellium API
 
     REST API to manage your virtual devices.  # noqa: E501
 
-    The version of the OpenAPI document: 4.5.0-16757
+    The version of the OpenAPI document: 4.5.0-16775
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

