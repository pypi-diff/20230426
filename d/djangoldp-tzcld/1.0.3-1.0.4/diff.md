# Comparing `tmp/djangoldp_tzcld-1.0.3.tar.gz` & `tmp/djangoldp_tzcld-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_tzcld-1.0.3.tar", last modified: Wed Apr  5 20:34:25 2023, max compression
+gzip compressed data, was "dist/djangoldp_tzcld-1.0.4.tar", last modified: Wed Apr 26 15:33:53 2023, max compression
```

## Comparing `djangoldp_tzcld-1.0.3.tar` & `djangoldp_tzcld-1.0.4.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:34:25.000000 djangoldp_tzcld-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-05 20:34:25.000000 djangoldp_tzcld-1.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:34:25.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld.egg-info/
--rw-r--r--   0 root         (0) root         (0)      272 2023-04-05 20:34:25.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 20:34:25.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1378 2023-04-05 20:34:25.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-05 20:34:25.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-05 20:34:25.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      272 2023-04-05 20:34:25.000000 djangoldp_tzcld-1.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:34:25.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/
--rw-rw-rw-   0 root         (0) root         (0)    17014 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2347 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-05 20:34:23.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 20:34:25.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     5896 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py
--rw-rw-rw-   0 root         (0) root         (0)     9812 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0017_merge_20230405_1526.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0002_tzcldcommunity_contact_job.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      817 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
--rw-rw-rw-   0 root         (0) root         (0)     1774 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py
--rw-rw-rw-   0 root         (0) root         (0)    18022 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py
--rw-rw-rw-   0 root         (0) root         (0)     4403 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
--rw-rw-rw-   0 root         (0) root         (0)     1816 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-04-05 20:34:05.000000 djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      272 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/
+-rw-rw-rw-   0 root         (0) root         (0)    18055 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2347 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-26 15:33:51.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:33:53.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5896 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py
+-rw-rw-rw-   0 root         (0) root         (0)     9812 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0002_tzcldcommunity_contact_job.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)    18022 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py
+-rw-rw-rw-   0 root         (0) root         (0)     4403 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-04-26 15:33:37.000000 djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py
```

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld.egg-info/SOURCES.txt` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,9 +24,12 @@
 djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
 djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
 djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
 djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
 djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
 djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
 djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
-djangoldp_tzcld/migrations/0017_merge_20230405_1526.py
+djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
+djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
+djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
+djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
 djangoldp_tzcld/migrations/__init__.py
```

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/models.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,34 +9,49 @@
 from djangoldp_tzcld.permissions import TzcldCommunityProfilePermissions
 
 #############################
 # Extend user model
 #############################
 
 
-class TzcldContactMember(Model):
-    member = models.OneToOneField(CommunityMember, on_delete=models.CASCADE, related_name="tzcld_contact_member")
-    is_primary = models.BooleanField(default=False)
+class TzcldTerritoryDepartment(Model):
+    name = models.CharField(max_length=254, blank=True, null=True, default='')
 
     def __str__(self):
         try:
             return '{} ({})'.format(self.name, self.urlid)
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        verbose_name = _('TZCLD Contact Member')
-        verbose_name_plural = _("TZCLD Contact Members")
+        verbose_name = _('TZCLD Department')
+        verbose_name_plural = _("TZCLD Departments")
         anonymous_perms = ['view']
-        authenticated_perms = ['view']
-        superuser_perms = ['inherit', 'change']
-        container_path = "tzcld-contact-member/"
-        serializer_fields = ['@id', 'member', 'is_primary']
+        container_path = "tzcld-departments/"
+        serializer_fields = ['@id', 'name']
         nested_fields = []
-        rdf_type = "tzcld:contactMember"
+        rdf_type = "tzcld:departments"
+
+class TzcldTerritoryRegion(Model):
+    name = models.CharField(max_length=254, blank=True, null=True, default='')
+
+    def __str__(self):
+        try:
+            return '{} ({})'.format(self.name, self.urlid)
+        except:
+            return self.urlid
+
+    class Meta(Model.Meta):
+        verbose_name = _('TZCLD Région')
+        verbose_name_plural = _("TZCLD Régions")
+        anonymous_perms = ['view']
+        container_path = "tzcld-regions/"
+        serializer_fields = ['@id', 'name']
+        nested_fields = []
+        rdf_type = "tzcld:regions"
 
 class TzcldProfilesMembership(Model):
     name = models.CharField(max_length=255, blank=False, null=True, default='')
 
 
     def __str__(self):
         try:
@@ -60,16 +75,18 @@
 class TzcldProfile(Model):
     user = models.OneToOneField(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, related_name="tzcld_profile")
     #description = models.CharField(max_length=255, blank=True, null=True, default='')
     #postal_code = models.CharField(max_length=255, blank=True, null=True, default='')
     #address = models.CharField(max_length=255, blank=True, null=True, default='')
     #phone = models.CharField(max_length=255, blank=True, null=True, default='')
     #position = models.CharField(max_length=255, blank=True, null=True, default='')
-    membership = models.ForeignKey(TzcldProfilesMembership, on_delete=models.DO_NOTHING,related_name='membership', blank=False, null=True)
     last_contribution_year = models.CharField(max_length=255, blank=True, null=True, default='')
+    regions = models.ManyToManyField(TzcldTerritoryRegion, related_name='profile_regions', blank=True)
+    departments = models.ManyToManyField(TzcldTerritoryDepartment, related_name='profile_department', blank=True)
+    is_member = models.BooleanField(default=False)
 
     def __str__(self):
         try:
             return '{} ({})'.format(self.user.get_full_name(), self.urlid)
         except:
             return self.urlid
 
@@ -77,79 +94,51 @@
         verbose_name = _('TZCLD Profile')
         verbose_name_plural = _("TZCLD Profiles")
         anonymous_perms = ['view']
         authenticated_perms = ['inherit']
         superuser_perms = ['inherit', 'change']
         ordering = ['user']
         #serializer_fields = ['@id', 'description', 'regions', 'postal_code', 'address', 'events', 'phone', 'orgs', 'position', 'membership', 'last_contribution_year', 'jobs']
-        serializer_fields = ['@id', 'membership', 'last_contribution_year', 'jobs']
+        serializer_fields = ['@id', 'last_contribution_year', 'jobs', 'regions', 'departments', 'is_member']
         rdf_type = "tzcld:profile"
         auto_author = 'user'
         depth = 3
 
-class TzcldTerritoryDepartment(Model):
-    name = models.CharField(max_length=254, blank=True, null=True, default='')
-
-    def __str__(self):
-        try:
-            return '{} ({})'.format(self.name, self.urlid)
-        except:
-            return self.urlid
-
-    class Meta(Model.Meta):
-        verbose_name = _('TZCLD Department')
-        verbose_name_plural = _("TZCLD Departments")
-        anonymous_perms = ['view']
-        container_path = "tzcld-departments/"
-        serializer_fields = ['@id', 'name']
-        nested_fields = []
-        rdf_type = "tzcld:departments"
-
-class TzcldTerritoryRegion(Model):
-    name = models.CharField(max_length=254, blank=True, null=True, default='')
-
-    def __str__(self):
-        try:
-            return '{} ({})'.format(self.name, self.urlid)
-        except:
-            return self.urlid
-
-    class Meta(Model.Meta):
-        verbose_name = _('TZCLD Région')
-        verbose_name_plural = _("TZCLD Régions")
-        anonymous_perms = ['view']
-        container_path = "tzcld-regions/"
-        serializer_fields = ['@id', 'name']
-        nested_fields = []
-        rdf_type = "tzcld:regions"
-
 class TzcldProfileJob(Model):
     position = models.CharField(max_length=255, blank=True, null=True, default='')
     organisation = models.CharField(max_length=255, blank=True, null=True, default='')
     address = models.CharField(max_length=255, blank=True, null=True, default='')
     postal_code = models.CharField(max_length=255, blank=True, null=True, default='')
     city = models.CharField(max_length=255, blank=True, null=True, default='')
     department = models.ForeignKey(TzcldTerritoryDepartment, on_delete=models.DO_NOTHING,related_name='job_department', blank=True, null=True)
-    address_public = models.BooleanField(default=False)
+    #address_public = models.BooleanField(default=False)
     profile = models.ForeignKey(TzcldProfile, on_delete=models.CASCADE,related_name='jobs', blank=True, null=True)
+    link = models.CharField(max_length=255, blank=True, null=True, default='')
+    
+    phone = models.CharField(max_length=255, blank=True, null=True, default='')
+    phone_public = models.BooleanField(default=False)
+    mobile_phone = models.CharField(max_length=255, blank=True, null=True, default='')
+    mobile_phone_public = models.BooleanField(default=False)
+    email = models.CharField(max_length=255, blank=True, null=True, default='')
+    email_public = models.BooleanField(default=False)
 
     def __str__(self):
         try:
             return '{} ({})'.format(self.position, self.urlid)
         except:
             return self.urlid
 
     class Meta(Model.Meta):
         verbose_name = _('TZCLD profile job')
         verbose_name_plural = _("TZCLD profiile jobs")
         anonymous_perms = ['view']
         authenticated_perms = ['inherit', 'view', 'add', 'change']
         superuser_perms = ['inherit', 'change']
         container_path = "tzcld-profile-job/"
-        serializer_fields = ['@id', 'position', 'organisation', 'address', 'postal_code', 'city', 'department', 'address_public', 'phones', 'emails', 'profile']
+        serializer_fields = ['@id', 'position', 'organisation', 'address', 'postal_code', 'city', 'department','profile', 'link','phone' ,'phone_public' ,'mobile_phone' ,'mobile_phone_public' ,'email' ,'email_public' ]
         nested_fields = []
         rdf_type = "tzcld:profileJob"
 
 #############################
 # Old models version
 #############################
 """
@@ -256,14 +245,15 @@
 
 class TzcldCommunity(Model):
     community = models.OneToOneField(Community, on_delete=models.CASCADE, related_name='tzcld_profile', null=True, blank=True)
     kind = models.ForeignKey(TzcldTerritoriesKind, on_delete=models.DO_NOTHING,related_name='kind', blank=True, null=True)
     step_state = models.ForeignKey(TzcldTerritoriesStepState, on_delete=models.DO_NOTHING,related_name='step_state', blank=False, null=True)
     department = models.ForeignKey(TzcldTerritoryDepartment, on_delete=models.DO_NOTHING,related_name='department', blank=True, null=True)
     region = models.ForeignKey(TzcldTerritoryRegion, on_delete=models.DO_NOTHING,related_name='region', blank=True, null=True)
+    membership = models.ForeignKey(TzcldProfilesMembership, on_delete=models.DO_NOTHING,related_name='membership', blank=False, null=True)
     """
     features = models.CharField(max_length=255, blank=True, null=True, default='')
     contact_mail_1 = models.CharField(max_length=255, blank=True, null=True, default='')
     contact_mail_2 = models.CharField(max_length=255, blank=True, null=True, default='')
     contact_mail_3 = models.CharField(max_length=255, blank=True, null=True, default='')
     contact_last_name = models.CharField(max_length=255, blank=True, null=True, default='')
     contact_first_name = models.CharField(max_length=255, blank=True, null=True, default='')
@@ -284,15 +274,15 @@
         permission_classes = [TzcldCommunityProfilePermissions]
         anonymous_perms = ['view']
         authenticated_perms = ['inherit', 'add']
         superuser_perms = ['view']
         ordering = ['community']
         container_path = "/tzcld-communities/"
         #serializer_fields = ['@id', 'contact_first_name', 'contact_last_name', 'contact_job', 'kind', 'features', 'region', 'contact_mail_1', 'contact_mail_2', 'contact_mail_3', 'membership', 'last_contribution_year']
-        serializer_fields = ['@id', 'community', 'kind', 'step_state', 'kind', 'department', 'region', 'locations']
+        serializer_fields = ['@id', 'community', 'kind', 'step_state', 'kind', 'department', 'region', 'locations', 'tzcld_community_contacts', 'membership']
         rdf_type = "tzcld:communityProfile"
         depth = 3
 
 
 class TzcldTerritoryLocation(Model):
     name = models.CharField(max_length=255, blank=True, null=True, default='')
     address = models.CharField(max_length=255, blank=True, null=True, default='')
@@ -371,14 +361,38 @@
         authenticated_perms = ['inherit']
         superuser_perms = ['inherit', 'change']
         container_path = "tzcld-contact-email/"
         serializer_fields = ['@id', 'email', 'email_type', 'email_public', 'job', 'location']
         nested_fields = []
         rdf_type = "tzcld:email"
 
+
+class TzcldContactMember(Model):
+    member = models.OneToOneField(CommunityMember, on_delete=models.CASCADE, related_name="tzcld_contact_member")
+    tzcldCommunity = models.ForeignKey(TzcldCommunity, on_delete=models.CASCADE, related_name='tzcld_community_contacts', null=True, blank=True)
+    is_primary = models.BooleanField(default=False)
+
+    def __str__(self):
+        try:
+            return '{} ({})'.format(self.name, self.urlid)
+        except:
+            return self.urlid
+
+    class Meta(Model.Meta):
+        verbose_name = _('TZCLD Contact Member')
+        verbose_name_plural = _("TZCLD Contact Members")
+        anonymous_perms = ['view']
+        authenticated_perms = ['view']
+        superuser_perms = ['inherit', 'change']
+        container_path = "tzcld-contact-member/"
+        serializer_fields = ['@id', 'member', 'is_primary']
+        nested_fields = []
+        rdf_type = "tzcld:contactMember"
+
+
 # Create tzcld user profile, job instance and contact email/phone when user is created
 @receiver(post_save, sender=settings.AUTH_USER_MODEL)
 def create_user_tzcld_profile(sender, instance, created, **kwargs):
     if not Model.is_external(instance) and created:
         tzcld_profile = TzcldProfile.objects.create(user=instance)
         profile_job = TzcldProfileJob.objects.create(profile=tzcld_profile)
         TzcldContactEmail.objects.create(job=profile_job)
```

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/permissions.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/admin.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0001_initial.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 class Migration(migrations.Migration):
 
     dependencies = [
         ('djangoldp_tzcld', '0011_auto_20230328_1045'),
     ]
 
     operations = [
+        migrations.RunSQL("DROP INDEX IF EXISTS djangoldp_tzcld_tzcldterritoryregion_urlid_83f59f84_like"),
         migrations.RenameModel(
             old_name='TzcldTerritoryRegion',
             new_name='TzcldTerritoryDepartment',
         ),
+        migrations.RunSQL("DROP INDEX IF EXISTS djangoldp_tzcld_tzcldterritoryregion_urlid_83f59f84_like"),
         migrations.RemoveField(
             model_name='tzcldcommunity',
             name='region',
         ),
         migrations.AddField(
             model_name='tzcldcommunity',
             name='department',
```

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.3/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py` & `djangoldp_tzcld-1.0.4/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py`

 * *Files identical despite different names*

