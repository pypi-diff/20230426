# Comparing `tmp/prisma_configure_mesh-1.0.0b1.tar.gz` & `tmp/prisma_configure_mesh-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prisma_configure_mesh-1.0.0b1.tar", last modified: Wed Jun  2 07:56:37 2021, max compression
+gzip compressed data, was "prisma_configure_mesh-1.1.0b1.tar", last modified: Wed Apr 26 05:31:01 2023, max compression
```

## Comparing `prisma_configure_mesh-1.0.0b1.tar` & `prisma_configure_mesh-1.1.0b1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-06-02 07:56:37.003940 prisma_configure_mesh-1.0.0b1/
--rw-r--r--   0 aaron      (501) staff       (20)     5070 2021-06-02 07:56:37.004105 prisma_configure_mesh-1.0.0b1/PKG-INFO
--rw-r--r--   0 aaron      (501) staff       (20)     3629 2021-06-02 07:45:16.000000 prisma_configure_mesh-1.0.0b1/README.md
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-06-02 07:56:36.997839 prisma_configure_mesh-1.0.0b1/prisma_configure_mesh.egg-info/
--rw-r--r--   0 aaron      (501) staff       (20)     5070 2021-06-02 07:56:36.000000 prisma_configure_mesh-1.0.0b1/prisma_configure_mesh.egg-info/PKG-INFO
--rw-r--r--   0 aaron      (501) staff       (20)      523 2021-06-02 07:56:36.000000 prisma_configure_mesh-1.0.0b1/prisma_configure_mesh.egg-info/SOURCES.txt
--rw-r--r--   0 aaron      (501) staff       (20)        1 2021-06-02 07:56:36.000000 prisma_configure_mesh-1.0.0b1/prisma_configure_mesh.egg-info/dependency_links.txt
--rw-r--r--   0 aaron      (501) staff       (20)       68 2021-06-02 07:56:36.000000 prisma_configure_mesh-1.0.0b1/prisma_configure_mesh.egg-info/entry_points.txt
--rw-r--r--   0 aaron      (501) staff       (20)       41 2021-06-02 07:56:36.000000 prisma_configure_mesh-1.0.0b1/prisma_configure_mesh.egg-info/requires.txt
--rw-r--r--   0 aaron      (501) staff       (20)       22 2021-06-02 07:56:36.000000 prisma_configure_mesh-1.0.0b1/prisma_configure_mesh.egg-info/top_level.txt
-drwxr-xr-x   0 aaron      (501) staff       (20)        0 2021-06-02 07:56:37.002858 prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/
--rw-r--r--   0 aaron      (501) staff       (20)    41839 2021-06-02 07:54:30.000000 prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/__init__.py
--rw-r--r--   0 aaron      (501) staff       (20)    30893 2021-06-02 07:36:07.000000 prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/anynets.py
--rw-r--r--   0 aaron      (501) staff       (20)     3248 2021-06-02 02:23:07.000000 prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/menus.py
--rw-r--r--   0 aaron      (501) staff       (20)    11720 2021-06-02 04:04:56.000000 prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/sites.py
--rw-r--r--   0 aaron      (501) staff       (20)     1930 2021-06-02 02:58:35.000000 prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/utils.py
--rw-r--r--   0 aaron      (501) staff       (20)       97 2021-06-02 03:22:34.000000 prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/versions.py
--rw-r--r--   0 aaron      (501) staff       (20)    49306 2021-06-02 07:21:13.000000 prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/vpn.py
--rw-r--r--   0 aaron      (501) staff       (20)      289 2021-06-02 07:56:37.004609 prisma_configure_mesh-1.0.0b1/setup.cfg
--rw-r--r--   0 aaron      (501) staff       (20)     1210 2021-06-02 07:40:31.000000 prisma_configure_mesh-1.0.0b1/setup.py
+drwxr-xr-x   0 aaron      (505) staff       (20)        0 2023-04-26 05:31:01.642204 prisma_configure_mesh-1.1.0b1/
+-rw-r--r--   0 aaron      (505) staff       (20)     1070 2021-06-01 20:27:55.000000 prisma_configure_mesh-1.1.0b1/LICENSE
+-rw-r--r--   0 aaron      (505) staff       (20)     8237 2023-04-26 05:31:01.642371 prisma_configure_mesh-1.1.0b1/PKG-INFO
+-rw-r--r--   0 aaron      (505) staff       (20)     7531 2023-04-26 05:28:20.000000 prisma_configure_mesh-1.1.0b1/README.md
+drwxr-xr-x   0 aaron      (505) staff       (20)        0 2023-04-26 05:31:01.635944 prisma_configure_mesh-1.1.0b1/prisma_configure_mesh.egg-info/
+-rw-r--r--   0 aaron      (505) staff       (20)     8237 2023-04-26 05:31:01.000000 prisma_configure_mesh-1.1.0b1/prisma_configure_mesh.egg-info/PKG-INFO
+-rw-r--r--   0 aaron      (505) staff       (20)      531 2023-04-26 05:31:01.000000 prisma_configure_mesh-1.1.0b1/prisma_configure_mesh.egg-info/SOURCES.txt
+-rw-r--r--   0 aaron      (505) staff       (20)        1 2023-04-26 05:31:01.000000 prisma_configure_mesh-1.1.0b1/prisma_configure_mesh.egg-info/dependency_links.txt
+-rw-r--r--   0 aaron      (505) staff       (20)       67 2023-04-26 05:31:01.000000 prisma_configure_mesh-1.1.0b1/prisma_configure_mesh.egg-info/entry_points.txt
+-rw-r--r--   0 aaron      (505) staff       (20)       41 2023-04-26 05:31:01.000000 prisma_configure_mesh-1.1.0b1/prisma_configure_mesh.egg-info/requires.txt
+-rw-r--r--   0 aaron      (505) staff       (20)       22 2023-04-26 05:31:01.000000 prisma_configure_mesh-1.1.0b1/prisma_configure_mesh.egg-info/top_level.txt
+drwxr-xr-x   0 aaron      (505) staff       (20)        0 2023-04-26 05:31:01.641413 prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/
+-rw-r--r--   0 aaron      (505) staff       (20)    60961 2023-04-26 05:02:11.000000 prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/__init__.py
+-rw-r--r--   0 aaron      (505) staff       (20)    45442 2023-04-26 05:17:19.000000 prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/anynets.py
+-rw-r--r--   0 aaron      (505) staff       (20)     3248 2021-06-02 02:23:07.000000 prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/menus.py
+-rw-r--r--   0 aaron      (505) staff       (20)    11720 2021-06-02 04:04:56.000000 prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/sites.py
+-rw-r--r--   0 aaron      (505) staff       (20)     1930 2021-06-02 02:58:35.000000 prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/utils.py
+-rw-r--r--   0 aaron      (505) staff       (20)      100 2023-04-26 05:30:05.000000 prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/versions.py
+-rw-r--r--   0 aaron      (505) staff       (20)    49306 2021-06-02 07:21:13.000000 prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/vpn.py
+-rw-r--r--   0 aaron      (505) staff       (20)      299 2023-04-26 05:31:01.642979 prisma_configure_mesh-1.1.0b1/setup.cfg
+-rw-r--r--   0 aaron      (505) staff       (20)     1220 2023-04-26 05:30:05.000000 prisma_configure_mesh-1.1.0b1/setup.py
```

### Comparing `prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/__init__.py` & `prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -60,18 +60,20 @@
     "reload_list_b": None,          # list of sites b to be used on re-loop of logic
     "reload_wn_list_a": None,       # list of WAN Networks a to be used on re-loop of logic
     "reload_wn_list_b": None,       # list of WAN Networks b to be used on re-loop of logic
     "loop_counter": 0               # Loop counter, arg files only loaded on first loop.
 }
 
 
-def siteid_to_name_dict(sdk_vars, sdk_session):
+def siteid_to_name_dict(sdk_vars, sdk_session, site_name_to_domain=False, site_id_to_domain=False):
     """
     Create a Site ID <-> Name xlation constructs
-    :param passed_sdk_vars: sdk_vars global info struct
+    :param sdk_vars: sdk_vars global info struct
+    :param site_name_to_domain: if not bool False, should be dict to receive site name->domain (service_endpoint) ID map.
+    :param site_id_to_domain: if not bool False, should be dict to receive site id->domain (service_endpoint) ID map.
     :return: xlate_dict, a dict with siteid key to site name. site_list, a list of site IDs
     """
     id_xlate_dict = {}
     name_xlate_dict = {}
     site_id_list = []
     site_name_list = []
     site_tags = {}
@@ -88,27 +90,34 @@
         return {}, {}, [], []
 
     # build translation dict
     for site in sites_list:
         name = site.get('name')
         site_id = site.get('id')
         role = site.get('element_cluster_role')
+        service_binding = site.get('service_binding')
 
         if name and site_id:
             id_xlate_dict[site_id] = name
             name_xlate_dict[name] = site_id
             site_id_list.append(site_id)
             site_name_list.append(name)
             if not site['tags']:
                 site['tags'] = []
             site_tags[name] = site['tags']
 
         if site_id and role:
             site_id_to_role[site_id] = role
 
+        # check for service binding / domain dict
+        if site_name_to_domain is not False and isinstance(site_name_to_domain, dict) and name and service_binding:
+            site_name_to_domain[name] = service_binding
+        if site_id_to_domain is not False and isinstance(site_id_to_domain, dict) and id and service_binding:
+            site_id_to_domain[site_id] = service_binding
+
     return id_xlate_dict, name_xlate_dict, site_id_list, site_name_list, site_id_to_role, site_tags
 
 
 def wannetworkid_to_name_dict(sdk_vars, sdk_session):
     """
     Create a Site ID <-> Name xlation constructs
     :param passed_sdk_vars: sdk_vars global info struct
@@ -144,15 +153,15 @@
 
         if wan_network_id and wn_type:
             wan_network_id_type[wan_network_id] = wn_type
 
     return id_xlate_dict, name_xlate_dict, wan_network_id_list, wan_network_name_list, wan_network_id_type
 
 
-def selective_loop_function():
+def custom_loop_function():
 
     # check for initial launch
     if sdk_vars["loop_counter"] == 0:
 
         sdk_vars['load_list_a'] = ARGS['load_list_a']
         sdk_vars['load_list_b'] = ARGS['load_list_b']
         sdk_vars['load_wn_list_a'] = ARGS['load_wn_list_a']
@@ -510,14 +519,384 @@
 
     # Increment global loop counter
     sdk_vars["loop_counter"] += 1
 
     return reload_or_exit
 
 
+def regional_loop_function(operation):
+    """
+    For enable Regional Domain Mesh (HUB/SPOKE)
+    :param operation: The operation string, one of 'create_n' (Full Mesh) 'delete_c' (hub/spoke)
+    :return:
+    """
+
+    if ARGS["verbose"] == 1:
+        logging.basicConfig(level=logging.INFO,
+                            format="%(levelname)s [%(name)s.%(funcName)s:%(lineno)d] %(message)s")
+        clilogger = logging.getLogger()
+        clilogger.setLevel(logging.INFO,)
+    elif ARGS["verbose"] >= 2:
+        logging.basicConfig(level=logging.DEBUG,
+                            format="%(levelname)s [%(name)s.%(funcName)s:%(lineno)d] %(message)s")
+        clilogger = logging.getLogger()
+        clilogger.setLevel(logging.DEBUG)
+    else:
+        # set logging off unless asked for
+        pass
+
+    sitename_to_domain_id = {}
+    siteid_to_domain_id = {}
+    # Get/update list of sites, create python dictionary to map site ID to name.
+    id_sitename_dict, sitename_id_dict, site_id_list, site_name_list, site_id_to_role_dict, site_tags \
+        = siteid_to_name_dict(sdk_vars, CGX_SESSION, site_name_to_domain=sitename_to_domain_id,
+                              site_id_to_domain=siteid_to_domain_id)
+    id_wan_network_name_dict, wan_network_name_id_dict, wan_network_id_list, wan_network_name_list, \
+        wan_network_to_type_dict = wannetworkid_to_name_dict(sdk_vars, CGX_SESSION)
+
+    # jd(siteid_to_domain_id)
+
+    # pull domain membership info
+    servicebindingmaps_cache = CGX_SESSION.extract_items(CGX_SESSION.get.servicebindingmaps())
+
+    sbm_name_to_id = CGX_SESSION.build_lookup_dict(servicebindingmaps_cache)
+    sbm_id_to_name = CGX_SESSION.build_lookup_dict(servicebindingmaps_cache, key_val='id', value_val='name')
+
+    # jd(sbm_name_to_id)
+    # jd(sbm_id_to_name)
+
+    domain_branch_count = {}
+    domain_dc_count = {}
+    domain_name_to_site_name_list = {}
+    domain_name_to_site_id_list = {}
+    for sbm_name, sbm_id in sbm_name_to_id.items():
+        branch_count = 0
+        dc_count = 0
+        domain_name_to_site_name_list[sbm_name] = []
+        domain_name_to_site_id_list[sbm_name] = []
+        # iterate sites and find matches
+        for site_id, domain_id in siteid_to_domain_id.items():
+            site_role = site_id_to_role_dict.get(site_id)
+            if domain_id == sbm_id:
+                domain_name_to_site_id_list[sbm_name].append(site_id)
+                domain_name_to_site_name_list[sbm_name].append(id_sitename_dict.get(site_id))
+                if site_role == "HUB":
+                    dc_count += 1
+                elif site_role == "SPOKE":
+                    branch_count += 1
+        domain_branch_count[sbm_name] = branch_count
+        domain_dc_count[sbm_name] = dc_count
+
+    # jd(domain_name_to_site_name_list)
+    # jd(domain_branch_count)
+    # jd(domain_dc_count)
+
+    logger.debug("SITE -> ROLE ({0}): {1}".format(len(site_id_to_role_dict),
+                                                  json.dumps(site_id_to_role_dict, indent=4)))
+
+    # Begin Site Selection - We'll do full mesh logic now, and prune it later by region.
+    site_list_a = site_name_list[:]
+    site_list_b = site_name_list[:]
+    # TODO count site types here.
+
+    # we need to process for both public and private WANs.
+    anynet_specific_type_pub = "public-anynet"
+    anynet_specific_type_priv = "private-anynet"
+
+    # convert site lists (by name) to ID lists. Look up ID in previous sitename_id dict. if exists, enter.
+    site_id_list_a = []
+    for site in site_list_a:
+        site_id = sitename_id_dict.get(site, None)
+        if site_id:
+            site_id_list_a.append(site_id)
+
+    site_id_list_b = []
+    for site in site_list_b:
+        site_id = sitename_id_dict.get(site, None)
+        if site_id:
+            site_id_list_b.append(site_id)
+
+    # combine site lists and remove duplicates so we can pull topology info from API once per site.
+    combined_site_id_list = list(site_id_list_a)
+    combined_site_id_list.extend(x for x in site_id_list_b if x not in site_id_list_a)
+
+    # print json.dumps(combined_site_id_list, indent=4)
+
+    # get/update topology
+
+    print("Loading VPN topology information for {0} sites, please wait.".format(len(combined_site_id_list)))
+
+    logger.debug('COMBINED_SITE_ID_LIST ({0}): {1}'.format(len(combined_site_id_list),
+                                                           json.dumps(combined_site_id_list, indent=4)))
+
+    swi_to_wan_network_dict = {}
+    swi_to_site_dict = {}
+    wan_network_to_swi_dict = {}
+    all_anynets_pub = {}
+    all_anynets_priv = {}
+    site_swi_dict_pub = {}
+    site_swi_dict_priv = {}
+
+    # could be a long query - start a progress bar.
+    pbar = ProgressBar(widgets=[Percentage(), Bar(), ETA()], max_value=len(combined_site_id_list)+1).start()
+    site_processed = 1
+
+    for site in combined_site_id_list:
+        site_swi_list_pub = []
+        site_swi_list_priv = []
+
+        query = {
+            "type": "basenet",
+            "nodes": [
+                site
+            ]
+        }
+
+        status = False
+        rest_call_retry = 0
+        topology = None
+
+        while not status:
+            resp = CGX_SESSION.post.topology(query)
+            status = resp.cgx_status
+            topology = resp.cgx_content
+
+            if not status:
+                print("API request for topology for site ID {0} failed/timed out. Retrying.".format(site))
+                rest_call_retry += 1
+                # have we hit retry limit?
+                if rest_call_retry >= sdk_vars['rest_call_max_retry']:
+                    # Bail out
+                    print("ERROR: could not query site ID {0}. Continuing.".format(site))
+                    status = True
+                    topology = False
+                else:
+                    # wait and keep going.
+                    time.sleep(1)
+
+        if status and topology:
+            # iterate topology. We need to iterate all of the matching SWIs, and existing anynet connections (sorted).
+            logger.debug("TOPOLOGY: {0}".format(json.dumps(topology, indent=4)))
+
+            for link in topology.get('links', []):
+                link_type = link.get('type', "")
+
+                # if an anynet link (SWI to SWI)
+                if link_type in [anynet_specific_type_pub, anynet_specific_type_priv]:
+                    # vpn record, check for uniqueness.
+                    # 4.4.1
+                    source_swi = link.get('source_wan_if_id')
+                    if not source_swi:
+                        # 4.3.x compatibility
+                        source_swi = link.get('source_wan_path_id')
+                        if source_swi:
+                            link['source_wan_if_id'] = source_swi
+                    # 4.4.1
+                    dest_swi = link.get('target_wan_if_id')
+                    if not dest_swi:
+                        # 4.3.x compatibility
+                        dest_swi = link.get('target_wan_path_id')
+                        if dest_swi:
+                            link['target_wan_if_id'] = dest_swi
+                    # create anynet lookup key
+                    anynet_lookup_key = "_".join(sorted([source_swi, dest_swi]))
+                    if link_type in [anynet_specific_type_pub]:
+                        if not all_anynets_pub.get(anynet_lookup_key, None):
+                            # path is not in current anynets, add
+                            all_anynets_pub[anynet_lookup_key] = link
+                    elif link_type in [anynet_specific_type_priv]:
+                        if not all_anynets_priv.get(anynet_lookup_key, None):
+                            # path is not in current anynets, add
+                            all_anynets_priv[anynet_lookup_key] = link
+
+        # Query 2 - now need to query SWI for site, since stub-topology may not be in topology info.
+        status = False
+        site_wan_if_result = False
+
+        while not status:
+            resp = CGX_SESSION.get.waninterfaces(site)
+            status = resp.cgx_status
+            site_wan_if_result = resp.cgx_content
+
+            if not status:
+                print("API request for Site WAN Interfaces for site ID {0} failed/timed out. Retrying.".format(site))
+                time.sleep(1)
+
+        if status and site_wan_if_result:
+            site_wan_if_items = site_wan_if_result.get('items', [])
+            logger.debug('SITE WAN IF ITEMS ({0}): {1}'.format(len(site_wan_if_items),
+                                                               json.dumps(site_wan_if_items, indent=4)))
+
+            # iterate all the site wan interfaces
+            for current_swi in site_wan_if_items:
+                # get the WN bound to the SWI.
+                wan_network_id = current_swi.get('network_id', "")
+                swi_id = current_swi.get('id', "")
+
+                if swi_id:
+                    # update SWI -> Site xlation dict
+                    swi_to_site_dict[swi_id] = site
+
+                # get the SWIs that match the mesh_type
+                if wan_network_id and swi_id and wan_network_to_type_dict.get(wan_network_id, "") in ['publicwan',
+                                                                                                      'privatewan']:
+                    logger.debug('SWI_ID = SITE: {0} = {1}'.format(swi_id, site))
+
+                    # query existing wan_network_to_swi dict if entry exists.
+                    existing_swi_list = wan_network_to_swi_dict.get(wan_network_id, [])
+
+                    # update swi -> WN xlate dict
+                    swi_to_wan_network_dict[swi_id] = wan_network_id
+
+                    # update site-level SWI list.
+                    if wan_network_to_type_dict.get(wan_network_id, "") == 'publicwan':
+                        site_swi_list_pub.append(swi_id)
+                    elif wan_network_to_type_dict.get(wan_network_id, "") == 'privatewan':
+                        site_swi_list_priv.append(swi_id)
+
+                    # update WN -> swi xlate dict
+                    existing_swi_list.append(swi_id)
+                    wan_network_to_swi_dict[wan_network_id] = existing_swi_list
+
+        # add all matching mesh_type stubs to site_swi_dict
+        site_swi_dict_pub[site] = site_swi_list_pub
+        site_swi_dict_priv[site] = site_swi_list_priv
+
+        # iterate bar and counter.
+        site_processed += 1
+        pbar.update(site_processed)
+
+    # finish after iteration.
+    pbar.finish()
+
+    # jd(all_anynets_pub)
+    # jd(all_anynets_priv)
+
+    # update all_anynets with site info. Can't do this above, because xlation table not finished when needed.
+    for anynet_key, link in all_anynets_pub.items():
+        source_swi = link.get('source_wan_if_id')
+        dest_swi = link.get('target_wan_if_id')
+        link['source_site_id'] = swi_to_site_dict.get(source_swi, 'UNKNOWN (Unable to map SWI to Site ID)')
+        link['target_site_id'] = swi_to_site_dict.get(dest_swi, 'UNKNOWN (Unable to map SWI to Site ID)')
+
+    for anynet_key, link in all_anynets_priv.items():
+        source_swi = link.get('source_wan_if_id')
+        dest_swi = link.get('target_wan_if_id')
+        link['source_site_id'] = swi_to_site_dict.get(source_swi, 'UNKNOWN (Unable to map SWI to Site ID)')
+        link['target_site_id'] = swi_to_site_dict.get(dest_swi, 'UNKNOWN (Unable to map SWI to Site ID)')
+
+    logger.debug("SWI -> WN xlate ({0}): {1}".format(len(swi_to_wan_network_dict),
+                                               json.dumps(swi_to_wan_network_dict, indent=4)))
+    logger.debug("All Anynets Pub ({0}): {1}".format(len(all_anynets_pub),
+                                                     json.dumps(all_anynets_pub, indent=4)))
+    logger.debug("All Anynets Pub ({0}): {1}".format(len(all_anynets_priv),
+                                                     json.dumps(all_anynets_priv, indent=4)))
+    logger.debug("SWI construct Pub ({0}): {1}".format(len(site_swi_dict_pub),
+                                                       json.dumps(site_swi_dict_pub, indent=4)))
+    logger.debug("SWI construct Priv ({0}): {1}".format(len(site_swi_dict_priv),
+                                                        json.dumps(site_swi_dict_priv, indent=4)))
+    logger.debug("WN xlate ({0}): {1}".format(len(wan_network_to_swi_dict),
+                                              json.dumps(wan_network_to_swi_dict, indent=4)))
+    logger.debug("SWI -> SITE xlate ({0}): {1}".format(len(swi_to_site_dict),
+                                              json.dumps(swi_to_site_dict, indent=4)))
+
+    # jd(all_anynets_pub)
+    # jd(all_anynets_priv)
+
+    regional_mesh_work_dict = {}
+    for domain_name, domain_site_id_list in domain_name_to_site_id_list.items():
+        regional_mesh_work_dict[domain_name] = {}
+        regional_mesh_work_dict[domain_name]["site_id_list"] = domain_site_id_list
+
+        new_anynets_pub, current_anynets_pub = vpn.no_menu_all_links(domain_site_id_list,
+                                                                     list(domain_site_id_list),
+                                                                     all_anynets_pub,
+                                                                     site_swi_dict_pub,
+                                                                     swi_to_wan_network_dict,
+                                                                     wan_network_to_swi_dict,
+                                                                     id_wan_network_name_dict,
+                                                                     wan_network_name_id_dict,
+                                                                     swi_to_site_dict,
+                                                                     id_sitename_dict,
+                                                                     'publicwan',
+                                                                     site_id_to_role_dict,
+                                                                     sdk_vars=sdk_vars, sdk_session=CGX_SESSION)
+        regional_mesh_work_dict[domain_name]["new_anynets_pub"] = new_anynets_pub
+        modifiable_anynets_pub = {}
+        # only do the modifiable ones
+        for key, value in current_anynets_pub.items():
+            # if modifiable, add to list
+            sub_type = value.get('sub_type', 'other')
+            if sub_type == 'on-demand':
+                modifiable_anynets_pub[key] = value
+
+        regional_mesh_work_dict[domain_name]["current_anynets_pub"] = modifiable_anynets_pub
+
+        new_anynets_priv, current_anynets_priv = vpn.no_menu_all_links(domain_site_id_list,
+                                                                       list(domain_site_id_list),
+                                                                       all_anynets_priv,
+                                                                       site_swi_dict_priv,
+                                                                       swi_to_wan_network_dict,
+                                                                       wan_network_to_swi_dict,
+                                                                       id_wan_network_name_dict,
+                                                                       wan_network_name_id_dict,
+                                                                       swi_to_site_dict,
+                                                                       id_sitename_dict,
+                                                                       'privatewan',
+                                                                       site_id_to_role_dict,
+                                                                       sdk_vars=sdk_vars, sdk_session=CGX_SESSION)
+        regional_mesh_work_dict[domain_name]["new_anynets_priv"] = new_anynets_priv
+        modifiable_anynets_priv = {}
+        # only do the modifiable ones
+        for key, value in current_anynets_priv.items():
+            # if modifiable, add to list
+            sub_type = value.get('sub_type', 'other')
+            if sub_type == 'on-demand':
+                modifiable_anynets_priv[key] = value
+
+        regional_mesh_work_dict[domain_name]["current_anynets_priv"] = modifiable_anynets_priv
+        # write some basic statistics
+        member_sites = len(domain_site_id_list)
+        new_anynets_count = len(new_anynets_pub) + len(new_anynets_priv)
+        current_anynets_count = len(modifiable_anynets_priv) + len(modifiable_anynets_pub)
+        regional_mesh_work_dict[domain_name]["statistics"] = {
+            "sites_count": member_sites,
+            "new_anynets_count": new_anynets_count,
+            "current_anynets_count": current_anynets_count
+        }
+
+        # determine current mesh mode for domain. Assume Custom to start, then update.
+        current_mode = "Custom"
+        if member_sites < 2:
+            # Not enough sites using this Domain. Ignore.
+            current_mode = "Insufficient Sites"
+        elif current_anynets_count == 0:
+            # no current site-site anynets, domain is in hub-spoke.
+            current_mode = "Hub/Spoke"
+        elif new_anynets_count == 0:
+            # no new possible site-site links. Domain is in Full Mesh.
+            current_mode = "Full Mesh"
+        regional_mesh_work_dict[domain_name]["current_mode"] = current_mode
+        # set pending mode to same as current for now.
+        regional_mesh_work_dict[domain_name]["pending_mode"] = current_mode
+
+    # for domain, domain_dict in regional_mesh_work_dict.items():
+    #     print(f"{domain}: ")
+    #     print(f"{domain_dict.get('current_mode')}")
+    #     jd(domain_dict.get("statistics"))
+    #     print("")
+    # jd(regional_mesh_work_dict)
+
+    reload_or_exit = anynets.regional_anynet_menu(regional_mesh_work_dict, swi_to_wan_network_dict,
+                                                  id_wan_network_name_dict, id_sitename_dict, site_id_to_role_dict,
+                                                  sdk_vars, CGX_SESSION)
+
+    return reload_or_exit
+
+
 def allchange_loop_function(operation):
     """
     For enable Full Mesh or Disable Full Mesh (HUB/SPOKE)
     :param operation: The operation string, one of 'create_n' (Full Mesh) 'delete_c' (hub/spoke)
     :return:
     """
 
@@ -917,36 +1296,44 @@
     while loop:
 
         # Print header
         print("")
 
         action = [
             ("Full Mesh", 'full_mesh'),
-            ("Partial/Selective Mesh", 'selective_mesh'),
-            ("Hub/Spoke Links Only", 'hub_spoke')
+            ("Regional Mesh", 'regional_mesh'),
+            ("Hub/Spoke Links Only", 'hub_spoke'),
+            ("Custom Mesh", 'custom_mesh')
         ]
 
         banner = "Choose Prisma SD-WAN Network Meshing Stance:"
         line_fmt = "{0}: {1}"
 
         # just pull 2nd value
         list_name, selected_action = menus.quick_menu(banner, line_fmt, action)
 
         if selected_action == 'full_mesh':
             # do full mesh then exit.
             print("\nChecking network state before moving to Full Mesh.")
             allchange_loop_function('create_n')
             sys.exit()
 
-        elif selected_action == 'selective_mesh':
-            print("\nStarting Interactive Mesh Modification.")
+        elif selected_action == 'regional_mesh':
+            # print("\nLoading Regional Meshing information.")
+            # start main loop for selective mesh
+            main_loop = True
+            while main_loop:
+                main_loop = regional_loop_function('nope')
+
+        elif selected_action == 'custom_mesh':
+            print("\nStarting Interactive Custom Mesh Modification.")
             # start main loop for selective mesh
             main_loop = True
             while main_loop:
-                main_loop = selective_loop_function()
+                main_loop = custom_loop_function()
 
         elif selected_action == "hub_spoke":
             # do Hub/Spoke then exit.
             print("\nChecking network state before moving to Hub/Spoke only.")
             allchange_loop_function('delete_c')
             sys.exit()
```

### Comparing `prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/anynets.py` & `prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/anynets.py`

 * *Files 22% similar despite different names*

```diff
@@ -426,14 +426,191 @@
 
     else:
         print("Canceling...")
 
     return do_we_go
 
 
+def apply_regional_mesh(regional_mesh_dict, sdk_vars, sdk_session):
+
+    new_anynets_pub = {}
+    new_anynets_priv = {}
+    remove_anynets_pub = {}
+    remove_anynets_priv = {}
+
+    for domain, domain_dict in regional_mesh_dict.items():
+        if domain_dict["current_mode"] == domain_dict["pending_mode"]:
+            # no changes here, skip..
+            continue
+        if domain_dict["pending_mode"] == "Full Mesh":
+            # we need to create the creatable anynets
+            new_anynets_pub.update(domain_dict.get("new_anynets_pub", {}))
+            new_anynets_priv.update(domain_dict.get("new_anynets_priv", {}))
+        elif domain_dict["pending_mode"] == "Hub/Spoke":
+            # if hub/spoke we need to remove all optional anynets
+            remove_anynets_pub.update(domain_dict.get("current_anynets_pub", {}))
+            remove_anynets_priv.update(domain_dict.get("current_anynets_priv", {}))
+
+
+    num_new_anynets_pub = len(list(new_anynets_pub.keys()))
+    num_new_anynets_priv = len(list(new_anynets_priv.keys()))
+    num_remove_anynets_pub = len(list(remove_anynets_pub.keys()))
+    num_remove_anynets_priv = len(list(remove_anynets_priv.keys()))
+    num_new_anynets = num_new_anynets_pub + num_new_anynets_priv
+    num_remove_anynets = num_remove_anynets_pub + num_remove_anynets_priv
+    num_anynet_changes = num_new_anynets + num_remove_anynets
+
+    if num_anynet_changes == 0:
+        print("No pending Prisma SD-WAN Regional Mesh changes to apply. Exiting.")
+        sys.exit()
+
+    quick_confirm_string = f"\nPending Prisma SD-WAN Regional Mesh changes will:\n"
+    if num_new_anynets_pub > 0:
+        quick_confirm_string += f"    Create {num_new_anynets_pub} NEW Public WAN Branch-Branch VPN Mesh Links\n"
+    if num_new_anynets_priv > 0:
+        quick_confirm_string += f"    Create {num_new_anynets_priv} NEW Private WAN Branch-Branch VPN Mesh Links\n"
+    if num_remove_anynets_pub > 0:
+        quick_confirm_string += f"    Remove {num_remove_anynets_pub} EXISTING Public WAN Branch-Branch VPN Mesh Links\n"
+    if num_remove_anynets_priv > 0:
+        quick_confirm_string += f"    Remove {num_remove_anynets_priv} EXISTING Private WAN Branch-Branch VPN Mesh Links\n"
+    quick_confirm_string += f"\n"
+    quick_confirm_string += f"Are you sure? "
+
+    # quick confirm
+    do_we_go = menus.quick_confirm(quick_confirm_string, 'N')
+
+    if do_we_go in ['y']:
+        print(f"\nDeploying {num_new_anynets} new and removing {num_remove_anynets} existing Branch-Branch VPN Mesh Links..")
+
+        counter = 1
+        pbar = ProgressBar(widgets=[Percentage(), Bar(), ETA()], max_value=num_anynet_changes+1).start()
+
+        for anynet_uniqueid, anynet in new_anynets_pub.items():
+
+            status = False
+            rest_call_retry = 0
+
+            while not status:
+                status, create_result = create_anynet_link(anynet['source_site_id'], anynet['source_wan_if_id'],
+                                                           anynet['target_site_id'], anynet['target_wan_if_id'],
+                                                           forced=True, admin_state=True, sdk_vars=sdk_vars,
+                                                           sdk_session=sdk_session)
+
+                if not status:
+                    print("API request to create Mesh VPN Link {0}({1}) <-> {2}({3})) failed/timed out. Retrying."
+                          "".format(anynet['source_site_id'], anynet['source_wan_if_id'],
+                                    anynet['target_site_id'], anynet['target_wan_if_id']))
+                    rest_call_retry += 1
+                    # have we hit retry limit?
+                    if rest_call_retry >= MODIFY_RETRY_COUNT:
+                        # Bail out
+                        print("ERROR: Could not create Mesh VPN Link {0}({1}) <-> {2}({3})). Continuing."
+                              "".format(anynet['source_site_id'], anynet['source_wan_if_id'],
+                                        anynet['target_site_id'], anynet['target_wan_if_id']))
+                        status = True
+                        create_result = False
+                    else:
+                        # wait and keep going.
+                        time.sleep(1)
+
+            counter += 1
+            pbar.update(counter)
+
+        for anynet_uniqueid, anynet in new_anynets_priv.items():
+
+            status = False
+            rest_call_retry = 0
+
+            while not status:
+                status, create_result = create_anynet_link(anynet['source_site_id'], anynet['source_wan_if_id'],
+                                                           anynet['target_site_id'], anynet['target_wan_if_id'],
+                                                           forced=True, admin_state=True, sdk_vars=sdk_vars,
+                                                           sdk_session=sdk_session)
+
+                if not status:
+                    print("API request to create Mesh VPN Link {0}({1}) <-> {2}({3})) failed/timed out. Retrying."
+                          "".format(anynet['source_site_id'], anynet['source_wan_if_id'],
+                                    anynet['target_site_id'], anynet['target_wan_if_id']))
+                    rest_call_retry += 1
+                    # have we hit retry limit?
+                    if rest_call_retry >= MODIFY_RETRY_COUNT:
+                        # Bail out
+                        print("ERROR: Could not create Mesh VPN Link {0}({1}) <-> {2}({3})). Continuing."
+                              "".format(anynet['source_site_id'], anynet['source_wan_if_id'],
+                                        anynet['target_site_id'], anynet['target_wan_if_id']))
+                        status = True
+                        create_result = False
+                    else:
+                        # wait and keep going.
+                        time.sleep(1)
+
+            counter += 1
+            pbar.update(counter)
+
+        for anynet_uniqueid, anynet in remove_anynets_pub.items():
+
+            status = False
+            rest_call_retry = 0
+
+            while not status:
+                status, disable_result = delete_anynet_link(anynet['path_id'], sdk_vars=sdk_vars,
+                                                            sdk_session=sdk_session)
+
+                if not status:
+                    print("API request to disable Mesh VPN Link {0} failed/timed out. Retrying."\
+                        .format(anynet['path_id']))
+                    rest_call_retry += 1
+                    if rest_call_retry >= MODIFY_RETRY_COUNT:
+                        # Bail out
+                        print("ERROR: Could not disable Mesh VPN Link {0}. Continuing.".format(anynet['path_id']))
+                        status = True
+                        disable_result = False
+                    else:
+                        # wait and keep going.
+                        time.sleep(1)
+            counter += 1
+            pbar.update(counter)
+
+        for anynet_uniqueid, anynet in remove_anynets_priv.items():
+
+            status = False
+            rest_call_retry = 0
+
+            while not status:
+                status, disable_result = delete_anynet_link(anynet['path_id'], sdk_vars=sdk_vars,
+                                                            sdk_session=sdk_session)
+
+                if not status:
+                    print("API request to disable Mesh VPN Link {0} failed/timed out. Retrying."\
+                        .format(anynet['path_id']))
+                    rest_call_retry += 1
+                    if rest_call_retry >= MODIFY_RETRY_COUNT:
+                        # Bail out
+                        print("ERROR: Could not disable Mesh VPN Link {0}. Continuing.".format(anynet['path_id']))
+                        status = True
+                        disable_result = False
+                    else:
+                        # wait and keep going.
+                        time.sleep(1)
+            counter += 1
+            pbar.update(counter)
+
+
+        # make sure to clear the bar.
+        pbar.finish()
+        print("\nPrisma SD-WAN Fabric successfully updated the Regional Meshing stance.")
+
+    else:
+        print("Canceling...")
+
+    return do_we_go
+
+
+
+
 def print_selection_overview(anynet_text_list, anynet_label):
 
     statistics = {
         'modifiable_anynets': 0,
         'always_anynets': 0,
         'other_anynets': 0,
         'new_anynets': 0
@@ -692,7 +869,142 @@
         create_anynets_menu_both(new_anynets_pub, new_anynets_priv, sdk_vars, sdk_session)
 
     else:
         sdk_session.interactive.logout()
         sys.exit()
 
     return
+
+def regional_anynet_menu(regional_mesh_info_dict, swi_to_wn_dict, id_wan_network_name_dict,
+                         id_sitename_dict, site_id_to_role_dict, sdk_vars, sdk_session):
+    """
+    Main menu for anynet manipulation
+    :param regional_mesh_info_dict: Dict containing detailed info on current/existing anynets
+    :param swi_to_wn_dict: xlation dict for SWI to Wan Network ID
+    :param id_wan_network_name_dict: xlation dict for WAN Network ID to WAN Network Name
+    :param id_sitename_dict: xlation dict for site ID to site Name
+    :param site_id_to_role_dict: site ID to Site Role text.
+    :param sdk_vars: Vars passed in for config/modify
+    :param sdk_session: Authenticated CloudGenix SDK Session.
+    :return: tuple with: action (string or true/false)
+             site_a_action_dict (Site-SWI dict for list A)
+             site_b_action_dict (Site-SWI dict for list B)
+    """
+
+    loop = True
+    while loop:
+        # add line
+        print("")
+        # build action menu
+        action = []
+        insufficient_sites = []
+
+        for domain, domain_dict in regional_mesh_info_dict.items():
+            current_mode = domain_dict.get("current_mode", "Custom")
+            site_count = domain_dict.get("statistics", {}).get("sites_count", "Unknown")
+            pending_mode = domain_dict.get("pending_mode", "Unknown")
+            if site_count in [0, 1, "Unknown"]:
+                # skip this domain, add to insufficient_sites
+                insufficient_sites.append(domain)
+            elif current_mode == pending_mode:
+                line_string = f"{domain} ({site_count} {'site' if site_count == 1 else 'sites'}): Current mode: {current_mode}"
+                action.append((line_string, domain))
+            else:
+                line_string = f"*{domain} ({site_count} {'site' if site_count == 1 else 'sites'}): Pending change to: {pending_mode}"
+                action.append((line_string, domain))
+
+        if insufficient_sites:
+            # some domains have too few sites to mesh. Note them.
+            action.append((f"Apply Changes\n"
+                           f"\n(Note: {len(insufficient_sites)} Regions were below minimum site membership (2) and ignored: "
+                           f"{', '.join(insufficient_sites)})", 'commit'))
+        else:
+            # all domains good - no notes.
+            action.append(("Apply Changes", 'commit'))
+
+        banner = "Select Region to change Meshing Stance:"
+        line_fmt = "{0}: {1}"
+
+        # just pull 2nd value
+        list_name, selected_action = menus.quick_menu(banner, line_fmt, action)
+
+
+        if selected_action == 'commit':
+            do_we_go = apply_regional_mesh(regional_mesh_info_dict, sdk_vars, sdk_session)
+            sys.exit()
+
+        elif selected_action in regional_mesh_info_dict.keys():
+            domain_dict = regional_mesh_info_dict[selected_action]
+            current_mode = domain_dict.get("current_mode", "Custom")
+            site_count = domain_dict.get("statistics", {}).get("sites_count", "Unknown")
+            pending_mode = domain_dict.get("pending_mode", "Unknown")
+            new_anynets_count = domain_dict.get("statistics", {}).get("new_anynets_count", "Unknown")
+            current_anynets_count = domain_dict.get("statistics", {}).get("current_anynets_count", "Unknown")
+
+            print(f"Region {selected_action}:\n"
+                  f"\tSites: {site_count}")
+            if current_mode == pending_mode:
+                  print(f"\tCurrent mode: {current_mode}\n")
+            else:
+                print(f"\tCurrent mode: {current_mode} (pending change to {pending_mode})\n")
+
+            if pending_mode == current_mode:
+                if current_mode not in ["Hub/Spoke", "Full Mesh"]:
+                    action = [
+                        ("Change to Full Mesh", "Full Mesh"),
+                        ("Change to Hub/Spoke", "Hub/Spoke"),
+                        ("Return to previous menu", "return")
+                    ]
+                elif current_mode == "Hub/Spoke":
+                    action = [
+                        ("Change to Full Mesh", "Full Mesh"),
+                        ("Return to previous menu", "return")
+                    ]
+                else:
+                    action = [
+                        ("Change to Hub/Spoke", "Hub/Spoke"),
+                        ("Return to previous menu", "return")
+                    ]
+            else:
+                if current_mode not in ["Hub/Spoke", "Full Mesh"] and pending_mode == "Full Mesh":
+                    action = [
+                        ("Change to Hub/Spoke", "Hub/Spoke"),
+                        ("Revert pending change to Full Mesh", "revert"),
+                        ("Return to previous menu", "return")
+                    ]
+                elif current_mode not in ["Hub/Spoke", "Full Mesh"] and pending_mode == "Hub/Spoke":
+                    action = [
+                        ("Change to Full Mesh", "Full Mesh"),
+                        ("Revert pending change to Hub/Spoke", "revert"),
+                        ("Return to previous menu", "return")
+                    ]
+                elif current_mode == "Hub/Spoke":
+                    # must be pending to Full Mesh
+                    action = [
+                        ("Revert pending change to Full Mesh", "revert"),
+                        ("Return to previous menu", "return")
+                    ]
+                else:
+                    # must be pending to Hub/Spoke
+                    action = [
+                        ("Revert pending change to Hub/Spoke", "revert"),
+                        ("Return to previous menu", "return")
+                    ]
+
+            banner = "Select an action for this region:"
+            line_fmt = "{0}: {1}"
+
+            # just pull 2nd value
+            list_name, sub_selected_action = menus.quick_menu(banner, line_fmt, action)
+
+            if sub_selected_action == "Hub/Spoke":
+                domain_dict["pending_mode"] = "Hub/Spoke"
+            elif sub_selected_action == "Full Mesh":
+                domain_dict["pending_mode"] = "Full Mesh"
+            elif sub_selected_action == "revert":
+                domain_dict["pending_mode"] = domain_dict["current_mode"]
+
+        else:
+            sdk_session.interactive.logout()
+            sys.exit()
+
+    return
```

### Comparing `prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/menus.py` & `prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/menus.py`

 * *Files identical despite different names*

### Comparing `prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/sites.py` & `prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/sites.py`

 * *Files identical despite different names*

### Comparing `prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/utils.py` & `prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/utils.py`

 * *Files identical despite different names*

### Comparing `prisma_configure_mesh-1.0.0b1/prisma_mesh_functions/vpn.py` & `prisma_configure_mesh-1.1.0b1/prisma_mesh_functions/vpn.py`

 * *Files identical despite different names*

### Comparing `prisma_configure_mesh-1.0.0b1/setup.py` & `prisma_configure_mesh-1.1.0b1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='prisma_configure_mesh',
-      version='1.0.0b1',
-      description='Utility for changing from Hub/Spoke to Partial or Full Mesh for Prisma SD-WAN.',
+      version='1.1.0b1',
+      description='Utility for changing from Hub/Spoke to Regional, Full, or Custom Mesh for Prisma SD-WAN.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/ebob9/prisma_configure_mesh',
       author='Aaron Edwards',
       author_email='prisma_configure_mesh@ebob9.com',
       license='MIT',
       install_requires=[
-            'cloudgenix >= 5.5.1b2',
+            'cloudgenix >= 6.2.1b1',
             'progressbar2 >= 3.53.1'
       ],
       packages=['prisma_mesh_functions'],
       entry_points={
             'console_scripts': [
                   'prisma_configure_mesh = prisma_mesh_functions:go'
                   ]
```

