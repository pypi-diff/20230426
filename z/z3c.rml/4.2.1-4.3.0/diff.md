# Comparing `tmp/z3c.rml-4.2.1.tar.gz` & `tmp/z3c.rml-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3c.rml-4.2.1.tar", last modified: Fri Sep 30 14:05:50 2022, max compression
+gzip compressed data, was "z3c.rml-4.3.0.tar", last modified: Tue Apr 25 15:24:08 2023, max compression
```

## Comparing `z3c.rml-4.2.1.tar` & `z3c.rml-4.3.0.tar`

### file list

```diff
@@ -1,437 +1,435 @@
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2022-09-30 14:05:50.629050 z3c.rml-4.2.1/
--rw-rw-r--   0 adi       (1000) adi       (1000)      218 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/AUTHORS.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)    19603 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/CHANGES.rst
--rw-rw-r--   0 adi       (1000) adi       (1000)      804 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/CONTRIBUTING.md
--rw-rw-r--   0 adi       (1000) adi       (1000)       32 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/COPYRIGHT.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)     2070 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/LICENSE.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)      504 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/MANIFEST.in
--rw-rw-r--   0 adi       (1000) adi       (1000)    27726 2022-09-30 14:05:50.629050 z3c.rml-4.2.1/PKG-INFO
--rw-rw-r--   0 adi       (1000) adi       (1000)     1173 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/README.rst
--rw-rw-r--   0 adi       (1000) adi       (1000)     4861 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/RML-DIFFERENCES.rst
--rw-rw-r--   0 adi       (1000) adi       (1000)      354 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/TODOS.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)      417 2022-09-30 14:05:50.629050 z3c.rml-4.2.1/setup.cfg
--rw-rw-r--   0 adi       (1000) adi       (1000)     2730 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/setup.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2022-09-30 14:05:50.609050 z3c.rml-4.2.1/src/
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2022-09-30 14:05:50.609050 z3c.rml-4.2.1/src/z3c/
--rw-rw-r--   0 adi       (1000) adi       (1000)      200 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/__init__.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2022-09-30 14:05:50.613050 z3c.rml-4.2.1/src/z3c/rml/
--rw-rw-r--   0 adi       (1000) adi       (1000)      894 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/README.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)      299 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/__init__.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    24330 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/attr.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    32142 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/canvas.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    47367 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/chart.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     4899 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/directive.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     5294 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/doclogic.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    25487 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/document.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     3391 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/dtd.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    52881 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/flowable.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    11118 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/form.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     5887 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/interfaces.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     5753 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/list.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     3738 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/num2words.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     3342 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/occurence.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     4215 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/page.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     1651 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/pagetemplate.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     1852 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/pagetemplate.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)    11001 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/paraparser.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     9674 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/pdfinclude.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     4803 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/platypus.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     8979 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/reference.pt
--rw-rw-r--   0 adi       (1000) adi       (1000)     9292 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/reference.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     7673 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/rlfix.py
--rw-rw-r--   0 adi       (1000) adi       (1000)   474971 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/rml-reference.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    85160 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/rml.dtd
--rw-rw-r--   0 adi       (1000) adi       (1000)     3545 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/rml2pdf.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     4303 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/rml2pdfscript.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     3626 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/special.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     3596 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/storyplace.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    27144 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/stylesheet.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    49344 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/svg2rlg.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     9164 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/template.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2022-09-30 14:05:50.613050 z3c.rml-4.2.1/src/z3c/rml/tests/
--rw-rw-r--   0 adi       (1000) adi       (1000)       18 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/__init__.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2022-09-30 14:05:50.621050 z3c.rml-4.2.1/src/z3c/rml/tests/expected/
--rw-rw-r--   0 adi       (1000) adi       (1000)     2054 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/encoding-test-latin1.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2053 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/encoding-test-utf8.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1737 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/printScaling.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2084 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-000-simple.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    15824 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-001-cmbox.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2481 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-001-hello.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    14776 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-002-paras.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2454 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-003-frames.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3634 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-004-fpt-templates.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3634 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-004-templates.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)   103700 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-005-fonts.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3434 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-006-barcodes.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    18447 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-008-tables.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     4668 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-009-splitting.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2205 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-010-linkURL.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     7479 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-011-keepwithnext.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     4464 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-017-outlines.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     7926 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-022-paras-oas.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    11780 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-029-keepinframe.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     6596 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-031-japanese.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     6359 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-032-images.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2390 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-034-cmyk.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    16663 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-035-numbering.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    16517 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-036-numbering-contd.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    15535 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-037-plugingraphic.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    19351 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-038-rect-href.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    21163 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-039-doc-programming.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    15604 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-040-colors.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    18987 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-041-masking.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    23147 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-042-longdoc.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    16162 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-043-headings.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    17185 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-044-codesnippets.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    16403 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-045-cmyk.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    18283 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-046-lists.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    29535 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-047-condPageBreak.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    25858 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-048-paragraph-flow-controls.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    16987 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-049-pre.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2487 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-050-header-footer.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1567 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-01.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1728 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-02.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2603 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-03.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2507 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-04.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3031 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-05.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2560 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-06.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1656 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-07.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1638 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-08.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3402 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-09.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2520 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-10.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2981 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-11.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     6351 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-12.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    69053 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/sample-shipment-chinese.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1808 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/simple-layout.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3528 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/special-text.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3843 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/symbols-set.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1949 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-addMapping.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1876 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-alias.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2825 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-barChart.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3803 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-barChart3d.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    10824 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-barCodeFlowable.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2809 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-barcode.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1793 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockNosplit.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1922 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-1.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2759 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-10.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2335 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-2.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2335 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-3.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2049 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-4.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2159 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-5.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2309 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-6.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2191 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-7.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2244 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-8.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2243 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-9.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2012 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-bulkData.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2398 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTableStyle-2.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1811 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTableStyle-3.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2686 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTableStyle.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     6957 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-bookmark.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1614 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-buttonField.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1841 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-circle.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2091 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-codesnippet.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1654 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-color.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2304 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-condPageBreak.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1888 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-cropMarks.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1574 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-curves.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2126 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-doc.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2105 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-docinit-viewer-options.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1776 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-document-annotations.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1563 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-document-pageDrawing.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1773 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-document-story.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1874 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-drawAlignedString.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1567 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-drawCenteredString.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1567 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-drawRightString.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1566 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-drawString.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1877 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-ellipse.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1632 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-fill.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2119 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-fixedSize.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1624 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-grid.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1683 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-hr.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2162 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-illustration.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     4205 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-image-1.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     5364 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-image-data-uri.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2889 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-image-mask.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    22478 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-image-svg.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     4090 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-image.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     4045 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-imageAndFlowables-svg.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     5986 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-imageAndFlowables.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     6068 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-img.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    21682 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-includePdfPages-edge-dupekey.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    28946 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-includePdfPages-firstPage.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    96766 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-includePdfPages-noAdditionalText.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    97285 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-includePdfPages.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2224 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-indent.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     4298 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-index.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2605 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-keepInFrame.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3287 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-keepTogether.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1638 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-lineMode.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3229 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-linePlot.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    34207 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-linePlot3D.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1563 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-lines.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1833 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-log.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    22418 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-mergePage-2.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    35305 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-mergePage.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1814 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-name.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1783 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-nextFrame.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2299 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-nextPage.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2070 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-outlineAdd.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1973 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pageGraphics.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1564 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pageInfo-2.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1551 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pageInfo.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3255 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pageNumber.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1791 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-border.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1468 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-comment.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1515 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-span-strike.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1569 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-span-texttransform.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1518 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-span-underline.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1858 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-span.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1573 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-strike.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1574 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-underline.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2096 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-wordWrap.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2760 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1744 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-path.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    96766 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pdfInclude-noAdditionalText.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3258 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pieChart.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    19465 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pieChart3d.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2254 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-place.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1959 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-plugInFlowable.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1885 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-plugInGraphic.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2128 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pre.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2686 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pto.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1791 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-rectange.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3205 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-registerCidFont.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    21768 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-registerTTFont-builtins.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    27508 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-registerTTFont.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    82730 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-registerType1Face.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1603 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-rotate.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1758 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-saveState-restoreState.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1581 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-scale.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    22549 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-selectField.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1576 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-setFont.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1588 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-setFontSize.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1865 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-setNextFrame.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2924 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-setNextTemplate.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1597 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-skew.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2077 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-spacer.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     3405 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-spiderChart.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1807 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-storyPlace.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1631 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-stroke.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1749 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-textAnnotation.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    22167 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-textField.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1597 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-transform.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1581 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-translate.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     6781 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-ul-ol-li.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2199 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-xpre.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     2033 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/expected/text-not-in-tags.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)     1053 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/flowable.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2022-09-30 14:05:50.625050 z3c.rml-4.2.1/src/z3c/rml/tests/input/
--rw-rw-r--   0 adi       (1000) adi       (1000)     3519 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/400x200.gif
--rw-rw-r--   0 adi       (1000) adi       (1000)    65932 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/Vera.ttf
--rw-rw-r--   0 adi       (1000) adi       (1000)     7892 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/VeraMono.ttf
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2022-09-30 14:05:50.629050 z3c.rml-4.2.1/src/z3c/rml/tests/input/data/
--rw-rw-r--   0 adi       (1000) adi       (1000)    10808 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/data/bad1-dupekey.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)   306050 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/data/fw2.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    24160 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/data/include-bookmarks1.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    18217 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/data/include-bookmarks2.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    10795 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/data/include1.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)    28946 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/data/include2.pdf
--rw-rw-r--   0 adi       (1000) adi       (1000)      766 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/encoding-test-latin1.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      732 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/encoding-test-utf8.rml
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2022-09-30 14:05:50.629050 z3c.rml-4.2.1/src/z3c/rml/tests/input/images/
--rw-rw-r--   0 adi       (1000) adi       (1000)     6360 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/images/cylinder.eps
--rw-rw-r--   0 adi       (1000) adi       (1000)      921 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/images/cylinder.png
--rw-rw-r--   0 adi       (1000) adi       (1000)    16277 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/images/cylinder.svg
--rw-rw-r--   0 adi       (1000) adi       (1000)     2920 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/images/cylinder.svgz
--rw-rw-r--   0 adi       (1000) adi       (1000)     2269 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/images/replogo.gif
--rw-rw-r--   0 adi       (1000) adi       (1000)     6150 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/logo_no_bar.png
--rw-rw-r--   0 adi       (1000) adi       (1000)      474 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/printScaling.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      371 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-000-simple.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2851 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-001-cmbox.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     3051 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-001-hello.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)    16873 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-002-paras.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     5809 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-003-frames.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     5757 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-004-fpt-templates.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     5729 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-004-templates.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2559 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-005-fonts.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1609 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-006-barcodes.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)    30537 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-008-tables.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     3066 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-009-splitting.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1089 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-010-linkURL.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     6106 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-011-keepwithnext.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1304 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-017-outlines.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)    12959 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-022-paras-oas.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)    24633 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-029-keepinframe.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     5717 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-031-japanese.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     8989 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-032-images.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     3119 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-034-cmyk.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     4380 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-035-numbering.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     4088 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-036-numbering-contd.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1089 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-037-plugingraphic.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     3948 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-038-rect-href.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     8030 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-039-doc-programming.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2391 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-040-colors.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     3258 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-041-masking.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     6212 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-042-longdoc.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2721 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-043-headings.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     4376 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-044-codesnippets.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     4624 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-045-cmyk.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     8269 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-046-lists.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)    23008 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-047-condPageBreak.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)    18794 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-048-paragraph-flow-controls.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     4409 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-049-pre.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      952 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-050-header-footer.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      248 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-01.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      582 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-02.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     4328 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-03.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     7321 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-04.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     4660 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-05.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     3115 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-06.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1625 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-07.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      682 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-08.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2475 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-09.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     3030 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-10.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2981 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-11.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     7542 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-12.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      859 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/simple-layout.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2648 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/special-text.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     7241 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/strapline.png
--rw-rw-r--   0 adi       (1000) adi       (1000)     9502 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/symbols-set.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1081 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-addMapping.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      582 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-alias.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2504 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-barChart.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2282 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-barChart3d.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     6949 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-barCodeFlowable.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      815 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-barcode.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2393 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockNosplit.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      652 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-1.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      773 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-10.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1081 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-2.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1091 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-3.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1098 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-4.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1766 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-5.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1807 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-6.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1306 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-7.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1332 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-8.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1962 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-9.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      559 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-bulkData.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2034 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTableStyle-2.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      881 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTableStyle-3.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     4343 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTableStyle.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1298 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-bookmark.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      496 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-buttonField.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      570 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-circle.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1127 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-codesnippet.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      786 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-color.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      560 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-condPageBreak.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      622 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-cropMarks.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      367 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-curves.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1154 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-doc.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      802 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-docinit-viewer-options.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      665 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-document-annotations.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      308 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-document-pageDrawing.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      510 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-document-story.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1554 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-drawAlignedString.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      335 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-drawCenteredString.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      327 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-drawRightString.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      309 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-drawString.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      628 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-ellipse.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      313 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-fill.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1733 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-fixedSize.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      339 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-grid.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      545 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-hr.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      972 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-illustration.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      698 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-image-1.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     6538 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-image-data-uri.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      720 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-image-mask.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1075 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-image-svg.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      633 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-image.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1971 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-imageAndFlowables-svg.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1945 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-imageAndFlowables.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2248 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-img.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      747 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-includePdfPages-firstPage.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1037 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-includePdfPages-noAdditionalText.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1085 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-includePdfPages.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1406 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-indent.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      984 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-index.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1916 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-keepInFrame.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2391 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-keepTogether.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      318 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-lineMode.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     4719 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-linePlot.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2559 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-linePlot3D.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      317 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-lines.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1177 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-log.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1570 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-mergePage-2.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1918 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-mergePage.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      663 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-name.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      509 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-nextFrame.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      523 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-nextPage.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      578 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-outlineAdd.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      582 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pageGraphics.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      338 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pageInfo-2.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      327 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pageInfo.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      944 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pageNumber.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      766 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-border.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      494 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-comment.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      737 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-span-strike.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1413 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-span-texttransform.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      765 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-span-underline.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      712 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-span.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      925 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-strike.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      973 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-underline.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1517 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-wordWrap.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1376 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1082 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-path.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     3008 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pieChart.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2482 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pieChart3d.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2021 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-place.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      688 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-plugInFlowable.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      464 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-plugInGraphic.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      510 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pre.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2944 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pto.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      454 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-rectange.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      787 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-registerCidFont.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      667 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-registerTTFont-builtins.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      811 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-registerTTFont.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      729 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-registerType1Face.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      403 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-rotate.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      608 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-saveState-restoreState.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      406 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-scale.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      947 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-selectField.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      342 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-setFont.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      430 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-setFontSize.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      817 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-setNextFrame.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      931 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-setNextTemplate.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      406 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-skew.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      827 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-spacer.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     2546 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-spiderChart.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1108 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-storyPlace.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      305 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-stroke.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      428 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-textAnnotation.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      750 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-textField.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      459 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-transform.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      414 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-translate.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     9866 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-ul-ol-li.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      686 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-xpre.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)      857 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/text-not-in-tags.rml
--rw-rw-r--   0 adi       (1000) adi       (1000)     1506 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/input/zope3logo.gif
--rw-rw-r--   0 adi       (1000) adi       (1000)     3392 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/module.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     1485 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/test_directive.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     1339 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/test_dtd.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     3886 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/test_num2words.py
--rw-rw-r--   0 adi       (1000) adi       (1000)      853 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/test_pagetemplate.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     1015 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/test_reference.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     6809 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/test_rml.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     2030 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/test_rml2pdf.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     2286 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/test_subprocess.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     3967 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c/rml/tests/test_svg2rlg.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2022-09-30 14:05:50.609050 z3c.rml-4.2.1/src/z3c.rml.egg-info/
--rw-rw-r--   0 adi       (1000) adi       (1000)    27726 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c.rml.egg-info/PKG-INFO
--rw-rw-r--   0 adi       (1000) adi       (1000)    18854 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c.rml.egg-info/SOURCES.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)        1 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c.rml.egg-info/dependency_links.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)      108 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c.rml.egg-info/entry_points.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)        4 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c.rml.egg-info/namespace_packages.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)        1 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c.rml.egg-info/not-zip-safe
--rw-rw-r--   0 adi       (1000) adi       (1000)      198 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c.rml.egg-info/requires.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)        4 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/src/z3c.rml.egg-info/top_level.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)     1311 2022-09-30 14:05:50.000000 z3c.rml-4.2.1/tox.ini
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-25 15:24:08.213793 z3c.rml-4.3.0/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      218 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/AUTHORS.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    20030 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/CHANGES.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      804 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/CONTRIBUTING.md
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       32 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/COPYRIGHT.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2070 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/LICENSE.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      504 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/MANIFEST.in
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    23661 2023-04-25 15:24:08.213793 z3c.rml-4.3.0/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2535 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/README.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4861 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/RML-DIFFERENCES.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      354 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/TODOS.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      433 2023-04-25 15:24:08.213793 z3c.rml-4.3.0/setup.cfg
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2749 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/setup.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-25 15:24:08.173793 z3c.rml-4.3.0/src/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-25 15:24:08.177793 z3c.rml-4.3.0/src/z3c/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       76 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-25 15:24:08.181793 z3c.rml-4.3.0/src/z3c/rml/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      894 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/README.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      299 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    24284 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/attr.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    31617 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/canvas.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    47417 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/chart.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4899 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/directive.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5294 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/doclogic.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    25487 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/document.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3380 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/dtd.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    52881 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/flowable.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    11118 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/form.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5887 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/interfaces.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5844 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/list.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3738 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/num2words.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3342 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/occurence.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4215 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/page.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1651 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/pagetemplate.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1852 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/pagetemplate.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    10923 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/paraparser.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9664 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/pdfinclude.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4793 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/platypus.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     8979 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/reference.pt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9288 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/reference.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7673 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/rlfix.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)   474971 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/rml-reference.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    85160 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/rml.dtd
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3574 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/rml2pdf.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4303 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/rml2pdfscript.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3626 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/special.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3596 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/storyplace.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    27144 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/stylesheet.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9164 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/template.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-25 15:24:08.181793 z3c.rml-4.3.0/src/z3c/rml/tests/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-25 15:24:08.197793 z3c.rml-4.3.0/src/z3c/rml/tests/expected/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2054 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/encoding-test-latin1.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2053 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/encoding-test-utf8.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1737 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/printScaling.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2084 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-000-simple.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    15824 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-001-cmbox.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2481 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-001-hello.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    14776 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-002-paras.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2454 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-003-frames.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3634 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-004-fpt-templates.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3634 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-004-templates.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)   103700 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-005-fonts.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3434 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-006-barcodes.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    18447 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-008-tables.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4668 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-009-splitting.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2205 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-010-linkURL.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7479 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-011-keepwithnext.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4464 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-017-outlines.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7926 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-022-paras-oas.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    11780 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-029-keepinframe.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6596 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-031-japanese.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6359 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-032-images.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2390 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-034-cmyk.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    16663 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-035-numbering.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    16517 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-036-numbering-contd.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    15535 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-037-plugingraphic.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    19351 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-038-rect-href.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    21163 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-039-doc-programming.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    15604 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-040-colors.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    18987 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-041-masking.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    23147 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-042-longdoc.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    16162 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-043-headings.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    17185 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-044-codesnippets.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    16403 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-045-cmyk.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    18283 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-046-lists.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    29535 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-047-condPageBreak.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    25858 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-048-paragraph-flow-controls.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    16987 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-049-pre.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2487 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-050-header-footer.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1567 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-01.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1728 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-02.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2603 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-03.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2507 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-04.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3031 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-05.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2560 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-06.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1656 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-07.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1638 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-08.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3402 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-09.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2520 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-10.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2981 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-11.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6351 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-12.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    69053 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/sample-shipment-chinese.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1808 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/simple-layout.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3528 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/special-text.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3843 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/symbols-set.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1949 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-addMapping.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1876 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-alias.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2825 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-barChart.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3803 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-barChart3d.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    10824 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-barCodeFlowable.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2809 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-barcode.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1793 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockNosplit.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1922 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-1.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2759 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-10.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2335 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-2.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2335 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-3.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2049 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-4.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2159 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-5.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2309 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-6.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2191 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-7.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2244 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-8.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2243 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-9.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2012 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-bulkData.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2398 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTableStyle-2.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1811 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTableStyle-3.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2686 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTableStyle.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6957 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-bookmark.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1614 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-buttonField.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1841 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-circle.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2091 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-codesnippet.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1654 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-color.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2304 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-condPageBreak.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1888 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-cropMarks.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1574 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-curves.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2126 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-doc.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2105 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-docinit-viewer-options.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1776 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-document-annotations.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1563 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-document-pageDrawing.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1773 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-document-story.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1874 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-drawAlignedString.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1567 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-drawCenteredString.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1567 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-drawRightString.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1566 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-drawString.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1877 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-ellipse.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1632 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-fill.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2119 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-fixedSize.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1624 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-grid.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1683 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-hr.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2162 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-illustration.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4205 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-image-1.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5364 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-image-data-uri.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2889 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-image-mask.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    22478 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-image-svg.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4090 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-image.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4045 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-imageAndFlowables-svg.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5986 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-imageAndFlowables.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6068 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-img.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    21682 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-includePdfPages-edge-dupekey.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    28946 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-includePdfPages-firstPage.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    96766 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-includePdfPages-noAdditionalText.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    97285 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-includePdfPages.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2224 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-indent.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4298 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-index.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2605 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-keepInFrame.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3287 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-keepTogether.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1638 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-lineMode.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3229 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-linePlot.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    34207 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-linePlot3D.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1563 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-lines.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1833 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-log.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    22418 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-mergePage-2.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    35305 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-mergePage.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1814 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-name.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1783 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-nextFrame.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2299 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-nextPage.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2070 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-outlineAdd.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1973 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pageGraphics.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1564 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pageInfo-2.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1551 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pageInfo.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3255 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pageNumber.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1791 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-border.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1468 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-comment.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1515 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-span-strike.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1569 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-span-texttransform.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1518 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-span-underline.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1858 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-span.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1573 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-strike.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1574 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-underline.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2096 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-wordWrap.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2760 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1744 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-path.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    96766 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pdfInclude-noAdditionalText.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3258 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pieChart.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    19465 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pieChart3d.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2254 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-place.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1959 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-plugInFlowable.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1885 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-plugInGraphic.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2128 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pre.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2686 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pto.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1791 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-rectange.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3205 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-registerCidFont.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    21768 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-registerTTFont-builtins.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    27508 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-registerTTFont.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    82730 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-registerType1Face.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1603 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-rotate.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1758 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-saveState-restoreState.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1581 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-scale.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    22549 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-selectField.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1576 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-setFont.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1588 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-setFontSize.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1865 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-setNextFrame.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2924 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-setNextTemplate.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1597 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-skew.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2077 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-spacer.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3405 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-spiderChart.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1807 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-storyPlace.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1631 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-stroke.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1749 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-textAnnotation.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    22167 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-textField.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1597 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-transform.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1581 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-translate.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6781 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-ul-ol-li.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2199 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-xpre.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2033 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/expected/text-not-in-tags.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1053 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/flowable.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-25 15:24:08.213793 z3c.rml-4.3.0/src/z3c/rml/tests/input/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3519 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/400x200.gif
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    65932 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/Vera.ttf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7892 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/VeraMono.ttf
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-25 15:24:08.213793 z3c.rml-4.3.0/src/z3c/rml/tests/input/data/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    10808 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/data/bad1-dupekey.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)   306050 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/data/fw2.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    24160 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/data/include-bookmarks1.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    18217 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/data/include-bookmarks2.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    10795 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/data/include1.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    28946 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/data/include2.pdf
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      766 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/encoding-test-latin1.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      732 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/encoding-test-utf8.rml
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-25 15:24:08.213793 z3c.rml-4.3.0/src/z3c/rml/tests/input/images/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6360 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/images/cylinder.eps
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      921 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/images/cylinder.png
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    16277 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/images/cylinder.svg
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2920 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/images/cylinder.svgz
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2269 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/images/replogo.gif
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6150 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/logo_no_bar.png
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      474 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/printScaling.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      371 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-000-simple.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2851 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-001-cmbox.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3051 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-001-hello.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    16873 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-002-paras.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5809 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-003-frames.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5757 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-004-fpt-templates.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5729 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-004-templates.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2559 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-005-fonts.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1609 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-006-barcodes.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    30537 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-008-tables.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3066 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-009-splitting.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1089 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-010-linkURL.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6106 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-011-keepwithnext.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1304 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-017-outlines.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    12959 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-022-paras-oas.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    24633 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-029-keepinframe.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5717 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-031-japanese.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     8989 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-032-images.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3119 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-034-cmyk.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4380 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-035-numbering.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4088 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-036-numbering-contd.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1089 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-037-plugingraphic.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3948 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-038-rect-href.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     8030 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-039-doc-programming.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2391 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-040-colors.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3258 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-041-masking.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6212 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-042-longdoc.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2721 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-043-headings.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4376 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-044-codesnippets.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4624 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-045-cmyk.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     8500 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-046-lists.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    23008 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-047-condPageBreak.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    18794 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-048-paragraph-flow-controls.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4409 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-049-pre.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      952 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-050-header-footer.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      248 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-01.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      582 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-02.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4328 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-03.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7321 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-04.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4660 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-05.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3115 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-06.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1625 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-07.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      682 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-08.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2475 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-09.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3030 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-10.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2981 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-11.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7542 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-12.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      859 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/simple-layout.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2648 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/special-text.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7241 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/strapline.png
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9502 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/symbols-set.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1081 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-addMapping.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      582 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-alias.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2504 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-barChart.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2282 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-barChart3d.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6949 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-barCodeFlowable.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      815 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-barcode.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2393 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockNosplit.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      652 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-1.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      773 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-10.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1081 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-2.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1091 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-3.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1098 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-4.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1766 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-5.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1807 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-6.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1306 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-7.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1332 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-8.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1962 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-9.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      559 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-bulkData.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2034 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTableStyle-2.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      881 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTableStyle-3.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4343 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTableStyle.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1298 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-bookmark.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      496 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-buttonField.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      570 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-circle.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1127 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-codesnippet.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      786 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-color.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      560 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-condPageBreak.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      622 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-cropMarks.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      367 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-curves.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1154 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-doc.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      802 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-docinit-viewer-options.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      665 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-document-annotations.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      308 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-document-pageDrawing.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      510 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-document-story.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1554 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-drawAlignedString.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      335 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-drawCenteredString.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      327 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-drawRightString.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      309 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-drawString.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      628 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-ellipse.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      313 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-fill.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1733 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-fixedSize.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      339 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-grid.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      545 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-hr.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      972 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-illustration.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      698 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-image-1.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6538 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-image-data-uri.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      720 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-image-mask.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1075 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-image-svg.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      633 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-image.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1971 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-imageAndFlowables-svg.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1945 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-imageAndFlowables.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2248 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-img.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      747 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-includePdfPages-firstPage.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1037 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-includePdfPages-noAdditionalText.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1085 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-includePdfPages.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1406 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-indent.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      984 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-index.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1916 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-keepInFrame.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2391 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-keepTogether.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      318 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-lineMode.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4719 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-linePlot.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2559 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-linePlot3D.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      317 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-lines.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1177 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-log.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1570 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-mergePage-2.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1918 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-mergePage.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      663 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-name.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      509 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-nextFrame.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      523 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-nextPage.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      578 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-outlineAdd.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      582 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pageGraphics.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      338 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pageInfo-2.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      327 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pageInfo.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      944 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pageNumber.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      766 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-border.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      494 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-comment.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      737 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-span-strike.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1413 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-span-texttransform.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      765 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-span-underline.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      712 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-span.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      925 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-strike.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      973 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-underline.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1517 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-wordWrap.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1376 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1082 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-path.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3008 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pieChart.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2482 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pieChart3d.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2021 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-place.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      688 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-plugInFlowable.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      464 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-plugInGraphic.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      510 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pre.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2944 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pto.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      454 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-rectange.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      787 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-registerCidFont.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      667 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-registerTTFont-builtins.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      811 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-registerTTFont.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      729 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-registerType1Face.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      403 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-rotate.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      608 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-saveState-restoreState.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      406 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-scale.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      947 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-selectField.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      342 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-setFont.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      430 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-setFontSize.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      817 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-setNextFrame.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      931 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-setNextTemplate.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      406 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-skew.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      827 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-spacer.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2546 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-spiderChart.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1108 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-storyPlace.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      305 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-stroke.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      428 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-textAnnotation.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      750 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-textField.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      459 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-transform.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      414 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-translate.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9866 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-ul-ol-li.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      686 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-xpre.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      857 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/text-not-in-tags.rml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1506 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/input/zope3logo.gif
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3392 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/module.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1485 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/test_directive.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1339 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/test_dtd.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3886 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/test_num2words.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      853 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/test_pagetemplate.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1015 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/test_reference.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6729 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/test_rml.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2043 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/test_rml2pdf.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2286 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/src/z3c/rml/tests/test_subprocess.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-25 15:24:08.177793 z3c.rml-4.3.0/src/z3c.rml.egg-info/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    23661 2023-04-25 15:24:08.000000 z3c.rml-4.3.0/src/z3c.rml.egg-info/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    18797 2023-04-25 15:24:08.000000 z3c.rml-4.3.0/src/z3c.rml.egg-info/SOURCES.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-04-25 15:24:08.000000 z3c.rml-4.3.0/src/z3c.rml.egg-info/dependency_links.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      108 2023-04-25 15:24:08.000000 z3c.rml-4.3.0/src/z3c.rml.egg-info/entry_points.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        4 2023-04-25 15:24:08.000000 z3c.rml-4.3.0/src/z3c.rml.egg-info/namespace_packages.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-04-25 15:24:08.000000 z3c.rml-4.3.0/src/z3c.rml.egg-info/not-zip-safe
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      205 2023-04-25 15:24:08.000000 z3c.rml-4.3.0/src/z3c.rml.egg-info/requires.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        4 2023-04-25 15:24:08.000000 z3c.rml-4.3.0/src/z3c.rml.egg-info/top_level.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1376 2023-04-25 15:24:07.000000 z3c.rml-4.3.0/tox.ini
```

### Comparing `z3c.rml-4.2.1/CHANGES.rst` & `z3c.rml-4.3.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,31 @@
 =======
 CHANGES
 =======
 
+4.3.0 (2023-04-25)
+------------------
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Added support for text anchor points on images.
+
+- Make sure we only close input files if we opened them.
+
+- Delegate image ratio to drawImage. (PR #105)
+
+- Accepts "None" for label box colors.
+
+- Use svglib for the svg to rml conversion instead of maintaining our own.
+
+- Allow unicode characters as bullets.
+
+
 4.2.1 (2022-09-30)
 ------------------
 
 - Add support for Python 3.10.
 
 - Add back support for Python 3.6.
```

### Comparing `z3c.rml-4.2.1/CONTRIBUTING.md` & `z3c.rml-4.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/LICENSE.txt` & `z3c.rml-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/RML-DIFFERENCES.rst` & `z3c.rml-4.3.0/RML-DIFFERENCES.rst`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/setup.py` & `z3c.rml-4.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,37 +29,37 @@
     'zope.pagetemplate',
     'zope.testrunner',
 ]
 
 
 setup(
     name="z3c.rml",
-    version='4.2.1',
+    version='4.3.0',
     author="Stephan Richter and the Zope Community",
-    author_email="zope-dev@zope.org",
+    author_email="zope-dev@zope.dev",
     description="An alternative implementation of RML",
     long_description=(
         read('README.rst')
         + '\n\n' +
         read('CHANGES.rst')
     ),
     license="ZPL 2.1",
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     keywords="rml reportlab pdf pagetemplate",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Natural Language :: English',
         'Operating System :: OS Independent',
     ],
     url='https://github.com/zopefoundation/z3c.rml',
     packages=find_packages('src'),
     package_dir={'': 'src'},
@@ -72,14 +72,15 @@
     install_requires=[
         'Pygments',
         'backports.tempfile',
         'lxml',
         'pikepdf>=3.0',
         'reportlab>=3.5.0',
         'setuptools',
+        'svglib',
         'zope.interface',
         'zope.schema',
     ],
     entry_points={
         'console_scripts': [
             'rml2pdf = z3c.rml.rml2pdf:main',
             'dtd = z3c.rml.dtd:main',
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/README.txt` & `z3c.rml-4.3.0/src/z3c/rml/README.txt`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/attr.py` & `z3c.rml-4.3.0/src/z3c/rml/attr.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,17 +452,14 @@
         # Under Python 3 all platforms need a protocol for local files
         if not urllib.parse.urlparse(value).scheme:
             value = 'file:///' + os.path.abspath(value)
         # If the file is not to be opened, simply return the path.
         if self.doNotOpen:
             return value
         # Open/Download the file
-        # We can't use urlopen directly because it has problems with data URIs
-        # in 2.7 and 3.3 which are resolved in 3.4. Fortunately Reportlab
-        # already has a utility function to help us work around this issue.
         fileObj = reportlab.lib.utils.open_for_read(value)
         sio = io.BytesIO(fileObj.read())
         fileObj.close()
         sio.seek(0)
         return sio
 
 
@@ -499,23 +496,28 @@
         if cache_key in manager.svgs:
             return manager.svgs[cache_key]
 
         from gzip import GzipFile
         from xml.etree import cElementTree
 
         from reportlab.graphics import renderPM
-
-        from z3c.rml.svg2rlg import Renderer
+        from svglib.svglib import SvgRenderer
 
         fileObj = super().fromUnicode(value)
         svg = fileObj.getvalue()
         if svg[:2] == b'\037\213':
-            svg = GzipFile(fileobj=fileObj).read()
-        svg = cElementTree.fromstring(svg)
-        svg = Renderer(value).render(svg)
+            fileObj = GzipFile(fileobj=fileObj)
+        parser = etree.XMLParser(
+            remove_comments=True,
+            recover=True,
+            resolve_entities=False)
+        svg = cElementTree.parse(fileObj, parser=parser).getroot()
+
+        renderer = SvgRenderer(value)
+        svg = renderer.render(svg)
 
         if preserve:
             if width is not None or height is not None:
                 if width is not None and height is None:
                     height = svg.height * width / svg.width
                 elif height is not None and width is None:
                     width = svg.width * height / svg.height
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/canvas.py` & `z3c.rml-4.3.0/src/z3c/rml/canvas.py`

 * *Files 3% similar despite different names*

```diff
@@ -372,40 +372,32 @@
         title='Mask',
         description='The color mask used to render the image, or "auto" to use'
                     ' the alpha channel if available.',
         default='auto',
         required=False,
         acceptAuto=True)
 
+    anchor = attr.Choice(
+        title='Text Anchor',
+        description='The position in the text to which the coordinates refer.',
+        choices='''nw   n   ne
+                w    c    e
+                sw   s   se'''.split(),
+        required=False)
+
 
 class Image(CanvasRMLDirective):
     signature = IImage
     callable = 'drawImage'
     attrMapping = {'file': 'image'}
 
     def process(self):
         kwargs = dict(self.getAttributeValues(attrMapping=self.attrMapping))
-        preserve = kwargs.pop('preserveAspectRatio')
         show = kwargs.pop('showBoundary')
 
-        if preserve:
-            imgX, imgY = kwargs['image'].getSize()
-
-            # Scale image correctly, if width and/or height were specified
-            if 'width' in kwargs and 'height' not in kwargs:
-                kwargs['height'] = imgY * kwargs['width'] / imgX
-            elif 'height' in kwargs and 'width' not in kwargs:
-                kwargs['width'] = imgX * kwargs['height'] / imgY
-            elif 'width' in kwargs and 'height' in kwargs:
-                if float(kwargs['width']) / \
-                        kwargs['height'] > float(imgX) / imgY:
-                    kwargs['width'] = imgX * kwargs['height'] / imgY
-                else:
-                    kwargs['height'] = imgY * kwargs['width'] / imgX
-
         canvas = attr.getManager(self, interfaces.ICanvasManager).canvas
         getattr(canvas, self.callable)(**kwargs)
 
         if show:
             width = kwargs.get('width', kwargs['image'].getSize()[0])
             height = kwargs.get('height', kwargs['image'].getSize()[1])
             canvas.rect(kwargs['x'], kwargs['y'], width, height)
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/chart.py` & `z3c.rml-4.3.0/src/z3c/rml/chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,24 +289,26 @@
             'autox',
             'autoy'),
         required=False)
 
     boxStrokeColor = attr.Color(
         title='Box Stroke Color',
         description=('The color of the box border line.'),
+        acceptNone=True,
         required=False)
 
     boxStrokeWidth = attr.Measurement(
         title='Box Stroke Width',
         description='The width of the box border line.',
         required=False)
 
     boxFillColor = attr.Color(
         title='Box Fill Color',
         description=('The color in which the box is filled.'),
+        acceptNone=True,
         required=False)
 
     boxTarget = attr.Text(
         title='Box Target',
         description='The box target.',
         required=False)
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/directive.py` & `z3c.rml-4.3.0/src/z3c/rml/directive.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/doclogic.py` & `z3c.rml-4.3.0/src/z3c/rml/doclogic.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/document.py` & `z3c.rml-4.3.0/src/z3c/rml/document.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/dtd.py` & `z3c.rml-4.3.0/src/z3c/rml/dtd.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     subElementList = ' | '.join(subElementList)
     if subElementList:
         subElementList = ' (' + subElementList + ')'
         if '#PCDATA' in subElementList:
             subElementList += occurence
     else:
         subElementList = ' EMPTY'
-    text = '\n<!ELEMENT %s%s>' % (name, subElementList)
+    text = '\n<!ELEMENT {}{}>'.format(name, subElementList)
     # Create a list of attributes for this element.
     for attrName, field in fields:
         # Ignore text nodes, since they are not attributes.
         if isinstance(field, attr.TextNode):
             continue
         # Create the type
         if isinstance(field, attr.Choice):
@@ -69,20 +69,20 @@
             type = 'CDATA'
         # Create required flag
         if field.required:
             required = '#REQUIRED'
         else:
             required = '#IMPLIED'
         # Put it all together
-        text += '\n<!ATTLIST %s %s %s %s>' % (name, attrName, type, required)
+        text += f'\n<!ATTLIST {name} {attrName} {type} {required}>'
     text += '\n'
     # DTD does not support redefinition of an element type or have context
     # specific elements.
     if (name, signature) in seen:
-        text = '\n<!--' + text + '-->\n'
+        text = f'\n<!--{text}-->\n'
     seen.append((name, signature))
     # Walk through all sub-elements, creating the DTD entries for them.
     for occurence in signature.queryTaggedValue('directives', ()):
         if (occurence.tag, occurence.signature) in seen:
             continue
         text += generateElement(occurence.tag, occurence.signature, seen)
     return text
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/flowable.py` & `z3c.rml-4.3.0/src/z3c/rml/flowable.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/form.py` & `z3c.rml-4.3.0/src/z3c/rml/form.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/interfaces.py` & `z3c.rml-4.3.0/src/z3c/rml/interfaces.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/list.py` & `z3c.rml-4.3.0/src/z3c/rml/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,18 +77,21 @@
 class OrderedListItem(ListItem):
     signature = IOrderedListItem
 
 
 class IUnorderedListItem(IListItem):
     """An ordered list item."""
 
-    value = attr.Choice(
+    value = attr.Combination(
         title='Bullet Value',
         description='The type of bullet character.',
-        choices=interfaces.UNORDERED_BULLET_VALUES,
+        value_types=(
+            attr.Choice(choices=interfaces.UNORDERED_BULLET_VALUES),
+            attr.Text(max_length=1)
+        ),
         required=False)
 
 
 class UnorderedListItem(ListItem):
     signature = IUnorderedListItem
 
     styleAttributes = ListItem.styleAttributes + ['value']
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/num2words.py` & `z3c.rml-4.3.0/src/z3c/rml/num2words.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/occurence.py` & `z3c.rml-4.3.0/src/z3c/rml/occurence.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/page.py` & `z3c.rml-4.3.0/src/z3c/rml/page.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/pagetemplate.py` & `z3c.rml-4.3.0/src/z3c/rml/pagetemplate.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/pagetemplate.txt` & `z3c.rml-4.3.0/src/z3c/rml/pagetemplate.txt`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/paraparser.py` & `z3c.rml-4.3.0/src/z3c/rml/paraparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,14 @@
 
         # ReportLab 3.4.0 introduced caching to Paragraph which breaks how
         # we've implemented lookaheads. To get around it we need to bust the
         # cache when dynamic tags are used.
 
         unprocessed_frags = self.frags
         bust_cache = any(isinstance(f, ParaFragWrapper) for f in self.frags)
-        # Paragraph is an old-style class in Python 2 so we can't use super()
         result = super().breakLines(*args, **kwargs)
         if bust_cache:
             self.frags = unprocessed_frags
         return result
 
 
 class ImageReader(reportlab.lib.utils.ImageReader):
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/pdfinclude.py` & `z3c.rml-4.3.0/src/z3c/rml/pdfinclude.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             for (prs, pre) in page_ranges:
                 # pdftk uses lower and upper bound inclusive.
                 merges.append('%s%i-%i' % (file_letter, prs + 1, pre))
 
         mergedFile = os.path.join(dir, 'merged.pdf')
         do('{} {} cat {} output {}'.format(
             self.EXECUTABLE,
-            ' '.join('{}="{}"'.format(l_, p) for l_, p in file_map.items()),
+            ' '.join(f'{l_}="{p}"' for l_, p in file_map.items()),
             ' '.join(merges),
             mergedFile))
 
         if not self.PRESERVE_OUTLINE:
             with open(mergedFile, 'rb') as file:
                 return io.BytesIO(file.read())
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/platypus.py` & `z3c.rml-4.3.0/src/z3c/rml/platypus.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                  fakeWidth=None):
 
         self.name = name
         self.maxWidth = maxWidth
         self.maxHeight = maxHeight
         self.mode = mode
         assert mode in ('error', 'overflow', 'shrink', 'truncate'), \
-            '{} invalid mode value {}'.format(self.identity(), mode)
+            f'{self.identity()} invalid mode value {mode}'
         # This is an unnecessary check, since wrap() handles None just fine!
         # assert maxHeight>=0,  \
         #       '%s invalid maxHeight value %s' % (self.identity(),maxHeight)
         if mergeSpace is None:
             mergeSpace = overlapAttachedSpace
         self.mergespace = mergeSpace
         self._content = content or []
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/reference.pt` & `z3c.rml-4.3.0/src/z3c/rml/reference.pt`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/reference.py` & `z3c.rml-4.3.0/src/z3c/rml/reference.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,33 +112,33 @@
 
 def formatField(field):
     return field.__class__.__name__
 
 
 def formatChoice(field):
     choices = ', '.join([repr(choice) for choice in field.choices.keys()])
-    return '%s of (%s)' % (field.__class__.__name__, choices)
+    return '{} of ({})'.format(field.__class__.__name__, choices)
 
 
 def formatSequence(field):
     vtFormatter = typeFormatters.get(field.value_type.__class__, formatField)
-    return '%s of %s' % (field.__class__.__name__,
-                         vtFormatter(field.value_type))
+    return '{} of {}'.format(
+        field.__class__.__name__, vtFormatter(field.value_type))
 
 
 def formatGrid(field):
     vtFormatter = typeFormatters.get(field.value_type.__class__, formatField)
     return '%s with %i cols of %s' % (
         field.__class__.__name__, field.columns, vtFormatter(field.value_type))
 
 
 def formatCombination(field):
     vts = [typeFormatters.get(vt.__class__, formatField)(vt)
            for vt in field.value_types]
-    return '%s of %s' % (field.__class__.__name__, ', '.join(vts))
+    return '{} of {}'.format(field.__class__.__name__, ', '.join(vts))
 
 
 typeFormatters = {
     attr.Choice: formatChoice,
     attr.Sequence: formatSequence,
     attr.Combination: formatCombination,
     attr.TextNodeSequence: formatSequence,
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/rlfix.py` & `z3c.rml-4.3.0/src/z3c/rml/rlfix.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/rml-reference.pdf` & `z3c.rml-4.3.0/src/z3c/rml/rml-reference.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/rml.dtd` & `z3c.rml-4.3.0/src/z3c/rml/rml.dtd`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/rml2pdf.py` & `z3c.rml-4.3.0/src/z3c/rml/rml2pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,47 +42,44 @@
     output = io.BytesIO()
     doc.process(output)
     output.seek(0)
     return output
 
 
 def go(xmlInputName, outputFileName=None, outDir=None, dtdDir=None):
-    if dtdDir is not None:
-        sys.stderr.write('The ``dtdDir`` option is not yet supported.\n')
-
     if hasattr(xmlInputName, 'read'):
         # it is already a file-like object
         xmlFile = xmlInputName
         xmlInputName = 'input.pdf'
     else:
-        xmlFile = open(xmlInputName, 'rb')
-    root = etree.parse(xmlFile).getroot()
-    doc = document.Document(root)
-    doc.filename = xmlInputName
+        with open(xmlInputName, 'rb') as xmlFile:
+            return go(xmlFile, outputFileName, outDir, dtdDir)
 
+    # If an output filename is specified, create an output file for it
     outputFile = None
-
-    # If an output filename is specified, create an output filepointer for it
     if outputFileName is not None:
         if hasattr(outputFileName, 'write'):
             # it is already a file-like object
             outputFile = outputFileName
             outputFileName = 'output.pdf'
         else:
             if outDir is not None:
                 outputFileName = os.path.join(outDir, outputFileName)
-            outputFile = open(outputFileName, 'wb')
+            with open(outputFileName, 'wb') as outputFile:
+                return go(xmlFile, outputFile, outDir, dtdDir)
+
+    if dtdDir is not None:
+        sys.stderr.write('The ``dtdDir`` option is not yet supported.\n')
+
+    root = etree.parse(xmlFile).getroot()
+    doc = document.Document(root)
+    doc.filename = xmlInputName
 
     # Create a Reportlab canvas by processing the document
-    try:
-        doc.process(outputFile)
-    finally:
-        if outputFile:
-            outputFile.close()
-        xmlFile.close()
+    doc.process(outputFile)
 
 
 def main(args=None):
     if args is None:
         parser = argparse.ArgumentParser(
             prog='rml2pdf',
             description='Converts file in RML format into PDF file.',
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/rml2pdfscript.py` & `z3c.rml-4.3.0/src/z3c/rml/rml2pdfscript.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/special.py` & `z3c.rml-4.3.0/src/z3c/rml/special.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/storyplace.py` & `z3c.rml-4.3.0/src/z3c/rml/storyplace.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/stylesheet.py` & `z3c.rml-4.3.0/src/z3c/rml/stylesheet.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/template.py` & `z3c.rml-4.3.0/src/z3c/rml/template.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/encoding-test-latin1.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/encoding-test-latin1.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/encoding-test-utf8.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/encoding-test-utf8.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/printScaling.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/printScaling.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-000-simple.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-000-simple.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-001-cmbox.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-001-cmbox.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-001-hello.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-001-hello.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-002-paras.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-002-paras.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-003-frames.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-003-frames.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-004-fpt-templates.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-004-fpt-templates.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-004-templates.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-004-templates.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-005-fonts.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-005-fonts.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-006-barcodes.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-006-barcodes.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-008-tables.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-008-tables.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-009-splitting.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-009-splitting.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-010-linkURL.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-010-linkURL.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-011-keepwithnext.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-011-keepwithnext.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-017-outlines.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-017-outlines.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-022-paras-oas.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-022-paras-oas.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-029-keepinframe.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-029-keepinframe.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-031-japanese.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-031-japanese.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-032-images.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-032-images.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-034-cmyk.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-034-cmyk.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-035-numbering.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-035-numbering.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-036-numbering-contd.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-036-numbering-contd.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-037-plugingraphic.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-037-plugingraphic.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-038-rect-href.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-038-rect-href.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-039-doc-programming.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-039-doc-programming.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-040-colors.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-040-colors.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-041-masking.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-041-masking.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-042-longdoc.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-042-longdoc.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-043-headings.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-043-headings.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-044-codesnippets.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-044-codesnippets.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-045-cmyk.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-045-cmyk.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-046-lists.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-046-lists.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-047-condPageBreak.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-047-condPageBreak.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-048-paragraph-flow-controls.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-048-paragraph-flow-controls.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-049-pre.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-049-pre.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-examples-050-header-footer.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-examples-050-header-footer.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-01.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-01.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-02.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-02.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-03.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-03.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-04.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-04.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-05.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-05.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-06.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-06.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-07.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-07.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-08.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-08.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-09.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-09.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-10.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-10.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-11.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-11.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/rml-guide-example-12.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/rml-guide-example-12.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/sample-shipment-chinese.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/sample-shipment-chinese.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/simple-layout.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/simple-layout.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/special-text.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/special-text.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/symbols-set.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/symbols-set.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-addMapping.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-addMapping.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-alias.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-alias.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-barChart.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-barChart.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-barChart3d.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-barChart3d.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-barCodeFlowable.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-barCodeFlowable.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-barcode.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-barcode.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockNosplit.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockNosplit.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-1.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-1.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-10.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-10.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-2.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-2.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-3.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-3.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-4.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-4.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-5.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-5.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-6.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-6.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-7.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-7.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-8.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-8.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-9.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-9.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTable-bulkData.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTable-bulkData.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTableStyle-2.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTableStyle-2.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTableStyle-3.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTableStyle-3.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-blockTableStyle.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-blockTableStyle.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-bookmark.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-bookmark.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-buttonField.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-buttonField.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-circle.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-circle.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-codesnippet.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-codesnippet.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-color.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-color.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-condPageBreak.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-condPageBreak.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-cropMarks.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-cropMarks.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-curves.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-curves.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-doc.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-doc.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-docinit-viewer-options.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-docinit-viewer-options.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-document-annotations.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-document-annotations.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-document-pageDrawing.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-document-pageDrawing.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-document-story.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-document-story.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-drawAlignedString.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-drawAlignedString.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-drawCenteredString.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-drawCenteredString.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-drawRightString.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-drawRightString.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-drawString.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-drawString.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-ellipse.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-ellipse.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-fill.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-fill.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-fixedSize.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-fixedSize.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-grid.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-grid.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-hr.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-hr.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-illustration.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-illustration.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-image-1.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-image-1.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-image-data-uri.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-image-data-uri.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-image-mask.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-image-mask.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-image-svg.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-image-svg.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-image.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-image.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-imageAndFlowables-svg.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-imageAndFlowables-svg.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-imageAndFlowables.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-imageAndFlowables.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-img.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-img.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-includePdfPages-edge-dupekey.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-includePdfPages-edge-dupekey.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-includePdfPages-firstPage.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-includePdfPages-firstPage.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-includePdfPages-noAdditionalText.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-includePdfPages-noAdditionalText.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-includePdfPages.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-includePdfPages.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-indent.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-indent.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-index.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-index.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-keepInFrame.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-keepInFrame.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-keepTogether.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-keepTogether.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-lineMode.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-lineMode.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-linePlot.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-linePlot.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-linePlot3D.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-linePlot3D.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-lines.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-lines.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-log.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-log.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-mergePage-2.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-mergePage-2.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-mergePage.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-mergePage.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-name.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-name.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-nextFrame.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-nextFrame.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-nextPage.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-nextPage.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-outlineAdd.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-outlineAdd.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pageGraphics.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pageGraphics.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pageInfo-2.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pageInfo-2.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pageInfo.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pageInfo.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pageNumber.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pageNumber.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-border.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-border.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-comment.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-comment.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-span-strike.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-span-strike.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-span-texttransform.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-span-texttransform.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-span-underline.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-span-underline.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-span.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-span.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-strike.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-strike.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-underline.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-underline.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para-wordWrap.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para-wordWrap.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-para.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-para.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-path.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-path.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pdfInclude-noAdditionalText.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pdfInclude-noAdditionalText.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pieChart.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pieChart.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pieChart3d.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pieChart3d.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-place.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-place.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-plugInFlowable.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-plugInFlowable.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-plugInGraphic.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-plugInGraphic.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pre.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pre.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-pto.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-pto.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-rectange.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-rectange.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-registerCidFont.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-registerCidFont.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-registerTTFont-builtins.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-registerTTFont-builtins.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-registerTTFont.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-registerTTFont.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-registerType1Face.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-registerType1Face.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-rotate.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-rotate.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-saveState-restoreState.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-saveState-restoreState.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-scale.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-scale.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-selectField.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-selectField.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-setFont.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-setFont.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-setFontSize.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-setFontSize.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-setNextFrame.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-setNextFrame.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-setNextTemplate.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-setNextTemplate.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-skew.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-skew.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-spacer.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-spacer.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-spiderChart.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-spiderChart.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-storyPlace.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-storyPlace.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-stroke.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-stroke.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-textAnnotation.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-textAnnotation.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-textField.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-textField.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-transform.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-transform.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-translate.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-translate.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-ul-ol-li.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-ul-ol-li.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/tag-xpre.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/tag-xpre.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/expected/text-not-in-tags.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/expected/text-not-in-tags.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/flowable.py` & `z3c.rml-4.3.0/src/z3c/rml/tests/flowable.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/400x200.gif` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/400x200.gif`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/Vera.ttf` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/Vera.ttf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/VeraMono.ttf` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/VeraMono.ttf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/data/bad1-dupekey.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/data/bad1-dupekey.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/data/fw2.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/data/fw2.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/data/include-bookmarks1.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/data/include-bookmarks1.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/data/include-bookmarks2.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/data/include-bookmarks2.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/data/include1.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/data/include1.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/data/include2.pdf` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/data/include2.pdf`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/encoding-test-latin1.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/encoding-test-latin1.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/encoding-test-utf8.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/encoding-test-utf8.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/images/cylinder.eps` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/images/cylinder.eps`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/images/cylinder.png` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/images/cylinder.png`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/images/cylinder.svg` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/images/cylinder.svg`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/images/cylinder.svgz` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/images/cylinder.svgz`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/images/replogo.gif` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/images/replogo.gif`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/logo_no_bar.png` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/logo_no_bar.png`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-001-cmbox.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-001-cmbox.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-001-hello.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-001-hello.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-002-paras.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-002-paras.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-003-frames.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-003-frames.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-004-fpt-templates.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-004-fpt-templates.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-004-templates.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-004-templates.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-005-fonts.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-005-fonts.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-006-barcodes.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-006-barcodes.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-008-tables.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-008-tables.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-009-splitting.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-009-splitting.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-010-linkURL.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-010-linkURL.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-011-keepwithnext.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-011-keepwithnext.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-017-outlines.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-017-outlines.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-022-paras-oas.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-022-paras-oas.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-029-keepinframe.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-029-keepinframe.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-031-japanese.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-031-japanese.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-032-images.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-032-images.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-034-cmyk.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-034-cmyk.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-035-numbering.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-035-numbering.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-036-numbering-contd.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-036-numbering-contd.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-037-plugingraphic.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-037-plugingraphic.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-038-rect-href.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-038-rect-href.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-039-doc-programming.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-039-doc-programming.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-040-colors.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-040-colors.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-041-masking.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-041-masking.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-042-longdoc.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-042-longdoc.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-043-headings.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-043-headings.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-044-codesnippets.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-044-codesnippets.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-045-cmyk.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-045-cmyk.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-046-lists.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-046-lists.rml`

 * *Files 1% similar despite different names*

#### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-046-lists.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-046-lists.rml`

```diff
@@ -264,10 +264,19 @@
       <li>
         <para style="normal">para 2</para>
         <para style="normal">another paragraph</para>
       </li>
       <li value="circle" bulletColor="green">
         <para style="normal">para 3</para>
       </li>
+      <li value="❍">
+        <para style="normal">Disc</para>
+      </li>
+      <li value="rarrowhead">
+        <para style="normal">Right arrow head</para>
+      </li>
+      <li value="•">
+        <para style="normal">Bullet, defined by unicode code point</para>
+      </li>
     </ul>
   </story>
 </document>
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-047-condPageBreak.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-047-condPageBreak.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-048-paragraph-flow-controls.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-048-paragraph-flow-controls.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-049-pre.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-049-pre.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-examples-050-header-footer.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-examples-050-header-footer.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-02.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-02.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-03.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-03.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-04.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-04.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-05.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-05.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-06.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-06.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-07.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-07.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-08.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-08.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-09.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-09.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-10.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-10.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-11.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-11.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/rml-guide-example-12.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/rml-guide-example-12.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/simple-layout.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/simple-layout.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/special-text.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/special-text.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/strapline.png` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/strapline.png`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/symbols-set.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/symbols-set.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-addMapping.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-addMapping.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-alias.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-alias.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-barChart.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-barChart.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-barChart3d.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-barChart3d.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-barCodeFlowable.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-barCodeFlowable.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-barcode.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-barcode.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockNosplit.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockNosplit.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-1.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-1.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-10.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-10.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-2.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-2.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-3.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-3.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-4.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-4.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-5.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-5.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-6.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-6.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-7.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-7.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-8.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-8.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-9.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-9.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTable-bulkData.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTable-bulkData.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTableStyle-2.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTableStyle-2.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTableStyle-3.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTableStyle-3.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-blockTableStyle.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-blockTableStyle.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-bookmark.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-bookmark.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-circle.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-circle.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-codesnippet.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-codesnippet.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-color.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-color.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-condPageBreak.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-condPageBreak.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-cropMarks.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-cropMarks.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-doc.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-doc.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-docinit-viewer-options.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-docinit-viewer-options.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-document-annotations.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-document-annotations.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-drawAlignedString.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-drawAlignedString.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-ellipse.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-ellipse.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-fixedSize.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-fixedSize.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-hr.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-hr.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-illustration.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-illustration.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-image-1.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-image-1.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-image-data-uri.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-image-data-uri.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-image-mask.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-image-mask.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-image-svg.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-image-svg.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-image.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-image.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-imageAndFlowables-svg.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-imageAndFlowables-svg.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-imageAndFlowables.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-imageAndFlowables.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-img.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-img.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-includePdfPages-firstPage.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-includePdfPages-firstPage.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-includePdfPages-noAdditionalText.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-includePdfPages-noAdditionalText.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-includePdfPages.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-includePdfPages.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-indent.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-indent.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-index.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-index.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-keepInFrame.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-keepInFrame.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-keepTogether.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-keepTogether.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-linePlot.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-linePlot.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-linePlot3D.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-linePlot3D.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-log.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-log.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-mergePage-2.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-mergePage-2.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-mergePage.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-mergePage.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-name.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-name.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-nextPage.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-nextPage.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-outlineAdd.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-outlineAdd.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pageGraphics.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pageGraphics.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pageNumber.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pageNumber.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-border.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-border.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-span-strike.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-span-strike.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-span-texttransform.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-span-texttransform.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-span-underline.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-span-underline.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-span.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-span.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-strike.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-strike.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-underline.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-underline.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para-wordWrap.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para-wordWrap.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-para.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-para.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-path.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-path.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pieChart.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pieChart.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pieChart3d.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pieChart3d.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-place.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-place.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-plugInFlowable.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-plugInFlowable.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-pto.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-pto.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-registerCidFont.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-registerCidFont.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-registerTTFont-builtins.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-registerTTFont-builtins.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-registerTTFont.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-registerTTFont.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-registerType1Face.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-registerType1Face.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-saveState-restoreState.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-saveState-restoreState.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-selectField.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-selectField.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-setNextFrame.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-setNextFrame.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-setNextTemplate.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-setNextTemplate.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-spacer.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-spacer.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-spiderChart.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-spiderChart.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-storyPlace.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-storyPlace.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-textField.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-textField.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-ul-ol-li.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-ul-ol-li.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/tag-xpre.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/tag-xpre.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/text-not-in-tags.rml` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/text-not-in-tags.rml`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/input/zope3logo.gif` & `z3c.rml-4.3.0/src/z3c/rml/tests/input/zope3logo.gif`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/module.py` & `z3c.rml-4.3.0/src/z3c/rml/tests/module.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/test_directive.py` & `z3c.rml-4.3.0/src/z3c/rml/tests/test_directive.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/test_dtd.py` & `z3c.rml-4.3.0/src/z3c/rml/tests/test_dtd.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/test_num2words.py` & `z3c.rml-4.3.0/src/z3c/rml/tests/test_num2words.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/test_pagetemplate.py` & `z3c.rml-4.3.0/src/z3c/rml/tests/test_pagetemplate.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/test_reference.py` & `z3c.rml-4.3.0/src/z3c/rml/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/test_rml.py` & `z3c.rml-4.3.0/src/z3c/rml/tests/test_rml.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,21 @@
 import logging
 import os
 import subprocess
 import sys
 import tempfile
 import unittest
 
+from PIL import Image
+from PIL import ImageChops
+
 import z3c.rml.tests
 from z3c.rml import rml2pdf
 
 
-try:
-    import Image
-    import ImageChops
-except ImportError:
-    from PIL import Image
-    from PIL import ImageChops
-
 LOG_FILE = os.path.join(os.path.dirname(__file__), 'render.log')
 
 
 def gs_command(path):
     return ('gs', '-q', '-sNOPAUSE', '-sDEVICE=png256',
             '-sOutputFile=%s[Page-%%d].png' % path[:-4],
             path, '-c', 'quit')
@@ -179,15 +175,15 @@
         print("ghostscript:")
         os.system("gs --version")
 
     suite = unittest.TestSuite()
     here = os.path.dirname(z3c.rml.tests.__file__)
     inputDir = os.path.join(here, 'input')
     outputDir = tempfile.mkdtemp('z3c.rml-output')
-    print('output dir: {}'.format(outputDir))
+    print(f'output dir: {outputDir}')
     expectDir = os.path.join(here, 'expected')
     for filename in os.listdir(inputDir):
         if not filename.endswith(".rml"):
             continue
 
         inPath = os.path.join(inputDir, filename)
         outPath = os.path.join(outputDir, filename[:-4] + '.pdf')
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/test_rml2pdf.py` & `z3c.rml-4.3.0/src/z3c/rml/tests/test_rml2pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 #
 ##############################################################################
 """Test RML to PDF converter.
 """
 
 import io
 import unittest
-
-import mock
+from unittest import mock
 
 from z3c.rml import rml2pdf
 
 
 class RML2PDFTest(unittest.TestCase):
 
     @mock.patch("z3c.rml.rml2pdf.go")
```

### Comparing `z3c.rml-4.2.1/src/z3c/rml/tests/test_subprocess.py` & `z3c.rml-4.3.0/src/z3c/rml/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `z3c.rml-4.2.1/src/z3c.rml.egg-info/SOURCES.txt` & `z3c.rml-4.3.0/src/z3c.rml.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -46,28 +46,26 @@
 src/z3c/rml/rml-reference.pdf
 src/z3c/rml/rml.dtd
 src/z3c/rml/rml2pdf.py
 src/z3c/rml/rml2pdfscript.py
 src/z3c/rml/special.py
 src/z3c/rml/storyplace.py
 src/z3c/rml/stylesheet.py
-src/z3c/rml/svg2rlg.py
 src/z3c/rml/template.py
 src/z3c/rml/tests/__init__.py
 src/z3c/rml/tests/flowable.py
 src/z3c/rml/tests/module.py
 src/z3c/rml/tests/test_directive.py
 src/z3c/rml/tests/test_dtd.py
 src/z3c/rml/tests/test_num2words.py
 src/z3c/rml/tests/test_pagetemplate.py
 src/z3c/rml/tests/test_reference.py
 src/z3c/rml/tests/test_rml.py
 src/z3c/rml/tests/test_rml2pdf.py
 src/z3c/rml/tests/test_subprocess.py
-src/z3c/rml/tests/test_svg2rlg.py
 src/z3c/rml/tests/expected/encoding-test-latin1.pdf
 src/z3c/rml/tests/expected/encoding-test-utf8.pdf
 src/z3c/rml/tests/expected/printScaling.pdf
 src/z3c/rml/tests/expected/rml-examples-000-simple.pdf
 src/z3c/rml/tests/expected/rml-examples-001-cmbox.pdf
 src/z3c/rml/tests/expected/rml-examples-001-hello.pdf
 src/z3c/rml/tests/expected/rml-examples-002-paras.pdf
```

### Comparing `z3c.rml-4.2.1/tox.ini` & `z3c.rml-4.3.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py36
     py37
     py38
     py39
     py310
+    py311
     coverage
 
 [testenv]
 usedevelop = true
 deps =
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
@@ -32,14 +32,15 @@
     check-python-versions >= 0.19.1
     wheel
     flake8
     isort
 
 [testenv:isort-apply]
 basepython = python3
+skip_install = true
 commands_pre =
 deps =
     isort
 commands =
     isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:coverage]
@@ -47,16 +48,16 @@
 allowlist_externals =
     mkdir
 deps =
     coverage
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    coverage html
-    coverage report -m --fail-under=82
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=82
 
 [coverage:run]
 branch = True
 source = z3c.rml
 
 [coverage:report]
 precision = 2
```

