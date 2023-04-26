# Comparing `tmp/linkml-1.5.0rc2.tar.gz` & `tmp/linkml-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml-1.5.0rc2.tar", max compression
+gzip compressed data, was "linkml-1.5.1.tar", max compression
```

## Comparing `linkml-1.5.0rc2.tar` & `linkml-1.5.1.tar`

### file list

```diff
@@ -1,107 +1,108 @@
--rw-r--r--   0        0        0     6555 2023-03-23 02:29:22.353478 linkml-1.5.0rc2/LICENSE
--rw-r--r--   0        0        0     1369 2023-03-23 02:29:22.353478 linkml-1.5.0rc2/README.md
--rw-r--r--   0        0        0     3227 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/__init__.py
--rw-r--r--   0        0        0      326 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/_version.py
--rw-r--r--   0        0        0    51005 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/PythonGenNotes.md
--rw-r--r--   0        0        0     3926 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/README.md
--rw-r--r--   0        0        0      616 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/common/__init__.py
--rw-r--r--   0        0        0     2040 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/common/type_designators.py
--rw-r--r--   0        0        0     3118 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/csvgen.py
--rw-r--r--   0        0        0     2721 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/docgen/class.md.jinja2
--rw-r--r--   0        0        0     2678 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/docgen/class_diagram.md.jinja2
--rw-r--r--   0        0        0     1321 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/docgen/common_metadata.md.jinja2
--rw-r--r--   0        0        0      866 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/docgen/enum.md.jinja2
--rw-r--r--   0        0        0     1190 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/docgen/index.md.jinja2
--rw-r--r--   0        0        0      501 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/docgen/index.tex.jinja2
--rw-r--r--   0        0        0       70 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/docgen/schema.md.jinja2
--rw-r--r--   0        0        0     2159 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/docgen/slot.md.jinja2
--rw-r--r--   0        0        0     1552 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/docgen/subset.md.jinja2
--rw-r--r--   0        0        0      483 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/docgen/type.md.jinja2
--rw-r--r--   0        0        0    32653 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/docgen.py
--rw-r--r--   0        0        0     5112 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/dotgen.py
--rw-r--r--   0        0        0    10863 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/erdiagramgen.py
--rw-r--r--   0        0        0     6727 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/excelgen.py
--rw-r--r--   0        0        0     3575 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/golrgen.py
--rw-r--r--   0        0        0     2347 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/graphqlgen.py
--rw-r--r--   0        0        0      444 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/javagen/example_template.java.jinja2
--rw-r--r--   0        0        0     1737 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/javagen/java_record_template.jinja2
--rw-r--r--   0        0        0     5499 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/javagen.py
--rw-r--r--   0        0        0     8821 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/jsonldcontextgen.py
--rw-r--r--   0        0        0     7952 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/jsonldgen.py
--rw-r--r--   0        0        0    19361 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/jsonschemagen.py
--rw-r--r--   0        0        0     3555 2023-03-23 02:29:22.373478 linkml-1.5.0rc2/linkml/generators/linkmlgen.py
--rw-r--r--   0        0        0    34422 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/markdowngen.py
--rw-r--r--   0        0        0     6532 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/namespacegen.py
--rw-r--r--   0        0        0     6695 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/oocodegen.py
--rw-r--r--   0        0        0    27365 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/owlgen.py
--rw-r--r--   0        0        0     4911 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/prefixmapgen.py
--rw-r--r--   0        0        0     9811 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/projectgen.py
--rw-r--r--   0        0        0     2443 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/protogen.py
--rw-r--r--   0        0        0    20322 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/pydanticgen.py
--rw-r--r--   0        0        0    48142 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/pythongen.py
--rw-r--r--   0        0        0     2825 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/rdfgen.py
--rw-r--r--   0        0        0     5621 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/shaclgen.py
--rw-r--r--   0        0        0     9547 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/shexgen.py
--rw-r--r--   0        0        0     6632 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/sparqlgen.py
--rw-r--r--   0        0        0      166 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2575 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
--rw-r--r--   0        0        0     1625 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
--rw-r--r--   0        0        0     9334 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/sqlalchemygen.py
--rw-r--r--   0        0        0    18626 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/sqlddlgen.py
--rw-r--r--   0        0        0    11387 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/sqltablegen.py
--rw-r--r--   0        0        0     7177 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/sssomgen.py
--rw-r--r--   0        0        0     1788 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/string_template.md
--rw-r--r--   0        0        0     3020 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/summarygen.py
--rw-r--r--   0        0        0     4760 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/terminusdbgen.py
--rw-r--r--   0        0        0     5555 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/typescriptgen.py
--rw-r--r--   0        0        0     1746 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/yamlgen.py
--rw-r--r--   0        0        0    13311 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/generators/yumlgen.py
--rw-r--r--   0        0        0        0 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/__init__.py
--rw-r--r--   0        0        0     3868 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/cli.py
--rw-r--r--   0        0        0      292 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/config/datamodel/.linkmllint.yaml
--rw-r--r--   0        0        0        0 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/config/datamodel/__init__.py
--rw-r--r--   0        0        0    17711 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/config/datamodel/config.py
--rw-r--r--   0        0        0     6980 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/config/datamodel/config.yaml
--rw-r--r--   0        0        0      540 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/config/default.yaml
--rw-r--r--   0        0        0      198 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/config/recommended.yaml
--rw-r--r--   0        0        0      269 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/formatters/__init__.py
--rw-r--r--   0        0        0      518 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/formatters/formatter.py
--rw-r--r--   0        0        0      767 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/formatters/json_formatter.py
--rw-r--r--   0        0        0     2605 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/formatters/markdown_formatter.py
--rw-r--r--   0        0        0     1990 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/formatters/terminal_formatter.py
--rw-r--r--   0        0        0      871 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/formatters/tsv_formatter.py
--rw-r--r--   0        0        0     3230 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/linter.py
--rw-r--r--   0        0        0    11658 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/linter/rules.py
--rw-r--r--   0        0        0       55 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/reporting/__init__.py
--rw-r--r--   0        0        0     9189 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/reporting/model.py
--rw-r--r--   0        0        0        0 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/transformers/__init__.py
--rw-r--r--   0        0        0    18594 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/transformers/relmodel_transformer.py
--rw-r--r--   0        0        0     5455 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/transformers/schema_renamer.py
--rw-r--r--   0        0        0        0 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/__init__.py
--rw-r--r--   0        0        0     6463 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/converter.py
--rw-r--r--   0        0        0     4384 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/datautils.py
--rw-r--r--   0        0        0      399 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/datavalidator.py
--rw-r--r--   0        0        0     6999 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/execute_tutorial.py
--rw-r--r--   0        0        0    39740 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/generator.py
--rw-r--r--   0        0        0      445 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/helpers.py
--rw-r--r--   0        0        0     5773 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/ifabsent_functions.py
--rw-r--r--   0        0        0     9498 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/mergeutils.py
--rw-r--r--   0        0        0     4560 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/rawloader.py
--rw-r--r--   0        0        0     9065 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/schema_builder.py
--rw-r--r--   0        0        0    13464 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/schema_fixer.py
--rw-r--r--   0        0        0    48537 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/schemaloader.py
--rw-r--r--   0        0        0    19733 2023-03-23 02:29:22.377478 linkml-1.5.0rc2/linkml/utils/schemasynopsis.py
--rw-r--r--   0        0        0    16297 2023-03-23 02:29:22.381478 linkml-1.5.0rc2/linkml/utils/sqlutils.py
--rw-r--r--   0        0        0     2395 2023-03-23 02:29:22.381478 linkml-1.5.0rc2/linkml/utils/typereferences.py
--rw-r--r--   0        0        0     1514 2023-03-23 02:29:22.381478 linkml-1.5.0rc2/linkml/utils/validation.py
--rw-r--r--   0        0        0      140 2023-03-23 02:29:22.381478 linkml-1.5.0rc2/linkml/validators/__init__.py
--rw-r--r--   0        0        0     5484 2023-03-23 02:29:22.381478 linkml-1.5.0rc2/linkml/validators/jsonschemavalidator.py
--rw-r--r--   0        0        0     4873 2023-03-23 02:29:22.381478 linkml-1.5.0rc2/linkml/validators/sparqlvalidator.py
--rw-r--r--   0        0        0        0 2023-03-23 02:29:22.381478 linkml-1.5.0rc2/linkml/workspaces/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 02:29:22.381478 linkml-1.5.0rc2/linkml/workspaces/datamodel/__init__.py
--rw-r--r--   0        0        0    15641 2023-03-23 02:29:22.381478 linkml-1.5.0rc2/linkml/workspaces/datamodel/workspaces.py
--rw-r--r--   0        0        0     4233 2023-03-23 02:29:22.381478 linkml-1.5.0rc2/linkml/workspaces/datamodel/workspaces.yaml
--rw-r--r--   0        0        0    11759 2023-03-23 02:29:22.381478 linkml-1.5.0rc2/linkml/workspaces/example_runner.py
--rw-r--r--   0        0        0     4872 2023-03-23 02:29:42.349410 linkml-1.5.0rc2/pyproject.toml
--rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 linkml-1.5.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     6555 2023-04-25 21:29:56.109279 linkml-1.5.1/LICENSE
+-rw-r--r--   0        0        0     1369 2023-04-25 21:29:56.109279 linkml-1.5.1/README.md
+-rw-r--r--   0        0        0     3227 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/__init__.py
+-rw-r--r--   0        0        0      326 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/_version.py
+-rw-r--r--   0        0        0    51005 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/PythonGenNotes.md
+-rw-r--r--   0        0        0     3926 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/README.md
+-rw-r--r--   0        0        0      616 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/common/__init__.py
+-rw-r--r--   0        0        0     2040 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/common/type_designators.py
+-rw-r--r--   0        0        0     3118 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/csvgen.py
+-rw-r--r--   0        0        0     2873 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/class.md.jinja2
+-rw-r--r--   0        0        0     2682 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/class_diagram.md.jinja2
+-rw-r--r--   0        0        0     1321 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/common_metadata.md.jinja2
+-rw-r--r--   0        0        0     1018 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/enum.md.jinja2
+-rw-r--r--   0        0        0     1190 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/index.md.jinja2
+-rw-r--r--   0        0        0      501 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/index.tex.jinja2
+-rw-r--r--   0        0        0       70 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/schema.md.jinja2
+-rw-r--r--   0        0        0     2557 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/slot.md.jinja2
+-rw-r--r--   0        0        0     1704 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/subset.md.jinja2
+-rw-r--r--   0        0        0      635 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/type.md.jinja2
+-rw-r--r--   0        0        0    32663 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen.py
+-rw-r--r--   0        0        0     5112 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/dotgen.py
+-rw-r--r--   0        0        0    10863 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/erdiagramgen.py
+-rw-r--r--   0        0        0     6894 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/excelgen.py
+-rw-r--r--   0        0        0     3575 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/golrgen.py
+-rw-r--r--   0        0        0     2347 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/graphqlgen.py
+-rw-r--r--   0        0        0      444 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/javagen/example_template.java.jinja2
+-rw-r--r--   0        0        0     1737 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/javagen/java_record_template.jinja2
+-rw-r--r--   0        0        0     5499 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/javagen.py
+-rw-r--r--   0        0        0     8821 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/jsonldcontextgen.py
+-rw-r--r--   0        0        0     7952 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/jsonldgen.py
+-rw-r--r--   0        0        0    19361 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/jsonschemagen.py
+-rw-r--r--   0        0        0     3555 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/linkmlgen.py
+-rw-r--r--   0        0        0    34422 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/markdowngen.py
+-rw-r--r--   0        0        0     6532 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/namespacegen.py
+-rw-r--r--   0        0        0     6695 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/oocodegen.py
+-rw-r--r--   0        0        0    27365 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/owlgen.py
+-rw-r--r--   0        0        0     4911 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/prefixmapgen.py
+-rw-r--r--   0        0        0     9811 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/projectgen.py
+-rw-r--r--   0        0        0     2443 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/protogen.py
+-rw-r--r--   0        0        0    20322 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/pydanticgen.py
+-rw-r--r--   0        0        0    49083 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/pythongen.py
+-rw-r--r--   0        0        0     2825 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/rdfgen.py
+-rw-r--r--   0        0        0     5621 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/shaclgen.py
+-rw-r--r--   0        0        0     9547 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/shexgen.py
+-rw-r--r--   0        0        0     6632 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sparqlgen.py
+-rw-r--r--   0        0        0      166 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2575 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
+-rw-r--r--   0        0        0     1625 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
+-rw-r--r--   0        0        0     9334 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sqlalchemygen.py
+-rw-r--r--   0        0        0    18626 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sqlddlgen.py
+-rw-r--r--   0        0        0    11387 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sqltablegen.py
+-rw-r--r--   0        0        0     7177 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sssomgen.py
+-rw-r--r--   0        0        0     1788 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/string_template.md
+-rw-r--r--   0        0        0     3020 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/summarygen.py
+-rw-r--r--   0        0        0     4760 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/terminusdbgen.py
+-rw-r--r--   0        0        0     5555 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/typescriptgen.py
+-rw-r--r--   0        0        0     1746 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/yamlgen.py
+-rw-r--r--   0        0        0    13311 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/yumlgen.py
+-rw-r--r--   0        0        0        0 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/__init__.py
+-rw-r--r--   0        0        0     3868 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/cli.py
+-rw-r--r--   0        0        0      292 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/config/datamodel/.linkmllint.yaml
+-rw-r--r--   0        0        0        0 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/config/datamodel/__init__.py
+-rw-r--r--   0        0        0    17711 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/config/datamodel/config.py
+-rw-r--r--   0        0        0     6980 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/config/datamodel/config.yaml
+-rw-r--r--   0        0        0      540 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/config/default.yaml
+-rw-r--r--   0        0        0      198 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/config/recommended.yaml
+-rw-r--r--   0        0        0      269 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/formatters/__init__.py
+-rw-r--r--   0        0        0      518 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/formatters/formatter.py
+-rw-r--r--   0        0        0      767 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/formatters/json_formatter.py
+-rw-r--r--   0        0        0     2605 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/formatters/markdown_formatter.py
+-rw-r--r--   0        0        0     1990 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/formatters/terminal_formatter.py
+-rw-r--r--   0        0        0      871 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/formatters/tsv_formatter.py
+-rw-r--r--   0        0        0     3230 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/linter.py
+-rw-r--r--   0        0        0    11658 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/rules.py
+-rw-r--r--   0        0        0       55 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/reporting/__init__.py
+-rw-r--r--   0        0        0     9189 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/reporting/model.py
+-rw-r--r--   0        0        0        0 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/transformers/__init__.py
+-rw-r--r--   0        0        0    18594 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/transformers/relmodel_transformer.py
+-rw-r--r--   0        0        0     5455 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/transformers/schema_renamer.py
+-rw-r--r--   0        0        0        0 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/utils/__init__.py
+-rw-r--r--   0        0        0     6463 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/utils/converter.py
+-rw-r--r--   0        0        0     4384 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/utils/datautils.py
+-rw-r--r--   0        0        0      490 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/utils/datavalidator.py
+-rw-r--r--   0        0        0     6999 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/utils/execute_tutorial.py
+-rw-r--r--   0        0        0    39740 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/generator.py
+-rw-r--r--   0        0        0      445 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/helpers.py
+-rw-r--r--   0        0        0     5773 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/ifabsent_functions.py
+-rw-r--r--   0        0        0     9498 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/mergeutils.py
+-rw-r--r--   0        0        0     4560 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/rawloader.py
+-rw-r--r--   0        0        0     9065 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/schema_builder.py
+-rw-r--r--   0        0        0    13464 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/schema_fixer.py
+-rw-r--r--   0        0        0    48537 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/schemaloader.py
+-rw-r--r--   0        0        0    19733 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/schemasynopsis.py
+-rw-r--r--   0        0        0    16297 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/sqlutils.py
+-rw-r--r--   0        0        0     2395 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/typereferences.py
+-rw-r--r--   0        0        0     1514 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/validation.py
+-rw-r--r--   0        0        0      140 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/validators/__init__.py
+-rw-r--r--   0        0        0     6165 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/validators/jsonschemavalidator.py
+-rw-r--r--   0        0        0     4873 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/validators/sparqlvalidator.py
+-rw-r--r--   0        0        0        0 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/workspaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/workspaces/datamodel/__init__.py
+-rw-r--r--   0        0        0    15641 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/workspaces/datamodel/workspaces.py
+-rw-r--r--   0        0        0     4233 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/workspaces/datamodel/workspaces.yaml
+-rw-r--r--   0        0        0    11759 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/workspaces/example_runner.py
+-rw-r--r--   0        0        0     4868 2023-04-25 21:30:31.461436 linkml-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6564 1970-01-01 00:00:00.000000 linkml-1.5.1/setup.py
+-rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 linkml-1.5.1/PKG-INFO
```

### Comparing `linkml-1.5.0rc2/LICENSE` & `linkml-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/README.md` & `linkml-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/__init__.py` & `linkml-1.5.1/linkml/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/PythonGenNotes.md` & `linkml-1.5.1/linkml/generators/PythonGenNotes.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/README.md` & `linkml-1.5.1/linkml/generators/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/__init__.py` & `linkml-1.5.1/linkml/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/common/type_designators.py` & `linkml-1.5.1/linkml/generators/common/type_designators.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/csvgen.py` & `linkml-1.5.1/linkml/generators/csvgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/docgen/class.md.jinja2` & `linkml-1.5.1/linkml/generators/docgen/class.md.jinja2`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 
 {%- if header -%}
 {{header}}
 {%- endif -%}
 
 
 {% if element.description %}
-_{{ element.description }}_
+{% set element_description_lines = element.description.split('\n') %}
+{% for element_description_line in element_description_lines %}
+_{{ element_description_line }}_
+{% endfor %}
 {% endif %}
 
 {% if element.abstract %}
 * __NOTE__: this is an abstract class and should not be instantiated directly
 {% endif %}
 
 URI: {{ gen.uri_link(element) }}
```

### Comparing `linkml-1.5.0rc2/linkml/generators/docgen/class_diagram.md.jinja2` & `linkml-1.5.1/linkml/generators/docgen/class_diagram.md.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -14,52 +14,52 @@
       {% for s in schemaview.class_children(element.name)|sort(attribute='name') -%}
         {{ gen.name(element) }} <|-- {{ gen.name(schemaview.get_element(s)) }}
       {% endfor %}
       
       {% for s in schemaview.class_induced_slots(element.name)|sort(attribute='name') -%}
         {{ gen.name(element) }} : {{gen.name(s)}}
         {% if s.range not in gen.all_type_object_names() %}
-          {{ gen.name(element) }} ..> {{ s.range }} : {{ gen.name(s) }}
+          {{ gen.name(element) }} --|> {{ s.range }} : {{ gen.name(s) }}
         {% endif %}
       {% endfor %}
 ```
 {% elif schemaview.class_parents(element.name) %}
 ```{{ gen.mermaid_directive() }}
  classDiagram
     class {{ gen.name(element) }}
       {% for s in schemaview.class_parents(element.name)|sort(attribute='name') -%}
         {{ gen.name(schemaview.get_element(s)) }} <|-- {{ gen.name(element) }}
       {% endfor %}
       {% for s in schemaview.class_induced_slots(element.name)|sort(attribute='name') -%}
         {{ gen.name(element) }} : {{gen.name(s)}}
         {% if s.range not in gen.all_type_object_names() %}
-          {{ gen.name(element) }} ..> {{ s.range }} : {{ gen.name(s) }}
+          {{ gen.name(element) }} --|> {{ s.range }} : {{ gen.name(s) }}
         {% endif %}
       {% endfor %}
 ```
 {% elif schemaview.class_children(element.name)  %}
 ```{{ gen.mermaid_directive() }}
  classDiagram
     class {{ gen.name(element) }}
       {% for s in schemaview.class_children(element.name)|sort(attribute='name') -%}
         {{ gen.name(element) }} <|-- {{ gen.name(schemaview.get_element(s)) }}
       {% endfor %}
       {% for s in schemaview.class_induced_slots(element.name)|sort(attribute='name') -%}
         {{ gen.name(element) }} : {{gen.name(s)}}
         {% if s.range not in gen.all_type_object_names() %}
-          {{ gen.name(element) }} ..> {{ s.range }} : {{ gen.name(s) }}
+          {{ gen.name(element) }} --|> {{ s.range }} : {{ gen.name(s) }}
         {% endif %}
       {% endfor %}
 ```
 {% else %}
 ```{{ gen.mermaid_directive() }}
  classDiagram
     class {{ gen.name(element) }}
       {% for s in schemaview.class_induced_slots(element.name)|sort(attribute='name') -%}
         {{ gen.name(element) }} : {{gen.name(s)}}
         {% if s.range not in gen.all_type_object_names() %}
-          {{ gen.name(element) }} ..> {{ s.range }} : {{ gen.name(s) }}
+          {{ gen.name(element) }} --|> {{ s.range }} : {{ gen.name(s) }}
         {% endif %}
       {% endfor %}
 ```
 {% endif %}
 {% endif %}
```

### Comparing `linkml-1.5.0rc2/linkml/generators/docgen/common_metadata.md.jinja2` & `linkml-1.5.1/linkml/generators/docgen/common_metadata.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/docgen/enum.md.jinja2` & `linkml-1.5.1/linkml/generators/docgen/enum.md.jinja2`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Enum: {{ gen.name(element) }}
 
 {% if element.description %}
-_{{ element.description }}_
+{% set element_description_lines = element.description.split('\n') %}
+{% for element_description_line in element_description_lines %}
+_{{ element_description_line }}_
+{% endfor %}
 {% endif %}
 
 URI: {{ gen.uri_link(element) }}
 
 {% if element.permissible_values -%}
 ## Permissible Values
```

### Comparing `linkml-1.5.0rc2/linkml/generators/docgen/index.md.jinja2` & `linkml-1.5.1/linkml/generators/docgen/index.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/docgen/slot.md.jinja2` & `linkml-1.5.1/linkml/generators/docgen/slot.md.jinja2`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Slot: {{ gen.name(element) }}
 
 {%- if header -%}
 {{header}}
 {%- endif -%}
 
 {% if element.description %}
-_{{ element.description }}_
+{% set element_description_lines = element.description.split('\n') %}
+{% for element_description_line in element_description_lines %}
+_{{ element_description_line }}_
+{% endfor %}
 {% endif %}
 
 URI: {{ gen.uri_link(element) }}
 
 
 {% if schemaview.slot_parents(element.name) or schemaview.slot_children(element.name, mixins=False) %}
 
@@ -20,52 +23,56 @@
 <!-- no inheritance hierarchy -->
 {% endif %}
 
 {% if schemaview.get_classes_by_slot(element, include_induced=True) %}
 
 ## Applicable Classes
 
-| Name | Description |
-| --- | --- |
+| Name | Description | Modifies Slot |
+| --- | --- | --- |
 {% for c in schemaview.get_classes_by_slot(element, include_induced=True) -%}
-{{ gen.link(c) }} | {{ schemaview.get_class(c).description|enshorten }}
+{{ gen.link(c) }} | {{ schemaview.get_class(c).description|enshorten }} | {% if c in schemaview.get_classes_modifying_slot(element) %} yes {% else %} no {% endif %} |
 {% endfor %}
 
 {% endif %}
 
+
 {% if schemaview.is_mixin(element.name) %}
 ## Mixin Usage
 
 | mixed into | description | range | domain |
 | --- | --- | --- | --- |
 {% for s in schemaview.slot_children(element.name, is_a=False) -%}
 | {{ gen.link(s) }} | {{ schemaview.get_slot(s).description|enshorten }} | {{ schemaview.get_slot(s).range }} | {{ schemaview.get_classes_by_slot(schemaview.get_slot(s))|join(', ') }} |
 {% endfor %}
 {% endif %}
 
 ## Properties
 
 * Range: {{gen.link(element.range)}}
-{%- if element.multivalued %}
+{% if element.multivalued %}
 * Multivalued: {{ element.multivalued }}
-{% endif %}
-{%- if element.required %}
+{% endif -%}
+{% if element.required %}
 * Required: {{ element.required }}
 {% elif element.recommended %}
 * Recommended: {{ element.recommended }}
-{% endif %}
-{%- if element.minimum_value %}
-* Minimum Value: {{ element.minimum_value }}
-{% endif %}
-{%- if element.maximum_value %}
-* Maximum Value: {{ element.maximum_value }}
-{% endif %}
-{%- if schemaview.is_mixin(element.name) %}
+{% endif -%}
+{% if element.minimum_value is not none %}
+* Minimum Value: {{ element.minimum_value|int }}
+{% endif -%}
+{% if element.maximum_value is not none %}
+* Maximum Value: {{ element.maximum_value|int }}
+{% endif -%}
+{% if element.pattern %}
+* Regex pattern: {{ '`' }}{{  element.pattern }}{{ '`' }}
+{% endif -%}
+{% if schemaview.is_mixin(element.name) %}
 * Mixin: {{ element.mixin }}
-{% endif %}
+{% endif -%}
 
 
 {% if schemaview.usage_index().get(element.name) %}
 ## Usages
 
 | used by | used in | type | used |
 | ---  | --- | --- | --- |
```

### Comparing `linkml-1.5.0rc2/linkml/generators/docgen/subset.md.jinja2` & `linkml-1.5.1/linkml/generators/docgen/subset.md.jinja2`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Subset: {{ gen.name(element) }}
 
 {%- if header -%}
 {{header}}
 {%- endif -%}
 
 {% if element.description %}
-_{{ element.description }}_
+{% set element_description_lines = element.description.split('\n') %}
+{% for element_description_line in element_description_lines %}
+_{{ element_description_line }}_
+{% endfor %}
 {% endif %}
 
 URI: {{ gen.uri_link(element) }}
 
 
 {% include "common_metadata.md.jinja2" %}
```

### Comparing `linkml-1.5.0rc2/linkml/generators/docgen.py` & `linkml-1.5.1/linkml/generators/docgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -787,15 +787,15 @@
     def get_direct_slots(self, cls: ClassDefinition) -> List[SlotDefinition]:
         """Fetch list of all own attributes of a class, i.e., 
         all slots that belong to the domain of a class.
 
         :param cls: class for which we want to determine the attributes
         :return: list of all own attributes of a class
         """
-        return [self.inject_slot_info(self.schemaview.induced_slot(sn)) for sn in self.get_direct_slot_names(cls)]
+        return [self.inject_slot_info(self.schemaview.induced_slot(sn, cls.name)) for sn in self.get_direct_slot_names(cls)]
 
     def get_indirect_slots(self, cls: ClassDefinition) -> List[SlotDefinition]:
         """Fetch list of all inherited attributes of a class, i.e., 
         all slots that belong to the domain of a class.
 
         :param cls: class for which we want to determine the attributes
         :return: list of all own attributes of a class
```

### Comparing `linkml-1.5.0rc2/linkml/generators/dotgen.py` & `linkml-1.5.1/linkml/generators/dotgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/erdiagramgen.py` & `linkml-1.5.1/linkml/generators/erdiagramgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/excelgen.py` & `linkml-1.5.1/linkml/generators/excelgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import logging
 
 from dataclasses import dataclass
 from typing import List
 
 import click
 
 from linkml_runtime.utils.schemaview import SchemaView
@@ -22,14 +23,15 @@
     generatorversion = "0.1.1"
     valid_formats = ["xlsx"]
     uses_schemaloader = False
     requires_metamodel = False
 
     def __post_init__(self) -> None:
         super().__post_init__()
+        self.logger = logging.getLogger(__name__)
         self.schemaview = SchemaView(self.schema)
 
     def create_workbook(self, workbook_name: str) -> Workbook:
         """
         Creates an Excel workbook using the openpyxl library and returns it.
 
         :param workbook_name: Name of the workbook to be created.
@@ -132,21 +134,21 @@
 
         dv.add(f"{column_letter}2:{column_letter}1048576")
 
         workbook_name = self.get_workbook_name(workbook)
         workbook.save(workbook_name)
 
     def serialize(self, **kwargs) -> str:
-        output = (
-            convert_to_snake_case(self.schema.name) + ".xlsx"
+        self.output = (
+            os.path.abspath(convert_to_snake_case(self.schema.name) + ".xlsx")
             if not self.output
             else self.output
         )
 
-        workbook = self.create_workbook(output)
+        workbook = self.create_workbook(self.output)
         self.remove_worksheet_by_name(workbook, "Sheet")
         self.create_schema_worksheets(workbook)
 
         sv = self.schemaview
         for cls_name, cls in sv.all_classes(imports=self.mergeimports).items():
             if not cls.mixin and not cls.abstract:
                 slots = [
@@ -164,25 +166,26 @@
                     if s.range in enum_list:
                         pv_list = []
                         for pv_name, _ in sv.get_enum(
                             s.range
                         ).permissible_values.items():
                             pv_list.append(pv_name)
                         self.column_enum_validation(workbook, cls_name, s.name, pv_list)
+        self.logger.info(f"The Excel workbook has been written to {self.output}")
 
 
 @shared_arguments(ExcelGenerator)
 @click.command()
 @click.option(
     "-o",
     "--output",
     type=click.Path(),
     help="""Name of Excel spreadsheet to be created""",
 )
 @click.version_option(__version__, "-V", "--version")
 def cli(yamlfile, **kwargs):
     """Generate Excel representation of a LinkML model"""
-    print(ExcelGenerator(yamlfile, **kwargs).serialize(**kwargs))
+    ExcelGenerator(yamlfile, **kwargs).serialize(**kwargs)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `linkml-1.5.0rc2/linkml/generators/golrgen.py` & `linkml-1.5.1/linkml/generators/golrgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/graphqlgen.py` & `linkml-1.5.1/linkml/generators/graphqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/javagen/java_record_template.jinja2` & `linkml-1.5.1/linkml/generators/javagen/java_record_template.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/javagen.py` & `linkml-1.5.1/linkml/generators/javagen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/jsonldcontextgen.py` & `linkml-1.5.1/linkml/generators/jsonldcontextgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/jsonldgen.py` & `linkml-1.5.1/linkml/generators/jsonldgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/jsonschemagen.py` & `linkml-1.5.1/linkml/generators/jsonschemagen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/linkmlgen.py` & `linkml-1.5.1/linkml/generators/linkmlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/markdowngen.py` & `linkml-1.5.1/linkml/generators/markdowngen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/namespacegen.py` & `linkml-1.5.1/linkml/generators/namespacegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/oocodegen.py` & `linkml-1.5.1/linkml/generators/oocodegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/owlgen.py` & `linkml-1.5.1/linkml/generators/owlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/prefixmapgen.py` & `linkml-1.5.1/linkml/generators/prefixmapgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/projectgen.py` & `linkml-1.5.1/linkml/generators/projectgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/protogen.py` & `linkml-1.5.1/linkml/generators/protogen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/pydanticgen.py` & `linkml-1.5.1/linkml/generators/pydanticgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/pythongen.py` & `linkml-1.5.1/linkml/generators/pythongen.py`

 * *Files 4% similar despite different names*

```diff
@@ -358,29 +358,42 @@
                         rval.append(f"class {classname}({parent_cls}):\n\tpass")
                         break  # We only do the first primary key
         return "\n\n\n".join(rval)
 
     def gen_typedefs(self) -> str:
         """Generate python type declarations for all defined types"""
         rval = []
-        for typ in self.schema.types.values():
-            if not typ.imported_from:
+        defs_to_generate = [x for x in self.schema.types.values() if not x.imported_from]
+        emitted_types = []
+        ## all imported_from types are already considered generated
+        emitted_types.extend([x.name for x in self.schema.types.values() if x.imported_from])
+        for typ in [x for x in defs_to_generate if not x.typeof]:
+            typname = camelcase(typ.name)
+            desc = f'\n\t""" {typ.description} """' if typ.description else ""
+            base_base = typ.base.rsplit(".")[-1]
+            rval.append(
+                f"class {typname}({base_base}):{desc}\n\t{self.gen_type_meta(typ)}\n\n"
+            )
+            emitted_types.append(typ.name)
+
+        while True:
+            defs_to_generate_typeof = [x for x in defs_to_generate if x.typeof and not x.name in emitted_types]
+            if len(defs_to_generate_typeof) == 0:
+                break
+            defs_can_generate = [x for x in defs_to_generate_typeof if x.typeof in emitted_types ]
+            if len(defs_can_generate) == 0:
+                raise ValueError(f"Can not generate type definition for {[f'{x.name} of {x.typeof}' for x in defs_to_generate_typeof]}. Forgot a link in the type hierarchy chain ?")
+            for typ in defs_can_generate:
                 typname = camelcase(typ.name)
                 desc = f'\n\t""" {typ.description} """' if typ.description else ""
-
-                if typ.typeof:
-                    parent_typename = camelcase(typ.typeof)
-                    rval.append(
-                        f"class {typname}({parent_typename}):{desc}\n\t{self.gen_type_meta(typ)}\n\n"
-                    )
-                else:
-                    base_base = typ.base.rsplit(".")[-1]
-                    rval.append(
-                        f"class {typname}({base_base}):{desc}\n\t{self.gen_type_meta(typ)}\n\n"
-                    )
+                parent_typename = camelcase(typ.typeof)
+                rval.append(
+                    f"class {typname}({parent_typename}):{desc}\n\t{self.gen_type_meta(typ)}\n\n"
+                )
+                emitted_types.append(typ.name)
         return "\n".join(rval)
 
     def gen_classdefs(self) -> str:
         """Create class definitions for all non-mixin classes in the model
         Note that apply_to classes are transformed to mixins
         """
         clist = self._sort_classes(self.schema.classes.values())
```

### Comparing `linkml-1.5.0rc2/linkml/generators/rdfgen.py` & `linkml-1.5.1/linkml/generators/rdfgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/shaclgen.py` & `linkml-1.5.1/linkml/generators/shaclgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/shexgen.py` & `linkml-1.5.1/linkml/generators/shexgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/sparqlgen.py` & `linkml-1.5.1/linkml/generators/sparqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py` & `linkml-1.5.1/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py` & `linkml-1.5.1/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/sqlalchemygen.py` & `linkml-1.5.1/linkml/generators/sqlalchemygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/sqlddlgen.py` & `linkml-1.5.1/linkml/generators/sqlddlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/sqltablegen.py` & `linkml-1.5.1/linkml/generators/sqltablegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/sssomgen.py` & `linkml-1.5.1/linkml/generators/sssomgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/string_template.md` & `linkml-1.5.1/linkml/generators/string_template.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/summarygen.py` & `linkml-1.5.1/linkml/generators/summarygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/terminusdbgen.py` & `linkml-1.5.1/linkml/generators/terminusdbgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/typescriptgen.py` & `linkml-1.5.1/linkml/generators/typescriptgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/yamlgen.py` & `linkml-1.5.1/linkml/generators/yamlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/generators/yumlgen.py` & `linkml-1.5.1/linkml/generators/yumlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/linter/cli.py` & `linkml-1.5.1/linkml/linter/cli.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/linter/config/datamodel/config.py` & `linkml-1.5.1/linkml/linter/config/datamodel/config.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/linter/config/datamodel/config.yaml` & `linkml-1.5.1/linkml/linter/config/datamodel/config.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/linter/config/default.yaml` & `linkml-1.5.1/linkml/linter/config/default.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/linter/formatters/formatter.py` & `linkml-1.5.1/linkml/linter/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/linter/formatters/json_formatter.py` & `linkml-1.5.1/linkml/linter/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/linter/formatters/markdown_formatter.py` & `linkml-1.5.1/linkml/linter/formatters/markdown_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/linter/formatters/terminal_formatter.py` & `linkml-1.5.1/linkml/linter/formatters/terminal_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/linter/formatters/tsv_formatter.py` & `linkml-1.5.1/linkml/linter/formatters/tsv_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/linter/linter.py` & `linkml-1.5.1/linkml/linter/linter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/linter/rules.py` & `linkml-1.5.1/linkml/linter/rules.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/reporting/model.py` & `linkml-1.5.1/linkml/reporting/model.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/transformers/relmodel_transformer.py` & `linkml-1.5.1/linkml/transformers/relmodel_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/transformers/schema_renamer.py` & `linkml-1.5.1/linkml/transformers/schema_renamer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/converter.py` & `linkml-1.5.1/linkml/utils/converter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/datautils.py` & `linkml-1.5.1/linkml/utils/datautils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/execute_tutorial.py` & `linkml-1.5.1/linkml/utils/execute_tutorial.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/generator.py` & `linkml-1.5.1/linkml/utils/generator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/ifabsent_functions.py` & `linkml-1.5.1/linkml/utils/ifabsent_functions.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/mergeutils.py` & `linkml-1.5.1/linkml/utils/mergeutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/rawloader.py` & `linkml-1.5.1/linkml/utils/rawloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/schema_builder.py` & `linkml-1.5.1/linkml/utils/schema_builder.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/schema_fixer.py` & `linkml-1.5.1/linkml/utils/schema_fixer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/schemaloader.py` & `linkml-1.5.1/linkml/utils/schemaloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/schemasynopsis.py` & `linkml-1.5.1/linkml/utils/schemasynopsis.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/sqlutils.py` & `linkml-1.5.1/linkml/utils/sqlutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/typereferences.py` & `linkml-1.5.1/linkml/utils/typereferences.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/utils/validation.py` & `linkml-1.5.1/linkml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/validators/jsonschemavalidator.py` & `linkml-1.5.1/linkml/validators/jsonschemavalidator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
+import logging
 import sys
 from dataclasses import dataclass
-from typing import TextIO, Type, Union
+from typing import TextIO, Type, Union, Dict, Optional
 
 import click
 import jsonschema
 from linkml_runtime.dumpers import json_dumper
 from linkml_runtime.linkml_model import SchemaDefinition, ClassDefinitionName
 from linkml_runtime.utils.compile_python import compile_python
 from linkml_runtime.utils.dictutils import as_simple_dict
@@ -17,14 +18,21 @@
 from linkml.generators.pythongen import PythonGenerator
 from linkml.utils import datautils
 from linkml.utils.datavalidator import DataValidator
 
 
 @dataclass
 class JsonSchemaDataValidator(DataValidator):
+    """
+    Implementation of DataValidator that wraps jsonschema validation
+    """
+
+    jsonschema_objs: Optional[Dict[str, Dict]] = None
+    """Cached outputs of jsonschema generation"""
+
     def validate_file(self, input: str, format: str = "json", **kwargs):
         return self.validate_object(obj)
 
     def validate_object(
         self, data: YAMLRoot, target_class: Type[YAMLRoot] = None, closed: bool = True
     ) -> None:
         """
@@ -37,21 +45,29 @@
         """
         if target_class is None:
             target_class = type(data)
         inst_dict = as_simple_dict(data)
         not_closed = not closed
         if self.schema is None:
             raise ValueError(f"schema object must be set")
-        jsonschemastr = JsonSchemaGenerator(
-            self.schema,
-            mergeimports=True,
-            top_class=target_class.class_name,
-            not_closed=not_closed,
-        ).serialize(not_closed=not_closed)
-        jsonschema_obj = json.loads(jsonschemastr)
+        if self.jsonschema_objs is None:
+            self.jsonschema_objs = {}
+        schema_id = self.schema.id if isinstance(self.schema, SchemaDefinition) else self.schema
+        if schema_id not in self.jsonschema_objs:
+            jsonschemastr = JsonSchemaGenerator(
+                self.schema,
+                mergeimports=True,
+                top_class=target_class.class_name,
+                not_closed=not_closed,
+            ).serialize(not_closed=not_closed)
+            jsonschema_obj = json.loads(jsonschemastr)
+            self.jsonschema_objs[schema_id] = jsonschema_obj
+        else:
+            logging.info(f"Using cached jsonschema for {schema_id}")
+            jsonschema_obj = self.jsonschema_objs[schema_id]
         return jsonschema.validate(inst_dict, schema=jsonschema_obj, format_checker=jsonschema.Draft7Validator.FORMAT_CHECKER)
 
     def validate_dict(
         self, data: dict, target_class: ClassDefinitionName = None, closed: bool = True
     ) -> None:
         """
         validates instance data against a schema
```

### Comparing `linkml-1.5.0rc2/linkml/validators/sparqlvalidator.py` & `linkml-1.5.1/linkml/validators/sparqlvalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/workspaces/datamodel/workspaces.py` & `linkml-1.5.1/linkml/workspaces/datamodel/workspaces.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/workspaces/datamodel/workspaces.yaml` & `linkml-1.5.1/linkml/workspaces/datamodel/workspaces.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/linkml/workspaces/example_runner.py` & `linkml-1.5.1/linkml/workspaces/example_runner.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.0rc2/pyproject.toml` & `linkml-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml"
-version = "1.5.0rc2"
+version = "1.5.1"
 description = "Linked Open Data Modeling Language"
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harold Solbrig <solbrig@jhu.edu>",
     "Sujay Patil <spatil@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>",
     "Sierra Moxon <smoxon@lbl.gov>",
@@ -101,15 +101,15 @@
 graphviz = ">=0.10.1"
 hbreader = "*"
 isodate = ">=0.6.0"
 jinja2 = ">= 3.1.0"
 jsonasobj2 = "==1.*,>=1.0.0,>=1.0.3"
 jsonschema = {extras = ["format"], version = ">=4.0.0"}
 linkml-dataops = "*"
-linkml-runtime = "1.5.0rc2"
+linkml-runtime = ">=1.5.0"
 myst-parser = "*"
 openpyxl = "*"
 parse = "*"
 prefixcommons = ">=0.1.7"
 prefixmaps = "^0.1.3"
 pydantic = "*"
 pyjsg = ">=0.11.6"
```

### Comparing `linkml-1.5.0rc2/PKG-INFO` & `linkml-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml
-Version: 1.5.0rc2
+Version: 1.5.1
 Summary: Linked Open Data Modeling Language
 Home-page: https://linkml.io/linkml/
 Keywords: schema,linked data,data modeling,rdf,owl,biolink
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.7.6,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,15 +30,15 @@
 Requires-Dist: graphviz (>=0.10.1)
 Requires-Dist: hbreader
 Requires-Dist: isodate (>=0.6.0)
 Requires-Dist: jinja2 (>=3.1.0)
 Requires-Dist: jsonasobj2 (>=1.0.3,<2.0.0)
 Requires-Dist: jsonschema[format] (>=4.0.0)
 Requires-Dist: linkml-dataops
-Requires-Dist: linkml-runtime (==1.5.0rc2)
+Requires-Dist: linkml-runtime (>=1.5.0)
 Requires-Dist: myst-parser
 Requires-Dist: openpyxl
 Requires-Dist: parse
 Requires-Dist: prefixcommons (>=0.1.7)
 Requires-Dist: prefixmaps (>=0.1.3,<0.2.0)
 Requires-Dist: pydantic
 Requires-Dist: pyjsg (>=0.11.6)
```

