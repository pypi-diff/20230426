# Comparing `tmp/krbjack-1.0.0.tar.gz` & `tmp/krbjack-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krbjack-1.0.0.tar", max compression
+gzip compressed data, was "krbjack-1.0.1.tar", max compression
```

## Comparing `krbjack-1.0.0.tar` & `krbjack-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-04-16 10:50:40.975309 krbjack-1.0.0/krbjack/__init__.py
--rw-r--r--   0        0        0     4844 2023-04-20 21:06:41.754965 krbjack-1.0.0/krbjack/__main__.py
--rw-r--r--   0        0        0     3349 2023-04-16 10:50:33.382821 krbjack-1.0.0/krbjack/custompipes.py
--rw-r--r--   0        0        0    10478 2023-04-20 20:56:42.382098 krbjack-1.0.0/krbjack/krbjacker.py
--rw-r--r--   0        0        0        0 2023-04-16 10:50:53.310403 krbjack-1.0.0/krbjack/modules/__init__.py
--rw-r--r--   0        0        0     7373 2023-04-20 21:12:00.797143 krbjack-1.0.0/krbjack/modules/psexec.py
--rw-r--r--   0        0        0     1784 2023-04-16 10:50:46.295130 krbjack-1.0.0/krbjack/modules/utils.py
--rw-r--r--   0        0        0     6012 2023-04-26 15:57:59.623958 krbjack-1.0.0/krbjack/tcpforward.py
--rw-r--r--   0        0        0     1485 2023-04-16 10:50:21.132287 krbjack-1.0.0/krbjack/utils.py
--rw-r--r--   0        0        0      446 2023-04-16 10:50:04.426169 krbjack-1.0.0/LICENSE
--rw-r--r--   0        0        0      649 2023-04-16 10:49:26.555106 krbjack-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9946 2023-04-20 21:09:09.235044 krbjack-1.0.0/README.md
--rw-r--r--   0        0        0    10809 1970-01-01 00:00:00.000000 krbjack-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-16 10:50:40.975309 krbjack-1.0.1/krbjack/__init__.py
+-rw-r--r--   0        0        0     4844 2023-04-20 21:06:41.754965 krbjack-1.0.1/krbjack/__main__.py
+-rw-r--r--   0        0        0     3349 2023-04-16 10:50:33.382821 krbjack-1.0.1/krbjack/custompipes.py
+-rw-r--r--   0        0        0    10478 2023-04-20 20:56:42.382098 krbjack-1.0.1/krbjack/krbjacker.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:50:53.310403 krbjack-1.0.1/krbjack/modules/__init__.py
+-rw-r--r--   0        0        0     7373 2023-04-20 21:12:00.797143 krbjack-1.0.1/krbjack/modules/psexec.py
+-rw-r--r--   0        0        0     1784 2023-04-16 10:50:46.295130 krbjack-1.0.1/krbjack/modules/utils.py
+-rw-r--r--   0        0        0     6012 2023-04-26 16:00:54.249740 krbjack-1.0.1/krbjack/tcpforward.py
+-rw-r--r--   0        0        0     1485 2023-04-16 10:50:21.132287 krbjack-1.0.1/krbjack/utils.py
+-rw-r--r--   0        0        0      446 2023-04-16 10:50:04.426169 krbjack-1.0.1/LICENSE
+-rw-r--r--   0        0        0      649 2023-04-26 16:01:35.796435 krbjack-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8900 2023-04-26 16:01:13.917585 krbjack-1.0.1/README.md
+-rw-r--r--   0        0        0     9763 1970-01-01 00:00:00.000000 krbjack-1.0.1/PKG-INFO
```

### Comparing `krbjack-1.0.0/krbjack/__main__.py` & `krbjack-1.0.1/krbjack/__main__.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.0/krbjack/custompipes.py` & `krbjack-1.0.1/krbjack/custompipes.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.0/krbjack/krbjacker.py` & `krbjack-1.0.1/krbjack/krbjacker.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.0/krbjack/modules/psexec.py` & `krbjack-1.0.1/krbjack/modules/psexec.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.0/krbjack/modules/utils.py` & `krbjack-1.0.1/krbjack/modules/utils.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.0/krbjack/tcpforward.py` & `krbjack-1.0.1/krbjack/tcpforward.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.0/krbjack/utils.py` & `krbjack-1.0.1/krbjack/utils.py`

 * *Files identical despite different names*

### Comparing `krbjack-1.0.0/pyproject.toml` & `krbjack-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "krbjack"
-version = "1.0.0"
+version = "1.0.1"
 description = "Kerberos AP-REQ hijacking tool with DNS unsecure updates abuse."
 authors = ["Virgile Jarry <virgile@mailbox.org>"]
 readme = "README.md"
 license = "Beerware"
 homepage = "https://github.com/almandin/krbjack"
 repository = "https://github.com/almandin/krbjack"
 documentation = "https://github.com/almandin/krbjack/README.md"
```

### Comparing `krbjack-1.0.0/README.md` & `krbjack-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: krbjack
+Version: 1.0.1
+Summary: Kerberos AP-REQ hijacking tool with DNS unsecure updates abuse.
+Home-page: https://github.com/almandin/krbjack
+License: Beerware
+Author: Virgile Jarry
+Author-email: virgile@mailbox.org
+Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: colorama (>=0.4.4,<0.5.0)
+Requires-Dist: dnspython (>=2.0.0,<3.0.0)
+Requires-Dist: impacket (>=0.10.0,<0.11.0)
+Requires-Dist: scapy (>=2.5.0,<3.0.0)
+Project-URL: Documentation, https://github.com/almandin/krbjack/README.md
+Project-URL: Repository, https://github.com/almandin/krbjack
+Description-Content-Type: text/markdown
+
 # KRBJack
 
 This tool can be used to abuse the dangerous `ZONE_UPDATE_UNSECURE` flag on DNS main domain zone in an Active Directory. This flag when set allows anyone unauthenticated to update, add and remove DNS records anonymously. It is quite common to see it during engagements as it is required to get some DHCP servers working with non-windows based systems, to get them update their own records. Even though this flag is extremely dangerous, I've never seen any tool to ease its exploitation. What I wanted to build is a mean to perform Man-in-the-Middle based on this dangerous flag, grab credentials and use them directly to own systems or the entire active directory services (though multiple tools can be used together to perform ntlm relay for example).
 
 The benefit from using this technique of man in the middle is that it goes through routers, as the "official" DNS records are poisonned. If proper routing is set (and if no firewall rule prevents it), someone on another broadcast domain can be targeted (unlike ARP poisoning which only works on you broadcast domain).
 
 Moreover I made the choice to perform fully functionnal AP_REQ hijacking to allow compromission of systems using kerberos instead of NetNTLM.
@@ -63,17 +85,10 @@
 Project Zero :
 - https://googleprojectzero.blogspot.com/2021/10/using-kerberos-for-authentication-relay.html
 - https://googleprojectzero.blogspot.com/2021/10/windows-exploitation-tricks-relaying.html
 
 Impacket :
 - https://github.com/fortra/impacket
 
-# Todo
-
-- Find a way to reset kerberos authentications such a way that clients can retry instantly to authenticate when we steal their tickets. I found that windows is quite sensible to failures and tend not to retry authentications when something goes wrong. Maybe answer with an `KRB_AP_ERR_TKT_EXPIRED` could have the expected effect.
-- Make it work against LDAP as it does not require signing by default AND allows for full domain compromise by adding a new domain admin.
-- Implement ntlm relaying altogether maybe ? So that this tool would be self-sufficient in case `ZONE_UPDATE_UNSECURE` is availabe. Multiple modules could be used at the same time, allowing one to run the first module available for an interesting packet.
-- Allow to disable the whitelist mechanism completely as it might be a problem when computer accounts connect first, then a user account is used on that computer. In this configuration (which could happen quite often) there is a risk that only computer accounts owned tickets are tried and not user owned tickets.
-
 # Disclaimer
 
-This tooling is made only for legal penetration testing and not for any other use. I am not responsible for how it is used by anyone or if it is used to penetrate systems without permission or proper contractual agreements. It is provided as is and without warranty of any sort.
+This tooling is made only for legal penetration testing and not for any other use. I am not responsible for how it is used by anyone or if it is used to penetrate systems without permission or proper contractual agreements. It is provided as is and without warranty of any sort.
```

### Comparing `krbjack-1.0.0/PKG-INFO` & `krbjack-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: krbjack
-Version: 1.0.0
-Summary: Kerberos AP-REQ hijacking tool with DNS unsecure updates abuse.
-Home-page: https://github.com/almandin/krbjack
-License: Beerware
-Author: Virgile Jarry
-Author-email: virgile@mailbox.org
-Requires-Python: >=3.9,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: colorama (>=0.4.4,<0.5.0)
-Requires-Dist: dnspython (>=2.0.0,<3.0.0)
-Requires-Dist: impacket (>=0.10.0,<0.11.0)
-Requires-Dist: scapy (>=2.5.0,<3.0.0)
-Project-URL: Documentation, https://github.com/almandin/krbjack/README.md
-Project-URL: Repository, https://github.com/almandin/krbjack
-Description-Content-Type: text/markdown
-
 # KRBJack
 
 This tool can be used to abuse the dangerous `ZONE_UPDATE_UNSECURE` flag on DNS main domain zone in an Active Directory. This flag when set allows anyone unauthenticated to update, add and remove DNS records anonymously. It is quite common to see it during engagements as it is required to get some DHCP servers working with non-windows based systems, to get them update their own records. Even though this flag is extremely dangerous, I've never seen any tool to ease its exploitation. What I wanted to build is a mean to perform Man-in-the-Middle based on this dangerous flag, grab credentials and use them directly to own systems or the entire active directory services (though multiple tools can be used together to perform ntlm relay for example).
 
 The benefit from using this technique of man in the middle is that it goes through routers, as the "official" DNS records are poisonned. If proper routing is set (and if no firewall rule prevents it), someone on another broadcast domain can be targeted (unlike ARP poisoning which only works on you broadcast domain).
 
 Moreover I made the choice to perform fully functionnal AP_REQ hijacking to allow compromission of systems using kerberos instead of NetNTLM.
@@ -85,17 +63,10 @@
 Project Zero :
 - https://googleprojectzero.blogspot.com/2021/10/using-kerberos-for-authentication-relay.html
 - https://googleprojectzero.blogspot.com/2021/10/windows-exploitation-tricks-relaying.html
 
 Impacket :
 - https://github.com/fortra/impacket
 
-# Todo
-
-- Find a way to reset kerberos authentications such a way that clients can retry instantly to authenticate when we steal their tickets. I found that windows is quite sensible to failures and tend not to retry authentications when something goes wrong. Maybe answer with an `KRB_AP_ERR_TKT_EXPIRED` could have the expected effect.
-- Make it work against LDAP as it does not require signing by default AND allows for full domain compromise by adding a new domain admin.
-- Implement ntlm relaying altogether maybe ? So that this tool would be self-sufficient in case `ZONE_UPDATE_UNSECURE` is availabe. Multiple modules could be used at the same time, allowing one to run the first module available for an interesting packet.
-- Allow to disable the whitelist mechanism completely as it might be a problem when computer accounts connect first, then a user account is used on that computer. In this configuration (which could happen quite often) there is a risk that only computer accounts owned tickets are tried and not user owned tickets.
-
 # Disclaimer
 
-This tooling is made only for legal penetration testing and not for any other use. I am not responsible for how it is used by anyone or if it is used to penetrate systems without permission or proper contractual agreements. It is provided as is and without warranty of any sort.
+This tooling is made only for legal penetration testing and not for any other use. I am not responsible for how it is used by anyone or if it is used to penetrate systems without permission or proper contractual agreements. It is provided as is and without warranty of any sort.
```

