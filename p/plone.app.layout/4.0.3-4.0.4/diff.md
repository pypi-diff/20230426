# Comparing `tmp/plone.app.layout-4.0.3.tar.gz` & `tmp/plone.app.layout-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.layout-4.0.3.tar", last modified: Sat Apr 15 09:04:32 2023, max compression
+gzip compressed data, was "plone.app.layout-4.0.4.tar", last modified: Wed Apr 26 21:57:04 2023, max compression
```

## Comparing `plone.app.layout-4.0.3.tar` & `plone.app.layout-4.0.4.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.489205 plone.app.layout-4.0.3/
--rw-r--r--   0 gil       (1000) gil       (1000)    60894 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/CHANGES.rst
--rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/CONTRIBUTING.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      122 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/MANIFEST.in
--rw-r--r--   0 gil       (1000) gil       (1000)    62562 2023-04-15 09:04:32.489205 plone.app.layout-4.0.3/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)      740 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/README.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.477204 plone.app.layout-4.0.3/docs/
--rw-r--r--   0 gil       (1000) gil       (1000)    15220 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/docs/LICENSE.GPL
--rw-r--r--   0 gil       (1000) gil       (1000)      678 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/docs/LICENSE.txt
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.477204 plone.app.layout-4.0.3/plone/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.478204 plone.app.layout-4.0.3/plone/app/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.478204 plone.app.layout-4.0.3/plone/app/layout/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.479204 plone.app.layout-4.0.3/plone/app/layout/analytics/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      322 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/configure.zcml
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.479204 plone.app.layout-4.0.3/plone/app/layout/analytics/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/tests/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1695 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/tests/analytics.txt
--rw-r--r--   0 gil       (1000) gil       (1000)      637 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/tests/test_doctests.py
--rw-r--r--   0 gil       (1000) gil       (1000)      199 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/view.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1024 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/analytics/view.py
--rw-r--r--   0 gil       (1000) gil       (1000)      550 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/configure.zcml
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.479204 plone.app.layout-4.0.3/plone/app/layout/dashboard/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/dashboard/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      100 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/dashboard/dashboard.py
--rw-r--r--   0 gil       (1000) gil       (1000)      103 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/dashboard/user_actions.py
--rw-r--r--   0 gil       (1000) gil       (1000)      885 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/favicon_handler.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.480204 plone.app.layout-4.0.3/plone/app/layout/globals/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1327 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     9179 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/context.py
--rw-r--r--   0 gil       (1000) gil       (1000)     4098 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/interface.py
--rw-r--r--   0 gil       (1000) gil       (1000)     6502 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/interfaces.py
--rw-r--r--   0 gil       (1000) gil       (1000)    12280 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/layout.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3805 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/portal.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.481204 plone.app.layout-4.0.3/plone/app/layout/globals/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.481204 plone.app.layout-4.0.3/plone/app/layout/globals/tests/data/
--rw-r--r--   0 gil       (1000) gil       (1000)       30 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/data/bodyclass_nametest.pt
--rw-r--r--   0 gil       (1000) gil       (1000)    10563 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_context.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3885 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_interface.py
--rw-r--r--   0 gil       (1000) gil       (1000)     8497 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_layout.py
--rw-r--r--   0 gil       (1000) gil       (1000)     6321 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_portal.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1375 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_tools.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1060 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/globals/tools.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.481204 plone.app.layout-4.0.3/plone/app/layout/icons/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/icons/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1553 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/icons/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     5639 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/icons/icons.py
--rw-r--r--   0 gil       (1000) gil       (1000)      759 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/icons/interfaces.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.482205 plone.app.layout-4.0.3/plone/app/layout/links/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      523 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/author.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1166 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)      284 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/favicon.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      249 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/rsslink.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      363 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/search.pt
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.482205 plone.app.layout-4.0.3/plone/app/layout/links/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)        2 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/tests/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      803 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/tests/test_canonical_url.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2707 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/tests/test_favicon_viewlet.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1402 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/tests/test_rssviewlet.py
--rw-r--r--   0 gil       (1000) gil       (1000)     7019 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/links/viewlets.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.483204 plone.app.layout-4.0.3/plone/app/layout/navigation/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      244 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     1749 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/interfaces.py
--rw-r--r--   0 gil       (1000) gil       (1000)    14357 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/navtree.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2186 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/root.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.483204 plone.app.layout-4.0.3/plone/app/layout/navigation/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/tests/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      524 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/navigation/tests/test_root.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.484204 plone.app.layout-4.0.3/plone/app/layout/nextprevious/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/nextprevious/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      989 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/nextprevious/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)      856 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/nextprevious/interfaces.py
--rw-r--r--   0 gil       (1000) gil       (1000)      909 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/nextprevious/links.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1673 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/nextprevious/nextprevious.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1611 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/nextprevious/view.py
--rw-r--r--   0 gil       (1000) gil       (1000)      323 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/permissions.zcml
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.484204 plone.app.layout-4.0.3/plone/app/layout/sitemap/
--rw-r--r--   0 gil       (1000) gil       (1000)      159 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/README.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      301 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     4491 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/sitemap.py
--rw-r--r--   0 gil       (1000) gil       (1000)      820 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/sitemap.xml
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.484204 plone.app.layout-4.0.3/plone/app/layout/sitemap/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)        2 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/tests/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)    11362 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/sitemap/tests/test_sitemap.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1184 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/testing.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.488205 plone.app.layout-4.0.3/plone/app/layout/viewlets/
--rw-r--r--   0 gil       (1000) gil       (1000)       40 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      409 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/anontools.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      445 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/colophon.pt
--rw-r--r--   0 gil       (1000) gil       (1000)    20134 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/common.py
--rw-r--r--   0 gil       (1000) gil       (1000)    10010 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)    18971 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/content.py
--rw-r--r--   0 gil       (1000) gil       (1000)     6137 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/content_history.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      782 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/contentviews.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1239 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/document_actions.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1978 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/document_byline.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      980 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/document_contributors.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1833 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/document_relateditems.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      375 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/document_rights.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      139 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/dublin_core.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      793 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/globalstatusmessage.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1579 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/globalstatusmessage.py
--rw-r--r--   0 gil       (1000) gil       (1000)      620 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/history_view.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      953 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/httpheaders.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2331 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/interfaces.py
--rw-r--r--   0 gil       (1000) gil       (1000)      920 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/keywords.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      361 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/logo.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1318 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/membertools.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1816 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/menu.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      811 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/path_bar.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      515 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/popup_content_history.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     3320 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/review_history.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1621 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/searchbox.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      661 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/sections.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      552 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/site_actions.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     5451 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/social.py
--rw-r--r--   0 gil       (1000) gil       (1000)       80 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/social_tags.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      294 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/social_tags_body.pt
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.489205 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      665 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/base.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2621 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/history.txt
--rw-r--r--   0 gil       (1000) gil       (1000)    27962 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_common.py
--rw-r--r--   0 gil       (1000) gil       (1000)    14111 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_content.py
--rw-r--r--   0 gil       (1000) gil       (1000)      590 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_functional.py
--rw-r--r--   0 gil       (1000) gil       (1000)     5391 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_history.py
--rw-r--r--   0 gil       (1000) gil       (1000)     5586 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_social.py
--rw-r--r--   0 gil       (1000) gil       (1000)      192 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/tiny_logo.pt
--rw-r--r--   0 gil       (1000) gil       (1000)       66 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/title.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      382 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/toc.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     2484 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/toolbar.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1779 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/toolbar.py
--rw-r--r--   0 gil       (1000) gil       (1000)       79 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone/app/layout/viewlets/viewport.pt
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 09:04:32.478204 plone.app.layout-4.0.3/plone.app.layout.egg-info/
--rw-r--r--   0 gil       (1000) gil       (1000)    62562 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     4974 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/SOURCES.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/dependency_links.txt
--rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/namespace_packages.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/not-zip-safe
--rw-r--r--   0 gil       (1000) gil       (1000)      486 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/requires.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/plone.app.layout.egg-info/top_level.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     1690 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/pyproject.toml
--rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 09:04:32.490204 plone.app.layout-4.0.3/setup.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)     2193 2023-04-15 09:04:32.000000 plone.app.layout-4.0.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.713079 plone.app.layout-4.0.4/
+-rw-r--r--   0 maurits    (501) staff       (20)    61299 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    62967 2023-04-26 21:57:04.713230 plone.app.layout-4.0.4/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      740 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.678431 plone.app.layout-4.0.4/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      678 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.678704 plone.app.layout-4.0.4/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.681021 plone.app.layout-4.0.4/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.682376 plone.app.layout-4.0.4/plone/app/layout/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.683377 plone.app.layout-4.0.4/plone/app/layout/analytics/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/analytics/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      322 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/analytics/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.684091 plone.app.layout-4.0.4/plone/app/layout/analytics/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/analytics/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1695 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/analytics/tests/analytics.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      637 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/analytics/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)      199 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/analytics/view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1024 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/analytics/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)      550 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.684804 plone.app.layout-4.0.4/plone/app/layout/dashboard/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/dashboard/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      100 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/dashboard/dashboard.py
+-rw-r--r--   0 maurits    (501) staff       (20)      103 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/dashboard/user_actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      885 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/favicon_handler.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.686924 plone.app.layout-4.0.4/plone/app/layout/globals/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1327 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9179 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/context.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4098 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/interface.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6502 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12280 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3805 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/portal.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.688547 plone.app.layout-4.0.4/plone/app/layout/globals/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.688863 plone.app.layout-4.0.4/plone/app/layout/globals/tests/data/
+-rw-r--r--   0 maurits    (501) staff       (20)       30 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/tests/data/bodyclass_nametest.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10563 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/tests/test_context.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3885 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/tests/test_interface.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8497 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/tests/test_layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6321 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/tests/test_portal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1375 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/tests/test_tools.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/globals/tools.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.690063 plone.app.layout-4.0.4/plone/app/layout/icons/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/icons/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1553 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/icons/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5639 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/icons/icons.py
+-rw-r--r--   0 maurits    (501) staff       (20)      759 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/icons/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.691891 plone.app.layout-4.0.4/plone/app/layout/links/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/links/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      523 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/links/author.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1166 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/links/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      284 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/links/favicon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/links/rsslink.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      363 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/links/search.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.693034 plone.app.layout-4.0.4/plone/app/layout/links/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/links/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      803 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/links/tests/test_canonical_url.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2707 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/links/tests/test_favicon_viewlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1402 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/links/tests/test_rssviewlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7019 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/links/viewlets.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.694308 plone.app.layout-4.0.4/plone/app/layout/navigation/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/navigation/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/navigation/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1749 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/navigation/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14357 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/navigation/navtree.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2186 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/navigation/root.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.694820 plone.app.layout-4.0.4/plone/app/layout/navigation/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/navigation/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      524 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/navigation/tests/test_root.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.696500 plone.app.layout-4.0.4/plone/app/layout/nextprevious/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/nextprevious/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      989 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/nextprevious/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      856 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/nextprevious/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      909 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/nextprevious/links.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1673 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/nextprevious/nextprevious.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1611 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/nextprevious/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)      323 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.697919 plone.app.layout-4.0.4/plone/app/layout/sitemap/
+-rw-r--r--   0 maurits    (501) staff       (20)      159 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/sitemap/README.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/sitemap/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      301 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/sitemap/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4491 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/sitemap/sitemap.py
+-rw-r--r--   0 maurits    (501) staff       (20)      820 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/sitemap/sitemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.698501 plone.app.layout-4.0.4/plone/app/layout/sitemap/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/sitemap/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11362 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/sitemap/tests/test_sitemap.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1184 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.710322 plone.app.layout-4.0.4/plone/app/layout/viewlets/
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      409 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/anontools.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      445 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/colophon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    20134 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/common.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10010 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    18430 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6137 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/content_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      782 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/contentviews.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1239 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/document_actions.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1978 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/document_byline.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      980 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/document_contributors.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1833 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/document_relateditems.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      375 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/document_rights.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      139 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/dublin_core.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      793 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/globalstatusmessage.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1579 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/globalstatusmessage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      620 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/history_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      953 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/httpheaders.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2331 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      920 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/keywords.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      361 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/logo.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1318 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/membertools.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1816 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/menu.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      811 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/path_bar.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      515 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/popup_content_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3320 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/review_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1621 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/searchbox.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      661 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/sections.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      552 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/site_actions.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5451 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/social.py
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/social_tags.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      294 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/social_tags_body.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.712853 plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      665 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2621 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/history.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    27962 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/test_common.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14111 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/test_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)      590 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/test_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5391 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/test_history.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5586 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/test_social.py
+-rw-r--r--   0 maurits    (501) staff       (20)      192 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/tiny_logo.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       66 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/title.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      382 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/toc.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2484 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/toolbar.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1779 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/toolbar.py
+-rw-r--r--   0 maurits    (501) staff       (20)       79 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/plone/app/layout/viewlets/viewport.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:57:04.680778 plone.app.layout-4.0.4/plone.app.layout.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    62967 2023-04-26 21:57:04.000000 plone.app.layout-4.0.4/plone.app.layout.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4974 2023-04-26 21:57:04.000000 plone.app.layout-4.0.4/plone.app.layout.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:57:04.000000 plone.app.layout-4.0.4/plone.app.layout.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-26 21:57:04.000000 plone.app.layout-4.0.4/plone.app.layout.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:57:04.000000 plone.app.layout-4.0.4/plone.app.layout.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      463 2023-04-26 21:57:04.000000 plone.app.layout-4.0.4/plone.app.layout.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:57:04.000000 plone.app.layout-4.0.4/plone.app.layout.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1690 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-26 21:57:04.713782 plone.app.layout-4.0.4/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2159 2023-04-26 21:57:03.000000 plone.app.layout-4.0.4/setup.py
```

### Comparing `plone.app.layout-4.0.3/CHANGES.rst` & `plone.app.layout-4.0.4/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,28 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.4 (2023-04-26)
+------------------
+
+Bug fixes:
+
+
+- Remove dead code for Archetypes relations lookup.
+  [@jensens] (rm-archetypes-code)
+- Add another unused `get_translations` method to deprecated ones.
+  Circula dependency on plone.app.multilingual is only for unused deprecated methods.
+  Move it's imports into methods-body and remove dependency from setup.py.
+  [@jensens] (rm-dep-pamultilingual)
+
+
 4.0.3 (2023-04-15)
 ------------------
 
 Bug fixes:
 
 
 - Remove Archetypes code from TOC viewlet.
```

### Comparing `plone.app.layout-4.0.3/PKG-INFO` & `plone.app.layout-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.layout
-Version: 4.0.3
+Version: 4.0.4
 Summary: Layout mechanisms for Plone
 Home-page: https://pypi.org/project/plone.app.layout
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone layout viewlet
 Classifier: Development Status :: 6 - Mature
@@ -49,14 +49,28 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.4 (2023-04-26)
+------------------
+
+Bug fixes:
+
+
+- Remove dead code for Archetypes relations lookup.
+  [@jensens] (rm-archetypes-code)
+- Add another unused `get_translations` method to deprecated ones.
+  Circula dependency on plone.app.multilingual is only for unused deprecated methods.
+  Move it's imports into methods-body and remove dependency from setup.py.
+  [@jensens] (rm-dep-pamultilingual)
+
+
 4.0.3 (2023-04-15)
 ------------------
 
 Bug fixes:
 
 
 - Remove Archetypes code from TOC viewlet.
```

### Comparing `plone.app.layout-4.0.3/README.rst` & `plone.app.layout-4.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/docs/LICENSE.GPL` & `plone.app.layout-4.0.4/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/docs/LICENSE.txt` & `plone.app.layout-4.0.4/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/analytics/tests/analytics.txt` & `plone.app.layout-4.0.4/plone/app/layout/analytics/tests/analytics.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/analytics/tests/test_doctests.py` & `plone.app.layout-4.0.4/plone/app/layout/analytics/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/analytics/view.py` & `plone.app.layout-4.0.4/plone/app/layout/analytics/view.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/configure.zcml` & `plone.app.layout-4.0.4/plone/app/layout/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/favicon_handler.py` & `plone.app.layout-4.0.4/plone/app/layout/favicon_handler.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/globals/configure.zcml` & `plone.app.layout-4.0.4/plone/app/layout/globals/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/globals/context.py` & `plone.app.layout-4.0.4/plone/app/layout/globals/context.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/globals/interface.py` & `plone.app.layout-4.0.4/plone/app/layout/globals/interface.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/globals/interfaces.py` & `plone.app.layout-4.0.4/plone/app/layout/globals/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/globals/layout.py` & `plone.app.layout-4.0.4/plone/app/layout/globals/layout.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/globals/portal.py` & `plone.app.layout-4.0.4/plone/app/layout/globals/portal.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_context.py` & `plone.app.layout-4.0.4/plone/app/layout/globals/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_interface.py` & `plone.app.layout-4.0.4/plone/app/layout/globals/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_layout.py` & `plone.app.layout-4.0.4/plone/app/layout/globals/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_portal.py` & `plone.app.layout-4.0.4/plone/app/layout/globals/tests/test_portal.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/globals/tests/test_tools.py` & `plone.app.layout-4.0.4/plone/app/layout/globals/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/globals/tools.py` & `plone.app.layout-4.0.4/plone/app/layout/globals/tools.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/icons/configure.zcml` & `plone.app.layout-4.0.4/plone/app/layout/icons/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/icons/icons.py` & `plone.app.layout-4.0.4/plone/app/layout/icons/icons.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/icons/interfaces.py` & `plone.app.layout-4.0.4/plone/app/layout/icons/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/links/author.pt` & `plone.app.layout-4.0.4/plone/app/layout/links/author.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/links/configure.zcml` & `plone.app.layout-4.0.4/plone/app/layout/links/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/links/tests/test_canonical_url.py` & `plone.app.layout-4.0.4/plone/app/layout/links/tests/test_canonical_url.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/links/tests/test_favicon_viewlet.py` & `plone.app.layout-4.0.4/plone/app/layout/links/tests/test_favicon_viewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/links/tests/test_rssviewlet.py` & `plone.app.layout-4.0.4/plone/app/layout/links/tests/test_rssviewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/links/viewlets.py` & `plone.app.layout-4.0.4/plone/app/layout/links/viewlets.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/navigation/interfaces.py` & `plone.app.layout-4.0.4/plone/app/layout/navigation/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/navigation/navtree.py` & `plone.app.layout-4.0.4/plone/app/layout/navigation/navtree.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/navigation/root.py` & `plone.app.layout-4.0.4/plone/app/layout/navigation/root.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/navigation/tests/test_root.py` & `plone.app.layout-4.0.4/plone/app/layout/navigation/tests/test_root.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/nextprevious/configure.zcml` & `plone.app.layout-4.0.4/plone/app/layout/nextprevious/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/nextprevious/interfaces.py` & `plone.app.layout-4.0.4/plone/app/layout/nextprevious/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/nextprevious/links.pt` & `plone.app.layout-4.0.4/plone/app/layout/nextprevious/links.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/nextprevious/nextprevious.pt` & `plone.app.layout-4.0.4/plone/app/layout/nextprevious/nextprevious.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/nextprevious/view.py` & `plone.app.layout-4.0.4/plone/app/layout/nextprevious/view.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/sitemap/sitemap.py` & `plone.app.layout-4.0.4/plone/app/layout/sitemap/sitemap.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/sitemap/sitemap.xml` & `plone.app.layout-4.0.4/plone/app/layout/sitemap/sitemap.xml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/sitemap/tests/test_sitemap.py` & `plone.app.layout-4.0.4/plone/app/layout/sitemap/tests/test_sitemap.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/testing.py` & `plone.app.layout-4.0.4/plone/app/layout/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/common.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/common.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/configure.zcml` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/content.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/content.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from AccessControl import getSecurityManager
 from Acquisition import aq_inner
 from DateTime import DateTime
 from plone.app.content.browser.interfaces import IFolderContentsView
 from plone.app.layout.globals.interfaces import IViewView
 from plone.app.layout.viewlets import ViewletBase
-from plone.app.multilingual.browser.vocabularies import translated_languages
-from plone.app.multilingual.interfaces import ITranslatable
-from plone.app.multilingual.interfaces import ITranslationManager
+from plone.app.relationfield.behavior import IRelatedItems
 from plone.base import PloneMessageFactory as _
 from plone.base.interfaces import ISecuritySchema
 from plone.base.interfaces import ISiteSchema
 from plone.base.utils import base_hasattr
 from plone.base.utils import logger
 from plone.memoize.instance import memoize
 from plone.memoize.view import memoize_contextless
@@ -24,29 +22,14 @@
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from urllib.parse import urlencode
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.component import queryMultiAdapter
 from zope.deprecation import deprecation
 
-import pkg_resources
-
-
-try:
-    pkg_resources.get_distribution("plone.app.relationfield")
-except pkg_resources.DistributionNotFound:
-    HAS_RELATIONFIELD = False
-else:
-    from plone.app.relationfield.behavior import IRelatedItems
-
-    HAS_RELATIONFIELD = True
-
-# XXX needs refactoring, since Plone 5 we have PAM in core.
-HAS_PAM = True
-
 
 class DocumentActionsViewlet(ViewletBase):
     index = ViewPageTemplateFile("document_actions.pt")
 
     def update(self):
         super().update()
 
@@ -71,15 +54,15 @@
         return getMultiAdapter((self.context, self.request), name="plone_context_state")
 
     @property
     @deprecation.deprecate(
         "The has_pam property is unused and will be removed in Plone 7"
     )
     def has_pam(self):
-        return HAS_PAM
+        return True
 
     @property
     @memoize_contextless
     def portal_membership(self):
         return getToolByName(self.context, "portal_membership")
 
     def show(self):
@@ -174,14 +157,18 @@
 
         return DateTime(date)
 
     @deprecation.deprecate(
         "The get_translations method is unused and will be removed in Plone 7"
     )
     def get_translations(self):
+        from plone.app.multilingual.browser.vocabularies import translated_languages
+        from plone.app.multilingual.interfaces import ITranslatable
+        from plone.app.multilingual.interfaces import ITranslationManager
+
         cts = []
         if ITranslatable.providedBy(self.context):
             t_langs = translated_languages(self.context)
             context_translations = ITranslationManager(self.context).get_translations()
             for lang in t_langs:
                 cts.append(
                     dict(
@@ -202,21 +189,27 @@
         self.portal_state = getMultiAdapter(
             (context, self.request), name="plone_portal_state"
         )
         self.context_state = getMultiAdapter(
             (self.context, self.request), name="plone_context_state"
         )
         self.anonymous = self.portal_state.anonymous()
-        self.has_pam = HAS_PAM
 
     def __call__(self):
         self.update()
 
         return self.index()
 
+    @property
+    @deprecation.deprecate(
+        "The has_pam property is unused and will be removed in Plone 7"
+    )
+    def has_pam(self):
+        return True
+
     def show(self):
         registry = getUtility(IRegistry)
         settings = registry.forInterface(
             ISecuritySchema,
             prefix="plone",
         )
         return not self.anonymous or settings.allow_anon_views_about
@@ -296,15 +289,22 @@
         # check if we have Effective Date set
         date = self.context.EffectiveDate()
         if not date or date == "None":
             return None
 
         return DateTime(date)
 
+    @deprecation.deprecate(
+        "The get_translations method is unused and will be removed in Plone 7"
+    )
     def get_translations(self):
+        from plone.app.multilingual.browser.vocabularies import translated_languages
+        from plone.app.multilingual.interfaces import ITranslatable
+        from plone.app.multilingual.interfaces import ITranslationManager
+
         cts = []
         if ITranslatable.providedBy(self.context):
             t_langs = translated_languages(self.context)
             context_translations = ITranslationManager(self.context).get_translations()
             for lang in t_langs:
                 cts.append(
                     dict(
@@ -316,43 +316,20 @@
         return cts
 
 
 class ContentRelatedItems(ViewletBase):
     index = ViewPageTemplateFile("document_relateditems.pt")
 
     def related_items(self):
-        context = aq_inner(self.context)
-        res = ()
-
-        # Archetypes
-        if base_hasattr(context, "getRawRelatedItems"):
-            catalog = getToolByName(context, "portal_catalog")
-            related = context.getRawRelatedItems()
-            if not related:
-                return ()
-            brains = catalog(UID=related)
-            if brains:
-                # build a position dict by iterating over the items once
-                positions = {v: i for (i, v) in enumerate(related)}
-                # We need to keep the ordering intact
-                res = list(brains)
-
-                def _key(brain):
-                    return positions.get(brain.UID, -1)
-
-                res.sort(key=_key)
-
-        # Dexterity
-        if HAS_RELATIONFIELD and IRelatedItems.providedBy(context):
-            related = context.relatedItems
-            if not related:
-                return ()
-            res = self.related2brains(related)
-
-        return res
+        if not IRelatedItems.providedBy(self.context):
+            return ()
+        related = aq_inner(self.context).relatedItems
+        if not related:
+            return ()
+        return self.related2brains(related)
 
     def related2brains(self, related):
         """Return a list of brains based on a list of relations. Will filter
         relations if the user has no permission to access the content.
 
         :param related: related items
         :type related: list of relations
```

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/content_history.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/content_history.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/contentviews.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/contentviews.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/document_actions.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/document_actions.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/document_byline.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/document_byline.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/document_contributors.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/document_contributors.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/document_relateditems.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/document_relateditems.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/globalstatusmessage.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/globalstatusmessage.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/globalstatusmessage.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/globalstatusmessage.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/history_view.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/history_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/httpheaders.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/httpheaders.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/interfaces.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/keywords.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/keywords.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/membertools.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/membertools.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/menu.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/menu.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/path_bar.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/path_bar.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/popup_content_history.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/popup_content_history.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/review_history.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/review_history.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/searchbox.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/searchbox.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/sections.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/sections.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/site_actions.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/site_actions.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/social.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/social.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/base.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/history.txt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/history.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_common.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_content.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_functional.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_history.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/tests/test_social.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/tests/test_social.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/toolbar.pt` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/toolbar.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone/app/layout/viewlets/toolbar.py` & `plone.app.layout-4.0.4/plone/app/layout/viewlets/toolbar.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/plone.app.layout.egg-info/PKG-INFO` & `plone.app.layout-4.0.4/plone.app.layout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.layout
-Version: 4.0.3
+Version: 4.0.4
 Summary: Layout mechanisms for Plone
 Home-page: https://pypi.org/project/plone.app.layout
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone layout viewlet
 Classifier: Development Status :: 6 - Mature
@@ -49,14 +49,28 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.4 (2023-04-26)
+------------------
+
+Bug fixes:
+
+
+- Remove dead code for Archetypes relations lookup.
+  [@jensens] (rm-archetypes-code)
+- Add another unused `get_translations` method to deprecated ones.
+  Circula dependency on plone.app.multilingual is only for unused deprecated methods.
+  Move it's imports into methods-body and remove dependency from setup.py.
+  [@jensens] (rm-dep-pamultilingual)
+
+
 4.0.3 (2023-04-15)
 ------------------
 
 Bug fixes:
 
 
 - Remove Archetypes code from TOC viewlet.
```

### Comparing `plone.app.layout-4.0.3/plone.app.layout.egg-info/SOURCES.txt` & `plone.app.layout-4.0.4/plone.app.layout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/pyproject.toml` & `plone.app.layout-4.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.3/setup.py` & `plone.app.layout-4.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.3"
+version = "4.0.4"
 
 long_description = open("README.rst").read() + "\n" + open("CHANGES.rst").read()
 
 setup(
     name="plone.app.layout",
     version=version,
     description="Layout mechanisms for Plone",
@@ -35,15 +35,14 @@
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
         "BTrees",
         "plone.app.content",
-        "plone.app.multilingual",
         "plone.app.relationfield",
         "plone.app.uuid",
         "plone.app.viewletmanager >=1.2",
         "plone.base >=1.0.4",
         "plone.dexterity",
         "plone.formwidget.namedfile",
         "plone.i18n",
```

