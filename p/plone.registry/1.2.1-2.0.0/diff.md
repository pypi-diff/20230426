# Comparing `tmp/plone.registry-1.2.1.tar.gz` & `tmp/plone.registry-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.registry-1.2.1.tar", last modified: Tue Jun 15 01:31:31 2021, max compression
+gzip compressed data, was "plone.registry-2.0.0.tar", last modified: Wed Apr 26 21:52:20 2023, max compression
```

## Comparing `plone.registry-1.2.1.tar` & `plone.registry-2.0.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:31:31.585785 plone.registry-1.2.1/
--rw-r--r--   0 ems174     (502) staff       (20)     4211 2021-06-15 01:31:31.000000 plone.registry-1.2.1/CHANGES.rst
--rw-r--r--   0 ems174     (502) staff       (20)       70 2021-06-15 01:31:31.000000 plone.registry-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 ems174     (502) staff       (20)      155 2021-06-15 01:31:31.000000 plone.registry-1.2.1/MANIFEST.in
--rw-r--r--   0 ems174     (502) staff       (20)    69160 2021-06-15 01:31:31.585985 plone.registry-1.2.1/PKG-INFO
--rw-r--r--   0 ems174     (502) staff       (20)      505 2021-06-15 01:31:31.000000 plone.registry-1.2.1/README.rst
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:31:31.583202 plone.registry-1.2.1/docs/
--rw-r--r--   0 ems174     (502) staff       (20)     1208 2021-06-15 01:31:31.000000 plone.registry-1.2.1/docs/INSTALL.txt
--rw-r--r--   0 ems174     (502) staff       (20)    12282 2021-06-15 01:31:31.000000 plone.registry-1.2.1/docs/LICENSE.GPL
--rw-r--r--   0 ems174     (502) staff       (20)      780 2021-06-15 01:31:31.000000 plone.registry-1.2.1/docs/LICENSE.txt
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:31:31.583300 plone.registry-1.2.1/plone/
--rw-r--r--   0 ems174     (502) staff       (20)       80 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/__init__.py
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:31:31.585683 plone.registry-1.2.1/plone/registry/
--rw-r--r--   0 ems174     (502) staff       (20)      155 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/__init__.py
--rw-r--r--   0 ems174     (502) staff       (20)      311 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/configure.zcml
--rw-r--r--   0 ems174     (502) staff       (20)     1800 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/events.py
--rw-r--r--   0 ems174     (502) staff       (20)     4932 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/events.rst
--rw-r--r--   0 ems174     (502) staff       (20)     8689 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/field.py
--rw-r--r--   0 ems174     (502) staff       (20)    25907 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/field.rst
--rw-r--r--   0 ems174     (502) staff       (20)     3133 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/fieldfactory.py
--rw-r--r--   0 ems174     (502) staff       (20)      688 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/fieldref.py
--rw-r--r--   0 ems174     (502) staff       (20)     6771 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/interfaces.py
--rw-r--r--   0 ems174     (502) staff       (20)     3240 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/record.py
--rw-r--r--   0 ems174     (502) staff       (20)     5487 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/recordsproxy.py
--rw-r--r--   0 ems174     (502) staff       (20)     9588 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/registry.py
--rw-r--r--   0 ems174     (502) staff       (20)    18403 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/registry.rst
--rw-r--r--   0 ems174     (502) staff       (20)     5754 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone/registry/tests.py
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:31:31.584207 plone.registry-1.2.1/plone.registry.egg-info/
--rw-r--r--   0 ems174     (502) staff       (20)    69160 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone.registry.egg-info/PKG-INFO
--rw-r--r--   0 ems174     (502) staff       (20)      847 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone.registry.egg-info/SOURCES.txt
--rw-r--r--   0 ems174     (502) staff       (20)        1 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone.registry.egg-info/dependency_links.txt
--rw-r--r--   0 ems174     (502) staff       (20)       33 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone.registry.egg-info/entry_points.txt
--rw-r--r--   0 ems174     (502) staff       (20)        6 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone.registry.egg-info/namespace_packages.txt
--rw-r--r--   0 ems174     (502) staff       (20)        1 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone.registry.egg-info/not-zip-safe
--rw-r--r--   0 ems174     (502) staff       (20)      108 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone.registry.egg-info/requires.txt
--rw-r--r--   0 ems174     (502) staff       (20)        6 2021-06-15 01:31:31.000000 plone.registry-1.2.1/plone.registry.egg-info/top_level.txt
--rw-r--r--   0 ems174     (502) staff       (20)      397 2021-06-15 01:31:31.000000 plone.registry-1.2.1/pyproject.toml
--rw-r--r--   0 ems174     (502) staff       (20)      226 2021-06-15 01:31:31.586242 plone.registry-1.2.1/setup.cfg
--rw-r--r--   0 ems174     (502) staff       (20)     2043 2021-06-15 01:31:31.000000 plone.registry-1.2.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:52:20.501615 plone.registry-2.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)     4393 2023-04-26 21:52:19.000000 plone.registry-2.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 21:52:19.000000 plone.registry-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      155 2023-04-26 21:52:19.000000 plone.registry-2.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    54556 2023-04-26 21:52:20.501802 plone.registry-2.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      505 2023-04-26 21:52:19.000000 plone.registry-2.0.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:52:20.495293 plone.registry-2.0.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1208 2023-04-26 21:52:19.000000 plone.registry-2.0.0/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-04-26 21:52:19.000000 plone.registry-2.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      780 2023-04-26 21:52:19.000000 plone.registry-2.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:52:20.495584 plone.registry-2.0.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:52:20.501418 plone.registry-2.0.0/plone/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      310 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1736 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4932 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/events.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8345 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/field.py
+-rw-r--r--   0 maurits    (501) staff       (20)    25907 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/field.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3133 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/fieldfactory.py
+-rw-r--r--   0 maurits    (501) staff       (20)      651 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/fieldref.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6525 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3213 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/record.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5076 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/recordsproxy.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9024 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/registry.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17828 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/registry.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5383 2023-04-26 21:52:19.000000 plone.registry-2.0.0/plone/registry/tests.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:52:20.497688 plone.registry-2.0.0/plone.registry.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    54556 2023-04-26 21:52:20.000000 plone.registry-2.0.0/plone.registry.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      806 2023-04-26 21:52:20.000000 plone.registry-2.0.0/plone.registry.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:52:20.000000 plone.registry-2.0.0/plone.registry.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:52:20.000000 plone.registry-2.0.0/plone.registry.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:52:20.000000 plone.registry-2.0.0/plone.registry.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      108 2023-04-26 21:52:20.000000 plone.registry-2.0.0/plone.registry.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:52:20.000000 plone.registry-2.0.0/plone.registry.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2893 2023-04-26 21:52:19.000000 plone.registry-2.0.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      270 2023-04-26 21:52:20.502259 plone.registry-2.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1946 2023-04-26 21:52:19.000000 plone.registry-2.0.0/setup.py
```

### Comparing `plone.registry-1.2.1/CHANGES.rst` & `plone.registry-2.0.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.0 (2023-04-26)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 compatibility.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (a864b30f)
+
+
 1.2.1 (2021-06-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix registry key validation regexp.
```

### Comparing `plone.registry-1.2.1/PKG-INFO` & `plone.registry-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,1790 +1,1790 @@
 Metadata-Version: 2.1
 Name: plone.registry
-Version: 1.2.1
+Version: 2.0.0
 Summary: Registry for application settings (like debconf/ about:config)
 Home-page: https://pypi.org/project/plone.registry
 Author: Martin Aspeli, Wichert Akkerman, Hanno Schlichting
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
-Description: ============
-        Introduction
-        ============
-        This package provides debconf-like (or about:config-like) settings registries
-        for Zope applications. A ``registry``, with a dict-like API, is used to get and
-        set values stored in ``records``. Each record contains the actual value, as
-        well as a ``field`` that describes the record in more detail. At a minimum, the
-        field contains information about the type of value allowed, as well as a short
-        title describing the record's purpose.
-        
-        .. contents:: Table of Contents
-        
-        
-        ================
-        Using registries
-        ================
-        
-        You can create a new registry simply by instantiating the Registry class.
-        The class and its data structures are persistent, so you can store them in the ZODB.
-        You may want to provide the registry object as local utility for easy access as well, though we won't do that here.
-        
-        ::
-        
-            >>> from plone.registry import Registry
-            >>> registry = Registry()
-        
-        The registry starts out empty.
-        To access the registry's records, you can use the ``records`` property.
-        This exposes a dict API where keys are strings and values are objects providing ``IRecords``.
-        
-        ::
-        
-            >>> len(registry.records)
-            0
-        
-        Simple records
-        ==============
-        
-        Let's now create a record.
-        A record must have a name.
-        This should be a dotted name, and contain ASCII characters only.
-        By convention, it should be all lowercase and start with the name of the package that defines the record.
-        
-        It is also possible to create a  number of records based on a single schema interface - see below.
-        For now, we will focus on simple records.
-        
-        Before we can create the record, we must create the field that describes it.
-        Fields are based on the venerable ``zope.schema`` package.
-        ``plone.registry`` only supports certain fields, and disallows use of a few properties even of those.
-        As a rule of thumb, so long as a field stores a Python primitive, it is supported; the same goes for attributes of fields.
-        
-        Thus:
-        
-        * Fields like ``Object``, ``InterfaceField`` and so on are *not* supported.
-        * A custom ``constraint`` method is *not* supported.
-        * The ``order`` attribute will *always* be set to ``-1``.
-        * For Choice fields, *only named vocabularies* are supported:
-          you can *not* reference a particular *source* or *source binder*.
-        * The ``key_type`` and ``value_type`` properties of ``Dict``, ``List``, ``Tuple``, ``Set`` and ``Frozenset`` may *only* contain persistent fields.
-        
-        See section "Persistent fields" for more details.
-        
-        Creating a record
-        -----------------
-        
-        The supported field types are found in the module ``plone.registry.field``.
-        These are named the same as the equivalent field in ``zope.schema``, and have the same constructors.
-        You must use one of these fields when creating records directly::
-        
-            >>> from plone.registry import field
-            >>> age_field = field.Int(title=u"Age", min=0, default=18)
-        
-            >>> from plone.registry import Record
-            >>> age_record = Record(age_field)
-        
-        Note that in this case, we did not supply a value.
-        The value will therefore be the field default::
-        
-            >>> age_record.value
-            18
-        
-        We can set a different value, either in the ``Record`` constructor or via the ``value`` attribute::
-        
-            >>> age_record.value = 2
-            >>> age_record.value
-            2
-        
-        Note that the value is validated against the field::
-        
-            >>> age_record.value = -1  # doctest: +SKIP_PYTHON_3
-            Traceback (most recent call last):
-            ...
-            TooSmall: (-1, 0)
-        
-            >>> age_record.value = -1  # doctest: +SKIP_PYTHON_2
-            Traceback (most recent call last):
-            ...
-            zope.schema._bootstrapinterfaces.TooSmall: (-1, 0)
-        
-            >>> age_record.value
-            2
-        
-        We can now add the field to the registry.
-        This is done via the ``record`` dictionary::
-        
-            >>> 'plone.registry.tests.age' in registry
-            False
-            >>> registry.records['plone.registry.tests.age'] = age_record
-        
-        At this point, the record will gain ``__name__`` and ``__parent__`` attributes::
-        
-            >>> age_record.__name__
-            'plone.registry.tests.age'
-        
-            >>> age_record.__parent__ is registry
-            True
-        
-        Creating a record with an initial value
-        ---------------------------------------
-        
-        We can create records more succinctly in *one go* by
-        
-        1. creating the field,
-        2. creating the Record and setting its value as and
-        3. assigning it to the registry,
-        
-        like this::
-        
-            >>> registry.records['plone.registry.tests.cms'] = \
-            ...     Record(field.TextLine(title=u"CMS of choice"), u"Plone")
-        
-        The record can now be obtained.
-        Note that it has a nice ``__repr__`` to help debugging.
-        
-            >>> registry.records['plone.registry.tests.cms']
-            <Record plone.registry.tests.cms>
-        
-        Accessing and manipulating record values
-        ----------------------------------------
-        
-        Once a record has been created and added to the registry,
-        you can access its value through dict-like operations on the registry itself::
-        
-            >>> 'plone.registry.tests.cms' in registry
-            True
-        
-            >>> registry['plone.registry.tests.cms']  # doctest: +IGNORE_U
-            u'Plone'
-        
-            >>> registry['plone.registry.tests.cms'] = u"Plone 3.x"
-        
-        Again, values are validated::
-        
-            >>> registry['plone.registry.tests.cms'] = b'Joomla'  # doctest: +SKIP_PYTHON_3
-            Traceback (most recent call last):
-            ...
-            WrongType: ('Joomla', <type 'unicode'>...)
-        
-            >>> registry['plone.registry.tests.cms'] = b'Joomla'  # doctest: +SKIP_PYTHON_2
-            Traceback (most recent call last):
-            ...
-            zope.schema._bootstrapinterfaces.WrongType: (b'Joomla', <class 'str'>, 'value')
-        
-        There is also a ``get()`` method::
-        
-            >>> registry.get('plone.registry.tests.cms')  # doctest: +IGNORE_U
-            u'Plone 3.x'
-            >>> registry.get('non-existent-key') is None
-            True
-        
-        Deleting records
-        ----------------
-        
-        Records may be deleted from the ``records`` property::
-        
-            >>> del registry.records['plone.registry.tests.cms']
-            >>> 'plone.registry.tests.cms' in registry.records
-            False
-            >>> 'plone.registry.tests.cms' in registry
-            False
-        
-        Creating records from interfaces
-        ================================
-        
-        As an application developer, it is often desirable to define settings as traditional interfaces with ``zope.schema fields``.
-        ``plone.registry`` includes support for creating a set of records from a single interface.
-        
-        To test this, we have created an interface, ``IMailSettings``.
-        It has two fields: ``sender`` and ``smtp_host``::
-        
-            >>> from plone.registry.tests import IMailSettings
-        
-        Note that this contains standard fields::
-        
-            >>> IMailSettings['sender']
-            <zope.schema._bootstrapfields.TextLine object at ...>
-        
-            >>> IMailSettings['smtp_host']
-            <zope.schema._field.URI object at ...>
-        
-        We can create records from this interface like this::
-        
-            >>> registry.registerInterface(IMailSettings)
-        
-        One record for each field in the interface has now been created.
-        Their names are the full dotted names to those fields::
-        
-            >>> sender_record = registry.records['plone.registry.tests.IMailSettings.sender']
-            >>> smtp_host_record = registry.records['plone.registry.tests.IMailSettings.smtp_host']
-        
-        The fields used in the records will be the equivalent persistent versions of the fields from the original interface::
-        
-            >>> sender_record.field
-            <plone.registry.field.TextLine object at ...>
-        
-            >>> smtp_host_record.field
-            <plone.registry.field.URI object at ...>
-        
-        This feat is accomplished internally by adapting the field to the ``IPersistentField`` interface.
-        There is a default adapter factory that works for all fields defined in ``plone.registry.field``.
-        You can of course define your own adapter if you have a custom field type.
-        But bear in mind the golden rules of any persistent field::
-        
-        * The field must store only primitives or other persistent fields
-        * It must not reference a function, class, interface or other method that could break if a package is uninstalled.
-        
-        If we have a field for which there is no ``IPersistentField`` adapter, we will get an error::
-        
-            >>> from plone.registry.tests import IMailPreferences
-            >>> IMailPreferences['settings']
-            <zope.schema._bootstrapfields.Object object at ...>
-        
-            >>> registry.registerInterface(IMailPreferences)
-            Traceback (most recent call last):
-            ...
-            TypeError: There is no persistent field equivalent for the field `settings` of type `Object`.
-        
-        Whoops!
-        We can, however, tell ``registerInterface()`` to ignore one or more fields::
-        
-            >>> registry.registerInterface(IMailPreferences, omit=('settings',))
-        
-        Once an interface's records have been registered, we can get and set their values as normal::
-        
-            >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
-            u'root@localhost'
-        
-            >>> registry['plone.registry.tests.IMailSettings.sender'] = u"webmaster@localhost"
-            >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
-            u'webmaster@localhost'
-        
-        If we sub-sequently re-register the same interface, the value will be retained if possible::
-        
-            >>> registry.registerInterface(IMailSettings)
-            >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
-            u'webmaster@localhost'
-        
-        However, if the value is no longer valid, we will revert to the default.
-        To test that, let's sneakily modify the field for a while::
-        
-            >>> old_field = IMailSettings['sender']
-            >>> IMailSettings._InterfaceClass__attrs['sender'] = field.Int(title=u"Definitely not a string", default=2)
-            >>> if hasattr(IMailSettings, '_v_attrs'):
-            ...     del IMailSettings._v_attrs['sender']
-            >>> registry.registerInterface(IMailSettings)
-            >>> registry['plone.registry.tests.IMailSettings.sender']
-            2
-        
-        But let's put it back the way it was::
-        
-            >>> IMailSettings._InterfaceClass__attrs['sender'] = old_field
-            >>> if hasattr(IMailSettings, '_v_attrs'):
-            ...     del IMailSettings._v_attrs['sender']
-            >>> registry.registerInterface(IMailSettings)
-            >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
-            u'root@localhost'
-        
-        Sometimes, you may want to use an interface as a template for multiple instances of a set of fields, rather than defining them all by hand.
-        This is especially useful when you want to allow third-party packages to provide information.
-        To accomplish this, we can provide a prefix with the ``registerInterface`` call.
-        This will take precedence over the ``__identifier__`` that is usually used.
-        
-            >>> registry.registerInterface(IMailSettings, prefix="plone.registry.tests.alternativesettings")
-        
-        These values are now available in the same way as the original settings::
-        
-            >>> sender_record = registry.records['plone.registry.tests.alternativesettings.sender']
-            >>> smtp_host_record = registry.records['plone.registry.tests.alternativesettings.smtp_host']
-            >>> registry['plone.registry.tests.alternativesettings.sender'] = u'alt@example.org'
-        
-        Accessing the original interface
-        --------------------------------
-        
-        Now that we have these records, we can look up the original interface.
-        This does not break the golden rules:
-        internally, we only store the name of the interface, and resolve it at runtime.
-        
-        Records that know about interfaces are marked with ``IInterfaceAwareRecord`` and have two additional properties:
-        ``interface`` and ``fieldName``::
-        
-            >>> from plone.registry.interfaces import IInterfaceAwareRecord
-            >>> IInterfaceAwareRecord.providedBy(age_record)
-            False
-            >>> IInterfaceAwareRecord.providedBy(sender_record)
-            True
-        
-            >>> sender_record.interfaceName
-            'plone.registry.tests.IMailSettings'
-        
-            >>> sender_record.interface is IMailSettings
-            True
-        
-        Using the records proxy
-        -----------------------
-        
-        Once the records for an interface has been created, it is possible to obtain a proxy object that provides the given interface, but reads and writes its values to the registry.
-        This is useful, for example, to create a form using ``zope.formlib`` or  ``z3c.form`` that is configured with widgets based on the
-        interface.
-        Or simply as a more convenient API when working with multiple, related settings.
-        
-        ::
-        
-            >>> proxy = registry.forInterface(IMailSettings)
-            >>> proxy
-            <RecordsProxy for plone.registry.tests.IMailSettings>
-        
-        If you use your registry values in code which might be encountered on normal HTML rendering paths (e.g. in a viewlet) you need to be aware that records might not exist or they are invalid.
-        ``forInterface()`` will raise KeyError on this kind of situations::
-        
-            try:
-                proxy = registry.forInterface(IMailSettings)
-            except KeyError:
-                # Gracefully handled cases
-                # when GenericSetup installer has not been run or rerun
-                # e.g. by returning or using some default values
-                pass
-        
-        The proxy is not a persistent object on its own::
-        
-            >>> from persistent.interfaces import IPersistent
-            >>> IPersistent.providedBy(proxy)
-            False
-        
-        It does, however, provide the requisite interface::
-        
-            >>> IMailSettings.providedBy(proxy)
-            True
-        
-        You can distinguish between the proxy and a 'normal' object by checking for the ``IRecordsProxy`` marker interface::
-        
-            >>> from plone.registry.interfaces import IRecordsProxy
-            >>> IRecordsProxy.providedBy(proxy)
-            True
-        
-        When we set a value, it is stored in the registry::
-        
-            >>> proxy.smtp_host = 'http://mail.server.com'
-            >>> registry['plone.registry.tests.IMailSettings.smtp_host']
-            'http://mail.server.com'
-        
-            >>> registry['plone.registry.tests.IMailSettings.smtp_host'] = 'smtp://mail.server.com'
-            >>> proxy.smtp_host
-            'smtp://mail.server.com'
-        
-        Values not in the interface will raise an ``AttributeError``::
-        
-            >>> proxy.age
-            Traceback (most recent call last):
-            ...
-            AttributeError: age
-        
-        Note that by default, the forInterface() method will check that the necessary records have been registered.
-        For example, we cannot use any old interface::
-        
-            >>> registry.forInterface(IInterfaceAwareRecord)
-            Traceback (most recent call last):
-            ...
-            KeyError: 'Interface `plone.registry.interfaces.IInterfaceAwareRecord` defines a field `...`, for which there is no record.'
-        
-        By default, we also cannot use an interface for which only some records exist::
-        
-            >>> registry.forInterface(IMailPreferences)
-            Traceback (most recent call last):
-            ...
-            KeyError: 'Interface `plone.registry.tests.IMailPreferences` defines a field `settings`, for which there is no record.'
-        
-        It is possible to disable this check, however.
-        This will be a bit more efficient::
-        
-            >>> registry.forInterface(IMailPreferences, check=False)
-            <RecordsProxy for plone.registry.tests.IMailPreferences>
-        
-        A better way, however, is to explicitly declare that some fields are omitted::
-        
-            >>> pref_proxy = registry.forInterface(IMailPreferences, omit=('settings',))
-        
-        In this case, the omitted fields will default to their 'missing' value::
-        
-            >>> pref_proxy.settings ==  IMailPreferences['settings'].missing_value
-            True
-        
-        However, trying to set the value will result in a ``AttributeError``::
-        
-            >>> pref_proxy.settings = None
-            Traceback (most recent call last):
-            ...
-            AttributeError: settings
-        
-        To access another instance of the field, supply the prefix::
-        
-            >>> alt_proxy = registry.forInterface(IMailSettings,
-            ...     prefix="plone.registry.tests.alternativesettings")
-            >>> alt_proxy.sender  # doctest: +IGNORE_U
-            u'alt@example.org'
-        
-        Collections of records proxies
-        ------------------------------
-        
-        A collection of record sets may be accessed using ``collectionOfInterface``::
-        
-            >>> collection = registry.collectionOfInterface(IMailSettings)
-        
-        You can create a new record set::
-        
-            >>> proxy = collection.setdefault('example')
-            >>> proxy.sender = u'collection@example.org'
-            >>> proxy.smtp_host = 'smtp://mail.example.org'
-        
-        Record sets are stored based under the prefix::
-        
-            >>> prefix = IMailSettings.__identifier__
-            >>> registry.records.values(prefix+'/', prefix+'0')
-            [<Record plone.registry.tests.IMailSettings/example.sender>,
-             <Record plone.registry.tests.IMailSettings/example.smtp_host>]
-            >>> registry['plone.registry.tests.IMailSettings/example.sender']  # doctest: +IGNORE_U
-            u'collection@example.org'
-        
-        Records may be set from an existing object::
-        
-            >>> class MailSettings:
-            ...     sender = u'someone@example.com'
-            ...     smtp_host = 'smtp://mail.example.com'
-            >>> collection['example_com'] = MailSettings()
-            >>> registry.records.values(prefix+'/', prefix+'0')
-            [<Record plone.registry.tests.IMailSettings/example.sender>,
-             <Record plone.registry.tests.IMailSettings/example.smtp_host>,
-             <Record plone.registry.tests.IMailSettings/example_com.sender>,
-             <Record plone.registry.tests.IMailSettings/example_com.smtp_host>]
-        
-        The collection may be iterated over::
-        
-            >>> for name in collection: print(name)
-            example
-            example_com
-        
-        And may be deleted::
-        
-            >>> del collection['example_com']
-            >>> registry.records.values(prefix+'/', prefix+'0')
-            [<Record plone.registry.tests.IMailSettings/example.sender>,
-             <Record plone.registry.tests.IMailSettings/example.smtp_host>]
-        
-        Using field references
-        ======================
-        
-        It is possible for one record to refer to another record's field.
-        This can be used to provide a simple "override" mechanism,
-        for example, where one record defines the field and a default value,
-        whilst another provides an override validated against the same field.
-        
-        Let us first create the base record and set its value::
-        
-            >>> timeout_field = field.Int(title=u"Timeout", min=0)
-            >>> registry.records['plone.registry.tests.timeout'] = Record(timeout_field, 10)
-        
-            >>> timeout_record = registry.records['plone.registry.tests.timeout']
-            >>> timeout_record.value
-            10
-        
-        Next, we create a field reference for this record::
-        
-            >>> from plone.registry import FieldRef
-            >>> timeout_override_field = FieldRef(timeout_record.__name__, timeout_record.field)
-        
-        We can use this to create a new record::
-        
-            >>> registry.records['plone.registry.tests.timeout.override'] = Record(timeout_override_field, 20)
-            >>> timeout_override_record = registry.records['plone.registry.tests.timeout.override']
-        
-        The two values are separate::
-        
-            >>> timeout_record.value
-            10
-            >>> timeout_override_record.value
-            20
-        
-            >>> registry['plone.registry.tests.timeout']
-            10
-            >>> registry['plone.registry.tests.timeout.override']
-            20
-        
-        Validation uses the underlying field::
-        
-            >>> registry['plone.registry.tests.timeout.override'] = -1  # doctest: +SKIP_PYTHON_3
-            Traceback (most recent call last):
-            ...
-            TooSmall: (-1, 0)
-        
-            >>> registry['plone.registry.tests.timeout.override'] = -1  # doctest: +SKIP_PYTHON_2
-            Traceback (most recent call last):
-            ...
-            zope.schema._bootstrapinterfaces.TooSmall: (-1, 0)
-        
-        The reference field exposes the standard field properties, e.g.::
-        
-            >>> timeout_override_record.field.title  # doctest: +SKIP_PYTHON_3
-            u'Timeout'
-            >>> timeout_override_record.field.min
-            0
-        
-        To look up the underlying record name, we can use the ``recordName`` property::
-        
-            >>> timeout_override_record.field.recordName
-            'plone.registry.tests.timeout'
-        
-        
-        ===============
-        Registry events
-        ===============
-        
-        The registry fires certain events. These are:
-        
-        ``plone.registry.interfaces.IRecordAddedEvent``
-            when a record has been added to the registry.
-        
-        ``plone.registry.interfaces.IRecordRemovedEvent``
-            when a record has been removed from the registry.
-        
-        ``plone.registry.interfaces.IRecordModifiedEvent``,
-            when a record's value is modified.
-        
-        To test these events, we will create, modify and remove a few records::
-        
-            >>> from zope.component.eventtesting import clearEvents
-            >>> clearEvents()
-            >>> from plone.registry import Registry, Record, field
-            >>> registry = Registry()
-        
-        Adding a new record to the registry should fire ``IRecordAddedEvents``::
-        
-            >>> registry.records['plone.registry.tests.age'] = \
-            ...     Record(field.Int(title=u"Age", min=0, default=18))
-        
-            >>> registry.records['plone.registry.tests.cms'] = \
-            ...     Record(field.TextLine(title=u"Preferred CMS"), value=u"Plone")
-        
-        When creating records from an interface, one event is fired for each field in the interface::
-        
-            >>> from plone.registry.tests import IMailSettings
-            >>> registry.registerInterface(IMailSettings)
-        
-        Deleting a record should fire an ``IRecordRemovedEvent``::
-        
-            >>> del registry.records['plone.registry.tests.cms']
-        
-        Changing a record should fire an ``IRecordModifiedEvent``::
-        
-            >>> registry['plone.registry.tests.age'] = 25
-            >>> registry.records['plone.registry.tests.age'].value = 24
-        
-        Let's take a look at the events that were just fired::
-        
-            >>> from plone.registry.interfaces import IRecordEvent
-            >>> from zope.component.eventtesting import getEvents
-            >>> getEvents(IRecordEvent)
-            [<RecordAddedEvent for plone.registry.tests.age>,
-             <RecordAddedEvent for plone.registry.tests.cms>,
-             <RecordAddedEvent for plone.registry.tests.IMailSettings.sender>,
-             <RecordAddedEvent for plone.registry.tests.IMailSettings.smtp_host>,
-             <RecordRemovedEvent for plone.registry.tests.cms>,
-             <RecordModifiedEvent for plone.registry.tests.age>,
-             <RecordModifiedEvent for plone.registry.tests.age>]
-        
-        For the modified events, we can also check the value before and after the change::
-        
-            >>> from plone.registry.interfaces import IRecordModifiedEvent
-            >>> [(repr(e), e.oldValue, e.newValue,) for e in getEvents(IRecordModifiedEvent)]
-            [('<RecordModifiedEvent for plone.registry.tests.age>', 18, 25),
-             ('<RecordModifiedEvent for plone.registry.tests.age>', 25, 24)]
-        
-        IObjectEvent-style redispatchers
-        ================================
-        
-        There is a special event handler.
-        It takes care of re-dispatching registry events based on the schema interface prescribed by the record.
-        
-        Let's re-set the event testing framework and register the re-dispatching event subscriber.
-        Normally, this would happen automatically by including this package's ZCML.
-        
-        ::
-        
-            >>> clearEvents()
-            >>> from zope.component import provideHandler
-            >>> from plone.registry.events import redispatchInterfaceAwareRecordEvents
-            >>> provideHandler(redispatchInterfaceAwareRecordEvents)
-        
-        We'll then register a schema interface::
-        
-            >>> from plone.registry.tests import IMailSettings
-            >>> registry.registerInterface(IMailSettings)
-        
-        We could now register an event handler to print any record event occurring on an ``IMailSettings`` record.
-        More specialised event handlers for e.g. ``IRecordModifiedEvent`` or ``IRecordRemovedEvent`` are of course also possible.
-        Note that it is not possible to re-dispatch ``IRecordAddedEvents``, so these are never caught.
-        
-            >>> from zope.component import adapter
-            >>> @adapter(IMailSettings, IRecordEvent)
-            ... def print_mail_settings_events(proxy, event):
-            ...     print("Got %s for %s" % (event, proxy))
-            >>> provideHandler(print_mail_settings_events)
-        
-        Let's now modify one of the records for this interface.
-        The event handler should react immediately::
-        
-            >>> registry['plone.registry.tests.IMailSettings.sender'] = u"Some sender"
-            Got <RecordModifiedEvent for plone.registry.tests.IMailSettings.sender> for <RecordsProxy for plone.registry.tests.IMailSettings>
-        
-        Let's also modify a non-interface-aware record, for comparison's sake.
-        Here, there is nothing printed::
-        
-            >>> registry['plone.registry.tests.age'] = 3
-        
-        We can try a record-removed event as well::
-        
-            >>> del registry.records['plone.registry.tests.IMailSettings.sender']
-            Got <RecordRemovedEvent for plone.registry.tests.IMailSettings.sender> for <RecordsProxy for plone.registry.tests.IMailSettings>
-        
-        The basic events that have been dispatched are::
-        
-            >>> getEvents(IRecordEvent)
-            [<RecordAddedEvent for plone.registry.tests.IMailSettings.sender>,
-             <RecordAddedEvent for plone.registry.tests.IMailSettings.smtp_host>,
-             <RecordModifiedEvent for plone.registry.tests.IMailSettings.sender>,
-             <RecordModifiedEvent for plone.registry.tests.age>,
-             <RecordRemovedEvent for plone.registry.tests.IMailSettings.sender>]
-        
-        
-        =================
-        Persistent fields
-        =================
-        
-        The persistent fields that are found in ``plone.registry.field`` are siblings of the ones found in zope.schema,
-        with persistence mixed in.
-        To avoid potentially breaking the registry with persistent references to symbols that may go away,
-        we purposefully limit the number of fields supported.
-        We also disallow some properties, and add some additional checks on others.
-        
-        The standard fields
-        ===================
-        
-        We will show each supported field in turn. For all fields, note that:
-        
-        * the ``order`` property will return ``-1`` no matter what setting the ``constraint`` property is diallowed
-        * the ``key_type`` and ``value_type`` properties, where applicable, must be set to a persistent field.
-        * for ``Choice`` fields, only named vocabularies and vocabularies based on simple values are supported:
-          sources and ``IVocabulary`` objects are not.
-        
-        Imports needed::
-        
-            >>> from plone.registry import field
-            >>> from zope import schema
-            >>> from persistent import Persistent
-        
-        Bytes
-        -----
-        
-        The bytes field describes a string of bytes::
-        
-            >>> f = field.Bytes(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.Bytes)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Bytes(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint('ABC')
-            True
-        
-        BytesLine
-        ---------
-        
-        The bytes field describes a string of bytes, disallowing newlines::
-        
-            >>> f = field.BytesLine(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.BytesLine)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.BytesLine(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(b'AB\nC')
-            False
-        
-        ASCII
-        -----
-        
-        The ASCII field describes a string containing only ASCII characters::
-        
-            >>> f = field.ASCII(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.ASCII)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.ASCII(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint('ab\nc')
-            True
-        
-        ASCIILine
-        ---------
-        
-        The ASCII line field describes a string containing only ASCII characters and disallowing newlines::
-        
-            >>> f = field.ASCIILine(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.ASCIILine)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.ASCIILine(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint('ab\nc')
-            False
-        
-        Text
-        ----
-        
-        The text field describes a unicode string::
-        
-            >>> f = field.Text(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.Text)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Text(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'ab\nc')
-            True
-        
-        TextLine
-        --------
-        
-        The text line field describes a unicode string, disallowing newlines::
-        
-            >>> f = field.TextLine(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.TextLine)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.TextLine(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'ab\nc')
-            False
-        
-        Bool
-        ----
-        
-        The bool field describes a boolean::
-        
-            >>> f = field.Bool(title=u"Test")
-            >>> isinstance(f, schema.Bool)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Bool(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(False)
-            True
-        
-        Int
-        ---
-        
-        The int field describes an integer or long::
-        
-            >>> f = field.Int(title=u"Test", min=-123, max=1234)
-            >>> isinstance(f, schema.Int)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Int(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(123)
-            True
-        
-        Float
-        -----
-        
-        The float field describes a float::
-        
-            >>> f = field.Float(title=u"Test", min=-123.0, max=1234.0)
-            >>> isinstance(f, schema.Float)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Float(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(123)
-            True
-        
-        Decimal
-        -------
-        
-        The decimal field describes a decimal::
-        
-            >>> import decimal
-            >>> f = field.Decimal(title=u"Test", min=decimal.Decimal('-123.0'), max=decimal.Decimal('1234.0'))
-            >>> isinstance(f, schema.Decimal)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Decimal(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(123)
-            True
-        
-        Password
-        --------
-        
-        The password field describes a unicode string used for a password::
-        
-            >>> f = field.Password(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.Password)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Password(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'ab\nc')
-            False
-        
-        SourceText
-        ----------
-        
-        The source  text field describes a unicode string with source code::
-        
-            >>> f = field.SourceText(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.SourceText)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.SourceText(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'ab\nc')
-            True
-        
-        URI
-        ---
-        
-        The URI field describes a URI string::
-        
-            >>> f = field.URI(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.URI)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.URI(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'abc')
-            True
-        
-        Id
-        --
-        
-        The id field describes a URI string or a dotted name::
-        
-            >>> f = field.Id(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.Id)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Id(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'abc')
-            True
-        
-        DottedName
-        ----------
-        
-        The dotted name field describes a Python dotted name::
-        
-            >>> f = field.DottedName(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.DottedName)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.DottedName(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'abc')
-            True
-        
-        Datetime
-        --------
-        
-        The date/time field describes a Python datetime object::
-        
-            >>> f = field.Datetime(title=u"Test")
-            >>> isinstance(f, schema.Datetime)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Datetime(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> import datetime
-            >>> f.constraint(datetime.datetime.now())
-            True
-        
-        Date
-        ----
-        
-        The date field describes a Python date object::
-        
-            >>> f = field.Date(title=u"Test")
-            >>> isinstance(f, schema.Date)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Date(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> import datetime
-            >>> f.constraint(datetime.date.today())
-            True
-        
-        Timedelta
-        ---------
-        
-        The time-delta field describes a Python timedelta object::
-        
-            >>> f = field.Timedelta(title=u"Test")
-            >>> isinstance(f, schema.Timedelta)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Timedelta(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> import datetime
-            >>> f.constraint(datetime.timedelta(1))
-            True
-        
-        Tuple
-        -----
-        
-        The tuple field describes a tuple::
-        
-            >>> f = field.Tuple(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=field.TextLine(title=u"Value"))
-            >>> isinstance(f, schema.Tuple)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Tuple(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=schema.TextLine(title=u"Value"))
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> f.value_type = schema.TextLine(title=u"Value")
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> field.Tuple(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint((1,2))
-            True
-        
-        List
-        ----
-        
-        The list field describes a tuple::
-        
-            >>> f = field.List(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=field.TextLine(title=u"Value"))
-            >>> isinstance(f, schema.List)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.List(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=schema.TextLine(title=u"Value"))
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> f.value_type = schema.TextLine(title=u"Value")
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> field.List(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint([1,2])
-            True
-        
-        Set
-        ---
-        
-        The set field describes a set::
-        
-            >>> f = field.Set(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=field.TextLine(title=u"Value"))
-            >>> isinstance(f, schema.Set)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Set(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=schema.TextLine(title=u"Value"))
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> f.value_type = schema.TextLine(title=u"Value")
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> field.Set(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(set([1,2]))
-            True
-        
-        Frozenset
-        ---------
-        
-        The set field describes a frozenset::
-        
-            >>> f = field.FrozenSet(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=field.TextLine(title=u"Value"))
-            >>> isinstance(f, schema.FrozenSet)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.FrozenSet(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=schema.TextLine(title=u"Value"))
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> f.value_type = schema.TextLine(title=u"Value")
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> field.FrozenSet(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(frozenset([1,2]))
-            True
-        
-        Dict
-        ----
-        
-        The set field describes a dict::
-        
-            >>> f = field.Dict(title=u"Test", min_length=0, max_length=10,
-            ...     key_type=field.ASCII(title=u"Key"),
-            ...     value_type=field.TextLine(title=u"Value"))
-            >>> isinstance(f, schema.Dict)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Dict(title=u"Test", min_length=0, max_length=10,
-            ...     key_type=schema.ASCII(title=u"Key"),
-            ...     value_type=field.TextLine(title=u"Value"))
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `key_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> f.key_type = schema.ASCII(title=u"Key")
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `key_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> field.Dict(title=u"Test", min_length=0, max_length=10,
-            ...     key_type=field.ASCII(title=u"Key"),
-            ...     value_type=schema.TextLine(title=u"Value"))
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> f.value_type = schema.TextLine(title=u"Value")
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> field.Dict(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(dict())
-            True
-        
-        Choice
-        ------
-        
-        A choice field represents a selection from a vocabulary.
-        For persistent fields, the vocabulary cannot be a ``source`` or any kind of object:
-        it must either be a list of primitives, or a named vocabulary::
-        
-            >>> f = field.Choice(title=u"Test", values=[1,2,3])
-            >>> isinstance(f, schema.Choice)
-            True
-        
-            >>> f.order
-            -1
-        
-        With a list of values given, the ``vocabulary`` property returns a vocabulary
-        constructed from the values on the fly, and ``vocabularyName`` is ``None``::
-        
-            >>> f.vocabulary
-            <zope.schema.vocabulary.SimpleVocabulary object at ...>
-        
-            >>> f.vocabularyName is None
-            True
-        
-        We will get an error if we use anything other than primitives::
-        
-            >>> f = field.Choice(title=u"Test", values=[object(), object()])
-            Traceback (most recent call last):
-            ...
-            ValueError: Vocabulary values may only contain primitive values.
-        
-        If a vocabulary name given, it is stored in ``vocabularyName``, and the ``vocabulary`` property returns ``None``::
-        
-            >>> f = field.Choice(title=u"Test", vocabulary='my.vocab')
-            >>> f.vocabulary is None
-            True
-        
-            >>> f.vocabularyName
-            'my.vocab'
-        
-        Other combinations are now allowed, such as specifying no vocabulary::
-        
-            >>> field.Choice(title=u"Test")
-            Traceback (most recent call last):
-            ...
-            AssertionError: You must specify either values or vocabulary.
-        
-        Or specifying both types::
-        
-            >>> field.Choice(title=u"Test", values=[1,2,3], vocabulary='my.vocab')
-            Traceback (most recent call last):
-            ...
-            AssertionError: You cannot specify both values and vocabulary.
-        
-        Or specifying an object source::
-        
-            >>> from zope.schema.vocabulary import SimpleVocabulary
-            >>> dummy_vocabulary = SimpleVocabulary.fromValues([1,2,3])
-            >>> field.Choice(title=u"Test", source=dummy_vocabulary)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields do not support sources, only named vocabularies or vocabularies based on simple value sets.
-        
-        Or specifying an object vocabulary::
-        
-            >>> field.Choice(title=u"Test", vocabulary=dummy_vocabulary)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields only support named vocabularies or vocabularies based on simple value sets.
-        
-        As with other fields, you also cannot set a constraint::
-        
-            >>> field.Choice(title=u"Test", values=[1,2,3], constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint('ABC')
-            True
-        
-        JSONField
-        ---------
-        
-        The set field describes a JSONField::
-        
-            >>> import plone.schema
-            >>> f = field.JSONField(title=u"Test")
-            >>> isinstance(f, plone.schema.JSONField)
-            True
-        
-            >>> f.order
-            -1
-        
-        ``IPersistentField`` adapters
-        =============================
-        
-        It is possible to adapt any non-persistent field to its related ``IPersistentField`` using the adapter factories in ``plone.registry`` fieldfactory.
-        These are set up in ``configure.zcml`` and explicitly registered in the test setup in ``tests.py``.
-        Custom adapters are of course also possible::
-        
-            >>> from plone.registry.interfaces import IPersistentField
-        
-            >>> f = schema.TextLine(title=u"Test")
-            >>> IPersistentField.providedBy(f)
-            False
-        
-            >>> p = IPersistentField(f)
-            >>> IPersistentField.providedBy(p)
-            True
-        
-            >>> isinstance(p, field.TextLine)
-            True
-        
-        Unsupported field types will not be adaptable by default::
-        
-            >>> f = schema.Object(title=u"Object", schema=IPersistentField)
-            >>> IPersistentField(f, None) is None
-            True
-        
-            >>> f = schema.InterfaceField(title=u"Interface")
-            >>> IPersistentField(f, None) is None
-            True
-        
-        After adaptation, the rules of persistent fields apply:
-        The ``order`` attribute is perpetually ``-1``.
-        Custom constraints are not allowed, and key and value type will be adapted to persistent fields as well.
-        If any of these constraints can not be met, the adaptation will fail.
-        
-        For constraints, the non-persistent value is simply ignored and the default method from the class will be used.
-        
-        ::
-        
-            >>> f = schema.TextLine(title=u"Test", constraint=lambda x: False)
-            >>> f.constraint
-            <function <lambda> at ...>
-        
-            >>> p = IPersistentField(f)
-            >>> p.constraint
-            <bound method TextLine.constraint of <plone.registry.field.TextLine object at ...>>
-        
-        The order property is similarly ignored::
-        
-            >>> f.order > 0
-            True
-        
-            >>> p.order
-            -1
-        
-        Key/value types will be adapted if possible::
-        
-            >>> f = schema.Dict(title=u"Test",
-            ...     key_type=schema.Id(title=u"Id"),
-            ...     value_type=schema.TextLine(title=u"Value"))
-            >>> p = IPersistentField(f)
-            >>> p.key_type
-            <plone.registry.field.Id object at ...>
-        
-            >>> p.value_type
-            <plone.registry.field.TextLine object at ...>
-        
-        If they cannot be adapted, there will be an error::
-        
-            >>> f = schema.Dict(title=u"Test",
-            ...     key_type=schema.Id(title=u"Id"),
-            ...     value_type=schema.Object(title=u"Value", schema=IPersistentField))
-            >>> p = IPersistentField(f)
-            Traceback (most recent call last):
-            ...
-            TypeError: ('Could not adapt', <zope.schema._field.Dict object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
-        
-            >>> f = schema.Dict(title=u"Test",
-            ...     key_type=schema.InterfaceField(title=u"Id"),
-            ...     value_type=schema.TextLine(title=u"Value"))
-            >>> p = IPersistentField(f)
-            Traceback (most recent call last):
-            ...
-            TypeError: ('Could not adapt', <zope.schema._field.Dict object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
-        
-        There is additional validation for choice fields that warrant a custom adapter.
-        These ensure that vocabularies are either stored as a list of simple values, or as named vocabularies.
-        
-        ::
-        
-            >>> f = schema.Choice(title=u"Test", values=[1,2,3])
-            >>> p = IPersistentField(f)
-            >>> p.vocabulary
-            <zope.schema.vocabulary.SimpleVocabulary object at ...>
-            >>> p._values
-            [1, 2, 3]
-            >>> p.vocabularyName is None
-            True
-        
-            >>> f = schema.Choice(title=u"Test", vocabulary='my.vocab')
-            >>> p = IPersistentField(f)
-            >>> p.vocabulary is None
-            True
-            >>> p._values is None
-            True
-            >>> p.vocabularyName
-            'my.vocab'
-        
-        Complex vocabularies or sources are not allowed::
-        
-            >>> from zope.schema.vocabulary import SimpleVocabulary
-            >>> dummy_vocabulary = SimpleVocabulary.fromItems([('a', 1), ('b', 2)])
-            >>> f = schema.Choice(title=u"Test", source=dummy_vocabulary)
-            >>> p = IPersistentField(f)
-            Traceback (most recent call last):
-            ...
-            TypeError: ('Could not adapt', <zope.schema._field.Choice object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
-        
-        
-            >>> f = schema.Choice(title=u"Test", vocabulary=dummy_vocabulary)
-            >>> p = IPersistentField(f)
-            Traceback (most recent call last):
-            ...
-            TypeError: ('Could not adapt', <zope.schema._field.Choice object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
-        
-        Changelog
-        =========
-        
-        .. You should *NOT* be adding new change log entries to this file.
-           You should create a file in the news directory instead.
-           For helpful instructions, please see:
-           https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
-        
-        .. towncrier release notes start
-        
-        1.2.1 (2021-06-14)
-        ------------------
-        
-        Bug fixes:
-        
-        
-        - Fix registry key validation regexp.
-          [jensens] (#23)
-        
-        
-        1.2.0 (2021-04-23)
-        ------------------
-        
-        New features:
-        
-        
-        - Allow plone.schema.JSONField be stored in registry (as dict-like)
-           [sneridagh] (#719)
-        
-        
-        1.1.6 (2020-04-22)
-        ------------------
-        
-        Bug fixes:
-        
-        
-        - Minor packaging updates. (#1)
-        
-        
-        1.1.5 (2018-12-14)
-        ------------------
-        
-        Bug fixes:
-        
-        - Avoid a deprecation warning that would turn into an error on Python 3.8.
-          [gforcada]
-        
-        
-        1.1.4 (2018-11-04)
-        ------------------
-        
-        Bug fixes:
-        
-        - Adapt test to changed object field in zope4
-          [pbauer]
-        
-        
-        1.1.3 (2018-06-22)
-        ------------------
-        
-        Bug fixes:
-        
-        - Improve performance of RecordsProxy.__iter__ which is now invoked more in
-          core Plone as part of the requireJS configuration
-          [MatthewWilkes]
-        
-        
-        1.1.2 (2016-12-06)
-        ------------------
-        
-        Bug fixes:
-        
-        - Fix tests to pass on Python 3.5
-          [datakurre]
-        
-        
-        1.1.1 (2016-11-19)
-        ------------------
-        
-        Bug fixes:
-        
-        - Fix endless recursion on getting values from broken records proxy objects
-          [tomgross]
-        
-        
-        1.1.0 (2016-07-05)
-        ------------------
-        
-        New features:
-        
-        - Give ``RecordsProxy`` a ``__parent__`` (the registry) in order to make it a good Zope citizen.
-          This helps in context of z3cform binders and other similar situations,
-          where a records proxy is used as context.
-          [jensens]
-        
-        
-        1.0.4 (2016-06-12)
-        ------------------
-        
-        Fixes:
-        
-        - More cleanup: PEP8, isort, readability.
-          [jensens]
-        
-        
-        1.0.3 (2016-02-26)
-        ------------------
-        
-        Fixes:
-        
-        - Replace deprecated ``zope.testing.doctestunit`` import with ``doctest``
-          module from stdlib.
-          [thet]
-        
-        - Cleanup: Pep8, utf8 headers, whitespace fixes, readability, ReST-fixes,
-          doc-style, etc.
-          [jensens]
-        
-        
-        1.0.2 (2014-09-11)
-        ------------------
-        
-        - Choice field construction compatible with a simple vocabulary of
-          string-based choices, which are converted to values on construction.
-          This provides compatibility for plone.registry/plone.app.registry
-          integration with plone.supermodel >= 1.2.5.
-          [seanupton]
-        
-        
-        1.0.1 (2013-01-13)
-        ------------------
-        
-        1.0 - 2011-05-13
-        ----------------
-        
-        - Release 1.0 Final
-          [esteele]
-        
-        - Add MANIFEST.in.
-          [WouterVH]
-        
-        
-        1.0b5 - 2011-04-06
-        ------------------
-        
-        - Make RecordsProxy type customizable through ``factory`` argument to
-          ``forInterface`` and ``collectionOfInterface``.
-          [elro]
-        
-        - Add ``collectionOfInterface`` support to registry.
-          [elro]
-        
-        - Fixed bug where prefix was ignored by registry.forInterface.
-          [elro]
-        
-        - Add optional min, max arguments for keys/values/items of _Records.
-          [elro]
-        
-        
-        1.0b4 - 2011-02-04
-        ------------------
-        
-        - Added support for field references, via the ``FieldRef`` class. See
-          ``registry.txt`` for details.
-          [optilude]
-        
-        - Change the internal persistent structure around to make it more efficient.
-          The API remains the same. Old registries will be migrated when first
-          accessed. Warning: This may lead to a "write-on-read" situation for the
-          first request in which the registry is being used.
-          [optilude]
-        
-        
-        1.0b3 - 2011-01-03
-        ------------------
-        
-         - Added prefix option to forInterface (as it was added to registerInterface)
-           [garbas]
-        
-        
-        1.0b2 - 2010-04-21
-        ------------------
-        
-        - Added support for Decimal fields
-          [optilude]
-        
-        - Add a prefix option to registerInterface to allow an interface to be used as
-          a template for a series of values, rather than single use.
-          [MatthewWilkes]
-        
-        
-        1.0b1 - 2009-08-02
-        ------------------
-        
-        - Fix a bug in bind() for Choice fields.
-          [optilude]
-        
-        
-        1.0a2 - 2009-07-12
-        ------------------
-        
-        - Changed API methods and arguments to mixedCase to be more consistent with
-          the rest of Zope. This is a non-backwards-compatible change. Our profuse
-          apologies, but it's now or never. :-/
-        
-          If you find that you get import errors or unknown keyword arguments in your
-          code, please change names from foo_bar too fooBar, e.g. for_interface()
-          becomes forInterface().
-          [optilude]
-        
-        
-        1.0a1 - 2009-04-17
-        ------------------
-        
-        - Initial release
-        
-        
 Keywords: configuration registry
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.1
-Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Provides-Extra: test
+
+============
+Introduction
+============
+This package provides debconf-like (or about:config-like) settings registries
+for Zope applications. A ``registry``, with a dict-like API, is used to get and
+set values stored in ``records``. Each record contains the actual value, as
+well as a ``field`` that describes the record in more detail. At a minimum, the
+field contains information about the type of value allowed, as well as a short
+title describing the record's purpose.
+
+.. contents:: Table of Contents
+
+
+================
+Using registries
+================
+
+You can create a new registry simply by instantiating the Registry class.
+The class and its data structures are persistent, so you can store them in the ZODB.
+You may want to provide the registry object as local utility for easy access as well, though we won't do that here.
+
+::
+
+    >>> from plone.registry import Registry
+    >>> registry = Registry()
+
+The registry starts out empty.
+To access the registry's records, you can use the ``records`` property.
+This exposes a dict API where keys are strings and values are objects providing ``IRecords``.
+
+::
+
+    >>> len(registry.records)
+    0
+
+Simple records
+==============
+
+Let's now create a record.
+A record must have a name.
+This should be a dotted name, and contain ASCII characters only.
+By convention, it should be all lowercase and start with the name of the package that defines the record.
+
+It is also possible to create a  number of records based on a single schema interface - see below.
+For now, we will focus on simple records.
+
+Before we can create the record, we must create the field that describes it.
+Fields are based on the venerable ``zope.schema`` package.
+``plone.registry`` only supports certain fields, and disallows use of a few properties even of those.
+As a rule of thumb, so long as a field stores a Python primitive, it is supported; the same goes for attributes of fields.
+
+Thus:
+
+* Fields like ``Object``, ``InterfaceField`` and so on are *not* supported.
+* A custom ``constraint`` method is *not* supported.
+* The ``order`` attribute will *always* be set to ``-1``.
+* For Choice fields, *only named vocabularies* are supported:
+  you can *not* reference a particular *source* or *source binder*.
+* The ``key_type`` and ``value_type`` properties of ``Dict``, ``List``, ``Tuple``, ``Set`` and ``Frozenset`` may *only* contain persistent fields.
+
+See section "Persistent fields" for more details.
+
+Creating a record
+-----------------
+
+The supported field types are found in the module ``plone.registry.field``.
+These are named the same as the equivalent field in ``zope.schema``, and have the same constructors.
+You must use one of these fields when creating records directly::
+
+    >>> from plone.registry import field
+    >>> age_field = field.Int(title=u"Age", min=0, default=18)
+
+    >>> from plone.registry import Record
+    >>> age_record = Record(age_field)
+
+Note that in this case, we did not supply a value.
+The value will therefore be the field default::
+
+    >>> age_record.value
+    18
+
+We can set a different value, either in the ``Record`` constructor or via the ``value`` attribute::
+
+    >>> age_record.value = 2
+    >>> age_record.value
+    2
+
+Note that the value is validated against the field::
+
+    >>> age_record.value = -1
+    Traceback (most recent call last):
+    ...
+    zope.schema._bootstrapinterfaces.TooSmall: (-1, 0)
+
+    >>> age_record.value
+    2
+
+We can now add the field to the registry.
+This is done via the ``record`` dictionary::
+
+    >>> 'plone.registry.tests.age' in registry
+    False
+    >>> registry.records['plone.registry.tests.age'] = age_record
+
+At this point, the record will gain ``__name__`` and ``__parent__`` attributes::
+
+    >>> age_record.__name__
+    'plone.registry.tests.age'
+
+    >>> age_record.__parent__ is registry
+    True
+
+Creating a record with an initial value
+---------------------------------------
+
+We can create records more succinctly in *one go* by
+
+1. creating the field,
+2. creating the Record and setting its value as and
+3. assigning it to the registry,
+
+like this::
+
+    >>> registry.records['plone.registry.tests.cms'] = \
+    ...     Record(field.TextLine(title=u"CMS of choice"), u"Plone")
+
+The record can now be obtained.
+Note that it has a nice ``__repr__`` to help debugging.
+
+    >>> registry.records['plone.registry.tests.cms']
+    <Record plone.registry.tests.cms>
+
+Accessing and manipulating record values
+----------------------------------------
+
+Once a record has been created and added to the registry,
+you can access its value through dict-like operations on the registry itself::
+
+    >>> 'plone.registry.tests.cms' in registry
+    True
+
+    >>> registry['plone.registry.tests.cms']  # doctest: +IGNORE_U
+    u'Plone'
+
+    >>> registry['plone.registry.tests.cms'] = u"Plone 3.x"
+
+Again, values are validated::
+
+    >>> registry['plone.registry.tests.cms'] = b'Joomla'
+    Traceback (most recent call last):
+    ...
+    zope.schema._bootstrapinterfaces.WrongType: (b'Joomla', <class 'str'>, 'value')
+
+There is also a ``get()`` method::
+
+    >>> registry.get('plone.registry.tests.cms')  # doctest: +IGNORE_U
+    u'Plone 3.x'
+    >>> registry.get('non-existent-key') is None
+    True
+
+Deleting records
+----------------
+
+Records may be deleted from the ``records`` property::
+
+    >>> del registry.records['plone.registry.tests.cms']
+    >>> 'plone.registry.tests.cms' in registry.records
+    False
+    >>> 'plone.registry.tests.cms' in registry
+    False
+
+Creating records from interfaces
+================================
+
+As an application developer, it is often desirable to define settings as traditional interfaces with ``zope.schema fields``.
+``plone.registry`` includes support for creating a set of records from a single interface.
+
+To test this, we have created an interface, ``IMailSettings``.
+It has two fields: ``sender`` and ``smtp_host``::
+
+    >>> from plone.registry.tests import IMailSettings
+
+Note that this contains standard fields::
+
+    >>> IMailSettings['sender']
+    <zope.schema._bootstrapfields.TextLine object at ...>
+
+    >>> IMailSettings['smtp_host']
+    <zope.schema._field.URI object at ...>
+
+We can create records from this interface like this::
+
+    >>> registry.registerInterface(IMailSettings)
+
+One record for each field in the interface has now been created.
+Their names are the full dotted names to those fields::
+
+    >>> sender_record = registry.records['plone.registry.tests.IMailSettings.sender']
+    >>> smtp_host_record = registry.records['plone.registry.tests.IMailSettings.smtp_host']
+
+The fields used in the records will be the equivalent persistent versions of the fields from the original interface::
+
+    >>> sender_record.field
+    <plone.registry.field.TextLine object at ...>
+
+    >>> smtp_host_record.field
+    <plone.registry.field.URI object at ...>
+
+This feat is accomplished internally by adapting the field to the ``IPersistentField`` interface.
+There is a default adapter factory that works for all fields defined in ``plone.registry.field``.
+You can of course define your own adapter if you have a custom field type.
+But bear in mind the golden rules of any persistent field::
+
+* The field must store only primitives or other persistent fields
+* It must not reference a function, class, interface or other method that could break if a package is uninstalled.
+
+If we have a field for which there is no ``IPersistentField`` adapter, we will get an error::
+
+    >>> from plone.registry.tests import IMailPreferences
+    >>> IMailPreferences['settings']
+    <zope.schema._bootstrapfields.Object object at ...>
+
+    >>> registry.registerInterface(IMailPreferences)
+    Traceback (most recent call last):
+    ...
+    TypeError: There is no persistent field equivalent for the field `settings` of type `Object`.
+
+Whoops!
+We can, however, tell ``registerInterface()`` to ignore one or more fields::
+
+    >>> registry.registerInterface(IMailPreferences, omit=('settings',))
+
+Once an interface's records have been registered, we can get and set their values as normal::
+
+    >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
+    u'root@localhost'
+
+    >>> registry['plone.registry.tests.IMailSettings.sender'] = u"webmaster@localhost"
+    >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
+    u'webmaster@localhost'
+
+If we sub-sequently re-register the same interface, the value will be retained if possible::
+
+    >>> registry.registerInterface(IMailSettings)
+    >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
+    u'webmaster@localhost'
+
+However, if the value is no longer valid, we will revert to the default.
+To test that, let's sneakily modify the field for a while::
+
+    >>> old_field = IMailSettings['sender']
+    >>> IMailSettings._InterfaceClass__attrs['sender'] = field.Int(title=u"Definitely not a string", default=2)
+    >>> if hasattr(IMailSettings, '_v_attrs'):
+    ...     del IMailSettings._v_attrs['sender']
+    >>> registry.registerInterface(IMailSettings)
+    >>> registry['plone.registry.tests.IMailSettings.sender']
+    2
+
+But let's put it back the way it was::
+
+    >>> IMailSettings._InterfaceClass__attrs['sender'] = old_field
+    >>> if hasattr(IMailSettings, '_v_attrs'):
+    ...     del IMailSettings._v_attrs['sender']
+    >>> registry.registerInterface(IMailSettings)
+    >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
+    u'root@localhost'
+
+Sometimes, you may want to use an interface as a template for multiple instances of a set of fields, rather than defining them all by hand.
+This is especially useful when you want to allow third-party packages to provide information.
+To accomplish this, we can provide a prefix with the ``registerInterface`` call.
+This will take precedence over the ``__identifier__`` that is usually used.
+
+    >>> registry.registerInterface(IMailSettings, prefix="plone.registry.tests.alternativesettings")
+
+These values are now available in the same way as the original settings::
+
+    >>> sender_record = registry.records['plone.registry.tests.alternativesettings.sender']
+    >>> smtp_host_record = registry.records['plone.registry.tests.alternativesettings.smtp_host']
+    >>> registry['plone.registry.tests.alternativesettings.sender'] = u'alt@example.org'
+
+Accessing the original interface
+--------------------------------
+
+Now that we have these records, we can look up the original interface.
+This does not break the golden rules:
+internally, we only store the name of the interface, and resolve it at runtime.
+
+Records that know about interfaces are marked with ``IInterfaceAwareRecord`` and have two additional properties:
+``interface`` and ``fieldName``::
+
+    >>> from plone.registry.interfaces import IInterfaceAwareRecord
+    >>> IInterfaceAwareRecord.providedBy(age_record)
+    False
+    >>> IInterfaceAwareRecord.providedBy(sender_record)
+    True
+
+    >>> sender_record.interfaceName
+    'plone.registry.tests.IMailSettings'
+
+    >>> sender_record.interface is IMailSettings
+    True
+
+Using the records proxy
+-----------------------
+
+Once the records for an interface has been created, it is possible to obtain a proxy object that provides the given interface, but reads and writes its values to the registry.
+This is useful, for example, to create a form using ``zope.formlib`` or  ``z3c.form`` that is configured with widgets based on the
+interface.
+Or simply as a more convenient API when working with multiple, related settings.
+
+::
+
+    >>> proxy = registry.forInterface(IMailSettings)
+    >>> proxy
+    <RecordsProxy for plone.registry.tests.IMailSettings>
+
+If you use your registry values in code which might be encountered on normal HTML rendering paths (e.g. in a viewlet) you need to be aware that records might not exist or they are invalid.
+``forInterface()`` will raise KeyError on this kind of situations::
+
+    try:
+        proxy = registry.forInterface(IMailSettings)
+    except KeyError:
+        # Gracefully handled cases
+        # when GenericSetup installer has not been run or rerun
+        # e.g. by returning or using some default values
+        pass
+
+The proxy is not a persistent object on its own::
+
+    >>> from persistent.interfaces import IPersistent
+    >>> IPersistent.providedBy(proxy)
+    False
+
+It does, however, provide the requisite interface::
+
+    >>> IMailSettings.providedBy(proxy)
+    True
+
+You can distinguish between the proxy and a 'normal' object by checking for the ``IRecordsProxy`` marker interface::
+
+    >>> from plone.registry.interfaces import IRecordsProxy
+    >>> IRecordsProxy.providedBy(proxy)
+    True
+
+When we set a value, it is stored in the registry::
+
+    >>> proxy.smtp_host = 'http://mail.server.com'
+    >>> registry['plone.registry.tests.IMailSettings.smtp_host']
+    'http://mail.server.com'
+
+    >>> registry['plone.registry.tests.IMailSettings.smtp_host'] = 'smtp://mail.server.com'
+    >>> proxy.smtp_host
+    'smtp://mail.server.com'
+
+Values not in the interface will raise an ``AttributeError``::
+
+    >>> proxy.age
+    Traceback (most recent call last):
+    ...
+    AttributeError: age
+
+Note that by default, the forInterface() method will check that the necessary records have been registered.
+For example, we cannot use any old interface::
+
+    >>> registry.forInterface(IInterfaceAwareRecord)
+    Traceback (most recent call last):
+    ...
+    KeyError: 'Interface `plone.registry.interfaces.IInterfaceAwareRecord` defines a field `...`, for which there is no record.'
+
+By default, we also cannot use an interface for which only some records exist::
+
+    >>> registry.forInterface(IMailPreferences)
+    Traceback (most recent call last):
+    ...
+    KeyError: 'Interface `plone.registry.tests.IMailPreferences` defines a field `settings`, for which there is no record.'
+
+It is possible to disable this check, however.
+This will be a bit more efficient::
+
+    >>> registry.forInterface(IMailPreferences, check=False)
+    <RecordsProxy for plone.registry.tests.IMailPreferences>
+
+A better way, however, is to explicitly declare that some fields are omitted::
+
+    >>> pref_proxy = registry.forInterface(IMailPreferences, omit=('settings',))
+
+In this case, the omitted fields will default to their 'missing' value::
+
+    >>> pref_proxy.settings ==  IMailPreferences['settings'].missing_value
+    True
+
+However, trying to set the value will result in a ``AttributeError``::
+
+    >>> pref_proxy.settings = None
+    Traceback (most recent call last):
+    ...
+    AttributeError: settings
+
+To access another instance of the field, supply the prefix::
+
+    >>> alt_proxy = registry.forInterface(IMailSettings,
+    ...     prefix="plone.registry.tests.alternativesettings")
+    >>> alt_proxy.sender  # doctest: +IGNORE_U
+    u'alt@example.org'
+
+Collections of records proxies
+------------------------------
+
+A collection of record sets may be accessed using ``collectionOfInterface``::
+
+    >>> collection = registry.collectionOfInterface(IMailSettings)
+
+You can create a new record set::
+
+    >>> proxy = collection.setdefault('example')
+    >>> proxy.sender = u'collection@example.org'
+    >>> proxy.smtp_host = 'smtp://mail.example.org'
+
+Record sets are stored based under the prefix::
+
+    >>> prefix = IMailSettings.__identifier__
+    >>> registry.records.values(prefix+'/', prefix+'0')
+    [<Record plone.registry.tests.IMailSettings/example.sender>,
+     <Record plone.registry.tests.IMailSettings/example.smtp_host>]
+    >>> registry['plone.registry.tests.IMailSettings/example.sender']  # doctest: +IGNORE_U
+    u'collection@example.org'
+
+Records may be set from an existing object::
+
+    >>> class MailSettings:
+    ...     sender = u'someone@example.com'
+    ...     smtp_host = 'smtp://mail.example.com'
+    >>> collection['example_com'] = MailSettings()
+    >>> registry.records.values(prefix+'/', prefix+'0')
+    [<Record plone.registry.tests.IMailSettings/example.sender>,
+     <Record plone.registry.tests.IMailSettings/example.smtp_host>,
+     <Record plone.registry.tests.IMailSettings/example_com.sender>,
+     <Record plone.registry.tests.IMailSettings/example_com.smtp_host>]
+
+The collection may be iterated over::
+
+    >>> for name in collection: print(name)
+    example
+    example_com
+
+And may be deleted::
+
+    >>> del collection['example_com']
+    >>> registry.records.values(prefix+'/', prefix+'0')
+    [<Record plone.registry.tests.IMailSettings/example.sender>,
+     <Record plone.registry.tests.IMailSettings/example.smtp_host>]
+
+Using field references
+======================
+
+It is possible for one record to refer to another record's field.
+This can be used to provide a simple "override" mechanism,
+for example, where one record defines the field and a default value,
+whilst another provides an override validated against the same field.
+
+Let us first create the base record and set its value::
+
+    >>> timeout_field = field.Int(title=u"Timeout", min=0)
+    >>> registry.records['plone.registry.tests.timeout'] = Record(timeout_field, 10)
+
+    >>> timeout_record = registry.records['plone.registry.tests.timeout']
+    >>> timeout_record.value
+    10
+
+Next, we create a field reference for this record::
+
+    >>> from plone.registry import FieldRef
+    >>> timeout_override_field = FieldRef(timeout_record.__name__, timeout_record.field)
+
+We can use this to create a new record::
+
+    >>> registry.records['plone.registry.tests.timeout.override'] = Record(timeout_override_field, 20)
+    >>> timeout_override_record = registry.records['plone.registry.tests.timeout.override']
+
+The two values are separate::
+
+    >>> timeout_record.value
+    10
+    >>> timeout_override_record.value
+    20
+
+    >>> registry['plone.registry.tests.timeout']
+    10
+    >>> registry['plone.registry.tests.timeout.override']
+    20
+
+Validation uses the underlying field::
+
+    >>> registry['plone.registry.tests.timeout.override'] = -1
+    Traceback (most recent call last):
+    ...
+    zope.schema._bootstrapinterfaces.TooSmall: (-1, 0)
+
+The reference field exposes the standard field properties, e.g.::
+
+    >>> timeout_override_record.field.title
+    'Timeout'
+    >>> timeout_override_record.field.min
+    0
+
+To look up the underlying record name, we can use the ``recordName`` property::
+
+    >>> timeout_override_record.field.recordName
+    'plone.registry.tests.timeout'
+
+
+===============
+Registry events
+===============
+
+The registry fires certain events. These are:
+
+``plone.registry.interfaces.IRecordAddedEvent``
+    when a record has been added to the registry.
+
+``plone.registry.interfaces.IRecordRemovedEvent``
+    when a record has been removed from the registry.
+
+``plone.registry.interfaces.IRecordModifiedEvent``,
+    when a record's value is modified.
+
+To test these events, we will create, modify and remove a few records::
+
+    >>> from zope.component.eventtesting import clearEvents
+    >>> clearEvents()
+    >>> from plone.registry import Registry, Record, field
+    >>> registry = Registry()
+
+Adding a new record to the registry should fire ``IRecordAddedEvents``::
+
+    >>> registry.records['plone.registry.tests.age'] = \
+    ...     Record(field.Int(title=u"Age", min=0, default=18))
+
+    >>> registry.records['plone.registry.tests.cms'] = \
+    ...     Record(field.TextLine(title=u"Preferred CMS"), value=u"Plone")
+
+When creating records from an interface, one event is fired for each field in the interface::
+
+    >>> from plone.registry.tests import IMailSettings
+    >>> registry.registerInterface(IMailSettings)
+
+Deleting a record should fire an ``IRecordRemovedEvent``::
+
+    >>> del registry.records['plone.registry.tests.cms']
+
+Changing a record should fire an ``IRecordModifiedEvent``::
+
+    >>> registry['plone.registry.tests.age'] = 25
+    >>> registry.records['plone.registry.tests.age'].value = 24
+
+Let's take a look at the events that were just fired::
+
+    >>> from plone.registry.interfaces import IRecordEvent
+    >>> from zope.component.eventtesting import getEvents
+    >>> getEvents(IRecordEvent)
+    [<RecordAddedEvent for plone.registry.tests.age>,
+     <RecordAddedEvent for plone.registry.tests.cms>,
+     <RecordAddedEvent for plone.registry.tests.IMailSettings.sender>,
+     <RecordAddedEvent for plone.registry.tests.IMailSettings.smtp_host>,
+     <RecordRemovedEvent for plone.registry.tests.cms>,
+     <RecordModifiedEvent for plone.registry.tests.age>,
+     <RecordModifiedEvent for plone.registry.tests.age>]
+
+For the modified events, we can also check the value before and after the change::
+
+    >>> from plone.registry.interfaces import IRecordModifiedEvent
+    >>> [(repr(e), e.oldValue, e.newValue,) for e in getEvents(IRecordModifiedEvent)]
+    [('<RecordModifiedEvent for plone.registry.tests.age>', 18, 25),
+     ('<RecordModifiedEvent for plone.registry.tests.age>', 25, 24)]
+
+IObjectEvent-style redispatchers
+================================
+
+There is a special event handler.
+It takes care of re-dispatching registry events based on the schema interface prescribed by the record.
+
+Let's re-set the event testing framework and register the re-dispatching event subscriber.
+Normally, this would happen automatically by including this package's ZCML.
+
+::
+
+    >>> clearEvents()
+    >>> from zope.component import provideHandler
+    >>> from plone.registry.events import redispatchInterfaceAwareRecordEvents
+    >>> provideHandler(redispatchInterfaceAwareRecordEvents)
+
+We'll then register a schema interface::
+
+    >>> from plone.registry.tests import IMailSettings
+    >>> registry.registerInterface(IMailSettings)
+
+We could now register an event handler to print any record event occurring on an ``IMailSettings`` record.
+More specialised event handlers for e.g. ``IRecordModifiedEvent`` or ``IRecordRemovedEvent`` are of course also possible.
+Note that it is not possible to re-dispatch ``IRecordAddedEvents``, so these are never caught.
+
+    >>> from zope.component import adapter
+    >>> @adapter(IMailSettings, IRecordEvent)
+    ... def print_mail_settings_events(proxy, event):
+    ...     print("Got %s for %s" % (event, proxy))
+    >>> provideHandler(print_mail_settings_events)
+
+Let's now modify one of the records for this interface.
+The event handler should react immediately::
+
+    >>> registry['plone.registry.tests.IMailSettings.sender'] = u"Some sender"
+    Got <RecordModifiedEvent for plone.registry.tests.IMailSettings.sender> for <RecordsProxy for plone.registry.tests.IMailSettings>
+
+Let's also modify a non-interface-aware record, for comparison's sake.
+Here, there is nothing printed::
+
+    >>> registry['plone.registry.tests.age'] = 3
+
+We can try a record-removed event as well::
+
+    >>> del registry.records['plone.registry.tests.IMailSettings.sender']
+    Got <RecordRemovedEvent for plone.registry.tests.IMailSettings.sender> for <RecordsProxy for plone.registry.tests.IMailSettings>
+
+The basic events that have been dispatched are::
+
+    >>> getEvents(IRecordEvent)
+    [<RecordAddedEvent for plone.registry.tests.IMailSettings.sender>,
+     <RecordAddedEvent for plone.registry.tests.IMailSettings.smtp_host>,
+     <RecordModifiedEvent for plone.registry.tests.IMailSettings.sender>,
+     <RecordModifiedEvent for plone.registry.tests.age>,
+     <RecordRemovedEvent for plone.registry.tests.IMailSettings.sender>]
+
+
+=================
+Persistent fields
+=================
+
+The persistent fields that are found in ``plone.registry.field`` are siblings of the ones found in zope.schema,
+with persistence mixed in.
+To avoid potentially breaking the registry with persistent references to symbols that may go away,
+we purposefully limit the number of fields supported.
+We also disallow some properties, and add some additional checks on others.
+
+The standard fields
+===================
+
+We will show each supported field in turn. For all fields, note that:
+
+* the ``order`` property will return ``-1`` no matter what setting the ``constraint`` property is diallowed
+* the ``key_type`` and ``value_type`` properties, where applicable, must be set to a persistent field.
+* for ``Choice`` fields, only named vocabularies and vocabularies based on simple values are supported:
+  sources and ``IVocabulary`` objects are not.
+
+Imports needed::
+
+    >>> from plone.registry import field
+    >>> from zope import schema
+    >>> from persistent import Persistent
+
+Bytes
+-----
+
+The bytes field describes a string of bytes::
+
+    >>> f = field.Bytes(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.Bytes)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Bytes(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint('ABC')
+    True
+
+BytesLine
+---------
+
+The bytes field describes a string of bytes, disallowing newlines::
+
+    >>> f = field.BytesLine(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.BytesLine)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.BytesLine(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(b'AB\nC')
+    False
+
+ASCII
+-----
+
+The ASCII field describes a string containing only ASCII characters::
+
+    >>> f = field.ASCII(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.ASCII)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.ASCII(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint('ab\nc')
+    True
+
+ASCIILine
+---------
+
+The ASCII line field describes a string containing only ASCII characters and disallowing newlines::
+
+    >>> f = field.ASCIILine(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.ASCIILine)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.ASCIILine(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint('ab\nc')
+    False
+
+Text
+----
+
+The text field describes a unicode string::
+
+    >>> f = field.Text(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.Text)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Text(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'ab\nc')
+    True
+
+TextLine
+--------
+
+The text line field describes a unicode string, disallowing newlines::
+
+    >>> f = field.TextLine(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.TextLine)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.TextLine(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'ab\nc')
+    False
+
+Bool
+----
+
+The bool field describes a boolean::
+
+    >>> f = field.Bool(title=u"Test")
+    >>> isinstance(f, schema.Bool)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Bool(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(False)
+    True
+
+Int
+---
+
+The int field describes an integer or long::
+
+    >>> f = field.Int(title=u"Test", min=-123, max=1234)
+    >>> isinstance(f, schema.Int)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Int(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(123)
+    True
+
+Float
+-----
+
+The float field describes a float::
+
+    >>> f = field.Float(title=u"Test", min=-123.0, max=1234.0)
+    >>> isinstance(f, schema.Float)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Float(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(123)
+    True
+
+Decimal
+-------
+
+The decimal field describes a decimal::
+
+    >>> import decimal
+    >>> f = field.Decimal(title=u"Test", min=decimal.Decimal('-123.0'), max=decimal.Decimal('1234.0'))
+    >>> isinstance(f, schema.Decimal)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Decimal(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(123)
+    True
+
+Password
+--------
+
+The password field describes a unicode string used for a password::
+
+    >>> f = field.Password(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.Password)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Password(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'ab\nc')
+    False
+
+SourceText
+----------
+
+The source  text field describes a unicode string with source code::
+
+    >>> f = field.SourceText(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.SourceText)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.SourceText(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'ab\nc')
+    True
+
+URI
+---
+
+The URI field describes a URI string::
+
+    >>> f = field.URI(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.URI)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.URI(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'abc')
+    True
+
+Id
+--
+
+The id field describes a URI string or a dotted name::
+
+    >>> f = field.Id(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.Id)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Id(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'abc')
+    True
+
+DottedName
+----------
+
+The dotted name field describes a Python dotted name::
+
+    >>> f = field.DottedName(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.DottedName)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.DottedName(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'abc')
+    True
+
+Datetime
+--------
+
+The date/time field describes a Python datetime object::
+
+    >>> f = field.Datetime(title=u"Test")
+    >>> isinstance(f, schema.Datetime)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Datetime(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> import datetime
+    >>> f.constraint(datetime.datetime.now())
+    True
+
+Date
+----
+
+The date field describes a Python date object::
+
+    >>> f = field.Date(title=u"Test")
+    >>> isinstance(f, schema.Date)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Date(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> import datetime
+    >>> f.constraint(datetime.date.today())
+    True
+
+Timedelta
+---------
+
+The time-delta field describes a Python timedelta object::
+
+    >>> f = field.Timedelta(title=u"Test")
+    >>> isinstance(f, schema.Timedelta)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Timedelta(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> import datetime
+    >>> f.constraint(datetime.timedelta(1))
+    True
+
+Tuple
+-----
+
+The tuple field describes a tuple::
+
+    >>> f = field.Tuple(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=field.TextLine(title=u"Value"))
+    >>> isinstance(f, schema.Tuple)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Tuple(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=schema.TextLine(title=u"Value"))
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> f.value_type = schema.TextLine(title=u"Value")
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> field.Tuple(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint((1,2))
+    True
+
+List
+----
+
+The list field describes a tuple::
+
+    >>> f = field.List(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=field.TextLine(title=u"Value"))
+    >>> isinstance(f, schema.List)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.List(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=schema.TextLine(title=u"Value"))
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> f.value_type = schema.TextLine(title=u"Value")
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> field.List(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint([1,2])
+    True
+
+Set
+---
+
+The set field describes a set::
+
+    >>> f = field.Set(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=field.TextLine(title=u"Value"))
+    >>> isinstance(f, schema.Set)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Set(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=schema.TextLine(title=u"Value"))
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> f.value_type = schema.TextLine(title=u"Value")
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> field.Set(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(set([1,2]))
+    True
+
+Frozenset
+---------
+
+The set field describes a frozenset::
+
+    >>> f = field.FrozenSet(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=field.TextLine(title=u"Value"))
+    >>> isinstance(f, schema.FrozenSet)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.FrozenSet(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=schema.TextLine(title=u"Value"))
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> f.value_type = schema.TextLine(title=u"Value")
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> field.FrozenSet(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(frozenset([1,2]))
+    True
+
+Dict
+----
+
+The set field describes a dict::
+
+    >>> f = field.Dict(title=u"Test", min_length=0, max_length=10,
+    ...     key_type=field.ASCII(title=u"Key"),
+    ...     value_type=field.TextLine(title=u"Value"))
+    >>> isinstance(f, schema.Dict)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Dict(title=u"Test", min_length=0, max_length=10,
+    ...     key_type=schema.ASCII(title=u"Key"),
+    ...     value_type=field.TextLine(title=u"Value"))
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `key_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> f.key_type = schema.ASCII(title=u"Key")
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `key_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> field.Dict(title=u"Test", min_length=0, max_length=10,
+    ...     key_type=field.ASCII(title=u"Key"),
+    ...     value_type=schema.TextLine(title=u"Value"))
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> f.value_type = schema.TextLine(title=u"Value")
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> field.Dict(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(dict())
+    True
+
+Choice
+------
+
+A choice field represents a selection from a vocabulary.
+For persistent fields, the vocabulary cannot be a ``source`` or any kind of object:
+it must either be a list of primitives, or a named vocabulary::
+
+    >>> f = field.Choice(title=u"Test", values=[1,2,3])
+    >>> isinstance(f, schema.Choice)
+    True
+
+    >>> f.order
+    -1
+
+With a list of values given, the ``vocabulary`` property returns a vocabulary
+constructed from the values on the fly, and ``vocabularyName`` is ``None``::
+
+    >>> f.vocabulary
+    <zope.schema.vocabulary.SimpleVocabulary object at ...>
+
+    >>> f.vocabularyName is None
+    True
+
+We will get an error if we use anything other than primitives::
+
+    >>> f = field.Choice(title=u"Test", values=[object(), object()])
+    Traceback (most recent call last):
+    ...
+    ValueError: Vocabulary values may only contain primitive values.
+
+If a vocabulary name given, it is stored in ``vocabularyName``, and the ``vocabulary`` property returns ``None``::
+
+    >>> f = field.Choice(title=u"Test", vocabulary='my.vocab')
+    >>> f.vocabulary is None
+    True
+
+    >>> f.vocabularyName
+    'my.vocab'
+
+Other combinations are now allowed, such as specifying no vocabulary::
+
+    >>> field.Choice(title=u"Test")
+    Traceback (most recent call last):
+    ...
+    AssertionError: You must specify either values or vocabulary.
+
+Or specifying both types::
+
+    >>> field.Choice(title=u"Test", values=[1,2,3], vocabulary='my.vocab')
+    Traceback (most recent call last):
+    ...
+    AssertionError: You cannot specify both values and vocabulary.
+
+Or specifying an object source::
+
+    >>> from zope.schema.vocabulary import SimpleVocabulary
+    >>> dummy_vocabulary = SimpleVocabulary.fromValues([1,2,3])
+    >>> field.Choice(title=u"Test", source=dummy_vocabulary)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields do not support sources, only named vocabularies or vocabularies based on simple value sets.
+
+Or specifying an object vocabulary::
+
+    >>> field.Choice(title=u"Test", vocabulary=dummy_vocabulary)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields only support named vocabularies or vocabularies based on simple value sets.
+
+As with other fields, you also cannot set a constraint::
+
+    >>> field.Choice(title=u"Test", values=[1,2,3], constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint('ABC')
+    True
+
+JSONField
+---------
+
+The set field describes a JSONField::
+
+    >>> import plone.schema
+    >>> f = field.JSONField(title=u"Test")
+    >>> isinstance(f, plone.schema.JSONField)
+    True
+
+    >>> f.order
+    -1
+
+``IPersistentField`` adapters
+=============================
+
+It is possible to adapt any non-persistent field to its related ``IPersistentField`` using the adapter factories in ``plone.registry`` fieldfactory.
+These are set up in ``configure.zcml`` and explicitly registered in the test setup in ``tests.py``.
+Custom adapters are of course also possible::
+
+    >>> from plone.registry.interfaces import IPersistentField
+
+    >>> f = schema.TextLine(title=u"Test")
+    >>> IPersistentField.providedBy(f)
+    False
+
+    >>> p = IPersistentField(f)
+    >>> IPersistentField.providedBy(p)
+    True
+
+    >>> isinstance(p, field.TextLine)
+    True
+
+Unsupported field types will not be adaptable by default::
+
+    >>> f = schema.Object(title=u"Object", schema=IPersistentField)
+    >>> IPersistentField(f, None) is None
+    True
+
+    >>> f = schema.InterfaceField(title=u"Interface")
+    >>> IPersistentField(f, None) is None
+    True
+
+After adaptation, the rules of persistent fields apply:
+The ``order`` attribute is perpetually ``-1``.
+Custom constraints are not allowed, and key and value type will be adapted to persistent fields as well.
+If any of these constraints can not be met, the adaptation will fail.
+
+For constraints, the non-persistent value is simply ignored and the default method from the class will be used.
+
+::
+
+    >>> f = schema.TextLine(title=u"Test", constraint=lambda x: False)
+    >>> f.constraint
+    <function <lambda> at ...>
+
+    >>> p = IPersistentField(f)
+    >>> p.constraint
+    <bound method TextLine.constraint of <plone.registry.field.TextLine object at ...>>
+
+The order property is similarly ignored::
+
+    >>> f.order > 0
+    True
+
+    >>> p.order
+    -1
+
+Key/value types will be adapted if possible::
+
+    >>> f = schema.Dict(title=u"Test",
+    ...     key_type=schema.Id(title=u"Id"),
+    ...     value_type=schema.TextLine(title=u"Value"))
+    >>> p = IPersistentField(f)
+    >>> p.key_type
+    <plone.registry.field.Id object at ...>
+
+    >>> p.value_type
+    <plone.registry.field.TextLine object at ...>
+
+If they cannot be adapted, there will be an error::
+
+    >>> f = schema.Dict(title=u"Test",
+    ...     key_type=schema.Id(title=u"Id"),
+    ...     value_type=schema.Object(title=u"Value", schema=IPersistentField))
+    >>> p = IPersistentField(f)
+    Traceback (most recent call last):
+    ...
+    TypeError: ('Could not adapt', <zope.schema._field.Dict object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
+
+    >>> f = schema.Dict(title=u"Test",
+    ...     key_type=schema.InterfaceField(title=u"Id"),
+    ...     value_type=schema.TextLine(title=u"Value"))
+    >>> p = IPersistentField(f)
+    Traceback (most recent call last):
+    ...
+    TypeError: ('Could not adapt', <zope.schema._field.Dict object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
+
+There is additional validation for choice fields that warrant a custom adapter.
+These ensure that vocabularies are either stored as a list of simple values, or as named vocabularies.
+
+::
+
+    >>> f = schema.Choice(title=u"Test", values=[1,2,3])
+    >>> p = IPersistentField(f)
+    >>> p.vocabulary
+    <zope.schema.vocabulary.SimpleVocabulary object at ...>
+    >>> p._values
+    [1, 2, 3]
+    >>> p.vocabularyName is None
+    True
+
+    >>> f = schema.Choice(title=u"Test", vocabulary='my.vocab')
+    >>> p = IPersistentField(f)
+    >>> p.vocabulary is None
+    True
+    >>> p._values is None
+    True
+    >>> p.vocabularyName
+    'my.vocab'
+
+Complex vocabularies or sources are not allowed::
+
+    >>> from zope.schema.vocabulary import SimpleVocabulary
+    >>> dummy_vocabulary = SimpleVocabulary.fromItems([('a', 1), ('b', 2)])
+    >>> f = schema.Choice(title=u"Test", source=dummy_vocabulary)
+    >>> p = IPersistentField(f)
+    Traceback (most recent call last):
+    ...
+    TypeError: ('Could not adapt', <zope.schema._field.Choice object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
+
+
+    >>> f = schema.Choice(title=u"Test", vocabulary=dummy_vocabulary)
+    >>> p = IPersistentField(f)
+    Traceback (most recent call last):
+    ...
+    TypeError: ('Could not adapt', <zope.schema._field.Choice object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
+
+Changelog
+=========
+
+.. You should *NOT* be adding new change log entries to this file.
+   You should create a file in the news directory instead.
+   For helpful instructions, please see:
+   https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
+
+.. towncrier release notes start
+
+2.0.0 (2023-04-26)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 compatibility.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (a864b30f)
+
+
+1.2.1 (2021-06-14)
+------------------
+
+Bug fixes:
+
+
+- Fix registry key validation regexp.
+  [jensens] (#23)
+
+
+1.2.0 (2021-04-23)
+------------------
+
+New features:
+
+
+- Allow plone.schema.JSONField be stored in registry (as dict-like)
+   [sneridagh] (#719)
+
+
+1.1.6 (2020-04-22)
+------------------
+
+Bug fixes:
+
+
+- Minor packaging updates. (#1)
+
+
+1.1.5 (2018-12-14)
+------------------
+
+Bug fixes:
+
+- Avoid a deprecation warning that would turn into an error on Python 3.8.
+  [gforcada]
+
+
+1.1.4 (2018-11-04)
+------------------
+
+Bug fixes:
+
+- Adapt test to changed object field in zope4
+  [pbauer]
+
+
+1.1.3 (2018-06-22)
+------------------
+
+Bug fixes:
+
+- Improve performance of RecordsProxy.__iter__ which is now invoked more in
+  core Plone as part of the requireJS configuration
+  [MatthewWilkes]
+
+
+1.1.2 (2016-12-06)
+------------------
+
+Bug fixes:
+
+- Fix tests to pass on Python 3.5
+  [datakurre]
+
+
+1.1.1 (2016-11-19)
+------------------
+
+Bug fixes:
+
+- Fix endless recursion on getting values from broken records proxy objects
+  [tomgross]
+
+
+1.1.0 (2016-07-05)
+------------------
+
+New features:
+
+- Give ``RecordsProxy`` a ``__parent__`` (the registry) in order to make it a good Zope citizen.
+  This helps in context of z3cform binders and other similar situations,
+  where a records proxy is used as context.
+  [jensens]
+
+
+1.0.4 (2016-06-12)
+------------------
+
+Fixes:
+
+- More cleanup: PEP8, isort, readability.
+  [jensens]
+
+
+1.0.3 (2016-02-26)
+------------------
+
+Fixes:
+
+- Replace deprecated ``zope.testing.doctestunit`` import with ``doctest``
+  module from stdlib.
+  [thet]
+
+- Cleanup: Pep8, utf8 headers, whitespace fixes, readability, ReST-fixes,
+  doc-style, etc.
+  [jensens]
+
+
+1.0.2 (2014-09-11)
+------------------
+
+- Choice field construction compatible with a simple vocabulary of
+  string-based choices, which are converted to values on construction.
+  This provides compatibility for plone.registry/plone.app.registry
+  integration with plone.supermodel >= 1.2.5.
+  [seanupton]
+
+
+1.0.1 (2013-01-13)
+------------------
+
+1.0 - 2011-05-13
+----------------
+
+- Release 1.0 Final
+  [esteele]
+
+- Add MANIFEST.in.
+  [WouterVH]
+
+
+1.0b5 - 2011-04-06
+------------------
+
+- Make RecordsProxy type customizable through ``factory`` argument to
+  ``forInterface`` and ``collectionOfInterface``.
+  [elro]
+
+- Add ``collectionOfInterface`` support to registry.
+  [elro]
+
+- Fixed bug where prefix was ignored by registry.forInterface.
+  [elro]
+
+- Add optional min, max arguments for keys/values/items of _Records.
+  [elro]
+
+
+1.0b4 - 2011-02-04
+------------------
+
+- Added support for field references, via the ``FieldRef`` class. See
+  ``registry.txt`` for details.
+  [optilude]
+
+- Change the internal persistent structure around to make it more efficient.
+  The API remains the same. Old registries will be migrated when first
+  accessed. Warning: This may lead to a "write-on-read" situation for the
+  first request in which the registry is being used.
+  [optilude]
+
+
+1.0b3 - 2011-01-03
+------------------
+
+ - Added prefix option to forInterface (as it was added to registerInterface)
+   [garbas]
+
+
+1.0b2 - 2010-04-21
+------------------
+
+- Added support for Decimal fields
+  [optilude]
+
+- Add a prefix option to registerInterface to allow an interface to be used as
+  a template for a series of values, rather than single use.
+  [MatthewWilkes]
+
+
+1.0b1 - 2009-08-02
+------------------
+
+- Fix a bug in bind() for Choice fields.
+  [optilude]
+
+
+1.0a2 - 2009-07-12
+------------------
+
+- Changed API methods and arguments to mixedCase to be more consistent with
+  the rest of Zope. This is a non-backwards-compatible change. Our profuse
+  apologies, but it's now or never. :-/
+
+  If you find that you get import errors or unknown keyword arguments in your
+  code, please change names from foo_bar too fooBar, e.g. for_interface()
+  becomes forInterface().
+  [optilude]
+
+
+1.0a1 - 2009-04-17
+------------------
+
+- Initial release
+
```

### Comparing `plone.registry-1.2.1/docs/INSTALL.txt` & `plone.registry-2.0.0/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.registry-1.2.1/docs/LICENSE.GPL` & `plone.registry-2.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.registry-1.2.1/docs/LICENSE.txt` & `plone.registry-2.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.registry-1.2.1/plone/registry/events.py` & `plone.registry-2.0.0/plone/registry/events.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,49 @@
-# -*- coding: utf-8 -*-
 from plone.registry.interfaces import IInterfaceAwareRecord
 from plone.registry.interfaces import IRecordAddedEvent
 from plone.registry.interfaces import IRecordEvent
 from plone.registry.interfaces import IRecordModifiedEvent
 from plone.registry.interfaces import IRecordRemovedEvent
 from plone.registry.recordsproxy import RecordsProxy
 from zope.component import adapter
 from zope.component import subscribers
 from zope.interface import implementer
 
 
 @implementer(IRecordEvent)
-class RecordEvent(object):
-
+class RecordEvent:
     def __init__(self, record):
         self.record = record
 
     def __repr__(self):
-        return "<%s for %s>" % (self.__class__.__name__, self.record.__name__)
+        return f"<{self.__class__.__name__} for {self.record.__name__}>"
 
 
 @implementer(IRecordAddedEvent)
 class RecordAddedEvent(RecordEvent):
     """record added"""
 
 
 @implementer(IRecordRemovedEvent)
 class RecordRemovedEvent(RecordEvent):
     """record removed"""
 
 
 @implementer(IRecordModifiedEvent)
 class RecordModifiedEvent(RecordEvent):
-
     def __init__(self, record, oldValue, newValue):
-        super(RecordModifiedEvent, self).__init__(record)
+        super().__init__(record)
         self.oldValue = oldValue
         self.newValue = newValue
 
 
 @adapter(IRecordEvent)
 def redispatchInterfaceAwareRecordEvents(event):
     """When an interface-aware record received a record event,
-    redispatch the event in a simlar manner to the IObjectEvent redispatcher.
+    redispatch the event in a similar manner to the IObjectEvent redispatcher.
 
     Note that this means one IRecordModifiedEvent will be fired for each
     change to a record.
     """
 
     record = event.record
```

### Comparing `plone.registry-1.2.1/plone/registry/events.rst` & `plone.registry-2.0.0/plone/registry/events.rst`

 * *Files identical despite different names*

### Comparing `plone.registry-1.2.1/plone/registry/field.py` & `plone.registry-2.0.0/plone/registry/field.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """This module defines persistent versions of various fields.
 
 The idea is that when a record is created, we copy relevant field properties
 from the transient schema field from zope.schema, into the corresponding
 persistent field. Not all field types are supported, but the common types
 are.
 """
@@ -10,131 +9,120 @@
 from plone.registry.interfaces import IPersistentField
 from zope.interface import implementer
 from zope.schema.interfaces import IContextSourceBinder
 from zope.schema.vocabulary import SimpleVocabulary
 
 import zope.schema
 import zope.schema._field
-import sys
+
 
 try:
     import plone.schema
+
     HASPLONESCHEMA = True
 except ImportError:
     HASPLONESCHEMA = False
 
-if sys.version_info >= (3,):
-    basestring = str
-    text_type = str
-    _primitives = (int, bool, str, bytes, tuple,
-                   list, set, frozenset, dict, float)
-else:
-    text_type = unicode
-    _primitives = (int, long, bool, str, unicode, tuple,
-                   list, set, frozenset, dict, float)
+_primitives = (int, bool, str, bytes, tuple, list, set, frozenset, dict, float)
 
 _missing_value_marker = object()
 
 
 def is_primitive(value):
     return value is None or isinstance(value, _primitives)
 
 
-class DisallowedProperty(object):
+class DisallowedProperty:
     """A property that may not be set on an instance. It may still be set
     defined in a base class.
     """
+
     uses = []
 
     def __init__(self, name):
         self._name = name
         DisallowedProperty.uses.append(name)
 
     def __get__(self, inst, type_=None):
         # look for the object in bases
         if type_ is not None:
             for c in type_.__mro__:
-                if self._name in c.__dict__ and not \
-                        isinstance(c.__dict__[self._name], DisallowedProperty):
+                if self._name in c.__dict__ and not isinstance(
+                    c.__dict__[self._name], DisallowedProperty
+                ):
                     function = c.__dict__[self._name]
                     return function.__get__(inst, type_)
         raise AttributeError(self._name)
 
     def __set__(self, inst, value):
         raise ValueError(
-            u"Persistent fields does not support setting the `{0}` "
-            u"property".format(self._name)
+            "Persistent fields does not support setting the `{}` "
+            "property".format(self._name)
         )
 
 
-class StubbornProperty(object):
-    """A property that stays stubbornly at a single, pre-defined value.
-    """
+class StubbornProperty:
+    """A property that stays stubbornly at a single, pre-defined value."""
+
     uses = []
 
     def __init__(self, name, value):
         StubbornProperty.uses.append(name)
         self._name = name
         self._value = value
 
     def __set__(self, inst, value):
         pass
 
     def __get__(self, inst, type_=None):
         return self._value
 
 
-class InterfaceConstrainedProperty(object):
-    """A property that may only contain values providing a certain interface.
-    """
+class InterfaceConstrainedProperty:
+    """A property that may only contain values providing a certain interface."""
+
     uses = []
 
     def __init__(self, name, interface):
         InterfaceConstrainedProperty.uses.append((name, interface))
         self._name = name
         self._interface = interface
 
     def __set__(self, inst, value):
-        if (
-            value != inst.missing_value
-            and not self._interface.providedBy(value)
-        ):
+        if value != inst.missing_value and not self._interface.providedBy(value):
             raise ValueError(
-                u"The property `{0}` may only contain objects "
-                "providing `{1}`.".format(
+                "The property `{}` may only contain objects "
+                "providing `{}`.".format(
                     self._name,
                     self._interface.__identifier__,
                 )
             )
         inst.__dict__[self._name] = value
 
 
 @implementer(IPersistentField)
 class PersistentField(Persistent):
-    """Base class for persistent field definitions.
-    """
+    """Base class for persistent field definitions."""
+
     # Persistent fields do not have an order
-    order = StubbornProperty('order', -1)
+    order = StubbornProperty("order", -1)
 
     # We don't allow setting a custom constraint, as this would introduce a
     # dependency on a symbol such as a function that may go away
-    constraint = DisallowedProperty('constraint')
+    constraint = DisallowedProperty("constraint")
 
     # Details about which interface/field name we originally came form, if any
     interfaceName = None
     fieldName = None
 
 
-class PersistentCollectionField(
-    PersistentField,
-    zope.schema._field.AbstractCollection
-):
-    """Ensure that value_type is a persistent field
-    """
-    value_type = InterfaceConstrainedProperty('value_type', IPersistentField)
+class PersistentCollectionField(PersistentField, zope.schema._field.AbstractCollection):
+    """Ensure that value_type is a persistent field"""
+
+    value_type = InterfaceConstrainedProperty("value_type", IPersistentField)
 
 
 class Bytes(PersistentField, zope.schema.Bytes):
     pass
 
 
 class BytesLine(PersistentField, zope.schema.BytesLine):
@@ -190,17 +178,16 @@
 
 
 class Password(PersistentField, zope.schema.Password):
     pass
 
 
 class Dict(PersistentField, zope.schema.Dict):
-
-    key_type = InterfaceConstrainedProperty('key_type', IPersistentField)
-    value_type = InterfaceConstrainedProperty('value_type', IPersistentField)
+    key_type = InterfaceConstrainedProperty("key_type", IPersistentField)
+    value_type = InterfaceConstrainedProperty("value_type", IPersistentField)
 
 
 class Datetime(PersistentField, zope.schema.Datetime):
     pass
 
 
 class Date(PersistentField, zope.schema.Date):
@@ -229,33 +216,34 @@
 
 class Choice(PersistentField, zope.schema.Choice):
     # We can only support string name or primitive=list vocabularies
     _values = None
     _vocabulary = None
 
     def __init__(self, values=None, vocabulary=None, source=None, **kw):
-
-        if vocabulary is not None and not isinstance(vocabulary, basestring):
+        if vocabulary is not None and not isinstance(vocabulary, str):
             values = self._normalized_values(vocabulary)
             if values is None:
                 raise ValueError(
                     "Persistent fields only support named vocabularies or "
                     "vocabularies based on simple value sets."
                 )
             vocabulary = None
         elif source is not None:
             raise ValueError(
                 "Persistent fields do not support sources, only named "
                 "vocabularies or vocabularies based on simple value sets."
             )
 
-        assert not (values is None and vocabulary is None), (
-            "You must specify either values or vocabulary.")
-        assert values is None or vocabulary is None, (
-            "You cannot specify both values and vocabulary.")
+        assert not (
+            values is None and vocabulary is None
+        ), "You must specify either values or vocabulary."
+        assert (
+            values is None or vocabulary is None
+        ), "You cannot specify both values and vocabulary."
 
         self.vocabularyName = None
 
         if values is not None:
             for value in values:
                 if not is_primitive(value):
                     raise ValueError(
@@ -266,27 +254,28 @@
             self.vocabularyName = vocabulary
 
         self._init_field = bool(self.vocabularyName)
         super(zope.schema.Choice, self).__init__(**kw)
         self._init_field = False
 
     def _normalized_values(self, vocabulary):
-        if getattr(vocabulary, '__iter__', None):
-            if all([isinstance(term.value, text_type) for term in vocabulary]):
+        if getattr(vocabulary, "__iter__", None):
+            if all([isinstance(term.value, str) for term in vocabulary]):
                 return [term.value for term in vocabulary]
         return None
 
     @property
     def vocabulary(self):
         # may be set by bind()
         if self._vocabulary is not None:
             return self._vocabulary
         if self._values is not None:
             return SimpleVocabulary.fromValues(self._values)
-    DisallowedProperty.uses.append('vocabulary')
+
+    DisallowedProperty.uses.append("vocabulary")
 
     # override bind to allow us to keep constraints on the 'vocabulary'
     # property
     def bind(self, object):
         clone = zope.schema.Field.bind(self, object)
         # get registered vocabulary if needed:
         if IContextSourceBinder.providedBy(self.vocabulary):
@@ -296,11 +285,11 @@
             vr = zope.schema.vocabulary.getVocabularyRegistry()
             clone._vocabulary = vr.get(object, self.vocabularyName)
             assert zope.schema.interfaces.ISource.providedBy(clone.vocabulary)
         return clone
 
 
 if HASPLONESCHEMA:
-    class JSONField(PersistentField, plone.schema.JSONField):
 
+    class JSONField(PersistentField, plone.schema.JSONField):
         key_type = InterfaceConstrainedProperty("key_type", IPersistentField)
         value_type = InterfaceConstrainedProperty("value_type", IPersistentField)
```

### Comparing `plone.registry-1.2.1/plone/registry/field.rst` & `plone.registry-2.0.0/plone/registry/field.rst`

 * *Files identical despite different names*

### Comparing `plone.registry-1.2.1/plone/registry/fieldfactory.py` & `plone.registry-2.0.0/plone/registry/fieldfactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.registry.field import DisallowedProperty
 from plone.registry.field import InterfaceConstrainedProperty
 from plone.registry.field import is_primitive
 from plone.registry.field import StubbornProperty
 from plone.registry.interfaces import IPersistentField
 from zope.component import adapter
 from zope.interface import implementer
@@ -14,16 +13,15 @@
 
 import plone.registry.field
 
 
 @implementer(IPersistentField)
 @adapter(IField)
 def persistentFieldAdapter(context):
-    """Turn a non-persistent field into a persistent one
-    """
+    """Turn a non-persistent field into a persistent one"""
 
     if IPersistentField.providedBy(context):
         return context
 
     # See if we have an equivalently-named field
 
     class_name = context.__class__.__name__
@@ -36,46 +34,47 @@
         return None
 
     ignored = list(DisallowedProperty.uses + StubbornProperty.uses)
     constrained = list(InterfaceConstrainedProperty.uses)
 
     instance = persistent_class.__new__(persistent_class)
 
-    context_dict = dict(
-        [(k, v) for k, v in context.__dict__.items() if k not in ignored]
-    )
+    context_dict = {k: v for k, v in context.__dict__.items() if k not in ignored}
 
     for key, iface in constrained:
         value = context_dict.get(key, None)
         if value is None or value == context.missing_value:
             continue
         value = iface(value, None)
         if value is None:
             __traceback_info__ = (
-                "The property `{0}` cannot be adapted to "
-                "`{1}`.".format(key, iface.__identifier__,)
+                "The property `{}` cannot be adapted to "
+                "`{}`.".format(
+                    key,
+                    iface.__identifier__,
+                )
             )
             return None
         context_dict[key] = value
 
     instance.__dict__.update(context_dict)
     return instance
 
 
 @implementer(IPersistentField)
 @adapter(IChoice)
 def choicePersistentFieldAdapter(context):
-    """Special handling for Choice fields.
-    """
+    """Special handling for Choice fields."""
     instance = persistentFieldAdapter(context)
     if instance is None:
         return None
 
-    if ISource.providedBy(context.vocabulary) or \
-            IContextSourceBinder.providedBy(context.vocabulary):
+    if ISource.providedBy(context.vocabulary) or IContextSourceBinder.providedBy(
+        context.vocabulary
+    ):
         safe = False
 
         # Attempt to reverse engineer a 'values' argument
         if isinstance(context.vocabulary, SimpleVocabulary):
             values = []
             safe = True
             for term in context.vocabulary:
```

### Comparing `plone.registry-1.2.1/plone/registry/fieldref.py` & `plone.registry-2.0.0/plone/registry/fieldref.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# -*- coding: utf-8 -*-
 from plone.registry.interfaces import IFieldRef
 from zope.interface import implementedBy
 from zope.interface import implementer
 
 
 @implementer(IFieldRef)
-class FieldRef(object):
-    """Default field reference.
-    """
+class FieldRef:
+    """Default field reference."""
 
     def __init__(self, name, originalField):
         self.recordName = name
         self.originalField = originalField
 
     @property
     def __providedBy__(self):
-        provided = getattr(self, '__provides__', None)
+        provided = getattr(self, "__provides__", None)
         if provided is None:
             provided = implementedBy(self.__class__)
 
         return provided + self.originalField.__providedBy__
 
     def __getattr__(self, name):
         return getattr(self.originalField, name)
```

### Comparing `plone.registry-1.2.1/plone/registry/interfaces.py` & `plone.registry-2.0.0/plone/registry/interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# -*- coding: utf-8 -*-
 from zope import schema
 from zope.interface import Interface
 from zope.interface.interfaces import IInterface
 from zope.schema.interfaces import IField
 from zope.schema.interfaces import InvalidDottedName
 
 
 class InvalidRegistryKey(InvalidDottedName):
-    """A registry key is a dotted name with up to one '/'.
-    """
+    """A registry key is a dotted name with up to one '/'."""
 
 
 class IPersistentField(IField):
     """A field that can be persistent along with a record.
 
     We provide our own implementation of the basic field types that are
     supported by the registry.
@@ -20,39 +18,35 @@
     A persistent field may track which interface and field it originally
     was constructed from. This is done by the registerInterface() method
     on the IRegistry, for example. Only the interface/field names are stored,
     not actual object references.
     """
 
     interfaceName = schema.DottedName(
-        title=u'Dotted name to an interface the field was constructed from',
-        required=False
+        title="Dotted name to an interface the field was constructed from",
+        required=False,
     )
     fieldName = schema.ASCIILine(
-        title=u'Name of the field in the original interface, if any',
-        required=False
+        title="Name of the field in the original interface, if any", required=False
     )
 
 
 class IFieldRef(Interface):
     """A reference to another field.
 
     This allows a record to use a field that belongs to another record. Field
     refs are allowed in the Record() constructor.
 
     Note that all attributes are read-only.
     """
 
     recordName = schema.DottedName(
-        title=u'Name of the record containing the reference field'
-    )
-    originalField = schema.Object(
-        title=u'Referenced field',
-        schema=IField
+        title="Name of the record containing the reference field"
     )
+    originalField = schema.Object(title="Referenced field", schema=IField)
 
 
 class IRecord(Interface):
     """A record stored in the registry.
 
     A record may be "bound" or "unbound". If bound, it will have a
     __parent__ attribute giving the IRegistry it belongs to. It will then
@@ -60,90 +54,82 @@
     the registry. If unbound, it will store its own values.
 
     A record becomes bound when added to the registry. Records retrieved from
     the registry are always bound.
     """
 
     field = schema.Object(
-        title=u'A field describing this record',
-        schema=IPersistentField
+        title="A field describing this record", schema=IPersistentField
     )
 
     value = schema.Field(
-        title=u'The value of this record',
-        description=u'Must be valid according to the record\'s field'
+        title="The value of this record",
+        description="Must be valid according to the record's field",
     )
 
 
 class IRecordEvent(Interface):
-    """Base interface for record level events
-    """
+    """Base interface for record level events"""
 
     record = schema.Object(
-        title=u'The record that was added.',
-        description=u'Both __name__ and __parent__ will be set before the '
-                    u'event is fired',
-        schema=IRecord
+        title="The record that was added.",
+        description="Both __name__ and __parent__ will be set before the "
+        "event is fired",
+        schema=IRecord,
     )
 
 
 class IRecordAddedEvent(IRecordEvent):
-    """Event fired when a record is added to a registry.
-    """
+    """Event fired when a record is added to a registry."""
 
 
 class IRecordRemovedEvent(IRecordEvent):
-    """Event fired when a record is removed from a registry.
-    """
+    """Event fired when a record is removed from a registry."""
 
 
 class IRecordModifiedEvent(IRecordEvent):
-    """Event fired when a record's value is modified.
-    """
+    """Event fired when a record's value is modified."""
 
-    oldValue = schema.Field(title=u'The record\'s previous value')
-    newValue = schema.Field(title=u'The record\'s new value')
+    oldValue = schema.Field(title="The record's previous value")
+    newValue = schema.Field(title="The record's new value")
 
 
 class IInterfaceAwareRecord(Interface):
     """A record will be marked with this interface if it knows which
     interface its field came from.
     """
 
-    interfaceName = schema.DottedName(title=u"Dotted name to interface")
+    interfaceName = schema.DottedName(title="Dotted name to interface")
 
     interface = schema.Object(
-        title=u'Interface that provided the record',
-        description=u'May be None if the interface is no longer available',
+        title="Interface that provided the record",
+        description="May be None if the interface is no longer available",
         schema=IInterface,
-        readonly=True
+        readonly=True,
     )
 
-    fieldName = schema.ASCIILine(
-        title=u'Name of the field in the original interface'
-    )
+    fieldName = schema.ASCIILine(title="Name of the field in the original interface")
 
 
 class IRegistry(Interface):
-    """The configuration registry
-    """
+    """The configuration registry"""
 
     records = schema.Dict(
-        title=u'The records of the registry',
+        title="The records of the registry",
         key_type=schema.DottedName(
-            title=u'Name of the record',
-            description=u'By convention, this should include the '
-                        u'package name and optionally an interface '
-                        u'named, if the record can be described by a '
-                        u'field in an interface (see also '
-                        u'registerInterface() below), e.g. '
-                        u'my.package.interfaces.IMySettings.somefield.',
+            title="Name of the record",
+            description="By convention, this should include the "
+            "package name and optionally an interface "
+            "named, if the record can be described by a "
+            "field in an interface (see also "
+            "registerInterface() below), e.g. "
+            "my.package.interfaces.IMySettings.somefield.",
         ),
         value_type=schema.Object(
-            title=u'The record for this name',
+            title="The record for this name",
             schema=IRecord,
         ),
     )
 
     def __getitem__(key):
         """Get the value under the given key. A record must have been
         installed for this key for this to be valid. Otherwise, a KeyError is
@@ -159,16 +145,15 @@
         """Set the value under the given key. A record must have been
         installed for this key for this to be valid. Otherwise, a KeyError is
         raised. If value is not of a type that's allowed by the record, a
         ValidationError is raised.
         """
 
     def __contains__(key):
-        """Determine if the registry contains a record for the given key.
-        """
+        """Determine if the registry contains a record for the given key."""
 
     def forInterface(interface, check=True, omit=(), prefix=None):
         """Get an IRecordsProxy for the given interface. If `check` is True,
         an error will be raised if one or more fields in the interface does
         not have an equivalent setting.
         """
 
@@ -186,24 +171,22 @@
     """This object is returned by IRegistry.forInterface(). It will be
     made to provide the relevant interface, i.e. it will have the
     attributes that the interface promises. Those attributes will be retrieved
     from or written to the underlying IRegistry.
     """
 
     __schema__ = schema.Object(
-        title=u'Interface providing records',
-        schema=IInterface,
-        readonly=True
+        title="Interface providing records", schema=IInterface, readonly=True
     )
 
     __registry__ = schema.Object(
-        title=u'Registry where records will be looked up',
+        title="Registry where records will be looked up",
         schema=IRegistry,
-        readonly=True)
+        readonly=True,
+    )
 
     __omitted__ = schema.Tuple(
-        title=u'Fields that are not stored in the registry',
-        description=u'If any of these are accessed, you will get an '
-                    u'AttributeError',
-        value_type=schema.ASCIILine(title=u'Fieldname'),
-        readonly=True
+        title="Fields that are not stored in the registry",
+        description="If any of these are accessed, you will get an " "AttributeError",
+        value_type=schema.ASCIILine(title="Fieldname"),
+        readonly=True,
     )
```

### Comparing `plone.registry-1.2.1/plone/registry/record.py` & `plone.registry-2.0.0/plone/registry/record.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from persistent import Persistent
 from plone.registry.events import RecordModifiedEvent
 from plone.registry.interfaces import IInterfaceAwareRecord
 from plone.registry.interfaces import IPersistentField
 from plone.registry.interfaces import IRecord
 from zope.dottedname.resolve import resolve
 from zope.event import notify
@@ -21,19 +20,18 @@
     field and value are read from and written to the parent registry.
 
     BBB: The current storage implementation does not actually store Record
     objects directly. However, we keep the Persistent base class so that old
     values may be loaded during automated migration.
     """
 
-    __name__ = u""
+    __name__ = ""
     __parent__ = None
 
     def __init__(self, field, value=_marker, _validate=True):
-
         if _validate and not IPersistentField.providedBy(field):
             raise ValueError("Field is not persistent")
 
         if value is _marker:
             value = field.default
         else:
             if _validate:
@@ -67,15 +65,14 @@
 
     def _get_value(self):
         if self.__parent__ is not None:
             return self.__parent__.records._values[self.__name__]
         return self._value
 
     def _set_value(self, value):
-
         field = self.field
 
         if field is None:
             raise ValueError("The record's field must be set before its value")
 
         field = field.bind(self)
         if value != field.missing_value:
```

### Comparing `plone.registry-1.2.1/plone/registry/recordsproxy.py` & `plone.registry-2.0.0/plone/registry/recordsproxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,42 @@
-# -*- coding: utf-8 -*-
+from collections.abc import MutableMapping
 from plone.registry.interfaces import IRecordsProxy
 from zope.interface import alsoProvides
 from zope.interface import implementer
 from zope.schema import getFieldsInOrder
 from zope.schema.interfaces import RequiredMissing
 
 import re
-import sys
 
 
-try:
-    from UserDict import UserDict
-    from UserDict import DictMixin
-except ImportError:
-    from collections import UserDict
-    from collections.abc import MutableMapping as DictMixin
-
-if sys.version_info >= (3,):
-    basestring = str
-
 _marker = object()
 
 
 @implementer(IRecordsProxy)
-class RecordsProxy(object):
-    """A proxy that maps an interface to a number of records
-    """
+class RecordsProxy:
+    """A proxy that maps an interface to a number of records"""
 
     def __init__(self, registry, schema, omitted=(), prefix=None):
         if prefix is None:
-            prefix = schema.__identifier__ + '.'
+            prefix = schema.__identifier__ + "."
         elif not prefix.endswith("."):
-            prefix += '.'
+            prefix += "."
 
         # skip __setattr__
-        self.__dict__['__schema__'] = schema
-        self.__dict__['__registry__'] = registry
-        self.__dict__['__omitted__'] = omitted
-        self.__dict__['__prefix__'] = prefix
-        self.__dict__['__parent__'] = registry
+        self.__dict__["__schema__"] = schema
+        self.__dict__["__registry__"] = registry
+        self.__dict__["__omitted__"] = omitted
+        self.__dict__["__prefix__"] = prefix
+        self.__dict__["__parent__"] = registry
 
         alsoProvides(self, schema)
 
     def __getattr__(self, name):
         if not self.__dict__ or name in self.__dict__.keys():
-           return super(RecordsProxy, self).__getattr__(name)
+            return super().__getattr__(name)
         if name not in self.__schema__:
             raise AttributeError(name)
         value = self.__registry__.get(self.__prefix__ + name, _marker)
         if value is _marker:
             value = self.__schema__[name].missing_value
         return value
 
@@ -58,102 +46,92 @@
             if full_name not in self.__registry__:
                 raise AttributeError(name)
             self.__registry__[full_name] = value
         else:
             self.__dict__[name] = value
 
     def __repr__(self):
-        return "<{0} for {1}>".format(
-            self.__class__.__name__,
-            self.__schema__.__identifier__
+        return "<{} for {}>".format(
+            self.__class__.__name__, self.__schema__.__identifier__
         )
 
 
-class RecordsProxyCollection(DictMixin):
-    """A proxy that maps a collection of RecordsProxy objects
-    """
+class RecordsProxyCollection(MutableMapping):
+    """A proxy that maps a collection of RecordsProxy objects"""
 
     _validkey = re.compile(r"([a-zA-Z][a-zA-Z0-9_.-]*)$").match
 
     # ord('.') == ord('/') - 1
 
-    def __init__(self, registry, schema, check=True, omitted=(), prefix=None,
-                 factory=None):
+    def __init__(
+        self, registry, schema, check=True, omitted=(), prefix=None, factory=None
+    ):
         if prefix is None:
             prefix = schema.__identifier__
 
         if not prefix.endswith("/"):
-            prefix += '/'
+            prefix += "/"
 
         self.registry = registry
         self.schema = schema
         self.check = check
         self.omitted = omitted
         self.prefix = prefix
         self.factory = factory
 
     def __getitem__(self, key):
         if key in iter(self):
             prefix = self.prefix + key
             proxy = self.registry.forInterface(
-                self.schema,
-                self.check,
-                self.omitted,
-                prefix,
-                self.factory
+                self.schema, self.check, self.omitted, prefix, self.factory
             )
             return proxy
         raise KeyError(key)
 
     def __iter__(self):
         min = self.prefix
-        max = self.prefix[:-1] + '0'
+        max = self.prefix[:-1] + "0"
         keys = self.registry.records.keys(min, max)
         len_prefix = len(self.prefix)
         last = None
         for name in keys:
             name = name[len_prefix:]
-            if '.' not in name:
+            if "." not in name:
                 yield name
             else:
-                key = name.rsplit('.', 1)[0]
+                key = name.rsplit(".", 1)[0]
                 if key != last:
                     yield key
                     last = key
 
     def __len__(self):
         return len(tuple(iter(self)))
 
     def keys(self):
         return list(iter(self))
 
     def _validate(self, key):
-        if not isinstance(key, basestring) or not self._validkey(key):
+        if not isinstance(key, str) or not self._validkey(key):
             raise TypeError(
-                'expected a valid key (alphanumeric or underscore, starting '
-                'with alpha)'
+                "expected a valid key (alphanumeric or underscore, starting "
+                "with alpha)"
             )
         return str(key)
 
     def has_key(self, key):
         key = self._validate(key)
         prefix = self.prefix + key
-        names = self.registry.records.keys(prefix + '.', prefix + '/')
+        names = self.registry.records.keys(prefix + ".", prefix + "/")
         return bool(names)
 
     def add(self, key):
         key = self._validate(key)
         prefix = self.prefix + key
         self.registry.registerInterface(self.schema, self.omitted, prefix)
-        proxy = self.registry.forInterface(
-            self.schema,
-            False,
-            self.omitted,
-            prefix
-        )
+        proxy = self.registry.forInterface(self.schema, False, self.omitted, prefix)
         return proxy
 
     def __setitem__(self, key, value):
         key = self._validate(key)
         data = {}
         for name, field in getFieldsInOrder(self.schema):
             if name in self.omitted or field.readonly:
@@ -176,10 +154,10 @@
                 self[key] = failobj
         return self[key]
 
     def __delitem__(self, key):
         if key not in self:
             raise KeyError(key)
         prefix = self.prefix + key
-        names = list(self.registry.records.keys(prefix + '.', prefix + '/'))
+        names = list(self.registry.records.keys(prefix + ".", prefix + "/"))
         for name in names:
             del self.registry.records[name]
```

### Comparing `plone.registry-1.2.1/plone/registry/registry.py` & `plone.registry-2.0.0/plone/registry/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from BTrees.OOBTree import OOBTree
 from persistent import Persistent
 from plone.registry.events import RecordAddedEvent
 from plone.registry.events import RecordRemovedEvent
 from plone.registry.fieldref import FieldRef
 from plone.registry.interfaces import IFieldRef
 from plone.registry.interfaces import InvalidRegistryKey
@@ -17,23 +16,18 @@
 from zope.interface import implementer
 from zope.schema import getFieldNames
 from zope.schema import getFieldsInOrder
 
 import re
 import warnings
 
-import sys
-if sys.version_info >= (3,):
-    basestring = str
-
 
 @implementer(IRegistry)
 class Registry(Persistent):
-    """The persistent registry
-    """
+    """The persistent registry"""
 
     def __init__(self):
         self._records = _Records(self)
 
     # Basic value access API
 
     def __getitem__(self, name):
@@ -60,118 +54,99 @@
         # XXX: On-the-fly migration
         if isinstance(self._records, Records):
             self._migrateRecords()
         return self._records
 
     # Schema interface API
 
-    def forInterface(self, interface, check=True, omit=(), prefix=None,
-                     factory=None):
+    def forInterface(self, interface, check=True, omit=(), prefix=None, factory=None):
         if prefix is None:
             prefix = interface.__identifier__
 
         if not prefix.endswith("."):
-            prefix += '.'
+            prefix += "."
 
         if check:
             for name in getFieldNames(interface):
                 if name not in omit and prefix + name not in self:
                     raise KeyError(
-                        "Interface `{0}` defines a field `{1}`, for which "
-                        "there is no record.".format(
-                            interface.__identifier__,
-                            name
-                        )
+                        "Interface `{}` defines a field `{}`, for which "
+                        "there is no record.".format(interface.__identifier__, name)
                     )
 
         if factory is None:
             factory = RecordsProxy
 
         return factory(self, interface, omitted=omit, prefix=prefix)
 
     def registerInterface(self, interface, omit=(), prefix=None):
         if prefix is None:
             prefix = interface.__identifier__
 
         if not prefix.endswith("."):
-            prefix += '.'
+            prefix += "."
 
         for name, field in getFieldsInOrder(interface):
             if name in omit or field.readonly:
                 continue
             record_name = prefix + name
             persistent_field = queryAdapter(field, IPersistentField)
             if persistent_field is None:
                 raise TypeError(
                     "There is no persistent field equivalent for the field "
-                    "`{0}` of type `{1}`.".format(
-                        name,
-                        field.__class__.__name__
-                    )
+                    "`{}` of type `{}`.".format(name, field.__class__.__name__)
                 )
 
             persistent_field.interfaceName = interface.__identifier__
             persistent_field.fieldName = name
 
             value = persistent_field.default
 
-            # Attempt to retain the exisiting value
+            # Attempt to retain the existing value
             if record_name in self.records:
                 existing_record = self.records[record_name]
                 value = existing_record.value
                 bound_field = persistent_field.bind(existing_record)
                 try:
                     bound_field.validate(value)
-                except:
+                except Exception:
                     value = persistent_field.default
 
-            self.records[record_name] = Record(
-                persistent_field,
-                value,
-                _validate=False
-            )
-
-    def collectionOfInterface(self, interface, check=True, omit=(),
-                              prefix=None, factory=None):
-        return RecordsProxyCollection(
-            self,
-            interface,
-            check,
-            omit,
-            prefix,
-            factory
-        )
+            self.records[record_name] = Record(persistent_field, value, _validate=False)
+
+    def collectionOfInterface(
+        self, interface, check=True, omit=(), prefix=None, factory=None
+    ):
+        return RecordsProxyCollection(self, interface, check, omit, prefix, factory)
 
     # BBB
 
     def _migrateRecords(self):
         """BBB: Migrate from the old Records structure to the new. This is
         done the first time the "old" structure is accessed.
         """
         records = _Records(self)
 
-        oldData = getattr(self._records, 'data', None)
+        oldData = getattr(self._records, "data", None)
         if oldData is not None:
             for name, oldRecord in oldData.iteritems():
                 oldRecord._p_activate()
-                if (
-                    'field' in oldRecord.__dict__
-                    and 'value' in oldRecord.__dict__
-                ):
-                    records._fields[name] = oldRecord.__dict__['field']
-                    records._values[name] = oldRecord.__dict__['value']
+                if "field" in oldRecord.__dict__ and "value" in oldRecord.__dict__:
+                    records._fields[name] = oldRecord.__dict__["field"]
+                    records._values[name] = oldRecord.__dict__["value"]
 
         self._records = records
 
 
-class _Records(object):
+class _Records:
     """The records stored in the registry. This implements dict-like access
     to records, where as the Registry object implements dict-like read-only
     access to values.
     """
+
     __parent__ = None
 
     # Similar to zope.schema._field._isdotted, but allows up to one '/'
     _validkey = re.compile(
         r"([a-zA-Z][a-zA-Z0-9_-]*)((?:\.[a-zA-Z0-9][a-zA-Z0-9_-]*)*)"
         r"([/][a-zA-Z0-9][a-zA-Z0-9_-]*)?((?:\.[a-zA-Z0-9][a-zA-Z0-9_-]*)*)$"
     ).match
@@ -205,15 +180,14 @@
 
         del self._fields[name]
         del self._values[name]
 
         notify(RecordRemovedEvent(record))
 
     def __getitem__(self, name):
-
         field = self._getField(name)
         value = self._values[name]
 
         record = Record(field, value, _validate=False)
         record.__name__ = name
         record.__parent__ = self.__parent__
 
@@ -249,15 +223,15 @@
     def minKey(self, key=None):
         return self._values.minKey(key)
 
     def values(self, min=None, max=None):
         return [self[name] for name in self.keys(min, max)]
 
     def items(self, min=None, max=None):
-        return [(name, self[name],) for name in self.keys(min, max)]
+        return [(name, self[name]) for name in self.keys(min, max)]
 
     def setdefault(self, key, value):
         if key not in self:
             self[key] = value
         return self[key]
 
     def clear(self):
@@ -266,44 +240,41 @@
 
     # Helper methods
 
     def _getField(self, name):
         field = self._fields[name]
 
         # Handle field reference pointers
-        if isinstance(field, basestring):
+        if isinstance(field, str):
             recordName = field
-            while isinstance(field, basestring):
+            while isinstance(field, str):
                 recordName = field
                 field = self._fields[recordName]
             field = FieldRef(recordName, field)
 
         return field
 
     def _setField(self, name, field):
         if not IPersistentField.providedBy(field):
             raise ValueError("The record's field must be an IPersistentField.")
         if IFieldRef.providedBy(field):
             if field.recordName not in self._fields:
-                raise ValueError(
-                    "Field reference points to non-existent record"
-                )
+                raise ValueError("Field reference points to non-existent record")
             self._fields[name] = field.recordName  # a pointer, of sorts
         else:
-            field.__name__ = 'value'
+            field.__name__ = "value"
             self._fields[name] = field
 
 
 class Records(_Records, Persistent):
     """BBB: This used to be the class for the _records attribute of the
     registry. Having this be a Persistent object was always a bad idea. We
     keep it here so that we can migrate to the new structure, but it should
     no longer be used.
     """
 
     def __init__(self, parent):
         warnings.warn(
-            "The Records persistent class is deprecated and should not be "
-            "used.",
-            DeprecationWarning
+            "The Records persistent class is deprecated and should not be " "used.",
+            DeprecationWarning,
         )
-        super(Records, self).__init__(parent)
+        super().__init__(parent)
```

### Comparing `plone.registry-1.2.1/plone/registry/registry.rst` & `plone.registry-2.0.0/plone/registry/registry.rst`

 * *Files 1% similar despite different names*

```diff
@@ -70,20 +70,15 @@
 
     >>> age_record.value = 2
     >>> age_record.value
     2
 
 Note that the value is validated against the field::
 
-    >>> age_record.value = -1  # doctest: +SKIP_PYTHON_3
-    Traceback (most recent call last):
-    ...
-    TooSmall: (-1, 0)
-
-    >>> age_record.value = -1  # doctest: +SKIP_PYTHON_2
+    >>> age_record.value = -1
     Traceback (most recent call last):
     ...
     zope.schema._bootstrapinterfaces.TooSmall: (-1, 0)
 
     >>> age_record.value
     2
 
@@ -134,20 +129,15 @@
     >>> registry['plone.registry.tests.cms']  # doctest: +IGNORE_U
     u'Plone'
 
     >>> registry['plone.registry.tests.cms'] = u"Plone 3.x"
 
 Again, values are validated::
 
-    >>> registry['plone.registry.tests.cms'] = b'Joomla'  # doctest: +SKIP_PYTHON_3
-    Traceback (most recent call last):
-    ...
-    WrongType: ('Joomla', <type 'unicode'>...)
-
-    >>> registry['plone.registry.tests.cms'] = b'Joomla'  # doctest: +SKIP_PYTHON_2
+    >>> registry['plone.registry.tests.cms'] = b'Joomla'
     Traceback (most recent call last):
     ...
     zope.schema._bootstrapinterfaces.WrongType: (b'Joomla', <class 'str'>, 'value')
 
 There is also a ``get()`` method::
 
     >>> registry.get('plone.registry.tests.cms')  # doctest: +IGNORE_U
@@ -484,28 +474,23 @@
     >>> registry['plone.registry.tests.timeout']
     10
     >>> registry['plone.registry.tests.timeout.override']
     20
 
 Validation uses the underlying field::
 
-    >>> registry['plone.registry.tests.timeout.override'] = -1  # doctest: +SKIP_PYTHON_3
-    Traceback (most recent call last):
-    ...
-    TooSmall: (-1, 0)
-
-    >>> registry['plone.registry.tests.timeout.override'] = -1  # doctest: +SKIP_PYTHON_2
+    >>> registry['plone.registry.tests.timeout.override'] = -1
     Traceback (most recent call last):
     ...
     zope.schema._bootstrapinterfaces.TooSmall: (-1, 0)
 
 The reference field exposes the standard field properties, e.g.::
 
-    >>> timeout_override_record.field.title  # doctest: +SKIP_PYTHON_3
-    u'Timeout'
+    >>> timeout_override_record.field.title
+    'Timeout'
     >>> timeout_override_record.field.min
     0
 
 To look up the underlying record name, we can use the ``recordName`` property::
 
     >>> timeout_override_record.field.recordName
     'plone.registry.tests.timeout'
```

### Comparing `plone.registry-1.2.1/plone/registry/tests.py` & `plone.registry-2.0.0/plone/registry/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,198 +1,174 @@
-# -*- coding: utf-8 -*-
 from plone.registry.fieldfactory import choicePersistentFieldAdapter
 from plone.registry.fieldfactory import persistentFieldAdapter
+from zope import schema
 from zope.component import eventtesting
 from zope.component import provideAdapter
 from zope.component import testing
-from zope import schema
 from zope.interface import Interface
 
 import doctest
 import re
-import sys
 import unittest
 
 
-SKIP_PYTHON_2 = doctest.register_optionflag('SKIP_PYTHON_2')
-SKIP_PYTHON_3 = doctest.register_optionflag('SKIP_PYTHON_3')
-IGNORE_B = doctest.register_optionflag('IGNORE_B')
-IGNORE_U = doctest.register_optionflag('IGNORE_U')
+IGNORE_U = doctest.register_optionflag("IGNORE_U")
 
 
 class PolyglotOutputChecker(doctest.OutputChecker):
     def check_output(self, want, got, optionflags):
         # fix changed objectfield class in zope4
         got = re.sub(
-            'zope.schema._field.Object',
-            'zope.schema._bootstrapfields.Object', got)
+            "zope.schema._field.Object", "zope.schema._bootstrapfields.Object", got
+        )
 
-        if optionflags & SKIP_PYTHON_3 and sys.version_info >= (3,):
-            return True
-        elif optionflags & SKIP_PYTHON_2:
-            return True
-
-        if hasattr(self, '_toAscii'):
+        if hasattr(self, "_toAscii"):
             got = self._toAscii(got)
             want = self._toAscii(want)
 
         # Naive fix for comparing byte strings
-        if got != want and optionflags & IGNORE_B:
-            got = re.sub(r'^b([\'"])', r'\1', got)
-            want = re.sub(r'^b([\'"])', r'\1', want)
-
-        # Naive fix for comparing byte strings
         if got != want and optionflags & IGNORE_U:
-            got = re.sub(r'^u([\'"])', r'\1', got)
-            want = re.sub(r'^u([\'"])', r'\1', want)
+            got = re.sub(r'^u([\'"])', r"\1", got)
+            want = re.sub(r'^u([\'"])', r"\1", want)
 
-        return doctest.OutputChecker.check_output(
-            self, want, got, optionflags)
+        return doctest.OutputChecker.check_output(self, want, got, optionflags)
 
 
 class IMailSettings(Interface):
-    """Settings for email
-    """
+    """Settings for email"""
 
-    sender = schema.TextLine(title=u"Mail sender", default=u"root@localhost")
-    smtp_host = schema.URI(title=u"SMTP host server")
+    sender = schema.TextLine(title="Mail sender", default="root@localhost")
+    smtp_host = schema.URI(title="SMTP host server")
 
 
 class IMailPreferences(Interface):
-    """Settings for email
-    """
-    max_daily = schema.Int(
-        title=u"Maximum number of emails per day",
-        min=0,
-        default=3
-    )
-    settings = schema.Object(
-        title=u"Mail setings to use",
-        schema=IMailSettings
-    )
+    """Settings for email"""
+
+    max_daily = schema.Int(title="Maximum number of emails per day", min=0, default=3)
+    settings = schema.Object(title="Mail settings to use", schema=IMailSettings)
 
 
 def setUp(test=None):
     testing.setUp()
     eventtesting.setUp()
 
     provideAdapter(persistentFieldAdapter)
     provideAdapter(choicePersistentFieldAdapter)
 
 
 class TestBugs(unittest.TestCase):
-    """Regression tests for bugs that have been fixed
-    """
+    """Regression tests for bugs that have been fixed"""
 
     def setUp(self):
         setUp(self)
 
     def tearDown(self):
         testing.tearDown(self)
 
     def test_bind_choice(self):
         from plone.registry.field import Choice
-
         from zope.schema.vocabulary import getVocabularyRegistry
         from zope.schema.vocabulary import SimpleVocabulary
 
         def vocabFactory(obj):
-            return SimpleVocabulary.fromValues(['one', 'two'])
+            return SimpleVocabulary.fromValues(["one", "two"])
 
         reg = getVocabularyRegistry()
-        reg.register('my.vocab', vocabFactory)
+        reg.register("my.vocab", vocabFactory)
 
-        class T(object):
+        class T:
             f = None
 
-        f = Choice(__name__='f', title=u"Test", vocabulary="my.vocab")
+        f = Choice(__name__="f", title="Test", vocabulary="my.vocab")
         t = T()
 
         # Bug: this would give "AttributeError: can't set attribute" on
         # clone.vocabulary
         f.bind(t)
 
     def test_fieldref_interfaces(self):
-        from plone.registry import field, FieldRef
+        from plone.registry import field
+        from plone.registry import FieldRef
         from plone.registry.interfaces import IFieldRef
         from zope.schema.interfaces import ICollection
 
         listField = field.List(value_type=field.ASCIILine())
-        ref = FieldRef('some.record', listField)
+        ref = FieldRef("some.record", listField)
 
         self.assertTrue(ICollection.providedBy(ref))
         self.assertTrue(IFieldRef.providedBy(ref))
 
 
 class TestMigration(unittest.TestCase):
-
     def setUp(self):
         setUp(self)
 
     def tearDown(self):
         testing.tearDown(self)
 
     def test_auto_migration(self):
-
         from BTrees.OOBTree import OOBTree
-
-        from plone.registry.registry import Registry, Records, _Records
-        from plone.registry.record import Record
         from plone.registry import field
+        from plone.registry.record import Record
+        from plone.registry.registry import _Records
+        from plone.registry.registry import Records
+        from plone.registry.registry import Registry
 
         # Create an "old-looking registry"
 
         registry = Registry()
         registry._records = Records(registry)
         registry._records.data = OOBTree()
 
-        f = field.TextLine(title=u"Foo")
+        f = field.TextLine(title="Foo")
 
-        record = Record(f, u"Bar")
-        record.__dict__['field'] = f
-        record.__dict__['value'] = u"Bar"
+        record = Record(f, "Bar")
+        record.__dict__["field"] = f
+        record.__dict__["value"] = "Bar"
 
-        registry._records.data['foo.bar'] = record
+        registry._records.data["foo.bar"] = record
 
         # Attempt to access it
 
-        value = registry['foo.bar']
+        value = registry["foo.bar"]
 
         # Migration should have happened
 
-        self.assertEqual(value, u"Bar")
-        self.assertEqual(registry.records['foo.bar'].field.title, u"Foo")
-        self.assertEqual(registry.records['foo.bar'].value, u"Bar")
+        self.assertEqual(value, "Bar")
+        self.assertEqual(registry.records["foo.bar"].field.title, "Foo")
+        self.assertEqual(registry.records["foo.bar"].value, "Bar")
 
         self.assertFalse(isinstance(registry._records, Records))
         self.assertTrue(isinstance(registry._records, _Records))
 
 
 def test_suite():
-    return unittest.TestSuite([
-        doctest.DocFileSuite(
-            'registry.rst',
-            package='plone.registry',
-            optionflags=doctest.NORMALIZE_WHITESPACE | doctest.ELLIPSIS,
-            setUp=setUp,
-            tearDown=testing.tearDown,
-            checker=PolyglotOutputChecker()
-        ),
-        doctest.DocFileSuite(
-            'events.rst',
-            package='plone.registry',
-            optionflags=doctest.NORMALIZE_WHITESPACE | doctest.ELLIPSIS,
-            setUp=setUp,
-            tearDown=testing.tearDown,
-            checker=PolyglotOutputChecker()
-        ),
-        doctest.DocFileSuite(
-            'field.rst',
-            package='plone.registry',
-            optionflags=doctest.NORMALIZE_WHITESPACE | doctest.ELLIPSIS,
-            setUp=setUp,
-            tearDown=testing.tearDown,
-            checker=PolyglotOutputChecker()
-        ),
-        unittest.makeSuite(TestBugs),
-        unittest.makeSuite(TestMigration),
-    ])
+    return unittest.TestSuite(
+        [
+            doctest.DocFileSuite(
+                "registry.rst",
+                package="plone.registry",
+                optionflags=doctest.NORMALIZE_WHITESPACE | doctest.ELLIPSIS,
+                setUp=setUp,
+                tearDown=testing.tearDown,
+                checker=PolyglotOutputChecker(),
+            ),
+            doctest.DocFileSuite(
+                "events.rst",
+                package="plone.registry",
+                optionflags=doctest.NORMALIZE_WHITESPACE | doctest.ELLIPSIS,
+                setUp=setUp,
+                tearDown=testing.tearDown,
+                checker=PolyglotOutputChecker(),
+            ),
+            doctest.DocFileSuite(
+                "field.rst",
+                package="plone.registry",
+                optionflags=doctest.NORMALIZE_WHITESPACE | doctest.ELLIPSIS,
+                setUp=setUp,
+                tearDown=testing.tearDown,
+                checker=PolyglotOutputChecker(),
+            ),
+            unittest.defaultTestLoader.loadTestsFromTestCase(TestBugs),
+            unittest.defaultTestLoader.loadTestsFromTestCase(TestMigration),
+        ]
+    )
```

### Comparing `plone.registry-1.2.1/plone.registry.egg-info/PKG-INFO` & `plone.registry-2.0.0/plone.registry.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,1790 +1,1790 @@
 Metadata-Version: 2.1
 Name: plone.registry
-Version: 1.2.1
+Version: 2.0.0
 Summary: Registry for application settings (like debconf/ about:config)
 Home-page: https://pypi.org/project/plone.registry
 Author: Martin Aspeli, Wichert Akkerman, Hanno Schlichting
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
-Description: ============
-        Introduction
-        ============
-        This package provides debconf-like (or about:config-like) settings registries
-        for Zope applications. A ``registry``, with a dict-like API, is used to get and
-        set values stored in ``records``. Each record contains the actual value, as
-        well as a ``field`` that describes the record in more detail. At a minimum, the
-        field contains information about the type of value allowed, as well as a short
-        title describing the record's purpose.
-        
-        .. contents:: Table of Contents
-        
-        
-        ================
-        Using registries
-        ================
-        
-        You can create a new registry simply by instantiating the Registry class.
-        The class and its data structures are persistent, so you can store them in the ZODB.
-        You may want to provide the registry object as local utility for easy access as well, though we won't do that here.
-        
-        ::
-        
-            >>> from plone.registry import Registry
-            >>> registry = Registry()
-        
-        The registry starts out empty.
-        To access the registry's records, you can use the ``records`` property.
-        This exposes a dict API where keys are strings and values are objects providing ``IRecords``.
-        
-        ::
-        
-            >>> len(registry.records)
-            0
-        
-        Simple records
-        ==============
-        
-        Let's now create a record.
-        A record must have a name.
-        This should be a dotted name, and contain ASCII characters only.
-        By convention, it should be all lowercase and start with the name of the package that defines the record.
-        
-        It is also possible to create a  number of records based on a single schema interface - see below.
-        For now, we will focus on simple records.
-        
-        Before we can create the record, we must create the field that describes it.
-        Fields are based on the venerable ``zope.schema`` package.
-        ``plone.registry`` only supports certain fields, and disallows use of a few properties even of those.
-        As a rule of thumb, so long as a field stores a Python primitive, it is supported; the same goes for attributes of fields.
-        
-        Thus:
-        
-        * Fields like ``Object``, ``InterfaceField`` and so on are *not* supported.
-        * A custom ``constraint`` method is *not* supported.
-        * The ``order`` attribute will *always* be set to ``-1``.
-        * For Choice fields, *only named vocabularies* are supported:
-          you can *not* reference a particular *source* or *source binder*.
-        * The ``key_type`` and ``value_type`` properties of ``Dict``, ``List``, ``Tuple``, ``Set`` and ``Frozenset`` may *only* contain persistent fields.
-        
-        See section "Persistent fields" for more details.
-        
-        Creating a record
-        -----------------
-        
-        The supported field types are found in the module ``plone.registry.field``.
-        These are named the same as the equivalent field in ``zope.schema``, and have the same constructors.
-        You must use one of these fields when creating records directly::
-        
-            >>> from plone.registry import field
-            >>> age_field = field.Int(title=u"Age", min=0, default=18)
-        
-            >>> from plone.registry import Record
-            >>> age_record = Record(age_field)
-        
-        Note that in this case, we did not supply a value.
-        The value will therefore be the field default::
-        
-            >>> age_record.value
-            18
-        
-        We can set a different value, either in the ``Record`` constructor or via the ``value`` attribute::
-        
-            >>> age_record.value = 2
-            >>> age_record.value
-            2
-        
-        Note that the value is validated against the field::
-        
-            >>> age_record.value = -1  # doctest: +SKIP_PYTHON_3
-            Traceback (most recent call last):
-            ...
-            TooSmall: (-1, 0)
-        
-            >>> age_record.value = -1  # doctest: +SKIP_PYTHON_2
-            Traceback (most recent call last):
-            ...
-            zope.schema._bootstrapinterfaces.TooSmall: (-1, 0)
-        
-            >>> age_record.value
-            2
-        
-        We can now add the field to the registry.
-        This is done via the ``record`` dictionary::
-        
-            >>> 'plone.registry.tests.age' in registry
-            False
-            >>> registry.records['plone.registry.tests.age'] = age_record
-        
-        At this point, the record will gain ``__name__`` and ``__parent__`` attributes::
-        
-            >>> age_record.__name__
-            'plone.registry.tests.age'
-        
-            >>> age_record.__parent__ is registry
-            True
-        
-        Creating a record with an initial value
-        ---------------------------------------
-        
-        We can create records more succinctly in *one go* by
-        
-        1. creating the field,
-        2. creating the Record and setting its value as and
-        3. assigning it to the registry,
-        
-        like this::
-        
-            >>> registry.records['plone.registry.tests.cms'] = \
-            ...     Record(field.TextLine(title=u"CMS of choice"), u"Plone")
-        
-        The record can now be obtained.
-        Note that it has a nice ``__repr__`` to help debugging.
-        
-            >>> registry.records['plone.registry.tests.cms']
-            <Record plone.registry.tests.cms>
-        
-        Accessing and manipulating record values
-        ----------------------------------------
-        
-        Once a record has been created and added to the registry,
-        you can access its value through dict-like operations on the registry itself::
-        
-            >>> 'plone.registry.tests.cms' in registry
-            True
-        
-            >>> registry['plone.registry.tests.cms']  # doctest: +IGNORE_U
-            u'Plone'
-        
-            >>> registry['plone.registry.tests.cms'] = u"Plone 3.x"
-        
-        Again, values are validated::
-        
-            >>> registry['plone.registry.tests.cms'] = b'Joomla'  # doctest: +SKIP_PYTHON_3
-            Traceback (most recent call last):
-            ...
-            WrongType: ('Joomla', <type 'unicode'>...)
-        
-            >>> registry['plone.registry.tests.cms'] = b'Joomla'  # doctest: +SKIP_PYTHON_2
-            Traceback (most recent call last):
-            ...
-            zope.schema._bootstrapinterfaces.WrongType: (b'Joomla', <class 'str'>, 'value')
-        
-        There is also a ``get()`` method::
-        
-            >>> registry.get('plone.registry.tests.cms')  # doctest: +IGNORE_U
-            u'Plone 3.x'
-            >>> registry.get('non-existent-key') is None
-            True
-        
-        Deleting records
-        ----------------
-        
-        Records may be deleted from the ``records`` property::
-        
-            >>> del registry.records['plone.registry.tests.cms']
-            >>> 'plone.registry.tests.cms' in registry.records
-            False
-            >>> 'plone.registry.tests.cms' in registry
-            False
-        
-        Creating records from interfaces
-        ================================
-        
-        As an application developer, it is often desirable to define settings as traditional interfaces with ``zope.schema fields``.
-        ``plone.registry`` includes support for creating a set of records from a single interface.
-        
-        To test this, we have created an interface, ``IMailSettings``.
-        It has two fields: ``sender`` and ``smtp_host``::
-        
-            >>> from plone.registry.tests import IMailSettings
-        
-        Note that this contains standard fields::
-        
-            >>> IMailSettings['sender']
-            <zope.schema._bootstrapfields.TextLine object at ...>
-        
-            >>> IMailSettings['smtp_host']
-            <zope.schema._field.URI object at ...>
-        
-        We can create records from this interface like this::
-        
-            >>> registry.registerInterface(IMailSettings)
-        
-        One record for each field in the interface has now been created.
-        Their names are the full dotted names to those fields::
-        
-            >>> sender_record = registry.records['plone.registry.tests.IMailSettings.sender']
-            >>> smtp_host_record = registry.records['plone.registry.tests.IMailSettings.smtp_host']
-        
-        The fields used in the records will be the equivalent persistent versions of the fields from the original interface::
-        
-            >>> sender_record.field
-            <plone.registry.field.TextLine object at ...>
-        
-            >>> smtp_host_record.field
-            <plone.registry.field.URI object at ...>
-        
-        This feat is accomplished internally by adapting the field to the ``IPersistentField`` interface.
-        There is a default adapter factory that works for all fields defined in ``plone.registry.field``.
-        You can of course define your own adapter if you have a custom field type.
-        But bear in mind the golden rules of any persistent field::
-        
-        * The field must store only primitives or other persistent fields
-        * It must not reference a function, class, interface or other method that could break if a package is uninstalled.
-        
-        If we have a field for which there is no ``IPersistentField`` adapter, we will get an error::
-        
-            >>> from plone.registry.tests import IMailPreferences
-            >>> IMailPreferences['settings']
-            <zope.schema._bootstrapfields.Object object at ...>
-        
-            >>> registry.registerInterface(IMailPreferences)
-            Traceback (most recent call last):
-            ...
-            TypeError: There is no persistent field equivalent for the field `settings` of type `Object`.
-        
-        Whoops!
-        We can, however, tell ``registerInterface()`` to ignore one or more fields::
-        
-            >>> registry.registerInterface(IMailPreferences, omit=('settings',))
-        
-        Once an interface's records have been registered, we can get and set their values as normal::
-        
-            >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
-            u'root@localhost'
-        
-            >>> registry['plone.registry.tests.IMailSettings.sender'] = u"webmaster@localhost"
-            >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
-            u'webmaster@localhost'
-        
-        If we sub-sequently re-register the same interface, the value will be retained if possible::
-        
-            >>> registry.registerInterface(IMailSettings)
-            >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
-            u'webmaster@localhost'
-        
-        However, if the value is no longer valid, we will revert to the default.
-        To test that, let's sneakily modify the field for a while::
-        
-            >>> old_field = IMailSettings['sender']
-            >>> IMailSettings._InterfaceClass__attrs['sender'] = field.Int(title=u"Definitely not a string", default=2)
-            >>> if hasattr(IMailSettings, '_v_attrs'):
-            ...     del IMailSettings._v_attrs['sender']
-            >>> registry.registerInterface(IMailSettings)
-            >>> registry['plone.registry.tests.IMailSettings.sender']
-            2
-        
-        But let's put it back the way it was::
-        
-            >>> IMailSettings._InterfaceClass__attrs['sender'] = old_field
-            >>> if hasattr(IMailSettings, '_v_attrs'):
-            ...     del IMailSettings._v_attrs['sender']
-            >>> registry.registerInterface(IMailSettings)
-            >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
-            u'root@localhost'
-        
-        Sometimes, you may want to use an interface as a template for multiple instances of a set of fields, rather than defining them all by hand.
-        This is especially useful when you want to allow third-party packages to provide information.
-        To accomplish this, we can provide a prefix with the ``registerInterface`` call.
-        This will take precedence over the ``__identifier__`` that is usually used.
-        
-            >>> registry.registerInterface(IMailSettings, prefix="plone.registry.tests.alternativesettings")
-        
-        These values are now available in the same way as the original settings::
-        
-            >>> sender_record = registry.records['plone.registry.tests.alternativesettings.sender']
-            >>> smtp_host_record = registry.records['plone.registry.tests.alternativesettings.smtp_host']
-            >>> registry['plone.registry.tests.alternativesettings.sender'] = u'alt@example.org'
-        
-        Accessing the original interface
-        --------------------------------
-        
-        Now that we have these records, we can look up the original interface.
-        This does not break the golden rules:
-        internally, we only store the name of the interface, and resolve it at runtime.
-        
-        Records that know about interfaces are marked with ``IInterfaceAwareRecord`` and have two additional properties:
-        ``interface`` and ``fieldName``::
-        
-            >>> from plone.registry.interfaces import IInterfaceAwareRecord
-            >>> IInterfaceAwareRecord.providedBy(age_record)
-            False
-            >>> IInterfaceAwareRecord.providedBy(sender_record)
-            True
-        
-            >>> sender_record.interfaceName
-            'plone.registry.tests.IMailSettings'
-        
-            >>> sender_record.interface is IMailSettings
-            True
-        
-        Using the records proxy
-        -----------------------
-        
-        Once the records for an interface has been created, it is possible to obtain a proxy object that provides the given interface, but reads and writes its values to the registry.
-        This is useful, for example, to create a form using ``zope.formlib`` or  ``z3c.form`` that is configured with widgets based on the
-        interface.
-        Or simply as a more convenient API when working with multiple, related settings.
-        
-        ::
-        
-            >>> proxy = registry.forInterface(IMailSettings)
-            >>> proxy
-            <RecordsProxy for plone.registry.tests.IMailSettings>
-        
-        If you use your registry values in code which might be encountered on normal HTML rendering paths (e.g. in a viewlet) you need to be aware that records might not exist or they are invalid.
-        ``forInterface()`` will raise KeyError on this kind of situations::
-        
-            try:
-                proxy = registry.forInterface(IMailSettings)
-            except KeyError:
-                # Gracefully handled cases
-                # when GenericSetup installer has not been run or rerun
-                # e.g. by returning or using some default values
-                pass
-        
-        The proxy is not a persistent object on its own::
-        
-            >>> from persistent.interfaces import IPersistent
-            >>> IPersistent.providedBy(proxy)
-            False
-        
-        It does, however, provide the requisite interface::
-        
-            >>> IMailSettings.providedBy(proxy)
-            True
-        
-        You can distinguish between the proxy and a 'normal' object by checking for the ``IRecordsProxy`` marker interface::
-        
-            >>> from plone.registry.interfaces import IRecordsProxy
-            >>> IRecordsProxy.providedBy(proxy)
-            True
-        
-        When we set a value, it is stored in the registry::
-        
-            >>> proxy.smtp_host = 'http://mail.server.com'
-            >>> registry['plone.registry.tests.IMailSettings.smtp_host']
-            'http://mail.server.com'
-        
-            >>> registry['plone.registry.tests.IMailSettings.smtp_host'] = 'smtp://mail.server.com'
-            >>> proxy.smtp_host
-            'smtp://mail.server.com'
-        
-        Values not in the interface will raise an ``AttributeError``::
-        
-            >>> proxy.age
-            Traceback (most recent call last):
-            ...
-            AttributeError: age
-        
-        Note that by default, the forInterface() method will check that the necessary records have been registered.
-        For example, we cannot use any old interface::
-        
-            >>> registry.forInterface(IInterfaceAwareRecord)
-            Traceback (most recent call last):
-            ...
-            KeyError: 'Interface `plone.registry.interfaces.IInterfaceAwareRecord` defines a field `...`, for which there is no record.'
-        
-        By default, we also cannot use an interface for which only some records exist::
-        
-            >>> registry.forInterface(IMailPreferences)
-            Traceback (most recent call last):
-            ...
-            KeyError: 'Interface `plone.registry.tests.IMailPreferences` defines a field `settings`, for which there is no record.'
-        
-        It is possible to disable this check, however.
-        This will be a bit more efficient::
-        
-            >>> registry.forInterface(IMailPreferences, check=False)
-            <RecordsProxy for plone.registry.tests.IMailPreferences>
-        
-        A better way, however, is to explicitly declare that some fields are omitted::
-        
-            >>> pref_proxy = registry.forInterface(IMailPreferences, omit=('settings',))
-        
-        In this case, the omitted fields will default to their 'missing' value::
-        
-            >>> pref_proxy.settings ==  IMailPreferences['settings'].missing_value
-            True
-        
-        However, trying to set the value will result in a ``AttributeError``::
-        
-            >>> pref_proxy.settings = None
-            Traceback (most recent call last):
-            ...
-            AttributeError: settings
-        
-        To access another instance of the field, supply the prefix::
-        
-            >>> alt_proxy = registry.forInterface(IMailSettings,
-            ...     prefix="plone.registry.tests.alternativesettings")
-            >>> alt_proxy.sender  # doctest: +IGNORE_U
-            u'alt@example.org'
-        
-        Collections of records proxies
-        ------------------------------
-        
-        A collection of record sets may be accessed using ``collectionOfInterface``::
-        
-            >>> collection = registry.collectionOfInterface(IMailSettings)
-        
-        You can create a new record set::
-        
-            >>> proxy = collection.setdefault('example')
-            >>> proxy.sender = u'collection@example.org'
-            >>> proxy.smtp_host = 'smtp://mail.example.org'
-        
-        Record sets are stored based under the prefix::
-        
-            >>> prefix = IMailSettings.__identifier__
-            >>> registry.records.values(prefix+'/', prefix+'0')
-            [<Record plone.registry.tests.IMailSettings/example.sender>,
-             <Record plone.registry.tests.IMailSettings/example.smtp_host>]
-            >>> registry['plone.registry.tests.IMailSettings/example.sender']  # doctest: +IGNORE_U
-            u'collection@example.org'
-        
-        Records may be set from an existing object::
-        
-            >>> class MailSettings:
-            ...     sender = u'someone@example.com'
-            ...     smtp_host = 'smtp://mail.example.com'
-            >>> collection['example_com'] = MailSettings()
-            >>> registry.records.values(prefix+'/', prefix+'0')
-            [<Record plone.registry.tests.IMailSettings/example.sender>,
-             <Record plone.registry.tests.IMailSettings/example.smtp_host>,
-             <Record plone.registry.tests.IMailSettings/example_com.sender>,
-             <Record plone.registry.tests.IMailSettings/example_com.smtp_host>]
-        
-        The collection may be iterated over::
-        
-            >>> for name in collection: print(name)
-            example
-            example_com
-        
-        And may be deleted::
-        
-            >>> del collection['example_com']
-            >>> registry.records.values(prefix+'/', prefix+'0')
-            [<Record plone.registry.tests.IMailSettings/example.sender>,
-             <Record plone.registry.tests.IMailSettings/example.smtp_host>]
-        
-        Using field references
-        ======================
-        
-        It is possible for one record to refer to another record's field.
-        This can be used to provide a simple "override" mechanism,
-        for example, where one record defines the field and a default value,
-        whilst another provides an override validated against the same field.
-        
-        Let us first create the base record and set its value::
-        
-            >>> timeout_field = field.Int(title=u"Timeout", min=0)
-            >>> registry.records['plone.registry.tests.timeout'] = Record(timeout_field, 10)
-        
-            >>> timeout_record = registry.records['plone.registry.tests.timeout']
-            >>> timeout_record.value
-            10
-        
-        Next, we create a field reference for this record::
-        
-            >>> from plone.registry import FieldRef
-            >>> timeout_override_field = FieldRef(timeout_record.__name__, timeout_record.field)
-        
-        We can use this to create a new record::
-        
-            >>> registry.records['plone.registry.tests.timeout.override'] = Record(timeout_override_field, 20)
-            >>> timeout_override_record = registry.records['plone.registry.tests.timeout.override']
-        
-        The two values are separate::
-        
-            >>> timeout_record.value
-            10
-            >>> timeout_override_record.value
-            20
-        
-            >>> registry['plone.registry.tests.timeout']
-            10
-            >>> registry['plone.registry.tests.timeout.override']
-            20
-        
-        Validation uses the underlying field::
-        
-            >>> registry['plone.registry.tests.timeout.override'] = -1  # doctest: +SKIP_PYTHON_3
-            Traceback (most recent call last):
-            ...
-            TooSmall: (-1, 0)
-        
-            >>> registry['plone.registry.tests.timeout.override'] = -1  # doctest: +SKIP_PYTHON_2
-            Traceback (most recent call last):
-            ...
-            zope.schema._bootstrapinterfaces.TooSmall: (-1, 0)
-        
-        The reference field exposes the standard field properties, e.g.::
-        
-            >>> timeout_override_record.field.title  # doctest: +SKIP_PYTHON_3
-            u'Timeout'
-            >>> timeout_override_record.field.min
-            0
-        
-        To look up the underlying record name, we can use the ``recordName`` property::
-        
-            >>> timeout_override_record.field.recordName
-            'plone.registry.tests.timeout'
-        
-        
-        ===============
-        Registry events
-        ===============
-        
-        The registry fires certain events. These are:
-        
-        ``plone.registry.interfaces.IRecordAddedEvent``
-            when a record has been added to the registry.
-        
-        ``plone.registry.interfaces.IRecordRemovedEvent``
-            when a record has been removed from the registry.
-        
-        ``plone.registry.interfaces.IRecordModifiedEvent``,
-            when a record's value is modified.
-        
-        To test these events, we will create, modify and remove a few records::
-        
-            >>> from zope.component.eventtesting import clearEvents
-            >>> clearEvents()
-            >>> from plone.registry import Registry, Record, field
-            >>> registry = Registry()
-        
-        Adding a new record to the registry should fire ``IRecordAddedEvents``::
-        
-            >>> registry.records['plone.registry.tests.age'] = \
-            ...     Record(field.Int(title=u"Age", min=0, default=18))
-        
-            >>> registry.records['plone.registry.tests.cms'] = \
-            ...     Record(field.TextLine(title=u"Preferred CMS"), value=u"Plone")
-        
-        When creating records from an interface, one event is fired for each field in the interface::
-        
-            >>> from plone.registry.tests import IMailSettings
-            >>> registry.registerInterface(IMailSettings)
-        
-        Deleting a record should fire an ``IRecordRemovedEvent``::
-        
-            >>> del registry.records['plone.registry.tests.cms']
-        
-        Changing a record should fire an ``IRecordModifiedEvent``::
-        
-            >>> registry['plone.registry.tests.age'] = 25
-            >>> registry.records['plone.registry.tests.age'].value = 24
-        
-        Let's take a look at the events that were just fired::
-        
-            >>> from plone.registry.interfaces import IRecordEvent
-            >>> from zope.component.eventtesting import getEvents
-            >>> getEvents(IRecordEvent)
-            [<RecordAddedEvent for plone.registry.tests.age>,
-             <RecordAddedEvent for plone.registry.tests.cms>,
-             <RecordAddedEvent for plone.registry.tests.IMailSettings.sender>,
-             <RecordAddedEvent for plone.registry.tests.IMailSettings.smtp_host>,
-             <RecordRemovedEvent for plone.registry.tests.cms>,
-             <RecordModifiedEvent for plone.registry.tests.age>,
-             <RecordModifiedEvent for plone.registry.tests.age>]
-        
-        For the modified events, we can also check the value before and after the change::
-        
-            >>> from plone.registry.interfaces import IRecordModifiedEvent
-            >>> [(repr(e), e.oldValue, e.newValue,) for e in getEvents(IRecordModifiedEvent)]
-            [('<RecordModifiedEvent for plone.registry.tests.age>', 18, 25),
-             ('<RecordModifiedEvent for plone.registry.tests.age>', 25, 24)]
-        
-        IObjectEvent-style redispatchers
-        ================================
-        
-        There is a special event handler.
-        It takes care of re-dispatching registry events based on the schema interface prescribed by the record.
-        
-        Let's re-set the event testing framework and register the re-dispatching event subscriber.
-        Normally, this would happen automatically by including this package's ZCML.
-        
-        ::
-        
-            >>> clearEvents()
-            >>> from zope.component import provideHandler
-            >>> from plone.registry.events import redispatchInterfaceAwareRecordEvents
-            >>> provideHandler(redispatchInterfaceAwareRecordEvents)
-        
-        We'll then register a schema interface::
-        
-            >>> from plone.registry.tests import IMailSettings
-            >>> registry.registerInterface(IMailSettings)
-        
-        We could now register an event handler to print any record event occurring on an ``IMailSettings`` record.
-        More specialised event handlers for e.g. ``IRecordModifiedEvent`` or ``IRecordRemovedEvent`` are of course also possible.
-        Note that it is not possible to re-dispatch ``IRecordAddedEvents``, so these are never caught.
-        
-            >>> from zope.component import adapter
-            >>> @adapter(IMailSettings, IRecordEvent)
-            ... def print_mail_settings_events(proxy, event):
-            ...     print("Got %s for %s" % (event, proxy))
-            >>> provideHandler(print_mail_settings_events)
-        
-        Let's now modify one of the records for this interface.
-        The event handler should react immediately::
-        
-            >>> registry['plone.registry.tests.IMailSettings.sender'] = u"Some sender"
-            Got <RecordModifiedEvent for plone.registry.tests.IMailSettings.sender> for <RecordsProxy for plone.registry.tests.IMailSettings>
-        
-        Let's also modify a non-interface-aware record, for comparison's sake.
-        Here, there is nothing printed::
-        
-            >>> registry['plone.registry.tests.age'] = 3
-        
-        We can try a record-removed event as well::
-        
-            >>> del registry.records['plone.registry.tests.IMailSettings.sender']
-            Got <RecordRemovedEvent for plone.registry.tests.IMailSettings.sender> for <RecordsProxy for plone.registry.tests.IMailSettings>
-        
-        The basic events that have been dispatched are::
-        
-            >>> getEvents(IRecordEvent)
-            [<RecordAddedEvent for plone.registry.tests.IMailSettings.sender>,
-             <RecordAddedEvent for plone.registry.tests.IMailSettings.smtp_host>,
-             <RecordModifiedEvent for plone.registry.tests.IMailSettings.sender>,
-             <RecordModifiedEvent for plone.registry.tests.age>,
-             <RecordRemovedEvent for plone.registry.tests.IMailSettings.sender>]
-        
-        
-        =================
-        Persistent fields
-        =================
-        
-        The persistent fields that are found in ``plone.registry.field`` are siblings of the ones found in zope.schema,
-        with persistence mixed in.
-        To avoid potentially breaking the registry with persistent references to symbols that may go away,
-        we purposefully limit the number of fields supported.
-        We also disallow some properties, and add some additional checks on others.
-        
-        The standard fields
-        ===================
-        
-        We will show each supported field in turn. For all fields, note that:
-        
-        * the ``order`` property will return ``-1`` no matter what setting the ``constraint`` property is diallowed
-        * the ``key_type`` and ``value_type`` properties, where applicable, must be set to a persistent field.
-        * for ``Choice`` fields, only named vocabularies and vocabularies based on simple values are supported:
-          sources and ``IVocabulary`` objects are not.
-        
-        Imports needed::
-        
-            >>> from plone.registry import field
-            >>> from zope import schema
-            >>> from persistent import Persistent
-        
-        Bytes
-        -----
-        
-        The bytes field describes a string of bytes::
-        
-            >>> f = field.Bytes(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.Bytes)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Bytes(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint('ABC')
-            True
-        
-        BytesLine
-        ---------
-        
-        The bytes field describes a string of bytes, disallowing newlines::
-        
-            >>> f = field.BytesLine(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.BytesLine)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.BytesLine(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(b'AB\nC')
-            False
-        
-        ASCII
-        -----
-        
-        The ASCII field describes a string containing only ASCII characters::
-        
-            >>> f = field.ASCII(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.ASCII)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.ASCII(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint('ab\nc')
-            True
-        
-        ASCIILine
-        ---------
-        
-        The ASCII line field describes a string containing only ASCII characters and disallowing newlines::
-        
-            >>> f = field.ASCIILine(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.ASCIILine)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.ASCIILine(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint('ab\nc')
-            False
-        
-        Text
-        ----
-        
-        The text field describes a unicode string::
-        
-            >>> f = field.Text(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.Text)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Text(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'ab\nc')
-            True
-        
-        TextLine
-        --------
-        
-        The text line field describes a unicode string, disallowing newlines::
-        
-            >>> f = field.TextLine(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.TextLine)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.TextLine(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'ab\nc')
-            False
-        
-        Bool
-        ----
-        
-        The bool field describes a boolean::
-        
-            >>> f = field.Bool(title=u"Test")
-            >>> isinstance(f, schema.Bool)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Bool(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(False)
-            True
-        
-        Int
-        ---
-        
-        The int field describes an integer or long::
-        
-            >>> f = field.Int(title=u"Test", min=-123, max=1234)
-            >>> isinstance(f, schema.Int)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Int(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(123)
-            True
-        
-        Float
-        -----
-        
-        The float field describes a float::
-        
-            >>> f = field.Float(title=u"Test", min=-123.0, max=1234.0)
-            >>> isinstance(f, schema.Float)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Float(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(123)
-            True
-        
-        Decimal
-        -------
-        
-        The decimal field describes a decimal::
-        
-            >>> import decimal
-            >>> f = field.Decimal(title=u"Test", min=decimal.Decimal('-123.0'), max=decimal.Decimal('1234.0'))
-            >>> isinstance(f, schema.Decimal)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Decimal(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(123)
-            True
-        
-        Password
-        --------
-        
-        The password field describes a unicode string used for a password::
-        
-            >>> f = field.Password(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.Password)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Password(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'ab\nc')
-            False
-        
-        SourceText
-        ----------
-        
-        The source  text field describes a unicode string with source code::
-        
-            >>> f = field.SourceText(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.SourceText)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.SourceText(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'ab\nc')
-            True
-        
-        URI
-        ---
-        
-        The URI field describes a URI string::
-        
-            >>> f = field.URI(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.URI)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.URI(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'abc')
-            True
-        
-        Id
-        --
-        
-        The id field describes a URI string or a dotted name::
-        
-            >>> f = field.Id(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.Id)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Id(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'abc')
-            True
-        
-        DottedName
-        ----------
-        
-        The dotted name field describes a Python dotted name::
-        
-            >>> f = field.DottedName(title=u"Test", min_length=0, max_length=10)
-            >>> isinstance(f, schema.DottedName)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.DottedName(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(u'abc')
-            True
-        
-        Datetime
-        --------
-        
-        The date/time field describes a Python datetime object::
-        
-            >>> f = field.Datetime(title=u"Test")
-            >>> isinstance(f, schema.Datetime)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Datetime(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> import datetime
-            >>> f.constraint(datetime.datetime.now())
-            True
-        
-        Date
-        ----
-        
-        The date field describes a Python date object::
-        
-            >>> f = field.Date(title=u"Test")
-            >>> isinstance(f, schema.Date)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Date(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> import datetime
-            >>> f.constraint(datetime.date.today())
-            True
-        
-        Timedelta
-        ---------
-        
-        The time-delta field describes a Python timedelta object::
-        
-            >>> f = field.Timedelta(title=u"Test")
-            >>> isinstance(f, schema.Timedelta)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Timedelta(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> import datetime
-            >>> f.constraint(datetime.timedelta(1))
-            True
-        
-        Tuple
-        -----
-        
-        The tuple field describes a tuple::
-        
-            >>> f = field.Tuple(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=field.TextLine(title=u"Value"))
-            >>> isinstance(f, schema.Tuple)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Tuple(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=schema.TextLine(title=u"Value"))
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> f.value_type = schema.TextLine(title=u"Value")
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> field.Tuple(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint((1,2))
-            True
-        
-        List
-        ----
-        
-        The list field describes a tuple::
-        
-            >>> f = field.List(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=field.TextLine(title=u"Value"))
-            >>> isinstance(f, schema.List)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.List(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=schema.TextLine(title=u"Value"))
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> f.value_type = schema.TextLine(title=u"Value")
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> field.List(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint([1,2])
-            True
-        
-        Set
-        ---
-        
-        The set field describes a set::
-        
-            >>> f = field.Set(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=field.TextLine(title=u"Value"))
-            >>> isinstance(f, schema.Set)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Set(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=schema.TextLine(title=u"Value"))
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> f.value_type = schema.TextLine(title=u"Value")
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> field.Set(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(set([1,2]))
-            True
-        
-        Frozenset
-        ---------
-        
-        The set field describes a frozenset::
-        
-            >>> f = field.FrozenSet(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=field.TextLine(title=u"Value"))
-            >>> isinstance(f, schema.FrozenSet)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.FrozenSet(title=u"Test", min_length=0, max_length=10,
-            ...     value_type=schema.TextLine(title=u"Value"))
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> f.value_type = schema.TextLine(title=u"Value")
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> field.FrozenSet(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(frozenset([1,2]))
-            True
-        
-        Dict
-        ----
-        
-        The set field describes a dict::
-        
-            >>> f = field.Dict(title=u"Test", min_length=0, max_length=10,
-            ...     key_type=field.ASCII(title=u"Key"),
-            ...     value_type=field.TextLine(title=u"Value"))
-            >>> isinstance(f, schema.Dict)
-            True
-        
-            >>> f.order
-            -1
-        
-            >>> field.Dict(title=u"Test", min_length=0, max_length=10,
-            ...     key_type=schema.ASCII(title=u"Key"),
-            ...     value_type=field.TextLine(title=u"Value"))
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `key_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> f.key_type = schema.ASCII(title=u"Key")
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `key_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> field.Dict(title=u"Test", min_length=0, max_length=10,
-            ...     key_type=field.ASCII(title=u"Key"),
-            ...     value_type=schema.TextLine(title=u"Value"))
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> f.value_type = schema.TextLine(title=u"Value")
-            Traceback (most recent call last):
-            ...
-            ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
-        
-            >>> field.Dict(title=u"Test", constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint(dict())
-            True
-        
-        Choice
-        ------
-        
-        A choice field represents a selection from a vocabulary.
-        For persistent fields, the vocabulary cannot be a ``source`` or any kind of object:
-        it must either be a list of primitives, or a named vocabulary::
-        
-            >>> f = field.Choice(title=u"Test", values=[1,2,3])
-            >>> isinstance(f, schema.Choice)
-            True
-        
-            >>> f.order
-            -1
-        
-        With a list of values given, the ``vocabulary`` property returns a vocabulary
-        constructed from the values on the fly, and ``vocabularyName`` is ``None``::
-        
-            >>> f.vocabulary
-            <zope.schema.vocabulary.SimpleVocabulary object at ...>
-        
-            >>> f.vocabularyName is None
-            True
-        
-        We will get an error if we use anything other than primitives::
-        
-            >>> f = field.Choice(title=u"Test", values=[object(), object()])
-            Traceback (most recent call last):
-            ...
-            ValueError: Vocabulary values may only contain primitive values.
-        
-        If a vocabulary name given, it is stored in ``vocabularyName``, and the ``vocabulary`` property returns ``None``::
-        
-            >>> f = field.Choice(title=u"Test", vocabulary='my.vocab')
-            >>> f.vocabulary is None
-            True
-        
-            >>> f.vocabularyName
-            'my.vocab'
-        
-        Other combinations are now allowed, such as specifying no vocabulary::
-        
-            >>> field.Choice(title=u"Test")
-            Traceback (most recent call last):
-            ...
-            AssertionError: You must specify either values or vocabulary.
-        
-        Or specifying both types::
-        
-            >>> field.Choice(title=u"Test", values=[1,2,3], vocabulary='my.vocab')
-            Traceback (most recent call last):
-            ...
-            AssertionError: You cannot specify both values and vocabulary.
-        
-        Or specifying an object source::
-        
-            >>> from zope.schema.vocabulary import SimpleVocabulary
-            >>> dummy_vocabulary = SimpleVocabulary.fromValues([1,2,3])
-            >>> field.Choice(title=u"Test", source=dummy_vocabulary)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields do not support sources, only named vocabularies or vocabularies based on simple value sets.
-        
-        Or specifying an object vocabulary::
-        
-            >>> field.Choice(title=u"Test", vocabulary=dummy_vocabulary)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields only support named vocabularies or vocabularies based on simple value sets.
-        
-        As with other fields, you also cannot set a constraint::
-        
-            >>> field.Choice(title=u"Test", values=[1,2,3], constraint=lambda x: True)
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint = lambda x: False
-            Traceback (most recent call last):
-            ...
-            ValueError: Persistent fields does not support setting the `constraint` property
-        
-            >>> f.constraint('ABC')
-            True
-        
-        JSONField
-        ---------
-        
-        The set field describes a JSONField::
-        
-            >>> import plone.schema
-            >>> f = field.JSONField(title=u"Test")
-            >>> isinstance(f, plone.schema.JSONField)
-            True
-        
-            >>> f.order
-            -1
-        
-        ``IPersistentField`` adapters
-        =============================
-        
-        It is possible to adapt any non-persistent field to its related ``IPersistentField`` using the adapter factories in ``plone.registry`` fieldfactory.
-        These are set up in ``configure.zcml`` and explicitly registered in the test setup in ``tests.py``.
-        Custom adapters are of course also possible::
-        
-            >>> from plone.registry.interfaces import IPersistentField
-        
-            >>> f = schema.TextLine(title=u"Test")
-            >>> IPersistentField.providedBy(f)
-            False
-        
-            >>> p = IPersistentField(f)
-            >>> IPersistentField.providedBy(p)
-            True
-        
-            >>> isinstance(p, field.TextLine)
-            True
-        
-        Unsupported field types will not be adaptable by default::
-        
-            >>> f = schema.Object(title=u"Object", schema=IPersistentField)
-            >>> IPersistentField(f, None) is None
-            True
-        
-            >>> f = schema.InterfaceField(title=u"Interface")
-            >>> IPersistentField(f, None) is None
-            True
-        
-        After adaptation, the rules of persistent fields apply:
-        The ``order`` attribute is perpetually ``-1``.
-        Custom constraints are not allowed, and key and value type will be adapted to persistent fields as well.
-        If any of these constraints can not be met, the adaptation will fail.
-        
-        For constraints, the non-persistent value is simply ignored and the default method from the class will be used.
-        
-        ::
-        
-            >>> f = schema.TextLine(title=u"Test", constraint=lambda x: False)
-            >>> f.constraint
-            <function <lambda> at ...>
-        
-            >>> p = IPersistentField(f)
-            >>> p.constraint
-            <bound method TextLine.constraint of <plone.registry.field.TextLine object at ...>>
-        
-        The order property is similarly ignored::
-        
-            >>> f.order > 0
-            True
-        
-            >>> p.order
-            -1
-        
-        Key/value types will be adapted if possible::
-        
-            >>> f = schema.Dict(title=u"Test",
-            ...     key_type=schema.Id(title=u"Id"),
-            ...     value_type=schema.TextLine(title=u"Value"))
-            >>> p = IPersistentField(f)
-            >>> p.key_type
-            <plone.registry.field.Id object at ...>
-        
-            >>> p.value_type
-            <plone.registry.field.TextLine object at ...>
-        
-        If they cannot be adapted, there will be an error::
-        
-            >>> f = schema.Dict(title=u"Test",
-            ...     key_type=schema.Id(title=u"Id"),
-            ...     value_type=schema.Object(title=u"Value", schema=IPersistentField))
-            >>> p = IPersistentField(f)
-            Traceback (most recent call last):
-            ...
-            TypeError: ('Could not adapt', <zope.schema._field.Dict object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
-        
-            >>> f = schema.Dict(title=u"Test",
-            ...     key_type=schema.InterfaceField(title=u"Id"),
-            ...     value_type=schema.TextLine(title=u"Value"))
-            >>> p = IPersistentField(f)
-            Traceback (most recent call last):
-            ...
-            TypeError: ('Could not adapt', <zope.schema._field.Dict object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
-        
-        There is additional validation for choice fields that warrant a custom adapter.
-        These ensure that vocabularies are either stored as a list of simple values, or as named vocabularies.
-        
-        ::
-        
-            >>> f = schema.Choice(title=u"Test", values=[1,2,3])
-            >>> p = IPersistentField(f)
-            >>> p.vocabulary
-            <zope.schema.vocabulary.SimpleVocabulary object at ...>
-            >>> p._values
-            [1, 2, 3]
-            >>> p.vocabularyName is None
-            True
-        
-            >>> f = schema.Choice(title=u"Test", vocabulary='my.vocab')
-            >>> p = IPersistentField(f)
-            >>> p.vocabulary is None
-            True
-            >>> p._values is None
-            True
-            >>> p.vocabularyName
-            'my.vocab'
-        
-        Complex vocabularies or sources are not allowed::
-        
-            >>> from zope.schema.vocabulary import SimpleVocabulary
-            >>> dummy_vocabulary = SimpleVocabulary.fromItems([('a', 1), ('b', 2)])
-            >>> f = schema.Choice(title=u"Test", source=dummy_vocabulary)
-            >>> p = IPersistentField(f)
-            Traceback (most recent call last):
-            ...
-            TypeError: ('Could not adapt', <zope.schema._field.Choice object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
-        
-        
-            >>> f = schema.Choice(title=u"Test", vocabulary=dummy_vocabulary)
-            >>> p = IPersistentField(f)
-            Traceback (most recent call last):
-            ...
-            TypeError: ('Could not adapt', <zope.schema._field.Choice object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
-        
-        Changelog
-        =========
-        
-        .. You should *NOT* be adding new change log entries to this file.
-           You should create a file in the news directory instead.
-           For helpful instructions, please see:
-           https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
-        
-        .. towncrier release notes start
-        
-        1.2.1 (2021-06-14)
-        ------------------
-        
-        Bug fixes:
-        
-        
-        - Fix registry key validation regexp.
-          [jensens] (#23)
-        
-        
-        1.2.0 (2021-04-23)
-        ------------------
-        
-        New features:
-        
-        
-        - Allow plone.schema.JSONField be stored in registry (as dict-like)
-           [sneridagh] (#719)
-        
-        
-        1.1.6 (2020-04-22)
-        ------------------
-        
-        Bug fixes:
-        
-        
-        - Minor packaging updates. (#1)
-        
-        
-        1.1.5 (2018-12-14)
-        ------------------
-        
-        Bug fixes:
-        
-        - Avoid a deprecation warning that would turn into an error on Python 3.8.
-          [gforcada]
-        
-        
-        1.1.4 (2018-11-04)
-        ------------------
-        
-        Bug fixes:
-        
-        - Adapt test to changed object field in zope4
-          [pbauer]
-        
-        
-        1.1.3 (2018-06-22)
-        ------------------
-        
-        Bug fixes:
-        
-        - Improve performance of RecordsProxy.__iter__ which is now invoked more in
-          core Plone as part of the requireJS configuration
-          [MatthewWilkes]
-        
-        
-        1.1.2 (2016-12-06)
-        ------------------
-        
-        Bug fixes:
-        
-        - Fix tests to pass on Python 3.5
-          [datakurre]
-        
-        
-        1.1.1 (2016-11-19)
-        ------------------
-        
-        Bug fixes:
-        
-        - Fix endless recursion on getting values from broken records proxy objects
-          [tomgross]
-        
-        
-        1.1.0 (2016-07-05)
-        ------------------
-        
-        New features:
-        
-        - Give ``RecordsProxy`` a ``__parent__`` (the registry) in order to make it a good Zope citizen.
-          This helps in context of z3cform binders and other similar situations,
-          where a records proxy is used as context.
-          [jensens]
-        
-        
-        1.0.4 (2016-06-12)
-        ------------------
-        
-        Fixes:
-        
-        - More cleanup: PEP8, isort, readability.
-          [jensens]
-        
-        
-        1.0.3 (2016-02-26)
-        ------------------
-        
-        Fixes:
-        
-        - Replace deprecated ``zope.testing.doctestunit`` import with ``doctest``
-          module from stdlib.
-          [thet]
-        
-        - Cleanup: Pep8, utf8 headers, whitespace fixes, readability, ReST-fixes,
-          doc-style, etc.
-          [jensens]
-        
-        
-        1.0.2 (2014-09-11)
-        ------------------
-        
-        - Choice field construction compatible with a simple vocabulary of
-          string-based choices, which are converted to values on construction.
-          This provides compatibility for plone.registry/plone.app.registry
-          integration with plone.supermodel >= 1.2.5.
-          [seanupton]
-        
-        
-        1.0.1 (2013-01-13)
-        ------------------
-        
-        1.0 - 2011-05-13
-        ----------------
-        
-        - Release 1.0 Final
-          [esteele]
-        
-        - Add MANIFEST.in.
-          [WouterVH]
-        
-        
-        1.0b5 - 2011-04-06
-        ------------------
-        
-        - Make RecordsProxy type customizable through ``factory`` argument to
-          ``forInterface`` and ``collectionOfInterface``.
-          [elro]
-        
-        - Add ``collectionOfInterface`` support to registry.
-          [elro]
-        
-        - Fixed bug where prefix was ignored by registry.forInterface.
-          [elro]
-        
-        - Add optional min, max arguments for keys/values/items of _Records.
-          [elro]
-        
-        
-        1.0b4 - 2011-02-04
-        ------------------
-        
-        - Added support for field references, via the ``FieldRef`` class. See
-          ``registry.txt`` for details.
-          [optilude]
-        
-        - Change the internal persistent structure around to make it more efficient.
-          The API remains the same. Old registries will be migrated when first
-          accessed. Warning: This may lead to a "write-on-read" situation for the
-          first request in which the registry is being used.
-          [optilude]
-        
-        
-        1.0b3 - 2011-01-03
-        ------------------
-        
-         - Added prefix option to forInterface (as it was added to registerInterface)
-           [garbas]
-        
-        
-        1.0b2 - 2010-04-21
-        ------------------
-        
-        - Added support for Decimal fields
-          [optilude]
-        
-        - Add a prefix option to registerInterface to allow an interface to be used as
-          a template for a series of values, rather than single use.
-          [MatthewWilkes]
-        
-        
-        1.0b1 - 2009-08-02
-        ------------------
-        
-        - Fix a bug in bind() for Choice fields.
-          [optilude]
-        
-        
-        1.0a2 - 2009-07-12
-        ------------------
-        
-        - Changed API methods and arguments to mixedCase to be more consistent with
-          the rest of Zope. This is a non-backwards-compatible change. Our profuse
-          apologies, but it's now or never. :-/
-        
-          If you find that you get import errors or unknown keyword arguments in your
-          code, please change names from foo_bar too fooBar, e.g. for_interface()
-          becomes forInterface().
-          [optilude]
-        
-        
-        1.0a1 - 2009-04-17
-        ------------------
-        
-        - Initial release
-        
-        
 Keywords: configuration registry
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.1
-Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Provides-Extra: test
+
+============
+Introduction
+============
+This package provides debconf-like (or about:config-like) settings registries
+for Zope applications. A ``registry``, with a dict-like API, is used to get and
+set values stored in ``records``. Each record contains the actual value, as
+well as a ``field`` that describes the record in more detail. At a minimum, the
+field contains information about the type of value allowed, as well as a short
+title describing the record's purpose.
+
+.. contents:: Table of Contents
+
+
+================
+Using registries
+================
+
+You can create a new registry simply by instantiating the Registry class.
+The class and its data structures are persistent, so you can store them in the ZODB.
+You may want to provide the registry object as local utility for easy access as well, though we won't do that here.
+
+::
+
+    >>> from plone.registry import Registry
+    >>> registry = Registry()
+
+The registry starts out empty.
+To access the registry's records, you can use the ``records`` property.
+This exposes a dict API where keys are strings and values are objects providing ``IRecords``.
+
+::
+
+    >>> len(registry.records)
+    0
+
+Simple records
+==============
+
+Let's now create a record.
+A record must have a name.
+This should be a dotted name, and contain ASCII characters only.
+By convention, it should be all lowercase and start with the name of the package that defines the record.
+
+It is also possible to create a  number of records based on a single schema interface - see below.
+For now, we will focus on simple records.
+
+Before we can create the record, we must create the field that describes it.
+Fields are based on the venerable ``zope.schema`` package.
+``plone.registry`` only supports certain fields, and disallows use of a few properties even of those.
+As a rule of thumb, so long as a field stores a Python primitive, it is supported; the same goes for attributes of fields.
+
+Thus:
+
+* Fields like ``Object``, ``InterfaceField`` and so on are *not* supported.
+* A custom ``constraint`` method is *not* supported.
+* The ``order`` attribute will *always* be set to ``-1``.
+* For Choice fields, *only named vocabularies* are supported:
+  you can *not* reference a particular *source* or *source binder*.
+* The ``key_type`` and ``value_type`` properties of ``Dict``, ``List``, ``Tuple``, ``Set`` and ``Frozenset`` may *only* contain persistent fields.
+
+See section "Persistent fields" for more details.
+
+Creating a record
+-----------------
+
+The supported field types are found in the module ``plone.registry.field``.
+These are named the same as the equivalent field in ``zope.schema``, and have the same constructors.
+You must use one of these fields when creating records directly::
+
+    >>> from plone.registry import field
+    >>> age_field = field.Int(title=u"Age", min=0, default=18)
+
+    >>> from plone.registry import Record
+    >>> age_record = Record(age_field)
+
+Note that in this case, we did not supply a value.
+The value will therefore be the field default::
+
+    >>> age_record.value
+    18
+
+We can set a different value, either in the ``Record`` constructor or via the ``value`` attribute::
+
+    >>> age_record.value = 2
+    >>> age_record.value
+    2
+
+Note that the value is validated against the field::
+
+    >>> age_record.value = -1
+    Traceback (most recent call last):
+    ...
+    zope.schema._bootstrapinterfaces.TooSmall: (-1, 0)
+
+    >>> age_record.value
+    2
+
+We can now add the field to the registry.
+This is done via the ``record`` dictionary::
+
+    >>> 'plone.registry.tests.age' in registry
+    False
+    >>> registry.records['plone.registry.tests.age'] = age_record
+
+At this point, the record will gain ``__name__`` and ``__parent__`` attributes::
+
+    >>> age_record.__name__
+    'plone.registry.tests.age'
+
+    >>> age_record.__parent__ is registry
+    True
+
+Creating a record with an initial value
+---------------------------------------
+
+We can create records more succinctly in *one go* by
+
+1. creating the field,
+2. creating the Record and setting its value as and
+3. assigning it to the registry,
+
+like this::
+
+    >>> registry.records['plone.registry.tests.cms'] = \
+    ...     Record(field.TextLine(title=u"CMS of choice"), u"Plone")
+
+The record can now be obtained.
+Note that it has a nice ``__repr__`` to help debugging.
+
+    >>> registry.records['plone.registry.tests.cms']
+    <Record plone.registry.tests.cms>
+
+Accessing and manipulating record values
+----------------------------------------
+
+Once a record has been created and added to the registry,
+you can access its value through dict-like operations on the registry itself::
+
+    >>> 'plone.registry.tests.cms' in registry
+    True
+
+    >>> registry['plone.registry.tests.cms']  # doctest: +IGNORE_U
+    u'Plone'
+
+    >>> registry['plone.registry.tests.cms'] = u"Plone 3.x"
+
+Again, values are validated::
+
+    >>> registry['plone.registry.tests.cms'] = b'Joomla'
+    Traceback (most recent call last):
+    ...
+    zope.schema._bootstrapinterfaces.WrongType: (b'Joomla', <class 'str'>, 'value')
+
+There is also a ``get()`` method::
+
+    >>> registry.get('plone.registry.tests.cms')  # doctest: +IGNORE_U
+    u'Plone 3.x'
+    >>> registry.get('non-existent-key') is None
+    True
+
+Deleting records
+----------------
+
+Records may be deleted from the ``records`` property::
+
+    >>> del registry.records['plone.registry.tests.cms']
+    >>> 'plone.registry.tests.cms' in registry.records
+    False
+    >>> 'plone.registry.tests.cms' in registry
+    False
+
+Creating records from interfaces
+================================
+
+As an application developer, it is often desirable to define settings as traditional interfaces with ``zope.schema fields``.
+``plone.registry`` includes support for creating a set of records from a single interface.
+
+To test this, we have created an interface, ``IMailSettings``.
+It has two fields: ``sender`` and ``smtp_host``::
+
+    >>> from plone.registry.tests import IMailSettings
+
+Note that this contains standard fields::
+
+    >>> IMailSettings['sender']
+    <zope.schema._bootstrapfields.TextLine object at ...>
+
+    >>> IMailSettings['smtp_host']
+    <zope.schema._field.URI object at ...>
+
+We can create records from this interface like this::
+
+    >>> registry.registerInterface(IMailSettings)
+
+One record for each field in the interface has now been created.
+Their names are the full dotted names to those fields::
+
+    >>> sender_record = registry.records['plone.registry.tests.IMailSettings.sender']
+    >>> smtp_host_record = registry.records['plone.registry.tests.IMailSettings.smtp_host']
+
+The fields used in the records will be the equivalent persistent versions of the fields from the original interface::
+
+    >>> sender_record.field
+    <plone.registry.field.TextLine object at ...>
+
+    >>> smtp_host_record.field
+    <plone.registry.field.URI object at ...>
+
+This feat is accomplished internally by adapting the field to the ``IPersistentField`` interface.
+There is a default adapter factory that works for all fields defined in ``plone.registry.field``.
+You can of course define your own adapter if you have a custom field type.
+But bear in mind the golden rules of any persistent field::
+
+* The field must store only primitives or other persistent fields
+* It must not reference a function, class, interface or other method that could break if a package is uninstalled.
+
+If we have a field for which there is no ``IPersistentField`` adapter, we will get an error::
+
+    >>> from plone.registry.tests import IMailPreferences
+    >>> IMailPreferences['settings']
+    <zope.schema._bootstrapfields.Object object at ...>
+
+    >>> registry.registerInterface(IMailPreferences)
+    Traceback (most recent call last):
+    ...
+    TypeError: There is no persistent field equivalent for the field `settings` of type `Object`.
+
+Whoops!
+We can, however, tell ``registerInterface()`` to ignore one or more fields::
+
+    >>> registry.registerInterface(IMailPreferences, omit=('settings',))
+
+Once an interface's records have been registered, we can get and set their values as normal::
+
+    >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
+    u'root@localhost'
+
+    >>> registry['plone.registry.tests.IMailSettings.sender'] = u"webmaster@localhost"
+    >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
+    u'webmaster@localhost'
+
+If we sub-sequently re-register the same interface, the value will be retained if possible::
+
+    >>> registry.registerInterface(IMailSettings)
+    >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
+    u'webmaster@localhost'
+
+However, if the value is no longer valid, we will revert to the default.
+To test that, let's sneakily modify the field for a while::
+
+    >>> old_field = IMailSettings['sender']
+    >>> IMailSettings._InterfaceClass__attrs['sender'] = field.Int(title=u"Definitely not a string", default=2)
+    >>> if hasattr(IMailSettings, '_v_attrs'):
+    ...     del IMailSettings._v_attrs['sender']
+    >>> registry.registerInterface(IMailSettings)
+    >>> registry['plone.registry.tests.IMailSettings.sender']
+    2
+
+But let's put it back the way it was::
+
+    >>> IMailSettings._InterfaceClass__attrs['sender'] = old_field
+    >>> if hasattr(IMailSettings, '_v_attrs'):
+    ...     del IMailSettings._v_attrs['sender']
+    >>> registry.registerInterface(IMailSettings)
+    >>> registry['plone.registry.tests.IMailSettings.sender']  # doctest: +IGNORE_U
+    u'root@localhost'
+
+Sometimes, you may want to use an interface as a template for multiple instances of a set of fields, rather than defining them all by hand.
+This is especially useful when you want to allow third-party packages to provide information.
+To accomplish this, we can provide a prefix with the ``registerInterface`` call.
+This will take precedence over the ``__identifier__`` that is usually used.
+
+    >>> registry.registerInterface(IMailSettings, prefix="plone.registry.tests.alternativesettings")
+
+These values are now available in the same way as the original settings::
+
+    >>> sender_record = registry.records['plone.registry.tests.alternativesettings.sender']
+    >>> smtp_host_record = registry.records['plone.registry.tests.alternativesettings.smtp_host']
+    >>> registry['plone.registry.tests.alternativesettings.sender'] = u'alt@example.org'
+
+Accessing the original interface
+--------------------------------
+
+Now that we have these records, we can look up the original interface.
+This does not break the golden rules:
+internally, we only store the name of the interface, and resolve it at runtime.
+
+Records that know about interfaces are marked with ``IInterfaceAwareRecord`` and have two additional properties:
+``interface`` and ``fieldName``::
+
+    >>> from plone.registry.interfaces import IInterfaceAwareRecord
+    >>> IInterfaceAwareRecord.providedBy(age_record)
+    False
+    >>> IInterfaceAwareRecord.providedBy(sender_record)
+    True
+
+    >>> sender_record.interfaceName
+    'plone.registry.tests.IMailSettings'
+
+    >>> sender_record.interface is IMailSettings
+    True
+
+Using the records proxy
+-----------------------
+
+Once the records for an interface has been created, it is possible to obtain a proxy object that provides the given interface, but reads and writes its values to the registry.
+This is useful, for example, to create a form using ``zope.formlib`` or  ``z3c.form`` that is configured with widgets based on the
+interface.
+Or simply as a more convenient API when working with multiple, related settings.
+
+::
+
+    >>> proxy = registry.forInterface(IMailSettings)
+    >>> proxy
+    <RecordsProxy for plone.registry.tests.IMailSettings>
+
+If you use your registry values in code which might be encountered on normal HTML rendering paths (e.g. in a viewlet) you need to be aware that records might not exist or they are invalid.
+``forInterface()`` will raise KeyError on this kind of situations::
+
+    try:
+        proxy = registry.forInterface(IMailSettings)
+    except KeyError:
+        # Gracefully handled cases
+        # when GenericSetup installer has not been run or rerun
+        # e.g. by returning or using some default values
+        pass
+
+The proxy is not a persistent object on its own::
+
+    >>> from persistent.interfaces import IPersistent
+    >>> IPersistent.providedBy(proxy)
+    False
+
+It does, however, provide the requisite interface::
+
+    >>> IMailSettings.providedBy(proxy)
+    True
+
+You can distinguish between the proxy and a 'normal' object by checking for the ``IRecordsProxy`` marker interface::
+
+    >>> from plone.registry.interfaces import IRecordsProxy
+    >>> IRecordsProxy.providedBy(proxy)
+    True
+
+When we set a value, it is stored in the registry::
+
+    >>> proxy.smtp_host = 'http://mail.server.com'
+    >>> registry['plone.registry.tests.IMailSettings.smtp_host']
+    'http://mail.server.com'
+
+    >>> registry['plone.registry.tests.IMailSettings.smtp_host'] = 'smtp://mail.server.com'
+    >>> proxy.smtp_host
+    'smtp://mail.server.com'
+
+Values not in the interface will raise an ``AttributeError``::
+
+    >>> proxy.age
+    Traceback (most recent call last):
+    ...
+    AttributeError: age
+
+Note that by default, the forInterface() method will check that the necessary records have been registered.
+For example, we cannot use any old interface::
+
+    >>> registry.forInterface(IInterfaceAwareRecord)
+    Traceback (most recent call last):
+    ...
+    KeyError: 'Interface `plone.registry.interfaces.IInterfaceAwareRecord` defines a field `...`, for which there is no record.'
+
+By default, we also cannot use an interface for which only some records exist::
+
+    >>> registry.forInterface(IMailPreferences)
+    Traceback (most recent call last):
+    ...
+    KeyError: 'Interface `plone.registry.tests.IMailPreferences` defines a field `settings`, for which there is no record.'
+
+It is possible to disable this check, however.
+This will be a bit more efficient::
+
+    >>> registry.forInterface(IMailPreferences, check=False)
+    <RecordsProxy for plone.registry.tests.IMailPreferences>
+
+A better way, however, is to explicitly declare that some fields are omitted::
+
+    >>> pref_proxy = registry.forInterface(IMailPreferences, omit=('settings',))
+
+In this case, the omitted fields will default to their 'missing' value::
+
+    >>> pref_proxy.settings ==  IMailPreferences['settings'].missing_value
+    True
+
+However, trying to set the value will result in a ``AttributeError``::
+
+    >>> pref_proxy.settings = None
+    Traceback (most recent call last):
+    ...
+    AttributeError: settings
+
+To access another instance of the field, supply the prefix::
+
+    >>> alt_proxy = registry.forInterface(IMailSettings,
+    ...     prefix="plone.registry.tests.alternativesettings")
+    >>> alt_proxy.sender  # doctest: +IGNORE_U
+    u'alt@example.org'
+
+Collections of records proxies
+------------------------------
+
+A collection of record sets may be accessed using ``collectionOfInterface``::
+
+    >>> collection = registry.collectionOfInterface(IMailSettings)
+
+You can create a new record set::
+
+    >>> proxy = collection.setdefault('example')
+    >>> proxy.sender = u'collection@example.org'
+    >>> proxy.smtp_host = 'smtp://mail.example.org'
+
+Record sets are stored based under the prefix::
+
+    >>> prefix = IMailSettings.__identifier__
+    >>> registry.records.values(prefix+'/', prefix+'0')
+    [<Record plone.registry.tests.IMailSettings/example.sender>,
+     <Record plone.registry.tests.IMailSettings/example.smtp_host>]
+    >>> registry['plone.registry.tests.IMailSettings/example.sender']  # doctest: +IGNORE_U
+    u'collection@example.org'
+
+Records may be set from an existing object::
+
+    >>> class MailSettings:
+    ...     sender = u'someone@example.com'
+    ...     smtp_host = 'smtp://mail.example.com'
+    >>> collection['example_com'] = MailSettings()
+    >>> registry.records.values(prefix+'/', prefix+'0')
+    [<Record plone.registry.tests.IMailSettings/example.sender>,
+     <Record plone.registry.tests.IMailSettings/example.smtp_host>,
+     <Record plone.registry.tests.IMailSettings/example_com.sender>,
+     <Record plone.registry.tests.IMailSettings/example_com.smtp_host>]
+
+The collection may be iterated over::
+
+    >>> for name in collection: print(name)
+    example
+    example_com
+
+And may be deleted::
+
+    >>> del collection['example_com']
+    >>> registry.records.values(prefix+'/', prefix+'0')
+    [<Record plone.registry.tests.IMailSettings/example.sender>,
+     <Record plone.registry.tests.IMailSettings/example.smtp_host>]
+
+Using field references
+======================
+
+It is possible for one record to refer to another record's field.
+This can be used to provide a simple "override" mechanism,
+for example, where one record defines the field and a default value,
+whilst another provides an override validated against the same field.
+
+Let us first create the base record and set its value::
+
+    >>> timeout_field = field.Int(title=u"Timeout", min=0)
+    >>> registry.records['plone.registry.tests.timeout'] = Record(timeout_field, 10)
+
+    >>> timeout_record = registry.records['plone.registry.tests.timeout']
+    >>> timeout_record.value
+    10
+
+Next, we create a field reference for this record::
+
+    >>> from plone.registry import FieldRef
+    >>> timeout_override_field = FieldRef(timeout_record.__name__, timeout_record.field)
+
+We can use this to create a new record::
+
+    >>> registry.records['plone.registry.tests.timeout.override'] = Record(timeout_override_field, 20)
+    >>> timeout_override_record = registry.records['plone.registry.tests.timeout.override']
+
+The two values are separate::
+
+    >>> timeout_record.value
+    10
+    >>> timeout_override_record.value
+    20
+
+    >>> registry['plone.registry.tests.timeout']
+    10
+    >>> registry['plone.registry.tests.timeout.override']
+    20
+
+Validation uses the underlying field::
+
+    >>> registry['plone.registry.tests.timeout.override'] = -1
+    Traceback (most recent call last):
+    ...
+    zope.schema._bootstrapinterfaces.TooSmall: (-1, 0)
+
+The reference field exposes the standard field properties, e.g.::
+
+    >>> timeout_override_record.field.title
+    'Timeout'
+    >>> timeout_override_record.field.min
+    0
+
+To look up the underlying record name, we can use the ``recordName`` property::
+
+    >>> timeout_override_record.field.recordName
+    'plone.registry.tests.timeout'
+
+
+===============
+Registry events
+===============
+
+The registry fires certain events. These are:
+
+``plone.registry.interfaces.IRecordAddedEvent``
+    when a record has been added to the registry.
+
+``plone.registry.interfaces.IRecordRemovedEvent``
+    when a record has been removed from the registry.
+
+``plone.registry.interfaces.IRecordModifiedEvent``,
+    when a record's value is modified.
+
+To test these events, we will create, modify and remove a few records::
+
+    >>> from zope.component.eventtesting import clearEvents
+    >>> clearEvents()
+    >>> from plone.registry import Registry, Record, field
+    >>> registry = Registry()
+
+Adding a new record to the registry should fire ``IRecordAddedEvents``::
+
+    >>> registry.records['plone.registry.tests.age'] = \
+    ...     Record(field.Int(title=u"Age", min=0, default=18))
+
+    >>> registry.records['plone.registry.tests.cms'] = \
+    ...     Record(field.TextLine(title=u"Preferred CMS"), value=u"Plone")
+
+When creating records from an interface, one event is fired for each field in the interface::
+
+    >>> from plone.registry.tests import IMailSettings
+    >>> registry.registerInterface(IMailSettings)
+
+Deleting a record should fire an ``IRecordRemovedEvent``::
+
+    >>> del registry.records['plone.registry.tests.cms']
+
+Changing a record should fire an ``IRecordModifiedEvent``::
+
+    >>> registry['plone.registry.tests.age'] = 25
+    >>> registry.records['plone.registry.tests.age'].value = 24
+
+Let's take a look at the events that were just fired::
+
+    >>> from plone.registry.interfaces import IRecordEvent
+    >>> from zope.component.eventtesting import getEvents
+    >>> getEvents(IRecordEvent)
+    [<RecordAddedEvent for plone.registry.tests.age>,
+     <RecordAddedEvent for plone.registry.tests.cms>,
+     <RecordAddedEvent for plone.registry.tests.IMailSettings.sender>,
+     <RecordAddedEvent for plone.registry.tests.IMailSettings.smtp_host>,
+     <RecordRemovedEvent for plone.registry.tests.cms>,
+     <RecordModifiedEvent for plone.registry.tests.age>,
+     <RecordModifiedEvent for plone.registry.tests.age>]
+
+For the modified events, we can also check the value before and after the change::
+
+    >>> from plone.registry.interfaces import IRecordModifiedEvent
+    >>> [(repr(e), e.oldValue, e.newValue,) for e in getEvents(IRecordModifiedEvent)]
+    [('<RecordModifiedEvent for plone.registry.tests.age>', 18, 25),
+     ('<RecordModifiedEvent for plone.registry.tests.age>', 25, 24)]
+
+IObjectEvent-style redispatchers
+================================
+
+There is a special event handler.
+It takes care of re-dispatching registry events based on the schema interface prescribed by the record.
+
+Let's re-set the event testing framework and register the re-dispatching event subscriber.
+Normally, this would happen automatically by including this package's ZCML.
+
+::
+
+    >>> clearEvents()
+    >>> from zope.component import provideHandler
+    >>> from plone.registry.events import redispatchInterfaceAwareRecordEvents
+    >>> provideHandler(redispatchInterfaceAwareRecordEvents)
+
+We'll then register a schema interface::
+
+    >>> from plone.registry.tests import IMailSettings
+    >>> registry.registerInterface(IMailSettings)
+
+We could now register an event handler to print any record event occurring on an ``IMailSettings`` record.
+More specialised event handlers for e.g. ``IRecordModifiedEvent`` or ``IRecordRemovedEvent`` are of course also possible.
+Note that it is not possible to re-dispatch ``IRecordAddedEvents``, so these are never caught.
+
+    >>> from zope.component import adapter
+    >>> @adapter(IMailSettings, IRecordEvent)
+    ... def print_mail_settings_events(proxy, event):
+    ...     print("Got %s for %s" % (event, proxy))
+    >>> provideHandler(print_mail_settings_events)
+
+Let's now modify one of the records for this interface.
+The event handler should react immediately::
+
+    >>> registry['plone.registry.tests.IMailSettings.sender'] = u"Some sender"
+    Got <RecordModifiedEvent for plone.registry.tests.IMailSettings.sender> for <RecordsProxy for plone.registry.tests.IMailSettings>
+
+Let's also modify a non-interface-aware record, for comparison's sake.
+Here, there is nothing printed::
+
+    >>> registry['plone.registry.tests.age'] = 3
+
+We can try a record-removed event as well::
+
+    >>> del registry.records['plone.registry.tests.IMailSettings.sender']
+    Got <RecordRemovedEvent for plone.registry.tests.IMailSettings.sender> for <RecordsProxy for plone.registry.tests.IMailSettings>
+
+The basic events that have been dispatched are::
+
+    >>> getEvents(IRecordEvent)
+    [<RecordAddedEvent for plone.registry.tests.IMailSettings.sender>,
+     <RecordAddedEvent for plone.registry.tests.IMailSettings.smtp_host>,
+     <RecordModifiedEvent for plone.registry.tests.IMailSettings.sender>,
+     <RecordModifiedEvent for plone.registry.tests.age>,
+     <RecordRemovedEvent for plone.registry.tests.IMailSettings.sender>]
+
+
+=================
+Persistent fields
+=================
+
+The persistent fields that are found in ``plone.registry.field`` are siblings of the ones found in zope.schema,
+with persistence mixed in.
+To avoid potentially breaking the registry with persistent references to symbols that may go away,
+we purposefully limit the number of fields supported.
+We also disallow some properties, and add some additional checks on others.
+
+The standard fields
+===================
+
+We will show each supported field in turn. For all fields, note that:
+
+* the ``order`` property will return ``-1`` no matter what setting the ``constraint`` property is diallowed
+* the ``key_type`` and ``value_type`` properties, where applicable, must be set to a persistent field.
+* for ``Choice`` fields, only named vocabularies and vocabularies based on simple values are supported:
+  sources and ``IVocabulary`` objects are not.
+
+Imports needed::
+
+    >>> from plone.registry import field
+    >>> from zope import schema
+    >>> from persistent import Persistent
+
+Bytes
+-----
+
+The bytes field describes a string of bytes::
+
+    >>> f = field.Bytes(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.Bytes)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Bytes(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint('ABC')
+    True
+
+BytesLine
+---------
+
+The bytes field describes a string of bytes, disallowing newlines::
+
+    >>> f = field.BytesLine(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.BytesLine)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.BytesLine(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(b'AB\nC')
+    False
+
+ASCII
+-----
+
+The ASCII field describes a string containing only ASCII characters::
+
+    >>> f = field.ASCII(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.ASCII)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.ASCII(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint('ab\nc')
+    True
+
+ASCIILine
+---------
+
+The ASCII line field describes a string containing only ASCII characters and disallowing newlines::
+
+    >>> f = field.ASCIILine(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.ASCIILine)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.ASCIILine(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint('ab\nc')
+    False
+
+Text
+----
+
+The text field describes a unicode string::
+
+    >>> f = field.Text(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.Text)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Text(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'ab\nc')
+    True
+
+TextLine
+--------
+
+The text line field describes a unicode string, disallowing newlines::
+
+    >>> f = field.TextLine(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.TextLine)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.TextLine(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'ab\nc')
+    False
+
+Bool
+----
+
+The bool field describes a boolean::
+
+    >>> f = field.Bool(title=u"Test")
+    >>> isinstance(f, schema.Bool)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Bool(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(False)
+    True
+
+Int
+---
+
+The int field describes an integer or long::
+
+    >>> f = field.Int(title=u"Test", min=-123, max=1234)
+    >>> isinstance(f, schema.Int)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Int(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(123)
+    True
+
+Float
+-----
+
+The float field describes a float::
+
+    >>> f = field.Float(title=u"Test", min=-123.0, max=1234.0)
+    >>> isinstance(f, schema.Float)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Float(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(123)
+    True
+
+Decimal
+-------
+
+The decimal field describes a decimal::
+
+    >>> import decimal
+    >>> f = field.Decimal(title=u"Test", min=decimal.Decimal('-123.0'), max=decimal.Decimal('1234.0'))
+    >>> isinstance(f, schema.Decimal)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Decimal(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(123)
+    True
+
+Password
+--------
+
+The password field describes a unicode string used for a password::
+
+    >>> f = field.Password(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.Password)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Password(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'ab\nc')
+    False
+
+SourceText
+----------
+
+The source  text field describes a unicode string with source code::
+
+    >>> f = field.SourceText(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.SourceText)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.SourceText(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'ab\nc')
+    True
+
+URI
+---
+
+The URI field describes a URI string::
+
+    >>> f = field.URI(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.URI)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.URI(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'abc')
+    True
+
+Id
+--
+
+The id field describes a URI string or a dotted name::
+
+    >>> f = field.Id(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.Id)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Id(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'abc')
+    True
+
+DottedName
+----------
+
+The dotted name field describes a Python dotted name::
+
+    >>> f = field.DottedName(title=u"Test", min_length=0, max_length=10)
+    >>> isinstance(f, schema.DottedName)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.DottedName(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(u'abc')
+    True
+
+Datetime
+--------
+
+The date/time field describes a Python datetime object::
+
+    >>> f = field.Datetime(title=u"Test")
+    >>> isinstance(f, schema.Datetime)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Datetime(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> import datetime
+    >>> f.constraint(datetime.datetime.now())
+    True
+
+Date
+----
+
+The date field describes a Python date object::
+
+    >>> f = field.Date(title=u"Test")
+    >>> isinstance(f, schema.Date)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Date(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> import datetime
+    >>> f.constraint(datetime.date.today())
+    True
+
+Timedelta
+---------
+
+The time-delta field describes a Python timedelta object::
+
+    >>> f = field.Timedelta(title=u"Test")
+    >>> isinstance(f, schema.Timedelta)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Timedelta(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> import datetime
+    >>> f.constraint(datetime.timedelta(1))
+    True
+
+Tuple
+-----
+
+The tuple field describes a tuple::
+
+    >>> f = field.Tuple(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=field.TextLine(title=u"Value"))
+    >>> isinstance(f, schema.Tuple)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Tuple(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=schema.TextLine(title=u"Value"))
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> f.value_type = schema.TextLine(title=u"Value")
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> field.Tuple(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint((1,2))
+    True
+
+List
+----
+
+The list field describes a tuple::
+
+    >>> f = field.List(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=field.TextLine(title=u"Value"))
+    >>> isinstance(f, schema.List)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.List(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=schema.TextLine(title=u"Value"))
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> f.value_type = schema.TextLine(title=u"Value")
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> field.List(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint([1,2])
+    True
+
+Set
+---
+
+The set field describes a set::
+
+    >>> f = field.Set(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=field.TextLine(title=u"Value"))
+    >>> isinstance(f, schema.Set)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Set(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=schema.TextLine(title=u"Value"))
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> f.value_type = schema.TextLine(title=u"Value")
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> field.Set(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(set([1,2]))
+    True
+
+Frozenset
+---------
+
+The set field describes a frozenset::
+
+    >>> f = field.FrozenSet(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=field.TextLine(title=u"Value"))
+    >>> isinstance(f, schema.FrozenSet)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.FrozenSet(title=u"Test", min_length=0, max_length=10,
+    ...     value_type=schema.TextLine(title=u"Value"))
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> f.value_type = schema.TextLine(title=u"Value")
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> field.FrozenSet(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(frozenset([1,2]))
+    True
+
+Dict
+----
+
+The set field describes a dict::
+
+    >>> f = field.Dict(title=u"Test", min_length=0, max_length=10,
+    ...     key_type=field.ASCII(title=u"Key"),
+    ...     value_type=field.TextLine(title=u"Value"))
+    >>> isinstance(f, schema.Dict)
+    True
+
+    >>> f.order
+    -1
+
+    >>> field.Dict(title=u"Test", min_length=0, max_length=10,
+    ...     key_type=schema.ASCII(title=u"Key"),
+    ...     value_type=field.TextLine(title=u"Value"))
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `key_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> f.key_type = schema.ASCII(title=u"Key")
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `key_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> field.Dict(title=u"Test", min_length=0, max_length=10,
+    ...     key_type=field.ASCII(title=u"Key"),
+    ...     value_type=schema.TextLine(title=u"Value"))
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> f.value_type = schema.TextLine(title=u"Value")
+    Traceback (most recent call last):
+    ...
+    ValueError: The property `value_type` may only contain objects providing `plone.registry.interfaces.IPersistentField`.
+
+    >>> field.Dict(title=u"Test", constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint(dict())
+    True
+
+Choice
+------
+
+A choice field represents a selection from a vocabulary.
+For persistent fields, the vocabulary cannot be a ``source`` or any kind of object:
+it must either be a list of primitives, or a named vocabulary::
+
+    >>> f = field.Choice(title=u"Test", values=[1,2,3])
+    >>> isinstance(f, schema.Choice)
+    True
+
+    >>> f.order
+    -1
+
+With a list of values given, the ``vocabulary`` property returns a vocabulary
+constructed from the values on the fly, and ``vocabularyName`` is ``None``::
+
+    >>> f.vocabulary
+    <zope.schema.vocabulary.SimpleVocabulary object at ...>
+
+    >>> f.vocabularyName is None
+    True
+
+We will get an error if we use anything other than primitives::
+
+    >>> f = field.Choice(title=u"Test", values=[object(), object()])
+    Traceback (most recent call last):
+    ...
+    ValueError: Vocabulary values may only contain primitive values.
+
+If a vocabulary name given, it is stored in ``vocabularyName``, and the ``vocabulary`` property returns ``None``::
+
+    >>> f = field.Choice(title=u"Test", vocabulary='my.vocab')
+    >>> f.vocabulary is None
+    True
+
+    >>> f.vocabularyName
+    'my.vocab'
+
+Other combinations are now allowed, such as specifying no vocabulary::
+
+    >>> field.Choice(title=u"Test")
+    Traceback (most recent call last):
+    ...
+    AssertionError: You must specify either values or vocabulary.
+
+Or specifying both types::
+
+    >>> field.Choice(title=u"Test", values=[1,2,3], vocabulary='my.vocab')
+    Traceback (most recent call last):
+    ...
+    AssertionError: You cannot specify both values and vocabulary.
+
+Or specifying an object source::
+
+    >>> from zope.schema.vocabulary import SimpleVocabulary
+    >>> dummy_vocabulary = SimpleVocabulary.fromValues([1,2,3])
+    >>> field.Choice(title=u"Test", source=dummy_vocabulary)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields do not support sources, only named vocabularies or vocabularies based on simple value sets.
+
+Or specifying an object vocabulary::
+
+    >>> field.Choice(title=u"Test", vocabulary=dummy_vocabulary)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields only support named vocabularies or vocabularies based on simple value sets.
+
+As with other fields, you also cannot set a constraint::
+
+    >>> field.Choice(title=u"Test", values=[1,2,3], constraint=lambda x: True)
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint = lambda x: False
+    Traceback (most recent call last):
+    ...
+    ValueError: Persistent fields does not support setting the `constraint` property
+
+    >>> f.constraint('ABC')
+    True
+
+JSONField
+---------
+
+The set field describes a JSONField::
+
+    >>> import plone.schema
+    >>> f = field.JSONField(title=u"Test")
+    >>> isinstance(f, plone.schema.JSONField)
+    True
+
+    >>> f.order
+    -1
+
+``IPersistentField`` adapters
+=============================
+
+It is possible to adapt any non-persistent field to its related ``IPersistentField`` using the adapter factories in ``plone.registry`` fieldfactory.
+These are set up in ``configure.zcml`` and explicitly registered in the test setup in ``tests.py``.
+Custom adapters are of course also possible::
+
+    >>> from plone.registry.interfaces import IPersistentField
+
+    >>> f = schema.TextLine(title=u"Test")
+    >>> IPersistentField.providedBy(f)
+    False
+
+    >>> p = IPersistentField(f)
+    >>> IPersistentField.providedBy(p)
+    True
+
+    >>> isinstance(p, field.TextLine)
+    True
+
+Unsupported field types will not be adaptable by default::
+
+    >>> f = schema.Object(title=u"Object", schema=IPersistentField)
+    >>> IPersistentField(f, None) is None
+    True
+
+    >>> f = schema.InterfaceField(title=u"Interface")
+    >>> IPersistentField(f, None) is None
+    True
+
+After adaptation, the rules of persistent fields apply:
+The ``order`` attribute is perpetually ``-1``.
+Custom constraints are not allowed, and key and value type will be adapted to persistent fields as well.
+If any of these constraints can not be met, the adaptation will fail.
+
+For constraints, the non-persistent value is simply ignored and the default method from the class will be used.
+
+::
+
+    >>> f = schema.TextLine(title=u"Test", constraint=lambda x: False)
+    >>> f.constraint
+    <function <lambda> at ...>
+
+    >>> p = IPersistentField(f)
+    >>> p.constraint
+    <bound method TextLine.constraint of <plone.registry.field.TextLine object at ...>>
+
+The order property is similarly ignored::
+
+    >>> f.order > 0
+    True
+
+    >>> p.order
+    -1
+
+Key/value types will be adapted if possible::
+
+    >>> f = schema.Dict(title=u"Test",
+    ...     key_type=schema.Id(title=u"Id"),
+    ...     value_type=schema.TextLine(title=u"Value"))
+    >>> p = IPersistentField(f)
+    >>> p.key_type
+    <plone.registry.field.Id object at ...>
+
+    >>> p.value_type
+    <plone.registry.field.TextLine object at ...>
+
+If they cannot be adapted, there will be an error::
+
+    >>> f = schema.Dict(title=u"Test",
+    ...     key_type=schema.Id(title=u"Id"),
+    ...     value_type=schema.Object(title=u"Value", schema=IPersistentField))
+    >>> p = IPersistentField(f)
+    Traceback (most recent call last):
+    ...
+    TypeError: ('Could not adapt', <zope.schema._field.Dict object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
+
+    >>> f = schema.Dict(title=u"Test",
+    ...     key_type=schema.InterfaceField(title=u"Id"),
+    ...     value_type=schema.TextLine(title=u"Value"))
+    >>> p = IPersistentField(f)
+    Traceback (most recent call last):
+    ...
+    TypeError: ('Could not adapt', <zope.schema._field.Dict object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
+
+There is additional validation for choice fields that warrant a custom adapter.
+These ensure that vocabularies are either stored as a list of simple values, or as named vocabularies.
+
+::
+
+    >>> f = schema.Choice(title=u"Test", values=[1,2,3])
+    >>> p = IPersistentField(f)
+    >>> p.vocabulary
+    <zope.schema.vocabulary.SimpleVocabulary object at ...>
+    >>> p._values
+    [1, 2, 3]
+    >>> p.vocabularyName is None
+    True
+
+    >>> f = schema.Choice(title=u"Test", vocabulary='my.vocab')
+    >>> p = IPersistentField(f)
+    >>> p.vocabulary is None
+    True
+    >>> p._values is None
+    True
+    >>> p.vocabularyName
+    'my.vocab'
+
+Complex vocabularies or sources are not allowed::
+
+    >>> from zope.schema.vocabulary import SimpleVocabulary
+    >>> dummy_vocabulary = SimpleVocabulary.fromItems([('a', 1), ('b', 2)])
+    >>> f = schema.Choice(title=u"Test", source=dummy_vocabulary)
+    >>> p = IPersistentField(f)
+    Traceback (most recent call last):
+    ...
+    TypeError: ('Could not adapt', <zope.schema._field.Choice object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
+
+
+    >>> f = schema.Choice(title=u"Test", vocabulary=dummy_vocabulary)
+    >>> p = IPersistentField(f)
+    Traceback (most recent call last):
+    ...
+    TypeError: ('Could not adapt', <zope.schema._field.Choice object at ...>, <InterfaceClass plone.registry.interfaces.IPersistentField>)
+
+Changelog
+=========
+
+.. You should *NOT* be adding new change log entries to this file.
+   You should create a file in the news directory instead.
+   For helpful instructions, please see:
+   https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
+
+.. towncrier release notes start
+
+2.0.0 (2023-04-26)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 compatibility.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (a864b30f)
+
+
+1.2.1 (2021-06-14)
+------------------
+
+Bug fixes:
+
+
+- Fix registry key validation regexp.
+  [jensens] (#23)
+
+
+1.2.0 (2021-04-23)
+------------------
+
+New features:
+
+
+- Allow plone.schema.JSONField be stored in registry (as dict-like)
+   [sneridagh] (#719)
+
+
+1.1.6 (2020-04-22)
+------------------
+
+Bug fixes:
+
+
+- Minor packaging updates. (#1)
+
+
+1.1.5 (2018-12-14)
+------------------
+
+Bug fixes:
+
+- Avoid a deprecation warning that would turn into an error on Python 3.8.
+  [gforcada]
+
+
+1.1.4 (2018-11-04)
+------------------
+
+Bug fixes:
+
+- Adapt test to changed object field in zope4
+  [pbauer]
+
+
+1.1.3 (2018-06-22)
+------------------
+
+Bug fixes:
+
+- Improve performance of RecordsProxy.__iter__ which is now invoked more in
+  core Plone as part of the requireJS configuration
+  [MatthewWilkes]
+
+
+1.1.2 (2016-12-06)
+------------------
+
+Bug fixes:
+
+- Fix tests to pass on Python 3.5
+  [datakurre]
+
+
+1.1.1 (2016-11-19)
+------------------
+
+Bug fixes:
+
+- Fix endless recursion on getting values from broken records proxy objects
+  [tomgross]
+
+
+1.1.0 (2016-07-05)
+------------------
+
+New features:
+
+- Give ``RecordsProxy`` a ``__parent__`` (the registry) in order to make it a good Zope citizen.
+  This helps in context of z3cform binders and other similar situations,
+  where a records proxy is used as context.
+  [jensens]
+
+
+1.0.4 (2016-06-12)
+------------------
+
+Fixes:
+
+- More cleanup: PEP8, isort, readability.
+  [jensens]
+
+
+1.0.3 (2016-02-26)
+------------------
+
+Fixes:
+
+- Replace deprecated ``zope.testing.doctestunit`` import with ``doctest``
+  module from stdlib.
+  [thet]
+
+- Cleanup: Pep8, utf8 headers, whitespace fixes, readability, ReST-fixes,
+  doc-style, etc.
+  [jensens]
+
+
+1.0.2 (2014-09-11)
+------------------
+
+- Choice field construction compatible with a simple vocabulary of
+  string-based choices, which are converted to values on construction.
+  This provides compatibility for plone.registry/plone.app.registry
+  integration with plone.supermodel >= 1.2.5.
+  [seanupton]
+
+
+1.0.1 (2013-01-13)
+------------------
+
+1.0 - 2011-05-13
+----------------
+
+- Release 1.0 Final
+  [esteele]
+
+- Add MANIFEST.in.
+  [WouterVH]
+
+
+1.0b5 - 2011-04-06
+------------------
+
+- Make RecordsProxy type customizable through ``factory`` argument to
+  ``forInterface`` and ``collectionOfInterface``.
+  [elro]
+
+- Add ``collectionOfInterface`` support to registry.
+  [elro]
+
+- Fixed bug where prefix was ignored by registry.forInterface.
+  [elro]
+
+- Add optional min, max arguments for keys/values/items of _Records.
+  [elro]
+
+
+1.0b4 - 2011-02-04
+------------------
+
+- Added support for field references, via the ``FieldRef`` class. See
+  ``registry.txt`` for details.
+  [optilude]
+
+- Change the internal persistent structure around to make it more efficient.
+  The API remains the same. Old registries will be migrated when first
+  accessed. Warning: This may lead to a "write-on-read" situation for the
+  first request in which the registry is being used.
+  [optilude]
+
+
+1.0b3 - 2011-01-03
+------------------
+
+ - Added prefix option to forInterface (as it was added to registerInterface)
+   [garbas]
+
+
+1.0b2 - 2010-04-21
+------------------
+
+- Added support for Decimal fields
+  [optilude]
+
+- Add a prefix option to registerInterface to allow an interface to be used as
+  a template for a series of values, rather than single use.
+  [MatthewWilkes]
+
+
+1.0b1 - 2009-08-02
+------------------
+
+- Fix a bug in bind() for Choice fields.
+  [optilude]
+
+
+1.0a2 - 2009-07-12
+------------------
+
+- Changed API methods and arguments to mixedCase to be more consistent with
+  the rest of Zope. This is a non-backwards-compatible change. Our profuse
+  apologies, but it's now or never. :-/
+
+  If you find that you get import errors or unknown keyword arguments in your
+  code, please change names from foo_bar too fooBar, e.g. for_interface()
+  becomes forInterface().
+  [optilude]
+
+
+1.0a1 - 2009-04-17
+------------------
+
+- Initial release
+
```

### Comparing `plone.registry-1.2.1/plone.registry.egg-info/SOURCES.txt` & `plone.registry-2.0.0/plone.registry.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 docs/INSTALL.txt
 docs/LICENSE.GPL
 docs/LICENSE.txt
 plone/__init__.py
 plone.registry.egg-info/PKG-INFO
 plone.registry.egg-info/SOURCES.txt
 plone.registry.egg-info/dependency_links.txt
-plone.registry.egg-info/entry_points.txt
 plone.registry.egg-info/namespace_packages.txt
 plone.registry.egg-info/not-zip-safe
 plone.registry.egg-info/requires.txt
 plone.registry.egg-info/top_level.txt
 plone/registry/__init__.py
 plone/registry/configure.zcml
 plone/registry/events.py
```

