# Comparing `tmp/SimpleIDML-1.1.6a1.tar.gz` & `tmp/SimpleIDML-1.1.6a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SimpleIDML-1.1.6a1.tar", last modified: Mon Apr 17 14:18:51 2023, max compression
+gzip compressed data, was "dist/SimpleIDML-1.1.6a2.tar", last modified: Wed Apr 26 13:43:22 2023, max compression
```

## Comparing `SimpleIDML-1.1.6a1.tar` & `SimpleIDML-1.1.6a2.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    29332 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1424 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/LICENSE
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       36 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/AUTHORS
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      278 2022-03-14 13:09:46.000000 SimpleIDML-1.1.6a1/tests/Makefile
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       62 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/coveragerc
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2067 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/extras.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6984 2020-12-04 14:34:01.000000 SimpleIDML-1.1.6a1/tests/regressiontests/indesign.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/__init__.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/SOAP/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7916 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/SOAP/indesign-service.xml
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1259 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1007 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-without-picture.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1071 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-false.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1279 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes2.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1041 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1073 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-ignorecontent.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1104 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-forcecontent2.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1105 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-forcecontent3.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1074 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-nested-tags.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      947 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete-informations.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1104 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-forcecontent.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1041 2020-06-30 07:14:18.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-remove-br.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1030 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     9296 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/utils.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7138 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/id_package.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   219693 2020-06-30 07:14:18.000000 SimpleIDML-1.1.6a1/tests/regressiontests/idml.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    25869 2020-05-27 07:40:19.000000 SimpleIDML-1.1.6a1/tests/regressiontests/components.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    36272 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-xml.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   335872 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-xml.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    45235 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   675840 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)  1303348 2020-11-24 09:03:39.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/package-pirate.zip
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    46702 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   466944 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   860160 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    37291 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages.idml
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206617 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   282004 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-elts-same-layer.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   207343 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-nested-tags.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   205726 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-ignorecontent.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   204178 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-without-picture.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   205708 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent3.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206957 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent2.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   278792 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   271361 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-0-photo-complex.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   208277 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2-prefixed.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206817 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   278787 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-complex.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   208159 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-setcontent-false.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206617 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   205722 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    41657 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/page-9modules.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   585728 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)  1015808 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/page-9modules.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    47823 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   335872 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-nested-xml.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    35520 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo-with-attributes.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   389120 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo-with-attributes.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    36554 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-nested-xml.idml
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7221 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Graphic.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    35821 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Styles.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    15342 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Fonts.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    73611 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Preferences.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    16154 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/designmap.xml
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/META-INF/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      253 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/META-INF/container.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    25538 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/META-INF/metadata.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       43 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/mimetype
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      732 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/BackingStory.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      274 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/Mapping.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1302 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/Tags.xml
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1315 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u1db.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2320 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u19f.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      940 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u188.xml
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Spreads/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    19082 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Spreads/Spread_ud6.xml
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/MasterSpreads/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2608 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/MasterSpreads/MasterSpread_ua5.xml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   360448 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages-layers-with-guides.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   575266 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo-package.zip
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40775 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages-layers-with-guides.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   864256 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)  1966080 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-bloc-notes.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    45371 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    49511 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-bloc-notes.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   140777 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/module1.pdf
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   372736 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_import-xml.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    30910 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-template.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40093 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_import-xml.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   569344 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   364544 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-0photo.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40088 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-0photo.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40175 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo.idml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   655360 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-edito.indd
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    42578 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-edito.idml
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    37435 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/Jacques-Yves_Cousteau.jpg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   103166 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/bouboune.jpg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)   190741 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/default2.jpg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    27644 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/default.jpg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1632 2022-03-14 13:09:46.000000 SimpleIDML-1.1.6a1/tests/runtests.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      198 2022-03-14 13:09:46.000000 SimpleIDML-1.1.6a1/MANIFEST.in
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1785 2023-04-17 14:17:50.000000 SimpleIDML-1.1.6a1/setup.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       38 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/setup.cfg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    22600 2023-04-17 06:31:13.000000 SimpleIDML-1.1.6a1/README.rst
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    29332 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6585 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/SOURCES.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       14 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/requires.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       12 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/top_level.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/dependency_links.txt
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/simple_idml/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      681 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a1/src/simple_idml/extras.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      322 2023-04-17 14:17:50.000000 SimpleIDML-1.1.6a1/src/simple_idml/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4486 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/test.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3436 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/utils.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1795 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/id_package.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    11609 2023-02-20 07:55:47.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/indesign.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/__init__.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      285 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/list_profiles.jsx
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      126 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/close_all_documents.jsx
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      636 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/save_as.jsx
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    12733 2022-01-18 09:35:17.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/export.jsx
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1190 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/package_to_print.jsx
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    50966 2023-04-17 12:02:50.000000 SimpleIDML-1.1.6a1/src/simple_idml/idml.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      247 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a1/src/simple_idml/exceptions.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    37323 2023-04-17 12:05:26.000000 SimpleIDML-1.1.6a1/src/simple_idml/components.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6906 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a1/src/simple_idml/ftp.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2369 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a1/src/simple_idml/commands.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2211 2023-04-17 11:58:25.000000 SimpleIDML-1.1.6a1/src/simple_idml/decorators.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/scripts/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      682 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/scripts/simpleidml_indesign_close_all_documents.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      618 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/scripts/simpleidml_create_package_from_dir.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3653 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a1/src/scripts/simpleidml_indesign_save_as.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    29323 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1424 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/LICENSE
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       36 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/AUTHORS
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      278 2022-03-14 13:09:46.000000 SimpleIDML-1.1.6a2/tests/Makefile
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       62 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/coveragerc
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2067 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/extras.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6984 2020-12-04 14:34:01.000000 SimpleIDML-1.1.6a2/tests/regressiontests/indesign.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/__init__.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/SOAP/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7916 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/SOAP/indesign-service.xml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1259 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1007 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-without-picture.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1071 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-false.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1279 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes2.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1041 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1073 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-ignorecontent.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1104 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-forcecontent2.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1105 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-forcecontent3.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1074 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-nested-tags.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      947 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete-informations.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1104 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-forcecontent.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1041 2020-06-30 07:14:18.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-remove-br.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1030 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     9296 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/utils.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7138 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/id_package.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   219693 2020-06-30 07:14:18.000000 SimpleIDML-1.1.6a2/tests/regressiontests/idml.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    25869 2020-05-27 07:40:19.000000 SimpleIDML-1.1.6a2/tests/regressiontests/components.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    36272 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo_imported-xml.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   335872 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo_imported-xml.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    45235 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   675840 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)  1303348 2020-11-24 09:03:39.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/package-pirate.zip
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    46702 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   466944 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/4-pages.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   860160 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    37291 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/4-pages.idml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206617 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   282004 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-elts-same-layer.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   207343 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-nested-tags.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   205726 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-ignorecontent.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   204178 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-without-picture.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   205708 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent3.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206957 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent2.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   278792 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   271361 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/4-pages-insert-article-0-photo-complex.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   208277 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2-prefixed.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206817 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   278787 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-complex.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   208159 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-setcontent-false.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206617 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   205722 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    41657 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/page-9modules.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   585728 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)  1015808 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/page-9modules.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    47823 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   335872 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo_imported-nested-xml.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    35520 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo-with-attributes.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   389120 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo-with-attributes.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    36554 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo_imported-nested-xml.idml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Resources/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7221 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Resources/Graphic.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    35821 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Resources/Styles.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    15342 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Resources/Fonts.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    73611 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Resources/Preferences.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    16154 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/designmap.xml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/META-INF/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      253 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/META-INF/container.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    25538 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/META-INF/metadata.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       43 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/mimetype
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/XML/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      732 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/XML/BackingStory.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      274 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/XML/Mapping.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1302 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/XML/Tags.xml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Stories/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1315 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Stories/Story_u1db.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2320 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Stories/Story_u19f.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      940 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Stories/Story_u188.xml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Spreads/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    19082 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Spreads/Spread_ud6.xml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/MasterSpreads/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2608 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/MasterSpreads/MasterSpread_ua5.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   360448 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/4-pages-layers-with-guides.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   575266 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo-package.zip
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40775 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/4-pages-layers-with-guides.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   864256 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/2articles-1photo.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)  1966080 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-bloc-notes.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    45371 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/2articles-1photo.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    49511 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-bloc-notes.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   140777 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/module1.pdf
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   372736 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo_import-xml.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    30910 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-template.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40093 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo_import-xml.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   569344 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   364544 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/2articles-0photo.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40088 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/2articles-0photo.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40175 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   655360 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-edito.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    42578 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-edito.idml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/media/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    37435 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/media/Jacques-Yves_Cousteau.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   103166 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/media/bouboune.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   190741 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/media/default2.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    27644 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/tests/regressiontests/IDML/media/default.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1632 2022-03-14 13:09:46.000000 SimpleIDML-1.1.6a2/tests/runtests.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      198 2022-03-14 13:09:46.000000 SimpleIDML-1.1.6a2/MANIFEST.in
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1785 2023-04-26 13:41:13.000000 SimpleIDML-1.1.6a2/setup.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       38 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/setup.cfg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    22591 2023-04-26 13:41:01.000000 SimpleIDML-1.1.6a2/README.rst
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:22.000000 SimpleIDML-1.1.6a2/src/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:22.000000 SimpleIDML-1.1.6a2/src/SimpleIDML.egg-info/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    29323 2023-04-26 13:43:22.000000 SimpleIDML-1.1.6a2/src/SimpleIDML.egg-info/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6585 2023-04-26 13:43:22.000000 SimpleIDML-1.1.6a2/src/SimpleIDML.egg-info/SOURCES.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       14 2023-04-26 13:43:22.000000 SimpleIDML-1.1.6a2/src/SimpleIDML.egg-info/requires.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       12 2023-04-26 13:43:22.000000 SimpleIDML-1.1.6a2/src/SimpleIDML.egg-info/top_level.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2023-04-26 13:43:22.000000 SimpleIDML-1.1.6a2/src/SimpleIDML.egg-info/dependency_links.txt
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:22.000000 SimpleIDML-1.1.6a2/src/simple_idml/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      681 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a2/src/simple_idml/extras.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      322 2023-04-26 13:41:31.000000 SimpleIDML-1.1.6a2/src/simple_idml/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4486 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/src/simple_idml/test.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3436 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/src/simple_idml/utils.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1795 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/src/simple_idml/id_package.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:22.000000 SimpleIDML-1.1.6a2/src/simple_idml/indesign/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    11609 2023-02-20 07:55:47.000000 SimpleIDML-1.1.6a2/src/simple_idml/indesign/indesign.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/src/simple_idml/indesign/__init__.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:23.000000 SimpleIDML-1.1.6a2/src/simple_idml/indesign/scripts/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      285 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/src/simple_idml/indesign/scripts/list_profiles.jsx
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      126 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/src/simple_idml/indesign/scripts/close_all_documents.jsx
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      636 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/src/simple_idml/indesign/scripts/save_as.jsx
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    12733 2022-01-18 09:35:17.000000 SimpleIDML-1.1.6a2/src/simple_idml/indesign/scripts/export.jsx
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1190 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/src/simple_idml/indesign/scripts/package_to_print.jsx
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    50971 2023-04-26 13:41:01.000000 SimpleIDML-1.1.6a2/src/simple_idml/idml.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      247 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a2/src/simple_idml/exceptions.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    37323 2023-04-26 13:41:01.000000 SimpleIDML-1.1.6a2/src/simple_idml/components.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6906 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a2/src/simple_idml/ftp.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2369 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a2/src/simple_idml/commands.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2211 2023-04-17 11:58:25.000000 SimpleIDML-1.1.6a2/src/simple_idml/decorators.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-26 13:43:22.000000 SimpleIDML-1.1.6a2/src/scripts/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      682 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/src/scripts/simpleidml_indesign_close_all_documents.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      618 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a2/src/scripts/simpleidml_create_package_from_dir.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3653 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a2/src/scripts/simpleidml_indesign_save_as.py
```

### Comparing `SimpleIDML-1.1.6a1/PKG-INFO` & `SimpleIDML-1.1.6a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SimpleIDML
-Version: 1.1.6a1
+Version: 1.1.6a2
 Summary: A library to manipulate Adobe(r) IDML(r) files.
 Home-page: https://github.com/Starou/SimpleIDML
 Author: Stanislas Guerra
 Author-email: stanislas.guerra@gmail.com
 License: BSD Licence
 Project-URL: Source Code, https://github.com/Starou/SimpleIDML
 Project-URL: Issue Tracker, https://github.com/Starou/SimpleIDML/issues
@@ -62,19 +62,19 @@
             vagrant ssh
             cd tests
             python runtests.py
         
         What is SimpleIDML?
         ===================
         
-        SimpleIDML is a Python library to manipulate Adobe® InDesign® IDML file. The main purpose being
+        SimpleIDML is a Python library to manipulate Adobe® InDesign® IDML files. The main purpose being
         the ability to compose IDML files together and produce complex documents from simple pieces and
         to separate the data from the structure.
         
-        The philosophy behind SimpleIDML is to keep separated the content and the structure and to use XML
+        The philosophy behind SimpleIDML is to keep the content and structure separated and to use XML
         files to feed your documents by using the XML Structure in InDesign.
         Keeping this isolation is important to ease the debugging and to keep track of what is going on.
         
         I urge you to take a look in the *regressiontests* directory for real-world examples.
         
         Uses cases - success story(ies)
         ===============================
@@ -101,24 +101,24 @@
         
         Architecture
         ''''''''''''
         
         These applications are web-applications. The communication is done by web-services feeding a task
         queue (RabbitMQ/Celery).
         
-        The performances are quite good. Composing a document require a fraction of a second.
+        The performances are quite good. Composing a document requires a fraction of a second.
         
         What are IDML files?
         ====================
         
         IDML (*InDesign Markup Language*) files are a Zip archives (Adobe calls them packages) storing
         essentially XML files. Adobe made a descent job because those files can completely express the
         content of the native (binary) documents.
-        This is a small revolution in the print world when it comes to automatically process files in both
-        ways from templates and database (Round-trip) without using proprietary server-edition of
+        This is a small revolution in the print world when it comes to automatically processing files both
+        from templates and database (Round-trip) without using the proprietary server-edition of
         Publishing Software.
         
         What does SimpleIDML do?
         ========================
         
         Package exploration
         -------------------
@@ -172,27 +172,27 @@
         document (The one you want to use to populate the content with data from an external XML file
         having the same structure).
         
         
         Build package
         -------------
         
-        There is a convenient script to create a IDML package from a flat directory called
+        There is a convenient script to create an IDML package from a flat directory called
         *simpleidml_create_package_from_dir.py* which should be in your PATH.
         
         
         Compose document
         ----------------
         
         **Important**: You should always use a ``with`` context when using side-effect methods on
         ``IDMLPackage`` instances returning new instances.
         
         
         For example, the following is bad because ``my_doc`` initial instance reference is lost and
-        the associated file cannot be properly closed. This may rise an exception on Windows platform
+        the associated file cannot be properly closed. This may raise an exception on Windows platform
         if you try to ``os.unlink()`` an unclosed file.
         
         .. code-block:: python
         
             from simple_idml import idml
             my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
             my_doc = my_doc.prefix("main")
@@ -205,16 +205,16 @@
             my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
             with my_doc.prefix("main") as f:
                 # some code.
         
         Insert elements
         '''''''''''''''
         
-        Using the XML Structure you can ask SimpleIDML to insert into a document at a XML tag the content
-        of another XML tag from another document. The tag paths are expressed using XPath_ syntax.
+        Using the XML Structure, SimpleIDML can insert the content of an XML tag from one document into an
+        XML tag of another document. The tag paths are expressed using XPath_ syntax.
         Note that you should always make a copy of your idml files before altering them with
         ``shutil.copy2(src, dst)`` for instance and prefix your document before using ``insert_idml()``
         to avoid reference collisions.
         
         .. code-block:: python
         
             >>> from simple_idml import idml
@@ -349,31 +349,31 @@
                     <Story>
                         <article>Lorem ipsum dolor sit amet, ...</article>
                         <informations>Lorem ipsum dolor sit amet,</informations>
                     </Story>
                 </module>
             </Root>
         
-        You can as well import XML file into your InDesign® documents. The following rules applies:
+        You can also import XML files into your InDesign® documents. The following rules applies:
         
         - A node having the attribute ``simpleidml-setcontent="false"`` will not update the content of the
           corresponding element into the idml document (but its children will be updated).
-        - A node having the attribute ``simpleidml-ignorecontent"true"`` will not update the content of the
+        - A node having the attribute ``simpleidml-ignorecontent="true"`` will not update the content of the
           corresponding element into the idml document **and** its children.
         - A node having the attribute ``simpleidml-setcontent="delete"`` will remove the corresponding
           element into the idml document (Story and Spread elements).
         - A node having the attribute ``simpleidml-setcontent="remove-previous-br"`` will remove the new-line
           characters before the element.
         - You can mix several flags using a comma (i.e.: ``simpleidml-setcontent="delete,remove-previous-br"``)
         - In a *ignorecontent* context the content of a child node can be turned on with the
           ``simpleidml-forcecontent="true"`` flag.
-        - Images references are passed by the *href* attribute. An empty value will remove the
+        - Image references are passed by the *href* attribute. An empty value will remove the
           corresponding page items into the document.
-        - Nested tag will be created if they are mapped with a *character-style*.
-        - The style applied to the newly created tag is a combinaison of the parent character-styles and
+        - A nested tag will be created if they are mapped with a *character-style*.
+        - The style applied to the newly created tag is a combination of the parent character-style and
           the mapped one.
         
         Please take a look into the tests for in-depth examples.
         
         Import PDF
         ----------
         
@@ -440,18 +440,18 @@
                                             [{"fmt": "pdf"}, {"fmt": "jpeg"}, {"fmt": "zip"}],
                                             "http://url-to-indesign-server:port",
                                             "/path/to/client/workdir",
                                             "/path/to/indesign-server/workdir")
         
         To convert an InDesign Package, use ``indesign.export_package_as()`` instead.
         
-        If the InDesign Server instance runs on a Windows machine, set the
+        If the InDesign Server instance is running on a Windows machine, set the
         ``indesign_server_path_style`` parameter to ``"windows"``.
         
-        If the client access to the working directory *via* FTP, you must specify that
+        If the client accesses the working directory *via* FTP, you must specify that
         in the ``ftp_params`` parameter:
         
         .. code-block:: python
         
             {
                 'auth': ("ftp://ftp.foo.org", "user_account", "s3cret-pa55word"),
                 'passive': False,
```

### Comparing `SimpleIDML-1.1.6a1/LICENSE` & `SimpleIDML-1.1.6a2/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/extras.py` & `SimpleIDML-1.1.6a2/tests/regressiontests/extras.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/indesign.py` & `SimpleIDML-1.1.6a2/tests/regressiontests/indesign.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/SOAP/indesign-service.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/SOAP/indesign-service.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-without-picture.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-without-picture.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-false.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-false.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes2.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes2.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-ignorecontent.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-ignorecontent.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-forcecontent2.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-forcecontent2.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-forcecontent3.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-forcecontent3.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-nested-tags.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-nested-tags.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete-informations.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete-informations.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-forcecontent.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-forcecontent.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-remove-br.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-remove-br.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/utils.py` & `SimpleIDML-1.1.6a2/tests/regressiontests/utils.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/id_package.py` & `SimpleIDML-1.1.6a2/tests/regressiontests/id_package.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/idml.py` & `SimpleIDML-1.1.6a2/tests/regressiontests/idml.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/components.py` & `SimpleIDML-1.1.6a2/tests/regressiontests/components.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-xml.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo_imported-xml.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-xml.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo_imported-xml.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/package-pirate.zip` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/package-pirate.zip`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/4-pages.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/4-pages.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-elts-same-layer.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-elts-same-layer.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-nested-tags.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-nested-tags.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-ignorecontent.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-ignorecontent.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-without-picture.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-without-picture.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent3.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent3.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent2.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent2.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-0-photo-complex.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/4-pages-insert-article-0-photo-complex.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2-prefixed.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2-prefixed.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-complex.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-complex.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-setcontent-false.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-setcontent-false.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/page-9modules.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/page-9modules.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/page-9modules.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/page-9modules.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-nested-xml.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo_imported-nested-xml.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo-with-attributes.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo-with-attributes.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo-with-attributes.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo-with-attributes.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-nested-xml.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo_imported-nested-xml.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Graphic.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Resources/Graphic.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Styles.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Resources/Styles.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Fonts.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Resources/Fonts.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Preferences.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Resources/Preferences.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/designmap.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/designmap.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/META-INF/metadata.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/META-INF/metadata.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/BackingStory.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/XML/BackingStory.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/Tags.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/XML/Tags.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u1db.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Stories/Story_u1db.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u19f.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Stories/Story_u19f.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u188.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Stories/Story_u188.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Spreads/Spread_ud6.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/Spreads/Spread_ud6.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/MasterSpreads/MasterSpread_ua5.xml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo/MasterSpreads/MasterSpread_ua5.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages-layers-with-guides.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/4-pages-layers-with-guides.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo-package.zip` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo-package.zip`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages-layers-with-guides.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/4-pages-layers-with-guides.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/2articles-1photo.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-bloc-notes.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-bloc-notes.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/2articles-1photo.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-bloc-notes.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-bloc-notes.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/module1.pdf` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/module1.pdf`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_import-xml.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo_import-xml.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-template.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-template.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_import-xml.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo_import-xml.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-0photo.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/2articles-0photo.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-0photo.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/2articles-0photo.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/article-1photo.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-edito.indd` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-edito.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-edito.idml` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/magazineA-edito.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/Jacques-Yves_Cousteau.jpg` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/media/Jacques-Yves_Cousteau.jpg`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/bouboune.jpg` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/media/bouboune.jpg`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/default2.jpg` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/media/default2.jpg`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/default.jpg` & `SimpleIDML-1.1.6a2/tests/regressiontests/IDML/media/default.jpg`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/tests/runtests.py` & `SimpleIDML-1.1.6a2/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/setup.py` & `SimpleIDML-1.1.6a2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = f.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="SimpleIDML",
-    version="1.1.6a1",
+    version="1.1.6a2",
     license='BSD Licence',
     author='Stanislas Guerra',
     author_email='stanislas.guerra@gmail.com',
     description='A library to manipulate Adobe(r) IDML(r) files.',
     long_description=README,
     url='https://github.com/Starou/SimpleIDML',
     project_urls={
```

### Comparing `SimpleIDML-1.1.6a1/README.rst` & `SimpleIDML-1.1.6a2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,19 @@
     vagrant ssh
     cd tests
     python runtests.py
 
 What is SimpleIDML?
 ===================
 
-SimpleIDML is a Python library to manipulate Adobe® InDesign® IDML file. The main purpose being
+SimpleIDML is a Python library to manipulate Adobe® InDesign® IDML files. The main purpose being
 the ability to compose IDML files together and produce complex documents from simple pieces and
 to separate the data from the structure.
 
-The philosophy behind SimpleIDML is to keep separated the content and the structure and to use XML
+The philosophy behind SimpleIDML is to keep the content and structure separated and to use XML
 files to feed your documents by using the XML Structure in InDesign.
 Keeping this isolation is important to ease the debugging and to keep track of what is going on.
 
 I urge you to take a look in the *regressiontests* directory for real-world examples.
 
 Uses cases - success story(ies)
 ===============================
@@ -91,24 +91,24 @@
 
 Architecture
 ''''''''''''
 
 These applications are web-applications. The communication is done by web-services feeding a task
 queue (RabbitMQ/Celery).
 
-The performances are quite good. Composing a document require a fraction of a second.
+The performances are quite good. Composing a document requires a fraction of a second.
 
 What are IDML files?
 ====================
 
 IDML (*InDesign Markup Language*) files are a Zip archives (Adobe calls them packages) storing
 essentially XML files. Adobe made a descent job because those files can completely express the
 content of the native (binary) documents.
-This is a small revolution in the print world when it comes to automatically process files in both
-ways from templates and database (Round-trip) without using proprietary server-edition of
+This is a small revolution in the print world when it comes to automatically processing files both
+from templates and database (Round-trip) without using the proprietary server-edition of
 Publishing Software.
 
 What does SimpleIDML do?
 ========================
 
 Package exploration
 -------------------
@@ -162,27 +162,27 @@
 document (The one you want to use to populate the content with data from an external XML file
 having the same structure).
 
 
 Build package
 -------------
 
-There is a convenient script to create a IDML package from a flat directory called
+There is a convenient script to create an IDML package from a flat directory called
 *simpleidml_create_package_from_dir.py* which should be in your PATH.
 
 
 Compose document
 ----------------
 
 **Important**: You should always use a ``with`` context when using side-effect methods on
 ``IDMLPackage`` instances returning new instances.
 
 
 For example, the following is bad because ``my_doc`` initial instance reference is lost and
-the associated file cannot be properly closed. This may rise an exception on Windows platform
+the associated file cannot be properly closed. This may raise an exception on Windows platform
 if you try to ``os.unlink()`` an unclosed file.
 
 .. code-block:: python
 
     from simple_idml import idml
     my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
     my_doc = my_doc.prefix("main")
@@ -195,16 +195,16 @@
     my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
     with my_doc.prefix("main") as f:
         # some code.
 
 Insert elements
 '''''''''''''''
 
-Using the XML Structure you can ask SimpleIDML to insert into a document at a XML tag the content
-of another XML tag from another document. The tag paths are expressed using XPath_ syntax.
+Using the XML Structure, SimpleIDML can insert the content of an XML tag from one document into an
+XML tag of another document. The tag paths are expressed using XPath_ syntax.
 Note that you should always make a copy of your idml files before altering them with
 ``shutil.copy2(src, dst)`` for instance and prefix your document before using ``insert_idml()``
 to avoid reference collisions.
 
 .. code-block:: python
 
     >>> from simple_idml import idml
@@ -339,31 +339,31 @@
             <Story>
                 <article>Lorem ipsum dolor sit amet, ...</article>
                 <informations>Lorem ipsum dolor sit amet,</informations>
             </Story>
         </module>
     </Root>
 
-You can as well import XML file into your InDesign® documents. The following rules applies:
+You can also import XML files into your InDesign® documents. The following rules applies:
 
 - A node having the attribute ``simpleidml-setcontent="false"`` will not update the content of the
   corresponding element into the idml document (but its children will be updated).
-- A node having the attribute ``simpleidml-ignorecontent"true"`` will not update the content of the
+- A node having the attribute ``simpleidml-ignorecontent="true"`` will not update the content of the
   corresponding element into the idml document **and** its children.
 - A node having the attribute ``simpleidml-setcontent="delete"`` will remove the corresponding
   element into the idml document (Story and Spread elements).
 - A node having the attribute ``simpleidml-setcontent="remove-previous-br"`` will remove the new-line
   characters before the element.
 - You can mix several flags using a comma (i.e.: ``simpleidml-setcontent="delete,remove-previous-br"``)
 - In a *ignorecontent* context the content of a child node can be turned on with the
   ``simpleidml-forcecontent="true"`` flag.
-- Images references are passed by the *href* attribute. An empty value will remove the
+- Image references are passed by the *href* attribute. An empty value will remove the
   corresponding page items into the document.
-- Nested tag will be created if they are mapped with a *character-style*.
-- The style applied to the newly created tag is a combinaison of the parent character-styles and
+- A nested tag will be created if they are mapped with a *character-style*.
+- The style applied to the newly created tag is a combination of the parent character-style and
   the mapped one.
 
 Please take a look into the tests for in-depth examples.
 
 Import PDF
 ----------
 
@@ -430,18 +430,18 @@
                                     [{"fmt": "pdf"}, {"fmt": "jpeg"}, {"fmt": "zip"}],
                                     "http://url-to-indesign-server:port",
                                     "/path/to/client/workdir",
                                     "/path/to/indesign-server/workdir")
 
 To convert an InDesign Package, use ``indesign.export_package_as()`` instead.
 
-If the InDesign Server instance runs on a Windows machine, set the
+If the InDesign Server instance is running on a Windows machine, set the
 ``indesign_server_path_style`` parameter to ``"windows"``.
 
-If the client access to the working directory *via* FTP, you must specify that
+If the client accesses the working directory *via* FTP, you must specify that
 in the ``ftp_params`` parameter:
 
 .. code-block:: python
 
     {
         'auth': ("ftp://ftp.foo.org", "user_account", "s3cret-pa55word"),
         'passive': False,
```

### Comparing `SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/PKG-INFO` & `SimpleIDML-1.1.6a2/src/SimpleIDML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SimpleIDML
-Version: 1.1.6a1
+Version: 1.1.6a2
 Summary: A library to manipulate Adobe(r) IDML(r) files.
 Home-page: https://github.com/Starou/SimpleIDML
 Author: Stanislas Guerra
 Author-email: stanislas.guerra@gmail.com
 License: BSD Licence
 Project-URL: Source Code, https://github.com/Starou/SimpleIDML
 Project-URL: Issue Tracker, https://github.com/Starou/SimpleIDML/issues
@@ -62,19 +62,19 @@
             vagrant ssh
             cd tests
             python runtests.py
         
         What is SimpleIDML?
         ===================
         
-        SimpleIDML is a Python library to manipulate Adobe® InDesign® IDML file. The main purpose being
+        SimpleIDML is a Python library to manipulate Adobe® InDesign® IDML files. The main purpose being
         the ability to compose IDML files together and produce complex documents from simple pieces and
         to separate the data from the structure.
         
-        The philosophy behind SimpleIDML is to keep separated the content and the structure and to use XML
+        The philosophy behind SimpleIDML is to keep the content and structure separated and to use XML
         files to feed your documents by using the XML Structure in InDesign.
         Keeping this isolation is important to ease the debugging and to keep track of what is going on.
         
         I urge you to take a look in the *regressiontests* directory for real-world examples.
         
         Uses cases - success story(ies)
         ===============================
@@ -101,24 +101,24 @@
         
         Architecture
         ''''''''''''
         
         These applications are web-applications. The communication is done by web-services feeding a task
         queue (RabbitMQ/Celery).
         
-        The performances are quite good. Composing a document require a fraction of a second.
+        The performances are quite good. Composing a document requires a fraction of a second.
         
         What are IDML files?
         ====================
         
         IDML (*InDesign Markup Language*) files are a Zip archives (Adobe calls them packages) storing
         essentially XML files. Adobe made a descent job because those files can completely express the
         content of the native (binary) documents.
-        This is a small revolution in the print world when it comes to automatically process files in both
-        ways from templates and database (Round-trip) without using proprietary server-edition of
+        This is a small revolution in the print world when it comes to automatically processing files both
+        from templates and database (Round-trip) without using the proprietary server-edition of
         Publishing Software.
         
         What does SimpleIDML do?
         ========================
         
         Package exploration
         -------------------
@@ -172,27 +172,27 @@
         document (The one you want to use to populate the content with data from an external XML file
         having the same structure).
         
         
         Build package
         -------------
         
-        There is a convenient script to create a IDML package from a flat directory called
+        There is a convenient script to create an IDML package from a flat directory called
         *simpleidml_create_package_from_dir.py* which should be in your PATH.
         
         
         Compose document
         ----------------
         
         **Important**: You should always use a ``with`` context when using side-effect methods on
         ``IDMLPackage`` instances returning new instances.
         
         
         For example, the following is bad because ``my_doc`` initial instance reference is lost and
-        the associated file cannot be properly closed. This may rise an exception on Windows platform
+        the associated file cannot be properly closed. This may raise an exception on Windows platform
         if you try to ``os.unlink()`` an unclosed file.
         
         .. code-block:: python
         
             from simple_idml import idml
             my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
             my_doc = my_doc.prefix("main")
@@ -205,16 +205,16 @@
             my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
             with my_doc.prefix("main") as f:
                 # some code.
         
         Insert elements
         '''''''''''''''
         
-        Using the XML Structure you can ask SimpleIDML to insert into a document at a XML tag the content
-        of another XML tag from another document. The tag paths are expressed using XPath_ syntax.
+        Using the XML Structure, SimpleIDML can insert the content of an XML tag from one document into an
+        XML tag of another document. The tag paths are expressed using XPath_ syntax.
         Note that you should always make a copy of your idml files before altering them with
         ``shutil.copy2(src, dst)`` for instance and prefix your document before using ``insert_idml()``
         to avoid reference collisions.
         
         .. code-block:: python
         
             >>> from simple_idml import idml
@@ -349,31 +349,31 @@
                     <Story>
                         <article>Lorem ipsum dolor sit amet, ...</article>
                         <informations>Lorem ipsum dolor sit amet,</informations>
                     </Story>
                 </module>
             </Root>
         
-        You can as well import XML file into your InDesign® documents. The following rules applies:
+        You can also import XML files into your InDesign® documents. The following rules applies:
         
         - A node having the attribute ``simpleidml-setcontent="false"`` will not update the content of the
           corresponding element into the idml document (but its children will be updated).
-        - A node having the attribute ``simpleidml-ignorecontent"true"`` will not update the content of the
+        - A node having the attribute ``simpleidml-ignorecontent="true"`` will not update the content of the
           corresponding element into the idml document **and** its children.
         - A node having the attribute ``simpleidml-setcontent="delete"`` will remove the corresponding
           element into the idml document (Story and Spread elements).
         - A node having the attribute ``simpleidml-setcontent="remove-previous-br"`` will remove the new-line
           characters before the element.
         - You can mix several flags using a comma (i.e.: ``simpleidml-setcontent="delete,remove-previous-br"``)
         - In a *ignorecontent* context the content of a child node can be turned on with the
           ``simpleidml-forcecontent="true"`` flag.
-        - Images references are passed by the *href* attribute. An empty value will remove the
+        - Image references are passed by the *href* attribute. An empty value will remove the
           corresponding page items into the document.
-        - Nested tag will be created if they are mapped with a *character-style*.
-        - The style applied to the newly created tag is a combinaison of the parent character-styles and
+        - A nested tag will be created if they are mapped with a *character-style*.
+        - The style applied to the newly created tag is a combination of the parent character-style and
           the mapped one.
         
         Please take a look into the tests for in-depth examples.
         
         Import PDF
         ----------
         
@@ -440,18 +440,18 @@
                                             [{"fmt": "pdf"}, {"fmt": "jpeg"}, {"fmt": "zip"}],
                                             "http://url-to-indesign-server:port",
                                             "/path/to/client/workdir",
                                             "/path/to/indesign-server/workdir")
         
         To convert an InDesign Package, use ``indesign.export_package_as()`` instead.
         
-        If the InDesign Server instance runs on a Windows machine, set the
+        If the InDesign Server instance is running on a Windows machine, set the
         ``indesign_server_path_style`` parameter to ``"windows"``.
         
-        If the client access to the working directory *via* FTP, you must specify that
+        If the client accesses the working directory *via* FTP, you must specify that
         in the ``ftp_params`` parameter:
         
         .. code-block:: python
         
             {
                 'auth': ("ftp://ftp.foo.org", "user_account", "s3cret-pa55word"),
                 'passive': False,
```

### Comparing `SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/SOURCES.txt` & `SimpleIDML-1.1.6a2/src/SimpleIDML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/extras.py` & `SimpleIDML-1.1.6a2/src/simple_idml/extras.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/test.py` & `SimpleIDML-1.1.6a2/src/simple_idml/test.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/utils.py` & `SimpleIDML-1.1.6a2/src/simple_idml/utils.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/id_package.py` & `SimpleIDML-1.1.6a2/src/simple_idml/id_package.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/indesign/indesign.py` & `SimpleIDML-1.1.6a2/src/simple_idml/indesign/indesign.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/save_as.jsx` & `SimpleIDML-1.1.6a2/src/simple_idml/indesign/scripts/save_as.jsx`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/export.jsx` & `SimpleIDML-1.1.6a2/src/simple_idml/indesign/scripts/export.jsx`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/package_to_print.jsx` & `SimpleIDML-1.1.6a2/src/simple_idml/indesign/scripts/package_to_print.jsx`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/idml.py` & `SimpleIDML-1.1.6a2/src/simple_idml/idml.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,15 +451,15 @@
                     _move_siblings_content(at, element_id)
 
         _import_node(source_node, at)
         return self
 
     @use_working_copy
     def import_pdf(self, pdf_path, at, crop="CropContentVisibleLayers", page_number=1):
-        self.set_attributes(at, {'href': pdf_path})
+        self.set_attributes(at, {'href': f'{pdf_path}'})
         spread = self.get_spread_object_by_xpath(at)
 
         # spread_elt is a <Rectangle> that will host the <PDF>.
         # The <PDF> element get the id of the <Rectangle>.
         spread_elt = self.get_spread_elem_by_xpath(at)
         element_id = self.get_element_content_id_by_xpath(at)
         spread_elt.set("Self", f"{element_id}-old")
```

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/components.py` & `SimpleIDML-1.1.6a2/src/simple_idml/components.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/ftp.py` & `SimpleIDML-1.1.6a2/src/simple_idml/ftp.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/commands.py` & `SimpleIDML-1.1.6a2/src/simple_idml/commands.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/simple_idml/decorators.py` & `SimpleIDML-1.1.6a2/src/simple_idml/decorators.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/scripts/simpleidml_indesign_close_all_documents.py` & `SimpleIDML-1.1.6a2/src/scripts/simpleidml_indesign_close_all_documents.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/scripts/simpleidml_create_package_from_dir.py` & `SimpleIDML-1.1.6a2/src/scripts/simpleidml_create_package_from_dir.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.6a1/src/scripts/simpleidml_indesign_save_as.py` & `SimpleIDML-1.1.6a2/src/scripts/simpleidml_indesign_save_as.py`

 * *Files identical despite different names*

