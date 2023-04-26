# Comparing `tmp/plone.rfc822-2.0.2.tar.gz` & `tmp/plone.rfc822-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.rfc822-2.0.2.tar", last modified: Wed Apr 22 21:18:46 2020, max compression
+gzip compressed data, was "plone.rfc822-3.0.0.tar", last modified: Wed Apr 26 21:54:14 2023, max compression
```

## Comparing `plone.rfc822-2.0.2.tar` & `plone.rfc822-3.0.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)    39069 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       70 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/CONTRIBUTING.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/plone.rfc822.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    39069 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/plone.rfc822.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/plone.rfc822.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/plone.rfc822.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)      694 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/plone.rfc822.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        5 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/plone.rfc822.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)      156 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/plone.rfc822.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/plone.rfc822.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/plone.rfc822.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      122 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1212 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1478 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1668 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/plone/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/plone/rfc822/
--rw-r--r--   0 maurits    (501) staff       (20)    14189 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/plone/rfc822/fields.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7693 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/plone/rfc822/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2922 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/plone/rfc822/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1196 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/plone/rfc822/supermodel.py
--rw-r--r--   0 maurits    (501) staff       (20)      524 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/plone/rfc822/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    10271 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/plone/rfc822/defaultfields.py
--rw-r--r--   0 maurits    (501) staff       (20)    21382 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/plone/rfc822/message.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1406 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/plone/rfc822/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     2816 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/plone/rfc822/supermodel.rst
--rw-r--r--   0 maurits    (501) staff       (20)     9806 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/plone/rfc822/_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)       80 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/plone/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       67 2020-04-22 21:18:46.000000 plone.rfc822-2.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     6930 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2562 2020-04-22 21:18:45.000000 plone.rfc822-2.0.2/CHANGES.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:54:14.864126 plone.rfc822-3.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)     2814 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    31987 2023-04-26 21:54:14.864346 plone.rfc822-3.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     6930 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:54:14.858953 plone.rfc822-3.0.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1212 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1478 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:54:14.859198 plone.rfc822-3.0.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:54:14.863927 plone.rfc822-3.0.0/plone/rfc822/
+-rw-r--r--   0 maurits    (501) staff       (20)      454 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone/rfc822/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8993 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone/rfc822/_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2936 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone/rfc822/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9970 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone/rfc822/defaultfields.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13908 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone/rfc822/fields.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7514 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone/rfc822/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    21366 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone/rfc822/message.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1211 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone/rfc822/supermodel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2816 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone/rfc822/supermodel.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1048 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone/rfc822/tests.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:54:14.861333 plone.rfc822-3.0.0/plone.rfc822.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    31987 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone.rfc822.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      655 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone.rfc822.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone.rfc822.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone.rfc822.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone.rfc822.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      185 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone.rfc822.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/plone.rfc822.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2897 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      268 2023-04-26 21:54:14.864930 plone.rfc822-3.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1794 2023-04-26 21:54:14.000000 plone.rfc822-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.rfc822-2.0.2/PKG-INFO` & `plone.rfc822-3.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,938 +1,956 @@
 Metadata-Version: 2.1
 Name: plone.rfc822
-Version: 2.0.2
+Version: 3.0.0
 Summary: RFC822 marshalling for zope.schema fields
 Home-page: https://pypi.org/project/plone.rfc822
 Author: Martin Aspeli and contributors
 Author-email: optilude@gmail.com
 License: BSD
-Description: Introduction
-        ============
-        
-        This package provides primitives for turning content objects described by ``zope.schema`` fields into RFC (2)822 style messages.
-        It utilizes the Python standard library's ``email`` module.
-        
-        It consists of:
-        
-        * A marker interface ``IPrimaryField`` which can be used to indicate the primary field of a schema.
-          The primary field will be used as the message body.
-          If there are more than one field marked as primary, the body is turned in a MIME multipart message.
-        * An interface ``IFieldMarshaler`` which describes marshalers that convert to and from strings suitable for encoding into an RFC 2822 style message.
-          These are multi-adapters on ``(context, field)``.
-          ``context`` is the content object and ``field`` is the schema field instance.
-        * Default implementations of ``IFieldMarshaler`` for the standard fields in the ``zope.schema`` package.
-        * Helper methods to construct messages from one or more schemata or a list of fields, and to parse a message and update a context object accordingly.
-        
-        The helper methods are described by ``plone.rfc822.interfaces.IMessageAPI``.
-        They are importable directly from the ``plone.rfc822`` package::
-        
-            def constructMessageFromSchema(context, schema, charset='utf-8'):
-                """Convenience method which calls ``constructMessage()`` with all the
-                fields, in order, of the given schema interface
-                """
-        
-            def constructMessageFromSchemata(context, schemata, charset='utf-8'):
-                """Convenience method which calls ``constructMessage()`` with all the
-                fields, in order, of all the given schemata (a sequence of schema
-                interfaces).
-                """
-        
-            def constructMessage(context, fields, charset='utf-8'):
-                """Helper method to construct a message.
-        
-                ``context`` is a content object.
-        
-                ``fields`` is a sequence of (name, field) pairs for the fields which make
-                up the message. This can be obtained from zope.schema.getFieldsInOrder,
-                for example.
-        
-                ``charset`` is the message charset.
-        
-                The message body will be constructed from the primary field, i.e. the
-                field which is marked with ``IPrimaryField``. If no such field exists,
-                the message will have no body. If multiple fields exist, the message will
-                be a multipart message. Otherwise, it will contain a scalar string
-                payload.
-        
-                A field will be ignored if ``(context, field)`` cannot be multi-adapted
-                to ``IFieldMarshaler``, or if the ``marshal()`` method returns None.
-                """
-        
-            def renderMessage(message, mangleFromHeader=False):
-                """Render a message to a string
-                """
-        
-            def initializeObjectFromSchema(context, schema, message, defaultCharset='utf-8'):
-                """Convenience method which calls ``initializeObject()`` with all the
-                fields, in order, of the given schema interface
-                """
-        
-            def initializeObjectFromSchemata(context, schemata, message, defaultCharset='utf-8'):
-                """Convenience method which calls ``initializeObject()`` with all the
-                fields in order, of all the given schemata (a sequence of schema
-                interfaces).
-                """
-        
-            def initializeObject(context, fields, message, defaultCharset='utf-8'):
-                """Initialise an object from a message.
-        
-                ``context`` is the content object to initialise.
-        
-                ``fields`` is a sequence of (name, field) pairs for the fields which make
-                up the message. This can be obtained from zope.schema.getFieldsInOrder,
-                for example.
-        
-                ``message`` is a ``Message`` object.
-        
-                ``defaultCharset`` is the default character set to use.
-        
-                If the message is a multipart message, the primary fields will be read
-                in order.
-                """
-        
-        The message format used adheres to the following rules:
-        
-        * All non-primary fields are represented as headers.
-          The header name is taken from the field name.
-          The value is an encoded string as returned by the ``marshal()`` method of the appropriate ``IFieldMarshal`` multi-adapter.
-        * If no ``IFieldMarshaler`` adapter can be found, the header is ignored.
-        * Similarly, if no fields are found for a given header when parsing a message, the header is ignored.
-        * If there is a single primary field, the message has a string payload, which is the marshalled value of the primary field.
-          In this case, the ``Content-Type`` header of the message will be obtained from the primary field's marshaler.
-        * If there are multiple primary fields, each is encoded into its own message, each with its own ``Content-Type`` header.
-          The outer message will have a content type of ``multipart/mixed`` and headers for other fields.
-        * A ``ValueError`` error is raised if a message is being parsed which has more or fewer parts than there are primary fields.
-        * Duplicate field names are allowed, and will be encoded as duplicate headers.
-          When parsing a message, there needs to be one field per header.
-          That is, if a message contains two headers with the name 'foo',
-          the list of field name/ instance pairs passed to the ``initializeObject()`` method should contain two pairs with the name 'foo'.
-          The first field will be used for the first header value, the second field will be used for the second header value.
-          If a third 'foo' header appears, it will be ignored.
-        * Since message headers are always lowercase, field names will be matched case-insensitively when parsing a message.
-        
-        Supermodel handler
-        ------------------
-        
-        If ``plone.supermodel`` is installed, this package  will register a namespace handler for the ``marshal`` namespace, with the URI ``http://namespaces.plone.org/supermodel/marshal``.
-        This can be used to mark a field as the primary field::
-        
-            <model xmlns="http://namespaces.plone.org/supermodel/schema"
-                   xmlns:marshal="http://namespaces.plone.org/supermodel/marshal">
-                <schema>
-                    <field type="zope.schema.Text" name="test" marshal:primary="true">
-                        <title>Test field</title>
-                    </field>
-                </schema>
-            </model>
-        
-        ``plone.supermodel`` may be installed as a dependency using the extra
-        ``[supermodel]``, but this is probably only useful for running the tests.
-        If the package is not installed, the handler will not be ignored.
-        
-        License note
-        ------------
-        
-        This package is released under the BSD license.
-        Contributors, please do not add dependencies on GPL code.
-        
-        Issue tracker
-        -------------
-        
-        Please report issues via the `Plone issue tracker`_.
-        
-        .. _`Plone issue tracker`: https://github.com/plone/plone.rfc822/issues
-        
-        Support
-        -------
-        
-        Dexterity use questions may be answered via `Plone's support channels`_.
-        
-        .. _`Plone's support channels`: http://plone.org/support
-        
-        Contributing
-        ------------
-        
-        Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.rfc822>`_.
-        
-        Contributors please read the document `Process for Plone core's development <https://docs.plone.org/develop/coredev/docs/index.html>`_
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
-        2.0.2 (2020-04-22)
-        ------------------
-        
-        Bug fixes:
-        
-        
-        - Minor packaging updates. (#1)
-        
-        
-        2.0.1 (2019-05-21)
-        ------------------
-        
-        Bug fixes:
-        
-        
-        - Use a better type check in the payload parser.
-          [Rotonen] (#7)
-        
-        
-        2.0.0 (2018-11-04)
-        ------------------
-        
-        Breaking changes:
-        
-        - Deprecate ``renderMessage(message)``,
-          use stdlibs ``message.as_string()`` from ``email.message.Message`` class instead.
-          [jensens]
-        
-        - Newline handling in MIME-headers: ``\n`` are now escaped explicit.
-          This follows RFC2822 section 3.2.2.
-          [jensens]
-        
-        - Drop support of Python 2.6
-          [jensens]
-        
-        New features:
-        
-        - ``constructMessage`` now handles base64 encoding automatically for all marshallers,
-          where ``marshaler.ascii`` is ``False`` and ``marshaler.getContentType`` is ``None``.
-          [jensens]
-        
-        - Support for Python 3+
-          Also big code overhaul included.
-          [jensens]
-        
-        
-        1.1.4 (2018-06-20)
-        ------------------
-        
-        New features:
-        
-        - Start basic Python 3 support.
-          [pbauer, dhavlik]
-        
-        
-        1.1.3 (2016-08-09)
-        ------------------
-        
-        Fixes:
-        
-        - code cleanup: pep8, isort, utf8 headers et al.
-          [jensens]
-        
-        - Use zope.interface decorator.
-          [gforcada]
-        
-        
-        1.1.2 (2016-02-21)
-        ------------------
-        
-        Fixes:
-        
-        - Fix test isolation problem.
-          [thet]
-        
-        - Replace deprecated ``zope.testing.doctest`` import with ``doctest`` module from stdlib.
-          [thet]
-        
-        
-        1.1.1 (2015-03-21)
-        ------------------
-        
-        - Update test to reflect the change in the representation of the model namespaces by adding the 18n xml namespace.
-          [sneridagh]
-        
-        - Make sure the tests do not fail if messages contain a trailing blank line. This fixes test failures on Ubuntu 14.04.
-          [timo]
-        
-        
-        1.1 (2013-08-14)
-        ----------------
-        
-        - Branch for Plone 4.2/4.3 compatibility changes.
-          [esteele]
-        
-        
-        1.0.2 (2013-07-28)
-        ------------------
-        
-        - Marshall collections as ASCII when possible.
-          [davisagli]
-        
-        - Add support for marshalling decimal fields.
-          [davisagli]
-        
-        1.0.1 (2013-01-01)
-        ------------------
-        
-        1.0 (2011-05-20)
-        ----------------
-        
-        * Relicensed under the BSD license.
-          See http://plone.org/foundation/materials/foundation-resolutions/plone-framework-components-relicensing-policy
-          [davisagli]
-        
-        1.0b2 (2011-02-11)
-        ------------------
-        
-        * Add IPrimaryFieldInfo to look up primary field information on a content item.
-        
-        1.0b1 (2009-10-08)
-        ------------------
-        
-        * Initial release
-        
-        Message construction and parsing
-        ================================
-        
-        This package contains helper methods to construct an RFC 2822 style message
-        from a list of schema fields, and to parse a message and initialise an object
-        based on its headers and body payload.
-        
-        Before we begin, let's load the default field marshalers and configure
-        annotations, which we will use later in this test::
-        
-            >>> configuration = u"""\
-            ... <configure
-            ...      xmlns="http://namespaces.zope.org/zope"
-            ...      i18n_domain="plone.rfc822.tests">
-            ...
-            ...     <include package="zope.component" file="meta.zcml" />
-            ...     <include package="zope.annotation" />
-            ...
-            ...     <include package="plone.rfc822" />
-            ...
-            ... </configure>
-            ... """
-        
-        ::
-        
-            >>> from six import StringIO
-            >>> from zope.configuration import xmlconfig
-            >>> xmlconfig.xmlconfig(StringIO(configuration))
-        
-        The primary field
-        -----------------
-        
-        The message body is assumed to originate from a "primary" field, which is
-        indicated via a marker interface.
-        
-        To illustrate the pattern, consider the following schema interface::
-        
-            >>> from zope.interface import Interface, alsoProvides
-            >>> from plone.rfc822.interfaces import IPrimaryField
-            >>> from zope import schema
-        
-            >>> class ITestContent(Interface):
-            ...
-            ...     title = schema.TextLine(title=u"Title")
-            ...     description = schema.Text(title=u"Description")
-            ...     body = schema.Text(title=u"Body text")
-            ...     emptyfield = schema.TextLine(title=u"Empty field", missing_value=u'missing')
-        
-        The primary field instance is marked like this::
-        
-            >>> alsoProvides(ITestContent['body'], IPrimaryField)
-        
-        Constructing a message
-        ----------------------
-        
-        Let's now say we have an instance providing this interface, which we want to
-        marshal to a message::
-        
-            >>> from zope.interface import implementer
-            >>> @implementer(ITestContent)
-            ... class TestContent(object):
-            ...     title = ""
-            ...     description = ""
-            ...     body = ""
-            ...     emptyfield = None
-        
-            >>> content = TestContent()
-            >>> content.title = "Test title"
-            >>> content.description = """Täst description
-            ... with a newline"""
-            >>> content.body = "<p>Test body</p>"
-        
-        We could create a message from this instance and schema like this::
-        
-            >>> from plone.rfc822 import constructMessageFromSchema
-            >>> msg = constructMessageFromSchema(content, ITestContent)
-        
-        The output looks like this::
-        
-            >>> print(msg.as_string())
-            title: Test title
-            description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
-            emptyfield:
-            Content-Type: text/plain; charset="utf-8"
-            <BLANKLINE>
-            <p>Test body</p>
-        
-        Notice how the non-ASCII header values are UTF-8 encoded.
-        The encoding algorithm is clever enough to only encode the value if it is necessary,
-        leaving more readable field values otherwise.
-        
-        The body here is of the default message type::
-        
-            >>> msg.get_default_type()
-            'text/plain'
-        
-        This is because none of the default field types manage a content type.
-        
-        The body is also utf-8 encoded, because the primary field specified this
-        encoding.
-        
-        If we want to use a different content type, we could set it explicitly::
-        
-            >>> msg.set_type('text/html')
-            >>> print(msg.as_string())
-            title: Test title
-            description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
-            emptyfield:
-            MIME-Version: 1.0
-            Content-Type: text/html; charset="utf-8"
-            <BLANKLINE>
-            <p>Test body</p>
-        
-        Alternatively, if we know that any ``IText`` field on an object providing
-        our ``ITestContent`` interface always stores HTML, could register a custom
-        ``IFieldMarshaler`` adapter which would indicate this to the message
-        constructor. Let's take a look at that now.
-        
-        Custom marshalers
-        -----------------
-        
-        The default marshaler can be obtained by multi-adapting the content object
-        and the field instance to ``IFieldMarshaler``:
-        
-            >>> from zope.component import getMultiAdapter
-            >>> from plone.rfc822.interfaces import IFieldMarshaler
-            >>> getMultiAdapter((content, ITestContent['body'],), IFieldMarshaler)
-            <plone.rfc822.defaultfields.UnicodeValueFieldMarshaler object at ...>
-        
-        Let's now create our own marshaler by extending this class and overriding
-        the ``getContentType()``:
-        
-            >>> from plone.rfc822.defaultfields import UnicodeValueFieldMarshaler
-            >>> from zope.schema.interfaces import IText
-            >>> from zope.component import adapter
-        
-            >>> @adapter(ITestContent, IText)
-            ... class TestBodyMarshaler(UnicodeValueFieldMarshaler):
-            ...     def getContentType(self):
-            ...         return 'text/html'
-        
-        Ordinarily, we'd register this with ZCML. For the purpose of the test, we'll
-        register it using the ``zope.component`` API.
-        
-            >>> from zope.component import provideAdapter
-            >>> provideAdapter(TestBodyMarshaler)
-        
-        Hint: If the schema contained multiple text fields, this adapter would apply
-        to all of them. To avoid that, we could either mark the field with a custom
-        marker interface (similary to the way we marked a field with ``IPrimaryField``
-        above), or have the marshaler check the field name.
-        
-        Let's now try again:
-        
-            >>> msg = constructMessageFromSchema(content, ITestContent)
-            >>> print(msg.as_string())
-            title: Test title
-            description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
-            emptyfield:
-            MIME-Version: 1.0
-            Content-Type: text/html; charset="utf-8"
-            <BLANKLINE>
-            <p>Test body</p>
-        
-        Notice how the Content-Type has changed.
-        
-        Consuming a message
-        -------------------
-        
-        A message can be used to initialise an object. The object has to be
-        constructed first:
-        
-            >>> newContent = TestContent()
-        
-        We then need to obtain a ``Message`` object. The ``email`` module contains
-        helper functions for this purpose.
-        
-            >>> messageBody = """\
-            ... title: Test title
-            ... description: =?utf-8?q?Test_description=0D=0Awith_a_newline?=
-            ... Content-Type: text/html
-            ...
-            ... <p>Test body</p>"""
-        
-            >>> from email import message_from_string
-            >>> msg = message_from_string(messageBody)
-        
-        The message can now be used to initialise the object according to the given
-        schema. This should be the same schema as the one used to construct the
-        message.
-        
-            >>> from plone.rfc822 import initializeObjectFromSchema
-            >>> initializeObjectFromSchema(newContent, ITestContent, msg)
-        
-            >>> newContent.title
-            'Test title'
-            >>> print(newContent.description)
-            Test description
-            with a newline
-        
-            >>> newContent.body
-            '<p>Test body</p>'
-        
-        We can also consume messages with a transfer encoding and a charset:
-        
-            >>> messageBody = """\
-            ... title: =?utf-8?q?Test_title?=
-            ... description: =?utf-8?q?Test_description=0D=0Awith_a_newline?=
-            ... emptyfield:
-            ... Content-Transfer-Encoding: base64
-            ... Content-Type: text/html; charset="utf-8"
-            ... <BLANKLINE>
-            ... PHA+VGVzdCBib2R5PC9wPg==
-            ... <BLANKLINE>"""
-        
-            >>> msg = message_from_string(messageBody)
-            >>> msg.get_content_type()
-            'text/html'
-            >>> msg.get_content_charset()
-            'utf-8'
-        
-            >>> initializeObjectFromSchema(newContent, ITestContent, msg)
-        
-            >>> newContent.title
-            'Test title'
-            >>> print(newContent.description)
-            Test description
-            with a newline
-            >>> newContent.body
-            '<p>Test body</p>'
-        
-        Note: Empty fields will result in the field's ``missing_value`` being used:
-        
-            >>> newContent.emptyfield
-            'missing'
-        
-        Handling multiple primary fields and duplicate field names
-        ----------------------------------------------------------
-        
-        It is possible that our type could have multiple primary fields or even
-        duplicate field names.
-        
-        For example, consider the following schema interface, intended to be used
-        in an annotation adapter:
-        
-            >>> class IPersonalDetails(Interface):
-            ...     description = schema.Text(title=u"Personal description")
-            ...     currentAge = schema.Int(title=u"Age", min=0)
-            ...     personalProfile = schema.Text(title=u"Profile")
-        
-            >>> alsoProvides(IPersonalDetails['personalProfile'], IPrimaryField)
-        
-        The annotation storage would look like this:
-        
-            >>> from persistent import Persistent
-            >>> @implementer(IPersonalDetails)
-            ... @adapter(ITestContent)
-            ... class PersonalDetailsAnnotation(Persistent):
-            ...
-            ...     def __init__(self):
-            ...         self.description = None
-            ...         self.currentAge = None
-            ...         self.personalProfile = None
-        
-            >>> from zope.annotation.factory import factory
-            >>> provideAdapter(factory(PersonalDetailsAnnotation))
-        
-        We should now be able to adapt a content instance to IPersonalDetails,
-        provided it is annotatable.
-        
-            >>> from zope.annotation.interfaces import IAttributeAnnotatable
-            >>> alsoProvides(content, IAttributeAnnotatable)
-        
-            >>> personalDetails = IPersonalDetails(content)
-            >>> personalDetails.description = u"<p>My description</p>"
-            >>> personalDetails.currentAge = 21
-            >>> personalDetails.personalProfile = u"<p>My profile</p>"
-        
-        The default marshalers will attempt to adapt the context to the schema of
-        a given field before getting or setting a value. If we pass multiple schemata
-        (or a combined sequence of fields) to the message constructor, it will
-        handle both duplicate field names (as duplicate headers) and multiple primary
-        fields (as multipart message attachments).
-        
-        Here are the fields it will see:
-        
-            >>> from zope.schema import getFieldsInOrder
-            >>> allFields = getFieldsInOrder(ITestContent) + \
-            ...             getFieldsInOrder(IPersonalDetails)
-        
-            >>> [f[0] for f in allFields]
-            ['title', 'description', 'body', 'emptyfield', 'description', 'currentAge', 'personalProfile']
-        
-            >>> [f[0] for f in allFields if IPrimaryField.providedBy(f[1])]
-            ['body', 'personalProfile']
-        
-        Let's now construct a message. Since we now have two fields called
-        ``description``, we will get two headers by that name. Since we have two
-        primary fields, we will get a multipart message with two attachments::
-        
-            >>> from plone.rfc822 import constructMessageFromSchemata
-            >>> msg = constructMessageFromSchemata(content, (ITestContent, IPersonalDetails,))
-            >>> msgString = msg.as_string()
-            >>> print(msgString)
-            title: Test title
-            description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
-            emptyfield:
-            description: <p>My description</p>
-            currentAge: 21
-            MIME-Version: 1.0
-            Content-Type: multipart/mixed; boundary="===============...=="
-            <BLANKLINE>
-            --===============...==
-            MIME-Version: 1.0
-            Content-Type: text/html; charset="utf-8"
-            <BLANKLINE>
-            <p>Test body</p>
-            --===============...==
-            MIME-Version: 1.0
-            Content-Type: text/html; charset="utf-8"
-            <BLANKLINE>
-            <p>My profile</p>
-            --===============...==--
-            <BLANKLINE>
-        
-        
-        (Note that we've used ellipses here for the doctest to work with the generated
-        boundary string).
-        
-        Notice how both messages have a MIME type of 'text/html' and no charset.
-        That is because of the custom adapter for ``(ITestContent, IText)`` which we
-        registered earlier.
-        
-        We can obviously read this message as well. Note that in this case, the order
-        of fields passed to ``initializeObject()`` is important, both to determine
-        which field gets which ``description`` header, and to match the two
-        attachments to the two primary fields:
-        
-            >>> newContent = TestContent()
-            >>> alsoProvides(newContent, IAttributeAnnotatable)
-        
-            >>> from plone.rfc822 import initializeObjectFromSchemata
-            >>> msg = message_from_string(msgString)
-            >>> initializeObjectFromSchemata(newContent, [ITestContent, IPersonalDetails], msg)
-        
-            >>> newContent.title
-            'Test title'
-        
-            >>> newContent.marker = True
-            >>> newContent.description
-            'T\xe4st description\nwith a newline'
-        
-            >>> newContent.body
-            '<p>Test body</p>'
-        
-            >>> newPersonalDetails = IPersonalDetails(newContent)
-            >>> newPersonalDetails.description
-            '<p>My description</p>'
-        
-            >>> newPersonalDetails.currentAge
-            21
-        
-            >>> newPersonalDetails.personalProfile
-            '<p>My profile</p>'
-        
-        Alternative ways to deal with multiple schemata
-        -----------------------------------------------
-        
-        In the example above, we created a single enveloping message with headers
-        corresponding to the fields in both our schemata, and only the primary fields
-        separated out into different attached payloads.
-        
-        An alternative approach would be to separate each schema out into its
-        own multipart message. To do that, we would simply use the
-        ``constructMessage()`` function multiple times.
-        
-            >>> mainMessage = constructMessageFromSchema(content, ITestContent)
-            >>> personalDetailsMessage = constructMessageFromSchema(content, IPersonalDetails)
-        
-            >>> from email.mime.multipart import MIMEMultipart
-            >>> envelope = MIMEMultipart()
-            >>> envelope.attach(mainMessage)
-            >>> envelope.attach(personalDetailsMessage)
-        
-            >>> envelopeString = envelope.as_string()
-            >>> print(envelopeString)
-            Content-Type: multipart/mixed; boundary="===============...=="
-            MIME-Version: 1.0
-            <BLANKLINE>
-            --===============...==
-            title: Test title
-            description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
-            emptyfield:
-            MIME-Version: 1.0
-            Content-Type: text/html; charset="utf-8"
-            <BLANKLINE>
-            <p>Test body</p>
-            --===============...==
-            description: <p>My description</p>
-            currentAge: 21
-            MIME-Version: 1.0
-            Content-Type: text/html; charset="utf-8"
-            <BLANKLINE>
-            <p>My profile</p>
-            --===============...==--...
-        
-        Which approach works best will depend largely on the intended recipient of
-        the message.
-        
-        Encoding the payload and handling filenames
-        -------------------------------------------
-        
-        Finally, let's consider a more complex example, inspired by the field
-        marshaler in ``plone.namedfile``.
-        
-        Let's say we have a value type intended to represent a binary file with a
-        filename and content type:
-        
-            >>> from zope.interface import Interface, implementer
-            >>> from zope import schema
-        
-            >>> class IFileValue(Interface):
-            ...     data = schema.Bytes(title=u"Raw data")
-            ...     contentType = schema.ASCIILine(title=u"MIME type")
-            ...     filename = schema.ASCIILine(title=u"Filename")
-        
-            >>> @implementer(IFileValue)
-            ... class FileValue(object):
-            ...
-            ...     def __init__(self, data, contentType, filename):
-            ...         self.data = data
-            ...         self.contentType = contentType
-            ...         self.filename = filename
-        
-        Suppose we had a custom field type to represent this:
-        
-            >>> from zope.schema.interfaces import IObject
-            >>> class IFileField(IObject):
-            ...     pass
-        
-            >>> @implementer(IFileField)
-            ... class FileField(schema.Object):
-            ...     schema = IFileValue
-            ...     def __init__(self, **kw):
-            ...         if 'schema' in kw:
-            ...             self.schema = kw.pop('schema')
-            ...         super(FileField, self).__init__(schema=self.schema, **kw)
-        
-        We can register a field marshaler for this field which will do the following:
-        
-        * Insist that the field is only used as a primary field, since it makes
-          little sense to encode a binary file in a header.
-        * Save the filename in a Content-Disposition header.
-        * Be capable of reading the filename again from this header.
-        * Encode the payload using base64
-        
-            >>> from plone.rfc822.interfaces import IFieldMarshaler
-            >>> from email.encoders import encode_base64
-        
-            >>> from zope.component import adapter
-            >>> from plone.rfc822.defaultfields import BaseFieldMarshaler
-        
-            >>> @adapter(Interface, IFileField)
-            ... class FileFieldMarshaler(BaseFieldMarshaler):
-            ...
-            ...     ascii = False
-            ...
-            ...     def encode(self, value, charset='utf-8', primary=False):
-            ...         if not primary:
-            ...             raise ValueError("File field cannot be marshaled as a non-primary field")
-            ...         if value is None:
-            ...             return None
-            ...         return value.data
-            ...
-            ...     def decode(self, value, message=None, charset='utf-8', contentType=None, primary=False):
-            ...         filename = None
-            ...         # get the filename from the Content-Disposition header if possible
-            ...         if primary and message is not None:
-            ...             filename = message.get_filename(None)
-            ...         return FileValue(value, contentType, filename)
-            ...
-            ...     def getContentType(self):
-            ...         value = self._query()
-            ...         if value is None:
-            ...             return None
-            ...         return value.contentType
-            ...
-            ...     def getCharset(self, default='utf-8'):
-            ...         return None # this is not text data!
-            ...
-            ...     def postProcessMessage(self, message):
-            ...         value = self._query()
-            ...         if value is not None:
-            ...             filename = value.filename
-            ...             if filename:
-            ...                 # Add a new header storing the filename if we have one
-            ...                 message.add_header('Content-Disposition', 'attachment', filename=filename)
-        
-            >>> from zope.component import provideAdapter
-            >>> provideAdapter(FileFieldMarshaler)
-        
-        To illustrate marshaling, let's create a content object that contains two file
-        fields.
-        
-            >>> class IFileContent(Interface):
-            ...     file1 = FileField()
-            ...     file2 = FileField()
-        
-            >>> @implementer(IFileContent)
-            ... class FileContent(object):
-            ...     file1 = None
-            ...     file2 = None
-        
-            >>> fileContent = FileContent()
-            >>> fileContent.file1 = FileValue('dummy file', 'text/plain', 'dummy1.txt')
-            >>> fileContent.file2 = FileValue('<html><body>test</body></html>', 'text/html', 'dummy2.html')
-        
-        At this point, neither of these fields is marked as a primary field. Let's see
-        what happens when we attempt to construct a message from this schema.
-        
-            >>> from plone.rfc822 import constructMessageFromSchema
-            >>> message = constructMessageFromSchema(fileContent, IFileContent)
-            >>> print(message.as_string())
-            <BLANKLINE>
-            <BLANKLINE>
-        
-        As expected, we got no message headers and no message body. Let's now mark one
-        field as primary:
-        
-            >>> from plone.rfc822.interfaces import IPrimaryField
-            >>> from zope.interface import alsoProvides
-            >>> alsoProvides(IFileContent['file1'], IPrimaryField)
-        
-            >>> message = constructMessageFromSchema(fileContent, IFileContent)
-            >>> messageBody = message.as_string()
-            >>> print(messageBody)
-            MIME-Version: 1.0
-            Content-Type: text/plain
-            Content-Transfer-Encoding: base64
-            Content-Disposition: attachment; filename="dummy1.txt"
-            <BLANKLINE>
-            ZHVtbXkgZmlsZQ==
-        
-        Here, we have a base64 encoded payload, a Content-Disposition header, and a
-        Content-Type header according to the primary field.
-        
-        We can also reconstruct the object from this message.
-        
-            >>> from plone.rfc822 import initializeObjectFromSchema
-            >>> from email import message_from_string
-        
-            >>> inputMessage = message_from_string(messageBody)
-            >>> newFileContent = FileContent()
-            >>> initializeObjectFromSchema(newFileContent, IFileContent, inputMessage)
-        
-            >>> newFileContent.file1.data
-            'dummy file'
-            >>> newFileContent.file1.contentType
-            'text/plain'
-            >>> newFileContent.file1.filename
-            'dummy1.txt'
-        
-            >>> newFileContent.file2 is None
-            True
-        
-        Let's now show what would happen if we encoded both files in the message.
-        In this case, we should get a multipart document with two payloads.
-        
-            >>> alsoProvides(IFileContent['file2'], IPrimaryField)
-            >>> message = constructMessageFromSchema(fileContent, IFileContent)
-            >>> messageBody = message.as_string()
-            >>> print(messageBody) # doctest: +ELLIPSIS
-            MIME-Version: 1.0
-            Content-Type: multipart/mixed; boundary="===============...=="
-            <BLANKLINE>
-            --===============...==
-            MIME-Version: 1.0
-            Content-Type: text/plain
-            Content-Transfer-Encoding: base64
-            Content-Disposition: attachment; filename="dummy1.txt"
-            <BLANKLINE>
-            ZHVtbXkgZmlsZQ==
-            --===============...==
-            MIME-Version: 1.0
-            Content-Type: text/html
-            Content-Transfer-Encoding: base64
-            Content-Disposition: attachment; filename="dummy2.html"
-            <BLANKLINE>
-            PGh0bWw+PGJvZHk+dGVzdDwvYm9keT48L2h0bWw+
-            --===============...==--...
-        
-        And again, we can reconstruct the object, this time with both fields:
-        
-            >>> inputMessage = message_from_string(messageBody)
-            >>> newFileContent = FileContent()
-            >>> initializeObjectFromSchema(newFileContent, IFileContent, inputMessage)
-        
-            >>> newFileContent.file1.data
-            'dummy file'
-            >>> newFileContent.file1.contentType
-            'text/plain'
-            >>> newFileContent.file1.filename
-            'dummy1.txt'
-        
-            >>> newFileContent.file2.data
-            '<html><body>test</body></html>'
-            >>> newFileContent.file2.contentType
-            'text/html'
-            >>> newFileContent.file2.filename
-            'dummy2.html'
-        
-        Specialities between Py2 and Py3
-        --------------------------------
-        
-        Test a special behavior which is different between Python 2 and 3 stdlib:
-        Newline handling in non-utf8 strings.
-        
-        Python 2.7 ``email.header`` keeps a line with an escaped value,
-        while Python 3.6 turns it into RFC2047 encoded headers, see https://tools.ietf.org/html/rfc2047.html
-        Technical both is fine.
-        
-        ::
-        
-            >>> import six
-            >>> content.description = "Test content\nwith newline difference"
-            >>> msg = constructMessageFromSchema(content, ITestContent)
-            >>> effective_output = msg.as_string()
-            >>> effective_output.split('\n')[1]
-            'description: =?utf-8?q?Test_content=5Cnwith_newline_difference?='
-        
 Keywords: zope schema rfc822
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
-Provides-Extra: test
+Requires-Python: >=3.8
 Provides-Extra: supermodel
+Provides-Extra: test
+
+Introduction
+============
+
+This package provides primitives for turning content objects described by ``zope.schema`` fields into RFC (2)822 style messages.
+It utilizes the Python standard library's ``email`` module.
+
+It consists of:
+
+* A marker interface ``IPrimaryField`` which can be used to indicate the primary field of a schema.
+  The primary field will be used as the message body.
+  If there are more than one field marked as primary, the body is turned in a MIME multipart message.
+* An interface ``IFieldMarshaler`` which describes marshalers that convert to and from strings suitable for encoding into an RFC 2822 style message.
+  These are multi-adapters on ``(context, field)``.
+  ``context`` is the content object and ``field`` is the schema field instance.
+* Default implementations of ``IFieldMarshaler`` for the standard fields in the ``zope.schema`` package.
+* Helper methods to construct messages from one or more schemata or a list of fields, and to parse a message and update a context object accordingly.
+
+The helper methods are described by ``plone.rfc822.interfaces.IMessageAPI``.
+They are importable directly from the ``plone.rfc822`` package::
+
+    def constructMessageFromSchema(context, schema, charset='utf-8'):
+        """Convenience method which calls ``constructMessage()`` with all the
+        fields, in order, of the given schema interface
+        """
+
+    def constructMessageFromSchemata(context, schemata, charset='utf-8'):
+        """Convenience method which calls ``constructMessage()`` with all the
+        fields, in order, of all the given schemata (a sequence of schema
+        interfaces).
+        """
+
+    def constructMessage(context, fields, charset='utf-8'):
+        """Helper method to construct a message.
+
+        ``context`` is a content object.
+
+        ``fields`` is a sequence of (name, field) pairs for the fields which make
+        up the message. This can be obtained from zope.schema.getFieldsInOrder,
+        for example.
+
+        ``charset`` is the message charset.
+
+        The message body will be constructed from the primary field, i.e. the
+        field which is marked with ``IPrimaryField``. If no such field exists,
+        the message will have no body. If multiple fields exist, the message will
+        be a multipart message. Otherwise, it will contain a scalar string
+        payload.
+
+        A field will be ignored if ``(context, field)`` cannot be multi-adapted
+        to ``IFieldMarshaler``, or if the ``marshal()`` method returns None.
+        """
+
+    def renderMessage(message, mangleFromHeader=False):
+        """Render a message to a string
+        """
+
+    def initializeObjectFromSchema(context, schema, message, defaultCharset='utf-8'):
+        """Convenience method which calls ``initializeObject()`` with all the
+        fields, in order, of the given schema interface
+        """
+
+    def initializeObjectFromSchemata(context, schemata, message, defaultCharset='utf-8'):
+        """Convenience method which calls ``initializeObject()`` with all the
+        fields in order, of all the given schemata (a sequence of schema
+        interfaces).
+        """
+
+    def initializeObject(context, fields, message, defaultCharset='utf-8'):
+        """Initialise an object from a message.
+
+        ``context`` is the content object to initialise.
+
+        ``fields`` is a sequence of (name, field) pairs for the fields which make
+        up the message. This can be obtained from zope.schema.getFieldsInOrder,
+        for example.
+
+        ``message`` is a ``Message`` object.
+
+        ``defaultCharset`` is the default character set to use.
+
+        If the message is a multipart message, the primary fields will be read
+        in order.
+        """
+
+The message format used adheres to the following rules:
+
+* All non-primary fields are represented as headers.
+  The header name is taken from the field name.
+  The value is an encoded string as returned by the ``marshal()`` method of the appropriate ``IFieldMarshal`` multi-adapter.
+* If no ``IFieldMarshaler`` adapter can be found, the header is ignored.
+* Similarly, if no fields are found for a given header when parsing a message, the header is ignored.
+* If there is a single primary field, the message has a string payload, which is the marshalled value of the primary field.
+  In this case, the ``Content-Type`` header of the message will be obtained from the primary field's marshaler.
+* If there are multiple primary fields, each is encoded into its own message, each with its own ``Content-Type`` header.
+  The outer message will have a content type of ``multipart/mixed`` and headers for other fields.
+* A ``ValueError`` error is raised if a message is being parsed which has more or fewer parts than there are primary fields.
+* Duplicate field names are allowed, and will be encoded as duplicate headers.
+  When parsing a message, there needs to be one field per header.
+  That is, if a message contains two headers with the name 'foo',
+  the list of field name/ instance pairs passed to the ``initializeObject()`` method should contain two pairs with the name 'foo'.
+  The first field will be used for the first header value, the second field will be used for the second header value.
+  If a third 'foo' header appears, it will be ignored.
+* Since message headers are always lowercase, field names will be matched case-insensitively when parsing a message.
+
+Supermodel handler
+------------------
+
+If ``plone.supermodel`` is installed, this package  will register a namespace handler for the ``marshal`` namespace, with the URI ``http://namespaces.plone.org/supermodel/marshal``.
+This can be used to mark a field as the primary field::
+
+    <model xmlns="http://namespaces.plone.org/supermodel/schema"
+           xmlns:marshal="http://namespaces.plone.org/supermodel/marshal">
+        <schema>
+            <field type="zope.schema.Text" name="test" marshal:primary="true">
+                <title>Test field</title>
+            </field>
+        </schema>
+    </model>
+
+``plone.supermodel`` may be installed as a dependency using the extra
+``[supermodel]``, but this is probably only useful for running the tests.
+If the package is not installed, the handler will not be ignored.
+
+License note
+------------
+
+This package is released under the BSD license.
+Contributors, please do not add dependencies on GPL code.
+
+Issue tracker
+-------------
+
+Please report issues via the `Plone issue tracker`_.
+
+.. _`Plone issue tracker`: https://github.com/plone/plone.rfc822/issues
+
+Support
+-------
+
+Dexterity use questions may be answered via `Plone's support channels`_.
+
+.. _`Plone's support channels`: http://plone.org/support
+
+Contributing
+------------
+
+Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.rfc822>`_.
+
+Contributors please read the document `Process for Plone core's development <https://docs.plone.org/develop/coredev/docs/index.html>`_
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
+3.0.0 (2023-04-26)
+------------------
+
+Breaking changes:
+
+
+- Remove long deprecated `renderMessage` function.
+  [@jensens] (1-1)
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
+2.0.2 (2020-04-22)
+------------------
+
+Bug fixes:
+
+
+- Minor packaging updates. (#1)
+
+
+2.0.1 (2019-05-21)
+------------------
+
+Bug fixes:
+
+
+- Use a better type check in the payload parser.
+  [Rotonen] (#7)
+
+
+2.0.0 (2018-11-04)
+------------------
+
+Breaking changes:
+
+- Deprecate ``renderMessage(message)``,
+  use stdlibs ``message.as_string()`` from ``email.message.Message`` class instead.
+  [jensens]
+
+- Newline handling in MIME-headers: ``\n`` are now escaped explicit.
+  This follows RFC2822 section 3.2.2.
+  [jensens]
+
+- Drop support of Python 2.6
+  [jensens]
+
+New features:
+
+- ``constructMessage`` now handles base64 encoding automatically for all marshallers,
+  where ``marshaler.ascii`` is ``False`` and ``marshaler.getContentType`` is ``None``.
+  [jensens]
+
+- Support for Python 3+
+  Also big code overhaul included.
+  [jensens]
+
+
+1.1.4 (2018-06-20)
+------------------
+
+New features:
+
+- Start basic Python 3 support.
+  [pbauer, dhavlik]
+
+
+1.1.3 (2016-08-09)
+------------------
+
+Fixes:
+
+- code cleanup: pep8, isort, utf8 headers et al.
+  [jensens]
+
+- Use zope.interface decorator.
+  [gforcada]
+
+
+1.1.2 (2016-02-21)
+------------------
+
+Fixes:
+
+- Fix test isolation problem.
+  [thet]
+
+- Replace deprecated ``zope.testing.doctest`` import with ``doctest`` module from stdlib.
+  [thet]
+
+
+1.1.1 (2015-03-21)
+------------------
+
+- Update test to reflect the change in the representation of the model namespaces by adding the 18n xml namespace.
+  [sneridagh]
+
+- Make sure the tests do not fail if messages contain a trailing blank line. This fixes test failures on Ubuntu 14.04.
+  [timo]
+
+
+1.1 (2013-08-14)
+----------------
+
+- Branch for Plone 4.2/4.3 compatibility changes.
+  [esteele]
+
+
+1.0.2 (2013-07-28)
+------------------
+
+- Marshall collections as ASCII when possible.
+  [davisagli]
+
+- Add support for marshalling decimal fields.
+  [davisagli]
+
+1.0.1 (2013-01-01)
+------------------
+
+1.0 (2011-05-20)
+----------------
+
+* Relicensed under the BSD license.
+  See http://plone.org/foundation/materials/foundation-resolutions/plone-framework-components-relicensing-policy
+  [davisagli]
+
+1.0b2 (2011-02-11)
+------------------
+
+* Add IPrimaryFieldInfo to look up primary field information on a content item.
+
+1.0b1 (2009-10-08)
+------------------
+
+* Initial release
+
+Message construction and parsing
+================================
+
+This package contains helper methods to construct an RFC 2822 style message
+from a list of schema fields, and to parse a message and initialise an object
+based on its headers and body payload.
+
+Before we begin, let's load the default field marshalers and configure
+annotations, which we will use later in this test::
+
+    >>> configuration = u"""\
+    ... <configure
+    ...      xmlns="http://namespaces.zope.org/zope"
+    ...      i18n_domain="plone.rfc822.tests">
+    ...
+    ...     <include package="zope.component" file="meta.zcml" />
+    ...     <include package="zope.annotation" />
+    ...
+    ...     <include package="plone.rfc822" />
+    ...
+    ... </configure>
+    ... """
+
+::
+
+    >>> from io import StringIO
+    >>> from zope.configuration import xmlconfig
+    >>> xmlconfig.xmlconfig(StringIO(configuration))
+
+The primary field
+-----------------
+
+The message body is assumed to originate from a "primary" field, which is
+indicated via a marker interface.
+
+To illustrate the pattern, consider the following schema interface::
+
+    >>> from zope.interface import Interface, alsoProvides
+    >>> from plone.rfc822.interfaces import IPrimaryField
+    >>> from zope import schema
+
+    >>> class ITestContent(Interface):
+    ...
+    ...     title = schema.TextLine(title=u"Title")
+    ...     description = schema.Text(title=u"Description")
+    ...     body = schema.Text(title=u"Body text")
+    ...     emptyfield = schema.TextLine(title=u"Empty field", missing_value=u'missing')
+
+The primary field instance is marked like this::
+
+    >>> alsoProvides(ITestContent['body'], IPrimaryField)
+
+Constructing a message
+----------------------
+
+Let's now say we have an instance providing this interface, which we want to
+marshal to a message::
+
+    >>> from zope.interface import implementer
+    >>> @implementer(ITestContent)
+    ... class TestContent(object):
+    ...     title = ""
+    ...     description = ""
+    ...     body = ""
+    ...     emptyfield = None
+
+    >>> content = TestContent()
+    >>> content.title = "Test title"
+    >>> content.description = """Täst description
+    ... with a newline"""
+    >>> content.body = "<p>Test body</p>"
+
+We could create a message from this instance and schema like this::
+
+    >>> from plone.rfc822 import constructMessageFromSchema
+    >>> msg = constructMessageFromSchema(content, ITestContent)
+
+The output looks like this::
+
+    >>> print(msg.as_string())
+    title: Test title
+    description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
+    emptyfield:
+    Content-Type: text/plain; charset="utf-8"
+    <BLANKLINE>
+    <p>Test body</p>
+
+Notice how the non-ASCII header values are UTF-8 encoded.
+The encoding algorithm is clever enough to only encode the value if it is necessary,
+leaving more readable field values otherwise.
+
+The body here is of the default message type::
+
+    >>> msg.get_default_type()
+    'text/plain'
+
+This is because none of the default field types manage a content type.
+
+The body is also utf-8 encoded, because the primary field specified this
+encoding.
+
+If we want to use a different content type, we could set it explicitly::
+
+    >>> msg.set_type('text/html')
+    >>> print(msg.as_string())
+    title: Test title
+    description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
+    emptyfield:
+    MIME-Version: 1.0
+    Content-Type: text/html; charset="utf-8"
+    <BLANKLINE>
+    <p>Test body</p>
+
+Alternatively, if we know that any ``IText`` field on an object providing
+our ``ITestContent`` interface always stores HTML, could register a custom
+``IFieldMarshaler`` adapter which would indicate this to the message
+constructor. Let's take a look at that now.
+
+Custom marshalers
+-----------------
+
+The default marshaler can be obtained by multi-adapting the content object
+and the field instance to ``IFieldMarshaler``:
+
+    >>> from zope.component import getMultiAdapter
+    >>> from plone.rfc822.interfaces import IFieldMarshaler
+    >>> getMultiAdapter((content, ITestContent['body'],), IFieldMarshaler)
+    <plone.rfc822.defaultfields.UnicodeValueFieldMarshaler object at ...>
+
+Let's now create our own marshaler by extending this class and overriding
+the ``getContentType()``:
+
+    >>> from plone.rfc822.defaultfields import UnicodeValueFieldMarshaler
+    >>> from zope.schema.interfaces import IText
+    >>> from zope.component import adapter
+
+    >>> @adapter(ITestContent, IText)
+    ... class TestBodyMarshaler(UnicodeValueFieldMarshaler):
+    ...     def getContentType(self):
+    ...         return 'text/html'
+
+Ordinarily, we'd register this with ZCML. For the purpose of the test, we'll
+register it using the ``zope.component`` API.
+
+    >>> from zope.component import provideAdapter
+    >>> provideAdapter(TestBodyMarshaler)
+
+Hint: If the schema contained multiple text fields, this adapter would apply
+to all of them. To avoid that, we could either mark the field with a custom
+marker interface (similarly to the way we marked a field with ``IPrimaryField``
+above), or have the marshaler check the field name.
+
+Let's now try again:
+
+    >>> msg = constructMessageFromSchema(content, ITestContent)
+    >>> print(msg.as_string())
+    title: Test title
+    description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
+    emptyfield:
+    MIME-Version: 1.0
+    Content-Type: text/html; charset="utf-8"
+    <BLANKLINE>
+    <p>Test body</p>
+
+Notice how the Content-Type has changed.
+
+Consuming a message
+-------------------
+
+A message can be used to initialise an object. The object has to be
+constructed first:
+
+    >>> newContent = TestContent()
+
+We then need to obtain a ``Message`` object. The ``email`` module contains
+helper functions for this purpose.
+
+    >>> messageBody = """\
+    ... title: Test title
+    ... description: =?utf-8?q?Test_description=0D=0Awith_a_newline?=
+    ... Content-Type: text/html
+    ...
+    ... <p>Test body</p>"""
+
+    >>> from email import message_from_string
+    >>> msg = message_from_string(messageBody)
+
+The message can now be used to initialise the object according to the given
+schema. This should be the same schema as the one used to construct the
+message.
+
+    >>> from plone.rfc822 import initializeObjectFromSchema
+    >>> initializeObjectFromSchema(newContent, ITestContent, msg)
+
+    >>> newContent.title
+    'Test title'
+    >>> print(newContent.description)
+    Test description
+    with a newline
+
+    >>> newContent.body
+    '<p>Test body</p>'
+
+We can also consume messages with a transfer encoding and a charset:
+
+    >>> messageBody = """\
+    ... title: =?utf-8?q?Test_title?=
+    ... description: =?utf-8?q?Test_description=0D=0Awith_a_newline?=
+    ... emptyfield:
+    ... Content-Transfer-Encoding: base64
+    ... Content-Type: text/html; charset="utf-8"
+    ... <BLANKLINE>
+    ... PHA+VGVzdCBib2R5PC9wPg==
+    ... <BLANKLINE>"""
+
+    >>> msg = message_from_string(messageBody)
+    >>> msg.get_content_type()
+    'text/html'
+    >>> msg.get_content_charset()
+    'utf-8'
+
+    >>> initializeObjectFromSchema(newContent, ITestContent, msg)
+
+    >>> newContent.title
+    'Test title'
+    >>> print(newContent.description)
+    Test description
+    with a newline
+    >>> newContent.body
+    '<p>Test body</p>'
+
+Note: Empty fields will result in the field's ``missing_value`` being used:
+
+    >>> newContent.emptyfield
+    'missing'
+
+Handling multiple primary fields and duplicate field names
+----------------------------------------------------------
+
+It is possible that our type could have multiple primary fields or even
+duplicate field names.
+
+For example, consider the following schema interface, intended to be used
+in an annotation adapter:
+
+    >>> class IPersonalDetails(Interface):
+    ...     description = schema.Text(title=u"Personal description")
+    ...     currentAge = schema.Int(title=u"Age", min=0)
+    ...     personalProfile = schema.Text(title=u"Profile")
+
+    >>> alsoProvides(IPersonalDetails['personalProfile'], IPrimaryField)
+
+The annotation storage would look like this:
+
+    >>> from persistent import Persistent
+    >>> @implementer(IPersonalDetails)
+    ... @adapter(ITestContent)
+    ... class PersonalDetailsAnnotation(Persistent):
+    ...
+    ...     def __init__(self):
+    ...         self.description = None
+    ...         self.currentAge = None
+    ...         self.personalProfile = None
+
+    >>> from zope.annotation.factory import factory
+    >>> provideAdapter(factory(PersonalDetailsAnnotation))
+
+We should now be able to adapt a content instance to IPersonalDetails,
+provided it is annotatable.
+
+    >>> from zope.annotation.interfaces import IAttributeAnnotatable
+    >>> alsoProvides(content, IAttributeAnnotatable)
+
+    >>> personalDetails = IPersonalDetails(content)
+    >>> personalDetails.description = u"<p>My description</p>"
+    >>> personalDetails.currentAge = 21
+    >>> personalDetails.personalProfile = u"<p>My profile</p>"
+
+The default marshalers will attempt to adapt the context to the schema of
+a given field before getting or setting a value. If we pass multiple schemata
+(or a combined sequence of fields) to the message constructor, it will
+handle both duplicate field names (as duplicate headers) and multiple primary
+fields (as multipart message attachments).
+
+Here are the fields it will see:
+
+    >>> from zope.schema import getFieldsInOrder
+    >>> allFields = getFieldsInOrder(ITestContent) + \
+    ...             getFieldsInOrder(IPersonalDetails)
+
+    >>> [f[0] for f in allFields]
+    ['title', 'description', 'body', 'emptyfield', 'description', 'currentAge', 'personalProfile']
+
+    >>> [f[0] for f in allFields if IPrimaryField.providedBy(f[1])]
+    ['body', 'personalProfile']
+
+Let's now construct a message. Since we now have two fields called
+``description``, we will get two headers by that name. Since we have two
+primary fields, we will get a multipart message with two attachments::
+
+    >>> from plone.rfc822 import constructMessageFromSchemata
+    >>> msg = constructMessageFromSchemata(content, (ITestContent, IPersonalDetails,))
+    >>> msgString = msg.as_string()
+    >>> print(msgString)
+    title: Test title
+    description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
+    emptyfield:
+    description: <p>My description</p>
+    currentAge: 21
+    MIME-Version: 1.0
+    Content-Type: multipart/mixed; boundary="===============...=="
+    <BLANKLINE>
+    --===============...==
+    MIME-Version: 1.0
+    Content-Type: text/html; charset="utf-8"
+    <BLANKLINE>
+    <p>Test body</p>
+    --===============...==
+    MIME-Version: 1.0
+    Content-Type: text/html; charset="utf-8"
+    <BLANKLINE>
+    <p>My profile</p>
+    --===============...==--
+    <BLANKLINE>
+
+
+(Note that we've used ellipses here for the doctest to work with the generated
+boundary string).
+
+Notice how both messages have a MIME type of 'text/html' and no charset.
+That is because of the custom adapter for ``(ITestContent, IText)`` which we
+registered earlier.
+
+We can obviously read this message as well. Note that in this case, the order
+of fields passed to ``initializeObject()`` is important, both to determine
+which field gets which ``description`` header, and to match the two
+attachments to the two primary fields:
+
+    >>> newContent = TestContent()
+    >>> alsoProvides(newContent, IAttributeAnnotatable)
+
+    >>> from plone.rfc822 import initializeObjectFromSchemata
+    >>> msg = message_from_string(msgString)
+    >>> initializeObjectFromSchemata(newContent, [ITestContent, IPersonalDetails], msg)
+
+    >>> newContent.title
+    'Test title'
+
+    >>> newContent.marker = True
+    >>> newContent.description
+    'T\xe4st description\nwith a newline'
+
+    >>> newContent.body
+    '<p>Test body</p>'
+
+    >>> newPersonalDetails = IPersonalDetails(newContent)
+    >>> newPersonalDetails.description
+    '<p>My description</p>'
+
+    >>> newPersonalDetails.currentAge
+    21
+
+    >>> newPersonalDetails.personalProfile
+    '<p>My profile</p>'
+
+Alternative ways to deal with multiple schemata
+-----------------------------------------------
+
+In the example above, we created a single enveloping message with headers
+corresponding to the fields in both our schemata, and only the primary fields
+separated out into different attached payloads.
+
+An alternative approach would be to separate each schema out into its
+own multipart message. To do that, we would simply use the
+``constructMessage()`` function multiple times.
+
+    >>> mainMessage = constructMessageFromSchema(content, ITestContent)
+    >>> personalDetailsMessage = constructMessageFromSchema(content, IPersonalDetails)
+
+    >>> from email.mime.multipart import MIMEMultipart
+    >>> envelope = MIMEMultipart()
+    >>> envelope.attach(mainMessage)
+    >>> envelope.attach(personalDetailsMessage)
+
+    >>> envelopeString = envelope.as_string()
+    >>> print(envelopeString)
+    Content-Type: multipart/mixed; boundary="===============...=="
+    MIME-Version: 1.0
+    <BLANKLINE>
+    --===============...==
+    title: Test title
+    description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
+    emptyfield:
+    MIME-Version: 1.0
+    Content-Type: text/html; charset="utf-8"
+    <BLANKLINE>
+    <p>Test body</p>
+    --===============...==
+    description: <p>My description</p>
+    currentAge: 21
+    MIME-Version: 1.0
+    Content-Type: text/html; charset="utf-8"
+    <BLANKLINE>
+    <p>My profile</p>
+    --===============...==--...
+
+Which approach works best will depend largely on the intended recipient of
+the message.
+
+Encoding the payload and handling filenames
+-------------------------------------------
+
+Finally, let's consider a more complex example, inspired by the field
+marshaler in ``plone.namedfile``.
+
+Let's say we have a value type intended to represent a binary file with a
+filename and content type:
+
+    >>> from zope.interface import Interface, implementer
+    >>> from zope import schema
+
+    >>> class IFileValue(Interface):
+    ...     data = schema.Bytes(title=u"Raw data")
+    ...     contentType = schema.ASCIILine(title=u"MIME type")
+    ...     filename = schema.ASCIILine(title=u"Filename")
+
+    >>> @implementer(IFileValue)
+    ... class FileValue(object):
+    ...
+    ...     def __init__(self, data, contentType, filename):
+    ...         self.data = data
+    ...         self.contentType = contentType
+    ...         self.filename = filename
+
+Suppose we had a custom field type to represent this:
+
+    >>> from zope.schema.interfaces import IObject
+    >>> class IFileField(IObject):
+    ...     pass
+
+    >>> @implementer(IFileField)
+    ... class FileField(schema.Object):
+    ...     schema = IFileValue
+    ...     def __init__(self, **kw):
+    ...         if 'schema' in kw:
+    ...             self.schema = kw.pop('schema')
+    ...         super(FileField, self).__init__(schema=self.schema, **kw)
+
+We can register a field marshaler for this field which will do the following:
+
+* Insist that the field is only used as a primary field, since it makes
+  little sense to encode a binary file in a header.
+* Save the filename in a Content-Disposition header.
+* Be capable of reading the filename again from this header.
+* Encode the payload using base64
+
+    >>> from plone.rfc822.interfaces import IFieldMarshaler
+    >>> from email.encoders import encode_base64
+
+    >>> from zope.component import adapter
+    >>> from plone.rfc822.defaultfields import BaseFieldMarshaler
+
+    >>> @adapter(Interface, IFileField)
+    ... class FileFieldMarshaler(BaseFieldMarshaler):
+    ...
+    ...     ascii = False
+    ...
+    ...     def encode(self, value, charset='utf-8', primary=False):
+    ...         if not primary:
+    ...             raise ValueError("File field cannot be marshaled as a non-primary field")
+    ...         if value is None:
+    ...             return None
+    ...         return value.data
+    ...
+    ...     def decode(self, value, message=None, charset='utf-8', contentType=None, primary=False):
+    ...         filename = None
+    ...         # get the filename from the Content-Disposition header if possible
+    ...         if primary and message is not None:
+    ...             filename = message.get_filename(None)
+    ...         return FileValue(value, contentType, filename)
+    ...
+    ...     def getContentType(self):
+    ...         value = self._query()
+    ...         if value is None:
+    ...             return None
+    ...         return value.contentType
+    ...
+    ...     def getCharset(self, default='utf-8'):
+    ...         return None # this is not text data!
+    ...
+    ...     def postProcessMessage(self, message):
+    ...         value = self._query()
+    ...         if value is not None:
+    ...             filename = value.filename
+    ...             if filename:
+    ...                 # Add a new header storing the filename if we have one
+    ...                 message.add_header('Content-Disposition', 'attachment', filename=filename)
+
+    >>> from zope.component import provideAdapter
+    >>> provideAdapter(FileFieldMarshaler)
+
+To illustrate marshaling, let's create a content object that contains two file
+fields.
+
+    >>> class IFileContent(Interface):
+    ...     file1 = FileField()
+    ...     file2 = FileField()
+
+    >>> @implementer(IFileContent)
+    ... class FileContent(object):
+    ...     file1 = None
+    ...     file2 = None
+
+    >>> fileContent = FileContent()
+    >>> fileContent.file1 = FileValue('dummy file', 'text/plain', 'dummy1.txt')
+    >>> fileContent.file2 = FileValue('<html><body>test</body></html>', 'text/html', 'dummy2.html')
+
+At this point, neither of these fields is marked as a primary field. Let's see
+what happens when we attempt to construct a message from this schema.
+
+    >>> from plone.rfc822 import constructMessageFromSchema
+    >>> message = constructMessageFromSchema(fileContent, IFileContent)
+    >>> print(message.as_string())
+    <BLANKLINE>
+    <BLANKLINE>
+
+As expected, we got no message headers and no message body. Let's now mark one
+field as primary:
+
+    >>> from plone.rfc822.interfaces import IPrimaryField
+    >>> from zope.interface import alsoProvides
+    >>> alsoProvides(IFileContent['file1'], IPrimaryField)
+
+    >>> message = constructMessageFromSchema(fileContent, IFileContent)
+    >>> messageBody = message.as_string()
+    >>> print(messageBody)
+    MIME-Version: 1.0
+    Content-Type: text/plain
+    Content-Transfer-Encoding: base64
+    Content-Disposition: attachment; filename="dummy1.txt"
+    <BLANKLINE>
+    ZHVtbXkgZmlsZQ==
+
+Here, we have a base64 encoded payload, a Content-Disposition header, and a
+Content-Type header according to the primary field.
+
+We can also reconstruct the object from this message.
+
+    >>> from plone.rfc822 import initializeObjectFromSchema
+    >>> from email import message_from_string
+
+    >>> inputMessage = message_from_string(messageBody)
+    >>> newFileContent = FileContent()
+    >>> initializeObjectFromSchema(newFileContent, IFileContent, inputMessage)
+
+    >>> newFileContent.file1.data
+    b'dummy file'
+    >>> newFileContent.file1.contentType
+    'text/plain'
+    >>> newFileContent.file1.filename
+    'dummy1.txt'
+
+    >>> newFileContent.file2 is None
+    True
+
+Let's now show what would happen if we encoded both files in the message.
+In this case, we should get a multipart document with two payloads.
+
+    >>> alsoProvides(IFileContent['file2'], IPrimaryField)
+    >>> message = constructMessageFromSchema(fileContent, IFileContent)
+    >>> messageBody = message.as_string()
+    >>> print(messageBody) # doctest: +ELLIPSIS
+    MIME-Version: 1.0
+    Content-Type: multipart/mixed; boundary="===============...=="
+    <BLANKLINE>
+    --===============...==
+    MIME-Version: 1.0
+    Content-Type: text/plain
+    Content-Transfer-Encoding: base64
+    Content-Disposition: attachment; filename="dummy1.txt"
+    <BLANKLINE>
+    ZHVtbXkgZmlsZQ==
+    --===============...==
+    MIME-Version: 1.0
+    Content-Type: text/html
+    Content-Transfer-Encoding: base64
+    Content-Disposition: attachment; filename="dummy2.html"
+    <BLANKLINE>
+    PGh0bWw+PGJvZHk+dGVzdDwvYm9keT48L2h0bWw+
+    --===============...==--...
+
+And again, we can reconstruct the object, this time with both fields:
+
+    >>> inputMessage = message_from_string(messageBody)
+    >>> newFileContent = FileContent()
+    >>> initializeObjectFromSchema(newFileContent, IFileContent, inputMessage)
+
+    >>> newFileContent.file1.data
+    b'dummy file'
+    >>> newFileContent.file1.contentType
+    'text/plain'
+    >>> newFileContent.file1.filename
+    'dummy1.txt'
+
+    >>> newFileContent.file2.data
+    b'<html><body>test</body></html>'
+    >>> newFileContent.file2.contentType
+    'text/html'
+    >>> newFileContent.file2.filename
+    'dummy2.html'
+
+Specialities between Py2 and Py3
+--------------------------------
+
+Test a special behavior which is different between Python 2 and 3 stdlib:
+Newline handling in non-utf8 strings.
+
+Python 2.7 ``email.header`` keeps a line with an escaped value,
+while Python 3.6 turns it into RFC2047 encoded headers, see https://tools.ietf.org/html/rfc2047.html
+Technical both is fine.
+
+::
+
+    >>> content.description = "Test content\nwith newline difference"
+    >>> msg = constructMessageFromSchema(content, ITestContent)
+    >>> effective_output = msg.as_string()
+    >>> effective_output.split('\n')[1]
+    'description: =?utf-8?q?Test_content=5Cnwith_newline_difference?='
```

### Comparing `plone.rfc822-2.0.2/plone.rfc822.egg-info/PKG-INFO` & `plone.rfc822-3.0.0/plone.rfc822.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,938 +1,956 @@
 Metadata-Version: 2.1
 Name: plone.rfc822
-Version: 2.0.2
+Version: 3.0.0
 Summary: RFC822 marshalling for zope.schema fields
 Home-page: https://pypi.org/project/plone.rfc822
 Author: Martin Aspeli and contributors
 Author-email: optilude@gmail.com
 License: BSD
-Description: Introduction
-        ============
-        
-        This package provides primitives for turning content objects described by ``zope.schema`` fields into RFC (2)822 style messages.
-        It utilizes the Python standard library's ``email`` module.
-        
-        It consists of:
-        
-        * A marker interface ``IPrimaryField`` which can be used to indicate the primary field of a schema.
-          The primary field will be used as the message body.
-          If there are more than one field marked as primary, the body is turned in a MIME multipart message.
-        * An interface ``IFieldMarshaler`` which describes marshalers that convert to and from strings suitable for encoding into an RFC 2822 style message.
-          These are multi-adapters on ``(context, field)``.
-          ``context`` is the content object and ``field`` is the schema field instance.
-        * Default implementations of ``IFieldMarshaler`` for the standard fields in the ``zope.schema`` package.
-        * Helper methods to construct messages from one or more schemata or a list of fields, and to parse a message and update a context object accordingly.
-        
-        The helper methods are described by ``plone.rfc822.interfaces.IMessageAPI``.
-        They are importable directly from the ``plone.rfc822`` package::
-        
-            def constructMessageFromSchema(context, schema, charset='utf-8'):
-                """Convenience method which calls ``constructMessage()`` with all the
-                fields, in order, of the given schema interface
-                """
-        
-            def constructMessageFromSchemata(context, schemata, charset='utf-8'):
-                """Convenience method which calls ``constructMessage()`` with all the
-                fields, in order, of all the given schemata (a sequence of schema
-                interfaces).
-                """
-        
-            def constructMessage(context, fields, charset='utf-8'):
-                """Helper method to construct a message.
-        
-                ``context`` is a content object.
-        
-                ``fields`` is a sequence of (name, field) pairs for the fields which make
-                up the message. This can be obtained from zope.schema.getFieldsInOrder,
-                for example.
-        
-                ``charset`` is the message charset.
-        
-                The message body will be constructed from the primary field, i.e. the
-                field which is marked with ``IPrimaryField``. If no such field exists,
-                the message will have no body. If multiple fields exist, the message will
-                be a multipart message. Otherwise, it will contain a scalar string
-                payload.
-        
-                A field will be ignored if ``(context, field)`` cannot be multi-adapted
-                to ``IFieldMarshaler``, or if the ``marshal()`` method returns None.
-                """
-        
-            def renderMessage(message, mangleFromHeader=False):
-                """Render a message to a string
-                """
-        
-            def initializeObjectFromSchema(context, schema, message, defaultCharset='utf-8'):
-                """Convenience method which calls ``initializeObject()`` with all the
-                fields, in order, of the given schema interface
-                """
-        
-            def initializeObjectFromSchemata(context, schemata, message, defaultCharset='utf-8'):
-                """Convenience method which calls ``initializeObject()`` with all the
-                fields in order, of all the given schemata (a sequence of schema
-                interfaces).
-                """
-        
-            def initializeObject(context, fields, message, defaultCharset='utf-8'):
-                """Initialise an object from a message.
-        
-                ``context`` is the content object to initialise.
-        
-                ``fields`` is a sequence of (name, field) pairs for the fields which make
-                up the message. This can be obtained from zope.schema.getFieldsInOrder,
-                for example.
-        
-                ``message`` is a ``Message`` object.
-        
-                ``defaultCharset`` is the default character set to use.
-        
-                If the message is a multipart message, the primary fields will be read
-                in order.
-                """
-        
-        The message format used adheres to the following rules:
-        
-        * All non-primary fields are represented as headers.
-          The header name is taken from the field name.
-          The value is an encoded string as returned by the ``marshal()`` method of the appropriate ``IFieldMarshal`` multi-adapter.
-        * If no ``IFieldMarshaler`` adapter can be found, the header is ignored.
-        * Similarly, if no fields are found for a given header when parsing a message, the header is ignored.
-        * If there is a single primary field, the message has a string payload, which is the marshalled value of the primary field.
-          In this case, the ``Content-Type`` header of the message will be obtained from the primary field's marshaler.
-        * If there are multiple primary fields, each is encoded into its own message, each with its own ``Content-Type`` header.
-          The outer message will have a content type of ``multipart/mixed`` and headers for other fields.
-        * A ``ValueError`` error is raised if a message is being parsed which has more or fewer parts than there are primary fields.
-        * Duplicate field names are allowed, and will be encoded as duplicate headers.
-          When parsing a message, there needs to be one field per header.
-          That is, if a message contains two headers with the name 'foo',
-          the list of field name/ instance pairs passed to the ``initializeObject()`` method should contain two pairs with the name 'foo'.
-          The first field will be used for the first header value, the second field will be used for the second header value.
-          If a third 'foo' header appears, it will be ignored.
-        * Since message headers are always lowercase, field names will be matched case-insensitively when parsing a message.
-        
-        Supermodel handler
-        ------------------
-        
-        If ``plone.supermodel`` is installed, this package  will register a namespace handler for the ``marshal`` namespace, with the URI ``http://namespaces.plone.org/supermodel/marshal``.
-        This can be used to mark a field as the primary field::
-        
-            <model xmlns="http://namespaces.plone.org/supermodel/schema"
-                   xmlns:marshal="http://namespaces.plone.org/supermodel/marshal">
-                <schema>
-                    <field type="zope.schema.Text" name="test" marshal:primary="true">
-                        <title>Test field</title>
-                    </field>
-                </schema>
-            </model>
-        
-        ``plone.supermodel`` may be installed as a dependency using the extra
-        ``[supermodel]``, but this is probably only useful for running the tests.
-        If the package is not installed, the handler will not be ignored.
-        
-        License note
-        ------------
-        
-        This package is released under the BSD license.
-        Contributors, please do not add dependencies on GPL code.
-        
-        Issue tracker
-        -------------
-        
-        Please report issues via the `Plone issue tracker`_.
-        
-        .. _`Plone issue tracker`: https://github.com/plone/plone.rfc822/issues
-        
-        Support
-        -------
-        
-        Dexterity use questions may be answered via `Plone's support channels`_.
-        
-        .. _`Plone's support channels`: http://plone.org/support
-        
-        Contributing
-        ------------
-        
-        Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.rfc822>`_.
-        
-        Contributors please read the document `Process for Plone core's development <https://docs.plone.org/develop/coredev/docs/index.html>`_
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
-        2.0.2 (2020-04-22)
-        ------------------
-        
-        Bug fixes:
-        
-        
-        - Minor packaging updates. (#1)
-        
-        
-        2.0.1 (2019-05-21)
-        ------------------
-        
-        Bug fixes:
-        
-        
-        - Use a better type check in the payload parser.
-          [Rotonen] (#7)
-        
-        
-        2.0.0 (2018-11-04)
-        ------------------
-        
-        Breaking changes:
-        
-        - Deprecate ``renderMessage(message)``,
-          use stdlibs ``message.as_string()`` from ``email.message.Message`` class instead.
-          [jensens]
-        
-        - Newline handling in MIME-headers: ``\n`` are now escaped explicit.
-          This follows RFC2822 section 3.2.2.
-          [jensens]
-        
-        - Drop support of Python 2.6
-          [jensens]
-        
-        New features:
-        
-        - ``constructMessage`` now handles base64 encoding automatically for all marshallers,
-          where ``marshaler.ascii`` is ``False`` and ``marshaler.getContentType`` is ``None``.
-          [jensens]
-        
-        - Support for Python 3+
-          Also big code overhaul included.
-          [jensens]
-        
-        
-        1.1.4 (2018-06-20)
-        ------------------
-        
-        New features:
-        
-        - Start basic Python 3 support.
-          [pbauer, dhavlik]
-        
-        
-        1.1.3 (2016-08-09)
-        ------------------
-        
-        Fixes:
-        
-        - code cleanup: pep8, isort, utf8 headers et al.
-          [jensens]
-        
-        - Use zope.interface decorator.
-          [gforcada]
-        
-        
-        1.1.2 (2016-02-21)
-        ------------------
-        
-        Fixes:
-        
-        - Fix test isolation problem.
-          [thet]
-        
-        - Replace deprecated ``zope.testing.doctest`` import with ``doctest`` module from stdlib.
-          [thet]
-        
-        
-        1.1.1 (2015-03-21)
-        ------------------
-        
-        - Update test to reflect the change in the representation of the model namespaces by adding the 18n xml namespace.
-          [sneridagh]
-        
-        - Make sure the tests do not fail if messages contain a trailing blank line. This fixes test failures on Ubuntu 14.04.
-          [timo]
-        
-        
-        1.1 (2013-08-14)
-        ----------------
-        
-        - Branch for Plone 4.2/4.3 compatibility changes.
-          [esteele]
-        
-        
-        1.0.2 (2013-07-28)
-        ------------------
-        
-        - Marshall collections as ASCII when possible.
-          [davisagli]
-        
-        - Add support for marshalling decimal fields.
-          [davisagli]
-        
-        1.0.1 (2013-01-01)
-        ------------------
-        
-        1.0 (2011-05-20)
-        ----------------
-        
-        * Relicensed under the BSD license.
-          See http://plone.org/foundation/materials/foundation-resolutions/plone-framework-components-relicensing-policy
-          [davisagli]
-        
-        1.0b2 (2011-02-11)
-        ------------------
-        
-        * Add IPrimaryFieldInfo to look up primary field information on a content item.
-        
-        1.0b1 (2009-10-08)
-        ------------------
-        
-        * Initial release
-        
-        Message construction and parsing
-        ================================
-        
-        This package contains helper methods to construct an RFC 2822 style message
-        from a list of schema fields, and to parse a message and initialise an object
-        based on its headers and body payload.
-        
-        Before we begin, let's load the default field marshalers and configure
-        annotations, which we will use later in this test::
-        
-            >>> configuration = u"""\
-            ... <configure
-            ...      xmlns="http://namespaces.zope.org/zope"
-            ...      i18n_domain="plone.rfc822.tests">
-            ...
-            ...     <include package="zope.component" file="meta.zcml" />
-            ...     <include package="zope.annotation" />
-            ...
-            ...     <include package="plone.rfc822" />
-            ...
-            ... </configure>
-            ... """
-        
-        ::
-        
-            >>> from six import StringIO
-            >>> from zope.configuration import xmlconfig
-            >>> xmlconfig.xmlconfig(StringIO(configuration))
-        
-        The primary field
-        -----------------
-        
-        The message body is assumed to originate from a "primary" field, which is
-        indicated via a marker interface.
-        
-        To illustrate the pattern, consider the following schema interface::
-        
-            >>> from zope.interface import Interface, alsoProvides
-            >>> from plone.rfc822.interfaces import IPrimaryField
-            >>> from zope import schema
-        
-            >>> class ITestContent(Interface):
-            ...
-            ...     title = schema.TextLine(title=u"Title")
-            ...     description = schema.Text(title=u"Description")
-            ...     body = schema.Text(title=u"Body text")
-            ...     emptyfield = schema.TextLine(title=u"Empty field", missing_value=u'missing')
-        
-        The primary field instance is marked like this::
-        
-            >>> alsoProvides(ITestContent['body'], IPrimaryField)
-        
-        Constructing a message
-        ----------------------
-        
-        Let's now say we have an instance providing this interface, which we want to
-        marshal to a message::
-        
-            >>> from zope.interface import implementer
-            >>> @implementer(ITestContent)
-            ... class TestContent(object):
-            ...     title = ""
-            ...     description = ""
-            ...     body = ""
-            ...     emptyfield = None
-        
-            >>> content = TestContent()
-            >>> content.title = "Test title"
-            >>> content.description = """Täst description
-            ... with a newline"""
-            >>> content.body = "<p>Test body</p>"
-        
-        We could create a message from this instance and schema like this::
-        
-            >>> from plone.rfc822 import constructMessageFromSchema
-            >>> msg = constructMessageFromSchema(content, ITestContent)
-        
-        The output looks like this::
-        
-            >>> print(msg.as_string())
-            title: Test title
-            description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
-            emptyfield:
-            Content-Type: text/plain; charset="utf-8"
-            <BLANKLINE>
-            <p>Test body</p>
-        
-        Notice how the non-ASCII header values are UTF-8 encoded.
-        The encoding algorithm is clever enough to only encode the value if it is necessary,
-        leaving more readable field values otherwise.
-        
-        The body here is of the default message type::
-        
-            >>> msg.get_default_type()
-            'text/plain'
-        
-        This is because none of the default field types manage a content type.
-        
-        The body is also utf-8 encoded, because the primary field specified this
-        encoding.
-        
-        If we want to use a different content type, we could set it explicitly::
-        
-            >>> msg.set_type('text/html')
-            >>> print(msg.as_string())
-            title: Test title
-            description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
-            emptyfield:
-            MIME-Version: 1.0
-            Content-Type: text/html; charset="utf-8"
-            <BLANKLINE>
-            <p>Test body</p>
-        
-        Alternatively, if we know that any ``IText`` field on an object providing
-        our ``ITestContent`` interface always stores HTML, could register a custom
-        ``IFieldMarshaler`` adapter which would indicate this to the message
-        constructor. Let's take a look at that now.
-        
-        Custom marshalers
-        -----------------
-        
-        The default marshaler can be obtained by multi-adapting the content object
-        and the field instance to ``IFieldMarshaler``:
-        
-            >>> from zope.component import getMultiAdapter
-            >>> from plone.rfc822.interfaces import IFieldMarshaler
-            >>> getMultiAdapter((content, ITestContent['body'],), IFieldMarshaler)
-            <plone.rfc822.defaultfields.UnicodeValueFieldMarshaler object at ...>
-        
-        Let's now create our own marshaler by extending this class and overriding
-        the ``getContentType()``:
-        
-            >>> from plone.rfc822.defaultfields import UnicodeValueFieldMarshaler
-            >>> from zope.schema.interfaces import IText
-            >>> from zope.component import adapter
-        
-            >>> @adapter(ITestContent, IText)
-            ... class TestBodyMarshaler(UnicodeValueFieldMarshaler):
-            ...     def getContentType(self):
-            ...         return 'text/html'
-        
-        Ordinarily, we'd register this with ZCML. For the purpose of the test, we'll
-        register it using the ``zope.component`` API.
-        
-            >>> from zope.component import provideAdapter
-            >>> provideAdapter(TestBodyMarshaler)
-        
-        Hint: If the schema contained multiple text fields, this adapter would apply
-        to all of them. To avoid that, we could either mark the field with a custom
-        marker interface (similary to the way we marked a field with ``IPrimaryField``
-        above), or have the marshaler check the field name.
-        
-        Let's now try again:
-        
-            >>> msg = constructMessageFromSchema(content, ITestContent)
-            >>> print(msg.as_string())
-            title: Test title
-            description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
-            emptyfield:
-            MIME-Version: 1.0
-            Content-Type: text/html; charset="utf-8"
-            <BLANKLINE>
-            <p>Test body</p>
-        
-        Notice how the Content-Type has changed.
-        
-        Consuming a message
-        -------------------
-        
-        A message can be used to initialise an object. The object has to be
-        constructed first:
-        
-            >>> newContent = TestContent()
-        
-        We then need to obtain a ``Message`` object. The ``email`` module contains
-        helper functions for this purpose.
-        
-            >>> messageBody = """\
-            ... title: Test title
-            ... description: =?utf-8?q?Test_description=0D=0Awith_a_newline?=
-            ... Content-Type: text/html
-            ...
-            ... <p>Test body</p>"""
-        
-            >>> from email import message_from_string
-            >>> msg = message_from_string(messageBody)
-        
-        The message can now be used to initialise the object according to the given
-        schema. This should be the same schema as the one used to construct the
-        message.
-        
-            >>> from plone.rfc822 import initializeObjectFromSchema
-            >>> initializeObjectFromSchema(newContent, ITestContent, msg)
-        
-            >>> newContent.title
-            'Test title'
-            >>> print(newContent.description)
-            Test description
-            with a newline
-        
-            >>> newContent.body
-            '<p>Test body</p>'
-        
-        We can also consume messages with a transfer encoding and a charset:
-        
-            >>> messageBody = """\
-            ... title: =?utf-8?q?Test_title?=
-            ... description: =?utf-8?q?Test_description=0D=0Awith_a_newline?=
-            ... emptyfield:
-            ... Content-Transfer-Encoding: base64
-            ... Content-Type: text/html; charset="utf-8"
-            ... <BLANKLINE>
-            ... PHA+VGVzdCBib2R5PC9wPg==
-            ... <BLANKLINE>"""
-        
-            >>> msg = message_from_string(messageBody)
-            >>> msg.get_content_type()
-            'text/html'
-            >>> msg.get_content_charset()
-            'utf-8'
-        
-            >>> initializeObjectFromSchema(newContent, ITestContent, msg)
-        
-            >>> newContent.title
-            'Test title'
-            >>> print(newContent.description)
-            Test description
-            with a newline
-            >>> newContent.body
-            '<p>Test body</p>'
-        
-        Note: Empty fields will result in the field's ``missing_value`` being used:
-        
-            >>> newContent.emptyfield
-            'missing'
-        
-        Handling multiple primary fields and duplicate field names
-        ----------------------------------------------------------
-        
-        It is possible that our type could have multiple primary fields or even
-        duplicate field names.
-        
-        For example, consider the following schema interface, intended to be used
-        in an annotation adapter:
-        
-            >>> class IPersonalDetails(Interface):
-            ...     description = schema.Text(title=u"Personal description")
-            ...     currentAge = schema.Int(title=u"Age", min=0)
-            ...     personalProfile = schema.Text(title=u"Profile")
-        
-            >>> alsoProvides(IPersonalDetails['personalProfile'], IPrimaryField)
-        
-        The annotation storage would look like this:
-        
-            >>> from persistent import Persistent
-            >>> @implementer(IPersonalDetails)
-            ... @adapter(ITestContent)
-            ... class PersonalDetailsAnnotation(Persistent):
-            ...
-            ...     def __init__(self):
-            ...         self.description = None
-            ...         self.currentAge = None
-            ...         self.personalProfile = None
-        
-            >>> from zope.annotation.factory import factory
-            >>> provideAdapter(factory(PersonalDetailsAnnotation))
-        
-        We should now be able to adapt a content instance to IPersonalDetails,
-        provided it is annotatable.
-        
-            >>> from zope.annotation.interfaces import IAttributeAnnotatable
-            >>> alsoProvides(content, IAttributeAnnotatable)
-        
-            >>> personalDetails = IPersonalDetails(content)
-            >>> personalDetails.description = u"<p>My description</p>"
-            >>> personalDetails.currentAge = 21
-            >>> personalDetails.personalProfile = u"<p>My profile</p>"
-        
-        The default marshalers will attempt to adapt the context to the schema of
-        a given field before getting or setting a value. If we pass multiple schemata
-        (or a combined sequence of fields) to the message constructor, it will
-        handle both duplicate field names (as duplicate headers) and multiple primary
-        fields (as multipart message attachments).
-        
-        Here are the fields it will see:
-        
-            >>> from zope.schema import getFieldsInOrder
-            >>> allFields = getFieldsInOrder(ITestContent) + \
-            ...             getFieldsInOrder(IPersonalDetails)
-        
-            >>> [f[0] for f in allFields]
-            ['title', 'description', 'body', 'emptyfield', 'description', 'currentAge', 'personalProfile']
-        
-            >>> [f[0] for f in allFields if IPrimaryField.providedBy(f[1])]
-            ['body', 'personalProfile']
-        
-        Let's now construct a message. Since we now have two fields called
-        ``description``, we will get two headers by that name. Since we have two
-        primary fields, we will get a multipart message with two attachments::
-        
-            >>> from plone.rfc822 import constructMessageFromSchemata
-            >>> msg = constructMessageFromSchemata(content, (ITestContent, IPersonalDetails,))
-            >>> msgString = msg.as_string()
-            >>> print(msgString)
-            title: Test title
-            description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
-            emptyfield:
-            description: <p>My description</p>
-            currentAge: 21
-            MIME-Version: 1.0
-            Content-Type: multipart/mixed; boundary="===============...=="
-            <BLANKLINE>
-            --===============...==
-            MIME-Version: 1.0
-            Content-Type: text/html; charset="utf-8"
-            <BLANKLINE>
-            <p>Test body</p>
-            --===============...==
-            MIME-Version: 1.0
-            Content-Type: text/html; charset="utf-8"
-            <BLANKLINE>
-            <p>My profile</p>
-            --===============...==--
-            <BLANKLINE>
-        
-        
-        (Note that we've used ellipses here for the doctest to work with the generated
-        boundary string).
-        
-        Notice how both messages have a MIME type of 'text/html' and no charset.
-        That is because of the custom adapter for ``(ITestContent, IText)`` which we
-        registered earlier.
-        
-        We can obviously read this message as well. Note that in this case, the order
-        of fields passed to ``initializeObject()`` is important, both to determine
-        which field gets which ``description`` header, and to match the two
-        attachments to the two primary fields:
-        
-            >>> newContent = TestContent()
-            >>> alsoProvides(newContent, IAttributeAnnotatable)
-        
-            >>> from plone.rfc822 import initializeObjectFromSchemata
-            >>> msg = message_from_string(msgString)
-            >>> initializeObjectFromSchemata(newContent, [ITestContent, IPersonalDetails], msg)
-        
-            >>> newContent.title
-            'Test title'
-        
-            >>> newContent.marker = True
-            >>> newContent.description
-            'T\xe4st description\nwith a newline'
-        
-            >>> newContent.body
-            '<p>Test body</p>'
-        
-            >>> newPersonalDetails = IPersonalDetails(newContent)
-            >>> newPersonalDetails.description
-            '<p>My description</p>'
-        
-            >>> newPersonalDetails.currentAge
-            21
-        
-            >>> newPersonalDetails.personalProfile
-            '<p>My profile</p>'
-        
-        Alternative ways to deal with multiple schemata
-        -----------------------------------------------
-        
-        In the example above, we created a single enveloping message with headers
-        corresponding to the fields in both our schemata, and only the primary fields
-        separated out into different attached payloads.
-        
-        An alternative approach would be to separate each schema out into its
-        own multipart message. To do that, we would simply use the
-        ``constructMessage()`` function multiple times.
-        
-            >>> mainMessage = constructMessageFromSchema(content, ITestContent)
-            >>> personalDetailsMessage = constructMessageFromSchema(content, IPersonalDetails)
-        
-            >>> from email.mime.multipart import MIMEMultipart
-            >>> envelope = MIMEMultipart()
-            >>> envelope.attach(mainMessage)
-            >>> envelope.attach(personalDetailsMessage)
-        
-            >>> envelopeString = envelope.as_string()
-            >>> print(envelopeString)
-            Content-Type: multipart/mixed; boundary="===============...=="
-            MIME-Version: 1.0
-            <BLANKLINE>
-            --===============...==
-            title: Test title
-            description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
-            emptyfield:
-            MIME-Version: 1.0
-            Content-Type: text/html; charset="utf-8"
-            <BLANKLINE>
-            <p>Test body</p>
-            --===============...==
-            description: <p>My description</p>
-            currentAge: 21
-            MIME-Version: 1.0
-            Content-Type: text/html; charset="utf-8"
-            <BLANKLINE>
-            <p>My profile</p>
-            --===============...==--...
-        
-        Which approach works best will depend largely on the intended recipient of
-        the message.
-        
-        Encoding the payload and handling filenames
-        -------------------------------------------
-        
-        Finally, let's consider a more complex example, inspired by the field
-        marshaler in ``plone.namedfile``.
-        
-        Let's say we have a value type intended to represent a binary file with a
-        filename and content type:
-        
-            >>> from zope.interface import Interface, implementer
-            >>> from zope import schema
-        
-            >>> class IFileValue(Interface):
-            ...     data = schema.Bytes(title=u"Raw data")
-            ...     contentType = schema.ASCIILine(title=u"MIME type")
-            ...     filename = schema.ASCIILine(title=u"Filename")
-        
-            >>> @implementer(IFileValue)
-            ... class FileValue(object):
-            ...
-            ...     def __init__(self, data, contentType, filename):
-            ...         self.data = data
-            ...         self.contentType = contentType
-            ...         self.filename = filename
-        
-        Suppose we had a custom field type to represent this:
-        
-            >>> from zope.schema.interfaces import IObject
-            >>> class IFileField(IObject):
-            ...     pass
-        
-            >>> @implementer(IFileField)
-            ... class FileField(schema.Object):
-            ...     schema = IFileValue
-            ...     def __init__(self, **kw):
-            ...         if 'schema' in kw:
-            ...             self.schema = kw.pop('schema')
-            ...         super(FileField, self).__init__(schema=self.schema, **kw)
-        
-        We can register a field marshaler for this field which will do the following:
-        
-        * Insist that the field is only used as a primary field, since it makes
-          little sense to encode a binary file in a header.
-        * Save the filename in a Content-Disposition header.
-        * Be capable of reading the filename again from this header.
-        * Encode the payload using base64
-        
-            >>> from plone.rfc822.interfaces import IFieldMarshaler
-            >>> from email.encoders import encode_base64
-        
-            >>> from zope.component import adapter
-            >>> from plone.rfc822.defaultfields import BaseFieldMarshaler
-        
-            >>> @adapter(Interface, IFileField)
-            ... class FileFieldMarshaler(BaseFieldMarshaler):
-            ...
-            ...     ascii = False
-            ...
-            ...     def encode(self, value, charset='utf-8', primary=False):
-            ...         if not primary:
-            ...             raise ValueError("File field cannot be marshaled as a non-primary field")
-            ...         if value is None:
-            ...             return None
-            ...         return value.data
-            ...
-            ...     def decode(self, value, message=None, charset='utf-8', contentType=None, primary=False):
-            ...         filename = None
-            ...         # get the filename from the Content-Disposition header if possible
-            ...         if primary and message is not None:
-            ...             filename = message.get_filename(None)
-            ...         return FileValue(value, contentType, filename)
-            ...
-            ...     def getContentType(self):
-            ...         value = self._query()
-            ...         if value is None:
-            ...             return None
-            ...         return value.contentType
-            ...
-            ...     def getCharset(self, default='utf-8'):
-            ...         return None # this is not text data!
-            ...
-            ...     def postProcessMessage(self, message):
-            ...         value = self._query()
-            ...         if value is not None:
-            ...             filename = value.filename
-            ...             if filename:
-            ...                 # Add a new header storing the filename if we have one
-            ...                 message.add_header('Content-Disposition', 'attachment', filename=filename)
-        
-            >>> from zope.component import provideAdapter
-            >>> provideAdapter(FileFieldMarshaler)
-        
-        To illustrate marshaling, let's create a content object that contains two file
-        fields.
-        
-            >>> class IFileContent(Interface):
-            ...     file1 = FileField()
-            ...     file2 = FileField()
-        
-            >>> @implementer(IFileContent)
-            ... class FileContent(object):
-            ...     file1 = None
-            ...     file2 = None
-        
-            >>> fileContent = FileContent()
-            >>> fileContent.file1 = FileValue('dummy file', 'text/plain', 'dummy1.txt')
-            >>> fileContent.file2 = FileValue('<html><body>test</body></html>', 'text/html', 'dummy2.html')
-        
-        At this point, neither of these fields is marked as a primary field. Let's see
-        what happens when we attempt to construct a message from this schema.
-        
-            >>> from plone.rfc822 import constructMessageFromSchema
-            >>> message = constructMessageFromSchema(fileContent, IFileContent)
-            >>> print(message.as_string())
-            <BLANKLINE>
-            <BLANKLINE>
-        
-        As expected, we got no message headers and no message body. Let's now mark one
-        field as primary:
-        
-            >>> from plone.rfc822.interfaces import IPrimaryField
-            >>> from zope.interface import alsoProvides
-            >>> alsoProvides(IFileContent['file1'], IPrimaryField)
-        
-            >>> message = constructMessageFromSchema(fileContent, IFileContent)
-            >>> messageBody = message.as_string()
-            >>> print(messageBody)
-            MIME-Version: 1.0
-            Content-Type: text/plain
-            Content-Transfer-Encoding: base64
-            Content-Disposition: attachment; filename="dummy1.txt"
-            <BLANKLINE>
-            ZHVtbXkgZmlsZQ==
-        
-        Here, we have a base64 encoded payload, a Content-Disposition header, and a
-        Content-Type header according to the primary field.
-        
-        We can also reconstruct the object from this message.
-        
-            >>> from plone.rfc822 import initializeObjectFromSchema
-            >>> from email import message_from_string
-        
-            >>> inputMessage = message_from_string(messageBody)
-            >>> newFileContent = FileContent()
-            >>> initializeObjectFromSchema(newFileContent, IFileContent, inputMessage)
-        
-            >>> newFileContent.file1.data
-            'dummy file'
-            >>> newFileContent.file1.contentType
-            'text/plain'
-            >>> newFileContent.file1.filename
-            'dummy1.txt'
-        
-            >>> newFileContent.file2 is None
-            True
-        
-        Let's now show what would happen if we encoded both files in the message.
-        In this case, we should get a multipart document with two payloads.
-        
-            >>> alsoProvides(IFileContent['file2'], IPrimaryField)
-            >>> message = constructMessageFromSchema(fileContent, IFileContent)
-            >>> messageBody = message.as_string()
-            >>> print(messageBody) # doctest: +ELLIPSIS
-            MIME-Version: 1.0
-            Content-Type: multipart/mixed; boundary="===============...=="
-            <BLANKLINE>
-            --===============...==
-            MIME-Version: 1.0
-            Content-Type: text/plain
-            Content-Transfer-Encoding: base64
-            Content-Disposition: attachment; filename="dummy1.txt"
-            <BLANKLINE>
-            ZHVtbXkgZmlsZQ==
-            --===============...==
-            MIME-Version: 1.0
-            Content-Type: text/html
-            Content-Transfer-Encoding: base64
-            Content-Disposition: attachment; filename="dummy2.html"
-            <BLANKLINE>
-            PGh0bWw+PGJvZHk+dGVzdDwvYm9keT48L2h0bWw+
-            --===============...==--...
-        
-        And again, we can reconstruct the object, this time with both fields:
-        
-            >>> inputMessage = message_from_string(messageBody)
-            >>> newFileContent = FileContent()
-            >>> initializeObjectFromSchema(newFileContent, IFileContent, inputMessage)
-        
-            >>> newFileContent.file1.data
-            'dummy file'
-            >>> newFileContent.file1.contentType
-            'text/plain'
-            >>> newFileContent.file1.filename
-            'dummy1.txt'
-        
-            >>> newFileContent.file2.data
-            '<html><body>test</body></html>'
-            >>> newFileContent.file2.contentType
-            'text/html'
-            >>> newFileContent.file2.filename
-            'dummy2.html'
-        
-        Specialities between Py2 and Py3
-        --------------------------------
-        
-        Test a special behavior which is different between Python 2 and 3 stdlib:
-        Newline handling in non-utf8 strings.
-        
-        Python 2.7 ``email.header`` keeps a line with an escaped value,
-        while Python 3.6 turns it into RFC2047 encoded headers, see https://tools.ietf.org/html/rfc2047.html
-        Technical both is fine.
-        
-        ::
-        
-            >>> import six
-            >>> content.description = "Test content\nwith newline difference"
-            >>> msg = constructMessageFromSchema(content, ITestContent)
-            >>> effective_output = msg.as_string()
-            >>> effective_output.split('\n')[1]
-            'description: =?utf-8?q?Test_content=5Cnwith_newline_difference?='
-        
 Keywords: zope schema rfc822
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
-Provides-Extra: test
+Requires-Python: >=3.8
 Provides-Extra: supermodel
+Provides-Extra: test
+
+Introduction
+============
+
+This package provides primitives for turning content objects described by ``zope.schema`` fields into RFC (2)822 style messages.
+It utilizes the Python standard library's ``email`` module.
+
+It consists of:
+
+* A marker interface ``IPrimaryField`` which can be used to indicate the primary field of a schema.
+  The primary field will be used as the message body.
+  If there are more than one field marked as primary, the body is turned in a MIME multipart message.
+* An interface ``IFieldMarshaler`` which describes marshalers that convert to and from strings suitable for encoding into an RFC 2822 style message.
+  These are multi-adapters on ``(context, field)``.
+  ``context`` is the content object and ``field`` is the schema field instance.
+* Default implementations of ``IFieldMarshaler`` for the standard fields in the ``zope.schema`` package.
+* Helper methods to construct messages from one or more schemata or a list of fields, and to parse a message and update a context object accordingly.
+
+The helper methods are described by ``plone.rfc822.interfaces.IMessageAPI``.
+They are importable directly from the ``plone.rfc822`` package::
+
+    def constructMessageFromSchema(context, schema, charset='utf-8'):
+        """Convenience method which calls ``constructMessage()`` with all the
+        fields, in order, of the given schema interface
+        """
+
+    def constructMessageFromSchemata(context, schemata, charset='utf-8'):
+        """Convenience method which calls ``constructMessage()`` with all the
+        fields, in order, of all the given schemata (a sequence of schema
+        interfaces).
+        """
+
+    def constructMessage(context, fields, charset='utf-8'):
+        """Helper method to construct a message.
+
+        ``context`` is a content object.
+
+        ``fields`` is a sequence of (name, field) pairs for the fields which make
+        up the message. This can be obtained from zope.schema.getFieldsInOrder,
+        for example.
+
+        ``charset`` is the message charset.
+
+        The message body will be constructed from the primary field, i.e. the
+        field which is marked with ``IPrimaryField``. If no such field exists,
+        the message will have no body. If multiple fields exist, the message will
+        be a multipart message. Otherwise, it will contain a scalar string
+        payload.
+
+        A field will be ignored if ``(context, field)`` cannot be multi-adapted
+        to ``IFieldMarshaler``, or if the ``marshal()`` method returns None.
+        """
+
+    def renderMessage(message, mangleFromHeader=False):
+        """Render a message to a string
+        """
+
+    def initializeObjectFromSchema(context, schema, message, defaultCharset='utf-8'):
+        """Convenience method which calls ``initializeObject()`` with all the
+        fields, in order, of the given schema interface
+        """
+
+    def initializeObjectFromSchemata(context, schemata, message, defaultCharset='utf-8'):
+        """Convenience method which calls ``initializeObject()`` with all the
+        fields in order, of all the given schemata (a sequence of schema
+        interfaces).
+        """
+
+    def initializeObject(context, fields, message, defaultCharset='utf-8'):
+        """Initialise an object from a message.
+
+        ``context`` is the content object to initialise.
+
+        ``fields`` is a sequence of (name, field) pairs for the fields which make
+        up the message. This can be obtained from zope.schema.getFieldsInOrder,
+        for example.
+
+        ``message`` is a ``Message`` object.
+
+        ``defaultCharset`` is the default character set to use.
+
+        If the message is a multipart message, the primary fields will be read
+        in order.
+        """
+
+The message format used adheres to the following rules:
+
+* All non-primary fields are represented as headers.
+  The header name is taken from the field name.
+  The value is an encoded string as returned by the ``marshal()`` method of the appropriate ``IFieldMarshal`` multi-adapter.
+* If no ``IFieldMarshaler`` adapter can be found, the header is ignored.
+* Similarly, if no fields are found for a given header when parsing a message, the header is ignored.
+* If there is a single primary field, the message has a string payload, which is the marshalled value of the primary field.
+  In this case, the ``Content-Type`` header of the message will be obtained from the primary field's marshaler.
+* If there are multiple primary fields, each is encoded into its own message, each with its own ``Content-Type`` header.
+  The outer message will have a content type of ``multipart/mixed`` and headers for other fields.
+* A ``ValueError`` error is raised if a message is being parsed which has more or fewer parts than there are primary fields.
+* Duplicate field names are allowed, and will be encoded as duplicate headers.
+  When parsing a message, there needs to be one field per header.
+  That is, if a message contains two headers with the name 'foo',
+  the list of field name/ instance pairs passed to the ``initializeObject()`` method should contain two pairs with the name 'foo'.
+  The first field will be used for the first header value, the second field will be used for the second header value.
+  If a third 'foo' header appears, it will be ignored.
+* Since message headers are always lowercase, field names will be matched case-insensitively when parsing a message.
+
+Supermodel handler
+------------------
+
+If ``plone.supermodel`` is installed, this package  will register a namespace handler for the ``marshal`` namespace, with the URI ``http://namespaces.plone.org/supermodel/marshal``.
+This can be used to mark a field as the primary field::
+
+    <model xmlns="http://namespaces.plone.org/supermodel/schema"
+           xmlns:marshal="http://namespaces.plone.org/supermodel/marshal">
+        <schema>
+            <field type="zope.schema.Text" name="test" marshal:primary="true">
+                <title>Test field</title>
+            </field>
+        </schema>
+    </model>
+
+``plone.supermodel`` may be installed as a dependency using the extra
+``[supermodel]``, but this is probably only useful for running the tests.
+If the package is not installed, the handler will not be ignored.
+
+License note
+------------
+
+This package is released under the BSD license.
+Contributors, please do not add dependencies on GPL code.
+
+Issue tracker
+-------------
+
+Please report issues via the `Plone issue tracker`_.
+
+.. _`Plone issue tracker`: https://github.com/plone/plone.rfc822/issues
+
+Support
+-------
+
+Dexterity use questions may be answered via `Plone's support channels`_.
+
+.. _`Plone's support channels`: http://plone.org/support
+
+Contributing
+------------
+
+Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.rfc822>`_.
+
+Contributors please read the document `Process for Plone core's development <https://docs.plone.org/develop/coredev/docs/index.html>`_
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
+3.0.0 (2023-04-26)
+------------------
+
+Breaking changes:
+
+
+- Remove long deprecated `renderMessage` function.
+  [@jensens] (1-1)
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
+2.0.2 (2020-04-22)
+------------------
+
+Bug fixes:
+
+
+- Minor packaging updates. (#1)
+
+
+2.0.1 (2019-05-21)
+------------------
+
+Bug fixes:
+
+
+- Use a better type check in the payload parser.
+  [Rotonen] (#7)
+
+
+2.0.0 (2018-11-04)
+------------------
+
+Breaking changes:
+
+- Deprecate ``renderMessage(message)``,
+  use stdlibs ``message.as_string()`` from ``email.message.Message`` class instead.
+  [jensens]
+
+- Newline handling in MIME-headers: ``\n`` are now escaped explicit.
+  This follows RFC2822 section 3.2.2.
+  [jensens]
+
+- Drop support of Python 2.6
+  [jensens]
+
+New features:
+
+- ``constructMessage`` now handles base64 encoding automatically for all marshallers,
+  where ``marshaler.ascii`` is ``False`` and ``marshaler.getContentType`` is ``None``.
+  [jensens]
+
+- Support for Python 3+
+  Also big code overhaul included.
+  [jensens]
+
+
+1.1.4 (2018-06-20)
+------------------
+
+New features:
+
+- Start basic Python 3 support.
+  [pbauer, dhavlik]
+
+
+1.1.3 (2016-08-09)
+------------------
+
+Fixes:
+
+- code cleanup: pep8, isort, utf8 headers et al.
+  [jensens]
+
+- Use zope.interface decorator.
+  [gforcada]
+
+
+1.1.2 (2016-02-21)
+------------------
+
+Fixes:
+
+- Fix test isolation problem.
+  [thet]
+
+- Replace deprecated ``zope.testing.doctest`` import with ``doctest`` module from stdlib.
+  [thet]
+
+
+1.1.1 (2015-03-21)
+------------------
+
+- Update test to reflect the change in the representation of the model namespaces by adding the 18n xml namespace.
+  [sneridagh]
+
+- Make sure the tests do not fail if messages contain a trailing blank line. This fixes test failures on Ubuntu 14.04.
+  [timo]
+
+
+1.1 (2013-08-14)
+----------------
+
+- Branch for Plone 4.2/4.3 compatibility changes.
+  [esteele]
+
+
+1.0.2 (2013-07-28)
+------------------
+
+- Marshall collections as ASCII when possible.
+  [davisagli]
+
+- Add support for marshalling decimal fields.
+  [davisagli]
+
+1.0.1 (2013-01-01)
+------------------
+
+1.0 (2011-05-20)
+----------------
+
+* Relicensed under the BSD license.
+  See http://plone.org/foundation/materials/foundation-resolutions/plone-framework-components-relicensing-policy
+  [davisagli]
+
+1.0b2 (2011-02-11)
+------------------
+
+* Add IPrimaryFieldInfo to look up primary field information on a content item.
+
+1.0b1 (2009-10-08)
+------------------
+
+* Initial release
+
+Message construction and parsing
+================================
+
+This package contains helper methods to construct an RFC 2822 style message
+from a list of schema fields, and to parse a message and initialise an object
+based on its headers and body payload.
+
+Before we begin, let's load the default field marshalers and configure
+annotations, which we will use later in this test::
+
+    >>> configuration = u"""\
+    ... <configure
+    ...      xmlns="http://namespaces.zope.org/zope"
+    ...      i18n_domain="plone.rfc822.tests">
+    ...
+    ...     <include package="zope.component" file="meta.zcml" />
+    ...     <include package="zope.annotation" />
+    ...
+    ...     <include package="plone.rfc822" />
+    ...
+    ... </configure>
+    ... """
+
+::
+
+    >>> from io import StringIO
+    >>> from zope.configuration import xmlconfig
+    >>> xmlconfig.xmlconfig(StringIO(configuration))
+
+The primary field
+-----------------
+
+The message body is assumed to originate from a "primary" field, which is
+indicated via a marker interface.
+
+To illustrate the pattern, consider the following schema interface::
+
+    >>> from zope.interface import Interface, alsoProvides
+    >>> from plone.rfc822.interfaces import IPrimaryField
+    >>> from zope import schema
+
+    >>> class ITestContent(Interface):
+    ...
+    ...     title = schema.TextLine(title=u"Title")
+    ...     description = schema.Text(title=u"Description")
+    ...     body = schema.Text(title=u"Body text")
+    ...     emptyfield = schema.TextLine(title=u"Empty field", missing_value=u'missing')
+
+The primary field instance is marked like this::
+
+    >>> alsoProvides(ITestContent['body'], IPrimaryField)
+
+Constructing a message
+----------------------
+
+Let's now say we have an instance providing this interface, which we want to
+marshal to a message::
+
+    >>> from zope.interface import implementer
+    >>> @implementer(ITestContent)
+    ... class TestContent(object):
+    ...     title = ""
+    ...     description = ""
+    ...     body = ""
+    ...     emptyfield = None
+
+    >>> content = TestContent()
+    >>> content.title = "Test title"
+    >>> content.description = """Täst description
+    ... with a newline"""
+    >>> content.body = "<p>Test body</p>"
+
+We could create a message from this instance and schema like this::
+
+    >>> from plone.rfc822 import constructMessageFromSchema
+    >>> msg = constructMessageFromSchema(content, ITestContent)
+
+The output looks like this::
+
+    >>> print(msg.as_string())
+    title: Test title
+    description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
+    emptyfield:
+    Content-Type: text/plain; charset="utf-8"
+    <BLANKLINE>
+    <p>Test body</p>
+
+Notice how the non-ASCII header values are UTF-8 encoded.
+The encoding algorithm is clever enough to only encode the value if it is necessary,
+leaving more readable field values otherwise.
+
+The body here is of the default message type::
+
+    >>> msg.get_default_type()
+    'text/plain'
+
+This is because none of the default field types manage a content type.
+
+The body is also utf-8 encoded, because the primary field specified this
+encoding.
+
+If we want to use a different content type, we could set it explicitly::
+
+    >>> msg.set_type('text/html')
+    >>> print(msg.as_string())
+    title: Test title
+    description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
+    emptyfield:
+    MIME-Version: 1.0
+    Content-Type: text/html; charset="utf-8"
+    <BLANKLINE>
+    <p>Test body</p>
+
+Alternatively, if we know that any ``IText`` field on an object providing
+our ``ITestContent`` interface always stores HTML, could register a custom
+``IFieldMarshaler`` adapter which would indicate this to the message
+constructor. Let's take a look at that now.
+
+Custom marshalers
+-----------------
+
+The default marshaler can be obtained by multi-adapting the content object
+and the field instance to ``IFieldMarshaler``:
+
+    >>> from zope.component import getMultiAdapter
+    >>> from plone.rfc822.interfaces import IFieldMarshaler
+    >>> getMultiAdapter((content, ITestContent['body'],), IFieldMarshaler)
+    <plone.rfc822.defaultfields.UnicodeValueFieldMarshaler object at ...>
+
+Let's now create our own marshaler by extending this class and overriding
+the ``getContentType()``:
+
+    >>> from plone.rfc822.defaultfields import UnicodeValueFieldMarshaler
+    >>> from zope.schema.interfaces import IText
+    >>> from zope.component import adapter
+
+    >>> @adapter(ITestContent, IText)
+    ... class TestBodyMarshaler(UnicodeValueFieldMarshaler):
+    ...     def getContentType(self):
+    ...         return 'text/html'
+
+Ordinarily, we'd register this with ZCML. For the purpose of the test, we'll
+register it using the ``zope.component`` API.
+
+    >>> from zope.component import provideAdapter
+    >>> provideAdapter(TestBodyMarshaler)
+
+Hint: If the schema contained multiple text fields, this adapter would apply
+to all of them. To avoid that, we could either mark the field with a custom
+marker interface (similarly to the way we marked a field with ``IPrimaryField``
+above), or have the marshaler check the field name.
+
+Let's now try again:
+
+    >>> msg = constructMessageFromSchema(content, ITestContent)
+    >>> print(msg.as_string())
+    title: Test title
+    description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
+    emptyfield:
+    MIME-Version: 1.0
+    Content-Type: text/html; charset="utf-8"
+    <BLANKLINE>
+    <p>Test body</p>
+
+Notice how the Content-Type has changed.
+
+Consuming a message
+-------------------
+
+A message can be used to initialise an object. The object has to be
+constructed first:
+
+    >>> newContent = TestContent()
+
+We then need to obtain a ``Message`` object. The ``email`` module contains
+helper functions for this purpose.
+
+    >>> messageBody = """\
+    ... title: Test title
+    ... description: =?utf-8?q?Test_description=0D=0Awith_a_newline?=
+    ... Content-Type: text/html
+    ...
+    ... <p>Test body</p>"""
+
+    >>> from email import message_from_string
+    >>> msg = message_from_string(messageBody)
+
+The message can now be used to initialise the object according to the given
+schema. This should be the same schema as the one used to construct the
+message.
+
+    >>> from plone.rfc822 import initializeObjectFromSchema
+    >>> initializeObjectFromSchema(newContent, ITestContent, msg)
+
+    >>> newContent.title
+    'Test title'
+    >>> print(newContent.description)
+    Test description
+    with a newline
+
+    >>> newContent.body
+    '<p>Test body</p>'
+
+We can also consume messages with a transfer encoding and a charset:
+
+    >>> messageBody = """\
+    ... title: =?utf-8?q?Test_title?=
+    ... description: =?utf-8?q?Test_description=0D=0Awith_a_newline?=
+    ... emptyfield:
+    ... Content-Transfer-Encoding: base64
+    ... Content-Type: text/html; charset="utf-8"
+    ... <BLANKLINE>
+    ... PHA+VGVzdCBib2R5PC9wPg==
+    ... <BLANKLINE>"""
+
+    >>> msg = message_from_string(messageBody)
+    >>> msg.get_content_type()
+    'text/html'
+    >>> msg.get_content_charset()
+    'utf-8'
+
+    >>> initializeObjectFromSchema(newContent, ITestContent, msg)
+
+    >>> newContent.title
+    'Test title'
+    >>> print(newContent.description)
+    Test description
+    with a newline
+    >>> newContent.body
+    '<p>Test body</p>'
+
+Note: Empty fields will result in the field's ``missing_value`` being used:
+
+    >>> newContent.emptyfield
+    'missing'
+
+Handling multiple primary fields and duplicate field names
+----------------------------------------------------------
+
+It is possible that our type could have multiple primary fields or even
+duplicate field names.
+
+For example, consider the following schema interface, intended to be used
+in an annotation adapter:
+
+    >>> class IPersonalDetails(Interface):
+    ...     description = schema.Text(title=u"Personal description")
+    ...     currentAge = schema.Int(title=u"Age", min=0)
+    ...     personalProfile = schema.Text(title=u"Profile")
+
+    >>> alsoProvides(IPersonalDetails['personalProfile'], IPrimaryField)
+
+The annotation storage would look like this:
+
+    >>> from persistent import Persistent
+    >>> @implementer(IPersonalDetails)
+    ... @adapter(ITestContent)
+    ... class PersonalDetailsAnnotation(Persistent):
+    ...
+    ...     def __init__(self):
+    ...         self.description = None
+    ...         self.currentAge = None
+    ...         self.personalProfile = None
+
+    >>> from zope.annotation.factory import factory
+    >>> provideAdapter(factory(PersonalDetailsAnnotation))
+
+We should now be able to adapt a content instance to IPersonalDetails,
+provided it is annotatable.
+
+    >>> from zope.annotation.interfaces import IAttributeAnnotatable
+    >>> alsoProvides(content, IAttributeAnnotatable)
+
+    >>> personalDetails = IPersonalDetails(content)
+    >>> personalDetails.description = u"<p>My description</p>"
+    >>> personalDetails.currentAge = 21
+    >>> personalDetails.personalProfile = u"<p>My profile</p>"
+
+The default marshalers will attempt to adapt the context to the schema of
+a given field before getting or setting a value. If we pass multiple schemata
+(or a combined sequence of fields) to the message constructor, it will
+handle both duplicate field names (as duplicate headers) and multiple primary
+fields (as multipart message attachments).
+
+Here are the fields it will see:
+
+    >>> from zope.schema import getFieldsInOrder
+    >>> allFields = getFieldsInOrder(ITestContent) + \
+    ...             getFieldsInOrder(IPersonalDetails)
+
+    >>> [f[0] for f in allFields]
+    ['title', 'description', 'body', 'emptyfield', 'description', 'currentAge', 'personalProfile']
+
+    >>> [f[0] for f in allFields if IPrimaryField.providedBy(f[1])]
+    ['body', 'personalProfile']
+
+Let's now construct a message. Since we now have two fields called
+``description``, we will get two headers by that name. Since we have two
+primary fields, we will get a multipart message with two attachments::
+
+    >>> from plone.rfc822 import constructMessageFromSchemata
+    >>> msg = constructMessageFromSchemata(content, (ITestContent, IPersonalDetails,))
+    >>> msgString = msg.as_string()
+    >>> print(msgString)
+    title: Test title
+    description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
+    emptyfield:
+    description: <p>My description</p>
+    currentAge: 21
+    MIME-Version: 1.0
+    Content-Type: multipart/mixed; boundary="===============...=="
+    <BLANKLINE>
+    --===============...==
+    MIME-Version: 1.0
+    Content-Type: text/html; charset="utf-8"
+    <BLANKLINE>
+    <p>Test body</p>
+    --===============...==
+    MIME-Version: 1.0
+    Content-Type: text/html; charset="utf-8"
+    <BLANKLINE>
+    <p>My profile</p>
+    --===============...==--
+    <BLANKLINE>
+
+
+(Note that we've used ellipses here for the doctest to work with the generated
+boundary string).
+
+Notice how both messages have a MIME type of 'text/html' and no charset.
+That is because of the custom adapter for ``(ITestContent, IText)`` which we
+registered earlier.
+
+We can obviously read this message as well. Note that in this case, the order
+of fields passed to ``initializeObject()`` is important, both to determine
+which field gets which ``description`` header, and to match the two
+attachments to the two primary fields:
+
+    >>> newContent = TestContent()
+    >>> alsoProvides(newContent, IAttributeAnnotatable)
+
+    >>> from plone.rfc822 import initializeObjectFromSchemata
+    >>> msg = message_from_string(msgString)
+    >>> initializeObjectFromSchemata(newContent, [ITestContent, IPersonalDetails], msg)
+
+    >>> newContent.title
+    'Test title'
+
+    >>> newContent.marker = True
+    >>> newContent.description
+    'T\xe4st description\nwith a newline'
+
+    >>> newContent.body
+    '<p>Test body</p>'
+
+    >>> newPersonalDetails = IPersonalDetails(newContent)
+    >>> newPersonalDetails.description
+    '<p>My description</p>'
+
+    >>> newPersonalDetails.currentAge
+    21
+
+    >>> newPersonalDetails.personalProfile
+    '<p>My profile</p>'
+
+Alternative ways to deal with multiple schemata
+-----------------------------------------------
+
+In the example above, we created a single enveloping message with headers
+corresponding to the fields in both our schemata, and only the primary fields
+separated out into different attached payloads.
+
+An alternative approach would be to separate each schema out into its
+own multipart message. To do that, we would simply use the
+``constructMessage()`` function multiple times.
+
+    >>> mainMessage = constructMessageFromSchema(content, ITestContent)
+    >>> personalDetailsMessage = constructMessageFromSchema(content, IPersonalDetails)
+
+    >>> from email.mime.multipart import MIMEMultipart
+    >>> envelope = MIMEMultipart()
+    >>> envelope.attach(mainMessage)
+    >>> envelope.attach(personalDetailsMessage)
+
+    >>> envelopeString = envelope.as_string()
+    >>> print(envelopeString)
+    Content-Type: multipart/mixed; boundary="===============...=="
+    MIME-Version: 1.0
+    <BLANKLINE>
+    --===============...==
+    title: Test title
+    description: =?utf-8?q?T=C3=A4st_description=5Cnwith_a_newline?=
+    emptyfield:
+    MIME-Version: 1.0
+    Content-Type: text/html; charset="utf-8"
+    <BLANKLINE>
+    <p>Test body</p>
+    --===============...==
+    description: <p>My description</p>
+    currentAge: 21
+    MIME-Version: 1.0
+    Content-Type: text/html; charset="utf-8"
+    <BLANKLINE>
+    <p>My profile</p>
+    --===============...==--...
+
+Which approach works best will depend largely on the intended recipient of
+the message.
+
+Encoding the payload and handling filenames
+-------------------------------------------
+
+Finally, let's consider a more complex example, inspired by the field
+marshaler in ``plone.namedfile``.
+
+Let's say we have a value type intended to represent a binary file with a
+filename and content type:
+
+    >>> from zope.interface import Interface, implementer
+    >>> from zope import schema
+
+    >>> class IFileValue(Interface):
+    ...     data = schema.Bytes(title=u"Raw data")
+    ...     contentType = schema.ASCIILine(title=u"MIME type")
+    ...     filename = schema.ASCIILine(title=u"Filename")
+
+    >>> @implementer(IFileValue)
+    ... class FileValue(object):
+    ...
+    ...     def __init__(self, data, contentType, filename):
+    ...         self.data = data
+    ...         self.contentType = contentType
+    ...         self.filename = filename
+
+Suppose we had a custom field type to represent this:
+
+    >>> from zope.schema.interfaces import IObject
+    >>> class IFileField(IObject):
+    ...     pass
+
+    >>> @implementer(IFileField)
+    ... class FileField(schema.Object):
+    ...     schema = IFileValue
+    ...     def __init__(self, **kw):
+    ...         if 'schema' in kw:
+    ...             self.schema = kw.pop('schema')
+    ...         super(FileField, self).__init__(schema=self.schema, **kw)
+
+We can register a field marshaler for this field which will do the following:
+
+* Insist that the field is only used as a primary field, since it makes
+  little sense to encode a binary file in a header.
+* Save the filename in a Content-Disposition header.
+* Be capable of reading the filename again from this header.
+* Encode the payload using base64
+
+    >>> from plone.rfc822.interfaces import IFieldMarshaler
+    >>> from email.encoders import encode_base64
+
+    >>> from zope.component import adapter
+    >>> from plone.rfc822.defaultfields import BaseFieldMarshaler
+
+    >>> @adapter(Interface, IFileField)
+    ... class FileFieldMarshaler(BaseFieldMarshaler):
+    ...
+    ...     ascii = False
+    ...
+    ...     def encode(self, value, charset='utf-8', primary=False):
+    ...         if not primary:
+    ...             raise ValueError("File field cannot be marshaled as a non-primary field")
+    ...         if value is None:
+    ...             return None
+    ...         return value.data
+    ...
+    ...     def decode(self, value, message=None, charset='utf-8', contentType=None, primary=False):
+    ...         filename = None
+    ...         # get the filename from the Content-Disposition header if possible
+    ...         if primary and message is not None:
+    ...             filename = message.get_filename(None)
+    ...         return FileValue(value, contentType, filename)
+    ...
+    ...     def getContentType(self):
+    ...         value = self._query()
+    ...         if value is None:
+    ...             return None
+    ...         return value.contentType
+    ...
+    ...     def getCharset(self, default='utf-8'):
+    ...         return None # this is not text data!
+    ...
+    ...     def postProcessMessage(self, message):
+    ...         value = self._query()
+    ...         if value is not None:
+    ...             filename = value.filename
+    ...             if filename:
+    ...                 # Add a new header storing the filename if we have one
+    ...                 message.add_header('Content-Disposition', 'attachment', filename=filename)
+
+    >>> from zope.component import provideAdapter
+    >>> provideAdapter(FileFieldMarshaler)
+
+To illustrate marshaling, let's create a content object that contains two file
+fields.
+
+    >>> class IFileContent(Interface):
+    ...     file1 = FileField()
+    ...     file2 = FileField()
+
+    >>> @implementer(IFileContent)
+    ... class FileContent(object):
+    ...     file1 = None
+    ...     file2 = None
+
+    >>> fileContent = FileContent()
+    >>> fileContent.file1 = FileValue('dummy file', 'text/plain', 'dummy1.txt')
+    >>> fileContent.file2 = FileValue('<html><body>test</body></html>', 'text/html', 'dummy2.html')
+
+At this point, neither of these fields is marked as a primary field. Let's see
+what happens when we attempt to construct a message from this schema.
+
+    >>> from plone.rfc822 import constructMessageFromSchema
+    >>> message = constructMessageFromSchema(fileContent, IFileContent)
+    >>> print(message.as_string())
+    <BLANKLINE>
+    <BLANKLINE>
+
+As expected, we got no message headers and no message body. Let's now mark one
+field as primary:
+
+    >>> from plone.rfc822.interfaces import IPrimaryField
+    >>> from zope.interface import alsoProvides
+    >>> alsoProvides(IFileContent['file1'], IPrimaryField)
+
+    >>> message = constructMessageFromSchema(fileContent, IFileContent)
+    >>> messageBody = message.as_string()
+    >>> print(messageBody)
+    MIME-Version: 1.0
+    Content-Type: text/plain
+    Content-Transfer-Encoding: base64
+    Content-Disposition: attachment; filename="dummy1.txt"
+    <BLANKLINE>
+    ZHVtbXkgZmlsZQ==
+
+Here, we have a base64 encoded payload, a Content-Disposition header, and a
+Content-Type header according to the primary field.
+
+We can also reconstruct the object from this message.
+
+    >>> from plone.rfc822 import initializeObjectFromSchema
+    >>> from email import message_from_string
+
+    >>> inputMessage = message_from_string(messageBody)
+    >>> newFileContent = FileContent()
+    >>> initializeObjectFromSchema(newFileContent, IFileContent, inputMessage)
+
+    >>> newFileContent.file1.data
+    b'dummy file'
+    >>> newFileContent.file1.contentType
+    'text/plain'
+    >>> newFileContent.file1.filename
+    'dummy1.txt'
+
+    >>> newFileContent.file2 is None
+    True
+
+Let's now show what would happen if we encoded both files in the message.
+In this case, we should get a multipart document with two payloads.
+
+    >>> alsoProvides(IFileContent['file2'], IPrimaryField)
+    >>> message = constructMessageFromSchema(fileContent, IFileContent)
+    >>> messageBody = message.as_string()
+    >>> print(messageBody) # doctest: +ELLIPSIS
+    MIME-Version: 1.0
+    Content-Type: multipart/mixed; boundary="===============...=="
+    <BLANKLINE>
+    --===============...==
+    MIME-Version: 1.0
+    Content-Type: text/plain
+    Content-Transfer-Encoding: base64
+    Content-Disposition: attachment; filename="dummy1.txt"
+    <BLANKLINE>
+    ZHVtbXkgZmlsZQ==
+    --===============...==
+    MIME-Version: 1.0
+    Content-Type: text/html
+    Content-Transfer-Encoding: base64
+    Content-Disposition: attachment; filename="dummy2.html"
+    <BLANKLINE>
+    PGh0bWw+PGJvZHk+dGVzdDwvYm9keT48L2h0bWw+
+    --===============...==--...
+
+And again, we can reconstruct the object, this time with both fields:
+
+    >>> inputMessage = message_from_string(messageBody)
+    >>> newFileContent = FileContent()
+    >>> initializeObjectFromSchema(newFileContent, IFileContent, inputMessage)
+
+    >>> newFileContent.file1.data
+    b'dummy file'
+    >>> newFileContent.file1.contentType
+    'text/plain'
+    >>> newFileContent.file1.filename
+    'dummy1.txt'
+
+    >>> newFileContent.file2.data
+    b'<html><body>test</body></html>'
+    >>> newFileContent.file2.contentType
+    'text/html'
+    >>> newFileContent.file2.filename
+    'dummy2.html'
+
+Specialities between Py2 and Py3
+--------------------------------
+
+Test a special behavior which is different between Python 2 and 3 stdlib:
+Newline handling in non-utf8 strings.
+
+Python 2.7 ``email.header`` keeps a line with an escaped value,
+while Python 3.6 turns it into RFC2047 encoded headers, see https://tools.ietf.org/html/rfc2047.html
+Technical both is fine.
+
+::
+
+    >>> content.description = "Test content\nwith newline difference"
+    >>> msg = constructMessageFromSchema(content, ITestContent)
+    >>> effective_output = msg.as_string()
+    >>> effective_output.split('\n')[1]
+    'description: =?utf-8?q?Test_content=5Cnwith_newline_difference?='
```

### Comparing `plone.rfc822-2.0.2/plone.rfc822.egg-info/SOURCES.txt` & `plone.rfc822-3.0.0/plone.rfc822.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 setup.py
 docs/INSTALL.txt
 docs/LICENSE.txt
 plone/__init__.py
 plone.rfc822.egg-info/PKG-INFO
 plone.rfc822.egg-info/SOURCES.txt
 plone.rfc822.egg-info/dependency_links.txt
-plone.rfc822.egg-info/entry_points.txt
 plone.rfc822.egg-info/namespace_packages.txt
 plone.rfc822.egg-info/not-zip-safe
 plone.rfc822.egg-info/requires.txt
 plone.rfc822.egg-info/top_level.txt
 plone/rfc822/__init__.py
 plone/rfc822/_utils.py
 plone/rfc822/configure.zcml
```

### Comparing `plone.rfc822-2.0.2/docs/INSTALL.txt` & `plone.rfc822-3.0.0/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.rfc822-2.0.2/docs/LICENSE.txt` & `plone.rfc822-3.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.rfc822-2.0.2/setup.py` & `plone.rfc822-3.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,64 @@
-# -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = '2.0.2'
+version = "3.0.0"
 
 setup(
-    name='plone.rfc822',
+    name="plone.rfc822",
     version=version,
     description="RFC822 marshalling for zope.schema fields",
     long_description=(
-        open("README.rst").read() + "\n" +
-        open("CHANGES.rst").read() + "\n" +
-        open(os.path.join("plone", "rfc822", "message.rst")).read()),
+        open("README.rst").read()
+        + "\n"
+        + open("CHANGES.rst").read()
+        + "\n"
+        + open(os.path.join("plone", "rfc822", "message.rst")).read()
+    ),
     # Get more strings from
     # https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
-        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: BSD License",
     ],
-    keywords='zope schema rfc822',
-    author='Martin Aspeli and contributors',
-    author_email='optilude@gmail.com',
-    url='https://pypi.org/project/plone.rfc822',
-    license='BSD',
+    keywords="zope schema rfc822",
+    author="Martin Aspeli and contributors",
+    author_email="optilude@gmail.com",
+    url="https://pypi.org/project/plone.rfc822",
+    license="BSD",
     packages=find_packages(),
-    namespace_packages=['plone'],
+    namespace_packages=["plone"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     extras_require={
-        'supermodel': ['plone.supermodel'],
-        'test': ['plone.testing', 'plone.supermodel'],
+        "supermodel": ["plone.supermodel"],
+        "test": [
+            "plone.testing",
+            "plone.supermodel",
+            "zope.annotation",
+            "zope.configuration",
+            "persistent",
+        ],
     },
     install_requires=[
-        'python-dateutil',
-        'setuptools',
-        'zope.component',
-        'zope.deprecation',
-        'zope.interface',
-        'zope.schema',
+        "python-dateutil",
+        "setuptools",
+        "zope.component",
+        "zope.interface",
+        "zope.schema",
     ],
     entry_points="""
     """,
 )
```

### Comparing `plone.rfc822-2.0.2/plone/rfc822/fields.rst` & `plone.rfc822-3.0.0/plone/rfc822/fields.rst`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     ...     _frozenset = schema.FrozenSet(value_type=schema.Timedelta())
 
 This interface is implemented by a the following class::
 
     >>> from decimal import Decimal
     >>> from zope.interface import implementer
     >>> import datetime
-    >>> import six
     >>> @implementer(ITestContent)
     ... class TestContent(object):
     ...     _text = u"text\xd8"
     ...     _text2 = u"text" # ascii safe
     ...     _textLine = u"textline\xd8"
     ...     _textLine2 = u"textline" # ascii safe
     ...     _password = u"password\xd8"
@@ -76,15 +75,15 @@
     ...     _bytesLine = 'bytesline'
     ...     _ascii = u'ascii'
     ...     _asciiLine = u'asciiline'
     ...     _uri = u'http://plone.org'
     ...     _id = u'some.id'
     ...     _dottedName = 'dotted.name'
     ...     _bool = True
-    ...     _int = long(-10) if six.PY2 else -10
+    ...     _int = -10
     ...     _float = 0.3
     ...     _decimal = Decimal("5.0")
     ...     _choice1 = u"two"
     ...     _choice2 = 'two'
     ...     _datetime = datetime.datetime(2009, 1, 2, 15, 10, 5, 1, tz)
     ...     _date = datetime.date(2008, 2, 3)
     ...     _timedelta = datetime.timedelta(3, 4, 5)
@@ -113,30 +112,30 @@
 Text
 ----
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_text']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'text\xc3\x98'
+    b'text\xc3\x98'
     >>> marshaler.decode(b'text\xc3\x98')
     'text\xd8'
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8')
     'utf-8'
     >>> marshaler.ascii
     False
 
 Text field types and derivatives will return True for the ``ascii`` property
 if the field value is within the ascii range::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_text2']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'text'
+    b'text'
     >>> marshaler.decode(b'text\xc3\x98')
     'text\xd8'
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8')
     'utf-8'
     >>> marshaler.ascii
@@ -145,15 +144,15 @@
 TextLine
 --------
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_textLine']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'textline\xc3\x98'
+    b'textline\xc3\x98'
     >>> marshaler.decode(b'textline\xc3\x98')
     'textline\xd8'
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8')
     'utf-8'
     >>> marshaler.ascii
@@ -162,15 +161,15 @@
 Text field types and derivatives will return True for the ``ascii`` property
 if the field value is within the ascii range.
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_textLine2']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'textline'
+    b'textline'
     >>> marshaler.decode(b'textline\xc3\x98')
     'textline\xd8'
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8')
     'utf-8'
     >>> marshaler.ascii
@@ -179,15 +178,15 @@
 Password
 --------
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_password']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'password\xc3\x98'
+    b'password\xc3\x98'
     >>> marshaler.decode(b'password\xc3\x98')
     'password\xd8'
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8')
     'utf-8'
     >>> marshaler.ascii
@@ -196,15 +195,15 @@
 Text field types and derivatives will return True for the ``ascii`` property
 if the field value is within the ascii range.
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_password2']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'password'
+    b'password'
     >>> marshaler.decode(b'password\xc3\x98')
     'password\xd8'
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8')
     'utf-8'
     >>> marshaler.ascii
@@ -215,15 +214,15 @@
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_bytes']), IFieldMarshaler)
     >>> marshaler.marshal()
     'bytes'
     >>> marshaler.decode(b'bytes')
-    'bytes'
+    b'bytes'
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8') is None
     True
     >>> marshaler.ascii
     True
 
@@ -232,15 +231,15 @@
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_bytesLine']), IFieldMarshaler)
     >>> marshaler.marshal()
     'bytesline'
     >>> marshaler.decode(b'bytesline')
-    'bytesline'
+    b'bytesline'
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8') is None
     True
     >>> marshaler.ascii
     True
 
@@ -250,15 +249,15 @@
 This is an ASCII field which is supposed to store text strings.
 Note: There is a BytesField which stores b'foo' binary string.
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_ascii']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'ascii'
+    b'ascii'
     >>> marshaler.decode(b'ascii')
     'ascii'
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8') is None
     True
     >>> marshaler.ascii
@@ -267,15 +266,15 @@
 ASCIILine
 ---------
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_asciiLine']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'asciiline'
+    b'asciiline'
     >>> marshaler.decode(b'asciiline')
     'asciiline'
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8') is None
     True
     >>> marshaler.ascii
@@ -286,81 +285,72 @@
 
 An URI is in Python 2 based on unicode text, in Python 3 on bytes.
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_uri']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'http://plone.org'
+    b'http://plone.org'
     >>> marshaler.decode(b'http://plone.org')
     'http://plone.org'
     >>> marshaler.getContentType() is None
     True
-    >>> if six.PY2:
-    ...     expected = None  # its IBytes based
-    ... else:
-    ...     expected = 'utf-8'
+    >>> expected = 'utf-8'
     >>> marshaler.getCharset('utf-8') == expected
     True
     >>> marshaler.ascii
     True
 
 Id
 --
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_id']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'some.id'
+    b'some.id'
     >>> marshaler.decode(b'some.id')
     'some.id'
     >>> marshaler.getContentType() is None
     True
-    >>> if six.PY2:
-    ...     expected = None  # its IBytes based
-    ... else:
-    ...     expected = 'utf-8'
+    >>> expected = 'utf-8'
     >>> marshaler.getCharset('utf-8') == expected
     True
     >>> marshaler.ascii
     True
 
 DottedName
 ----------
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_dottedName']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'dotted.name'
+    b'dotted.name'
     >>> marshaler.decode(b'dotted.name')
     'dotted.name'
     >>> marshaler.getContentType() is None
     True
-    >>> if six.PY2:
-    ...     expected = None  # its IBytes based
-    ... else:
-    ...     expected = 'utf-8'
+    >>> expected = 'utf-8'
     >>> marshaler.getCharset('utf-8') == expected
     True
     >>> marshaler.ascii
     True
 
 Bool
 ----
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_bool']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'True'
+    b'True'
     >>> t._bool = False
     >>> marshaler.marshal()
-    'False'
+    b'False'
     >>> t._bool = True
     >>> marshaler.decode(b'True')
     True
     >>> marshaler.decode(b'False')
     False
     >>> marshaler.getContentType() is None
     True
@@ -372,15 +362,15 @@
 Int
 ---
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_int']), IFieldMarshaler)
     >>> marshaler.marshal()
-    '-10'
+    b'-10'
     >>> marshaler.decode(b'-10')
     -10
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8') is None
     True
     >>> marshaler.ascii
@@ -389,15 +379,15 @@
 Float
 -----
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_float']), IFieldMarshaler)
     >>> marshaler.marshal()
-    '0.3'
+    b'0.3'
     >>> marshaler.decode(b'0.25')
     0.25
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8') is None
     True
     >>> marshaler.ascii
@@ -406,15 +396,15 @@
 Decimal
 -------
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_decimal']), IFieldMarshaler)
     >>> marshaler.marshal()
-    '5.0'
+    b'5.0'
     >>> marshaler.decode(b'5.0')
     Decimal('5.0')
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8') is None
     True
     >>> marshaler.ascii
@@ -423,27 +413,27 @@
 Choice
 ------
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_choice1']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'two'
+    b'two'
     >>> marshaler.decode(b'one')
     'one'
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8')
     'utf-8'
     >>> marshaler.ascii
     True
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_choice2']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'two'
+    b'two'
     >>> marshaler.decode(b'three')
     'three'
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8')
     'utf-8'
     >>> marshaler.ascii
@@ -503,15 +493,15 @@
 Tuple
 -----
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_tuple']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'one\xc3\x98||two'
+    b'one\xc3\x98||two'
     >>> marshaler.decode(b'one\xc3\x98||two')
     ('one\xd8', 'two')
     >>> marshaler.getContentType() is None
     True
     >>> marshaler.getCharset('utf-8')
     'utf-8'
     >>> marshaler.ascii
@@ -520,15 +510,15 @@
 List
 ----
 
 ::
 
     >>> marshaler = getMultiAdapter((t, ITestContent['_list']), IFieldMarshaler)
     >>> marshaler.marshal()
-    'three||four'
+    b'three||four'
     >>> marshaler.decode(b'three||four')
     ['three', 'four']
     >>> marshaler.getContentType() is None
     True
 
     ValueType of the list is ASCIILine!
     >>> marshaler.getCharset('utf-8') is None
```

### Comparing `plone.rfc822-2.0.2/plone/rfc822/interfaces.py` & `plone.rfc822-3.0.0/plone/rfc822/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-# -*- coding: utf-8 -*-
 from zope import schema
 from zope.interface import Attribute
 from zope.interface import Interface
 
 
 class IPrimaryField(Interface):
-    """Marker interface for the primary field in a schema
-    """
+    """Marker interface for the primary field in a schema"""
 
 
 class IPrimaryFieldInfo(Interface):
     """Information about the primary field of a content item
 
     Content type frameworks should register an adapter to this interface.
     """
+
     fieldname = Attribute("Field name")
     field = Attribute("Field")
     value = Attribute("Field value")
 
 
 class IMessageAPI(Interface):
     """Functions provided by this module
 
-    These can all be imported as::
+    These can all be imported as:
 
-        >>> from plone.rfc822 import constructMessage
+    from plone.rfc822 import constructMessage
     """
 
-    def constructMessageFromSchema(context, schema, charset='utf-8'):
+    def constructMessageFromSchema(context, schema, charset="utf-8"):
         """Convenience method which calls ``constructMessage()`` with all the
         fields, in order, of the given schema interface
         """
 
-    def constructMessageFromSchemata(context, schemata, charset='utf-8'):
+    def constructMessageFromSchemata(context, schemata, charset="utf-8"):
         """Convenience method which calls ``constructMessage()`` with all the
         fields, in order, of all the given schemata (a sequence of schema
         interfaces).
         """
 
-    def constructMessage(context, fields, charset='utf-8'):
+    def constructMessage(context, fields, charset="utf-8"):
         """Helper method to construct a message.
 
         ``context`` is a content object.
 
         ``fields`` is a sequence of (name, field) pairs for the fields which
         make up the message. This can be obtained from
         zope.schema.getFieldsInOrder, for example.
@@ -61,36 +60,28 @@
 
     def renderMessage(message, mangleFromHeader=False):
         """Render a message to a string
 
         DEPRECATED. Use 'message.as_string()' instead.
         """
 
-    def initializeObjectFromSchema(
-        context,
-        schema,
-        message,
-        defaultCharset='utf-8'
-    ):
+    def initializeObjectFromSchema(context, schema, message, defaultCharset="utf-8"):
         """Convenience method which calls ``initializeObject()`` with all the
         fields, in order, of the given schema interface
         """
 
     def initializeObjectFromSchemata(
-        context,
-        schemata,
-        message,
-        defaultCharset='utf-8'
+        context, schemata, message, defaultCharset="utf-8"
     ):
         """Convenience method which calls ``initializeObject()`` with all the
         fields in order, of all the given schemata (a sequence of schema
         interfaces).
         """
 
-    def initializeObject(context, fields, message, defaultCharset='utf-8'):
+    def initializeObject(context, fields, message, defaultCharset="utf-8"):
         """Initialise an object from a message.
 
         ``context`` is the content object to initialise.
 
         ``fields`` is a sequence of (name, field) pairs for the fields which
         make up the message. This can be obtained from
         zope.schema.getFieldsInOrder, for example.
@@ -109,23 +100,23 @@
     demarshalling from RFC2822 message headers.
 
     This interface deals in six.text_type strings, which will be
     encoded/decoded elsewhere.
     """
 
     ascii = schema.Bool(
-        title=u"ASCII only",
-        description=u"Set this to true if this marshaler is guaranteed "
+        title="ASCII only",
+        description="Set this to true if this marshaler is guaranteed "
         "to return ASCII characters only. This will allow "
         "a header to be rendered without an encoding wrapper",
         default=False,
         required=True,
     )
 
-    def marshal(charset='utf-8', primary=False):
+    def marshal(charset="utf-8", primary=False):
         """Return the value of the adapted field on the adapted context.
 
         Note: It may be necessary to adapt the context to the field's
               interface (``field.interface``) before getting the value.
 
         ``charset`` is the default message charset. For string values, you
         should use this charset to encode the string. For binary values,
@@ -138,19 +129,15 @@
         in the field.
 
         Raise ``ValueError`` if marshaling is impossible. The field will be
         skipped.
         """
 
     def demarshal(
-        value,
-        message=None,
-        charset='utf-8',
-        contentType=None,
-        primary=False
+        value, message=None, charset="utf-8", contentType=None, primary=False
     ):
         """Update the value of the adapted field on the adapted context.
 
         Note: It may be necessary to adapt the context to the field's
               interface (``field.interface``) before getting the value.
 
         ``value`` is the string value from the message.
@@ -167,31 +154,25 @@
 
         ``contentType`` is the ``Content-Type`` header from the message, or
         None if this is not available. This is mainly used for primary fields.
 
         Raise ``ValueError`` if the demarshalling cannot be completed.
         """
 
-    def encode(value, charset='utf-8', primary=False):
+    def encode(value, charset="utf-8", primary=False):
         """Like marshal(), but acts on the passed-in ``value`` instead of
         reading it from the field.
 
         This is only used for collection fields and other situations where
         the value is not read from an instance.
 
         Return None if the value cannot be encoded.
         """
 
-    def decode(
-        value,
-        message=None,
-        charset='utf-8',
-        contentType=None,
-        primary=False
-    ):
+    def decode(value, message=None, charset="utf-8", contentType=None, primary=False):
         """Like demarshal, but return the value instead of updating the field.
 
         This is only used for collection fields and other situations where
         the instance should not be updated directly.
 
         Raise ValueError if the value cannot be extracted.
         """
@@ -200,15 +181,15 @@
         """Return the MIME type of the field. The value should be appropriate
         for the Content-Type HTTP header. This is mainly used for marshalling
         the primary field to the message body.
 
         May return None if a content type does not make sense.
         """
 
-    def getCharset(defualt='utf-8'):
+    def getCharset(default="utf-8"):
         """Return the charset of the field. The value should be appropriate
         for the 'charset' parameter to the Content-Type HTTP header. This is
         mainly used for marshalling
 
         The ``default`` parameter contains the message's default charset.
 
         Must return None if the message should not have a charset, i.e. it
```

### Comparing `plone.rfc822-2.0.2/plone/rfc822/configure.zcml` & `plone.rfc822-3.0.0/plone/rfc822/configure.zcml`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,101 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:five="http://namespaces.zope.org/five"
     xmlns:zcml="http://namespaces.zope.org/zcml"
-    i18n_domain="plone.rfc822">
+    i18n_domain="plone.rfc822"
+    >
 
-    <!-- Standard IFromUnicode marshaler -->
-    <adapter factory=".defaultfields.UnicodeFieldMarshaler" />
+  <!-- Standard IFromUnicode marshaler -->
+  <adapter factory=".defaultfields.UnicodeFieldMarshaler" />
 
-    <!-- Text, TextLine, Password, SourceText may be ASCII safe -->
-    <adapter
-        for="* zope.schema.interfaces.INativeString"
-        factory=".defaultfields.UnicodeValueFieldMarshaler"
-        />
-    <!-- ASCII Field marshaller -->
-    <adapter
-        for="* zope.schema.interfaces.IASCII"
-        factory=".defaultfields.ASCIISafeFieldMarshaler"
-        />
-    <adapter
-        for="* zope.schema.interfaces.IASCIILine"
-        factory=".defaultfields.ASCIISafeFieldMarshaler"
-        />
-
-    <!-- Bool and Choice omit to declare that they supports IFromUnicode in zope.schema 3.3 -->
-    <adapter
-        for="* zope.schema.interfaces.IBool"
-        factory=".defaultfields.ASCIISafeFieldMarshaler"
-        />
-    <!-- We need this as a workaround for this issue:
+  <!-- Text, TextLine, Password, SourceText may be ASCII safe -->
+  <adapter
+      factory=".defaultfields.UnicodeValueFieldMarshaler"
+      for="*
+           zope.schema.interfaces.INativeString"
+      />
+  <!-- ASCII Field marshaller -->
+  <adapter
+      factory=".defaultfields.ASCIISafeFieldMarshaler"
+      for="*
+           zope.schema.interfaces.IASCII"
+      />
+  <adapter
+      factory=".defaultfields.ASCIISafeFieldMarshaler"
+      for="*
+           zope.schema.interfaces.IASCIILine"
+      />
+
+  <!-- Bool and Choice omit to declare that they supports IFromUnicode in zope.schema 3.3 -->
+  <adapter
+      factory=".defaultfields.ASCIISafeFieldMarshaler"
+      for="*
+           zope.schema.interfaces.IBool"
+      />
+  <!-- We need this as a workaround for this issue:
       https://github.com/zopefoundation/zope.schema/issues/80
     -->
-    <adapter
-        for="* zope.schema._bootstrapfields.Bool"
-        factory=".defaultfields.ASCIISafeFieldMarshaler"
-        />
-    <adapter
-        for="* zope.schema.interfaces.IChoice"
-        factory=".defaultfields.UnicodeValueFieldMarshaler"
-        />
-
-    <!-- Int, Float, and Decimal are ASCII safe -->
-    <adapter
-        for="* zope.schema.interfaces.IInt"
-        factory=".defaultfields.ASCIISafeFieldMarshaler"
-        />
-    <adapter
-        for="* zope.schema.interfaces.IFloat"
-        factory=".defaultfields.ASCIISafeFieldMarshaler"
-        />
-    <adapter
-        for="* zope.schema.interfaces.IDecimal"
-        factory=".defaultfields.ASCIISafeFieldMarshaler"
-        />
-
-    <!-- Somehow this is necessary because these are in _bootstrapfields -->
-    <adapter
-        for="* zope.schema.Text"
-        factory=".defaultfields.UnicodeValueFieldMarshaler"
-        />
-    <adapter
-        for="* zope.schema.TextLine"
-        factory=".defaultfields.UnicodeValueFieldMarshaler"
-        />
-    <adapter
-        for="* zope.schema.Password"
-        factory=".defaultfields.UnicodeValueFieldMarshaler"
-        />
-    <adapter
-        for="* zope.schema.Int"
-        factory=".defaultfields.ASCIISafeFieldMarshaler"
-        />
-
-    <adapter factory=".defaultfields.BytesFieldMarshaler" />
-    <adapter factory=".defaultfields.DatetimeMarshaler" />
-    <adapter factory=".defaultfields.DateMarshaler" />
-    <adapter factory=".defaultfields.TimedeltaMarshaler" />
-    <adapter factory=".defaultfields.CollectionMarshaler" />
-
-    <!-- Configure plone.supermodel handler if available -->
-    <utility zcml:condition="installed plone.supermodel"
-        factory=".supermodel.PrimaryFieldMetadataHandler"
-        name="plone.rfc822.marshal"
-        />
+  <adapter
+      factory=".defaultfields.ASCIISafeFieldMarshaler"
+      for="*
+           zope.schema._bootstrapfields.Bool"
+      />
+  <adapter
+      factory=".defaultfields.UnicodeValueFieldMarshaler"
+      for="*
+           zope.schema.interfaces.IChoice"
+      />
+
+  <!-- Int, Float, and Decimal are ASCII safe -->
+  <adapter
+      factory=".defaultfields.ASCIISafeFieldMarshaler"
+      for="*
+           zope.schema.interfaces.IInt"
+      />
+  <adapter
+      factory=".defaultfields.ASCIISafeFieldMarshaler"
+      for="*
+           zope.schema.interfaces.IFloat"
+      />
+  <adapter
+      factory=".defaultfields.ASCIISafeFieldMarshaler"
+      for="*
+           zope.schema.interfaces.IDecimal"
+      />
+
+  <!-- Somehow this is necessary because these are in _bootstrapfields -->
+  <adapter
+      factory=".defaultfields.UnicodeValueFieldMarshaler"
+      for="*
+           zope.schema.Text"
+      />
+  <adapter
+      factory=".defaultfields.UnicodeValueFieldMarshaler"
+      for="*
+           zope.schema.TextLine"
+      />
+  <adapter
+      factory=".defaultfields.UnicodeValueFieldMarshaler"
+      for="*
+           zope.schema.Password"
+      />
+  <adapter
+      factory=".defaultfields.ASCIISafeFieldMarshaler"
+      for="*
+           zope.schema.Int"
+      />
+
+  <adapter factory=".defaultfields.BytesFieldMarshaler" />
+  <adapter factory=".defaultfields.DatetimeMarshaler" />
+  <adapter factory=".defaultfields.DateMarshaler" />
+  <adapter factory=".defaultfields.TimedeltaMarshaler" />
+  <adapter factory=".defaultfields.CollectionMarshaler" />
+
+  <!-- Configure plone.supermodel handler if available -->
+  <utility
+      factory=".supermodel.PrimaryFieldMetadataHandler"
+      name="plone.rfc822.marshal"
+      zcml:condition="installed plone.supermodel"
+      />
 
 </configure>
```

### Comparing `plone.rfc822-2.0.2/plone/rfc822/defaultfields.py` & `plone.rfc822-3.0.0/plone/rfc822/defaultfields.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Default field marshalers for the fields in zope.schema.
 
 Note that none of the marshalers will return a value for getContentType(),
 because none of the standard field types maintain this information.
 
 These field implement IFromUnicode and are supported by a single marshaler:
 
@@ -41,201 +40,188 @@
 from zope.schema.interfaces import IDate
 from zope.schema.interfaces import IDatetime
 from zope.schema.interfaces import IFromUnicode
 from zope.schema.interfaces import ITimedelta
 
 import datetime
 import dateutil.parser
-import six
 
 
 _marker = object()
 
 
 @implementer(IFieldMarshaler)
-class BaseFieldMarshaler(object):
-    """Base class for field marshalers
-    """
+class BaseFieldMarshaler:
+    """Base class for field marshalers"""
 
     ascii = False
 
     def __init__(self, context, field):
         self.context = context
         self.field = field.bind(context)
         self.instance = context
         if field.interface is not None:
             self.instance = field.interface(context, context)
 
-    def marshal(self, charset='utf-8', primary=False):
+    def marshal(self, charset="utf-8", primary=False):
         value = self._query(_marker)
-        return (
-            None if value is _marker else self.encode(value, charset, primary)
-        )
+        return None if value is _marker else self.encode(value, charset, primary)
 
     def demarshal(
         self,
         value,
         message=None,
-        charset='utf-8',
+        charset="utf-8",
         contentType=None,
         primary=False,
     ):
-
         if value:
-            fieldValue = self.decode(
-                value, message, charset, contentType, primary
-            )
+            fieldValue = self.decode(value, message, charset, contentType, primary)
         else:
             fieldValue = self.field.missing_value
         self._set(fieldValue)
 
-    def encode(self, value, charset='utf-8', primary=False):
+    def encode(self, value, charset="utf-8", primary=False):
         return None
 
     def decode(
         self,
         value,
         message=None,
-        charset='utf-8',
+        charset="utf-8",
         contentType=None,
         primary=False,
     ):
-        raise ValueError(
-            'Demarshalling not implemented for %s' % repr(self.field)
-        )
+        raise ValueError("Demarshalling not implemented for %s" % repr(self.field))
 
     def getContentType(self):
         return None
 
-    def getCharset(self, default='utf-8'):
+    def getCharset(self, default="utf-8"):
         return None
 
     def postProcessMessage(self, message):
         pass
 
     # Helper methods
 
     def _query(self, default=None):
         return self.field.query(self.instance, default)
 
     def _set(self, value):
-        if getattr(self.instance, 'marker', False):
+        if getattr(self.instance, "marker", False):
             print(self.field.__name__)
             print(value)
-            print('-' * 5)
+            print("-" * 5)
         try:
             self.field.set(self.instance, value)
         except TypeError as e:
             raise ValueError(e)
 
 
 @adapter(Interface, IFromUnicode)
 class UnicodeFieldMarshaler(BaseFieldMarshaler):
-    """Default marshaler for fields that support IFromUnicode
-    """
+    """Default marshaler for fields that support IFromUnicode"""
 
-    def encode(self, value, charset='utf-8', primary=False):
+    def encode(self, value, charset="utf-8", primary=False):
         if value is None:
             return
-        if isinstance(value, six.binary_type):
+        if isinstance(value, bytes):
             # value already encoded
             return value
-        return six.text_type(value).encode(charset)
+        return str(value).encode(charset)
 
     def decode(
         self,
         value,
         message=None,
-        charset='utf-8',
+        charset="utf-8",
         contentType=None,
         primary=False,
     ):
-        if isinstance(value, six.binary_type):
+        if isinstance(value, bytes):
             unicodeValue = value.decode(charset)
         else:
             unicodeValue = value
         try:
             return self.field.fromUnicode(unicodeValue)
         except Exception as e:
             raise ValueError(e)
 
-    def getCharset(self, default='utf-8'):
+    def getCharset(self, default="utf-8"):
         return default
 
 
 class UnicodeValueFieldMarshaler(UnicodeFieldMarshaler):
     """Default marshaler for fields that contain unicode data and so may be
     ASCII safe.
     """
 
-    def encode(self, value, charset='utf-8', primary=False):
-        encoded = super(UnicodeValueFieldMarshaler, self).encode(
-            value, charset, primary
-        )
-        if not encoded or max(six.iterbytes(encoded)) < 128:
+    def encode(self, value, charset="utf-8", primary=False):
+        encoded = super().encode(value, charset, primary)
+        if not encoded or max(iter(encoded)) < 128:
             self.ascii = True
         else:
             self.ascii = False
         return encoded
 
 
 class ASCIISafeFieldMarshaler(UnicodeFieldMarshaler):
     """Default marshaler for fields that are ASCII safe, but still support
     IFromUnicode. This includes Int, Float, Decimal, and Bool.
     """
 
     ascii = True
 
-    def getCharset(self, default='utf-8'):
+    def getCharset(self, default="utf-8"):
         return None
 
 
 @adapter(Interface, IBytes)
 class BytesFieldMarshaler(BaseFieldMarshaler):
     """Default marshaler for IBytes fields and children. These store str
     objects, so we will attempt to encode them directly.
     """
 
     ascii = True
 
-    def encode(self, value, charset='utf-8', primary=False):
+    def encode(self, value, charset="utf-8", primary=False):
         return value
 
     def decode(
         self,
         value,
         message=None,
-        charset='utf-8',
+        charset="utf-8",
         contentType=None,
         primary=False,
     ):
         return value
 
 
 @adapter(Interface, IDatetime)
 class DatetimeMarshaler(BaseFieldMarshaler):
-    """Marshaler for Python datetime values
-    """
+    """Marshaler for Python datetime values"""
 
     ascii = True
 
-    def encode(self, value, charset='utf-8', primary=False):
+    def encode(self, value, charset="utf-8", primary=False):
         if value is None:
             return None
         return value.isoformat()
 
     def decode(
         self,
         value,
         message=None,
-        charset='utf-8',
+        charset="utf-8",
         contentType=None,
         primary=False,
     ):
-        if isinstance(value, six.binary_type):
+        if isinstance(value, bytes):
             value = value.decode(charset)
         try:
             return dateutil.parser.parse(value)
         except Exception as e:
             raise ValueError(e)
 
 
@@ -246,24 +232,24 @@
     Note: we don't use the date formatting support in the 'email' module as
     this does not seem to be capable of round-tripping values with time zone
     information.
     """
 
     ascii = True
 
-    def encode(self, value, charset='utf-8', primary=False):
+    def encode(self, value, charset="utf-8", primary=False):
         if value is None:
             return None
         return value.isoformat()
 
     def decode(
         self,
         value,
         message=None,
-        charset='utf-8',
+        charset="utf-8",
         contentType=None,
         primary=False,
     ):
         unicodeValue = value.decode(charset)
         try:
             return dateutil.parser.parse(unicodeValue).date()
         except Exception as e:
@@ -277,50 +263,49 @@
     Note: we don't use the date formatting support in the 'email' module as
     this does not seem to be capable of round-tripping values with time zone
     information.
     """
 
     ascii = True
 
-    def encode(self, value, charset='utf-8', primary=False):
+    def encode(self, value, charset="utf-8", primary=False):
         if value is None:
             return None
         return "%d:%d:%d" % (value.days, value.seconds, value.microseconds)
 
     def decode(
         self,
         value,
         message=None,
-        charset='utf-8',
+        charset="utf-8",
         contentType=None,
         primary=False,
     ):
         try:
-            days, seconds, microseconds = [int(v) for v in value.split(":")]
+            days, seconds, microseconds = (int(v) for v in value.split(":"))
             return datetime.timedelta(days, seconds, microseconds)
         except Exception as e:
             raise ValueError(e)
 
 
 @adapter(Interface, ICollection)
 class CollectionMarshaler(BaseFieldMarshaler):
-    """Marshaler for collection values
-    """
+    """Marshaler for collection values"""
 
     ascii = False
 
-    def getCharset(self, default='utf-8'):
+    def getCharset(self, default="utf-8"):
         valueTypeMarshaler = queryMultiAdapter(
             (self.context, self.field.value_type), IFieldMarshaler
         )
         if valueTypeMarshaler is None:
             return None
         return valueTypeMarshaler.getCharset(default)
 
-    def encode(self, value, charset='utf-8', primary=False):
+    def encode(self, value, charset="utf-8", primary=False):
         if value is None:
             return None
 
         valueTypeMarshaler = queryMultiAdapter(
             (self.context, self.field.value_type), IFieldMarshaler
         )
         if valueTypeMarshaler is None:
@@ -329,51 +314,49 @@
         ascii = True
         value_lines = []
         for item in value:
             marshaledValue = valueTypeMarshaler.encode(
                 item, charset=charset, primary=primary
             )
             if marshaledValue is None:
-                marshaledValue = ''
+                marshaledValue = ""
             value_lines.append(marshaledValue)
             if not valueTypeMarshaler.ascii:
                 ascii = False
 
         self.ascii = ascii
-        if value_lines and isinstance(value_lines[0], six.binary_type):
-            return b'||'.join(value_lines)
+        if value_lines and isinstance(value_lines[0], bytes):
+            return b"||".join(value_lines)
         else:
-            return '||'.join(value_lines)
+            return "||".join(value_lines)
 
     def decode(
         self,
         value,
         message=None,
-        charset='utf-8',
+        charset="utf-8",
         contentType=None,
         primary=False,
     ):
         valueTypeMarshaler = queryMultiAdapter(
             (self.context, self.field.value_type), IFieldMarshaler
         )
         if valueTypeMarshaler is None:
             raise ValueError(
-                'Cannot demarshal value type %s' % repr(self.field.value_type)
+                "Cannot demarshal value type %s" % repr(self.field.value_type)
             )
 
         listValue = []
-        if isinstance(value, six.binary_type):
-            lines = value.split(b'||')
+        if isinstance(value, bytes):
+            lines = value.split(b"||")
         else:
-            lines = value.split('||')
+            lines = value.split("||")
         for line in lines:
             listValue.append(
-                valueTypeMarshaler.decode(
-                    line, message, charset, contentType, primary
-                )
+                valueTypeMarshaler.decode(line, message, charset, contentType, primary)
             )
 
         sequenceType = self.field._type
         if isinstance(sequenceType, (list, tuple)):
             sequenceType = sequenceType[-1]
 
         return sequenceType(listValue)
```

### Comparing `plone.rfc822-2.0.2/plone/rfc822/message.rst` & `plone.rfc822-3.0.0/plone/rfc822/message.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     ...     <include package="plone.rfc822" />
     ...
     ... </configure>
     ... """
 
 ::
 
-    >>> from six import StringIO
+    >>> from io import StringIO
     >>> from zope.configuration import xmlconfig
     >>> xmlconfig.xmlconfig(StringIO(configuration))
 
 The primary field
 -----------------
 
 The message body is assumed to originate from a "primary" field, which is
@@ -143,15 +143,15 @@
 register it using the ``zope.component`` API.
 
     >>> from zope.component import provideAdapter
     >>> provideAdapter(TestBodyMarshaler)
 
 Hint: If the schema contained multiple text fields, this adapter would apply
 to all of them. To avoid that, we could either mark the field with a custom
-marker interface (similary to the way we marked a field with ``IPrimaryField``
+marker interface (similarly to the way we marked a field with ``IPrimaryField``
 above), or have the marshaler check the field name.
 
 Let's now try again:
 
     >>> msg = constructMessageFromSchema(content, ITestContent)
     >>> print(msg.as_string())
     title: Test title
@@ -550,15 +550,15 @@
     >>> from email import message_from_string
 
     >>> inputMessage = message_from_string(messageBody)
     >>> newFileContent = FileContent()
     >>> initializeObjectFromSchema(newFileContent, IFileContent, inputMessage)
 
     >>> newFileContent.file1.data
-    'dummy file'
+    b'dummy file'
     >>> newFileContent.file1.contentType
     'text/plain'
     >>> newFileContent.file1.filename
     'dummy1.txt'
 
     >>> newFileContent.file2 is None
     True
@@ -592,22 +592,22 @@
 And again, we can reconstruct the object, this time with both fields:
 
     >>> inputMessage = message_from_string(messageBody)
     >>> newFileContent = FileContent()
     >>> initializeObjectFromSchema(newFileContent, IFileContent, inputMessage)
 
     >>> newFileContent.file1.data
-    'dummy file'
+    b'dummy file'
     >>> newFileContent.file1.contentType
     'text/plain'
     >>> newFileContent.file1.filename
     'dummy1.txt'
 
     >>> newFileContent.file2.data
-    '<html><body>test</body></html>'
+    b'<html><body>test</body></html>'
     >>> newFileContent.file2.contentType
     'text/html'
     >>> newFileContent.file2.filename
     'dummy2.html'
 
 Specialities between Py2 and Py3
 --------------------------------
@@ -617,13 +617,12 @@
 
 Python 2.7 ``email.header`` keeps a line with an escaped value,
 while Python 3.6 turns it into RFC2047 encoded headers, see https://tools.ietf.org/html/rfc2047.html
 Technical both is fine.
 
 ::
 
-    >>> import six
     >>> content.description = "Test content\nwith newline difference"
     >>> msg = constructMessageFromSchema(content, ITestContent)
     >>> effective_output = msg.as_string()
     >>> effective_output.split('\n')[1]
     'description: =?utf-8?q?Test_content=5Cnwith_newline_difference?='
```

### Comparing `plone.rfc822-2.0.2/plone/rfc822/supermodel.rst` & `plone.rfc822-3.0.0/plone/rfc822/supermodel.rst`

 * *Files identical despite different names*

### Comparing `plone.rfc822-2.0.2/plone/rfc822/_utils.py` & `plone.rfc822-3.0.0/plone/rfc822/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,34 @@
-# -*- coding: utf-8 -*-
 """Implementation of IMessageAPI methods.
 
 import these from plone.rfc822 directly, not from this module.
 
 See interfaces.py for details.
 """
 from email.encoders import encode_base64
 from email.header import decode_header
 from email.header import Header
 from email.message import Message
 from plone.rfc822.interfaces import IFieldMarshaler
 from plone.rfc822.interfaces import IPrimaryField
 from zope.component import queryMultiAdapter
-from zope.deprecation import deprecate
 from zope.schema import getFieldsInOrder
 
 import logging
-import six
 
 
 logger = logging.getLogger("plone.rfc822")
 
 
-def safe_native_string(value, encoding='utf8'):
-    ''' Try to convert value into a native string
-    '''
-    if six.PY2:
-        if isinstance(value, six.text_type):
-            return value.encode(encoding)
-    elif isinstance(value, six.binary_type):
+def safe_native_string(value, encoding="utf8"):
+    """Try to convert value into a native string"""
+    if isinstance(value, bytes):
         return value.decode(encoding)
     if not isinstance(value, str):
-        raise ValueError('Cannot convert %r into a native string' % value)
+        raise ValueError("Cannot convert %r into a native string" % value)
     return value
 
 
 def constructMessageFromSchema(context, schema, charset="utf-8"):
     return constructMessage(context, getFieldsInOrder(schema), charset)
 
 
@@ -97,72 +90,50 @@
 
 def constructMessage(context, fields, charset="utf-8"):
     msg = Message()
     primaries = []
 
     # First get all headers, storing primary fields for later
     for name, field in fields:
-        value = ''
+        value = ""
         if IPrimaryField.providedBy(field):
             primaries.append((name, field))
             continue
         marshaler = queryMultiAdapter((context, field), IFieldMarshaler)
         if marshaler is None:
-            logger.debug(
-                "No marshaler found for field {0} of {1}".format(
-                    name, repr(context)
-                )
-            )
+            logger.debug(f"No marshaler found for field {name} of {repr(context)}")
             continue
         try:
             value = marshaler.marshal(charset, primary=False)
         except ValueError as e:
-            logger.debug(
-                "Marshaling of {0} for {1} failed: {2}".format(
-                    name, repr(context), str(e)
-                )
-            )
+            logger.debug(f"Marshaling of {name} for {repr(context)} failed: {str(e)}")
             continue
         if value is None:
             value = ""
         # Enforce native strings
         value = safe_native_string(value)
         if marshaler.ascii and "\n" not in value:
             msg[name] = value
         else:
             # see https://tools.ietf.org/html/rfc2822#section-3.2.2
-            if '\n' in value:
+            if "\n" in value:
                 value = value.replace("\n", r"\n")
             msg[name] = Header(value, charset)
 
     # Then deal with the primary field
     _add_payload_to_message(context, msg, primaries, charset)
 
     return msg
 
 
-@deprecate(
-    "Use 'message.as_string()' from 'email.message.Message' class instead."
-)
-def renderMessage(message, mangleFromHeader=False):
-    # to be removed in a 3.x series
-    return message.as_string(mangleFromHeader)
-
-
-def initializeObjectFromSchema(
-    context, schema, message, defaultCharset="utf-8"
-):
-    initializeObject(
-        context, getFieldsInOrder(schema), message, defaultCharset
-    )
-
-
-def initializeObjectFromSchemata(
-    context, schemata, message, defaultCharset="utf-8"
-):
+def initializeObjectFromSchema(context, schema, message, defaultCharset="utf-8"):
+    initializeObject(context, getFieldsInOrder(schema), message, defaultCharset)
+
+
+def initializeObjectFromSchemata(context, schemata, message, defaultCharset="utf-8"):
     """Convenience method which calls ``initializeObject()`` with all the
     fields in order, of all the given schemata (a sequence of schema
     interfaces).
     """
 
     fields = []
     for schema in schemata:
@@ -190,35 +161,31 @@
         header_fields.setdefault(name.lower(), []).append(field)
 
     # Demarshal each header
     for name, value in message.items():
         name = name.lower()
         fieldset = header_fields.get(name, None)
         if fieldset is None or len(fieldset) == 0:
-            logger.debug("No matching field found for header {0}".format(name))
+            logger.debug(f"No matching field found for header {name}")
             continue
         field = fieldset.pop(0)
         marshaler = queryMultiAdapter((context, field), IFieldMarshaler)
         if marshaler is None:
-            logger.debug(
-                "No marshaler found for field {0} of {1}".format(
-                    name, repr(context)
-                )
-            )
+            logger.debug(f"No marshaler found for field {name} of {repr(context)}")
             continue
         header_value, header_charset = decode_header(value)[0]
         if header_charset is None:
             header_charset = charset
 
         # MIME messages always use CRLF.
         # For headers, we're probably safer with \n
         #
         # Also, replace escaped Newlines, for details see
         # https://tools.ietf.org/html/rfc2822#section-3.2.2
-        if isinstance(header_value, six.binary_type):
+        if isinstance(header_value, bytes):
             header_value = header_value.replace(b"\r\n", b"\n")
             header_value = header_value.replace(b"\\n", b"\n")
         else:
             header_value = header_value.replace("\r\n", "\n")
             header_value = header_value.replace(r"\\n", "\n")
         try:
             marshaler.demarshal(
@@ -228,29 +195,29 @@
                 contentType=content_type,
                 primary=False,
             )
         except ValueError as e:
             # interface allows demarshal() to raise ValueError to indicate
             # marshalling failed
             logger.debug(
-                "Demarshalling of {0} for {1} failed: {2}".format(
+                "Demarshalling of {} for {} failed: {}".format(
                     name, repr(context), str(e)
                 )
             )
             continue
 
     # Then demarshal the primary field(s)
     payloads = message.get_payload()
 
     # do nothing if we don't have a payload
     if not payloads:
         return
 
     # A single payload is a string, multiparts are lists
-    if isinstance(payloads, six.string_types):
+    if isinstance(payloads, str):
         if len(primary) != 1:
             raise ValueError(
                 "Got a single string payload for message, but no primary "
                 "fields found for %s" % repr(context)
             )
         payloads = [message]
 
@@ -266,19 +233,15 @@
         if charset is not None:
             charset = str(charset)
         else:
             charset = "utf-8"
 
         marshaler = queryMultiAdapter((context, field), IFieldMarshaler)
         if marshaler is None:
-            logger.debug(
-                "No marshaler found for primary field {0} of {0}".format(
-                    name, repr(context)
-                )
-            )
+            logger.debug(f"No marshaler found for primary field {name} of {context!r}")
             continue
         payload_value = payload.get_payload(decode=True)
         payload_charset = payload.get_content_charset(charset)
         try:
             marshaler.demarshal(
                 payload_value,
                 message=payload,
@@ -286,12 +249,12 @@
                 contentType=payload_content_type,
                 primary=True,
             )
         except ValueError as e:
             # interface allows demarshal() to raise ValueError to
             # indicate marshalling failed
             logger.debug(
-                "Demarshalling of {0} for {1} failed: {2}".format(
+                "Demarshalling of {} for {} failed: {}".format(
                     name, repr(context), str(e)
                 )
             )
             continue
```

### Comparing `plone.rfc822-2.0.2/README.rst` & `plone.rfc822-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.rfc822-2.0.2/CHANGES.rst` & `plone.rfc822-3.0.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,33 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.0 (2023-04-26)
+------------------
+
+Breaking changes:
+
+
+- Remove long deprecated `renderMessage` function.
+  [@jensens] (1-1)
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
 2.0.2 (2020-04-22)
 ------------------
 
 Bug fixes:
 
 
 - Minor packaging updates. (#1)
```

