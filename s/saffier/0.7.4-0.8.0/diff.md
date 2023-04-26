# Comparing `tmp/saffier-0.7.4.tar.gz` & `tmp/saffier-0.8.0.tar.gz`

## Comparing `saffier-0.7.4.tar` & `saffier-0.8.0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/__init__.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/exceptions.py
--rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/fields.py
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/metaclass.py
--rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/models.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/py.typed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/testclient.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/types.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/conf/enums.py
--rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/conf/functional.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/conf/global_settings.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/conf/module_import.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/__init__.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/base.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/datastructures.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/events.py
--rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/formats.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/registry.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/schemas.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/sync.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/unique.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/terminal/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/terminal/base.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/terminal/print.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/terminal/terminal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/connection.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/constants.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/datastructures.py
--rw-r--r--   0        0        0    15800 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/fields.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/manager.py
--rw-r--r--   0        0        0    23146 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/queryset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/query/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/query/protocols.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/__init__.py
--rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/base.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/cli.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/constants.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/decorators.py
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/env.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/branches.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/check.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/current.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/downgrade.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/edit.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/heads.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/history.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/init.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/list_templates.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/makemigrations.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/merge.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/migrate.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/revision.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/show.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/stamp.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/shell/__init__.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/shell/enums.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/shell/ipython.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/shell/ptpython.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/shell/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/templates/default/README
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/templates/default/alembic.ini.mako
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/templates/default/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/templates/default/script.py.mako
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/sqlalchemy/fields.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/sqlalchemy/protocols.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/sqlalchemy/types.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.7.4/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.7.4/LICENSE
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.7.4/README.md
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 saffier-0.7.4/pyproject.toml
--rw-r--r--   0        0        0    11190 2020-02-02 00:00:00.000000 saffier-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/__init__.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/exceptions.py
+-rw-r--r--   0        0        0    11401 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/fields.py
+-rw-r--r--   0        0        0    14214 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/metaclass.py
+-rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/models.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/py.typed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/testclient.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/types.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/conf/enums.py
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/conf/functional.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/conf/global_settings.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/conf/module_import.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/__init__.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/base.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/datastructures.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/events.py
+-rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/formats.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/registry.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/schemas.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/sync.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/unique.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/terminal/base.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/terminal/print.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/core/terminal/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/connection.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/constants.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/datastructures.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/fields.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/manager.py
+-rw-r--r--   0        0        0    26886 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/queryset.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/related.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/query/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/db/query/protocols.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/__init__.py
+-rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/base.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/cli.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/constants.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/decorators.py
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/env.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/branches.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/check.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/current.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/downgrade.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/edit.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/heads.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/history.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/init.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/list_templates.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/makemigrations.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/merge.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/migrate.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/revision.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/show.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/stamp.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/shell/__init__.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/shell/enums.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/operations/shell/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/templates/default/README
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/templates/default/alembic.ini.mako
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/templates/default/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/migrations/templates/default/script.py.mako
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/sqlalchemy/fields.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/sqlalchemy/protocols.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.8.0/saffier/sqlalchemy/types.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.8.0/README.md
+-rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 saffier-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    11190 2020-02-02 00:00:00.000000 saffier-0.8.0/PKG-INFO
```

### Comparing `saffier-0.7.4/saffier/__init__.py` & `saffier-0.8.0/saffier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.4"
+__version__ = "0.8.0"
 
 from saffier.conf import settings
 from saffier.conf.global_settings import SaffierSettings
 
 from .core.registry import Registry
 from .db.connection import Database
 from .db.constants import CASCADE, RESTRICT, SET_NULL
```

### Comparing `saffier-0.7.4/saffier/exceptions.py` & `saffier-0.8.0/saffier/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,9 +33,13 @@
     ...
 
 
 class ImproperlyConfigured(SaffierException):
     ...
 
 
+class ForeignKeyBadConfigured(SaffierException):
+    ...
+
+
 class CommandEnvironmentError(SaffierException):
     ...
```

### Comparing `saffier-0.7.4/saffier/fields.py` & `saffier-0.8.0/saffier/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 from datetime import date, datetime
 
 import sqlalchemy
 
-from saffier.db.constants import SET_NULL
+from saffier.db.constants import CASCADE, SET_NULL
 from saffier.db.fields import (
     URL,
     UUID,
     Any,
     Boolean,
     Date,
     DateTime,
@@ -42,14 +42,15 @@
         self.null = kwargs.get("null", False)
         self.primary_key = primary_key
         self.index = index
         self.unique = unique
         self.validator: typing.Union[SaffierField, typing.Type[SaffierField]] = self.get_validator(
             **kwargs
         )
+        self.owner = kwargs.pop("owner", None)
 
     def get_column(self, name: str) -> sqlalchemy.Column:
         """
         Returns a column type for the model field.
         """
         column_type = self.get_column_type()
         constraints = self.get_constraints()
@@ -232,23 +233,35 @@
     ForeignKey field object
     """
 
     class ForeignKeyValidator(SaffierField):
         def check(self, value: typing.Any) -> typing.Any:
             return value.pk
 
-    def __init__(self, to: typing.Any, null: bool = False, on_delete: typing.Optional[str] = None):
+    def __init__(
+        self,
+        to: typing.Any,
+        null: bool = False,
+        on_delete: typing.Optional[str] = None,
+        on_update: typing.Optional[str] = None,
+        related_name: typing.Optional[str] = None,
+    ):
         assert on_delete is not None, "on_delete must not be null."
 
         if on_delete == SET_NULL and not null:
             raise AssertionError("When SET_NULL is enabled, null must be True.")
 
+        if on_update and (on_update == SET_NULL and not null):
+            raise AssertionError("When SET_NULL is enabled, null must be True.")
+
         super().__init__(null=null)
         self.to = to
         self.on_delete = on_delete
+        self.on_update = on_update or CASCADE
+        self.related_name = related_name
 
     @property
     def target(self) -> typing.Any:
         if not hasattr(self, "_target"):
             if isinstance(self.to, str):
                 self._target = self.registry.models[self.to]  # type: ignore
             else:
@@ -261,15 +274,19 @@
     def get_column(self, name: str) -> sqlalchemy.Column:
         target = self.target
         to_field = target.fields[target.pkname]
 
         column_type = to_field.get_column_type()
         constraints = [
             sqlalchemy.schema.ForeignKey(
-                f"{target._meta.tablename}.{target.pkname}", ondelete=self.on_delete
+                f"{target._meta.tablename}.{target.pkname}",
+                ondelete=self.on_delete,
+                onupdate=self.on_update,
+                name=f"fk_{self.owner._meta.tablename}_{target._meta.tablename}"
+                f"_{target.pkname}_{name}",
             )
         ]
         return sqlalchemy.Column(name, column_type, *constraints, nullable=self.null)
 
     def expand_relationship(self, value: typing.Any) -> typing.Any:
         target = self.target
         if isinstance(value, target):
```

### Comparing `saffier-0.7.4/saffier/metaclass.py` & `saffier-0.8.0/saffier/metaclass.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 
 import sqlalchemy
 
 from saffier import fields as saffier_fields
 from saffier.core.registry import Registry
 from saffier.db.datastructures import Index, UniqueConstraint
 from saffier.db.manager import Manager
-from saffier.exceptions import ImproperlyConfigured
+from saffier.db.related import RelatedField
+from saffier.exceptions import ForeignKeyBadConfigured, ImproperlyConfigured
 from saffier.fields import BigIntegerField, Field
 from saffier.types import DictAny
 
 if TYPE_CHECKING:
-    from saffier.models import Model
+    from saffier.models import Model, ReflectModel
 
 
 class MetaInfo:
     __slots__ = (
         "abstract",
         "fields",
         "fields_mapping",
@@ -30,14 +31,15 @@
         "parents",
         "pk",
         "one_to_one_fields",
         "pk_attribute",
         "manager",
         "_model",
         "reflect",
+        "_managers",
     )
 
     def __init__(self, meta: typing.Optional["Model.Meta"] = None) -> None:
         self.abstract: bool = getattr(meta, "abstract", False)
         self.fields: typing.Set = set()
         self.fields_mapping: typing.Dict[str, Field] = {}
         self.registry: typing.Optional[typing.Type[Registry]] = getattr(meta, "registry", None)
@@ -48,14 +50,15 @@
         self.foreign_key_fields: typing.Set[str] = set()
         self.pk_attribute: typing.Union[Field, str] = getattr(meta, "pk_attribute", "")
         self._model: typing.Optional[typing.Type["Model"]] = None
         self.manager: Manager = getattr(meta, "manager", Manager())
         self.unique_together: typing.Any = getattr(meta, "unique_together", None)
         self.indexes: typing.Any = getattr(meta, "indexes", None)
         self.reflect: bool = getattr(meta, "reflect", False)
+        self._managers: bool = getattr(meta, "_managers", None)
 
 
 def _check_model_inherited_registry(
     bases: typing.Tuple[typing.Type, ...]
 ) -> typing.Type[Registry]:
     """
     When a registry is missing from the Meta class, it should look up for the bases
@@ -94,14 +97,48 @@
     else:
         if not meta.abstract:
             for key, value in inspect.getmembers(base):
                 if isinstance(value, Manager) and key not in attrs:
                     attrs[key] = value.__class__()
 
 
+def _set_related_name_for_foreign_keys(
+    foreign_keys: typing.Set[
+        typing.Union[saffier_fields.OneToOneField, saffier_fields.ForeignKey]
+    ],
+    model_class: typing.Union["Model", "ReflectModel"],
+) -> None:
+    """
+    Sets the related name for the foreign keys.
+    When a `related_name` is generated, creates a RelatedField from the table pointed
+    from the ForeignKey declaration and the the table declaring it.
+    """
+    for foreign_key in foreign_keys:
+        default_related_name = getattr(foreign_key, "related_name", None)
+
+        if not default_related_name:
+            default_related_name = f"{model_class.__name__.lower()}s_set"
+
+        elif hasattr(foreign_key.target, default_related_name):
+            raise ForeignKeyBadConfigured(
+                f"Multiple related_name with the same value '{default_related_name}' found to the same target. Related names must be different."
+            )
+
+        foreign_key.related_name = default_related_name
+
+        related_field = RelatedField(
+            related_name=default_related_name,
+            related_to=foreign_key.target,
+            related_from=model_class,
+        )
+
+        # Set the related name
+        setattr(foreign_key.target, default_related_name, related_field)
+
+
 class BaseModelMeta(type):
     __slots__ = ()
 
     def __new__(
         cls, name: str, bases: typing.Tuple[typing.Type, ...], attrs: DictAny
     ) -> typing.Any:
         fields: typing.Dict[str, Field] = {}
@@ -216,14 +253,16 @@
                 )
 
             if getattr(meta, "unique_together", None) is not None:
                 raise ImproperlyConfigured("unique_together cannot be in abstract classes.")
 
             if getattr(meta, "indexes", None) is not None:
                 raise ImproperlyConfigured("indexes cannot be in abstract classes.")
+        else:
+            meta._managers = [k for k, v in attrs.items() if isinstance(v, Manager)]
 
         # Handle the registry of models
         if getattr(meta, "registry", None) is None:
             if hasattr(new_class, "_db_model") and new_class._db_model:
                 meta.registry = _check_model_inherited_registry(bases)
             else:
                 return new_class
@@ -275,18 +314,27 @@
 
         new_class._db_model = True
         new_class.fields = meta.fields_mapping
 
         meta._model = new_class  # type: ignore
         meta.manager.model_class = new_class
 
+        # Sets the foreign key fields
+        if meta.foreign_key_fields:
+            _set_related_name_for_foreign_keys(meta.foreign_key_fields, new_class)
+
+        # Set the manager
         for _, value in attrs.items():
             if isinstance(value, Manager):
                 value.model_class = new_class
 
+        # Set the owner of the field
+        for _, value in new_class.fields.items():
+            value.owner = new_class
+
         return new_class
 
     @property
     def table(cls) -> typing.Any:
         """
         Making sure the tables on inheritance state, creates the new
         one properly.
```

### Comparing `saffier-0.7.4/saffier/models.py` & `saffier-0.8.0/saffier/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 
     def __init__(self, **kwargs: typing.Any) -> None:
         if "pk" in kwargs:
             kwargs[self.pkname] = kwargs.pop("pk")
 
         for k, v in kwargs.items():
             if k not in self.fields:
-                raise ValueError(f"Invalid keyword {k} for class {self.__class__.__name__}")
+                if not hasattr(self, k):
+                    raise ValueError(f"Invalid keyword {k} for class {self.__class__.__name__}")
             setattr(self, k, v)
 
     class Meta:
         """
         The `Meta` class used to configure each metadata of the model.
         Abstract classes are not generated in the database, instead, they are simply used as
         a reference for field generation.
@@ -177,18 +178,25 @@
         if not select_related:
             select_related = []
 
         # Instantiate any child instances first.
         for related in select_related:
             if "__" in related:
                 first_part, remainder = related.split("__", 1)
-                model_cls = cls.fields[first_part].target
+                try:
+                    model_cls = cls.fields[first_part].target
+                except KeyError:
+                    model_cls = getattr(cls, first_part).related_from
+
                 item[first_part] = model_cls._from_row(row, select_related=[remainder])
             else:
-                model_cls = cls.fields[related].target
+                try:
+                    model_cls = cls.fields[related].target
+                except KeyError:
+                    model_cls = getattr(cls, related).related_from
                 item[related] = model_cls._from_row(row)
 
         # Pull out the regular column values.
         for column in cls.table.columns:
             # Making sure when a table is reflected, maps the right fields of the ReflectModel
             if column.name not in cls.fields.keys():
                 continue
```

### Comparing `saffier-0.7.4/saffier/conf/__init__.py` & `saffier-0.8.0/saffier/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/conf/functional.py` & `saffier-0.8.0/saffier/conf/functional.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/conf/global_settings.py` & `saffier-0.8.0/saffier/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/conf/module_import.py` & `saffier-0.8.0/saffier/conf/module_import.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/core/base.py` & `saffier-0.8.0/saffier/core/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/core/datastructures.py` & `saffier-0.8.0/saffier/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/core/events.py` & `saffier-0.8.0/saffier/core/events.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/core/formats.py` & `saffier-0.8.0/saffier/core/formats.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/core/registry.py` & `saffier-0.8.0/saffier/core/registry.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/core/schemas.py` & `saffier-0.8.0/saffier/core/schemas.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/core/sync.py` & `saffier-0.8.0/saffier/core/sync.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/core/unique.py` & `saffier-0.8.0/saffier/core/unique.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/core/utils.py` & `saffier-0.8.0/saffier/core/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/core/terminal/base.py` & `saffier-0.8.0/saffier/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/core/terminal/print.py` & `saffier-0.8.0/saffier/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/core/terminal/terminal.py` & `saffier-0.8.0/saffier/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/db/datastructures.py` & `saffier-0.8.0/saffier/db/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/db/fields.py` & `saffier-0.8.0/saffier/db/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     ) -> None:
         super().__init__(**kwargs)
         if null and default is NO_DEFAULT:
             default = None
 
         if default is not NO_DEFAULT:
             self.default = default
+
         self.null = null
         self.read_only = read_only
         self.title = title
         self.description = description
         self.help_text = help_text
 
     def check(self, value: typing.Any) -> typing.Any:
```

### Comparing `saffier-0.7.4/saffier/db/manager.py` & `saffier-0.8.0/saffier/db/manager.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/db/queryset.py` & `saffier-0.8.0/saffier/db/queryset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import copy
 import typing
 
 import sqlalchemy
 
+import saffier
 from saffier.core.schemas import Schema
 from saffier.core.utils import ModelUtil
-from saffier.db.constants import FILTER_OPERATORS
+from saffier.db.constants import DEFAULT_RELATED_LOOKUP_FIELD, FILTER_OPERATORS
 from saffier.db.query.protocols import AwaitableQuery
 from saffier.exceptions import DoesNotFound, MultipleObjectsReturned
 from saffier.fields import CharField, TextField
 
 if typing.TYPE_CHECKING:  # pragma: no cover
-    from saffier.models import Model
+    from saffier.models import Model, ReflectModel
 
 
 SaffierModel = typing.TypeVar("SaffierModel", bound="Model")
+ReflectSaffierModel = typing.TypeVar("ReflectSaffierModel", bound="ReflectModel")
+
+SaffierModels = typing.Union[SaffierModel, ReflectSaffierModel]
 
 
 class QuerySetProps:
     """
     Properties used by the Queryset are placed in isolation
     for clean access and maintainance.
     """
@@ -37,15 +41,15 @@
         return Schema(fields=fields)
 
     @property
     def pkname(self) -> typing.Any:
         return self.model_class.pkname  # type: ignore
 
 
-class BaseQuerySet(QuerySetProps, ModelUtil, AwaitableQuery[SaffierModel]):
+class BaseQuerySet(QuerySetProps, ModelUtil, AwaitableQuery[SaffierModels]):
     ESCAPE_CHARACTERS = ["%", "_"]
 
     def __init__(
         self,
         model_class: typing.Any = None,
         filter_clauses: typing.Any = None,
         select_related: typing.Any = None,
@@ -98,29 +102,92 @@
         self, distinct_on: typing.Any, expression: typing.Any
     ) -> typing.Any:
         """Filters selects only specific fields"""
         distinct_on = list(map(self._prepare_fields_for_distinct, distinct_on))
         expression = expression.distinct(*distinct_on)
         return expression
 
+    def is_multiple_foreign_key(
+        self, model_class: typing.Union[typing.Type["Model"], typing.Type["ReflectModel"]]
+    ) -> typing.Tuple[bool, typing.List[typing.Tuple[str, str, str]]]:
+        """
+        Checks if the table has multiple foreign keys to the same table.
+        Iterates through all fields of type ForeignKey and OneToOneField and checks if there are
+        multiple FKs to the same destination table.
+
+        Returns a tuple of bool, list of tuples
+        """
+        fields = model_class.fields
+        foreign_keys = []
+        has_many = False
+
+        counter = 0
+
+        for key, value in fields.items():
+            tablename = None
+
+            if counter > 1:
+                has_many = True
+
+            if isinstance(value, (saffier.ForeignKey, saffier.OneToOneField)):
+                tablename = value.to if isinstance(value.to, str) else value.to.__name__
+
+                if tablename not in foreign_keys:
+                    foreign_keys.append((key, tablename, value.related_name))
+                    counter += 1
+                else:
+                    counter += 1
+
+        return has_many, foreign_keys
+
     def _build_tables_select_from_relationship(self) -> typing.Any:
         """
-        Builds the tables relationships
+        Builds the tables relationships and joins.
+        When a table contains more than one foreign key pointing to the same
+        destination table, a lookup for the related field is made to understand
+        from which foreign key the table is looked up from.
         """
         tables = [self.table]
         select_from = self.table
+        has_many_fk_same_table = False
 
         for item in self._select_related:
             model_class = self.model_class
             select_from = self.table
 
             for part in item.split("__"):
-                model_class = model_class.fields[part].target
+                try:
+                    model_class = model_class.fields[part].target
+                except KeyError:
+                    # Check related fields
+                    model_class = getattr(model_class, part).related_from
+                    has_many_fk_same_table, keys = self.is_multiple_foreign_key(model_class)
+
                 table = model_class.table
-                select_from = sqlalchemy.sql.join(select_from, table)
+
+                # If there is multiple FKs to the same table
+                if not has_many_fk_same_table:
+                    select_from = sqlalchemy.sql.join(select_from, table)
+                else:
+                    lookup_field = None
+
+                    # Extract the table field from the related
+                    # Assign to a lookup_field
+                    for values in keys:
+                        field, _, related_name = values
+                        if related_name == part:
+                            lookup_field = field
+                            break
+
+                    select_from = sqlalchemy.sql.join(
+                        select_from,
+                        table,
+                        select_from.c.id == getattr(table.c, lookup_field),
+                    )
+
                 tables.append(table)
 
         return tables, select_from
 
     def _build_select(self) -> typing.Any:
         """
         Builds the query select based on the given parameters and filters.
@@ -184,21 +251,34 @@
                     related_str = "__".join(related_parts)
                     if related_str not in select_related:
                         select_related.append(related_str)
 
                     # Walk the relationships to the actual model class
                     # against which the comparison is being made.
                     for part in related_parts:
-                        model_class = model_class.fields[part].target
+                        try:
+                            model_class = model_class.fields[part].target
+                        except KeyError:
+                            model_class = getattr(model_class, part).related_from
 
                 column = model_class.table.columns[field_name]
 
             else:
                 op = "exact"
-                column = self.table.columns[key]
+                try:
+                    column = self.table.columns[key]
+                except KeyError as error:
+                    # Check for related fields
+                    # if an Attribute error is raised, we need to make sure
+                    # It raises the KeyError from the previous check
+                    try:
+                        model_class = getattr(self.model_class, key).related_to
+                        column = model_class.table.columns[DEFAULT_RELATED_LOOKUP_FIELD]
+                    except AttributeError:
+                        raise KeyError(str(error)) from error
 
             # Map the operation code onto SQLAlchemy's ColumnElement
             # https://docs.sqlalchemy.org/en/latest/core/sqlelement.html#sqlalchemy.sql.expression.ColumnElement
             op_attr = FILTER_OPERATORS[op]
             has_escaped_character = False
 
             if op in ["contains", "icontains"]:
@@ -290,15 +370,15 @@
     def sql(self) -> str:
         return str(self._expression)
 
     @sql.setter
     def sql(self, value: typing.Any) -> None:
         self._expression = value
 
-    async def __aiter__(self) -> typing.AsyncIterator[SaffierModel]:
+    async def __aiter__(self) -> typing.AsyncIterator[SaffierModels]:
         for value in await self:  # type: ignore
             yield value
 
     def _set_query_expression(self, expression: typing.Any) -> None:
         """
         Sets the value of the sql property to the expression used.
         """
@@ -540,15 +620,17 @@
         """
         new_objs = [self._validate_kwargs(**obj) for obj in objs]
 
         expression = self.table.insert().values(new_objs)
         self._set_query_expression(expression)
         await self.database.execute(expression)
 
-    async def bulk_update(self, objs: typing.List[SaffierModel], fields: typing.List[str]) -> None:
+    async def bulk_update(
+        self, objs: typing.List[SaffierModels], fields: typing.List[str]
+    ) -> None:
         """
         Bulk updates records in a table.
 
         A similar solution was suggested here: https://github.com/encode/orm/pull/148
 
         It is thought to be a clean approach to a simple problem so it was added here and
         refactored to be compatible with Saffier.
@@ -637,20 +719,28 @@
             await instance.update(**defaults)
             return instance, False
         except DoesNotFound:
             kwargs.update(defaults)
             instance = await self.create(**kwargs)
             return instance, True
 
+    async def contains(self, instance: SaffierModels) -> SaffierModels:
+        """Returns true if the QuerySet contains the provided object.
+        False if otherwise.
+        """
+        if getattr(instance, "pk", None) is None:
+            raise ValueError("'obj' must be a model or reflect model instance.")
+        return await self.filter(pk=instance.pk).exists()
+
     async def _execute(self) -> typing.Any:
         return await self.all()
 
     def __await__(
         self,
-    ) -> typing.Generator[typing.Any, None, typing.List[SaffierModel]]:
+    ) -> typing.Generator[typing.Any, None, typing.List[SaffierModels]]:
         return self._execute().__await__()
 
     def __class_getitem__(cls, *args: typing.Any, **kwargs: typing.Any) -> typing.Any:
         return cls
 
     def __deepcopy__(self, memo: typing.Any) -> typing.Any:
         """Don't populate the QuerySet's cache."""
```

### Comparing `saffier-0.7.4/saffier/db/query/protocols.py` & `saffier-0.8.0/saffier/db/query/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/base.py` & `saffier-0.8.0/saffier/migrations/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/cli.py` & `saffier-0.8.0/saffier/migrations/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             cmd.callback = self.wrap_args(cmd.callback)
         return super().add_command(cmd, name)
 
     def wrap_args(self, func: typing.Any) -> typing.Any:
         params = inspect.signature(func).parameters
 
         @wraps(func)
-        def wrapped(ctx: click.Context, /, *args: typing, **kwargs: typing) -> typing:
+        def wrapped(ctx: click.Context, /, *args: typing.Any, **kwargs: typing.Any) -> typing.Any:
             scaffold = ctx.ensure_object(MigrationEnv)
             if "env" in params:
                 kwargs["env"] = scaffold
             return func(*args, **kwargs)
 
         return click.pass_context(wrapped)
```

### Comparing `saffier-0.7.4/saffier/migrations/env.py` & `saffier-0.8.0/saffier/migrations/env.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/__init__.py` & `saffier-0.8.0/saffier/migrations/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/branches.py` & `saffier-0.8.0/saffier/migrations/operations/branches.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/current.py` & `saffier-0.8.0/saffier/migrations/operations/current.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/downgrade.py` & `saffier-0.8.0/saffier/migrations/operations/downgrade.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/heads.py` & `saffier-0.8.0/saffier/migrations/operations/heads.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/history.py` & `saffier-0.8.0/saffier/migrations/operations/history.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/init.py` & `saffier-0.8.0/saffier/migrations/operations/init.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/makemigrations.py` & `saffier-0.8.0/saffier/migrations/operations/makemigrations.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/merge.py` & `saffier-0.8.0/saffier/migrations/operations/merge.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/migrate.py` & `saffier-0.8.0/saffier/migrations/operations/migrate.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/revision.py` & `saffier-0.8.0/saffier/migrations/operations/revision.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/stamp.py` & `saffier-0.8.0/saffier/migrations/operations/stamp.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/shell/base.py` & `saffier-0.8.0/saffier/migrations/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/shell/ipython.py` & `saffier-0.8.0/saffier/migrations/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/shell/ptpython.py` & `saffier-0.8.0/saffier/migrations/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/operations/shell/utils.py` & `saffier-0.8.0/saffier/migrations/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/templates/default/alembic.ini.mako` & `saffier-0.8.0/saffier/migrations/templates/default/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/migrations/templates/default/env.py` & `saffier-0.8.0/saffier/migrations/templates/default/env.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/sqlalchemy/fields.py` & `saffier-0.8.0/saffier/sqlalchemy/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/saffier/sqlalchemy/protocols.py` & `saffier-0.8.0/saffier/sqlalchemy/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/LICENSE` & `saffier-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/README.md` & `saffier-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `saffier-0.7.4/pyproject.toml` & `saffier-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "alembic>=1.9.3,<2.0.0",
     "anyio>=3.6.2,<4",
     "click>=8.1.3,<9.0.0",
     "loguru>=0.6.0,<0.7.0",
-    "databasez>=0.2.0",
+    "databasez>=0.2.2",
     "orjson >=3.8.5,<4.0.0",
     "pydantic>=1.10.5,<2.0.0",
     "rich>=13.3.1,<14.0.0",
 ]
 keywords = [
     "api",
     "rest",
@@ -158,14 +158,16 @@
 ]
 ignore = [
     "E501", # line too long, handled by black
     "B008", # do not perform function calls in argument defaults
     "C901", # too complex
 ]
 
+exclude = ["docs_src/*"]
+
 [[tool.mypy.overrides]]
 module = "saffier.tests.*"
 ignore_missing_imports = true
 check_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = ["sqlalchemy.*", "asyncpg", "alembic", "sqlalchemy_utils.*"]
```

### Comparing `saffier-0.7.4/PKG-INFO` & `saffier-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saffier
-Version: 0.7.4
+Version: 0.8.0
 Summary: The only python ORM you will ever need.
 Project-URL: Homepage, https://github.com/tarsil/saffier
 Project-URL: Documentation, https://saffier.tarsild.io/
 Project-URL: Changelog, https://saffier.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/saffier
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -35,15 +35,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: alembic<2.0.0,>=1.9.3
 Requires-Dist: anyio<4,>=3.6.2
 Requires-Dist: click<9.0.0,>=8.1.3
-Requires-Dist: databasez>=0.2.0
+Requires-Dist: databasez>=0.2.2
 Requires-Dist: loguru<0.7.0,>=0.6.0
 Requires-Dist: orjson<4.0.0,>=3.8.5
 Requires-Dist: pydantic<2.0.0,>=1.10.5
 Requires-Dist: rich<14.0.0,>=13.3.1
 Provides-Extra: all
 Requires-Dist: databasez[mysql,postgresql,sqlite]; extra == 'all'
 Requires-Dist: ipython<9.0.0,>=8.10.0; extra == 'all'
```

