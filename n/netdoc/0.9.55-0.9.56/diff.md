# Comparing `tmp/netdoc-0.9.55.tar.gz` & `tmp/netdoc-0.9.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netdoc-0.9.55.tar", last modified: Thu Apr 13 18:43:38 2023, max compression
+gzip compressed data, was "netdoc-0.9.56.tar", last modified: Tue Apr 25 14:22:47 2023, max compression
```

## Comparing `netdoc-0.9.55.tar` & `netdoc-0.9.56.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.55/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      241 2023-04-05 08:40:22.000000 netdoc-0.9.55/MANIFEST.in
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-13 18:43:38.029746 netdoc-0.9.55/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     9911 2023-04-10 16:30:59.000000 netdoc-0.9.55/README.md
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.881743 netdoc-0.9.55/netdoc/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2147 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.897744 netdoc-0.9.55/netdoc/api/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/api/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2812 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/api/serializers.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      597 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/api/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1207 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/api/views.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.901744 netdoc-0.9.55/netdoc/discoverers/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/discoverers/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6978 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/discoverers/netmiko_cisco_ios.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5160 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/discoverers/netmiko_cisco_nxos.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6514 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/discoverers/netmiko_cisco_xr.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6406 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/discoverers/netmiko_hp_comware.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4511 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/discoverers/netmiko_linux.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3613 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/filtersets.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6587 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/forms.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.917744 netdoc-0.9.55/netdoc/ingestors/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1205 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3682 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2014 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2457 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1705 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      822 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1544 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1951 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2602 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3930 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1660 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      886 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1010 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1238 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3649 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2349 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      824 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2000 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2668 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3907 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1509 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2020 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      888 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      909 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1204 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1529 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3645 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2347 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1802 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2892 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2709 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_route.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      980 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1562 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      894 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2980 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1385 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2626 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1038 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1687 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2035 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2933 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3935 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1514 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      895 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      899 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1202 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_linux_arp__an.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1008 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_linux_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1412 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_address_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1933 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_link_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2450 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_route_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      711 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_vrf_show.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.917744 netdoc-0.9.55/netdoc/migrations/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13632 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/migrations/0001_initial.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1800 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3399 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3022 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      577 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      453 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/migrations/0006_alter_routetableentry_metric.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      419 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/migrations/0007_discoverylog_supported.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/migrations/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15079 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/models.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2436 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/navigation.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2988 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/nornir_inventory.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.921744 netdoc-0.9.55/netdoc/reports/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5880 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/reports/NetDoc.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.921744 netdoc-0.9.55/netdoc/schemas/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1937 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/arptableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4319 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/cable.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/credential.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4216 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/device.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1508 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/devicerole.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1714 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/devicetype.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3905 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/discoverable.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3176 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/discoverylog.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8799 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1362 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/ipaddress.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1978 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/macaddresstableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1453 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/manufacturer.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/prefix.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2904 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/routetableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      884 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/site.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1623 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2476 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/schemas/vrf.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.921744 netdoc-0.9.55/netdoc/scripts/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13085 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/scripts/NetDoc.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.873743 netdoc-0.9.55/netdoc/static/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.877743 netdoc-0.9.55/netdoc/static/netdoc/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.925744 netdoc-0.9.55/netdoc/static/netdoc/css/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/css/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/css/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)   220164 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/css/vis-network.min.css
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.017746 netdoc-0.9.55/netdoc/static/netdoc/img/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      305 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/access-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/backup.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    28633 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/circuit.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8387 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/core-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     9522 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/distribution-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15596 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/firewall.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1614 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/internal-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5537 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/isp-cpe-material.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5079 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/non-racked-devices.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15857 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/power-feed.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18685 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/power-panel.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4710 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/power-units.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    34335 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/provider-networks.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13504 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/router.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4484 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/server.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/storage.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8308 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/unknown.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/wan-network.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6975 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/img/wireless-ap.png
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.021746 netdoc-0.9.55/netdoc/static/netdoc/js/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/js/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/js/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4198 2023-04-05 14:32:29.000000 netdoc-0.9.55/netdoc/static/netdoc/js/diagram.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/js/netdoc.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)   702066 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/js/vis-network.min.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)  1930592 2023-04-05 08:40:22.000000 netdoc-0.9.55/netdoc/static/netdoc/js/vis-network.min.js.map
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8198 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/tables.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3912 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/tasks.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.877743 netdoc-0.9.55/netdoc/templates/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/netdoc/templates/netdoc/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3038 2023-04-10 16:21:20.000000 netdoc-0.9.55/netdoc/templates/netdoc/arptableentry.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/netdoc/templates/netdoc/buttons/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      451 2023-04-10 16:17:25.000000 netdoc-0.9.55/netdoc/templates/netdoc/buttons/discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      337 2023-04-10 16:17:25.000000 netdoc-0.9.55/netdoc/templates/netdoc/buttons/export.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1669 2023-04-10 16:21:17.000000 netdoc-0.9.55/netdoc/templates/netdoc/credential.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1439 2023-04-10 16:29:06.000000 netdoc-0.9.55/netdoc/templates/netdoc/diagram.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2654 2023-04-10 16:23:32.000000 netdoc-0.9.55/netdoc/templates/netdoc/discoverable.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1217 2023-04-10 16:26:08.000000 netdoc-0.9.55/netdoc/templates/netdoc/discoverable_bulk_discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      638 2023-04-10 16:26:30.000000 netdoc-0.9.55/netdoc/templates/netdoc/discoverable_discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-04-10 16:23:40.000000 netdoc-0.9.55/netdoc/templates/netdoc/discoverable_list.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5123 2023-04-10 16:23:17.000000 netdoc-0.9.55/netdoc/templates/netdoc/discoverylog.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/netdoc/templates/netdoc/htmx/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1005 2023-04-10 16:17:25.000000 netdoc-0.9.55/netdoc/templates/netdoc/htmx/discover_form.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1025 2023-04-10 16:17:25.000000 netdoc-0.9.55/netdoc/templates/netdoc/htmx/logexport_form.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3046 2023-04-10 16:20:47.000000 netdoc-0.9.55/netdoc/templates/netdoc/macaddresstableentry.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/netdoc/templatetags/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/templatetags/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/netdoc/templatetags/__pycache__/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      148 2023-04-10 14:52:59.000000 netdoc-0.9.55/netdoc/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-04-10 14:52:59.000000 netdoc-0.9.55/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      890 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/templatetags/netdoc_buttons.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:38.029746 netdoc-0.9.55/netdoc/tests/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/tests/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15086 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/tests/test.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    11155 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/topologies.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5128 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    27100 2023-04-13 18:43:34.000000 netdoc-0.9.55/netdoc/utils.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18389 2023-04-13 18:43:33.000000 netdoc-0.9.55/netdoc/views.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 18:43:37.897744 netdoc-0.9.55/netdoc.egg-info/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-13 18:43:37.000000 netdoc-0.9.55/netdoc.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6905 2023-04-13 18:43:37.000000 netdoc-0.9.55/netdoc.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-13 18:43:37.000000 netdoc-0.9.55/netdoc.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-05 14:49:45.000000 netdoc-0.9.55/netdoc.egg-info/not-zip-safe
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      132 2023-04-13 18:43:37.000000 netdoc-0.9.55/netdoc.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        7 2023-04-13 18:43:37.000000 netdoc-0.9.55/netdoc.egg-info/top_level.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-04-13 18:43:38.029746 netdoc-0.9.55/setup.cfg
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1272 2023-04-13 18:43:34.000000 netdoc-0.9.55/setup.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.935201 netdoc-0.9.56/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.56/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      241 2023-04-05 08:40:22.000000 netdoc-0.9.56/MANIFEST.in
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-25 14:22:47.935201 netdoc-0.9.56/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     9982 2023-04-24 17:00:01.000000 netdoc-0.9.56/README.md
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.839199 netdoc-0.9.56/netdoc/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2218 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.847200 netdoc-0.9.56/netdoc/api/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/api/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2812 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/api/serializers.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      597 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/api/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1207 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/api/views.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.851199 netdoc-0.9.56/netdoc/discoverers/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/discoverers/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6978 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/discoverers/netmiko_cisco_ios.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5160 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/discoverers/netmiko_cisco_nxos.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6514 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/discoverers/netmiko_cisco_xr.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6406 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/discoverers/netmiko_hp_comware.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4511 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/discoverers/netmiko_linux.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3613 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/filtersets.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6587 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/forms.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.887200 netdoc-0.9.56/netdoc/ingestors/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1205 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3710 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2014 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2457 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1705 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      822 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1544 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1951 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2602 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3959 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1660 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      886 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1010 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1238 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3677 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2349 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      824 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2000 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2668 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3936 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1509 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2020 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      888 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      909 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1204 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1529 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3673 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2347 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1802 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2921 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2709 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_route.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      980 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1562 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      894 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2980 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1385 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2626 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1038 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1687 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2035 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2962 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3964 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1514 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      895 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      899 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1202 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_linux_arp__an.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1008 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_linux_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1412 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_address_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1933 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_link_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2450 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_route_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      711 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_vrf_show.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.891200 netdoc-0.9.56/netdoc/migrations/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13632 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0001_initial.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1800 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3399 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3022 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      577 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      453 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0006_alter_routetableentry_metric.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      419 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/0007_discoverylog_supported.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/migrations/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15079 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/models.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2436 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/navigation.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2988 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/nornir_inventory.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.891200 netdoc-0.9.56/netdoc/reports/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5880 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/reports/NetDoc.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.895200 netdoc-0.9.56/netdoc/schemas/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1937 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/arptableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4549 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/cable.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/credential.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4374 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/device.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1508 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/devicerole.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1714 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/devicetype.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3905 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/discoverable.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3176 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/discoverylog.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8791 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1362 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/ipaddress.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1978 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/macaddresstableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1453 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/manufacturer.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/prefix.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2904 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/routetableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      884 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/site.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1623 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2476 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/schemas/vrf.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.895200 netdoc-0.9.56/netdoc/scripts/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13085 2023-04-25 14:22:45.000000 netdoc-0.9.56/netdoc/scripts/NetDoc.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.831199 netdoc-0.9.56/netdoc/static/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.831199 netdoc-0.9.56/netdoc/static/netdoc/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.895200 netdoc-0.9.56/netdoc/static/netdoc/css/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/css/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/css/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)   220164 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/css/vis-network.min.css
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.907201 netdoc-0.9.56/netdoc/static/netdoc/img/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      305 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/access-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/backup.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    28633 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/circuit.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8387 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/core-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     9522 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/distribution-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15596 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/firewall.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1614 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/internal-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5537 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/isp-cpe-material.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5079 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/non-racked-devices.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15857 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/power-feed.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18685 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/power-panel.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4710 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/power-units.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    34335 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/provider-networks.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13504 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/router.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4484 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/server.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/storage.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8308 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/unknown.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/wan-network.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6975 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/img/wireless-ap.png
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.911201 netdoc-0.9.56/netdoc/static/netdoc/js/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/js/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/js/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4198 2023-04-05 14:32:29.000000 netdoc-0.9.56/netdoc/static/netdoc/js/diagram.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/js/netdoc.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)   702066 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/js/vis-network.min.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)  1930592 2023-04-05 08:40:22.000000 netdoc-0.9.56/netdoc/static/netdoc/js/vis-network.min.js.map
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8198 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/tables.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3912 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/tasks.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.831199 netdoc-0.9.56/netdoc/templates/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.927201 netdoc-0.9.56/netdoc/templates/netdoc/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3038 2023-04-10 16:21:20.000000 netdoc-0.9.56/netdoc/templates/netdoc/arptableentry.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.931201 netdoc-0.9.56/netdoc/templates/netdoc/buttons/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      451 2023-04-10 16:17:25.000000 netdoc-0.9.56/netdoc/templates/netdoc/buttons/discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      337 2023-04-10 16:17:25.000000 netdoc-0.9.56/netdoc/templates/netdoc/buttons/export.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1669 2023-04-10 16:21:17.000000 netdoc-0.9.56/netdoc/templates/netdoc/credential.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1439 2023-04-10 16:29:06.000000 netdoc-0.9.56/netdoc/templates/netdoc/diagram.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2654 2023-04-10 16:23:32.000000 netdoc-0.9.56/netdoc/templates/netdoc/discoverable.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1217 2023-04-10 16:26:08.000000 netdoc-0.9.56/netdoc/templates/netdoc/discoverable_bulk_discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      638 2023-04-10 16:26:30.000000 netdoc-0.9.56/netdoc/templates/netdoc/discoverable_discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-04-10 16:23:40.000000 netdoc-0.9.56/netdoc/templates/netdoc/discoverable_list.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5123 2023-04-10 16:23:17.000000 netdoc-0.9.56/netdoc/templates/netdoc/discoverylog.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.931201 netdoc-0.9.56/netdoc/templates/netdoc/htmx/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1005 2023-04-10 16:17:25.000000 netdoc-0.9.56/netdoc/templates/netdoc/htmx/discover_form.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1025 2023-04-10 16:17:25.000000 netdoc-0.9.56/netdoc/templates/netdoc/htmx/logexport_form.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3046 2023-04-10 16:20:47.000000 netdoc-0.9.56/netdoc/templates/netdoc/macaddresstableentry.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.931201 netdoc-0.9.56/netdoc/templatetags/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/templatetags/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.931201 netdoc-0.9.56/netdoc/templatetags/__pycache__/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      148 2023-04-16 15:43:43.000000 netdoc-0.9.56/netdoc/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-04-16 15:43:43.000000 netdoc-0.9.56/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      890 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/templatetags/netdoc_buttons.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.935201 netdoc-0.9.56/netdoc/tests/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/tests/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    16779 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/tests/test.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    11155 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/topologies.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5128 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    27006 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/utils.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18389 2023-04-25 14:22:44.000000 netdoc-0.9.56/netdoc/views.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-25 14:22:47.843199 netdoc-0.9.56/netdoc.egg-info/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-25 14:22:47.000000 netdoc-0.9.56/netdoc.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6905 2023-04-25 14:22:47.000000 netdoc-0.9.56/netdoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-25 14:22:47.000000 netdoc-0.9.56/netdoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-05 14:49:45.000000 netdoc-0.9.56/netdoc.egg-info/not-zip-safe
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      132 2023-04-25 14:22:47.000000 netdoc-0.9.56/netdoc.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        7 2023-04-25 14:22:47.000000 netdoc-0.9.56/netdoc.egg-info/top_level.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-04-25 14:22:47.935201 netdoc-0.9.56/setup.cfg
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1272 2023-04-25 14:22:45.000000 netdoc-0.9.56/setup.py
```

### Comparing `netdoc-0.9.55/LICENSE` & `netdoc-0.9.56/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/README.md` & `netdoc-0.9.56/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,16 @@
         'NTC_TEMPLATES_DIR': '/opt/ntc-templates/ntc_templates/templates',
         'NORNIR_LOG': '/tmp/nornir.log',
         'NORNIR_TIMEOUT': 300,
         'NORNIR_SKIP_LIST': [
             r'show ver',
             r'.* bgp .*',
         ],
+        "RAISE_ON_CDP_FAIL": True,
+        "RAISE_ON_LLDP_FAIL": True,
     },
 }
 RQ_DEFAULT_TIMEOUT = 600
 SECRET_KEY = '01234567890123456789012345678901234567890123456789'
 ~~~
 
 Upgrade and install dependencies for netbox:
```

### Comparing `netdoc-0.9.55/netdoc/__init__.py` & `netdoc-0.9.56/netdoc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Main class."""
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.9.55"
+__version__ = "0.9.56"
 
 import os
 import pkgutil
 import shutil
 
 from django.conf import settings
 
@@ -27,16 +27,18 @@
     author = "Andrea Dainese"
     author_email = "andrea@adainese.it"
     base_url = "netdoc"
     required_settings = ["NTC_TEMPLATES_DIR"]
     default_settings = {
         "NTC_TEMPLATES_DIR": "/opt/ntc-templates/ntc_templates/templates",
         "NORNIR_LOG": f"{settings.BASE_DIR}/nornir.log",
-        "NORNIR_TIMEOUT": 120,
+        "NORNIR_TIMEOUT": 300,
         "NORNIR_SKIP_LIST": [],
+        "RAISE_ON_CDP_FAIL": True,
+        "RAISE_ON_LLDP_FAIL": True,
     }
 
 
 config = NetdocConfig  # pylint: disable=invalid-name
 
 # Setting NTC_TEMPLATES_DIR
 os.environ.setdefault("NET_TEXTFSM", PLUGIN_SETTINGS.get("NTC_TEMPLATES_DIR"))
```

### Comparing `netdoc-0.9.55/netdoc/api/serializers.py` & `netdoc-0.9.56/netdoc/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/api/urls.py` & `netdoc-0.9.56/netdoc/api/urls.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/api/views.py` & `netdoc-0.9.56/netdoc/api/views.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/discoverers/netmiko_cisco_ios.py` & `netdoc-0.9.56/netdoc/discoverers/netmiko_cisco_ios.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/discoverers/netmiko_cisco_nxos.py` & `netdoc-0.9.56/netdoc/discoverers/netmiko_cisco_nxos.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/discoverers/netmiko_cisco_xr.py` & `netdoc-0.9.56/netdoc/discoverers/netmiko_cisco_xr.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/discoverers/netmiko_hp_comware.py` & `netdoc-0.9.56/netdoc/discoverers/netmiko_hp_comware.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/discoverers/netmiko_linux.py` & `netdoc-0.9.56/netdoc/discoverers/netmiko_linux.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/filtersets.py` & `netdoc-0.9.56/netdoc/filtersets.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/forms.py` & `netdoc-0.9.56/netdoc/forms.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 __license__ = "GPLv3"
 
 from django import forms
 
 from dcim.models import Device, Site, DeviceRole
 from ipam.models import VRF
 
-from netbox.forms import (
-    NetBoxModelForm,
-    NetBoxModelFilterSetForm,
-    NetBoxModelCSVForm,
-    NetBoxModelBulkEditForm,
-)
 from utilities.forms import (
     CSVModelChoiceField,
     DynamicModelChoiceField,
     DynamicModelMultipleChoiceField,
     StaticSelect,
     BOOLEAN_WITH_BLANK_CHOICES,
     add_blank_choice,
 )
+from netbox.forms import (
+    NetBoxModelForm,
+    NetBoxModelFilterSetForm,
+    NetBoxModelCSVForm,
+    NetBoxModelBulkEditForm,
+)
 
 from netdoc.models import (
     Credential,
     Discoverable,
     DiscoveryLog,
     DiscoveryModeChoices,
     DiagramModeChoices,
```

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_hostname.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,12 +85,13 @@
                 }
                 discoverable.create(**remote_discoverable_data)
 
         # Link
         cable.link(
             left_interface_id=local_interface_o.id,
             right_interface_id=remote_interface_o.id,
+            protocol="cdp",
         )
 
     # Update the log
     log.ingested = True
     log.save()
```

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,12 +92,13 @@
                 }
                 discoverable.create(**remote_discoverable_data)
 
         # Link
         cable.link(
             left_interface_id=local_interface_o.id,
             right_interface_id=remote_interface_o.id,
+            protocol="lldp",
         )
 
     # Update the log
     log.ingested = True
     log.save()
```

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_hostname.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,12 +83,13 @@
                 }
                 discoverable.create(**remote_discoverable_data)
 
         # Link
         cable.link(
             left_interface_id=local_interface_o.id,
             right_interface_id=remote_interface_o.id,
+            protocol="cdp",
         )
 
     # Update the log
     log.ingested = True
     log.save()
```

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,12 +92,13 @@
                 }
                 discoverable.create(**remote_discoverable_data)
 
         # Link
         cable.link(
             left_interface_id=local_interface_o.id,
             right_interface_id=remote_interface_o.id,
+            protocol="lldp",
         )
 
     # Update the log
     log.ingested = True
     log.save()
```

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_hostname.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_arp.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,12 +83,13 @@
                 }
                 discoverable.create(**remote_discoverable_data)
 
         # Link
         cable.link(
             left_interface_id=local_interface_o.id,
             right_interface_id=remote_interface_o.id,
+            protocol="cdp",
         )
 
     # Update the log
     log.ingested = True
     log.save()
```

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,12 +71,13 @@
             }
             remote_interface_o = interface.create(**remote_interface_data)
 
         # Link
         cable.link(
             left_interface_id=local_interface_o.id,
             right_interface_id=remote_interface_o.id,
+            protocol="lldp",
         )
 
     # Update the log
     log.ingested = True
     log.save()
```

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_route.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_route.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_arp.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_interface.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,12 +71,13 @@
             }
             remote_interface_o = interface.create(**remote_interface_data)
 
         # Link
         cable.link(
             left_interface_id=local_interface_o.id,
             right_interface_id=remote_interface_o.id,
+            protocol="lldp",
         )
 
     # Update the log
     log.ingested = True
     log.save()
```

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,12 +92,13 @@
                 }
                 discoverable.create(**remote_discoverable_data)
 
         # Link
         cable.link(
             left_interface_id=local_interface_o.id,
             right_interface_id=remote_interface_o.id,
+            protocol="lldp",
         )
 
     # Update the log
     log.ingested = True
     log.save()
```

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_hp_comware_hostname.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_hp_comware_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_linux_arp__an.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_linux_arp__an.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_linux_hostname.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_linux_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_address_show.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_address_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_link_show.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_link_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_route_show.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_route_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/ingestors/netmiko_linux_ip_vrf_show.py` & `netdoc-0.9.56/netdoc/ingestors/netmiko_linux_ip_vrf_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/migrations/0001_initial.py` & `netdoc-0.9.56/netdoc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py` & `netdoc-0.9.56/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py` & `netdoc-0.9.56/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py` & `netdoc-0.9.56/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py` & `netdoc-0.9.56/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/models.py` & `netdoc-0.9.56/netdoc/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 import re
 from OuiLookup import OuiLookup
 
 from django.db import models
 from django.urls import reverse
 
-from netbox.models import NetBoxModel
 from ipam.fields import IPAddressField
 from dcim.fields import MACAddressField
 from utilities.choices import ChoiceSet
+from netbox.models import NetBoxModel
 
 from netdoc.utils import parse_netmiko_output, CONFIG_COMMANDS, FAILURE_OUTPUT
 
 
 class DeviceImageChoices(ChoiceSet):
     """Image used in diagrams associated to device roles."""
```

### Comparing `netdoc-0.9.55/netdoc/navigation.py` & `netdoc-0.9.56/netdoc/navigation.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/nornir_inventory.py` & `netdoc-0.9.56/netdoc/nornir_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/reports/NetDoc.py` & `netdoc-0.9.56/netdoc/reports/NetDoc.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/arptableentry.py` & `netdoc-0.9.56/netdoc/schemas/arptableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/cable.py` & `netdoc-0.9.56/netdoc/schemas/cable.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 
 from jsonschema import validate, FormatChecker
 
+from django.conf import settings
 from django.db.utils import IntegrityError
 from django.contrib.contenttypes.models import ContentType
 
 from dcim.models import Interface as Interface_model, Cable, CableTermination
 
 from netdoc.schemas import interface
 
+PLUGIN_SETTINGS = settings.PLUGINS_CONFIG.get("netdoc", {})
 TERMINATION_TYPE = ContentType.objects.get(model="interface")
 
 
 def get_schema():
     """Return the JSON schema to validate ArpTableEntry data."""
     return {
         "type": "object",
@@ -65,19 +67,20 @@
     if left_interface_o.name < right_interface_o.name:
         # Interface comparison
         return left_interface_o, right_interface_o
     # Interface names cannot be equal
     return right_interface_o, left_interface_o
 
 
-def link(**kwargs):
+def link(protocol=None, **kwargs):
     """Link two Interface objects.
 
     Both Interface objects must not be already linked.
     """
+    protocol = protocol.upper()
     validate(kwargs, get_schema_create(), format_checker=FormatChecker())
 
     # Sort interfaces
     left_interface_o, right_interface_o = sort_interfaces(**kwargs)
 
     try:
         cable_o = Cable.objects.filter(terminations__interface=left_interface_o).get(
@@ -95,20 +98,22 @@
             )
 
             # Trigger Cable update
             cable_o._terminations_modified = True  # pylint: disable=protected-access
             cable_o.full_clean()
             cable_o.save()
         except IntegrityError as exc:
-            # Crossed L2 connections with multiple devices (do we have a hub or a CDP/LLDP
+            # L2 connections with multiple devices (do we have a hub or a CDP/LLDP
             # forwarding device?)
-            raise IntegrityError(
-                f"Multiple neighbors on {left_interface_o.device}:{left_interface_o}"
-                + f" or {right_interface_o.device}:{right_interface_o}"
-            ) from exc
+            if PLUGIN_SETTINGS.get(f"RAISE_ON_{protocol}_FAIL"):
+                raise IntegrityError(
+                    f"Multiple neighbors on {left_interface_o.device}:{left_interface_o}"
+                    + f" or {right_interface_o.device}:{right_interface_o}"
+                ) from exc
+            pass
 
 
 def unlink(**kwargs):
     """Unlink two Interface objects."""
     validate(kwargs, get_schema_create(), format_checker=FormatChecker())
 
     # Sort interfaces
```

### Comparing `netdoc-0.9.55/netdoc/schemas/credential.py` & `netdoc-0.9.56/netdoc/schemas/credential.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/device.py` & `netdoc-0.9.56/netdoc/schemas/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,26 +70,33 @@
 
 
 def create(manufacturer="Unknown", **kwargs):
     """Create a Device.
 
     Before need to get or create Manufacturer, DeviceModel, and DeviceType.
     """
+    unknown_model = (
+        "Unknown device"
+        if manufacturer == "Unknown"
+        else f"Unknown {manufacturer} device"
+    )
     manufacturer_o = manufacturer_api.get(name=manufacturer)
     if not manufacturer_o:
         manufacturer_o = manufacturer_api.create(name=manufacturer)
 
     devicerole_o = devicerole.get(name="Unknown")
     if not devicerole_o:
         devicerole_o = devicerole.create(name="Unknown")
 
-    devicetype_o = devicetype.get(model="Unknown", manufacturer_id=manufacturer_o.id)
+    devicetype_o = devicetype.get(
+        model=unknown_model, manufacturer_id=manufacturer_o.id
+    )
     if not devicetype_o:
         devicetype_o = devicetype.create(
-            model="Unknown", manufacturer_id=manufacturer_o.id
+            model=unknown_model, manufacturer_id=manufacturer_o.id
         )
 
     kwargs.update(
         {
             "device_role_id": devicerole_o.id,
             "device_type_id": devicetype_o.id,
         }
```

### Comparing `netdoc-0.9.55/netdoc/schemas/devicerole.py` & `netdoc-0.9.56/netdoc/schemas/devicerole.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/devicetype.py` & `netdoc-0.9.56/netdoc/schemas/devicetype.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/discoverable.py` & `netdoc-0.9.56/netdoc/schemas/discoverable.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/discoverylog.py` & `netdoc-0.9.56/netdoc/schemas/discoverylog.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/interface.py` & `netdoc-0.9.56/netdoc/schemas/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,27 +109,27 @@
         "name",
         "type",
         "device_id",
     ]
     return schema
 
 
-def create(int_type="other", **kwargs):
+def create(type="other", **kwargs):
     """Create an Interface."""
     # The following are updated in update_mode
     if "mode" in kwargs:
         del kwargs["mode"]
     if "untagged_vlan_id" in kwargs:
         del kwargs["untagged_vlan_id"]
     if "tagged_vlan_ids" in kwargs:
         del kwargs["tagged_vlan_ids"]
 
     data = {
         **kwargs,
-        "type": int_type,  # Default type is other
+        "type": type,  # Default type is other
         "label": utils.normalize_interface_label(kwargs.get("name")),  # Set label
     }
 
     data = utils.delete_empty_keys(data)
     obj = utils.object_create(Interface_model, **data)
     return obj
```

### Comparing `netdoc-0.9.55/netdoc/schemas/ipaddress.py` & `netdoc-0.9.56/netdoc/schemas/ipaddress.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/macaddresstableentry.py` & `netdoc-0.9.56/netdoc/schemas/macaddresstableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/manufacturer.py` & `netdoc-0.9.56/netdoc/schemas/manufacturer.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/prefix.py` & `netdoc-0.9.56/netdoc/schemas/prefix.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/routetableentry.py` & `netdoc-0.9.56/netdoc/schemas/routetableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/site.py` & `netdoc-0.9.56/netdoc/schemas/site.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/vlan.py` & `netdoc-0.9.56/netdoc/schemas/vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/schemas/vrf.py` & `netdoc-0.9.56/netdoc/schemas/vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/scripts/NetDoc.py` & `netdoc-0.9.56/netdoc/scripts/NetDoc.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/css/LICENSE` & `netdoc-0.9.56/netdoc/static/netdoc/css/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/css/vis-network.min.css` & `netdoc-0.9.56/netdoc/static/netdoc/css/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/LICENSE` & `netdoc-0.9.56/netdoc/static/netdoc/img/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/access-switch.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/access-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/backup.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/backup.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/circuit.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/circuit.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/core-switch.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/core-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/distribution-switch.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/distribution-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/firewall.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/firewall.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/internal-switch.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/internal-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/isp-cpe-material.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/isp-cpe-material.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/non-racked-devices.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/non-racked-devices.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/power-feed.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/power-feed.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/power-panel.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/power-panel.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/power-units.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/power-units.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/provider-networks.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/provider-networks.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/router.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/router.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/server.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/server.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/storage.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/storage.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/unknown.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/unknown.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/wan-network.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/wan-network.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/img/wireless-ap.png` & `netdoc-0.9.56/netdoc/static/netdoc/img/wireless-ap.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/js/LICENSE` & `netdoc-0.9.56/netdoc/static/netdoc/js/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/js/diagram.js` & `netdoc-0.9.56/netdoc/static/netdoc/js/diagram.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/js/netdoc.js` & `netdoc-0.9.56/netdoc/static/netdoc/js/netdoc.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/js/vis-network.min.js` & `netdoc-0.9.56/netdoc/static/netdoc/js/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/static/netdoc/js/vis-network.min.js.map` & `netdoc-0.9.56/netdoc/static/netdoc/js/vis-network.min.js.map`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/tables.py` & `netdoc-0.9.56/netdoc/tables.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/tasks.py` & `netdoc-0.9.56/netdoc/tasks.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/templates/netdoc/arptableentry.html` & `netdoc-0.9.56/netdoc/templates/netdoc/arptableentry.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/templates/netdoc/credential.html` & `netdoc-0.9.56/netdoc/templates/netdoc/credential.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/templates/netdoc/diagram.html` & `netdoc-0.9.56/netdoc/templates/netdoc/diagram.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/templates/netdoc/discoverable.html` & `netdoc-0.9.56/netdoc/templates/netdoc/discoverable.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/templates/netdoc/discoverable_bulk_discover.html` & `netdoc-0.9.56/netdoc/templates/netdoc/discoverable_bulk_discover.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/templates/netdoc/discoverable_discover.html` & `netdoc-0.9.56/netdoc/templates/netdoc/discoverable_discover.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/templates/netdoc/discoverable_list.html` & `netdoc-0.9.56/netdoc/templates/netdoc/discoverable_list.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/templates/netdoc/discoverylog.html` & `netdoc-0.9.56/netdoc/templates/netdoc/discoverylog.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/templates/netdoc/htmx/discover_form.html` & `netdoc-0.9.56/netdoc/templates/netdoc/htmx/discover_form.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/templates/netdoc/htmx/logexport_form.html` & `netdoc-0.9.56/netdoc/templates/netdoc/htmx/logexport_form.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/templates/netdoc/macaddresstableentry.html` & `netdoc-0.9.56/netdoc/templates/netdoc/macaddresstableentry.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc` & `netdoc-0.9.56/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 10 14:52:50 2023 UTC, .py size: 890 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c222 3464 7a03 0000  o........"4dz...
+00000000: 6f0d 0d0a 0000 0000 564d 3864 7a03 0000  o.......VM8dz...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 6406 6c05 6d06 5a06 0100 6405  Z.d.d.l.m.Z...d.
 00000050: 6407 6c07 6d08 5a08 0100 6405 6408 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6506 a00b a100 5a0c 650c  m.Z...e.....Z.e.
 00000070: a00d 6409 a101 640a 640b 8400 8301 5a0e  ..d...d.d.....Z.
```

### Comparing `netdoc-0.9.55/netdoc/templatetags/netdoc_buttons.py` & `netdoc-0.9.56/netdoc/templatetags/netdoc_buttons.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/tests/test.py` & `netdoc-0.9.56/netdoc/tests/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     # Test total Device objects
     device_qs = Device.objects.all()
     test_o.assertEquals(len(device_qs), len(expected_results))
 
     # Test each item
     for expected_result in expected_results:
         device_o = Device.objects.get(name=expected_result.get("name"))
+        test_o.assertEquals(device_o.device_type.model, expected_result.get("model"))
         test_o.assertEquals(
             device_o.device_type.manufacturer.name, expected_result.get("manufacturer")
         )
         test_o.assertEquals(device_o.serial, expected_result.get("serial"))
 
         if device_o.site:
             test_o.assertEquals(device_o.site.name, expected_result.get("site"))
@@ -290,14 +291,44 @@
             interface__label=expected_result.get("interface"),
             mac_address=expected_result.get("mac_address"),
             ip_address=expected_result.get("ip_address") + "/32",
         )
         test_o.assertEquals(arp_o.vendor, expected_result.get("vendor"))
 
 
+def test_routes(test_o, expected_results):
+    """Test RouteTableEntry given an expected_results dict."""
+    # Test total RouteTableEntry objects
+    route_qs = RouteTableEntry.objects.all()
+    test_o.assertEquals(len(route_qs), len(expected_results))
+
+    # Test each item
+    for expected_result in expected_results:
+        route_o = RouteTableEntry.objects.get(
+            device__name=expected_result.get("device"),
+            destination=expected_result.get("destination"),
+            distance=expected_result.get("distance"),
+            metric=expected_result.get("metric"),
+            protocol=expected_result.get("protocol"),
+            vrf__name=expected_result.get("vrf"),
+        )
+        if route_o.nexthop_ip:
+            test_o.assertEquals(
+                str(route_o.nexthop_ip.ip), expected_result.get("nexthop_ip")
+            )
+        else:
+            test_o.assertIs(expected_result.get("nexthop_ip"), None)
+        if route_o.nexthop_if:
+            test_o.assertEquals(
+                route_o.nexthop_if.label, expected_result.get("nexthop_if")
+            )
+        else:
+            test_o.assertIs(expected_result.get("nexthop_if"), None)
+
+
 def load_scenario(lab_path):
     """Load DiscoveryLog files and return the list of expected result files."""
     expected_result_files = []
 
     # Purge all data
     print("Deleting old data... ", end="")
     Cable.objects.all().delete()
@@ -338,14 +369,23 @@
             if filename.endswith(".json"):
                 filepath_medata = f"{dirpath}/{filename}"
                 filepath_raw_output = filepath_medata.replace(".json", ".raw")
                 address = filename.split("-")[0]
                 with open(filepath_medata, "r", encoding="utf-8") as log_fh:
                     # Load metadata
                     discoverablelog_json = json.load(log_fh)
+                    discoverablelog_json["command"] = discoverablelog_json["details"][
+                        "command"
+                    ]
+                    discoverablelog_json["order"] = discoverablelog_json["details"][
+                        "order"
+                    ]
+                    discoverablelog_json["template"] = discoverablelog_json["details"][
+                        "template"
+                    ]
                 with open(filepath_raw_output, "r", encoding="utf-8") as raw_fh:
                     # Load raw output
                     raw_output = raw_fh.read()
 
                 # Create discoverable
                 discoverable_o, created = discoverable_api.get_or_create(
                     address=address,
```

### Comparing `netdoc-0.9.55/netdoc/topologies.py` & `netdoc-0.9.56/netdoc/topologies.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/urls.py` & `netdoc-0.9.56/netdoc/urls.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc/utils.py` & `netdoc-0.9.56/netdoc/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,25 +187,22 @@
                         delete_empty_keys(v_i)
     return dct
 
 
 def export_log(log):
     """Export DiscoveryLog in JSON format."""
     data = {
-        "command": log.command,
         "configuration": log.configuration,
         "details": log.details,
-        "order": log.order,
+        "discoverable__mode": log.discoverable.mode,
+        "ingested": log.ingested,
+        "parsed": log.parsed,
         "parsed_output": log.parsed_output,
         "raw_output": log.raw_output,
-        "template": log.template,
         "success": log.success,
-        "parsed": log.parsed,
-        "ingested": log.ingested,
-        "discoverable__mode": log.discoverable.mode,
     }
     return data
 
 
 def filter_keys(dct, allowed_keys):
     """Return a dict with only allowed keys."""
     filtered_dct = {}
```

### Comparing `netdoc-0.9.55/netdoc/views.py` & `netdoc-0.9.56/netdoc/views.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/netdoc.egg-info/SOURCES.txt` & `netdoc-0.9.56/netdoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.55/setup.py` & `netdoc-0.9.56/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     twine upload dist/*
 """
 
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.9.55"
+__version__ = "0.9.56"
 
 from setuptools import find_packages, setup
 
 setup(
     name="netdoc",
     version=__version__,
     description="Network Documentation plugin for NetBox",
```

