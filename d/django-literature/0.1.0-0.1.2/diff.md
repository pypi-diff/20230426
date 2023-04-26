# Comparing `tmp/django_literature-0.1.0.tar.gz` & `tmp/django_literature-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_literature-0.1.0.tar", max compression
+gzip compressed data, was "django_literature-0.1.2.tar", max compression
```

## Comparing `django_literature-0.1.0.tar` & `django_literature-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,50 @@
--rw-r--r--   0        0        0     1089 2023-01-22 13:37:50.598682 django_literature-0.1.0/LICENSE
--rw-r--r--   0        0        0     1723 2023-01-22 13:37:51.078682 django_literature-0.1.0/README.rst
--rw-r--r--   0        0        0       22 2023-01-22 14:25:57.538689 django_literature-0.1.0/literature/__init__.py
--rw-r--r--   0        0        0      124 2023-01-29 12:36:10.377767 django_literature-0.1.0/literature/adaptors/__init__.py
--rw-r--r--   0        0        0     3039 2023-01-27 16:13:52.212509 django_literature-0.1.0/literature/adaptors/base.py
--rw-r--r--   0        0        0     4120 2023-01-27 13:44:47.942639 django_literature-0.1.0/literature/adaptors/bibtex.py
--rw-r--r--   0        0        0     1837 2023-01-27 19:36:29.492330 django_literature-0.1.0/literature/adaptors/crossref.py
--rw-r--r--   0        0        0      964 2023-01-29 12:42:30.727759 django_literature-0.1.0/literature/adaptors/datacite.py
--rw-r--r--   0        0        0      259 2023-01-26 11:51:39.952813 django_literature-0.1.0/literature/adaptors/ris.py
--rw-r--r--   0        0        0     8468 2023-02-09 16:47:45.607047 django_literature-0.1.0/literature/admin.py
--rw-r--r--   0        0        0      441 2023-01-27 16:14:29.472508 django_literature-0.1.0/literature/apps.py
--rw-r--r--   0        0        0      710 2023-01-19 14:42:05.397873 django_literature-0.1.0/literature/choices.py
--rw-r--r--   0        0        0      880 2023-01-26 16:42:23.783242 django_literature-0.1.0/literature/conf.py
--rw-r--r--   0        0        0      192 2023-01-27 12:32:17.422703 django_literature-0.1.0/literature/exceptions.py
--rw-r--r--   0        0        0      761 2023-02-01 14:08:24.137874 django_literature-0.1.0/literature/fields.py
--rw-r--r--   0        0        0     4463 2023-02-01 13:56:30.517888 django_literature-0.1.0/literature/managers.py
--rw-r--r--   0        0        0    16773 2023-01-27 19:22:39.072342 django_literature-0.1.0/literature/migrations/0001_initial.py
--rw-r--r--   0        0        0      581 2023-02-11 12:13:50.929993 django_literature-0.1.0/literature/migrations/0002_alter_literature_authors.py
--rw-r--r--   0        0        0        0 2022-12-12 09:15:45.708496 django_literature-0.1.0/literature/migrations/__init__.py
--rw-r--r--   0        0        0     8837 2023-02-04 17:39:02.636526 django_literature-0.1.0/literature/models.py
--rw-r--r--   0        0        0      452 2023-01-22 23:27:58.860336 django_literature-0.1.0/literature/templates/admin/pdf_file_input.html
--rw-r--r--   0        0        0        0 2023-01-11 17:13:43.116699 django_literature-0.1.0/literature/templates/literature/literature_detail.html
--rw-r--r--   0        0        0        0 2023-01-11 17:13:31.896699 django_literature-0.1.0/literature/templates/literature/literature_list.html
--rw-r--r--   0        0        0     2214 2023-01-27 15:59:06.772521 django_literature-0.1.0/literature/utils.py
--rw-r--r--   0        0        0      268 2023-01-22 13:49:20.948684 django_literature-0.1.0/literature/views.py
--rw-r--r--   0        0        0      144 2023-01-22 23:34:55.020334 django_literature-0.1.0/literature/widgets.py
--rw-r--r--   0        0        0     1071 2023-03-23 11:57:05.398679 django_literature-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2392 1970-01-01 00:00:00.000000 django_literature-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-25 14:17:45.323626 django_literature-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1736 2023-04-25 14:17:45.323626 django_literature-0.1.2/README.rst
+-rw-r--r--   0        0        0       22 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/__init__.py
+-rw-r--r--   0        0        0     6237 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/admin.py
+-rw-r--r--   0        0        0        0 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/api/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/api/serialize.py
+-rw-r--r--   0        0        0      249 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/api/urls.py
+-rw-r--r--   0        0        0      370 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/api/views.py
+-rw-r--r--   0        0        0      250 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/apps.py
+-rw-r--r--   0        0        0     2514 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/choices.py
+-rw-r--r--   0        0        0      724 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/conf.py
+-rw-r--r--   0        0        0    36126 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/csl_map.py
+-rw-r--r--   0        0        0     1332 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/drf.py
+-rw-r--r--   0        0        0      192 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/exceptions.py
+-rw-r--r--   0        0        0      761 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/fields.py
+-rw-r--r--   0        0        0     5189 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/forms.py
+-rw-r--r--   0        0        0     2906 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/formset.py
+-rw-r--r--   0        0        0     4159 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/managers.py
+-rw-r--r--   0        0        0    13989 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/migrations/0001_initial.py
+-rw-r--r--   0        0        0      655 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/migrations/0002_alter_literature_published.py
+-rw-r--r--   0        0        0      478 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/migrations/0003_literature_csl.py
+-rw-r--r--   0        0        0     2871 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/migrations/0004_remove_literature_doi_remove_literature_isbn_and_more.py
+-rw-r--r--   0        0        0      577 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/migrations/0005_remove_literature_pid_remove_literature_pid_type_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/migrations/__init__.py
+-rw-r--r--   0        0        0     8632 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/models.py
+-rw-r--r--   0        0        0     6071 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/base.html
+-rw-r--r--   0        0        0     2370 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/admin/change_list.html
+-rw-r--r--   0        0        0     2085 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/admin/search.html
+-rw-r--r--   0        0        0      615 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/author_detail.html
+-rw-r--r--   0        0        0     1349 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/author_list.html
+-rw-r--r--   0        0        0       73 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/bibliography.html
+-rw-r--r--   0        0        0      665 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/citation/bootstrap.html
+-rw-r--r--   0        0        0      465 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/citation/plain_text.html
+-rw-r--r--   0        0        0      332 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/literature_detail.html
+-rw-r--r--   0        0        0     1591 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/literature_form.html
+-rw-r--r--   0        0        0      788 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/literature_form1.html
+-rw-r--r--   0        0        0      186 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/literature_list.html
+-rw-r--r--   0        0        0      301 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/widgets/identifier.html
+-rw-r--r--   0        0        0     1128 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/widgets/pdf_viewer.html
+-rw-r--r--   0        0        0     1120 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/widgets/postgres_array_widget.html
+-rw-r--r--   0        0        0      348 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templates/literature/widgets/preview.html
+-rw-r--r--   0        0        0        0 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templatetags/__init__.py
+-rw-r--r--   0        0        0      568 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/templatetags/literature.py
+-rw-r--r--   0        0        0     1296 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/test.py
+-rw-r--r--   0        0        0      429 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/urls.py
+-rw-r--r--   0        0        0     1241 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/utils.py
+-rw-r--r--   0        0        0     3040 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/views.py
+-rw-r--r--   0        0        0      538 2023-04-25 14:17:45.323626 django_literature-0.1.2/literature/widgets.py
+-rw-r--r--   0        0        0     3936 2023-04-25 14:18:11.520056 django_literature-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3080 1970-01-01 00:00:00.000000 django_literature-0.1.2/PKG-INFO
```

### Comparing `django_literature-0.1.0/LICENSE` & `django_literature-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.0/README.rst` & `django_literature-0.1.2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 .. image:: https://badge.fury.io/py/django-literature.svg
     :target: https://badge.fury.io/py/django-literature
 
 .. image:: https://travis-ci.org/SSJenny90/django-literature.svg?branch=master
     :target: https://travis-ci.org/SSJenny90/django-literature
 
-.. image:: https://codecov.io/gh/SSJenny90/django-literature/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/SSJenny90/django-literature
+.. image:: https://codecov.io/gh/SSJenny90/django-literature/branch/main/graph/badge.svg?token=0Q18CLIKZE 
+ :target: https://codecov.io/gh/SSJenny90/django-literature
 
 A scientific literature management app for Django
 
 Documentation
 -------------
 
 The full documentation is at https://django-literature.readthedocs.io.
```

### Comparing `django_literature-0.1.0/literature/conf.py` & `django_literature-0.1.2/literature/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,28 +4,20 @@
 
 __all__ = ("settings", "LiteratureConf")
 
 
 class LiteratureConf(AppConf):
     """Settings for Django Literature"""
 
-    MODELS = {}
-    """Point the application to the working models. Required when extending
-    the default models."""
-
-    DEFAULT_STYLE = "harvard"
-    """Default citation style. Must be included in the templates/crossref/styles
+    DEFAULT_CITATION_STYLE = "plain_text"
+    """Default citation style. Must be included in the templates/literautre/citation/
      folder."""
 
-    AUTHOR_TRUNCATE_AFTER = 2
-
     INACTIVE_AFTER = 5
 
-    HYPERLINK = True
-
     PDF_RENAMER = "literature.utils.simple_file_renamer"
 
     AUTOLABEL = "literature.utils.simple_autolabeler"
 
     ADAPTORS = [
         "literature.adaptors.crossref.Crossref",
         "literature.adaptors.datacite.Datacite",
```

### Comparing `django_literature-0.1.0/literature/fields.py` & `django_literature-0.1.2/literature/fields.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.0/literature/managers.py` & `django_literature-0.1.2/literature/managers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 from datetime import date
 
-from asgiref.sync import sync_to_async
 from dateutil.relativedelta import relativedelta
-
-# from .adaptors.base import AdaptorError, RemoteAdaptorError
-from django.db import IntegrityError, transaction
 from django.db.models import Count, Max, Q
 from django.db.models.query import QuerySet
 from django.utils.module_loading import import_string
-from django.utils.translation import gettext as _
 
 from literature.conf import settings
 
 from .exceptions import AdaptorError, RemoteAdaptorError
 
 
 class AuthorQuerySet(QuerySet):
@@ -41,23 +36,21 @@
         )
 
     def as_lead(self):
         """Convenience filter for retrieving only authors that
         are listed as the lead author on a publication."""
 
         return (
-            self.prefetch_related("works")
+            self.prefetch_related("literature")
             .annotate(as_lead=Count("position", filter=Q(position__position=1)))
             .filter(as_lead__gt=0)
         )
 
     def with_last_published(self):
-        return self.prefetch_related("works").annotate(
-            last_published=Max("works__published")
-        )
+        return self.prefetch_related("literature").annotate(last_published=Max("literature__published"))
 
     def is_active(self):
         cutoff = date.today() - relativedelta(years=settings.LITERATURE_INACTIVE_AFTER)
         return self.with_last_published().filter(last_published__gt=cutoff)
 
 
 AuthorManager = AuthorQuerySet.as_manager
@@ -73,20 +66,15 @@
         Args:
             doi (_type_): _description_
             adaptor (_type_, optional): _description_. Defaults to None.
 
         Returns:
             _type_: _description_
         """
-        if adaptor:
-            adaptors = [adaptor]
-        else:
-            adaptors = [
-                import_string(ac) for ac in getattr(settings, "LITERATURE_ADAPTORS")
-            ]
+        adaptors = [adaptor] if adaptor else [import_string(ac) for ac in settings.LITERATURE_ADAPTORS]
 
         for adaptor in adaptors:
             try:
                 return adaptor(doi=doi).get_data()
             except AdaptorError:
                 # raised if the adaptor is not remote
                 pass
@@ -99,27 +87,27 @@
 
         Args:
             doi (_type_): _description_
         """
         try:
             return self.get(doi=doi), False
         except self.model.DoesNotExist:
-            for adaptor_class in getattr(settings, "LITERATURE_ADAPTORS"):
+            for adaptor_class in settings.LITERATURE_ADAPTORS:
                 if adaptor_class.is_remote:
                     obj, created = self.resolve_doi_for_adaptor(doi, adaptor_class)
 
     # def _resolve_doi(self, doi, adaptor):
     #     """
     #     For a given adaptor, attempt to resolve a doi by querying the remote data source.
     #     """
     #     # if not adaptor.is_remote:
     #     # raise AdaptorError(_(f"{adaptor} cannot resolve remote sources."))
 
     #     # initialize the adaptor with the given doi in an attempt to
     #     # fetch data from the adaptor's API
     #     return adaptor(doi=doi).get_data()
 
-    async def aresolve_doi_for_adaptor(self, doi):
-        return await sync_to_async(self.resolve_doi_for_adaptor)(doi)
+    # async def aresolve_doi_for_adaptor(self, doi):
+    #     return await sync_to_async(self.resolve_doi_for_adaptor)(doi)
 
 
 LiteratureManager = LiteratureQuerySet.as_manager
```

### Comparing `django_literature-0.1.0/literature/models.py` & `django_literature-0.1.2/literature/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 from datetime import date
 
 from django.core.validators import (
     FileExtensionValidator,
     MaxValueValidator,
-    MinValueValidator,
     RegexValidator,
 )
 from django.db import models
 from django.urls import reverse
 from django.utils.encoding import force_str
 from django.utils.translation import gettext as _
 from model_utils import FieldTracker
 from model_utils.models import TimeStampedModel
 from sortedm2m.fields import SortedManyToManyField
 from taggit.managers import TaggableManager
 
-from .choices import MonthChoices
+from .choices import IdentifierTypes, TypeChoices
 from .managers import AuthorManager, LiteratureManager
-from .utils import get_current_year, pdf_file_renamer
+from .utils import pdf_file_renamer
 
 
 class LiteratureAuthor(models.Model):
     """An intermediate table for the Work-Author m2m relationship.
     `SortedManyToManyField` automatically creates this table, however, there is no access via querysets. Defining here instead allows us to have access to the intermediate table in order to query author position.
     """
 
     literature = models.ForeignKey("literature.Literature", on_delete=models.CASCADE)
-    author = models.ForeignKey(
-        "literature.Author", related_name="position", on_delete=models.CASCADE
-    )
+    author = models.ForeignKey("literature.Author", related_name="position", on_delete=models.CASCADE)
     position = models.IntegerField()
 
     _sort_field_name = "position"
 
     def __str__(self):
         return str(self.position)
 
@@ -41,15 +38,15 @@
     objects = AuthorManager()
 
     given = models.CharField(_("given name"), max_length=255, blank=True, null=True)
     family = models.CharField(_("family name"), max_length=255, blank=True)
     ORCID = models.CharField(
         "ORCID",
         max_length=64,
-        validators=[RegexValidator("^(?:\d{4}-){3}\d{3}[\d,x]")],
+        validators=[RegexValidator("^(?:\\d{4}-){3}\\d{3}[\\d,x]")],
         blank=True,
         null=True,
     )
 
     # literature = SortedManyToManyField(
     #     to="literature.Literature",
     #     verbose_name=_("literature"),
@@ -90,188 +87,167 @@
         return f"{self.given[0]}. {self.family}"
 
     def family_g(self):
         """Returns "Smith, J." """
         return f"{self.family}, {self.given[0]}."
 
 
+class Identifier(TimeStampedModel):
+    ID = models.CharField(max_length=512, verbose_name=_("Permanent Identifier"), primary_key=True)
+    literature = models.ForeignKey("literature.Literature", verbose_name=_("literature"), on_delete=models.CASCADE)
+    type = models.IntegerField(choices=IdentifierTypes.choices)  # noqa: A003
+
+    class Meta:
+        verbose_name = _("ID")
+        verbose_name_plural = _("IDs")
+        # ordering = ["citation_key"]
+        default_related_name = "identifiers"
+        unique_together = ["ID", "literature"]
+
+    def __str__(self):
+        return f"{self.get_type_display()} <{self.ID}>"
+
+
 class Literature(TimeStampedModel):
     """Model for storing literature data"""
 
     objects = LiteratureManager()
 
+    # ARTICLE TYPE
+    type = models.CharField(_("type"), choices=TypeChoices.choices, max_length=255)  # noqa: A003
+
+    # THE FOLLOWING FIELDS ARE DEFINED HERE AS THEY MAY BENEFIT FROM INDEXING
     abstract = models.TextField(_("abstract"), blank=True, null=True)
-    authors = SortedManyToManyField(
-        to="literature.Author",
-        verbose_name=_("authors"),
-        related_name="literature",
-        through=LiteratureAuthor,
-        sort_value_field_name="number",
-        blank=True,
-    )
-    author_str = models.TextField(
-        _("authors"),
-        null=True,
-        blank=True,
-        help_text=_(
-            'List of authors in the format "LastName, GivenName" separated by semi-colons. E.g Smith, John; Klose, Sarah;'
-        ),
-    )
-    comment = models.TextField(
-        _("comment"),
-        help_text=_("General comments regarding the entry."),
-        blank=True,
-        null=True,
-    )
     container_title = models.CharField(
         _("container title"),
-        help_text=_("The journal, book or other container title of the entry."),
+        help_text=_(
+            "Title of the container holding the item (e.g. the book title for a book chapter, the journal title for a"
+            " journal article; the album title for a recording; the session title for multi-part presentation at a"
+            " conference)."
+        ),
         max_length=512,
         null=True,
         blank=True,
     )
-    collections = models.ManyToManyField(
-        to="literature.collection",
-        verbose_name=_("collection"),
-        help_text=_("Add the entry to a collection."),
-        blank=True,
-    )
-    doi = models.CharField(
-        max_length=255, verbose_name="DOI", blank=True, null=True, unique=True
-    )
-    institution = models.CharField(
-        _("institution"),
-        max_length=255,
-        help_text=_("Name of the institution."),
-        blank=True,
-        null=True,
-    )
-    issn = models.CharField(
-        "ISSN",
-        max_length=255,
-        null=True,
-        blank=True,
-    )
-    isbn = models.CharField(
-        "ISBN",
-        max_length=255,
-        null=True,
-        blank=True,
-    )
-    issue = models.IntegerField(_("issue number"), blank=True, null=True)
-    keywords = TaggableManager(
+    keyword = TaggableManager(
         verbose_name=_("key words"),
-        help_text=_("A list of comma-separated keywords."),
+        help_text=_("Keyword(s) or tag(s) attached to the item."),
         blank=True,
     )
-    label = models.CharField(
-        _("label"),
-        help_text=_(
-            "A human readable identifier. Whitespace and hyphens will be converted to underscores."
-        ),
+    citation_key = models.CharField(
+        _("citation key"),
+        help_text=_("A human readable identifier of the literature item (analogous to a BibTeX entrykey)."),
         max_length=255,
         blank=True,
-        # null=True,
+        null=True,
         unique=True,
     )
     language = models.CharField(_("language"), max_length=2, blank=True, null=True)
-    month = models.PositiveSmallIntegerField(
-        _("month"),
-        help_text=_("The month of publication."),
-        choices=MonthChoices.choices,
+    title = models.TextField(
+        _("title"),
+        help_text=_("Primary title of the item."),
         blank=True,
         null=True,
     )
-    pages = models.CharField(
-        _("pages"),
-        help_text=_(
-            "Either a single digit indicating the page number or two hyphen-separated digits representing a range."
-        ),
-        max_length=32,
-        validators=[RegexValidator("^(\d+-{1,2}?\d+)$")],
-        null=True,
+
+    # DJANGO LITERATURE SPECIFIC FIELDS
+    authors = SortedManyToManyField(
+        to="literature.Author",
+        verbose_name=_("authors"),
+        related_name="literature",
+        through=LiteratureAuthor,
+        sort_value_field_name="number",
+        blank=True,
+    )
+    collections = models.ManyToManyField(
+        to="literature.collection",
+        verbose_name=_("collection"),
+        help_text=_("Add the entry to a collection."),
         blank=True,
     )
     pdf = models.FileField(
         "PDF",
         upload_to=pdf_file_renamer,
         validators=[FileExtensionValidator(["pdf"])],
         null=True,
         blank=True,
     )
     published = models.DateField(
         _("date published"),
         max_length=255,
-        validators=[MaxValueValidator(date.today)],
-    )
-    publisher = models.CharField(
-        _("publisher"),
-        help_text=_("Name of the publisher."),
         blank=True,
         null=True,
-        max_length=255,
+        validators=[MaxValueValidator(date.today)],
     )
-    source = models.CharField(
-        _("source"),
-        help_text=_("The source of metadata for the entry."),
-        max_length=255,
-        default="Admin Upload",
+    comment = models.TextField(
+        _("comment"),
+        help_text=_("General comments regarding the entry."),
         blank=True,
-    )
-    title = models.CharField(
-        _("title"),
-        max_length=512,
-    )
-    type = models.CharField(_("entry type"), max_length=255)
-    url = models.URLField(
-        "URL", help_text=_("A link to the URL resource."), blank=True, null=True
-    )
-    volume = models.IntegerField(_("volume"), blank=True, null=True)
-    year = models.PositiveSmallIntegerField(
-        _("year"),
-        help_text=_("The year of publication."),
-        validators=[MinValueValidator(1900), MaxValueValidator(get_current_year)],
-    )
-
-    last_synced = models.DateTimeField(
-        _("last synced"),
-        help_text=_("Last time the entry was synced with an online resource."),
         null=True,
-        blank=True,
     )
 
+    # RAW CSL DATA FIELD
+    CSL = models.JSONField(_("Citation Style Language"), blank=True)
+
     # tracks whether changes have been made to any fields since the last save
     tracker = FieldTracker()
 
     class Meta:
         verbose_name = _("literature")
         verbose_name_plural = _("literature")
-        ordering = ["label"]
+        ordering = ["citation_key"]
         default_related_name = "literature"
 
     def __str__(self):
-        return force_str(self.label)
+        return force_str(self.citation_key)
 
     def save(self, *args, **kwargs):
-        # not implemented
-        if self.tracker.has_changed("doi"):
-            self.objects.resolve(self.doi, self.source)
-
-        if self.tracker.has_changed("year"):
-            self.published = date(year=self.year, month=self.month or 1, day=1)
-        return super().save(*args, **kwargs)
+        if self.tracker.has_changed("CSL"):
+            self.parse_csl()
+
+        # if self.tracker.has_changed("year"):
+        # self.published = date(year=self.year, month=self.month or 1, day=1)
+
+        super().save(*args, **kwargs)
+        # if self.tracker.has_changed("CSL"):
+        self.update_identifiers()
+        return self
+
+    def parse_csl(self):
+        CSL = {k.replace("-", "_"): v for k, v in self.CSL.items()}
+        for field in [f.name for f in self._meta.fields]:
+            if field == "id":
+                continue
+            if CSL.get(field):
+                setattr(self, field, CSL[field])
+
+    def update_identifiers(self):
+        # update identifier fields
+        for field in IdentifierTypes.labels:
+            if self.CSL.get(field):
+                obj, new = Identifier.objects.get_or_create(
+                    ID=self.CSL.get(field), type=getattr(IdentifierTypes, field), literature=self
+                )
+                if new:
+                    print(f"Creating new {field}")
+                    obj.save()
 
     @staticmethod
     def autocomplete_search_fields():
         return (
             "title__icontains",
             "authors__family__icontains",
-            "label__icontains",
+            "citation_key__icontains",
         )
 
+    # def to_internal_value(self, data):
+    # data['container_title'] = data['container-title']
+    # data.pop('container-title', None)
+    # return data
+
 
 class Collection(TimeStampedModel):
     """
     Model representing a collection of publications.
     """
 
     class Meta:
```

### Comparing `django_literature-0.1.0/PKG-INFO` & `django_literature-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 Metadata-Version: 2.1
 Name: django-literature
-Version: 0.1.0
+Version: 0.1.2
 Summary: A scientific literature management tool for Django
+Home-page: https://github.com/SSJenny90/django-literature
 License: MIT
+Keywords: django,literature,publications,scientific,research
 Author: Sam Jennings
 Author-email: samuel.scott.jennings@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: Django :: 3.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: django (>=3.2)
+Requires-Dist: django-appconf (>=1.0.5,<2.0.0)
+Requires-Dist: django-formset (>=0.13.4,<0.14.0)
 Requires-Dist: django-model-utils (>=4.3.1,<5.0.0)
 Requires-Dist: django-sortedm2m (>=3.1.1,<4.0.0)
 Requires-Dist: django-taggit (>=3.1.0,<4.0.0)
+Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
+Requires-Dist: drf-schema-adapter (>=3.0.6,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/x-rst
 
 =============================
 Django Literature
 =============================
 
 .. image:: https://badge.fury.io/py/django-literature.svg
     :target: https://badge.fury.io/py/django-literature
 
 .. image:: https://travis-ci.org/SSJenny90/django-literature.svg?branch=master
     :target: https://travis-ci.org/SSJenny90/django-literature
 
-.. image:: https://codecov.io/gh/SSJenny90/django-literature/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/SSJenny90/django-literature
+.. image:: https://codecov.io/gh/SSJenny90/django-literature/branch/main/graph/badge.svg?token=0Q18CLIKZE 
+ :target: https://codecov.io/gh/SSJenny90/django-literature
 
 A scientific literature management app for Django
 
 Documentation
 -------------
 
 The full documentation is at https://django-literature.readthedocs.io.
```

