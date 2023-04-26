# Comparing `tmp/netbox-vlan-manager-0.0.2.tar.gz` & `tmp/netbox-vlan-manager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-vlan-manager-0.0.2.tar", last modified: Tue Mar  7 18:44:14 2023, max compression
+gzip compressed data, was "netbox-vlan-manager-0.0.3.tar", last modified: Tue Apr 25 15:13:14 2023, max compression
```

## Comparing `netbox-vlan-manager-0.0.2.tar` & `netbox-vlan-manager-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 18:44:14.047529 netbox-vlan-manager-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1609 2023-03-07 18:44:14.047529 netbox-vlan-manager-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1256 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 18:44:14.047529 netbox-vlan-manager-0.0.2/netbox_vlan_manager/
--rw-r--r--   0 runner    (1001) docker     (116)      400 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 18:44:14.047529 netbox-vlan-manager-0.0.2/netbox_vlan_manager/api/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      718 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (116)      216 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)      385 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/api/views.py
--rw-r--r--   0 runner    (1001) docker     (116)      576 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 18:44:14.047529 netbox-vlan-manager-0.0.2/netbox_vlan_manager/migrations/
--rw-r--r--   0 runner    (1001) docker     (116)     1364 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      743 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/models.py
--rw-r--r--   0 runner    (1001) docker     (116)      537 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/navigation.py
--rw-r--r--   0 runner    (1001) docker     (116)     2683 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 18:44:14.047529 netbox-vlan-manager-0.0.2/netbox_vlan_manager/templatetags/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      196 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/templatetags/view_helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)      996 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     1491 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager/views.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 18:44:14.047529 netbox-vlan-manager-0.0.2/netbox_vlan_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1609 2023-03-07 18:44:14.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      807 2023-03-07 18:44:14.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-07 18:44:14.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-07 18:44:13.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       20 2023-03-07 18:44:14.000000 netbox-vlan-manager-0.0.2/netbox_vlan_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-07 18:44:14.047529 netbox-vlan-manager-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1210 2023-03-07 18:44:04.000000 netbox-vlan-manager-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/netbox_vlan_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/netbox_vlan_manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/netbox_vlan_manager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/netbox_vlan_manager/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/templatetags/view_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-25 15:13:14.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 15:13:14.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:13:14.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:13:14.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 15:13:14.000000 netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 15:13:14.236038 netbox-vlan-manager-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-25 15:13:01.000000 netbox-vlan-manager-0.0.3/setup.py
```

### Comparing `netbox-vlan-manager-0.0.2/LICENSE` & `netbox-vlan-manager-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.2/PKG-INFO` & `netbox-vlan-manager-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-vlan-manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: VLAN Manager for multiple VLAN Groups
 Home-page: https://github.com/miyuk/netbox-vlan-manager/
 Author: miyuk
 Author-email: miyuk@miyuk.net
 Classifier: Development Status :: 1 - Planning
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `netbox-vlan-manager-0.0.2/README.md` & `netbox-vlan-manager-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.2/netbox_vlan_manager/api/serializers.py` & `netbox-vlan-manager-0.0.3/netbox_vlan_manager/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.2/netbox_vlan_manager/forms.py` & `netbox-vlan-manager-0.0.3/netbox_vlan_manager/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.2/netbox_vlan_manager/migrations/0001_initial.py` & `netbox-vlan-manager-0.0.3/netbox_vlan_manager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.2/netbox_vlan_manager/models.py` & `netbox-vlan-manager-0.0.3/netbox_vlan_manager/models.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.2/netbox_vlan_manager/navigation.py` & `netbox-vlan-manager-0.0.3/netbox_vlan_manager/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.2/netbox_vlan_manager/tables.py` & `netbox-vlan-manager-0.0.3/netbox_vlan_manager/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.2/netbox_vlan_manager/urls.py` & `netbox-vlan-manager-0.0.3/netbox_vlan_manager/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,8 +32,13 @@
         'vlan-group-sets/<int:pk>/changelog/',
         ObjectChangeLogView.as_view(),
         name='vlangroupset_changelog',
         kwargs={
             'model': models.VLANGroupSet
         }
     ),
+    path(
+        'vlan-group-sets/<int:pk>/export-vlans/',
+        views.VLANGroupSetExportVLANs.as_view(),
+        name='export_vlans'
+    ),
 )
```

### Comparing `netbox-vlan-manager-0.0.2/netbox_vlan_manager/views.py` & `netbox-vlan-manager-0.0.3/netbox_vlan_manager/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.db.models import Count
 from netbox.views import generic
 from ipam.models import VLAN
 from . import models, tables, forms
 from .tables import VLANGroupSetVLANTable
-
+from django_tables2.export.export import TableExport
 
 class VLANGroupSetView(generic.ObjectView):
     queryset = models.VLANGroupSet.objects.all()
 
     def get_extra_context(self, request, instance):
         vlan_groups = instance.vlan_groups.all()
         max_vid = max(vlan_groups, key=(lambda x: x.max_vid)).max_vid
@@ -40,7 +40,31 @@
 class VLANGroupSetEditView(generic.ObjectEditView):
     queryset = models.VLANGroupSet.objects.all()
     form = forms.VLANGroupSetForm
 
 
 class VLANGroupSetDeleteView(generic.ObjectDeleteView):
     queryset = models.VLANGroupSet.objects.all()
+
+class VLANGroupSetExportVLANs(generic.ObjectView):
+    queryset = models.VLANGroupSet.objects.all()
+
+    def get(self, request, **kwargs):
+        print(kwargs)
+        instance = self.get_object(**kwargs)
+        vlan_groups = instance.vlan_groups.all()
+        max_vid = max(vlan_groups, key=(lambda x: x.max_vid)).max_vid
+        min_vid = min(vlan_groups, key=(lambda x: x.min_vid)).min_vid
+
+        vlan_group_vlans = []
+        for vid in range(min_vid, max_vid + 1):
+            item = {}
+            item['vid'] = vid
+            vlans = VLAN.objects.filter(vid=vid)
+            item['vlans'] = vlans
+            item['status'] = 'Available' if vlans.count() == 0 else 'In Use'
+            vlan_group_vlans.append(item)
+        vlans_table = VLANGroupSetVLANTable(
+            vlan_group_vlans, vlan_groups=vlan_groups)
+        vlans_table.configure(request)
+        exporter = TableExport('csv', vlans_table)
+        return exporter.response(f'VLANGroupSetVLANs_{instance.name}.csv')
```

### Comparing `netbox-vlan-manager-0.0.2/netbox_vlan_manager.egg-info/PKG-INFO` & `netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-vlan-manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: VLAN Manager for multiple VLAN Groups
 Home-page: https://github.com/miyuk/netbox-vlan-manager/
 Author: miyuk
 Author-email: miyuk@miyuk.net
 Classifier: Development Status :: 1 - Planning
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `netbox-vlan-manager-0.0.2/netbox_vlan_manager.egg-info/SOURCES.txt` & `netbox-vlan-manager-0.0.3/netbox_vlan_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.0.2/setup.py` & `netbox-vlan-manager-0.0.3/setup.py`

 * *Files identical despite different names*

