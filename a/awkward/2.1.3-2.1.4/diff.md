# Comparing `tmp/awkward-2.1.3.tar.gz` & `tmp/awkward-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Apr 13 15:38:23 2023, max compression
+gzip compressed data, last modified: Mon Apr 24 16:57:22 2023, max compression
```

## Comparing `awkward-2.1.3.tar` & `awkward-2.1.4.tar`

### file list

```diff
@@ -1,838 +1,846 @@
--rw-r--r--   0        0        0     1893 2023-04-13 15:38:23.000000 awkward-2.1.3/CITATION.cff
--rw-r--r--   0        0        0    13578 2023-04-13 15:38:23.000000 awkward-2.1.3/CONTRIBUTING.md
--rw-r--r--   0        0        0    22687 2023-04-13 15:38:23.000000 awkward-2.1.3/README.md
--rw-r--r--   0        0        0      241 2023-04-13 15:38:23.000000 awkward-2.1.3/requirements-test.txt
--rw-r--r--   0        0        0     7833 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_toc.yml
--rw-r--r--   0        0        0     7624 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/conf.py
--rw-r--r--   0        0        0      346 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/environment.yml.cog
--rw-r--r--   0        0        0     2603 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/index.md
--rw-r--r--   0        0        0    11642 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/prepare_docstrings.py
--rw-r--r--   0        0        0     4448 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/redirects-user-guide.json
--rw-r--r--   0        0        0    11436 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/redirects.json
--rw-r--r--   0        0        0      463 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/requirements.txt
--rw-r--r--   0        0        0      369 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/switcher.json
--rw-r--r--   0        0        0      930 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_static/css/awkward.css
--rw-r--r--   0        0        0      354 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_static/css/try-awkward-array.css
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0      469 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_templates/funding.html
--rw-r--r--   0        0        0      474 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_templates/redirect.html
--rw-r--r--   0        0        0     2968 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/getting-started/community-tutorials.md
--rw-r--r--   0        0        0     4654 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/getting-started/index.md
--rw-r--r--   0        0        0     3346 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/getting-started/papers-and-talks.md
--rw-r--r--   0        0        0       82 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/getting-started/try-awkward-array.md
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    12847 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/getting-started/demo/what-is-an-awkward-array.ipynb
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    17067 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/example-hierarchy.svg
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
-lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    25309 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/reference/ak.behavior.rst
--rw-r--r--   0        0        0     1430 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/reference/ak.builder.ArrayBuilder.rst
--rw-r--r--   0        0        0    64727 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/reference/awkwardforth.rst
--rw-r--r--   0        0        0      270 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/reference/index.md
--rw-r--r--   0        0        0     7252 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/reference/toctree.txt
--rw-r--r--   0        0        0     8320 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/10-minutes-to-awkward-array.md
--rw-r--r--   0        0        0      926 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-combinatorics-best-match.md
--rw-r--r--   0        0        0      930 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
--rw-r--r--   0        0        0      263 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-combinatorics.md
--rw-r--r--   0        0        0     8335 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-arrow.md
--rw-r--r--   0        0        0     6392 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-buffers.md
--rw-r--r--   0        0        0     2455 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-json.md
--rw-r--r--   0        0        0    13475 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-numpy.md
--rw-r--r--   0        0        0     7182 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-pandas.md
--rw-r--r--   0        0        0    18830 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-python.md
--rw-r--r--   0        0        0     3554 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-rdataframe.md
--rw-r--r--   0        0        0      271 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert.md
--rw-r--r--   0        0        0    11973 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-arraybuilder.md
--rw-r--r--   0        0        0    36520 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-constructors.md
--rw-r--r--   0        0        0     7383 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-lists.md
--rw-r--r--   0        0        0     7456 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-missing.md
--rw-r--r--   0        0        0    11542 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-records.md
--rw-r--r--   0        0        0     4066 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-strings.md
--rw-r--r--   0        0        0      866 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-unflatten-group.md
--rw-r--r--   0        0        0      267 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create.md
--rw-r--r--   0        0        0      834 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-examine-checking-validity.md
--rw-r--r--   0        0        0     2919 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-examine-list-fields.md
--rw-r--r--   0        0        0      848 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-examine-simple-slicing.md
--rw-r--r--   0        0        0      838 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-examine-single-item.md
--rw-r--r--   0        0        0     6778 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-examine-type.md
--rw-r--r--   0        0        0      269 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-examine.md
--rw-r--r--   0        0        0      844 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-filter-cut-mask.md
--rw-r--r--   0        0        0     3889 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-filter-masked.md
--rw-r--r--   0        0        0      840 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-filter-num.md
--rw-r--r--   0        0        0     7955 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-filter-ragged.md
--rw-r--r--   0        0        0      265 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-filter.md
--rw-r--r--   0        0        0      818 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math-argminmax.md
--rw-r--r--   0        0        0      822 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math-broadcasting.md
--rw-r--r--   0        0        0      828 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math-gpu.md
--rw-r--r--   0        0        0      838 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math-numpy.md
--rw-r--r--   0        0        0      846 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math-reducing.md
--rw-r--r--   0        0        0      870 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math-statistics.md
--rw-r--r--   0        0        0      265 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math.md
--rw-r--r--   0        0        0     3411 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-add-fields.md
--rw-r--r--   0        0        0      842 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-concatenate.md
--rw-r--r--   0        0        0    19083 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-flatten.md
--rw-r--r--   0        0        0     7568 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-pad.md
--rw-r--r--   0        0        0      852 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-rename-records.md
--rw-r--r--   0        0        0      832 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-sort.md
--rw-r--r--   0        0        0     9624 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-zip-project.md
--rw-r--r--   0        0        0      273 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure.md
--rw-r--r--   0        0        0     2599 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-specialize-differentiate-jax.md
--rw-r--r--   0        0        0      870 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-specialize-in-numba.md
--rw-r--r--   0        0        0      838 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-specialize-lorentz.md
--rw-r--r--   0        0        0      874 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-specialize-override-numpy.md
--rw-r--r--   0        0        0      870 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-specialize-subclass.md
--rw-r--r--   0        0        0      277 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-specialize.md
--rw-r--r--   0        0        0    11724 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-use-header-only-layoutbuilder.md
--rw-r--r--   0        0        0      900 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-use-in-numba-arraybuilder.md
--rw-r--r--   0        0        0     9973 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-use-in-numba-cuda.ipynb
--rw-r--r--   0        0        0      900 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-use-in-numba-features.md
--rw-r--r--   0        0        0      279 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-use-in-numba.md
--rw-r--r--   0        0        0      344 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/index.md
--rw-r--r--   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/requirements.txt
--rw-r--r--   0        0        0   367587 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-data-analysts.png
--rw-r--r--   0        0        0   794465 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-data-analysts.svg
--rw-r--r--   0        0        0   140700 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-developers.png
--rw-r--r--   0        0        0   328307 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-developers.svg
--rw-r--r--   0        0        0    73584 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-doxygen.png
--rw-r--r--   0        0        0    58179 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-sphinx.png
--rw-r--r--   0        0        0   127063 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-tutorials-alternate.png
--rw-r--r--   0        0        0   173327 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-tutorials.png
--rw-r--r--   0        0        0    12541 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-1-0-layers.pdf
--rw-r--r--   0        0        0    65246 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-1-0-layers.png
--rw-r--r--   0        0        0    41004 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-1-0-layers.svg
--rw-r--r--   0        0        0    14946 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-timeline.pdf
--rw-r--r--   0        0        0   125180 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-timeline.png
--rw-r--r--   0        0        0    70209 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-timeline.svg
--rw-r--r--   0        0        0   436595 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
--rw-r--r--   0        0        0   426911 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
--rw-r--r--   0        0        0   335955 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip.png
--rw-r--r--   0        0        0   325268 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip.svg
--rw-r--r--   0        0        0   129696 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline.png
--rw-r--r--   0        0        0   120554 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline.svg
--rw-r--r--   0        0        0     5208 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-broadcasting.png
--rw-r--r--   0        0        0    25065 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-broadcasting.svg
--rw-r--r--   0        0        0     5754 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-cartesian.png
--rw-r--r--   0        0        0    32616 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-cartesian.svg
--rw-r--r--   0        0        0     9584 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-combinations.png
--rw-r--r--   0        0        0    39524 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-combinations.svg
--rw-r--r--   0        0        0    10808 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-schematic.png
--rw-r--r--   0        0        0    25779 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-schematic.svg
--rw-r--r--   0        0        0    18178 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    36024 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-hierarchy.png
--rw-r--r--   0        0        0    17092 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-hierarchy.svg
--rw-r--r--   0        0        0    21120 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-reduction-sum-only.svg
--rw-r--r--   0        0        0    29325 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    55553 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-reduction.png
--rw-r--r--   0        0        0    21631 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-reduction.svg
--rw-r--r--   0        0        0    10978 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/git-strategy.pdf
--rw-r--r--   0        0        0    58904 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/git-strategy.png
--rw-r--r--   0        0        0    28990 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/git-strategy.svg
--rw-r--r--   0        0        0   113587 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/how-it-works-muons.png
--rw-r--r--   0        0        0    57471 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/how-it-works-muons.svg
--rw-r--r--   0        0        0    58475 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/how-it-works.svg
--rw-r--r--   0        0        0    63989 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/sorting-axis.svg
--rw-r--r--   0        0        0   124038 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/all.svg
--rw-r--r--   0        0        0   128558 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/any.svg
--rw-r--r--   0        0        0   134490 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/argmax.svg
--rw-r--r--   0        0        0   133192 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/argmin.svg
--rw-r--r--   0        0        0   106277 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/count.svg
--rw-r--r--   0        0        0   116417 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/count_nonzero.svg
--rw-r--r--   0        0        0   111789 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/max.svg
--rw-r--r--   0        0        0   109239 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/min.svg
--rw-r--r--   0        0        0   124702 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/product.svg
--rw-r--r--   0        0        0   108897 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/sum.svg
--rw-r--r--   0        0        0     8347 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/logo/favicon.ico
--rw-r--r--   0        0        0     8984 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0    11964 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24707 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0    18767 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/logo/logo.svg
--rw-r--r--   0        0        0    90413 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/photos/desire-path.jpg
--rw-r--r--   0        0        0    52113 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/plots/awkward-0-popularity.pdf
--rw-r--r--   0        0        0   146109 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/plots/awkward-0-popularity.png
--rw-r--r--   0        0        0   147576 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/plots/awkward-0-popularity.svg
--rw-r--r--   0        0        0    26938 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/plots/bikeroutes-scaling.svg
--rw-r--r--   0        0        0     8891 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/screenshots/github-issues-documentation.png
--rw-r--r--   0        0        0     1325 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/__init__.py
--rw-r--r--   0        0        0     5418 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_behavior.py
--rw-r--r--   0        0        0    38046 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_broadcasting.py
--rw-r--r--   0        0        0    13398 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_do.py
--rw-r--r--   0        0        0    11999 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_errors.py
--rw-r--r--   0        0        0     5672 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_kernels.py
--rw-r--r--   0        0        0     5825 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_layout.py
--rw-r--r--   0        0        0     9983 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_lookup.py
--rw-r--r--   0        0        0     5454 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_parameters.py
--rw-r--r--   0        0        0     9965 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_prettyprint.py
--rw-r--r--   0        0        0    24569 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_reducers.py
--rw-r--r--   0        0        0     2041 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_regularize.py
--rw-r--r--   0        0        0      420 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_singleton.py
--rw-r--r--   0        0        0    23934 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_slicing.py
--rw-r--r--   0        0        0      647 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_typetracer.py
--rw-r--r--   0        0        0     1163 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_typing.py
--rw-r--r--   0        0        0     2439 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_util.py
--rw-r--r--   0        0        0      758 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_v2.py
--rw-r--r--   0        0        0      233 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/builder.py
--rw-r--r--   0        0        0      866 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/cppyy.py
--rw-r--r--   0        0        0      271 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forth.py
--rw-r--r--   0        0        0   103301 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/highlevel.py
--rw-r--r--   0        0        0     8005 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/index.py
--rw-r--r--   0        0        0     3988 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/jax.py
--rw-r--r--   0        0        0     2764 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/numba.py
--rw-r--r--   0        0        0     8272 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/record.py
--rw-r--r--   0        0        0      165 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/typetracer.py
--rw-r--r--   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/__init__.py
--rw-r--r--   0        0        0     1336 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/backend.py
--rw-r--r--   0        0        0     1259 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/cupy.py
--rw-r--r--   0        0        0     3574 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/dispatch.py
--rw-r--r--   0        0        0     1781 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/jax.py
--rw-r--r--   0        0        0      944 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/numpy.py
--rw-r--r--   0        0        0     1902 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/typetracer.py
--rw-r--r--   0        0        0       88 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/__init__.py
--rw-r--r--   0        0        0    32504 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/avro.py
--rw-r--r--   0        0        0    53533 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cling.py
--rw-r--r--   0        0        0      985 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/hist.py
--rw-r--r--   0        0        0     4485 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numexpr.py
--rw-r--r--   0        0        0    10027 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numpy.py
--rw-r--r--   0        0        0    37988 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/pyarrow.py
--rw-r--r--   0        0        0     7038 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/__init__.py
--rw-r--r--   0        0        0     2555 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
--rw-r--r--   0        0        0     4326 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
--rw-r--r--   0        0        0      987 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
--rw-r--r--   0        0        0     2542 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3034 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0      630 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
--rw-r--r--   0        0        0      830 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3196 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
--rw-r--r--   0        0        0     2668 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0      749 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
--rw-r--r--   0        0        0     2749 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
--rw-r--r--   0        0        0      552 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
--rw-r--r--   0        0        0      637 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
--rw-r--r--   0        0        0     2886 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
--rw-r--r--   0        0        0     2904 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3416 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0     3531 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
--rw-r--r--   0        0        0      556 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
--rw-r--r--   0        0        0      695 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3036 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
--rw-r--r--   0        0        0      795 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
--rw-r--r--   0        0        0     2523 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0     2729 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
--rw-r--r--   0        0        0     1035 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
--rw-r--r--   0        0        0      961 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
--rw-r--r--   0        0        0     2593 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
--rw-r--r--   0        0        0     1536 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
--rw-r--r--   0        0        0     1710 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     2012 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1184 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
--rw-r--r--   0        0        0      755 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu
--rw-r--r--   0        0        0      806 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
--rw-r--r--   0        0        0      744 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
--rw-r--r--   0        0        0     1169 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0     1059 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
--rw-r--r--   0        0        0     3208 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
--rw-r--r--   0        0        0      575 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
--rw-r--r--   0        0        0      830 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
--rw-r--r--   0        0        0      650 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
--rw-r--r--   0        0        0     2610 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
--rw-r--r--   0        0        0     1126 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
--rw-r--r--   0        0        0      951 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      721 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
--rw-r--r--   0        0        0     1003 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
--rw-r--r--   0        0        0     1339 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
--rw-r--r--   0        0        0      835 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
--rw-r--r--   0        0        0      975 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
--rw-r--r--   0        0        0      802 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
--rw-r--r--   0        0        0     1123 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu
--rw-r--r--   0        0        0      623 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu
--rw-r--r--   0        0        0      789 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
--rw-r--r--   0        0        0     1040 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     1020 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1045 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      974 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
--rw-r--r--   0        0        0      946 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
--rw-r--r--   0        0        0      980 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
--rw-r--r--   0        0        0      663 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
--rw-r--r--   0        0        0      586 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
--rw-r--r--   0        0        0     2580 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
--rw-r--r--   0        0        0     1360 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
--rw-r--r--   0        0        0      461 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
--rw-r--r--   0        0        0      534 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
--rw-r--r--   0        0        0      529 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
--rw-r--r--   0        0        0      830 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
--rw-r--r--   0        0        0      636 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
--rw-r--r--   0        0        0      689 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0      457 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
--rw-r--r--   0        0        0      830 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
--rw-r--r--   0        0        0     2043 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
--rw-r--r--   0        0        0     2198 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
--rw-r--r--   0        0        0     2043 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
--rw-r--r--   0        0        0     2198 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
--rw-r--r--   0        0        0     3054 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
--rw-r--r--   0        0        0     3289 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
--rw-r--r--   0        0        0     2022 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
--rw-r--r--   0        0        0     2022 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
--rw-r--r--   0        0        0     3202 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
--rw-r--r--   0        0        0     3012 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
--rw-r--r--   0        0        0     3171 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
--rw-r--r--   0        0        0     3439 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
--rw-r--r--   0        0        0     3439 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
--rw-r--r--   0        0        0      865 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
--rw-r--r--   0        0        0      443 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
--rw-r--r--   0        0        0     3195 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
--rw-r--r--   0        0        0     1859 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/header-only/awkward/BuilderOptions.h
--rw-r--r--   0        0        0    19822 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
--rw-r--r--   0        0        0    89307 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
--rw-r--r--   0        0        0      298 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/header-only/awkward/demo_impl.h
--rw-r--r--   0        0        0     8025 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/header-only/awkward/utils.h
--rw-r--r--   0        0        0      239 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/jax/__init__.py
--rw-r--r--   0        0        0     6627 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/jax/reducers.py
--rw-r--r--   0        0        0     5982 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/jax/trees.py
--rw-r--r--   0        0        0       88 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numba/__init__.py
--rw-r--r--   0        0        0    35824 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numba/arrayview.py
--rw-r--r--   0        0        0     1182 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numba/arrayview_cuda.py
--rw-r--r--   0        0        0    31514 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numba/builder.py
--rw-r--r--   0        0        0    12431 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numba/growablebuffer.py
--rw-r--r--   0        0        0    49132 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numba/layout.py
--rw-r--r--   0        0        0       88 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/rdataframe/__init__.py
--rw-r--r--   0        0        0     9377 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/rdataframe/from_rdataframe.py
--rw-r--r--   0        0        0     9922 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/rdataframe/to_rdataframe.py
--rw-r--r--   0        0        0     1487 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
--rw-r--r--   0        0        0     1111 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/__init__.py
--rw-r--r--   0        0        0    12293 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/array_module.py
--rw-r--r--   0        0        0     4939 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/cupy.py
--rw-r--r--   0        0        0     1357 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/dispatch.py
--rw-r--r--   0        0        0     2010 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/jax.py
--rw-r--r--   0        0        0     2922 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/numpy.py
--rw-r--r--   0        0        0    13706 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/numpylike.py
--rw-r--r--   0        0        0     2288 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/shape.py
--rw-r--r--   0        0        0    42477 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/typetracer.py
--rw-r--r--   0        0        0     2527 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/ufuncs.py
--rw-r--r--   0        0        0       88 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/behaviors/__init__.py
--rw-r--r--   0        0        0     3479 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/behaviors/categorical.py
--rw-r--r--   0        0        0     3898 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/behaviors/mixins.py
--rw-r--r--   0        0        0     8509 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/behaviors/string.py
--rw-r--r--   0        0        0      986 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/__init__.py
--rw-r--r--   0        0        0    27803 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/bitmaskedarray.py
--rw-r--r--   0        0        0    40840 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/bytemaskedarray.py
--rw-r--r--   0        0        0    45437 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/content.py
--rw-r--r--   0        0        0    13345 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/emptyarray.py
--rw-r--r--   0        0        0    40347 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/indexedarray.py
--rw-r--r--   0        0        0    63427 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/indexedoptionarray.py
--rw-r--r--   0        0        0    59821 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/listarray.py
--rw-r--r--   0        0        0    85132 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/listoffsetarray.py
--rw-r--r--   0        0        0    49416 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/numpyarray.py
--rw-r--r--   0        0        0    40491 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/recordarray.py
--rw-r--r--   0        0        0    54541 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/regulararray.py
--rw-r--r--   0        0        0    56952 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/unionarray.py
--rw-r--r--   0        0        0    18843 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/unmaskedarray.py
--rw-r--r--   0        0        0      951 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/__init__.py
--rw-r--r--   0        0        0     6081 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/bitmaskedform.py
--rw-r--r--   0        0        0     5368 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/bytemaskedform.py
--rw-r--r--   0        0        0     3369 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/emptyform.py
--rw-r--r--   0        0        0    12450 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/form.py
--rw-r--r--   0        0        0     5638 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/indexedform.py
--rw-r--r--   0        0        0     5133 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/indexedoptionform.py
--rw-r--r--   0        0        0     5621 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/listform.py
--rw-r--r--   0        0        0     4715 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/listoffsetform.py
--rw-r--r--   0        0        0     6004 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/numpyform.py
--rw-r--r--   0        0        0     8208 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/recordform.py
--rw-r--r--   0        0        0     5084 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/regularform.py
--rw-r--r--   0        0        0     7760 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/unionform.py
--rw-r--r--   0        0        0     4229 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/unmaskedform.py
--rw-r--r--   0        0        0     4779 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/__init__.py
--rw-r--r--   0        0        0     3998 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_all.py
--rw-r--r--   0        0        0     5141 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_almost_equal.py
--rw-r--r--   0        0        0     4001 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_any.py
--rw-r--r--   0        0        0     5109 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_argcartesian.py
--rw-r--r--   0        0        0     3819 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_argcombinations.py
--rw-r--r--   0        0        0     6888 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_argmax.py
--rw-r--r--   0        0        0     6845 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_argmin.py
--rw-r--r--   0        0        0     3158 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_argsort.py
--rw-r--r--   0        0        0      952 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_backend.py
--rw-r--r--   0        0        0     9515 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_broadcast_arrays.py
--rw-r--r--   0        0        0     6595 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_broadcast_fields.py
--rw-r--r--   0        0        0    16060 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_cartesian.py
--rw-r--r--   0        0        0     1420 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_categories.py
--rw-r--r--   0        0        0     8118 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_combinations.py
--rw-r--r--   0        0        0    12213 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_concatenate.py
--rw-r--r--   0        0        0     2715 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_copy.py
--rw-r--r--   0        0        0     5817 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_corr.py
--rw-r--r--   0        0        0     5228 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_count.py
--rw-r--r--   0        0        0     4035 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_count_nonzero.py
--rw-r--r--   0        0        0     5170 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_covar.py
--rw-r--r--   0        0        0     4579 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_drop_none.py
--rw-r--r--   0        0        0     1106 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_fields.py
--rw-r--r--   0        0        0     5288 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_fill_none.py
--rw-r--r--   0        0        0     3432 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_firsts.py
--rw-r--r--   0        0        0     7802 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_flatten.py
--rw-r--r--   0        0        0     3154 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_arrow.py
--rw-r--r--   0        0        0      813 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_arrow_schema.py
--rw-r--r--   0        0        0     2727 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_avro_file.py
--rw-r--r--   0        0        0    14453 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_buffers.py
--rw-r--r--   0        0        0     1839 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_categorical.py
--rw-r--r--   0        0        0     1651 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_cupy.py
--rw-r--r--   0        0        0     4111 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_iter.py
--rw-r--r--   0        0        0     1716 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_jax.py
--rw-r--r--   0        0        0    30067 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_json.py
--rw-r--r--   0        0        0     2282 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_numpy.py
--rw-r--r--   0        0        0    11860 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_parquet.py
--rw-r--r--   0        0        0     3324 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_rdataframe.py
--rw-r--r--   0        0        0     2965 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_regular.py
--rw-r--r--   0        0        0     8859 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_full_like.py
--rw-r--r--   0        0        0      873 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_is_categorical.py
--rw-r--r--   0        0        0     2478 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_is_none.py
--rw-r--r--   0        0        0      705 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_is_tuple.py
--rw-r--r--   0        0        0      930 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_is_valid.py
--rw-r--r--   0        0        0     2568 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_isclose.py
--rw-r--r--   0        0        0     9131 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_linear_fit.py
--rw-r--r--   0        0        0     3258 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_local_index.py
--rw-r--r--   0        0        0     4757 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_mask.py
--rw-r--r--   0        0        0     7430 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_max.py
--rw-r--r--   0        0        0     9067 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_mean.py
--rw-r--r--   0        0        0     3568 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_merge_option_of_records.py
--rw-r--r--   0        0        0    12378 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_merge_union_of_records.py
--rw-r--r--   0        0        0     3217 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_metadata_from_parquet.py
--rw-r--r--   0        0        0     7382 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_min.py
--rw-r--r--   0        0        0     4908 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_moment.py
--rw-r--r--   0        0        0     2081 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_nan_to_none.py
--rw-r--r--   0        0        0     5103 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_nan_to_num.py
--rw-r--r--   0        0        0     3874 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_num.py
--rw-r--r--   0        0        0     1951 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_ones_like.py
--rw-r--r--   0        0        0     4362 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_pad_none.py
--rw-r--r--   0        0        0     1786 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_parameters.py
--rw-r--r--   0        0        0     6360 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_prod.py
--rw-r--r--   0        0        0     4710 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_ptp.py
--rw-r--r--   0        0        0     2275 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_ravel.py
--rw-r--r--   0        0        0     9604 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_run_lengths.py
--rw-r--r--   0        0        0     3028 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_singletons.py
--rw-r--r--   0        0        0     3339 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_softmax.py
--rw-r--r--   0        0        0     2670 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_sort.py
--rw-r--r--   0        0        0     8124 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_std.py
--rw-r--r--   0        0        0     3058 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_strings_astype.py
--rw-r--r--   0        0        0    11718 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_sum.py
--rw-r--r--   0        0        0     4931 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_arrow.py
--rw-r--r--   0        0        0     6725 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_arrow_table.py
--rw-r--r--   0        0        0     2370 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_backend.py
--rw-r--r--   0        0        0     6378 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_buffers.py
--rw-r--r--   0        0        0     6050 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_categorical.py
--rw-r--r--   0        0        0     1107 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_cupy.py
--rw-r--r--   0        0        0    13370 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_dataframe.py
--rw-r--r--   0        0        0     1106 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_jax.py
--rw-r--r--   0        0        0    11652 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_json.py
--rw-r--r--   0        0        0     4507 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_layout.py
--rw-r--r--   0        0        0     2612 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_list.py
--rw-r--r--   0        0        0     2123 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_numpy.py
--rw-r--r--   0        0        0     3354 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_packed.py
--rw-r--r--   0        0        0    16968 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_parquet.py
--rw-r--r--   0        0        0     2785 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_rdataframe.py
--rw-r--r--   0        0        0     3347 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_regular.py
--rw-r--r--   0        0        0    23979 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_transform.py
--rw-r--r--   0        0        0     4304 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_type.py
--rw-r--r--   0        0        0     9461 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_unflatten.py
--rw-r--r--   0        0        0     2484 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_unzip.py
--rw-r--r--   0        0        0     1138 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_validity_error.py
--rw-r--r--   0        0        0     2659 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_values_astype.py
--rw-r--r--   0        0        0     9352 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_var.py
--rw-r--r--   0        0        0     5562 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_where.py
--rw-r--r--   0        0        0     5641 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_with_field.py
--rw-r--r--   0        0        0     2610 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_with_name.py
--rw-r--r--   0        0        0     1848 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_with_parameter.py
--rw-r--r--   0        0        0     3756 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_without_field.py
--rw-r--r--   0        0        0     1509 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_without_parameters.py
--rw-r--r--   0        0        0     2134 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_zeros_like.py
--rw-r--r--   0        0        0     8819 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_zip.py
--rw-r--r--   0        0        0      707 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/__init__.py
--rw-r--r--   0        0        0   163323 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/_awkward_datashape_parser.py
--rw-r--r--   0        0        0     1914 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/arraytype.py
--rw-r--r--   0        0        0     2451 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/listtype.py
--rw-r--r--   0        0        0     5652 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/numpytype.py
--rw-r--r--   0        0        0     4180 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/optiontype.py
--rw-r--r--   0        0        0     8067 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/recordtype.py
--rw-r--r--   0        0        0     3133 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/regulartype.py
--rw-r--r--   0        0        0     1105 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/scalartype.py
--rw-r--r--   0        0        0     9622 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/type.py
--rw-r--r--   0        0        0     3725 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/uniontype.py
--rw-r--r--   0        0        0     1937 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/unknowntype.py
--rw-r--r--   0        0        0       88 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/__init__.py
--rw-r--r--   0        0        0     3358 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0002_minimal_listarray.py
--rw-r--r--   0        0        0      487 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0006_deep_iteration.py
--rw-r--r--   0        0        0     5565 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0008_slices_and_getitem.py
--rw-r--r--   0        0        0    13378 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0011_listarray.py
--rw-r--r--   0        0        0     4462 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0013_error_handling_struct.py
--rw-r--r--   0        0        0    17019 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0014_finish_up_getitem.py
--rw-r--r--   0        0        0     5169 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0018_fromiter_fillable.py
--rw-r--r--   0        0        0     8833 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0019_use_json_library.py
--rw-r--r--   0        0        0    13687 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0020_support_unsigned_indexes.py
--rw-r--r--   0        0        0     6391 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0021_emptyarray.py
--rw-r--r--   0        0        0    10743 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0023_regular_array.py
--rw-r--r--   0        0        0     4890 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0024_use_regular_array.py
--rw-r--r--   0        0        0    25581 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0025_record_array.py
--rw-r--r--   0        0        0     3436 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0028_add_dressed_types.py
--rw-r--r--   0        0        0     6361 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0032_replace_dressedtype.py
--rw-r--r--   0        0        0    12027 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0046_start_indexedarray.py
--rw-r--r--   0        0        0      898 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
--rw-r--r--   0        0        0    12231 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0057_introducing_forms.py
--rw-r--r--   0        0        0     5430 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0070_argmin_and_argmax.py
--rw-r--r--   0        0        0     5384 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0072_fillna_operation.py
--rw-r--r--   0        0        0    15655 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0074_argsort_and_sort.py
--rw-r--r--   0        0        0     2836 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0077_zip_operation.py
--rw-r--r--   0        0        0    11934 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0078_argcross_and_cross.py
--rw-r--r--   0        0        0    12124 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0079_argchoose_and_choose.py
--rw-r--r--   0        0        0     7071 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
--rw-r--r--   0        0        0     6615 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0084_start_unionarray.py
--rw-r--r--   0        0        0     6551 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0086_nep13_ufunc.py
--rw-r--r--   0        0        0    12540 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0089_numpy_functions.py
--rw-r--r--   0        0        0    46684 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0093_simplify_uniontypes_and_optiontypes.py
--rw-r--r--   0        0        0     6959 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0107_assign_fields_to_records.py
--rw-r--r--   0        0        0    46658 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0111_jagged_and_masked_getitem.py
--rw-r--r--   0        0        0    77410 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0115_generic_reducer_operation.py
--rw-r--r--   0        0        0    35162 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0118_numba_cpointers.py
--rw-r--r--   0        0        0     1091 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0119_numexpr_and_broadcast_arrays.py
--rw-r--r--   0        0        0     1106 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0124_strings_in_numba.py
--rw-r--r--   0        0        0    32114 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0127_tomask_operation.py
--rw-r--r--   0        0        0     3683 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0127b_tomask_operation_numba.py
--rw-r--r--   0        0        0      838 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0138_emptyarray_type.py
--rw-r--r--   0        0        0    17923 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0150_flatten.py
--rw-r--r--   0        0        0     3602 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0163_negative_axis_wrap.py
--rw-r--r--   0        0        0     9779 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0166_0167_0170_random_issues.py
--rw-r--r--   0        0        0     4552 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0173_astype_operation.py
--rw-r--r--   0        0        0    24034 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0184_concatenate_operation.py
--rw-r--r--   0        0        0     2063 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0193_is_none_axis_parameter.py
--rw-r--r--   0        0        0     3352 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0198_tutorial_documentation_1.py
--rw-r--r--   0        0        0     8998 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0222_count_with_axis0.py
--rw-r--r--   0        0        0    75605 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0224_arrow_to_awkward.py
--rw-r--r--   0        0        0      581 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0264_reduce_last_empty.py
--rw-r--r--   0        0        0     3251 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0273_path_for_with_field.py
--rw-r--r--   0        0        0      743 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0286_broadcast_single_value_with_field.py
--rw-r--r--   0        0        0     2205 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0290_bug_fixes_for_hats.py
--rw-r--r--   0        0        0     4806 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0315_integerindex.py
--rw-r--r--   0        0        0     5745 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0331_pandas_indexedarray.py
--rw-r--r--   0        0        0     1257 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0334_fully_broadcastable_where.py
--rw-r--r--   0        0        0      566 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0339_highlevel_sorting_function.py
--rw-r--r--   0        0        0     6757 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0348_form_keys.py
--rw-r--r--   0        0        0     4523 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0355_mixins.py
--rw-r--r--   0        0        0    10396 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0395_complex_type_arrays.py
--rw-r--r--   0        0        0     4934 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0395_fix_numba_indexedarray.py
--rw-r--r--   0        0        0     3212 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0397_arrays_as_constants_in_numba.py
--rw-r--r--   0        0        0    14529 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
--rw-r--r--   0        0        0    22467 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0404_array_validity_check.py
--rw-r--r--   0        0        0    14282 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0410_fix_argminmax_positions_for_missing_values.py
--rw-r--r--   0        0        0    17455 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0437_stream_of_many_json_files.py
--rw-r--r--   0        0        0    32921 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0447_preserve_regularness_in_reduce.py
--rw-r--r--   0        0        0    24075 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0449_merge_many_arrays_in_one_pass.py
--rw-r--r--   0        0        0     4059 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0493_zeros_ones_full_like.py
--rw-r--r--   0        0        0     1606 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0496_provide_local_index.py
--rw-r--r--   0        0        0     2059 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0499_getitem_indexedarray_bug.py
--rw-r--r--   0        0        0     1286 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0504_block_ufuncs_for_strings.py
--rw-r--r--   0        0        0     2926 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0511_copy_and_deepcopy.py
--rw-r--r--   0        0        0     9119 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
--rw-r--r--   0        0        0      365 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0546_fill_none_replacement_value_type.py
--rw-r--r--   0        0        0     1102 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0549_numba_array_asarray.py
--rw-r--r--   0        0        0     4268 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0557_min_max_initial_argument.py
--rw-r--r--   0        0        0      537 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0559_fix_booleans_in_numba.py
--rw-r--r--   0        0        0      636 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0572_numba_array_ndim.py
--rw-r--r--   0        0        0     4901 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0582_propagate_context_in_broadcast_and_apply.py
--rw-r--r--   0        0        0     1099 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0583_implement_unflatten_function.py
--rw-r--r--   0        0        0     3084 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0590_allow_regulararray_size_zero.py
--rw-r--r--   0        0        0     5957 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
--rw-r--r--   0        0        0      478 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0627_behavior_from_dict_of_arrays.py
--rw-r--r--   0        0        0     8205 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0652_tests_of_complex_numbers.py
--rw-r--r--   0        0        0     2338 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0674_categorical_validation.py
--rw-r--r--   0        0        0      750 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0713_getitem_field_should_simplify_optiontype.py
--rw-r--r--   0        0        0     1242 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
--rw-r--r--   0        0        0     1055 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0730_unflatten_axis_parameter.py
--rw-r--r--   0        0        0     2569 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0733_run_lengths.py
--rw-r--r--   0        0        0     2127 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0736_implement_argsort_for_strings.py
--rw-r--r--   0        0        0      330 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0758_ak_zip_scallars.py
--rw-r--r--   0        0        0     1122 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0766_prevent_combinations_of_characters.py
--rw-r--r--   0        0        0    26349 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0773_typeparser.py
--rw-r--r--   0        0        0      779 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
--rw-r--r--   0        0        0      871 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0794_ak_cartesian_on_empty_array.py
--rw-r--r--   0        0        0     1148 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0803_argsort_fix_type.py
--rw-r--r--   0        0        0     1364 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0806_empty_lists_cartesian_fix.py
--rw-r--r--   0        0        0     6311 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0813_full_like_dtype_arg.py
--rw-r--r--   0        0        0     1661 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0815_broadcast_union_types_to_all_possibilities.py
--rw-r--r--   0        0        0      488 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0819_issue.py
--rw-r--r--   0        0        0      682 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0828_arrow_datatype_null.py
--rw-r--r--   0        0        0    23609 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0835_datetime_type.py
--rw-r--r--   0        0        0      676 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0835_datetime_type_pandas.py
--rw-r--r--   0        0        0     4662 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0835_datetime_type_pyarrow.py
--rw-r--r--   0        0        0      680 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0850_argsort_mask_array.py
--rw-r--r--   0        0        0      449 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0863_is_none_numpy_array.py
--rw-r--r--   0        0        0     1029 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0866_getitem_field_and_flatten_unions.py
--rw-r--r--   0        0        0      929 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0875_arrow_null_type.py
--rw-r--r--   0        0        0      901 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0879_non_primitive_with_field.py
--rw-r--r--   0        0        0      563 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0884_index_and_identifier_refactoring.py
--rw-r--r--   0        0        0     1086 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0889_ptp.py
--rw-r--r--   0        0        0    53355 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0896_content_classes_refactoring.py
--rw-r--r--   0        0        0     1751 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0898_unzip_heterogeneous_records.py
--rw-r--r--   0        0        0      421 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
--rw-r--r--   0        0        0      530 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0905_leading_zeros_in_unflatten.py
--rw-r--r--   0        0        0     1048 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0906_arrow_fixed_size_list_type.py
--rw-r--r--   0        0        0      666 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0910_unflatten_counts_relation.py
--rw-r--r--   0        0        0     5261 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0912_packed.py
--rw-r--r--   0        0        0   115760 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0914_types_and_forms.py
--rw-r--r--   0        0        0     1877 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0916_datetime_values_astype.py
--rw-r--r--   0        0        0     5522 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0927_numpy_array_nbytes.py
--rw-r--r--   0        0        0      709 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0930_bug_in_unionarray_purelist_parameter.py
--rw-r--r--   0        0        0     1627 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0945_argsort_sort_nan_array.py
--rw-r--r--   0        0        0    28028 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0958_new_forms_must_accept_old_form_json.py
--rw-r--r--   0        0        0    28284 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0959__getitem_array_implementation.py
--rw-r--r--   0        0        0      651 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0975_mask_multidimensional_numpy_array.py
--rw-r--r--   0        0        0      644 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0979_where_multidimentional_numpy_array.py
--rw-r--r--   0        0        0     5803 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0982_missing_case_in_nonlocal_reducers.py
--rw-r--r--   0        0        0     1976 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0984_ravel.py
--rw-r--r--   0        0        0     1806 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0992_correct_ptp_unmasking.py
--rw-r--r--   0        0        0     2100 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
--rw-r--r--   0        0        0      429 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1006_packed_regular_array_zero_size.py
--rw-r--r--   0        0        0      416 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1007_from_buffers_empty_ndarray.py
--rw-r--r--   0        0        0      551 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1017_numpyarray_broadcast.py
--rw-r--r--   0        0        0      785 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1030_mixin_class_name.py
--rw-r--r--   0        0        0    52114 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1031_start_getitem_next.py
--rw-r--r--   0        0        0    18007 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1031b_start_getitem_next_specialized.py
--rw-r--r--   0        0        0     1146 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1049_concatenate_single_array.py
--rw-r--r--   0        0        0     1559 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1055_fill_none_numpy_dimension.py
--rw-r--r--   0        0        0    42250 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1059_localindex.py
--rw-r--r--   0        0        0      551 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1066_to_numpy_masked_structured_array.py
--rw-r--r--   0        0        0      685 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1071_mask_identity_false_should_not_return_option_type.py
--rw-r--r--   0        0        0    27714 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1072_sort.py
--rw-r--r--   0        0        0    44140 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1074_combinations.py
--rw-r--r--   0        0        0     5181 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1075_validityerror.py
--rw-r--r--   0        0        0      273 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1106_argminmax_axis_None_missing_values.py
--rw-r--r--   0        0        0    25531 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1110_type_tracer_1.py
--rw-r--r--   0        0        0     1870 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1116_project_maskedarrays.py
--rw-r--r--   0        0        0    28234 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1125_to_arrow_from_arrow.py
--rw-r--r--   0        0        0     6276 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1132_utility_methods_for_highlevel_functions.py
--rw-r--r--   0        0        0    21098 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1134_from_buffers_to_buffers.py
--rw-r--r--   0        0        0    57322 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1135_rpad_operation.py
--rw-r--r--   0        0        0     4639 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1136_regulararray_zeros_in_shape.py
--rw-r--r--   0        0        0    10487 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1137_num.py
--rw-r--r--   0        0        0    10222 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1142_numbers_to_type.py
--rw-r--r--   0        0        0     2559 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1149_datetime_sort.py
--rw-r--r--   0        0        0      630 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1154_arrow_tables_should_preserve_parameters.py
--rw-r--r--   0        0        0    27983 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1162_ak_from_json_schema.py
--rw-r--r--   0        0        0      766 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1183_bugs_found_by_dask_project_2.py
--rw-r--r--   0        0        0     1286 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1189_fix_singletons_for_non_optional_data.py
--rw-r--r--   0        0        0      551 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1192_iterables_in___array_function__.py
--rw-r--r--   0        0        0      608 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1193_is_none_nested_option.py
--rw-r--r--   0        0        0     2601 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1233_ak_with_name.py
--rw-r--r--   0        0        0    26467 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1240_v2_implementation_of_numba_1.py
--rw-r--r--   0        0        0     1146 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1259_simplify_optiontype.py
--rw-r--r--   0        0        0     1560 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1260_simplify_masked_option_types.py
--rw-r--r--   0        0        0      681 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1271_fix_4D_reducers.py
--rw-r--r--   0        0        0    33003 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1294_to_and_from_parquet.py
--rw-r--r--   0        0        0     1945 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
--rw-r--r--   0        0        0    62340 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1300_awkward_to_cpp_converter_with_cling.py
--rw-r--r--   0        0        0    39474 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1300b_same_for_numba.py
--rw-r--r--   0        0        0      367 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1305_mixed_awkward_numpy_slicing.py
--rw-r--r--   0        0        0     1702 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1308_zip_after_option.py
--rw-r--r--   0        0        0     1703 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1318_array_function_types.py
--rw-r--r--   0        0        0     1730 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1320_mask_identity_defaults.py
--rw-r--r--   0        0        0      647 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1344_broadcast_arrays_depth_limit.py
--rw-r--r--   0        0        0     6621 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1345_avro_reader.py
--rw-r--r--   0        0        0     4562 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1351_is_tuple.py
--rw-r--r--   0        0        0     8362 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1374_to_rdataframe.py
--rw-r--r--   0        0        0     1755 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1377_ravel_string.py
--rw-r--r--   0        0        0     1468 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1379_reducers_with_axis_None_and_typetracers.py
--rw-r--r--   0        0        0     1384 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1399_from_jax.py
--rw-r--r--   0        0        0     1227 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1399_to_jax.py
--rw-r--r--   0        0        0      297 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1400_with_name_record.py
--rw-r--r--   0        0        0      449 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1403_from_numpy_strings.py
--rw-r--r--   0        0        0     3470 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1405_slicing_untested_cases.py
--rw-r--r--   0        0        0     6909 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1415_behaviour_forwarding.py
--rw-r--r--   0        0        0    18809 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1440_start_v2_to_parquet.py
--rw-r--r--   0        0        0    14402 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1447_jax_autodiff_slices_ufuncs.py
--rw-r--r--   0        0        0     8591 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1449_v2_to_json_from_json_functions.py
--rw-r--r--   0        0        0      692 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1453_write_single_records_to_parquet.py
--rw-r--r--   0        0        0     9828 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1473_from_rdataframe.py
--rw-r--r--   0        0        0    24648 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1477_generator_entry_type_as_rvec.py
--rw-r--r--   0        0        0     3579 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1490_jax_reducers_combinations.py
--rw-r--r--   0        0        0     3905 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1502_getitem_jagged_issue1406.py
--rw-r--r--   0        0        0     1733 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1504_typetracer_like.py
--rw-r--r--   0        0        0     4913 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1508_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     2186 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1511_set_attribute.py
--rw-r--r--   0        0        0      754 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1539_isnone_axis_check_issue1417.py
--rw-r--r--   0        0        0     1570 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1559_fix_ufuncs_records_1439.py
--rw-r--r--   0        0        0      990 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1565_axis_wrap_if_negative_record.py
--rw-r--r--   0        0        0     1085 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1567_fix_longlong_in_Index.py
--rw-r--r--   0        0        0     3022 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1568_fix_lengths_empty_regular_slices.py
--rw-r--r--   0        0        0      385 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1578_to_arrow_empty_recordarray.py
--rw-r--r--   0        0        0     5911 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1586_concatenate_should_preserve_regulararray.py
--rw-r--r--   0        0        0      216 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1593_empty_slice_list_record.py
--rw-r--r--   0        0        0     7260 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1604_preserve_form_in_concatenate.py
--rw-r--r--   0        0        0     3636 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1607_no_reducers_on_records.py
--rw-r--r--   0        0        0    10035 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1613_generator_tolayout_records.py
--rw-r--r--   0        0        0      727 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1619_from_parquet_empty_field.py
--rw-r--r--   0        0        0     6024 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1620_layout_builders.py
--rw-r--r--   0        0        0     8122 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1625_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0      770 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1642_from_iter_of_tuples.py
--rw-r--r--   0        0        0      389 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1644_concatenate_zeros_length.py
--rw-r--r--   0        0        0     4317 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1650_Record_to_list_should_listify_itself.py
--rw-r--r--   0        0        0      560 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1671_categorical_type.py
--rw-r--r--   0        0        0    11761 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1672_broadcast_parameters.py
--rw-r--r--   0        0        0     4453 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1677_array_builder_in_numba.py
--rw-r--r--   0        0        0      544 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1685_IndexedArray_project_parameters.py
--rw-r--r--   0        0        0      778 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1686_UnionArray_simplified_preserve_parameters.py
--rw-r--r--   0        0        0      936 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1688_pack_categorical.py
--rw-r--r--   0        0        0      525 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1703_fill_none_typetracer.py
--rw-r--r--   0        0        0     1743 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1707_broadcast_parameters_ufunc.py
--rw-r--r--   0        0        0      512 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1709_ak_array_constructor_behavior.py
--rw-r--r--   0        0        0      398 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1735_from_numpy_mask.py
--rw-r--r--   0        0        0      577 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1747_bytemaskedarray_mergemany.py
--rw-r--r--   0        0        0      824 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1753_indexedarray_merge_kernel.py
--rw-r--r--   0        0        0     1480 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1762_jax_behavior_support.py
--rw-r--r--   0        0        0      589 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1764_jax_jacobian.py
--rw-r--r--   0        0        0      962 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1765_add_ioanas_test_of_to_arraylib.py
--rw-r--r--   0        0        0     4790 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1766_record_form_fields.py
--rw-r--r--   0        0        0     2905 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1781_rdataframe_snapshot.py
--rw-r--r--   0        0        0      701 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1784_reduce_leading_sublist.py
--rw-r--r--   0        0        0      567 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1790_reduce_regulararray.py
--rw-r--r--   0        0        0     4191 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1791_reduce_trailing_sublist.py
--rw-r--r--   0        0        0     1027 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1794_run_lengths_empty_sublist.py
--rw-r--r--   0        0        0      407 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1823_fill_none_axis_none.py
--rw-r--r--   0        0        0      481 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1826_ravel_preserve_none.py
--rw-r--r--   0        0        0     1451 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1829_to_from_rdataframe_bool.py
--rw-r--r--   0        0        0      588 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
--rw-r--r--   0        0        0     1097 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1847_numpy_array_contiguous.py
--rw-r--r--   0        0        0      681 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
--rw-r--r--   0        0        0     1640 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1867_pass_behavior_through_combinations.py
--rw-r--r--   0        0        0    17239 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1904_drop_none.py
--rw-r--r--   0        0        0     3553 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1914_improved_axis_to_posaxis.py
--rw-r--r--   0        0        0     3444 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
--rw-r--r--   0        0        0      921 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1930_unflatten_counts_checks.py
--rw-r--r--   0        0        0      769 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1936_with_field_broadcasting.py
--rw-r--r--   0        0        0      551 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1940_ak_backend.py
--rw-r--r--   0        0        0     1457 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1943_regular_indexing.py
--rw-r--r--   0        0        0      188 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1944_to_numpy_empty_record_array.py
--rw-r--r--   0        0        0     1131 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1960_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     3286 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1961_ak_without_field.py
--rw-r--r--   0        0        0      280 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1978_akRecord_constructor_should_retain_type.py
--rw-r--r--   0        0        0      349 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
--rw-r--r--   0        0        0      371 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2008_ak_type_layout.py
--rw-r--r--   0        0        0    10222 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2020_reduce_axis_none.py
--rw-r--r--   0        0        0      803 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2021_check_TypeTracerArray_in_ak_where.py
--rw-r--r--   0        0        0      645 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2023_from_rdataframe.py
--rw-r--r--   0        0        0     2854 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
--rw-r--r--   0        0        0     1219 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2047_ak_transform_regular_to_jagged.py
--rw-r--r--   0        0        0      406 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2051_arraybuilder_behavior_propagation.py
--rw-r--r--   0        0        0     1275 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2055_array_builder_check.py
--rw-r--r--   0        0        0     1659 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2058_merge_numpy_array.py
--rw-r--r--   0        0        0      708 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2064_fill_none_record.py
--rw-r--r--   0        0        0      799 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2067_to_buffers_byteorder.py
--rw-r--r--   0        0        0      741 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2070_to_layout_string.py
--rw-r--r--   0        0        0     1172 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2071_unflatten_non_packed_counts.py
--rw-r--r--   0        0        0      291 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2076_ak_unzip_record.py
--rw-r--r--   0        0        0      545 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2078_array_function_wrap.py
--rw-r--r--   0        0        0      589 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2082_broadcast_zero_size.py
--rw-r--r--   0        0        0     2765 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2096_ak_scalar_type.py
--rw-r--r--   0        0        0      977 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2101_pickle_behavior_class.py
--rw-r--r--   0        0        0      519 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2104_numpy_merge_option.py
--rw-r--r--   0        0        0     2715 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2106_pickle_class.py
--rw-r--r--   0        0        0      722 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2108_fill_none_indexed.py
--rw-r--r--   0        0        0     2100 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2115_fix_up_typetracers.py
--rw-r--r--   0        0        0      487 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2120_missing_field_error.py
--rw-r--r--   0        0        0     1110 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2125_type_of_scalar.py
--rw-r--r--   0        0        0     1893 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2150_typetracer_high_level_ufunc.py
--rw-r--r--   0        0        0     1898 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2179_parameter_merging_rules.py
--rw-r--r--   0        0        0      510 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2181_with_name_len.py
--rw-r--r--   0        0        0     2957 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2185_merge_union_of_records.py
--rw-r--r--   0        0        0      528 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
--rw-r--r--   0        0        0     5548 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2198_almost_equal.py
--rw-r--r--   0        0        0     1252 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2202_filter_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0     1453 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2214_offset_bool_index.py
--rw-r--r--   0        0        0      334 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2219_flatten_empty.py
--rw-r--r--   0        0        0      663 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2226_slice_regulararray_typetracer.py
--rw-r--r--   0        0        0     1728 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2229_getitem_range_slice.py
--rw-r--r--   0        0        0     4003 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2234_from_rdataframe_keep_order.py
--rw-r--r--   0        0        0     3962 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2236_merge_union_of_records_option.py
--rw-r--r--   0        0        0      485 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2240_merge_union_parameters.py
--rw-r--r--   0        0        0     1338 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2240_simplify_merge_as_union.py
--rw-r--r--   0        0        0      512 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2246_slice_not_packed.py
--rw-r--r--   0        0        0      733 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2250_full_like_bool.py
--rw-r--r--   0        0        0     1835 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2258_from_rdataframe_with_arguments.py
--rw-r--r--   0        0        0      492 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2259_run_lengths_typetracer.py
--rw-r--r--   0        0        0      560 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2263_to_packed_list.py
--rw-r--r--   0        0        0      877 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2266_fix_nan_to_num.py
--rw-r--r--   0        0        0      909 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2267_broadcast_fields.py
--rw-r--r--   0        0        0     1336 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2293_unflatten_typetracer.py
--rw-r--r--   0        0        0      406 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2294_view_unknown_scalar.py
--rw-r--r--   0        0        0     2262 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2297_common_backend.py
--rw-r--r--   0        0        0      455 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2304_index_typetracer.py
--rw-r--r--   0        0        0     2929 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2306_cppyy_git.py
--rw-r--r--   0        0        0     4386 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2319_from_buffers_array.py
--rw-r--r--   0        0        0      721 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2327_array_interface.py
--rw-r--r--   0        0        0     1728 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2329_cartesian_broadcasting_fixes.py
--rw-r--r--   0        0        0      489 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2346_broadcast_depth_limit.py
--rw-r--r--   0        0        0    15621 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2349_growablebuffer_in_numba.py
--rw-r--r--   0        0        0      618 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2354_ufunc_same_backend.py
--rw-r--r--   0        0        0      647 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2355_to_backend_record.py
--rw-r--r--   0        0        0     1435 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2361_typetracer_asarray_nd.py
--rw-r--r--   0        0        0     2921 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2368_type_is_equal.py
--rw-r--r--   0        0        0     5259 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2373_unzip_touching.py
--rw-r--r--   0        0        0     5857 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2374_cartesian_touching.py
--rw-r--r--   0        0        0     1037 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2385_with_field_empty_record.py
--rw-r--r--   0        0        0      926 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2395_copy_asarray_touch.py
--rw-r--r--   0        0        0      128 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/__init__.py
--rw-r--r--   0        0        0      218 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/array_enum_test_data.avro
--rw-r--r--   0        0        0      176 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/array_string_test_data.avro
--rw-r--r--   0        0        0      152 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/array_test_data.avro
--rw-r--r--   0        0        0      115 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/bool_test_data.avro
--rw-r--r--   0        0        0      130 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/bytes_test_data.avro
--rw-r--r--   0        0        0      158 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/double_test_data.avro
--rw-r--r--   0        0        0      191 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/enum_null_test_data.avro
--rw-r--r--   0        0        0      180 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/enum_test_data.avro
--rw-r--r--   0        0        0      218 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/fixed_test_data.avro
--rw-r--r--   0        0        0      116 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/float_test_data.avro
--rw-r--r--   0        0        0      106 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/int_null_test_data.avro
--rw-r--r--   0        0        0      128 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/int_string_null_test_data.avro
--rw-r--r--   0        0        0       89 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/int_test_data.avro
--rw-r--r--   0        0        0     3035 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/list-depths-records-list.parquet
--rw-r--r--   0        0        0     2871 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/list-depths-records.parquet
--rw-r--r--   0        0        0      497 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/list-depths-simple.parquet
--rw-r--r--   0        0        0     1136 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/list-depths-strings.parquet
--rw-r--r--   0        0        0     1060 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/list-depths.parquet
--rw-r--r--   0        0        0      465 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/list-lengths.parquet
--rw-r--r--   0        0        0      116 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/long_test_data.avro
--rw-r--r--   0        0        0      681 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nonnullable-depths.parquet
--rw-r--r--   0        0        0       75 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/null_test_data.avro
--rw-r--r--   0        0        0      719 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-depths.parquet
--rw-r--r--   0        0        0      635 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-levels.parquet
--rw-r--r--   0        0        0     3050 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-list-depths-records-list.parquet
--rw-r--r--   0        0        0     2926 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-list-depths-records.parquet
--rw-r--r--   0        0        0     1179 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-list-depths-strings.parquet
--rw-r--r--   0        0        0     1101 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-list-depths.parquet
--rw-r--r--   0        0        0      430 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-record-primitives-simple.parquet
--rw-r--r--   0        0        0     1181 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-record-primitives.parquet
--rw-r--r--   0        0        0     1193 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/record-primitives.parquet
--rw-r--r--   0        0        0      326 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/record_0_test_data.avro
--rw-r--r--   0        0        0      368 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/record_1_test_data.avro
--rw-r--r--   0        0        0      263 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/record_null_test_data.avro
--rw-r--r--   0        0        0      423 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/record_test_data.avro
--rw-r--r--   0        0        0      116 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/string_null_test_data.avro
--rw-r--r--   0        0        0      125 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/string_test_data.avro
--rw-r--r--   0        0        0      544 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/test-nan-inf.json
--rw-r--r--   0        0        0      155 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/test-record-array.json
--rw-r--r--   0        0        0      803 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/test-two-arrays.json
--rw-r--r--   0        0        0      535 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/test.json
--rw-r--r--   0        0        0      180 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/zero-record-batches.parquet
--rw-r--r--   0        0        0       88 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/__init__.py
--rw-r--r--   0        0        0     7072 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1276_cuda_num.py
--rw-r--r--   0        0        0     9911 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1276_cuda_transfers.py
--rw-r--r--   0        0        0     1197 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1276_cupy_interop.py
--rw-r--r--   0        0        0     1782 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1276_from_cupy.py
--rw-r--r--   0        0        0    42786 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1300_same_for_numba_cuda.py
--rw-r--r--   0        0        0      834 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1381_check_errors.py
--rw-r--r--   0        0        0    11252 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1809_array_cuda_jit.py
--rw-r--r--   0        0        0     2212 2023-04-13 15:38:23.000000 awkward-2.1.3/.gitignore
--rw-r--r--   0        0        0     1520 2023-04-13 15:38:23.000000 awkward-2.1.3/LICENSE
--rw-r--r--   0        0        0     8479 2023-04-13 15:38:23.000000 awkward-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     6933 2023-04-13 15:38:23.000000 awkward-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1893 2023-04-24 16:57:22.000000 awkward-2.1.4/CITATION.cff
+-rw-r--r--   0        0        0    13578 2023-04-24 16:57:22.000000 awkward-2.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    22687 2023-04-24 16:57:22.000000 awkward-2.1.4/README.md
+-rw-r--r--   0        0        0      241 2023-04-24 16:57:22.000000 awkward-2.1.4/requirements-test.txt
+-rw-r--r--   0        0        0     7833 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/_toc.yml
+-rw-r--r--   0        0        0     7624 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/conf.py
+-rw-r--r--   0        0        0      346 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/environment.yml.cog
+-rw-r--r--   0        0        0     2603 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/index.md
+-rw-r--r--   0        0        0    11642 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/prepare_docstrings.py
+-rw-r--r--   0        0        0     4448 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/redirects-user-guide.json
+-rw-r--r--   0        0        0    11436 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/redirects.json
+-rw-r--r--   0        0        0      463 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/requirements.txt
+-rw-r--r--   0        0        0      369 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/switcher.json
+-rw-r--r--   0        0        0      930 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/_static/css/awkward.css
+-rw-r--r--   0        0        0      354 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/_static/css/try-awkward-array.css
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0      469 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/_templates/funding.html
+-rw-r--r--   0        0        0      474 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/_templates/redirect.html
+-rw-r--r--   0        0        0     2968 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/getting-started/community-tutorials.md
+-rw-r--r--   0        0        0     4654 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/getting-started/index.md
+-rw-r--r--   0        0        0     3346 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/getting-started/papers-and-talks.md
+-rw-r--r--   0        0        0       82 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/getting-started/try-awkward-array.md
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    12847 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/getting-started/demo/what-is-an-awkward-array.ipynb
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    17067 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/image/example-hierarchy.svg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    25309 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/reference/ak.behavior.rst
+-rw-r--r--   0        0        0     1426 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/reference/ak.builder.ArrayBuilder.rst
+-rw-r--r--   0        0        0    64727 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/reference/awkwardforth.rst
+-rw-r--r--   0        0        0      270 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/reference/index.md
+-rw-r--r--   0        0        0     7252 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/reference/toctree.txt
+-rw-r--r--   0        0        0     8320 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/10-minutes-to-awkward-array.md
+-rw-r--r--   0        0        0      926 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-combinatorics-best-match.md
+-rw-r--r--   0        0        0      930 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
+-rw-r--r--   0        0        0      263 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-combinatorics.md
+-rw-r--r--   0        0        0     8335 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-convert-arrow.md
+-rw-r--r--   0        0        0     6392 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-convert-buffers.md
+-rw-r--r--   0        0        0     2455 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-convert-json.md
+-rw-r--r--   0        0        0    13475 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-convert-numpy.md
+-rw-r--r--   0        0        0     7182 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-convert-pandas.md
+-rw-r--r--   0        0        0    18830 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-convert-python.md
+-rw-r--r--   0        0        0     3554 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-convert-rdataframe.md
+-rw-r--r--   0        0        0      271 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-convert.md
+-rw-r--r--   0        0        0    11973 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-create-arraybuilder.md
+-rw-r--r--   0        0        0    36520 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-create-constructors.md
+-rw-r--r--   0        0        0     7383 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-create-lists.md
+-rw-r--r--   0        0        0     7456 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-create-missing.md
+-rw-r--r--   0        0        0    11542 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-create-records.md
+-rw-r--r--   0        0        0     4066 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-create-strings.md
+-rw-r--r--   0        0        0      866 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-create-unflatten-group.md
+-rw-r--r--   0        0        0      267 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-create.md
+-rw-r--r--   0        0        0      834 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-examine-checking-validity.md
+-rw-r--r--   0        0        0     2919 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-examine-list-fields.md
+-rw-r--r--   0        0        0      848 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-examine-simple-slicing.md
+-rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-examine-single-item.md
+-rw-r--r--   0        0        0     6778 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-examine-type.md
+-rw-r--r--   0        0        0      269 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-examine.md
+-rw-r--r--   0        0        0      844 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-filter-cut-mask.md
+-rw-r--r--   0        0        0     3889 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-filter-masked.md
+-rw-r--r--   0        0        0      840 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-filter-num.md
+-rw-r--r--   0        0        0     7955 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-filter-ragged.md
+-rw-r--r--   0        0        0      265 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-filter.md
+-rw-r--r--   0        0        0      818 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-math-argminmax.md
+-rw-r--r--   0        0        0      822 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-math-broadcasting.md
+-rw-r--r--   0        0        0      828 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-math-gpu.md
+-rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-math-numpy.md
+-rw-r--r--   0        0        0      846 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-math-reducing.md
+-rw-r--r--   0        0        0      870 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-math-statistics.md
+-rw-r--r--   0        0        0      265 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-math.md
+-rw-r--r--   0        0        0     3411 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-restructure-add-fields.md
+-rw-r--r--   0        0        0      842 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-restructure-concatenate.md
+-rw-r--r--   0        0        0    19083 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-restructure-flatten.md
+-rw-r--r--   0        0        0     7568 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-restructure-pad.md
+-rw-r--r--   0        0        0      852 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-restructure-rename-records.md
+-rw-r--r--   0        0        0      832 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-restructure-sort.md
+-rw-r--r--   0        0        0     9624 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-restructure-zip-project.md
+-rw-r--r--   0        0        0      273 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-restructure.md
+-rw-r--r--   0        0        0     2599 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-specialize-differentiate-jax.md
+-rw-r--r--   0        0        0      870 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-specialize-in-numba.md
+-rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-specialize-lorentz.md
+-rw-r--r--   0        0        0      874 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-specialize-override-numpy.md
+-rw-r--r--   0        0        0      870 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-specialize-subclass.md
+-rw-r--r--   0        0        0      277 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-specialize.md
+-rw-r--r--   0        0        0    11724 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-use-header-only-layoutbuilder.md
+-rw-r--r--   0        0        0      900 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-use-in-numba-arraybuilder.md
+-rw-r--r--   0        0        0     9973 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-use-in-numba-cuda.ipynb
+-rw-r--r--   0        0        0      900 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-use-in-numba-features.md
+-rw-r--r--   0        0        0      279 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/how-to-use-in-numba.md
+-rw-r--r--   0        0        0      344 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/index.md
+-rw-r--r--   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/docs/user-guide/requirements.txt
+-rw-r--r--   0        0        0   367587 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/panel-data-analysts.png
+-rw-r--r--   0        0        0   794465 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/panel-data-analysts.svg
+-rw-r--r--   0        0        0   140700 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/panel-developers.png
+-rw-r--r--   0        0        0   328307 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/panel-developers.svg
+-rw-r--r--   0        0        0    73584 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/panel-doxygen.png
+-rw-r--r--   0        0        0    58179 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/panel-sphinx.png
+-rw-r--r--   0        0        0   127063 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/panel-tutorials-alternate.png
+-rw-r--r--   0        0        0   173327 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/panel-tutorials.png
+-rw-r--r--   0        0        0    12541 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/awkward-1-0-layers.pdf
+-rw-r--r--   0        0        0    65246 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/awkward-1-0-layers.png
+-rw-r--r--   0        0        0    41004 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/awkward-1-0-layers.svg
+-rw-r--r--   0        0        0    14946 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/awkward-timeline.pdf
+-rw-r--r--   0        0        0   125180 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/awkward-timeline.png
+-rw-r--r--   0        0        0    70209 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/awkward-timeline.svg
+-rw-r--r--   0        0        0   436595 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
+-rw-r--r--   0        0        0   426911 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
+-rw-r--r--   0        0        0   335955 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/awkward-uproot-timeline-pip.png
+-rw-r--r--   0        0        0   325268 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/awkward-uproot-timeline-pip.svg
+-rw-r--r--   0        0        0   129696 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/awkward-uproot-timeline.png
+-rw-r--r--   0        0        0   120554 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/awkward-uproot-timeline.svg
+-rw-r--r--   0        0        0     5208 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/cartoon-broadcasting.png
+-rw-r--r--   0        0        0    25065 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/cartoon-broadcasting.svg
+-rw-r--r--   0        0        0     5754 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/cartoon-cartesian.png
+-rw-r--r--   0        0        0    32616 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/cartoon-cartesian.svg
+-rw-r--r--   0        0        0     9584 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/cartoon-combinations.png
+-rw-r--r--   0        0        0    39524 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/cartoon-combinations.svg
+-rw-r--r--   0        0        0    10808 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/cartoon-schematic.png
+-rw-r--r--   0        0        0    25779 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/cartoon-schematic.svg
+-rw-r--r--   0        0        0    18178 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    36024 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/example-hierarchy.png
+-rw-r--r--   0        0        0    17092 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/example-hierarchy.svg
+-rw-r--r--   0        0        0    21120 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/example-reduction-sum-only.svg
+-rw-r--r--   0        0        0    29325 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    55553 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/example-reduction.png
+-rw-r--r--   0        0        0    21631 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/example-reduction.svg
+-rw-r--r--   0        0        0    10978 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/git-strategy.pdf
+-rw-r--r--   0        0        0    58904 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/git-strategy.png
+-rw-r--r--   0        0        0    28990 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/git-strategy.svg
+-rw-r--r--   0        0        0   113587 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/how-it-works-muons.png
+-rw-r--r--   0        0        0    57471 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/how-it-works-muons.svg
+-rw-r--r--   0        0        0    58475 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/how-it-works.svg
+-rw-r--r--   0        0        0    63989 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/sorting-axis.svg
+-rw-r--r--   0        0        0   124038 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/reducers/all.svg
+-rw-r--r--   0        0        0   128558 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/reducers/any.svg
+-rw-r--r--   0        0        0   134490 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/reducers/argmax.svg
+-rw-r--r--   0        0        0   133192 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/reducers/argmin.svg
+-rw-r--r--   0        0        0   106277 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/reducers/count.svg
+-rw-r--r--   0        0        0   116417 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/reducers/count_nonzero.svg
+-rw-r--r--   0        0        0   111789 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/reducers/max.svg
+-rw-r--r--   0        0        0   109239 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/reducers/min.svg
+-rw-r--r--   0        0        0   124702 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/reducers/product.svg
+-rw-r--r--   0        0        0   108897 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/diagrams/reducers/sum.svg
+-rw-r--r--   0        0        0     8347 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/logo/favicon.ico
+-rw-r--r--   0        0        0     8984 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0    11964 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24707 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0    18767 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0    90413 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/photos/desire-path.jpg
+-rw-r--r--   0        0        0    52113 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/plots/awkward-0-popularity.pdf
+-rw-r--r--   0        0        0   146109 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/plots/awkward-0-popularity.png
+-rw-r--r--   0        0        0   147576 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/plots/awkward-0-popularity.svg
+-rw-r--r--   0        0        0    26938 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/plots/bikeroutes-scaling.svg
+-rw-r--r--   0        0        0     8891 2023-04-24 16:57:22.000000 awkward-2.1.4/docs-img/screenshots/github-issues-documentation.png
+-rw-r--r--   0        0        0     1325 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/__init__.py
+-rw-r--r--   0        0        0     5418 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_behavior.py
+-rw-r--r--   0        0        0    37836 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_broadcasting.py
+-rw-r--r--   0        0        0    13424 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_do.py
+-rw-r--r--   0        0        0    12017 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_errors.py
+-rw-r--r--   0        0        0     5672 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_kernels.py
+-rw-r--r--   0        0        0     5860 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_layout.py
+-rw-r--r--   0        0        0     9983 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_lookup.py
+-rw-r--r--   0        0        0     5454 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_parameters.py
+-rw-r--r--   0        0        0     9965 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_prettyprint.py
+-rw-r--r--   0        0        0    24569 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_reducers.py
+-rw-r--r--   0        0        0     2041 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_regularize.py
+-rw-r--r--   0        0        0      420 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_singleton.py
+-rw-r--r--   0        0        0    23934 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_slicing.py
+-rw-r--r--   0        0        0      647 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_typetracer.py
+-rw-r--r--   0        0        0     1163 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_typing.py
+-rw-r--r--   0        0        0     2439 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_util.py
+-rw-r--r--   0        0        0      758 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_v2.py
+-rw-r--r--   0        0        0      233 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/builder.py
+-rw-r--r--   0        0        0      866 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/cppyy.py
+-rw-r--r--   0        0        0      271 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forth.py
+-rw-r--r--   0        0        0   103299 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/highlevel.py
+-rw-r--r--   0        0        0     8005 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/index.py
+-rw-r--r--   0        0        0     3988 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/jax.py
+-rw-r--r--   0        0        0     6017 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/numba.py
+-rw-r--r--   0        0        0     8272 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/record.py
+-rw-r--r--   0        0        0      165 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/typetracer.py
+-rw-r--r--   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_backends/__init__.py
+-rw-r--r--   0        0        0     1336 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_backends/backend.py
+-rw-r--r--   0        0        0     1259 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_backends/cupy.py
+-rw-r--r--   0        0        0     3763 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_backends/dispatch.py
+-rw-r--r--   0        0        0     1781 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_backends/jax.py
+-rw-r--r--   0        0        0      944 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_backends/numpy.py
+-rw-r--r--   0        0        0     1902 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_backends/typetracer.py
+-rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/__init__.py
+-rw-r--r--   0        0        0    32504 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/avro.py
+-rw-r--r--   0        0        0    53533 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cling.py
+-rw-r--r--   0        0        0      985 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/hist.py
+-rw-r--r--   0        0        0     4485 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/numexpr.py
+-rw-r--r--   0        0        0    11488 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/numpy.py
+-rw-r--r--   0        0        0    37988 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/pyarrow.py
+-rw-r--r--   0        0        0     7038 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/__init__.py
+-rw-r--r--   0        0        0     2555 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
+-rw-r--r--   0        0        0     4326 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
+-rw-r--r--   0        0        0      987 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
+-rw-r--r--   0        0        0     2542 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3034 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0      630 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
+-rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3196 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0     2668 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0      749 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
+-rw-r--r--   0        0        0     2749 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
+-rw-r--r--   0        0        0      552 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
+-rw-r--r--   0        0        0      637 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
+-rw-r--r--   0        0        0     2886 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
+-rw-r--r--   0        0        0     2904 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3416 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0     3531 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
+-rw-r--r--   0        0        0      556 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
+-rw-r--r--   0        0        0      695 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3036 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0      795 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
+-rw-r--r--   0        0        0     2523 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0     2729 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
+-rw-r--r--   0        0        0     1035 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
+-rw-r--r--   0        0        0      961 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
+-rw-r--r--   0        0        0     2593 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
+-rw-r--r--   0        0        0     1536 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
+-rw-r--r--   0        0        0     1710 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     2012 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1184 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
+-rw-r--r--   0        0        0      755 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu
+-rw-r--r--   0        0        0      806 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
+-rw-r--r--   0        0        0      744 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
+-rw-r--r--   0        0        0     1169 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0     1059 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
+-rw-r--r--   0        0        0     3208 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
+-rw-r--r--   0        0        0      575 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
+-rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
+-rw-r--r--   0        0        0      650 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
+-rw-r--r--   0        0        0     2610 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
+-rw-r--r--   0        0        0     1126 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
+-rw-r--r--   0        0        0      951 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      721 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
+-rw-r--r--   0        0        0     1003 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
+-rw-r--r--   0        0        0     1339 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
+-rw-r--r--   0        0        0      835 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
+-rw-r--r--   0        0        0      975 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
+-rw-r--r--   0        0        0      802 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
+-rw-r--r--   0        0        0     1123 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu
+-rw-r--r--   0        0        0      623 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu
+-rw-r--r--   0        0        0      789 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
+-rw-r--r--   0        0        0     1040 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     1020 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1045 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      974 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
+-rw-r--r--   0        0        0      946 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
+-rw-r--r--   0        0        0      980 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
+-rw-r--r--   0        0        0      663 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
+-rw-r--r--   0        0        0      586 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
+-rw-r--r--   0        0        0     2580 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
+-rw-r--r--   0        0        0     1360 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
+-rw-r--r--   0        0        0      461 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
+-rw-r--r--   0        0        0      534 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
+-rw-r--r--   0        0        0      529 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
+-rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
+-rw-r--r--   0        0        0      636 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
+-rw-r--r--   0        0        0      689 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0      457 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
+-rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
+-rw-r--r--   0        0        0     2043 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
+-rw-r--r--   0        0        0     2198 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
+-rw-r--r--   0        0        0     2043 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
+-rw-r--r--   0        0        0     2198 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
+-rw-r--r--   0        0        0     3054 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
+-rw-r--r--   0        0        0     3289 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
+-rw-r--r--   0        0        0     2022 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
+-rw-r--r--   0        0        0     2022 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
+-rw-r--r--   0        0        0     3202 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
+-rw-r--r--   0        0        0     3012 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
+-rw-r--r--   0        0        0     3171 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
+-rw-r--r--   0        0        0     3439 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
+-rw-r--r--   0        0        0     3439 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
+-rw-r--r--   0        0        0      865 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
+-rw-r--r--   0        0        0      443 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
+-rw-r--r--   0        0        0     3195 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
+-rw-r--r--   0        0        0     1859 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/header-only/awkward/BuilderOptions.h
+-rw-r--r--   0        0        0    19822 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
+-rw-r--r--   0        0        0    89307 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
+-rw-r--r--   0        0        0      298 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/header-only/awkward/demo_impl.h
+-rw-r--r--   0        0        0     8025 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/header-only/awkward/utils.h
+-rw-r--r--   0        0        0      239 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/jax/__init__.py
+-rw-r--r--   0        0        0     6627 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/jax/reducers.py
+-rw-r--r--   0        0        0     5982 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/jax/trees.py
+-rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/numba/__init__.py
+-rw-r--r--   0        0        0    35824 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/numba/arrayview.py
+-rw-r--r--   0        0        0     1182 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/numba/arrayview_cuda.py
+-rw-r--r--   0        0        0    31514 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/numba/builder.py
+-rw-r--r--   0        0        0     9624 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/numba/growablebuffer.py
+-rw-r--r--   0        0        0    49132 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/numba/layout.py
+-rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/rdataframe/__init__.py
+-rw-r--r--   0        0        0     9377 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/rdataframe/from_rdataframe.py
+-rw-r--r--   0        0        0     9922 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/rdataframe/to_rdataframe.py
+-rw-r--r--   0        0        0     1487 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
+-rw-r--r--   0        0        0     1111 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_nplikes/__init__.py
+-rw-r--r--   0        0        0    13294 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_nplikes/array_module.py
+-rw-r--r--   0        0        0     4939 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_nplikes/cupy.py
+-rw-r--r--   0        0        0     1357 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_nplikes/dispatch.py
+-rw-r--r--   0        0        0     2010 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_nplikes/jax.py
+-rw-r--r--   0        0        0     2922 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_nplikes/numpy.py
+-rw-r--r--   0        0        0    14150 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_nplikes/numpylike.py
+-rw-r--r--   0        0        0     2288 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_nplikes/shape.py
+-rw-r--r--   0        0        0    43770 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_nplikes/typetracer.py
+-rw-r--r--   0        0        0     2527 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/_nplikes/ufuncs.py
+-rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/behaviors/__init__.py
+-rw-r--r--   0        0        0     3479 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/behaviors/categorical.py
+-rw-r--r--   0        0        0     3898 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/behaviors/mixins.py
+-rw-r--r--   0        0        0     8509 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/behaviors/string.py
+-rw-r--r--   0        0        0      986 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/__init__.py
+-rw-r--r--   0        0        0    27803 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/bitmaskedarray.py
+-rw-r--r--   0        0        0    40958 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/bytemaskedarray.py
+-rw-r--r--   0        0        0    45437 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/content.py
+-rw-r--r--   0        0        0    13347 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/emptyarray.py
+-rw-r--r--   0        0        0    40382 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/indexedarray.py
+-rw-r--r--   0        0        0    63462 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/indexedoptionarray.py
+-rw-r--r--   0        0        0    59821 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/listarray.py
+-rw-r--r--   0        0        0    85149 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/listoffsetarray.py
+-rw-r--r--   0        0        0    49439 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/numpyarray.py
+-rw-r--r--   0        0        0    40526 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/recordarray.py
+-rw-r--r--   0        0        0    54541 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/regulararray.py
+-rw-r--r--   0        0        0    56997 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/unionarray.py
+-rw-r--r--   0        0        0    18878 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/contents/unmaskedarray.py
+-rw-r--r--   0        0        0      951 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/__init__.py
+-rw-r--r--   0        0        0     6081 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/bitmaskedform.py
+-rw-r--r--   0        0        0     5368 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/bytemaskedform.py
+-rw-r--r--   0        0        0     3369 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/emptyform.py
+-rw-r--r--   0        0        0    12450 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/form.py
+-rw-r--r--   0        0        0     5638 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/indexedform.py
+-rw-r--r--   0        0        0     5133 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/indexedoptionform.py
+-rw-r--r--   0        0        0     5621 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/listform.py
+-rw-r--r--   0        0        0     4715 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/listoffsetform.py
+-rw-r--r--   0        0        0     6004 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/numpyform.py
+-rw-r--r--   0        0        0     8208 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/recordform.py
+-rw-r--r--   0        0        0     5084 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/regularform.py
+-rw-r--r--   0        0        0     7760 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/unionform.py
+-rw-r--r--   0        0        0     4229 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/forms/unmaskedform.py
+-rw-r--r--   0        0        0     4779 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/__init__.py
+-rw-r--r--   0        0        0     3998 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_all.py
+-rw-r--r--   0        0        0     7381 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_almost_equal.py
+-rw-r--r--   0        0        0     4001 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_any.py
+-rw-r--r--   0        0        0     5109 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_argcartesian.py
+-rw-r--r--   0        0        0     3819 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_argcombinations.py
+-rw-r--r--   0        0        0     6888 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_argmax.py
+-rw-r--r--   0        0        0     6845 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_argmin.py
+-rw-r--r--   0        0        0     3158 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_argsort.py
+-rw-r--r--   0        0        0      952 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_backend.py
+-rw-r--r--   0        0        0     9855 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_broadcast_arrays.py
+-rw-r--r--   0        0        0     6595 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_broadcast_fields.py
+-rw-r--r--   0        0        0    15615 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_cartesian.py
+-rw-r--r--   0        0        0     1420 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_categories.py
+-rw-r--r--   0        0        0     8118 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_combinations.py
+-rw-r--r--   0        0        0    12213 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_concatenate.py
+-rw-r--r--   0        0        0     2715 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_copy.py
+-rw-r--r--   0        0        0     5817 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_corr.py
+-rw-r--r--   0        0        0     5228 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_count.py
+-rw-r--r--   0        0        0     4035 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_count_nonzero.py
+-rw-r--r--   0        0        0     5170 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_covar.py
+-rw-r--r--   0        0        0     4581 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_drop_none.py
+-rw-r--r--   0        0        0     1106 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_fields.py
+-rw-r--r--   0        0        0     5323 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_fill_none.py
+-rw-r--r--   0        0        0     3467 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_firsts.py
+-rw-r--r--   0        0        0     7802 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_flatten.py
+-rw-r--r--   0        0        0     3154 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_arrow.py
+-rw-r--r--   0        0        0      813 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_arrow_schema.py
+-rw-r--r--   0        0        0     2727 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_avro_file.py
+-rw-r--r--   0        0        0    14453 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_buffers.py
+-rw-r--r--   0        0        0     1839 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_categorical.py
+-rw-r--r--   0        0        0     1651 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_cupy.py
+-rw-r--r--   0        0        0     4109 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_iter.py
+-rw-r--r--   0        0        0     1716 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_jax.py
+-rw-r--r--   0        0        0    30065 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_json.py
+-rw-r--r--   0        0        0     2282 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_numpy.py
+-rw-r--r--   0        0        0    11860 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_parquet.py
+-rw-r--r--   0        0        0     3324 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_rdataframe.py
+-rw-r--r--   0        0        0     3000 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_from_regular.py
+-rw-r--r--   0        0        0     8859 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_full_like.py
+-rw-r--r--   0        0        0      873 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_is_categorical.py
+-rw-r--r--   0        0        0     2513 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_is_none.py
+-rw-r--r--   0        0        0      705 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_is_tuple.py
+-rw-r--r--   0        0        0      930 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_is_valid.py
+-rw-r--r--   0        0        0     2568 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_isclose.py
+-rw-r--r--   0        0        0     9131 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_linear_fit.py
+-rw-r--r--   0        0        0     3258 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_local_index.py
+-rw-r--r--   0        0        0     4757 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_mask.py
+-rw-r--r--   0        0        0     7430 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_max.py
+-rw-r--r--   0        0        0     9067 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_mean.py
+-rw-r--r--   0        0        0     3603 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_merge_option_of_records.py
+-rw-r--r--   0        0        0    12413 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_merge_union_of_records.py
+-rw-r--r--   0        0        0     3217 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_metadata_from_parquet.py
+-rw-r--r--   0        0        0     7382 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_min.py
+-rw-r--r--   0        0        0     4908 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_moment.py
+-rw-r--r--   0        0        0     2081 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_nan_to_none.py
+-rw-r--r--   0        0        0     5103 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_nan_to_num.py
+-rw-r--r--   0        0        0     3909 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_num.py
+-rw-r--r--   0        0        0     1951 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_ones_like.py
+-rw-r--r--   0        0        0     4362 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_pad_none.py
+-rw-r--r--   0        0        0     1786 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_parameters.py
+-rw-r--r--   0        0        0     6360 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_prod.py
+-rw-r--r--   0        0        0     4710 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_ptp.py
+-rw-r--r--   0        0        0     2275 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_ravel.py
+-rw-r--r--   0        0        0     9604 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_run_lengths.py
+-rw-r--r--   0        0        0     3063 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_singletons.py
+-rw-r--r--   0        0        0     3339 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_softmax.py
+-rw-r--r--   0        0        0     2670 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_sort.py
+-rw-r--r--   0        0        0     8124 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_std.py
+-rw-r--r--   0        0        0     3058 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_strings_astype.py
+-rw-r--r--   0        0        0    11718 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_sum.py
+-rw-r--r--   0        0        0     4931 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_arrow.py
+-rw-r--r--   0        0        0     6725 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_arrow_table.py
+-rw-r--r--   0        0        0     2370 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_backend.py
+-rw-r--r--   0        0        0     6378 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_buffers.py
+-rw-r--r--   0        0        0     6050 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_categorical.py
+-rw-r--r--   0        0        0     1107 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_cupy.py
+-rw-r--r--   0        0        0    13370 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_dataframe.py
+-rw-r--r--   0        0        0     1106 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_jax.py
+-rw-r--r--   0        0        0    11652 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_json.py
+-rw-r--r--   0        0        0     4507 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_layout.py
+-rw-r--r--   0        0        0     2612 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_list.py
+-rw-r--r--   0        0        0     2123 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_numpy.py
+-rw-r--r--   0        0        0     3354 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_packed.py
+-rw-r--r--   0        0        0    16968 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_parquet.py
+-rw-r--r--   0        0        0     2785 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_rdataframe.py
+-rw-r--r--   0        0        0     3382 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_to_regular.py
+-rw-r--r--   0        0        0    23979 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_transform.py
+-rw-r--r--   0        0        0     4304 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_type.py
+-rw-r--r--   0        0        0     9461 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_unflatten.py
+-rw-r--r--   0        0        0     2484 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_unzip.py
+-rw-r--r--   0        0        0     1138 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_validity_error.py
+-rw-r--r--   0        0        0     2659 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_values_astype.py
+-rw-r--r--   0        0        0     9352 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_var.py
+-rw-r--r--   0        0        0     5862 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_where.py
+-rw-r--r--   0        0        0     5788 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_with_field.py
+-rw-r--r--   0        0        0     2610 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_with_name.py
+-rw-r--r--   0        0        0     1848 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_with_parameter.py
+-rw-r--r--   0        0        0     3756 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_without_field.py
+-rw-r--r--   0        0        0     1509 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_without_parameters.py
+-rw-r--r--   0        0        0     2134 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_zeros_like.py
+-rw-r--r--   0        0        0     8819 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/operations/ak_zip.py
+-rw-r--r--   0        0        0      707 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/types/__init__.py
+-rw-r--r--   0        0        0   163323 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/types/_awkward_datashape_parser.py
+-rw-r--r--   0        0        0     1914 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/types/arraytype.py
+-rw-r--r--   0        0        0     2451 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/types/listtype.py
+-rw-r--r--   0        0        0     5652 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/types/numpytype.py
+-rw-r--r--   0        0        0     4180 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/types/optiontype.py
+-rw-r--r--   0        0        0     8067 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/types/recordtype.py
+-rw-r--r--   0        0        0     3133 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/types/regulartype.py
+-rw-r--r--   0        0        0     1105 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/types/scalartype.py
+-rw-r--r--   0        0        0     9622 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/types/type.py
+-rw-r--r--   0        0        0     3725 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/types/uniontype.py
+-rw-r--r--   0        0        0     1937 2023-04-24 16:57:22.000000 awkward-2.1.4/src/awkward/types/unknowntype.py
+-rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     3358 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0002_minimal_listarray.py
+-rw-r--r--   0        0        0      487 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0006_deep_iteration.py
+-rw-r--r--   0        0        0     5565 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0008_slices_and_getitem.py
+-rw-r--r--   0        0        0    13378 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0011_listarray.py
+-rw-r--r--   0        0        0     4462 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0013_error_handling_struct.py
+-rw-r--r--   0        0        0    17019 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0014_finish_up_getitem.py
+-rw-r--r--   0        0        0     5169 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0018_fromiter_fillable.py
+-rw-r--r--   0        0        0     8833 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0019_use_json_library.py
+-rw-r--r--   0        0        0    13687 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0020_support_unsigned_indexes.py
+-rw-r--r--   0        0        0     6391 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0021_emptyarray.py
+-rw-r--r--   0        0        0    10743 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0023_regular_array.py
+-rw-r--r--   0        0        0     4890 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0024_use_regular_array.py
+-rw-r--r--   0        0        0    25581 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0025_record_array.py
+-rw-r--r--   0        0        0     3436 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0028_add_dressed_types.py
+-rw-r--r--   0        0        0     6361 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0032_replace_dressedtype.py
+-rw-r--r--   0        0        0    12027 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0046_start_indexedarray.py
+-rw-r--r--   0        0        0      898 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
+-rw-r--r--   0        0        0    12231 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0057_introducing_forms.py
+-rw-r--r--   0        0        0     5430 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0070_argmin_and_argmax.py
+-rw-r--r--   0        0        0     5384 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0072_fillna_operation.py
+-rw-r--r--   0        0        0    15655 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0074_argsort_and_sort.py
+-rw-r--r--   0        0        0     2836 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0077_zip_operation.py
+-rw-r--r--   0        0        0    11934 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0078_argcross_and_cross.py
+-rw-r--r--   0        0        0    12124 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0079_argchoose_and_choose.py
+-rw-r--r--   0        0        0     7071 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
+-rw-r--r--   0        0        0     6615 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0084_start_unionarray.py
+-rw-r--r--   0        0        0     6551 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0086_nep13_ufunc.py
+-rw-r--r--   0        0        0    12540 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0089_numpy_functions.py
+-rw-r--r--   0        0        0    46684 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0093_simplify_uniontypes_and_optiontypes.py
+-rw-r--r--   0        0        0     6959 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0107_assign_fields_to_records.py
+-rw-r--r--   0        0        0    46658 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0111_jagged_and_masked_getitem.py
+-rw-r--r--   0        0        0    77410 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0115_generic_reducer_operation.py
+-rw-r--r--   0        0        0    35162 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0118_numba_cpointers.py
+-rw-r--r--   0        0        0     1091 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0119_numexpr_and_broadcast_arrays.py
+-rw-r--r--   0        0        0     1106 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0124_strings_in_numba.py
+-rw-r--r--   0        0        0    32114 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0127_tomask_operation.py
+-rw-r--r--   0        0        0     3683 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0127b_tomask_operation_numba.py
+-rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0138_emptyarray_type.py
+-rw-r--r--   0        0        0    17923 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0150_flatten.py
+-rw-r--r--   0        0        0     3602 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0163_negative_axis_wrap.py
+-rw-r--r--   0        0        0     9779 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0166_0167_0170_random_issues.py
+-rw-r--r--   0        0        0     4552 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0173_astype_operation.py
+-rw-r--r--   0        0        0    24034 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0184_concatenate_operation.py
+-rw-r--r--   0        0        0     2063 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0193_is_none_axis_parameter.py
+-rw-r--r--   0        0        0     3352 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0198_tutorial_documentation_1.py
+-rw-r--r--   0        0        0     8998 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0222_count_with_axis0.py
+-rw-r--r--   0        0        0    75605 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0224_arrow_to_awkward.py
+-rw-r--r--   0        0        0      581 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0264_reduce_last_empty.py
+-rw-r--r--   0        0        0     3251 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0273_path_for_with_field.py
+-rw-r--r--   0        0        0      743 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0286_broadcast_single_value_with_field.py
+-rw-r--r--   0        0        0     2205 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0290_bug_fixes_for_hats.py
+-rw-r--r--   0        0        0     4806 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0315_integerindex.py
+-rw-r--r--   0        0        0     5745 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0331_pandas_indexedarray.py
+-rw-r--r--   0        0        0     1257 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0334_fully_broadcastable_where.py
+-rw-r--r--   0        0        0      566 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0339_highlevel_sorting_function.py
+-rw-r--r--   0        0        0     6757 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0348_form_keys.py
+-rw-r--r--   0        0        0     4523 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0355_mixins.py
+-rw-r--r--   0        0        0    10396 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0395_complex_type_arrays.py
+-rw-r--r--   0        0        0     4934 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0395_fix_numba_indexedarray.py
+-rw-r--r--   0        0        0     3212 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0397_arrays_as_constants_in_numba.py
+-rw-r--r--   0        0        0    14529 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
+-rw-r--r--   0        0        0    22467 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0404_array_validity_check.py
+-rw-r--r--   0        0        0    14282 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0410_fix_argminmax_positions_for_missing_values.py
+-rw-r--r--   0        0        0    17455 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0437_stream_of_many_json_files.py
+-rw-r--r--   0        0        0    32921 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0447_preserve_regularness_in_reduce.py
+-rw-r--r--   0        0        0    24075 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0449_merge_many_arrays_in_one_pass.py
+-rw-r--r--   0        0        0     4059 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0493_zeros_ones_full_like.py
+-rw-r--r--   0        0        0     1606 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0496_provide_local_index.py
+-rw-r--r--   0        0        0     2059 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0499_getitem_indexedarray_bug.py
+-rw-r--r--   0        0        0     1286 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0504_block_ufuncs_for_strings.py
+-rw-r--r--   0        0        0     2926 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0511_copy_and_deepcopy.py
+-rw-r--r--   0        0        0     9119 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
+-rw-r--r--   0        0        0      365 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0546_fill_none_replacement_value_type.py
+-rw-r--r--   0        0        0     1102 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0549_numba_array_asarray.py
+-rw-r--r--   0        0        0     4268 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0557_min_max_initial_argument.py
+-rw-r--r--   0        0        0      537 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0559_fix_booleans_in_numba.py
+-rw-r--r--   0        0        0      636 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0572_numba_array_ndim.py
+-rw-r--r--   0        0        0     4901 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0582_propagate_context_in_broadcast_and_apply.py
+-rw-r--r--   0        0        0     1099 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0583_implement_unflatten_function.py
+-rw-r--r--   0        0        0     3084 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0590_allow_regulararray_size_zero.py
+-rw-r--r--   0        0        0     5957 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
+-rw-r--r--   0        0        0      478 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0627_behavior_from_dict_of_arrays.py
+-rw-r--r--   0        0        0     8205 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0652_tests_of_complex_numbers.py
+-rw-r--r--   0        0        0     2338 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0674_categorical_validation.py
+-rw-r--r--   0        0        0      750 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0713_getitem_field_should_simplify_optiontype.py
+-rw-r--r--   0        0        0     1242 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
+-rw-r--r--   0        0        0     1055 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0730_unflatten_axis_parameter.py
+-rw-r--r--   0        0        0     2569 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0733_run_lengths.py
+-rw-r--r--   0        0        0     2127 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0736_implement_argsort_for_strings.py
+-rw-r--r--   0        0        0      330 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0758_ak_zip_scallars.py
+-rw-r--r--   0        0        0     1122 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0766_prevent_combinations_of_characters.py
+-rw-r--r--   0        0        0    26349 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0773_typeparser.py
+-rw-r--r--   0        0        0      779 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
+-rw-r--r--   0        0        0      871 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0794_ak_cartesian_on_empty_array.py
+-rw-r--r--   0        0        0     1148 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0803_argsort_fix_type.py
+-rw-r--r--   0        0        0     1364 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0806_empty_lists_cartesian_fix.py
+-rw-r--r--   0        0        0     6311 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0813_full_like_dtype_arg.py
+-rw-r--r--   0        0        0     1661 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0815_broadcast_union_types_to_all_possibilities.py
+-rw-r--r--   0        0        0      488 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0819_issue.py
+-rw-r--r--   0        0        0      682 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0828_arrow_datatype_null.py
+-rw-r--r--   0        0        0    23609 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0835_datetime_type.py
+-rw-r--r--   0        0        0      676 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0835_datetime_type_pandas.py
+-rw-r--r--   0        0        0     4662 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0835_datetime_type_pyarrow.py
+-rw-r--r--   0        0        0      680 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0850_argsort_mask_array.py
+-rw-r--r--   0        0        0      449 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0863_is_none_numpy_array.py
+-rw-r--r--   0        0        0     1029 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0866_getitem_field_and_flatten_unions.py
+-rw-r--r--   0        0        0      929 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0875_arrow_null_type.py
+-rw-r--r--   0        0        0      901 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0879_non_primitive_with_field.py
+-rw-r--r--   0        0        0      563 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0884_index_and_identifier_refactoring.py
+-rw-r--r--   0        0        0     1086 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0889_ptp.py
+-rw-r--r--   0        0        0    53355 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0896_content_classes_refactoring.py
+-rw-r--r--   0        0        0     1751 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0898_unzip_heterogeneous_records.py
+-rw-r--r--   0        0        0      421 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
+-rw-r--r--   0        0        0      530 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0905_leading_zeros_in_unflatten.py
+-rw-r--r--   0        0        0     1048 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0906_arrow_fixed_size_list_type.py
+-rw-r--r--   0        0        0      666 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0910_unflatten_counts_relation.py
+-rw-r--r--   0        0        0     5261 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0912_packed.py
+-rw-r--r--   0        0        0   115760 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0914_types_and_forms.py
+-rw-r--r--   0        0        0     1877 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0916_datetime_values_astype.py
+-rw-r--r--   0        0        0     5522 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0927_numpy_array_nbytes.py
+-rw-r--r--   0        0        0      709 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0930_bug_in_unionarray_purelist_parameter.py
+-rw-r--r--   0        0        0     1627 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0945_argsort_sort_nan_array.py
+-rw-r--r--   0        0        0    28028 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0958_new_forms_must_accept_old_form_json.py
+-rw-r--r--   0        0        0    28284 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0959__getitem_array_implementation.py
+-rw-r--r--   0        0        0      651 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0975_mask_multidimensional_numpy_array.py
+-rw-r--r--   0        0        0      644 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0979_where_multidimentional_numpy_array.py
+-rw-r--r--   0        0        0     5803 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0982_missing_case_in_nonlocal_reducers.py
+-rw-r--r--   0        0        0     1976 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0984_ravel.py
+-rw-r--r--   0        0        0     1806 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_0992_correct_ptp_unmasking.py
+-rw-r--r--   0        0        0     2100 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
+-rw-r--r--   0        0        0      429 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1006_packed_regular_array_zero_size.py
+-rw-r--r--   0        0        0      416 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1007_from_buffers_empty_ndarray.py
+-rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1017_numpyarray_broadcast.py
+-rw-r--r--   0        0        0      785 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1030_mixin_class_name.py
+-rw-r--r--   0        0        0    52114 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1031_start_getitem_next.py
+-rw-r--r--   0        0        0    18007 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1031b_start_getitem_next_specialized.py
+-rw-r--r--   0        0        0     1146 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1049_concatenate_single_array.py
+-rw-r--r--   0        0        0     1559 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1055_fill_none_numpy_dimension.py
+-rw-r--r--   0        0        0    42250 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1059_localindex.py
+-rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1066_to_numpy_masked_structured_array.py
+-rw-r--r--   0        0        0      685 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1071_mask_identity_false_should_not_return_option_type.py
+-rw-r--r--   0        0        0    27714 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1072_sort.py
+-rw-r--r--   0        0        0    44140 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1074_combinations.py
+-rw-r--r--   0        0        0     5181 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1075_validityerror.py
+-rw-r--r--   0        0        0      273 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1106_argminmax_axis_None_missing_values.py
+-rw-r--r--   0        0        0    25531 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1110_type_tracer_1.py
+-rw-r--r--   0        0        0     1870 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1116_project_maskedarrays.py
+-rw-r--r--   0        0        0    28234 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1125_to_arrow_from_arrow.py
+-rw-r--r--   0        0        0     6276 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1132_utility_methods_for_highlevel_functions.py
+-rw-r--r--   0        0        0    21098 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1134_from_buffers_to_buffers.py
+-rw-r--r--   0        0        0    57322 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1135_rpad_operation.py
+-rw-r--r--   0        0        0     4639 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1136_regulararray_zeros_in_shape.py
+-rw-r--r--   0        0        0    10487 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1137_num.py
+-rw-r--r--   0        0        0    10222 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1142_numbers_to_type.py
+-rw-r--r--   0        0        0     2559 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1149_datetime_sort.py
+-rw-r--r--   0        0        0      630 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1154_arrow_tables_should_preserve_parameters.py
+-rw-r--r--   0        0        0    27983 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1162_ak_from_json_schema.py
+-rw-r--r--   0        0        0      766 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1183_bugs_found_by_dask_project_2.py
+-rw-r--r--   0        0        0     1286 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1189_fix_singletons_for_non_optional_data.py
+-rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1192_iterables_in___array_function__.py
+-rw-r--r--   0        0        0      608 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1193_is_none_nested_option.py
+-rw-r--r--   0        0        0     2601 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1233_ak_with_name.py
+-rw-r--r--   0        0        0    26467 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1240_v2_implementation_of_numba_1.py
+-rw-r--r--   0        0        0     1146 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1259_simplify_optiontype.py
+-rw-r--r--   0        0        0     1560 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1260_simplify_masked_option_types.py
+-rw-r--r--   0        0        0      681 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1271_fix_4D_reducers.py
+-rw-r--r--   0        0        0    33003 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1294_to_and_from_parquet.py
+-rw-r--r--   0        0        0     1945 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
+-rw-r--r--   0        0        0    62340 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1300_awkward_to_cpp_converter_with_cling.py
+-rw-r--r--   0        0        0    39474 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1300b_same_for_numba.py
+-rw-r--r--   0        0        0      367 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1305_mixed_awkward_numpy_slicing.py
+-rw-r--r--   0        0        0     1702 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1308_zip_after_option.py
+-rw-r--r--   0        0        0     1703 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1318_array_function_types.py
+-rw-r--r--   0        0        0     1730 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1320_mask_identity_defaults.py
+-rw-r--r--   0        0        0      647 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1344_broadcast_arrays_depth_limit.py
+-rw-r--r--   0        0        0     6621 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1345_avro_reader.py
+-rw-r--r--   0        0        0     4562 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1351_is_tuple.py
+-rw-r--r--   0        0        0     8362 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1374_to_rdataframe.py
+-rw-r--r--   0        0        0     1755 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1377_ravel_string.py
+-rw-r--r--   0        0        0     1468 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1379_reducers_with_axis_None_and_typetracers.py
+-rw-r--r--   0        0        0     1384 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1399_from_jax.py
+-rw-r--r--   0        0        0     1227 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1399_to_jax.py
+-rw-r--r--   0        0        0      297 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1400_with_name_record.py
+-rw-r--r--   0        0        0      449 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1403_from_numpy_strings.py
+-rw-r--r--   0        0        0     3470 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1405_slicing_untested_cases.py
+-rw-r--r--   0        0        0     6909 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1415_behaviour_forwarding.py
+-rw-r--r--   0        0        0    18809 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1440_start_v2_to_parquet.py
+-rw-r--r--   0        0        0    14402 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1447_jax_autodiff_slices_ufuncs.py
+-rw-r--r--   0        0        0     8591 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1449_v2_to_json_from_json_functions.py
+-rw-r--r--   0        0        0      692 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1453_write_single_records_to_parquet.py
+-rw-r--r--   0        0        0     9828 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1473_from_rdataframe.py
+-rw-r--r--   0        0        0    24648 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1477_generator_entry_type_as_rvec.py
+-rw-r--r--   0        0        0     3579 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1490_jax_reducers_combinations.py
+-rw-r--r--   0        0        0     3905 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1502_getitem_jagged_issue1406.py
+-rw-r--r--   0        0        0     1733 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1504_typetracer_like.py
+-rw-r--r--   0        0        0     4913 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1508_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     2186 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1511_set_attribute.py
+-rw-r--r--   0        0        0      754 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1539_isnone_axis_check_issue1417.py
+-rw-r--r--   0        0        0     1570 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1559_fix_ufuncs_records_1439.py
+-rw-r--r--   0        0        0      990 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1565_axis_wrap_if_negative_record.py
+-rw-r--r--   0        0        0     1085 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1567_fix_longlong_in_Index.py
+-rw-r--r--   0        0        0     3022 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1568_fix_lengths_empty_regular_slices.py
+-rw-r--r--   0        0        0      385 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1578_to_arrow_empty_recordarray.py
+-rw-r--r--   0        0        0     5911 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1586_concatenate_should_preserve_regulararray.py
+-rw-r--r--   0        0        0      216 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1593_empty_slice_list_record.py
+-rw-r--r--   0        0        0     7260 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1604_preserve_form_in_concatenate.py
+-rw-r--r--   0        0        0     3636 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1607_no_reducers_on_records.py
+-rw-r--r--   0        0        0    10035 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1613_generator_tolayout_records.py
+-rw-r--r--   0        0        0      727 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1619_from_parquet_empty_field.py
+-rw-r--r--   0        0        0     6024 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1620_layout_builders.py
+-rw-r--r--   0        0        0     8122 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1625_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0      770 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1642_from_iter_of_tuples.py
+-rw-r--r--   0        0        0      389 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1644_concatenate_zeros_length.py
+-rw-r--r--   0        0        0     4317 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1650_Record_to_list_should_listify_itself.py
+-rw-r--r--   0        0        0      560 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1671_categorical_type.py
+-rw-r--r--   0        0        0    11761 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1672_broadcast_parameters.py
+-rw-r--r--   0        0        0     4453 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1677_array_builder_in_numba.py
+-rw-r--r--   0        0        0      544 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1685_IndexedArray_project_parameters.py
+-rw-r--r--   0        0        0      778 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1686_UnionArray_simplified_preserve_parameters.py
+-rw-r--r--   0        0        0      936 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1688_pack_categorical.py
+-rw-r--r--   0        0        0      525 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1703_fill_none_typetracer.py
+-rw-r--r--   0        0        0     1743 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1707_broadcast_parameters_ufunc.py
+-rw-r--r--   0        0        0      512 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1709_ak_array_constructor_behavior.py
+-rw-r--r--   0        0        0      398 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1735_from_numpy_mask.py
+-rw-r--r--   0        0        0      577 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1747_bytemaskedarray_mergemany.py
+-rw-r--r--   0        0        0      824 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1753_indexedarray_merge_kernel.py
+-rw-r--r--   0        0        0     1480 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1762_jax_behavior_support.py
+-rw-r--r--   0        0        0      589 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1764_jax_jacobian.py
+-rw-r--r--   0        0        0      962 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1765_add_ioanas_test_of_to_arraylib.py
+-rw-r--r--   0        0        0     4790 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1766_record_form_fields.py
+-rw-r--r--   0        0        0     2905 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1781_rdataframe_snapshot.py
+-rw-r--r--   0        0        0      701 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1784_reduce_leading_sublist.py
+-rw-r--r--   0        0        0      567 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1790_reduce_regulararray.py
+-rw-r--r--   0        0        0     4191 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1791_reduce_trailing_sublist.py
+-rw-r--r--   0        0        0     1027 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1794_run_lengths_empty_sublist.py
+-rw-r--r--   0        0        0      407 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1823_fill_none_axis_none.py
+-rw-r--r--   0        0        0      481 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1826_ravel_preserve_none.py
+-rw-r--r--   0        0        0     1451 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1829_to_from_rdataframe_bool.py
+-rw-r--r--   0        0        0      588 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
+-rw-r--r--   0        0        0     1097 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1847_numpy_array_contiguous.py
+-rw-r--r--   0        0        0      681 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
+-rw-r--r--   0        0        0     1640 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1867_pass_behavior_through_combinations.py
+-rw-r--r--   0        0        0    17239 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1904_drop_none.py
+-rw-r--r--   0        0        0     3553 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1914_improved_axis_to_posaxis.py
+-rw-r--r--   0        0        0     3444 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
+-rw-r--r--   0        0        0      921 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1930_unflatten_counts_checks.py
+-rw-r--r--   0        0        0      769 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1936_with_field_broadcasting.py
+-rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1940_ak_backend.py
+-rw-r--r--   0        0        0     1457 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1943_regular_indexing.py
+-rw-r--r--   0        0        0      188 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1944_to_numpy_empty_record_array.py
+-rw-r--r--   0        0        0     1131 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1960_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     3286 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1961_ak_without_field.py
+-rw-r--r--   0        0        0      280 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1978_akRecord_constructor_should_retain_type.py
+-rw-r--r--   0        0        0      349 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
+-rw-r--r--   0        0        0      371 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2008_ak_type_layout.py
+-rw-r--r--   0        0        0    10222 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2020_reduce_axis_none.py
+-rw-r--r--   0        0        0      803 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2021_check_TypeTracerArray_in_ak_where.py
+-rw-r--r--   0        0        0      645 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2023_from_rdataframe.py
+-rw-r--r--   0        0        0     2854 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
+-rw-r--r--   0        0        0     1219 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2047_ak_transform_regular_to_jagged.py
+-rw-r--r--   0        0        0      406 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2051_arraybuilder_behavior_propagation.py
+-rw-r--r--   0        0        0     1275 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2055_array_builder_check.py
+-rw-r--r--   0        0        0     1659 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2058_merge_numpy_array.py
+-rw-r--r--   0        0        0      708 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2064_fill_none_record.py
+-rw-r--r--   0        0        0      799 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2067_to_buffers_byteorder.py
+-rw-r--r--   0        0        0      741 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2070_to_layout_string.py
+-rw-r--r--   0        0        0     1172 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2071_unflatten_non_packed_counts.py
+-rw-r--r--   0        0        0      291 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2076_ak_unzip_record.py
+-rw-r--r--   0        0        0      545 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2078_array_function_wrap.py
+-rw-r--r--   0        0        0      589 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2082_broadcast_zero_size.py
+-rw-r--r--   0        0        0     2765 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2096_ak_scalar_type.py
+-rw-r--r--   0        0        0      977 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2101_pickle_behavior_class.py
+-rw-r--r--   0        0        0      519 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2104_numpy_merge_option.py
+-rw-r--r--   0        0        0     2715 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2106_pickle_class.py
+-rw-r--r--   0        0        0      722 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2108_fill_none_indexed.py
+-rw-r--r--   0        0        0     2100 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2115_fix_up_typetracers.py
+-rw-r--r--   0        0        0      487 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2120_missing_field_error.py
+-rw-r--r--   0        0        0     1110 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2125_type_of_scalar.py
+-rw-r--r--   0        0        0     1893 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2150_typetracer_high_level_ufunc.py
+-rw-r--r--   0        0        0     1898 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2179_parameter_merging_rules.py
+-rw-r--r--   0        0        0      510 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2181_with_name_len.py
+-rw-r--r--   0        0        0     2957 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2185_merge_union_of_records.py
+-rw-r--r--   0        0        0      528 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
+-rw-r--r--   0        0        0     5548 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2198_almost_equal.py
+-rw-r--r--   0        0        0     1252 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2202_filter_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0     1453 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2214_offset_bool_index.py
+-rw-r--r--   0        0        0      334 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2219_flatten_empty.py
+-rw-r--r--   0        0        0      663 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2226_slice_regulararray_typetracer.py
+-rw-r--r--   0        0        0     1728 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2229_getitem_range_slice.py
+-rw-r--r--   0        0        0     4003 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2234_from_rdataframe_keep_order.py
+-rw-r--r--   0        0        0     3962 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2236_merge_union_of_records_option.py
+-rw-r--r--   0        0        0      485 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2240_merge_union_parameters.py
+-rw-r--r--   0        0        0     1338 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2240_simplify_merge_as_union.py
+-rw-r--r--   0        0        0      512 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2246_slice_not_packed.py
+-rw-r--r--   0        0        0      733 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2250_full_like_bool.py
+-rw-r--r--   0        0        0     1835 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2258_from_rdataframe_with_arguments.py
+-rw-r--r--   0        0        0      492 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2259_run_lengths_typetracer.py
+-rw-r--r--   0        0        0      560 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2263_to_packed_list.py
+-rw-r--r--   0        0        0      877 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2266_fix_nan_to_num.py
+-rw-r--r--   0        0        0      909 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2267_broadcast_fields.py
+-rw-r--r--   0        0        0     1336 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2293_unflatten_typetracer.py
+-rw-r--r--   0        0        0      406 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2294_view_unknown_scalar.py
+-rw-r--r--   0        0        0     2262 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2297_common_backend.py
+-rw-r--r--   0        0        0      455 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2304_index_typetracer.py
+-rw-r--r--   0        0        0      648 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2305_nep_18_lazy_conversion.py
+-rw-r--r--   0        0        0     2929 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2306_cppyy_git.py
+-rw-r--r--   0        0        0     4386 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2319_from_buffers_array.py
+-rw-r--r--   0        0        0      721 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2327_array_interface.py
+-rw-r--r--   0        0        0     1728 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2329_cartesian_broadcasting_fixes.py
+-rw-r--r--   0        0        0      489 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2346_broadcast_depth_limit.py
+-rw-r--r--   0        0        0    15615 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2349_growablebuffer_in_numba.py
+-rw-r--r--   0        0        0      618 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2354_ufunc_same_backend.py
+-rw-r--r--   0        0        0      647 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2355_to_backend_record.py
+-rw-r--r--   0        0        0     1435 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2361_typetracer_asarray_nd.py
+-rw-r--r--   0        0        0     2921 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2368_type_is_equal.py
+-rw-r--r--   0        0        0     5259 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2373_unzip_touching.py
+-rw-r--r--   0        0        0     5857 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2374_cartesian_touching.py
+-rw-r--r--   0        0        0     1037 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2385_with_field_empty_record.py
+-rw-r--r--   0        0        0      926 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2395_copy_asarray_touch.py
+-rw-r--r--   0        0        0      212 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2407_broadcast_no_arrays.py
+-rw-r--r--   0        0        0     1070 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2410_string_broadcast.py
+-rw-r--r--   0        0        0      800 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2411_cartesian_axis_validation.py
+-rw-r--r--   0        0        0      704 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2417_bytemasked_singletons.py
+-rw-r--r--   0        0        0      351 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2418_union_broadcast_unknown.py
+-rw-r--r--   0        0        0     1563 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2424_almost_equal_union_record.py
+-rw-r--r--   0        0        0      545 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/test_2426_is_equal_to.py
+-rw-r--r--   0        0        0      128 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/array_enum_test_data.avro
+-rw-r--r--   0        0        0      176 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/array_string_test_data.avro
+-rw-r--r--   0        0        0      152 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/array_test_data.avro
+-rw-r--r--   0        0        0      115 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/bool_test_data.avro
+-rw-r--r--   0        0        0      130 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/bytes_test_data.avro
+-rw-r--r--   0        0        0      158 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/double_test_data.avro
+-rw-r--r--   0        0        0      191 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/enum_null_test_data.avro
+-rw-r--r--   0        0        0      180 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/enum_test_data.avro
+-rw-r--r--   0        0        0      218 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/fixed_test_data.avro
+-rw-r--r--   0        0        0      116 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/float_test_data.avro
+-rw-r--r--   0        0        0      106 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/int_null_test_data.avro
+-rw-r--r--   0        0        0      128 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/int_string_null_test_data.avro
+-rw-r--r--   0        0        0       89 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/int_test_data.avro
+-rw-r--r--   0        0        0     3035 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2871 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/list-depths-records.parquet
+-rw-r--r--   0        0        0      497 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/list-depths-simple.parquet
+-rw-r--r--   0        0        0     1136 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/list-depths-strings.parquet
+-rw-r--r--   0        0        0     1060 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/list-depths.parquet
+-rw-r--r--   0        0        0      465 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/list-lengths.parquet
+-rw-r--r--   0        0        0      116 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/long_test_data.avro
+-rw-r--r--   0        0        0      681 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/nonnullable-depths.parquet
+-rw-r--r--   0        0        0       75 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/null_test_data.avro
+-rw-r--r--   0        0        0      719 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/nullable-depths.parquet
+-rw-r--r--   0        0        0      635 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/nullable-levels.parquet
+-rw-r--r--   0        0        0     3050 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/nullable-list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2926 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/nullable-list-depths-records.parquet
+-rw-r--r--   0        0        0     1179 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/nullable-list-depths-strings.parquet
+-rw-r--r--   0        0        0     1101 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/nullable-list-depths.parquet
+-rw-r--r--   0        0        0      430 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/nullable-record-primitives-simple.parquet
+-rw-r--r--   0        0        0     1181 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/nullable-record-primitives.parquet
+-rw-r--r--   0        0        0     1193 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/record-primitives.parquet
+-rw-r--r--   0        0        0      326 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/record_0_test_data.avro
+-rw-r--r--   0        0        0      368 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/record_1_test_data.avro
+-rw-r--r--   0        0        0      263 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/record_null_test_data.avro
+-rw-r--r--   0        0        0      423 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/record_test_data.avro
+-rw-r--r--   0        0        0      116 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/string_null_test_data.avro
+-rw-r--r--   0        0        0      125 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/string_test_data.avro
+-rw-r--r--   0        0        0      544 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/test-nan-inf.json
+-rw-r--r--   0        0        0      155 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/test-record-array.json
+-rw-r--r--   0        0        0      803 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/test-two-arrays.json
+-rw-r--r--   0        0        0      535 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/test.json
+-rw-r--r--   0        0        0      180 2023-04-24 16:57:22.000000 awkward-2.1.4/tests/samples/zero-record-batches.parquet
+-rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.1.4/tests-cuda/__init__.py
+-rw-r--r--   0        0        0     7072 2023-04-24 16:57:22.000000 awkward-2.1.4/tests-cuda/test_1276_cuda_num.py
+-rw-r--r--   0        0        0     9911 2023-04-24 16:57:22.000000 awkward-2.1.4/tests-cuda/test_1276_cuda_transfers.py
+-rw-r--r--   0        0        0     1197 2023-04-24 16:57:22.000000 awkward-2.1.4/tests-cuda/test_1276_cupy_interop.py
+-rw-r--r--   0        0        0     1782 2023-04-24 16:57:22.000000 awkward-2.1.4/tests-cuda/test_1276_from_cupy.py
+-rw-r--r--   0        0        0    42786 2023-04-24 16:57:22.000000 awkward-2.1.4/tests-cuda/test_1300_same_for_numba_cuda.py
+-rw-r--r--   0        0        0      834 2023-04-24 16:57:22.000000 awkward-2.1.4/tests-cuda/test_1381_check_errors.py
+-rw-r--r--   0        0        0    11252 2023-04-24 16:57:22.000000 awkward-2.1.4/tests-cuda/test_1809_array_cuda_jit.py
+-rw-r--r--   0        0        0     2212 2023-04-24 16:57:22.000000 awkward-2.1.4/.gitignore
+-rw-r--r--   0        0        0     1520 2023-04-24 16:57:22.000000 awkward-2.1.4/LICENSE
+-rw-r--r--   0        0        0     8479 2023-04-24 16:57:22.000000 awkward-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6933 2023-04-24 16:57:22.000000 awkward-2.1.4/PKG-INFO
```

### Comparing `awkward-2.1.3/CITATION.cff` & `awkward-2.1.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/CONTRIBUTING.md` & `awkward-2.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/README.md` & `awkward-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/_toc.yml` & `awkward-2.1.4/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/conf.py` & `awkward-2.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/index.md` & `awkward-2.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/prepare_docstrings.py` & `awkward-2.1.4/docs/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/redirects-user-guide.json` & `awkward-2.1.4/docs/redirects-user-guide.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/redirects.json` & `awkward-2.1.4/docs/redirects.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/_static/css/awkward.css` & `awkward-2.1.4/docs/_static/css/awkward.css`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/getting-started/community-tutorials.md` & `awkward-2.1.4/docs/getting-started/community-tutorials.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/getting-started/index.md` & `awkward-2.1.4/docs/getting-started/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/getting-started/papers-and-talks.md` & `awkward-2.1.4/docs/getting-started/papers-and-talks.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/getting-started/demo/what-is-an-awkward-array.ipynb` & `awkward-2.1.4/docs/getting-started/demo/what-is-an-awkward-array.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/image/example-hierarchy.svg` & `awkward-2.1.4/docs/image/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/reference/ak.behavior.rst` & `awkward-2.1.4/docs/reference/ak.behavior.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/reference/ak.builder.ArrayBuilder.rst` & `awkward-2.1.4/docs/reference/ak.builder.ArrayBuilder.rst`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 The low-level ArrayBuilder that builds :class:`ak.contents.Content` arrays. This
 object is wrapped by :class:`ak.ArrayBuilder`.
 
 (Method names in the high-level interface have been changed to include
 underscores after "begin" and "end," but that hasn't happened in the
 low-level interface, yet or possibly at all.)
 
-.. py:class:: ArrayBuilder(initial=1024, resize=1.5)
+.. py:class:: ArrayBuilder(initial=1024, resize=8)
 
 .. py:method:: ArrayBuilder.__getitem__(where)
 
-.. py:method:: ArrayBuilder.__init__(initial=1024, resize=1.5)
+.. py:method:: ArrayBuilder.__init__(initial=1024, resize=8)
 
 .. py:method:: ArrayBuilder.__iter__()
 
 .. py:method:: ArrayBuilder.__len__()
 
 .. py:method:: ArrayBuilder.__repr__()
```

### Comparing `awkward-2.1.3/docs/reference/awkwardforth.rst` & `awkward-2.1.4/docs/reference/awkwardforth.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/reference/toctree.txt` & `awkward-2.1.4/docs/reference/toctree.txt`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/10-minutes-to-awkward-array.md` & `awkward-2.1.4/docs/user-guide/10-minutes-to-awkward-array.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-combinatorics-best-match.md` & `awkward-2.1.4/docs/user-guide/how-to-combinatorics-best-match.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-combinatorics-cartesian-combinations.md` & `awkward-2.1.4/docs/user-guide/how-to-combinatorics-cartesian-combinations.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-convert-arrow.md` & `awkward-2.1.4/docs/user-guide/how-to-convert-arrow.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-convert-buffers.md` & `awkward-2.1.4/docs/user-guide/how-to-convert-buffers.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-convert-json.md` & `awkward-2.1.4/docs/user-guide/how-to-convert-json.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-convert-numpy.md` & `awkward-2.1.4/docs/user-guide/how-to-convert-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-convert-pandas.md` & `awkward-2.1.4/docs/user-guide/how-to-convert-pandas.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-convert-python.md` & `awkward-2.1.4/docs/user-guide/how-to-convert-python.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-convert-rdataframe.md` & `awkward-2.1.4/docs/user-guide/how-to-convert-rdataframe.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-create-arraybuilder.md` & `awkward-2.1.4/docs/user-guide/how-to-create-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-create-constructors.md` & `awkward-2.1.4/docs/user-guide/how-to-create-constructors.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-create-lists.md` & `awkward-2.1.4/docs/user-guide/how-to-create-lists.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-create-missing.md` & `awkward-2.1.4/docs/user-guide/how-to-create-missing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-create-records.md` & `awkward-2.1.4/docs/user-guide/how-to-create-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-create-strings.md` & `awkward-2.1.4/docs/user-guide/how-to-create-strings.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-create-unflatten-group.md` & `awkward-2.1.4/docs/user-guide/how-to-create-unflatten-group.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-examine-checking-validity.md` & `awkward-2.1.4/docs/user-guide/how-to-examine-checking-validity.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-examine-list-fields.md` & `awkward-2.1.4/docs/user-guide/how-to-examine-list-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-examine-simple-slicing.md` & `awkward-2.1.4/docs/user-guide/how-to-examine-simple-slicing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-examine-single-item.md` & `awkward-2.1.4/docs/user-guide/how-to-examine-single-item.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-examine-type.md` & `awkward-2.1.4/docs/user-guide/how-to-examine-type.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-filter-cut-mask.md` & `awkward-2.1.4/docs/user-guide/how-to-filter-cut-mask.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-filter-masked.md` & `awkward-2.1.4/docs/user-guide/how-to-filter-masked.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-filter-num.md` & `awkward-2.1.4/docs/user-guide/how-to-filter-num.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-filter-ragged.md` & `awkward-2.1.4/docs/user-guide/how-to-filter-ragged.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-math-argminmax.md` & `awkward-2.1.4/docs/user-guide/how-to-math-argminmax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-math-broadcasting.md` & `awkward-2.1.4/docs/user-guide/how-to-math-broadcasting.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-math-gpu.md` & `awkward-2.1.4/docs/user-guide/how-to-math-gpu.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-math-numpy.md` & `awkward-2.1.4/docs/user-guide/how-to-math-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-math-reducing.md` & `awkward-2.1.4/docs/user-guide/how-to-math-reducing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-math-statistics.md` & `awkward-2.1.4/docs/user-guide/how-to-math-statistics.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-restructure-add-fields.md` & `awkward-2.1.4/docs/user-guide/how-to-restructure-add-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-restructure-concatenate.md` & `awkward-2.1.4/docs/user-guide/how-to-restructure-concatenate.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-restructure-flatten.md` & `awkward-2.1.4/docs/user-guide/how-to-restructure-flatten.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-restructure-pad.md` & `awkward-2.1.4/docs/user-guide/how-to-restructure-pad.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-restructure-rename-records.md` & `awkward-2.1.4/docs/user-guide/how-to-restructure-rename-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-restructure-sort.md` & `awkward-2.1.4/docs/user-guide/how-to-restructure-sort.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-restructure-zip-project.md` & `awkward-2.1.4/docs/user-guide/how-to-restructure-zip-project.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-specialize-differentiate-jax.md` & `awkward-2.1.4/docs/user-guide/how-to-specialize-differentiate-jax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-specialize-in-numba.md` & `awkward-2.1.4/docs/user-guide/how-to-specialize-in-numba.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-specialize-lorentz.md` & `awkward-2.1.4/docs/user-guide/how-to-specialize-lorentz.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-specialize-override-numpy.md` & `awkward-2.1.4/docs/user-guide/how-to-specialize-override-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-specialize-subclass.md` & `awkward-2.1.4/docs/user-guide/how-to-specialize-subclass.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-use-header-only-layoutbuilder.md` & `awkward-2.1.4/docs/user-guide/how-to-use-header-only-layoutbuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-use-in-numba-arraybuilder.md` & `awkward-2.1.4/docs/user-guide/how-to-use-in-numba-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-use-in-numba-cuda.ipynb` & `awkward-2.1.4/docs/user-guide/how-to-use-in-numba-cuda.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs/user-guide/how-to-use-in-numba-features.md` & `awkward-2.1.4/docs/user-guide/how-to-use-in-numba-features.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/panel-data-analysts.png` & `awkward-2.1.4/docs-img/panel-data-analysts.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/panel-data-analysts.svg` & `awkward-2.1.4/docs-img/panel-data-analysts.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/panel-developers.png` & `awkward-2.1.4/docs-img/panel-developers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/panel-developers.svg` & `awkward-2.1.4/docs-img/panel-developers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/panel-doxygen.png` & `awkward-2.1.4/docs-img/panel-doxygen.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/panel-sphinx.png` & `awkward-2.1.4/docs-img/panel-sphinx.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/panel-tutorials-alternate.png` & `awkward-2.1.4/docs-img/panel-tutorials-alternate.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/panel-tutorials.png` & `awkward-2.1.4/docs-img/panel-tutorials.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/awkward-1-0-layers.pdf` & `awkward-2.1.4/docs-img/diagrams/awkward-1-0-layers.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/awkward-1-0-layers.png` & `awkward-2.1.4/docs-img/diagrams/awkward-1-0-layers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/awkward-1-0-layers.svg` & `awkward-2.1.4/docs-img/diagrams/awkward-1-0-layers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/awkward-timeline.pdf` & `awkward-2.1.4/docs-img/diagrams/awkward-timeline.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/awkward-timeline.png` & `awkward-2.1.4/docs-img/diagrams/awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/awkward-timeline.svg` & `awkward-2.1.4/docs-img/diagrams/awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.png` & `awkward-2.1.4/docs-img/diagrams/awkward-uproot-timeline-pip-github.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg` & `awkward-2.1.4/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip.png` & `awkward-2.1.4/docs-img/diagrams/awkward-uproot-timeline-pip.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip.svg` & `awkward-2.1.4/docs-img/diagrams/awkward-uproot-timeline-pip.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline.png` & `awkward-2.1.4/docs-img/diagrams/awkward-uproot-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline.svg` & `awkward-2.1.4/docs-img/diagrams/awkward-uproot-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/cartoon-broadcasting.png` & `awkward-2.1.4/docs-img/diagrams/cartoon-broadcasting.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/cartoon-broadcasting.svg` & `awkward-2.1.4/docs-img/diagrams/cartoon-broadcasting.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/cartoon-cartesian.png` & `awkward-2.1.4/docs-img/diagrams/cartoon-cartesian.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/cartoon-cartesian.svg` & `awkward-2.1.4/docs-img/diagrams/cartoon-cartesian.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/cartoon-combinations.png` & `awkward-2.1.4/docs-img/diagrams/cartoon-combinations.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/cartoon-combinations.svg` & `awkward-2.1.4/docs-img/diagrams/cartoon-combinations.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/cartoon-schematic.png` & `awkward-2.1.4/docs-img/diagrams/cartoon-schematic.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/cartoon-schematic.svg` & `awkward-2.1.4/docs-img/diagrams/cartoon-schematic.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/example-array.svg` & `awkward-2.1.4/docs-img/diagrams/example-array.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/example-hierarchy.png` & `awkward-2.1.4/docs-img/diagrams/example-hierarchy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/example-hierarchy.svg` & `awkward-2.1.4/docs-img/diagrams/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/example-reduction-sum-only.svg` & `awkward-2.1.4/docs-img/diagrams/example-reduction-sum-only.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/example-reduction-sum.svg` & `awkward-2.1.4/docs-img/diagrams/example-reduction-sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/example-reduction.png` & `awkward-2.1.4/docs-img/diagrams/example-reduction.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/example-reduction.svg` & `awkward-2.1.4/docs-img/diagrams/example-reduction.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/git-strategy.pdf` & `awkward-2.1.4/docs-img/diagrams/git-strategy.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/git-strategy.png` & `awkward-2.1.4/docs-img/diagrams/git-strategy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/git-strategy.svg` & `awkward-2.1.4/docs-img/diagrams/git-strategy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/how-it-works-muons.png` & `awkward-2.1.4/docs-img/diagrams/how-it-works-muons.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/how-it-works-muons.svg` & `awkward-2.1.4/docs-img/diagrams/how-it-works-muons.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/how-it-works.svg` & `awkward-2.1.4/docs-img/diagrams/how-it-works.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/sorting-axis.svg` & `awkward-2.1.4/docs-img/diagrams/sorting-axis.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/reducers/all.svg` & `awkward-2.1.4/docs-img/diagrams/reducers/all.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/reducers/any.svg` & `awkward-2.1.4/docs-img/diagrams/reducers/any.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/reducers/argmax.svg` & `awkward-2.1.4/docs-img/diagrams/reducers/argmax.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/reducers/argmin.svg` & `awkward-2.1.4/docs-img/diagrams/reducers/argmin.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/reducers/count.svg` & `awkward-2.1.4/docs-img/diagrams/reducers/count.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/reducers/count_nonzero.svg` & `awkward-2.1.4/docs-img/diagrams/reducers/count_nonzero.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/reducers/max.svg` & `awkward-2.1.4/docs-img/diagrams/reducers/max.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/reducers/min.svg` & `awkward-2.1.4/docs-img/diagrams/reducers/min.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/reducers/product.svg` & `awkward-2.1.4/docs-img/diagrams/reducers/product.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/diagrams/reducers/sum.svg` & `awkward-2.1.4/docs-img/diagrams/reducers/sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/logo/favicon.ico` & `awkward-2.1.4/docs-img/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/logo/logo-300px-white.png` & `awkward-2.1.4/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/logo/logo-300px.png` & `awkward-2.1.4/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/logo/logo-600px.png` & `awkward-2.1.4/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/logo/logo.svg` & `awkward-2.1.4/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/photos/desire-path.jpg` & `awkward-2.1.4/docs-img/photos/desire-path.jpg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/plots/awkward-0-popularity.pdf` & `awkward-2.1.4/docs-img/plots/awkward-0-popularity.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/plots/awkward-0-popularity.png` & `awkward-2.1.4/docs-img/plots/awkward-0-popularity.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/plots/awkward-0-popularity.svg` & `awkward-2.1.4/docs-img/plots/awkward-0-popularity.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/plots/bikeroutes-scaling.svg` & `awkward-2.1.4/docs-img/plots/bikeroutes-scaling.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/docs-img/screenshots/github-issues-documentation.png` & `awkward-2.1.4/docs-img/screenshots/github-issues-documentation.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/__init__.py` & `awkward-2.1.4/src/awkward/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_behavior.py` & `awkward-2.1.4/src/awkward/_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_broadcasting.py` & `awkward-2.1.4/src/awkward/_broadcasting.py`

 * *Files 1% similar despite different names*

```diff
@@ -813,30 +813,31 @@
             IndexedOptionArray.simplified(index, x, parameters=p)
             for x, p in zip(outcontent, parameters)
         )
 
     def broadcast_any_union():
         if not backend.nplike.known_data:
             # assert False
-            union_num_contents, length = [], None
+            union_num_contents = []
+            length = None
             for x in contents:
                 if x.is_union:
                     x._touch_data(recursive=False)
                     union_num_contents.append(len(x.contents))
                     if length is None:
-                        length = x.tags.data.shape[0]
-            assert length is not unknown_length
+                        length = x.length
 
             all_combos = list(
                 itertools.product(*[range(x) for x in union_num_contents])
             )
 
             tags = backend.index_nplike.empty(length, dtype=np.int8)
             index = backend.index_nplike.empty(length, dtype=np.int64)
-            numoutputs, outcontents = None, []
+            numoutputs = None
+            outcontents = []
             for combo in all_combos:
                 nextinputs = []
                 i = 0
                 for x in inputs:
                     if isinstance(x, UnionArray):
                         nextinputs.append(x._contents[combo[i]])
                         i += 1
@@ -852,21 +853,17 @@
                         copy.copy(depth_context),
                         lateral_context,
                         behavior,
                         options,
                     )
                 )
                 assert isinstance(outcontents[-1], tuple)
-                if numoutputs is None:
-                    numoutputs = outcontents[-1].length
-                else:
-                    assert (
-                        numoutputs is unknown_length
-                        or outcontents[-1].length is unknown_length
-                    ) or numoutputs == outcontents[-1].length
+                if numoutputs is not None:
+                    assert numoutputs == len(outcontents[-1])
+                numoutputs = len(outcontents[-1])
 
             assert numoutputs is not None
 
         else:
             union_tags, union_num_contents, length = [], [], None
             for x in contents:
                 if x.is_union:
```

### Comparing `awkward-2.1.3/src/awkward/_do.py` & `awkward-2.1.4/src/awkward/_do.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import copy
 from collections.abc import Mapping, MutableMapping
 from numbers import Integral
 
 import awkward as ak
 from awkward._backends.backend import Backend
+from awkward._errors import AxisError
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._typing import Any, AxisMaybeNone, Literal
 from awkward.contents.content import ActionType, Content
 from awkward.forms import form
 from awkward.record import Record
 
 np = NumpyMetadata.instance()
@@ -150,44 +151,44 @@
 def unique(layout: Content, axis=None):
     if axis == -1 or axis is None:
         negaxis = axis if axis is None else -axis
         if negaxis is not None:
             branch, depth = layout.branch_depth
             if branch:
                 if negaxis <= 0:
-                    raise np.AxisError(
+                    raise AxisError(
                         "cannot use non-negative axis on a nested list structure "
                         "of variable depth (negative axis counts from the leaves "
                         "of the tree; non-negative from the root)"
                     )
                 if negaxis > depth:
-                    raise np.AxisError(
+                    raise AxisError(
                         "cannot use axis={} on a nested list structure that splits into "
                         "different depths, the minimum of which is depth={} from the leaves".format(
                             axis, depth
                         )
                     )
             else:
                 if negaxis <= 0:
                     negaxis = negaxis + depth
                 if not (0 < negaxis and negaxis <= depth):
-                    raise np.AxisError(
+                    raise AxisError(
                         "axis={} exceeds the depth of this array ({})".format(
                             axis, depth
                         )
                     )
 
         starts = ak.index.Index64.zeros(1, nplike=layout._backend.index_nplike)
         parents = ak.index.Index64.zeros(
             layout.length, nplike=layout._backend.index_nplike
         )
 
         return layout._unique(negaxis, starts, parents, 1)
 
-    raise np.AxisError(
+    raise AxisError(
         "unique expects axis 'None' or '-1', got axis={} that is not supported yet".format(
             axis
         )
     )
 
 
 def pad_none(
```

### Comparing `awkward-2.1.3/src/awkward/_errors.py` & `awkward-2.1.4/src/awkward/_errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from __future__ import annotations
 
 import sys
 import threading
 import warnings
 from collections.abc import Mapping, Sequence
 
+import numpy  # noqa: TID251
+
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._typing import TypeVar
 
 np = NumpyMetadata.instance()
 
 
 E = TypeVar("E", bound=Exception)
@@ -119,16 +121,14 @@
                     valuestr = repr(value)
                 else:
                     valuestr = repr(value[:57]) + "..."
             except Exception as err:
                 valuestr = f"repr-raised-{type(err).__name__}"
 
         elif isinstance(value, np.ndarray):
-            import numpy  # noqa: TID251
-
             if not numpy.__version__.startswith("1.13."):  # 'threshold' argument
                 prefix = f"{type(value).__module__}.{type(value).__name__}("
                 suffix = ")"
                 try:
                     valuestr = numpy.array2string(
                         value,
                         max_line_width=width - len(prefix) - len(suffix),
@@ -360,7 +360,10 @@
         version, date, will_be, message
     )
     warnings.warn(warning, category, stacklevel=stacklevel + 1)
 
 
 class FieldNotFoundError(IndexError):
     ...
+
+
+AxisError = numpy.AxisError
```

### Comparing `awkward-2.1.3/src/awkward/_kernels.py` & `awkward-2.1.4/src/awkward/_kernels.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_layout.py` & `awkward-2.1.4/src/awkward/_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 from collections.abc import Mapping
 
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._errors import AxisError
 from awkward._nplikes.dispatch import nplike_of
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
@@ -152,15 +153,15 @@
 
 
 def maybe_posaxis(layout, axis, depth):
     from awkward.record import Record
 
     if isinstance(layout, Record):
         if axis == 0:
-            raise np.AxisError("Record type at axis=0 is a scalar, not an array")
+            raise AxisError("Record type at axis=0 is a scalar, not an array")
         return maybe_posaxis(layout._array, axis, depth)
 
     if axis >= 0:
         return axis
 
     else:
         is_branching, additional_depth = layout.branch_depth
```

### Comparing `awkward-2.1.3/src/awkward/_lookup.py` & `awkward-2.1.4/src/awkward/_lookup.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_parameters.py` & `awkward-2.1.4/src/awkward/_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_prettyprint.py` & `awkward-2.1.4/src/awkward/_prettyprint.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_reducers.py` & `awkward-2.1.4/src/awkward/_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_regularize.py` & `awkward-2.1.4/src/awkward/_regularize.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_slicing.py` & `awkward-2.1.4/src/awkward/_slicing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_typetracer.py` & `awkward-2.1.4/src/awkward/_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_typing.py` & `awkward-2.1.4/src/awkward/_typing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_util.py` & `awkward-2.1.4/src/awkward/_util.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_v2.py` & `awkward-2.1.4/src/awkward/_v2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/cppyy.py` & `awkward-2.1.4/src/awkward/cppyy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/highlevel.py` & `awkward-2.1.4/src/awkward/highlevel.py`

 * *Files 0% similar despite different names*

```diff
@@ -2231,15 +2231,15 @@
         ]
 
     Note that this is a *general* method for building arrays; if the type is
     known in advance, more specialized procedures can be faster. This should
     be considered the "least effort" approach.
     """
 
-    def __init__(self, *, behavior=None, initial=1024, resize=1.5):
+    def __init__(self, *, behavior=None, initial=1024, resize=8):
         self._layout = _ext.ArrayBuilder(initial=initial, resize=resize)
         self.behavior = behavior
 
     @classmethod
     def _wrap(cls, layout, behavior=None):
         """
         Args:
```

### Comparing `awkward-2.1.3/src/awkward/index.py` & `awkward-2.1.4/src/awkward/index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/jax.py` & `awkward-2.1.4/src/awkward/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/record.py` & `awkward-2.1.4/src/awkward/record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_backends/backend.py` & `awkward-2.1.4/src/awkward/_backends/backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_backends/cupy.py` & `awkward-2.1.4/src/awkward/_backends/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_backends/dispatch.py` & `awkward-2.1.4/src/awkward/_backends/dispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
-from collections.abc import Collection
+from collections.abc import Iterable
 
 from awkward._backends.backend import Backend
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyLike, NumpyMetadata
 from awkward._typing import Callable, TypeAlias, TypeVar
 from awkward._util import unset
 
@@ -42,29 +42,35 @@
         _name_to_backend_cls[backend_cls.name] = backend_cls
 
         return backend_cls
 
     return wrapper
 
 
-def common_backend(backends: Collection[Backend]) -> Backend:
+def common_backend(backends: Iterable[Backend]) -> Backend:
     unique_backends = frozenset(backends)
     # Either we have one nplike, or one + typetracer
     if len(unique_backends) == 1:
         return next(iter(unique_backends))
     else:
         # We allow typetracers to mix with other nplikes, and take precedence
         for backend in unique_backends:
             if not backend.nplike.known_data:
                 return backend
 
-        raise ValueError(
-            "cannot operate on arrays with incompatible backends. Use #ak.to_backend to coerce the arrays "
-            "to the same backend"
-        )
+        if len(unique_backends) > 1:
+            raise ValueError(
+                "cannot operate on arrays with incompatible backends. Use #ak.to_backend to coerce the arrays "
+                "to the same backend"
+            )
+
+        else:
+            raise ValueError(
+                "no backends were given in order to determine a common backend."
+            )
 
 
 def _backend_of(obj, default: D = unset) -> Backend | D:
     cls = type(obj)
     try:
         lookup = _type_to_backend_lookup[cls]
         return lookup(obj)
```

### Comparing `awkward-2.1.3/src/awkward/_backends/jax.py` & `awkward-2.1.4/src/awkward/_backends/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_backends/numpy.py` & `awkward-2.1.4/src/awkward/_backends/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_backends/typetracer.py` & `awkward-2.1.4/src/awkward/_backends/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/avro.py` & `awkward-2.1.4/src/awkward/_connect/avro.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cling.py` & `awkward-2.1.4/src/awkward/_connect/cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/hist.py` & `awkward-2.1.4/src/awkward/_connect/hist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/numexpr.py` & `awkward-2.1.4/src/awkward/_connect/numexpr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/numpy.py` & `awkward-2.1.4/src/awkward/_connect/numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
+import collections
 import functools
 import inspect
+from collections.abc import Iterable
+from itertools import chain
 
 import numpy
 
 import awkward as ak
-from awkward._backends.dispatch import backend_of
+from awkward._backends.backend import Backend
+from awkward._backends.dispatch import backend_of, common_backend
 from awkward._behavior import (
     behavior_of,
     find_custom_cast,
     find_ufunc,
     find_ufunc_generic,
 )
 from awkward._layout import wrap_layout
+from awkward._nplikes import to_nplike
 from awkward._regularize import is_non_string_like_iterable
+from awkward._typing import Iterator
 from awkward._util import numpy_at_least
 from awkward.contents.numpyarray import NumpyArray
 
 # NumPy 1.13.1 introduced NEP13, without which Awkward ufuncs won't work, which
 # would be worse than lacking a feature: it would cause unexpected output.
 # NumPy 1.17.0 introduced NEP18, which is optional (use ak.* instead of np.*).
 if not numpy_at_least("1.13.1"):
@@ -40,35 +46,67 @@
     else:
         return numpy.array(out, *args, **kwargs)
 
 
 implemented = {}
 
 
-def _to_rectilinear(arg):
-    backend = backend_of(arg, default=None)
-    # We have some array-like object that our backend mechanism understands
-    if backend is not None:
-        return ak.operations.to_numpy(arg)
+def _find_backends(args: Iterable) -> Iterator[Backend]:
+    """
+    Args:
+        args: iterable of objects to visit
+
+    Yields the encountered backends of layout / array-like arguments encountered
+    in the argument list.
+    """
+    stack = collections.deque(args)
+    while stack:
+        arg = stack.popleft()
+        # If the argument declares a backend, easy!
+        backend = backend_of(arg, default=None)
+        if backend is not None:
+            yield backend
+        # Otherwise, traverse into supported sequence types
+        elif isinstance(arg, (tuple, list)):
+            stack.extend(arg)
+
+
+def _to_rectilinear(arg, backend: Backend):
+    # Is this object something we already associate with a backend?
+    arg_backend = backend_of(arg, default=None)
+    if arg_backend is not None:
+        arg_nplike = arg_backend.nplike
+        # Is this argument already in a backend-supported form?
+        if arg_nplike.is_own_array(arg):
+            # Convert to the appropriate nplike
+            return to_nplike(
+                arg_nplike.asarray(arg), backend.nplike, from_nplike=arg_nplike
+            )
+        # Otherwise, cast to layout and convert
+        else:
+            layout = ak.to_layout(arg, allow_record=False, allow_other=False)
+            return layout.to_backend(backend).to_backend_array(allow_missing=True)
     elif isinstance(arg, tuple):
-        return tuple(_to_rectilinear(x) for x in arg)
+        return tuple(_to_rectilinear(x, backend) for x in arg)
     elif isinstance(arg, list):
-        return [_to_rectilinear(x) for x in arg]
+        return [_to_rectilinear(x, backend) for x in arg]
     elif is_non_string_like_iterable(arg):
         raise TypeError(
             f"encountered an unsupported iterable value {arg!r} whilst converting arguments to NumPy-friendly "
             f"types. If this argument should be supported, please file a bug report."
         )
     else:
         return arg
 
 
 def _array_function_no_impl(func, types, args, kwargs, behavior):
-    rectilinear_args = tuple(_to_rectilinear(x) for x in args)
-    rectilinear_kwargs = {k: _to_rectilinear(v) for k, v in kwargs.items()}
+    backend = common_backend(_find_backends(chain(args, kwargs.values())))
+
+    rectilinear_args = tuple(_to_rectilinear(x, backend) for x in args)
+    rectilinear_kwargs = {k: _to_rectilinear(v, backend) for k, v in kwargs.items()}
     result = func(*rectilinear_args, **rectilinear_kwargs)
     # We want the result to be a layout (this will fail for functions returning non-array convertibles)
     out = ak.operations.ak_to_layout._impl(
         result, allow_record=True, allow_other=True, regulararray=True
     )
     return wrap_layout(out, behavior=behavior, allow_other=True)
```

### Comparing `awkward-2.1.3/src/awkward/_connect/pyarrow.py` & `awkward-2.1.4/src/awkward/_connect/pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/__init__.py` & `awkward-2.1.4/src/awkward/_connect/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu` & `awkward-2.1.4/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/header-only/awkward/BuilderOptions.h` & `awkward-2.1.4/src/awkward/_connect/header-only/awkward/BuilderOptions.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/header-only/awkward/GrowableBuffer.h` & `awkward-2.1.4/src/awkward/_connect/header-only/awkward/GrowableBuffer.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/header-only/awkward/LayoutBuilder.h` & `awkward-2.1.4/src/awkward/_connect/header-only/awkward/LayoutBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/header-only/awkward/utils.h` & `awkward-2.1.4/src/awkward/_connect/header-only/awkward/utils.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/jax/reducers.py` & `awkward-2.1.4/src/awkward/_connect/jax/reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/jax/trees.py` & `awkward-2.1.4/src/awkward/_connect/jax/trees.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/numba/arrayview.py` & `awkward-2.1.4/src/awkward/_connect/numba/arrayview.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/numba/arrayview_cuda.py` & `awkward-2.1.4/src/awkward/_connect/numba/arrayview_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/numba/builder.py` & `awkward-2.1.4/src/awkward/_connect/numba/builder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/numba/growablebuffer.py` & `awkward-2.1.4/src/awkward/_connect/numba/growablebuffer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,16 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
+import math
+
 import numba
 import numba.core.typing.npydecl
 import numpy
 
-
-class GrowableBuffer:
-    def __init__(self, dtype, *, initial=1024, resize=8.0):
-        # all mutable data are in arrays that can be in-place shared with Numba
-        self._panels = numba.typed.List([numpy.empty((initial,), dtype=dtype)])
-        self._length_pos = numpy.zeros((2,), dtype=numpy.int64)
-        self._resize = resize
-
-    @classmethod
-    def _from_data(cls, panels, length_pos, resize):
-        out = cls.__new__(cls)
-        out._panels = panels
-        out._length_pos = length_pos
-        out._resize = resize
-        return out
-
-    @property
-    def dtype(self):
-        return self._panels[0].dtype
-
-    def __repr__(self):
-        return f"<GrowableBuffer of {self.dtype!r} with {self._length} items>"
-
-    @property
-    def _length(self):
-        return self._length_pos[0]
-
-    @_length.setter
-    def _length(self, value):
-        self._length_pos[0] = value
-
-    def _length_inc(self, value):
-        self._length_pos[0] += value
-
-    @property
-    def _pos(self):
-        return self._length_pos[1]
-
-    @_pos.setter
-    def _pos(self, value):
-        self._length_pos[1] = value
-
-    def _pos_inc(self, value):
-        self._length_pos[1] += value
-
-    def __len__(self):
-        return self._length
-
-    def append(self, datum):
-        if self._pos == len(self._panels[-1]):
-            self._add_panel()
-
-        self._panels[-1][self._pos] = datum
-        self._pos_inc(1)
-        self._length_inc(1)
-
-    def extend(self, data):
-        panel_index = len(self._panels) - 1
-        pos = self._pos
-
-        available = len(self._panels[-1]) - pos
-        while len(data) > available:
-            self._add_panel()
-            available += len(self._panels[-1])
-
-        remaining = len(data)
-        while remaining > 0:
-            panel = self._panels[panel_index]
-            available_in_panel = len(panel) - pos
-            to_write = min(remaining, available_in_panel)
-
-            start = len(data) - remaining
-            panel[pos : pos + to_write] = data[start : start + to_write]
-
-            if panel_index == len(self._panels) - 1:
-                self._pos_inc(to_write)
-            remaining -= to_write
-            pos = 0
-            panel_index += 1
-
-        self._length_inc(len(data))
-
-    def _add_panel(self):
-        panel_length = len(self._panels[-1])
-        if len(self._panels) == 1:
-            # only resize the first time, and by a large factor (C++ should do this, too!)
-            panel_length = int(numpy.ceil(panel_length * self._resize))
-
-        self._panels.append(numpy.empty((panel_length,), dtype=self.dtype))
-        self._pos = 0
-
-    def snapshot(self):
-        out = numpy.empty((self._length,), dtype=self.dtype)
-
-        start = 0
-        stop = 0
-        for panel in self._panels[:-1]:  # full panels, not including the last
-            stop += len(panel)
-            out[start:stop] = panel
-            start = stop
-
-        stop += self._pos
-        out[start:stop] = self._panels[-1][: self._pos]
-
-        return out
+from awkward.numba import GrowableBuffer
 
 
 class GrowableBufferType(numba.types.Type):
     def __init__(self, dtype):
         super().__init__(name=f"ak.GrowableBuffer({dtype})")
         self._dtype = dtype
 
@@ -326,22 +224,18 @@
 
         return len_impl
 
 
 @numba.extending.overload_method(GrowableBufferType, "_add_panel")
 def GrowableBuffer_add_panel(growablebuffer):
     def add_panel(growablebuffer):
-        last_panel = growablebuffer._panels[-1]
+        first_panel = growablebuffer._panels[0]
+        panel_length = int(math.ceil(len(first_panel) * growablebuffer._resize))
 
-        panel_length = len(last_panel)
-        if len(growablebuffer._panels) == 1:
-            # only resize the first time
-            panel_length = int(numpy.ceil(panel_length * growablebuffer._resize))
-
-        growablebuffer._panels.append(numpy.empty((panel_length,), last_panel.dtype))
+        growablebuffer._panels.append(numpy.empty((panel_length,), first_panel.dtype))
         growablebuffer._pos_set(0)
 
     return add_panel
 
 
 @numba.extending.overload_method(GrowableBufferType, "append")
 def GrowableBuffer_append(growablebuffer, datum):
@@ -359,19 +253,27 @@
 @numba.extending.overload_method(GrowableBufferType, "extend")
 def GrowableBuffer_extend(growablebuffer, data):
     def extend(growablebuffer, data):
         panel_index = len(growablebuffer._panels) - 1
         pos = growablebuffer._pos_get()
 
         available = len(growablebuffer._panels[-1]) - pos
-        while len(data) > available:
-            growablebuffer._add_panel()
+        remaining = len(data)
+
+        if remaining > available:
+            panel_length = int(
+                math.ceil(len(growablebuffer._panels[0]) * growablebuffer._resize)
+            )
+
+            growablebuffer._panels.append(
+                numpy.empty((max(remaining, panel_length),), dtype=growablebuffer.dtype)
+            )
+            growablebuffer._pos_set(0)
             available += len(growablebuffer._panels[-1])
 
-        remaining = len(data)
         while remaining > 0:
             panel = growablebuffer._panels[panel_index]
             available_in_panel = len(panel) - pos
             to_write = min(remaining, available_in_panel)
 
             start = len(data) - remaining
             panel[pos : pos + to_write] = data[start : start + to_write]
```

### Comparing `awkward-2.1.3/src/awkward/_connect/numba/layout.py` & `awkward-2.1.4/src/awkward/_connect/numba/layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/rdataframe/from_rdataframe.py` & `awkward-2.1.4/src/awkward/_connect/rdataframe/from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/rdataframe/to_rdataframe.py` & `awkward-2.1.4/src/awkward/_connect/rdataframe/to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h` & `awkward-2.1.4/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_nplikes/__init__.py` & `awkward-2.1.4/src/awkward/_nplikes/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_nplikes/array_module.py` & `awkward-2.1.4/src/awkward/_nplikes/array_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import math
 
 import numpy
 
-from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyLike, NumpyMetadata
+from awkward._nplikes.numpylike import (
+    ArrayLike,
+    IndexType,
+    NumpyLike,
+    NumpyMetadata,
+    UniqueAllResult,
+)
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._typing import Final, Literal
 
 np = NumpyMetadata.instance()
 
 
 class ArrayModuleNumpyLike(NumpyLike):
@@ -188,14 +194,39 @@
             x,
             return_counts=False,
             return_index=False,
             return_inverse=False,
             equal_nan=False,
         )
 
+    def unique_all(self, x: ArrayLike) -> UniqueAllResult:
+        values, indices, inverse_indices, counts = self._module.unique(
+            x, return_counts=True, return_index=True, return_inverse=True
+        )
+        # np.unique() flattens inverse indices, but they need to share x's shape
+        # See https://github.com/numpy/numpy/issues/20638
+        inverse_indices = inverse_indices.reshape(x.shape)
+        return UniqueAllResult(values, indices, inverse_indices, counts)
+
+    def sort(
+        self,
+        x: ArrayLike,
+        *,
+        axis: int = -1,
+        descending: bool = False,
+        stable: bool = True,
+    ) -> ArrayLike:
+        # Note: this keyword argument is different, and the default is different.
+        kind = "stable" if stable else "quicksort"
+        res = self._module.sort(x, axis=axis, kind=kind)
+        if descending:
+            return self._module.flip(res, axis=axis)
+        else:
+            return res
+
     def concat(
         self,
         arrays: list[ArrayLike] | tuple[ArrayLike, ...],
         *,
         axis: int | None = 0,
     ) -> ArrayLike:
         return self._module.concatenate(arrays, axis=axis, casting="same_kind")
```

### Comparing `awkward-2.1.3/src/awkward/_nplikes/cupy.py` & `awkward-2.1.4/src/awkward/_nplikes/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_nplikes/dispatch.py` & `awkward-2.1.4/src/awkward/_nplikes/dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_nplikes/jax.py` & `awkward-2.1.4/src/awkward/_nplikes/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_nplikes/numpy.py` & `awkward-2.1.4/src/awkward/_nplikes/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_nplikes/numpylike.py` & `awkward-2.1.4/src/awkward/_nplikes/numpylike.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,32 @@
 
 import numpy
 
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._singleton import Singleton
 from awkward._typing import (
     Literal,
+    NamedTuple,
     Protocol,
     Self,
     SupportsIndex,
     TypeAlias,
     overload,
 )
 
 IndexType: TypeAlias = "int | ArrayLike"
 
 
+class UniqueAllResult(NamedTuple):
+    values: ArrayLike
+    indices: ArrayLike
+    inverse_indices: ArrayLike
+    counts: ArrayLike
+
+
 class ArrayLike(Protocol):
     @property
     @abstractmethod
     def dtype(self) -> dtype:
         ...
 
     @property
@@ -399,14 +407,29 @@
         ...
 
     @abstractmethod
     def unique_values(self, x: ArrayLike) -> ArrayLike:
         ...
 
     @abstractmethod
+    def unique_all(self, x: ArrayLike) -> UniqueAllResult:
+        ...
+
+    @abstractmethod
+    def sort(
+        self,
+        x: ArrayLike,
+        *,
+        axis: int = -1,
+        descending: bool = False,
+        stable: bool = True,
+    ) -> ArrayLike:
+        ...
+
+    @abstractmethod
     def concat(
         self,
         arrays: list[ArrayLike] | tuple[ArrayLike, ...],
         *,
         axis: int | None = 0,
     ) -> ArrayLike:
         ...
```

### Comparing `awkward-2.1.3/src/awkward/_nplikes/shape.py` & `awkward-2.1.4/src/awkward/_nplikes/shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/_nplikes/typetracer.py` & `awkward-2.1.4/src/awkward/_nplikes/typetracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 from numbers import Number
 
 import numpy
 from numpy.lib.mixins import NDArrayOperatorsMixin
 
 import awkward as ak
 from awkward._nplikes.dispatch import register_nplike
-from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyLike, NumpyMetadata
+from awkward._nplikes.numpylike import (
+    ArrayLike,
+    IndexType,
+    NumpyLike,
+    NumpyMetadata,
+    UniqueAllResult,
+)
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._regularize import is_integer, is_non_string_like_sequence
 from awkward._typing import (
     Any,
     Final,
     Literal,
     Self,
@@ -1077,14 +1083,34 @@
         result_dtype = numpy.result_type(x1, x2)
         return TypeTracerArray._new(result_dtype, shape=condition.shape)
 
     def unique_values(self, x: ArrayLike) -> TypeTracerArray:
         try_touch_data(x)
         return TypeTracerArray._new(x.dtype, shape=(unknown_length,))
 
+    def unique_all(self, x: ArrayLike) -> UniqueAllResult:
+        try_touch_data(x)
+        return UniqueAllResult(
+            TypeTracerArray._new(x.dtype, shape=(unknown_length,)),
+            TypeTracerArray._new(np.int64, shape=(unknown_length,)),
+            TypeTracerArray._new(np.int64, shape=x.shape),
+            TypeTracerArray._new(np.int64, shape=(unknown_length,)),
+        )
+
+    def sort(
+        self,
+        x: ArrayLike,
+        *,
+        axis: int = -1,
+        descending: bool = False,
+        stable: bool = True,
+    ) -> ArrayLike:
+        try_touch_data(x)
+        return TypeTracerArray._new(x.dtype, shape=x.shape)
+
     def concat(self, arrays, *, axis: int | None = 0) -> TypeTracerArray:
         if axis is None:
             assert all(x.ndim == 1 for x in arrays)
         elif axis != 0:
             raise NotImplementedError("concat with axis != 0")
         for x in arrays:
             try_touch_data(x)
@@ -1114,15 +1140,29 @@
         x: ArrayLike,
         repeats: ArrayLike | int,
         *,
         axis: int | None = None,
     ) -> TypeTracerArray:
         try_touch_data(x)
         try_touch_data(repeats)
-        raise NotImplementedError
+
+        if axis is None:
+            size = x.size
+            if isinstance(repeats, TypeTracerArray) and repeats.ndim > 0:
+                raise NotImplementedError
+            else:
+                size = size * self.index_as_shape_item(repeats)
+            return TypeTracerArray._new(x.dtype, (size,))
+        else:
+            shape = list(x.shape)
+            if isinstance(repeats, TypeTracerArray) and repeats.ndim > 0:
+                raise NotImplementedError
+            else:
+                shape[axis] = shape[axis] * self.index_as_shape_item(repeats)
+            return TypeTracerArray._new(x.dtype, shape=tuple(shape))
 
     def tile(self, x: ArrayLike, reps: int) -> TypeTracerArray:
         try_touch_data(x)
         raise NotImplementedError
 
     def stack(
         self,
```

### Comparing `awkward-2.1.3/src/awkward/_nplikes/ufuncs.py` & `awkward-2.1.4/src/awkward/_nplikes/ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/behaviors/categorical.py` & `awkward-2.1.4/src/awkward/behaviors/categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/behaviors/mixins.py` & `awkward-2.1.4/src/awkward/behaviors/mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/behaviors/string.py` & `awkward-2.1.4/src/awkward/behaviors/string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/contents/__init__.py` & `awkward-2.1.4/src/awkward/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/contents/bitmaskedarray.py` & `awkward-2.1.4/src/awkward/contents/bitmaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/contents/bytemaskedarray.py` & `awkward-2.1.4/src/awkward/contents/bytemaskedarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import copy
 import json
 import math
 
 import awkward as ak
 from awkward._backends.backend import Backend
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer
 from awkward._parameters import (
     parameters_intersect,
@@ -563,15 +564,15 @@
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
             raise AssertionError(repr(head))
 
     def project(self, mask=None):
         mask_length = self._mask.length
-        numnull = ak.index.Index64.zeros(1, nplike=self._backend.index_nplike)
+        _numnull = ak.index.Index64.zeros(1, nplike=self._backend.index_nplike)
 
         if mask is not None:
             if self._backend.nplike.known_data and mask_length != mask.length:
                 raise ValueError(
                     "mask length ({}) is not equal to {} length ({})".format(
                         mask.length, type(self).__name__, mask_length
                     )
@@ -603,31 +604,32 @@
             next = ByteMaskedArray(
                 nextmask, self._content, valid_when, parameters=self._parameters
             )
             return next.project()
 
         else:
             assert (
-                numnull.nplike is self._backend.index_nplike
+                _numnull.nplike is self._backend.index_nplike
                 and self._mask.nplike is self._backend.index_nplike
             )
             self._handle_error(
                 self._backend[
                     "awkward_ByteMaskedArray_numnull",
-                    numnull.dtype.type,
+                    _numnull.dtype.type,
                     self._mask.dtype.type,
                 ](
-                    numnull.data,
+                    _numnull.data,
                     self._mask.data,
                     mask_length,
                     self._valid_when,
                 )
             )
+            numnull = self._backend.index_nplike.index_as_shape_item(_numnull[0])
             nextcarry = ak.index.Index64.empty(
-                mask_length - numnull[0], nplike=self._backend.index_nplike
+                mask_length - numnull, nplike=self._backend.index_nplike
             )
             assert (
                 nextcarry.nplike is self._backend.index_nplike
                 and self._mask.nplike is self._backend.index_nplike
             )
             self._handle_error(
                 self._backend[
@@ -643,15 +645,15 @@
             )
 
             return self._content._carry(nextcarry, False)
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise np.AxisError("axis=0 not allowed for flatten")
+            raise AxisError("axis=0 not allowed for flatten")
         else:
             numnull, nextcarry, outindex = self._nextcarry_outindex()
 
             next = self._content._carry(nextcarry, False)
 
             offsets, flattened = next._offsets_and_flattened(axis, depth)
```

### Comparing `awkward-2.1.3/src/awkward/contents/content.py` & `awkward-2.1.4/src/awkward/contents/content.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/contents/emptyarray.py` & `awkward-2.1.4/src/awkward/contents/emptyarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import copy
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._backends.numpy import NumpyBackend
 from awkward._backends.typetracer import TypeTracerBackend
-from awkward._errors import deprecate
+from awkward._errors import AxisError, deprecate
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
@@ -232,15 +232,15 @@
 
         else:
             raise AssertionError(repr(head))
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise np.AxisError(self, "axis=0 not allowed for flatten")
+            raise AxisError(self, "axis=0 not allowed for flatten")
         else:
             offsets = ak.index.Index64.zeros(1, nplike=self._backend.index_nplike)
             return (
                 offsets,
                 EmptyArray(parameters=self._parameters, backend=self._backend),
             )
 
@@ -263,15 +263,15 @@
         if posaxis is not None and posaxis + 1 == depth:
             return ak.contents.NumpyArray(
                 self._backend.nplike.empty(0, dtype=np.int64),
                 parameters=None,
                 backend=self._backend,
             )
         else:
-            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
+            raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
 
     def _numbers_to_type(self, name, including_unknown):
         if including_unknown:
             return self.to_NumpyArray(ak.types.numpytype.primitive_to_dtype(name))
         else:
             return self
 
@@ -327,15 +327,15 @@
 
     def _nbytes_part(self):
         return 0
 
     def _pad_none(self, target, axis, depth, clip):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 != depth:
-            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
+            raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         else:
             return self._pad_none_axis0(target, True)
 
     def _to_arrow(self, pyarrow, mask_node, validbytes, length, options):
         if options["emptyarray_to"] is None:
             return pyarrow.Array.from_buffers(
                 ak._connect.pyarrow.to_awkwardarrow_type(
```

### Comparing `awkward-2.1.3/src/awkward/contents/indexedarray.py` & `awkward-2.1.4/src/awkward/contents/indexedarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 
 import awkward as ak
 from awkward._backends.backend import Backend
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.typetracer import TypeTracer
 from awkward._parameters import (
     parameters_intersect,
     parameters_union,
@@ -464,15 +465,15 @@
                     exclude=(("__array__", "categorical"),),
                 )
             )
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise np.AxisError("axis=0 not allowed for flatten")
+            raise AxisError("axis=0 not allowed for flatten")
 
         else:
             return self.project()._offsets_and_flattened(axis, depth)
 
     def _mergeable_next(self, other, mergebool):
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
```

### Comparing `awkward-2.1.3/src/awkward/contents/indexedoptionarray.py` & `awkward-2.1.4/src/awkward/contents/indexedoptionarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 
 import awkward as ak
 from awkward._backends.backend import Backend
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer
 from awkward._parameters import (
     parameters_intersect,
@@ -560,15 +561,15 @@
             )
 
             return self._content._carry(nextcarry, False)
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise np.AxisError("axis=0 not allowed for flatten")
+            raise AxisError("axis=0 not allowed for flatten")
         else:
             numnull, nextcarry, outindex = self._nextcarry_outindex()
             next = self._content._carry(nextcarry, False)
 
             offsets, flattened = next._offsets_and_flattened(axis, depth)
 
             if offsets.length == 0:
```

### Comparing `awkward-2.1.3/src/awkward/contents/listarray.py` & `awkward-2.1.4/src/awkward/contents/listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/contents/listoffsetarray.py` & `awkward-2.1.4/src/awkward/contents/listoffsetarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 
 import awkward as ak
 from awkward._backends.backend import Backend
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import TypeTracer, is_unknown_scalar
 from awkward._parameters import (
     type_parameters_equal,
@@ -704,15 +705,15 @@
 
         else:
             raise AssertionError(repr(head))
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise np.AxisError("axis=0 not allowed for flatten")
+            raise AxisError("axis=0 not allowed for flatten")
 
         elif posaxis is not None and posaxis + 1 == depth + 1:
             listoffsetarray = self.to_ListOffsetArray64(True)
             stop = listoffsetarray.offsets[-1]
             content = listoffsetarray.content._getitem_range(0, stop)
             return (listoffsetarray.offsets, content)
 
@@ -920,30 +921,30 @@
         branch, depth = self.branch_depth
 
         if (
             self.parameter("__array__") == "string"
             or self.parameter("__array__") == "bytestring"
         ):
             if branch or (negaxis != depth):
-                raise np.AxisError("array with strings can only be sorted with axis=-1")
+                raise AxisError("array with strings can only be sorted with axis=-1")
 
             # FIXME: check validity error
 
             if isinstance(self._content, ak.contents.NumpyArray):
                 out, nextoffsets = self._content._as_unique_strings(self._offsets)
                 return ak.contents.ListOffsetArray(
                     nextoffsets, out, parameters=self._parameters
                 )
 
         if not branch and (negaxis == depth):
             if (
                 self.parameter("__array__") == "string"
                 or self.parameter("__array__") == "bytestring"
             ):
-                raise np.AxisError("array with strings can only be sorted with axis=-1")
+                raise AxisError("array with strings can only be sorted with axis=-1")
 
             if self._backend.nplike.known_data and parents.nplike.known_data:
                 assert self._offsets.length - 1 == parents.length
 
             (
                 distincts,
                 maxcount,
@@ -1036,15 +1037,15 @@
         branch, depth = self.branch_depth
 
         if (
             self.parameter("__array__") == "string"
             or self.parameter("__array__") == "bytestring"
         ):
             if branch or (negaxis != depth):
-                raise np.AxisError("array with strings can only be sorted with axis=-1")
+                raise AxisError("array with strings can only be sorted with axis=-1")
 
             # FIXME: check validity error
 
             if isinstance(self._content, ak.contents.NumpyArray):
                 nextcarry = ak.index.Index64.empty(
                     self._offsets.length - 1, self._backend.index_nplike
                 )
@@ -1082,15 +1083,15 @@
                 )
 
         if not branch and (negaxis == depth):
             if (
                 self.parameter("__array__") == "string"
                 or self.parameter("__array__") == "bytestring"
             ):
-                raise np.AxisError("array with strings can only be sorted with axis=-1")
+                raise AxisError("array with strings can only be sorted with axis=-1")
 
             if self._backend.nplike.known_data and parents.nplike.known_data:
                 assert self._offsets.length - 1 == parents.length
 
             (
                 distincts,
                 maxcount,
@@ -1221,15 +1222,15 @@
         index_nplike = self._backend.index_nplike
 
         if (
             self.parameter("__array__") == "string"
             or self.parameter("__array__") == "bytestring"
         ):
             if branch or (negaxis != depth):
-                raise np.AxisError("array with strings can only be sorted with axis=-1")
+                raise AxisError("array with strings can only be sorted with axis=-1")
 
             # FIXME: check validity error
 
             if isinstance(self._content, ak.contents.NumpyArray):
                 nextcarry = ak.index.Index64.empty(
                     self._offsets.length - 1, index_nplike
                 )
@@ -1265,15 +1266,15 @@
                 return self._carry(nextcarry, False)
 
         if not branch and (negaxis == depth):
             if (
                 self.parameter("__array__") == "string"
                 or self.parameter("__array__") == "bytestring"
             ):
-                raise np.AxisError("array with strings can only be sorted with axis=-1")
+                raise AxisError("array with strings can only be sorted with axis=-1")
 
             if self._backend.nplike.known_data and parents.nplike.known_data:
                 assert self._offsets.length - 1 == parents.length
 
             (
                 distincts,
                 maxcount,
```

### Comparing `awkward-2.1.3/src/awkward/contents/numpyarray.py` & `awkward-2.1.4/src/awkward/contents/numpyarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import copy
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._backends.typetracer import TypeTracerBackend
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes import to_nplike
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
 from awkward._nplikes.typetracer import TypeTracerArray
 from awkward._parameters import (
@@ -403,21 +404,21 @@
 
         else:
             raise AssertionError(repr(head))
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise np.AxisError("axis=0 not allowed for flatten")
+            raise AxisError("axis=0 not allowed for flatten")
 
         elif len(self.shape) != 1:
             return self.to_RegularArray()._offsets_and_flattened(axis, depth)
 
         else:
-            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
+            raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
 
     def _mergeable_next(self, other, mergebool):
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # Check against option contents
         elif other.is_option or other.is_indexed:
@@ -510,15 +511,15 @@
         return self
 
     def _local_index(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             return self._local_index_axis0()
         elif len(self.shape) <= 1:
-            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
+            raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         else:
             return self.to_RegularArray()._local_index(axis, depth)
 
     def to_contiguous(self) -> Self:
         if self.is_contiguous:
             return self
         else:
@@ -1060,15 +1061,15 @@
             )
 
     def _combinations(self, n, replacement, recordlookup, parameters, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             return self._combinations_axis0(n, replacement, recordlookup, parameters)
         elif len(self.shape) <= 1:
-            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
+            raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         else:
             return self.to_RegularArray()._combinations(
                 n, replacement, recordlookup, parameters, axis, depth
             )
 
     def _reduce_next(
         self,
@@ -1196,15 +1197,15 @@
     def _pad_none(self, target, axis, depth, clip):
         if len(self.shape) == 0:
             raise ValueError("cannot apply ak.pad_none to a scalar")
         elif len(self.shape) > 1 or not self.is_contiguous:
             return self.to_RegularArray()._pad_none(target, axis, depth, clip)
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 != depth:
-            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
+            raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         if not clip:
             if target < self.length:
                 return self
             else:
                 return self._pad_none(target, axis, depth, clip=True)
         else:
             return self._pad_none_axis0(target, clip=True)
```

### Comparing `awkward-2.1.3/src/awkward/contents/recordarray.py` & `awkward-2.1.4/src/awkward/contents/recordarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from collections.abc import Iterable
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._backends.numpy import NumpyBackend
 from awkward._backends.typetracer import TypeTracerBackend
 from awkward._behavior import find_record_reducer
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._parameters import (
     parameters_intersect,
     type_parameters_equal,
@@ -591,15 +592,15 @@
                 backend=self._backend,
             )
             return next._getitem_next(nexthead, nexttail, advanced)
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise np.AxisError("axis=0 not allowed for flatten")
+            raise AxisError("axis=0 not allowed for flatten")
 
         elif posaxis is not None and posaxis + 1 == depth + 1:
             raise ValueError(
                 "arrays of records cannot be flattened (but their contents can be; try a different 'axis')"
             )
 
         else:
```

### Comparing `awkward-2.1.3/src/awkward/contents/regulararray.py` & `awkward-2.1.4/src/awkward/contents/regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/contents/unionarray.py` & `awkward-2.1.4/src/awkward/contents/unionarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import copy
 import ctypes
 from collections.abc import Iterable, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import OneOf, TypeTracer
 from awkward._parameters import parameters_intersect, parameters_union
@@ -806,15 +807,15 @@
         else:
             raise AssertionError(repr(head))
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
 
         if posaxis is not None and posaxis + 1 == depth:
-            raise np.AxisError("axis=0 not allowed for flatten")
+            raise AxisError("axis=0 not allowed for flatten")
 
         else:
             has_offsets = False
             offsetsraws = self._backend.index_nplike.empty(
                 len(self._contents), dtype=np.intp
             )
             contents = []
@@ -1578,15 +1579,15 @@
             index,
             contents,
             parameters=self._parameters,
         )
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
         return (
-            self.tags == other.tags
+            self.tags.is_equal_to(other.tags)
             and self.index.is_equal_to(other.index, index_dtype, numpyarray)
             and len(self.contents) == len(other.contents)
             and all(
                 self.contents[i].is_equal_to(other.contents[i], index_dtype, numpyarray)
                 for i in range(len(self.contents))
             )
         )
```

### Comparing `awkward-2.1.3/src/awkward/contents/unmaskedarray.py` & `awkward-2.1.4/src/awkward/contents/unmaskedarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import copy
 import math
 
 import awkward as ak
 from awkward._backends.backend import Backend
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.typetracer import MaybeNone
 from awkward._parameters import (
     parameters_intersect,
     parameters_union,
@@ -295,15 +296,15 @@
             ).project()
         else:
             return self._content
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise np.AxisError("axis=0 not allowed for flatten")
+            raise AxisError("axis=0 not allowed for flatten")
         else:
             offsets, flattened = self._content._offsets_and_flattened(axis, depth)
             if offsets.length == 0:
                 return (
                     offsets,
                     UnmaskedArray(flattened, parameters=self._parameters),
                 )
```

### Comparing `awkward-2.1.3/src/awkward/forms/__init__.py` & `awkward-2.1.4/src/awkward/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/bitmaskedform.py` & `awkward-2.1.4/src/awkward/forms/bitmaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/bytemaskedform.py` & `awkward-2.1.4/src/awkward/forms/bytemaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/emptyform.py` & `awkward-2.1.4/src/awkward/forms/emptyform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/form.py` & `awkward-2.1.4/src/awkward/forms/form.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/indexedform.py` & `awkward-2.1.4/src/awkward/forms/indexedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/indexedoptionform.py` & `awkward-2.1.4/src/awkward/forms/indexedoptionform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/listform.py` & `awkward-2.1.4/src/awkward/forms/listform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/listoffsetform.py` & `awkward-2.1.4/src/awkward/forms/listoffsetform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/numpyform.py` & `awkward-2.1.4/src/awkward/forms/numpyform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/recordform.py` & `awkward-2.1.4/src/awkward/forms/recordform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/regularform.py` & `awkward-2.1.4/src/awkward/forms/regularform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/unionform.py` & `awkward-2.1.4/src/awkward/forms/unionform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/forms/unmaskedform.py` & `awkward-2.1.4/src/awkward/forms/unmaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/__init__.py` & `awkward-2.1.4/src/awkward/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_all.py` & `awkward-2.1.4/src/awkward/operations/ak_all.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_almost_equal.py` & `awkward-2.1.4/src/awkward/operations/ak_almost_equal.py`

 * *Files 25% similar despite different names*

```diff
@@ -101,43 +101,88 @@
                 left.offsets, right.offsets
             ) and visitor(
                 left.content[: left.offsets[-1]], right.content[: right.offsets[-1]]
             )
         elif left.is_regular:
             return (left.size == right.size) and visitor(left.content, right.content)
         elif left.is_numpy:
-            return (
-                is_approx_dtype(left.dtype, right.dtype)
-                and backend.nplike.all(
-                    backend.nplike.isclose(
-                        left.data, right.data, rtol=rtol, atol=atol, equal_nan=False
+            # Timelike types must be exactly compared, including their units
+            if (
+                np.issubdtype(left.dtype, np.datetime64)
+                or np.issubdtype(right.dtype, np.datetime64)
+                or np.issubdtype(left.dtype, np.timedelta64)
+                or np.issubdtype(right.dtype, np.timedelta64)
+            ):
+                return (
+                    (left.dtype == right.dtype)
+                    and backend.nplike.all(left.data == right.data)
+                    and left.shape == right.shape
+                )
+            else:
+                return (
+                    is_approx_dtype(left.dtype, right.dtype)
+                    and backend.nplike.all(
+                        backend.nplike.isclose(
+                            left.data, right.data, rtol=rtol, atol=atol, equal_nan=False
+                        )
                     )
+                    and left.shape == right.shape
                 )
-                and left.shape == right.shape
-            )
-
         elif left.is_option:
             return backend.index_nplike.array_equal(
                 left.index.data < 0, right.index.data < 0
             ) and visitor(left.project().to_packed(), right.project().to_packed())
         elif left.is_union:
-            return (len(left.contents) == len(right.contents)) and all(
-                visitor(left.project(i).to_packed(), right.project(i).to_packed())
-                for i, _ in enumerate(left.contents)
+            # For two unions with different content orderings to match, the tags should be equal at each index
+            # Therefore, we can order the contents by index appearance
+            def ordered_unique_values(values):
+                # First, find unique values and their appearance (from smallest to largest)
+                # unique_index is in ascending order of `unique` value
+                (
+                    unique,
+                    unique_index,
+                    *_,
+                ) = backend.index_nplike.unique_all(values)
+                # Now re-order `unique` by order of appearance (`unique_index`)
+                return values[backend.index_nplike.sort(unique_index)]
+
+            # Find order of appearance for each union tags, and assume these are one-to-one maps
+            left_tag_order = ordered_unique_values(left.tags.data)
+            right_tag_order = ordered_unique_values(right.tags.data)
+
+            # Create map from left tags to right tags
+            left_tag_to_right_tag = backend.index_nplike.empty(
+                left_tag_order.size, dtype=np.int64
             )
+            left_tag_to_right_tag[left_tag_order] = right_tag_order
+
+            # Map left tags onto right, such that the result should equal right.tags
+            # if the two tag arrays are equivalent
+            new_left_tag = left_tag_to_right_tag[left.tags.data]
+            if not backend.index_nplike.all(new_left_tag == right.tags.data):
+                return False
+
+            # Now project out the contents, and check for equality
+            for i, j in zip(left_tag_order, right_tag_order):
+                if not visitor(
+                    left.project(i).to_packed(), right.project(j).to_packed()
+                ):
+                    return False
+            return True
+
         elif left.is_record:
             return (
                 (
                     get_record_class(left, left_behavior)
                     is get_record_class(right, right_behavior)
                     or not check_parameters
                 )
-                and (left.fields == right.fields)
-                and (left.is_tuple == right.is_tuple)
-                and all(visitor(x, y) for x, y in zip(left.contents, right.contents))
+                and left.is_tuple == right.is_tuple
+                and (left.is_tuple or (len(left.fields) == len(right.fields)))
+                and all(visitor(left.content(f), right.content(f)) for f in left.fields)
             )
         elif left.is_unknown:
             return True
 
         else:
             raise AssertionError
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_any.py` & `awkward-2.1.4/src/awkward/operations/ak_any.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_argcartesian.py` & `awkward-2.1.4/src/awkward/operations/ak_argcartesian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_argcombinations.py` & `awkward-2.1.4/src/awkward/operations/ak_argcombinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_argmax.py` & `awkward-2.1.4/src/awkward/operations/ak_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_argmin.py` & `awkward-2.1.4/src/awkward/operations/ak_argmin.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_argsort.py` & `awkward-2.1.4/src/awkward/operations/ak_argsort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_backend.py` & `awkward-2.1.4/src/awkward/operations/ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_broadcast_arrays.py` & `awkward-2.1.4/src/awkward/operations/ak_broadcast_arrays.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,25 +204,36 @@
     depth_limit,
     broadcast_parameters_rule,
     left_broadcast,
     right_broadcast,
     highlevel,
     behavior,
 ):
+    # Need at least one array!
+    if len(arrays) == 0:
+        return []
+
     backend = backend_of(*arrays, default=cpu)
 
     inputs = []
     for x in arrays:
         y = ak.operations.to_layout(x, allow_record=True, allow_other=True)
         if not isinstance(y, (ak.contents.Content, ak.Record)):
             y = ak.contents.NumpyArray(backend.nplike.asarray([y]))
         inputs.append(y.to_backend(backend))
 
     def action(inputs, depth, **kwargs):
-        if depth == depth_limit or all(x.is_numpy for x in inputs):
+        # The depth limit is the depth at which we must return, i.e.
+        # the _first_ layout at that depth
+        if depth == depth_limit:
+            return tuple(inputs)
+        # Walk through non-leaf nodes
+        elif all(
+            x.purelist_depth == 1 and not (x.is_option or x.is_indexed) for x in inputs
+        ):
             return tuple(inputs)
         else:
             return None
 
     behavior = behavior_of(*arrays, behavior=behavior)
     out = ak._broadcasting.broadcast_and_apply(
         inputs,
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_broadcast_fields.py` & `awkward-2.1.4/src/awkward/operations/ak_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_cartesian.py` & `awkward-2.1.4/src/awkward/operations/ak_cartesian.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("cartesian",)
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
@@ -213,57 +214,61 @@
         behavior = behavior_of(*arrays.values(), behavior=behavior)
         array_layouts = {
             name: ak.operations.to_layout(
                 layout, allow_record=False, allow_other=False
             ).to_backend(backend)
             for name, layout in arrays.items()
         }
+        layouts = list(array_layouts.values())
+        fields = list(array_layouts.keys())
 
     else:
         arrays = list(arrays)
         backend = backend_of(*arrays, default=cpu)
         behavior = behavior_of(*arrays, behavior=behavior)
         array_layouts = [
             ak.operations.to_layout(
                 layout, allow_record=False, allow_other=False
             ).to_backend(backend)
             for layout in arrays
         ]
+        layouts = array_layouts
+        fields = None
 
     if with_name is not None:
         if parameters is None:
             parameters = {}
         else:
             parameters = dict(parameters)
         parameters["__record__"] = with_name
 
-    if isinstance(array_layouts, dict):
-        layouts = list(array_layouts.values())
-    else:
-        layouts = array_layouts
-
     posaxis = maybe_posaxis(layouts[0], axis, 1)
-
     # Validate `posaxis`
     if posaxis is None or posaxis < 0:
-        raise ValueError("negative axis depth is ambiguous")
+        raise AxisError("negative axis depth is ambiguous")
+    # Ensure other layouts have same positive value for axis
     for layout in layouts[1:]:
         if maybe_posaxis(layout, axis, 1) != posaxis:
-            raise ValueError(
+            raise AxisError(
                 "arrays to cartesian-product do not have the same depth for negative axis"
             )
+    depths = [obj.purelist_depth for obj in layouts]
+    if posaxis >= max(depths):
+        raise AxisError(
+            f"axis={axis} exceeds the max depth of the given arrays (which is {max(depths)})"
+        )
 
     # Validate `nested`
     if nested is None or nested is False:
         nested = []
     elif nested is True:
-        if isinstance(array_layouts, dict):
-            nested = list(array_layouts.keys())[:-1]
+        if fields is not None:
+            nested = list(fields)[:-1]
         else:
-            nested = list(range(len(array_layouts))[:-1])
+            nested = list(range(len(layouts))[:-1])
     else:
         if isinstance(array_layouts, dict):
             if any(not (isinstance(x, str) and x in array_layouts) for x in nested):
                 raise ValueError(
                     "the 'nested' parameter of cartesian must be dict keys "
                     "for a dict of arrays"
                 )
@@ -279,25 +284,16 @@
             ):
                 raise ValueError(
                     "the 'nested' parameter of cartesian must be integers in "
                     "[0, len(arrays) - 1) for an iterable of arrays"
                 )
 
     if posaxis == 0:
-        if isinstance(array_layouts, dict):
-            fields = []
-            tonested = []
-            for i, (name, _) in enumerate(array_layouts.items()):
-                fields.append(name)
-                if name in nested:
-                    tonested.append(i)
-            nested = tonested
-
-        else:
-            fields = None
+        if fields is not None:
+            nested = [i for i, name in enumerate(fields) if name in nested]
 
         indexes = [
             ak.index.Index64(backend.index_nplike.reshape(x, (-1,)))
             for x in backend.index_nplike.meshgrid(
                 *[
                     backend.index_nplike.arange(x.length, dtype=np.int64)
                     for x in layouts
@@ -373,37 +369,23 @@
             posaxis + i + 1
             for i, _ in enumerate(array_layouts)
             if i < len(array_layouts) - 1 and i not in nested
         ]
         # This list *must* be sorted in reverse order
         axes_to_flatten.reverse()
 
-        if isinstance(array_layouts, dict):
-            fields = list(array_layouts.keys())
-            new_layouts = [
-                ak._do.recursively_apply(
-                    layout,
-                    apply_pad_inner_list_at_axis,
-                    behavior,
-                    lateral_context={"i": i},
-                )
-                for i, (_, layout) in enumerate(array_layouts.items())
-            ]
-
-        else:
-            fields = None
-            new_layouts = [
-                ak._do.recursively_apply(
-                    layout,
-                    apply_pad_inner_list_at_axis,
-                    behavior,
-                    lateral_context={"i": i},
-                )
-                for i, layout in enumerate(array_layouts)
-            ]
+        new_layouts = [
+            ak._do.recursively_apply(
+                layout,
+                apply_pad_inner_list_at_axis,
+                behavior,
+                lateral_context={"i": i},
+            )
+            for i, layout in enumerate(layouts)
+        ]
 
         def apply_build_record(inputs, depth, **kwargs):
             if depth == posaxis + len(array_layouts):
                 return (ak.contents.RecordArray(inputs, fields, parameters=parameters),)
 
             else:
                 return None
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_categories.py` & `awkward-2.1.4/src/awkward/operations/ak_categories.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_combinations.py` & `awkward-2.1.4/src/awkward/operations/ak_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_concatenate.py` & `awkward-2.1.4/src/awkward/operations/ak_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_copy.py` & `awkward-2.1.4/src/awkward/operations/ak_copy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_corr.py` & `awkward-2.1.4/src/awkward/operations/ak_corr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_count.py` & `awkward-2.1.4/src/awkward/operations/ak_count.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_count_nonzero.py` & `awkward-2.1.4/src/awkward/operations/ak_count_nonzero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_covar.py` & `awkward-2.1.4/src/awkward/operations/ak_covar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_drop_none.py` & `awkward-2.1.4/src/awkward/operations/ak_drop_none.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("drop_none",)
 import awkward as ak
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -65,17 +66,15 @@
 
         def action(layout, continuation, **kwargs):
             return drop_nones(continuation())
 
     else:
         max_axis = layout.branch_depth[1] - 1
         if axis > max_axis:
-            raise np.AxisError(
-                f"axis={axis} exceeds the depth ({max_axis}) of this array"
-            )
+            raise AxisError(f"axis={axis} exceeds the depth ({max_axis}) of this array")
 
         def recompute_offsets(layout, depth, **kwargs):
             posaxis = maybe_posaxis(layout, axis, depth)
             if (
                 posaxis == 0
                 and posaxis == depth - 1
                 or posaxis == depth
@@ -85,15 +84,15 @@
                 out = layout._rebuild_without_nones(none_indexes, layout.content)
                 return out
 
         def action(layout, depth, **kwargs):
             if layout.is_record:
                 posaxises = {maybe_posaxis(x, axis, depth) for x in layout.contents}
                 if len(posaxises) > 1 and any(x < depth for x in posaxises):
-                    raise np.AxisError(
+                    raise AxisError(
                         f"axis={axis} implies different levels in records that might require part of a record to be dropped, which is impossible"
                     )
             posaxis = maybe_posaxis(layout, axis, depth)
             if posaxis == 0:
                 if not layout.is_option:
                     return layout
                 else:
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_fields.py` & `awkward-2.1.4/src/awkward/operations/ak_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_fill_none.py` & `awkward-2.1.4/src/awkward/operations/ak_fill_none.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 __all__ = ("fill_none",)
 import numbers
 
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_sized_iterable, regularize_axis
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
@@ -132,13 +133,13 @@
                     return ak._do.fill_none(layout, valuelayout)
                 elif layout.is_union or layout.is_record or layout.is_indexed:
                     return None
                 else:
                     return layout
 
             elif layout.is_leaf:
-                raise np.AxisError(
+                raise AxisError(
                     f"axis={axis} exceeds the depth of this array ({depth})"
                 )
 
     out = ak._do.recursively_apply(arraylayout, action, behavior)
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_firsts.py` & `awkward-2.1.4/src/awkward/operations/ak_firsts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("firsts",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer, regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -86,14 +87,14 @@
                 index[empties] = -1
 
                 return ak.contents.IndexedOptionArray.simplified(
                     ak.index.Index64(index), layout._content
                 )
 
             elif layout.is_leaf:
-                raise np.AxisError(
+                raise AxisError(
                     f"axis={axis} exceeds the depth of this array ({depth})"
                 )
 
         out = ak._do.recursively_apply(layout, action, behavior, numpy_to_regular=True)
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_flatten.py` & `awkward-2.1.4/src/awkward/operations/ak_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_arrow.py` & `awkward-2.1.4/src/awkward/operations/ak_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_arrow_schema.py` & `awkward-2.1.4/src/awkward/operations/ak_from_arrow_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_avro_file.py` & `awkward-2.1.4/src/awkward/operations/ak_from_avro_file.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_buffers.py` & `awkward-2.1.4/src/awkward/operations/ak_from_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_categorical.py` & `awkward-2.1.4/src/awkward/operations/ak_from_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_cupy.py` & `awkward-2.1.4/src/awkward/operations/ak_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_iter.py` & `awkward-2.1.4/src/awkward/operations/ak_from_iter.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def from_iter(
     iterable,
     *,
     allow_record=True,
     highlevel=True,
     behavior=None,
     initial=1024,
-    resize=1.5,
+    resize=8,
 ):
     """
     Args:
         iterable (Python iterable): Data to convert into an Awkward Array.
         allow_record (bool): If True, the outermost element may be a record
             (returning #ak.Record or #ak.record.Record type, depending on
             `highlevel`); if False, the outermost element must be an array.
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_jax.py` & `awkward-2.1.4/src/awkward/operations/ak_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_json.py` & `awkward-2.1.4/src/awkward/operations/ak_from_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     schema=None,
     nan_string=None,
     posinf_string=None,
     neginf_string=None,
     complex_record_fields=None,
     buffersize=65536,
     initial=1024,
-    resize=1.5,
+    resize=8,
     highlevel=True,
     behavior=None,
 ):
     """
     Args:
         source (bytes/str, pathlib.Path, or file-like object): Data source of the
             JSON-formatted string(s). If bytes/str, the string is parsed. If a
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_numpy.py` & `awkward-2.1.4/src/awkward/operations/ak_from_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_parquet.py` & `awkward-2.1.4/src/awkward/operations/ak_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_rdataframe.py` & `awkward-2.1.4/src/awkward/operations/ak_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_from_regular.py` & `awkward-2.1.4/src/awkward/operations/ak_from_regular.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("from_regular",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -65,14 +66,14 @@
         def action(layout, depth, **kwargs):
             posaxis = maybe_posaxis(layout, axis, depth)
             if posaxis == depth and layout.is_regular:
                 return layout.to_ListOffsetArray64(False)
             elif posaxis == depth and layout.is_list:
                 return layout
             elif layout.is_leaf:
-                raise np.AxisError(
+                raise AxisError(
                     f"axis={axis} exceeds the depth of this array ({depth})"
                 )
 
         out = ak._do.recursively_apply(layout, action, behavior, numpy_to_regular=True)
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_full_like.py` & `awkward-2.1.4/src/awkward/operations/ak_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_is_categorical.py` & `awkward-2.1.4/src/awkward/operations/ak_is_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_is_none.py` & `awkward-2.1.4/src/awkward/operations/ak_is_none.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("is_none",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer, regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -53,12 +54,12 @@
             else:
                 nplike = layout._backend.nplike
                 return ak.contents.NumpyArray(
                     nplike.zeros(layout.length, dtype=np.bool_)
                 )
 
         elif layout.is_leaf:
-            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
+            raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
 
     out = ak._do.recursively_apply(layout, action, behavior, numpy_to_regular=True)
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_is_tuple.py` & `awkward-2.1.4/src/awkward/operations/ak_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_is_valid.py` & `awkward-2.1.4/src/awkward/operations/ak_is_valid.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_isclose.py` & `awkward-2.1.4/src/awkward/operations/ak_isclose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_linear_fit.py` & `awkward-2.1.4/src/awkward/operations/ak_linear_fit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_local_index.py` & `awkward-2.1.4/src/awkward/operations/ak_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_mask.py` & `awkward-2.1.4/src/awkward/operations/ak_mask.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_max.py` & `awkward-2.1.4/src/awkward/operations/ak_max.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_mean.py` & `awkward-2.1.4/src/awkward/operations/ak_mean.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_merge_option_of_records.py` & `awkward-2.1.4/src/awkward/operations/ak_merge_option_of_records.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("merge_option_of_records",)
 import awkward as ak
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
@@ -64,15 +65,15 @@
             )
 
     layout = ak._do.recursively_apply(layout, apply_displace_index)
 
     def apply(layout, depth, backend, **kwargs):
         posaxis = maybe_posaxis(layout, axis, depth)
         if depth < posaxis + 1 and layout.is_leaf:
-            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
+            raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         elif depth == posaxis + 1 and layout.is_option and layout.content.is_record:
             layout = layout.to_IndexedOptionArray64()
 
             record = layout.content
             # Transpose option-of-record to record-of-option
             return ak.contents.RecordArray(
                 [
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_merge_union_of_records.py` & `awkward-2.1.4/src/awkward/operations/ak_merge_union_of_records.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("merge_union_of_records",)
 import awkward as ak
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import ArrayLike, NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
@@ -151,15 +152,15 @@
             dtype=index.dtype,
         )
         return dense_index
 
     def apply(layout, depth, backend, **kwargs):
         posaxis = maybe_posaxis(layout, axis, depth)
         if depth < posaxis + 1 and layout.is_leaf:
-            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
+            raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         elif depth == posaxis + 1 and layout.is_union:
             if not all(
                 x.is_record or x.is_indexed or x.is_option for x in layout.contents
             ):
                 return
 
             # Any option types need to be re-written
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_metadata_from_parquet.py` & `awkward-2.1.4/src/awkward/operations/ak_metadata_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_min.py` & `awkward-2.1.4/src/awkward/operations/ak_min.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_moment.py` & `awkward-2.1.4/src/awkward/operations/ak_moment.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_nan_to_none.py` & `awkward-2.1.4/src/awkward/operations/ak_nan_to_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_nan_to_num.py` & `awkward-2.1.4/src/awkward/operations/ak_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_num.py` & `awkward-2.1.4/src/awkward/operations/ak_num.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("num",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer, regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -92,12 +93,12 @@
     def action(layout, depth, **kwargs):
         posaxis = maybe_posaxis(layout, axis, depth)
 
         if posaxis == depth and layout.is_list:
             return ak.contents.NumpyArray(layout.stops.data - layout.starts.data)
 
         elif layout.is_leaf:
-            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
+            raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
 
     out = ak._do.recursively_apply(layout, action, behavior, numpy_to_regular=True)
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_ones_like.py` & `awkward-2.1.4/src/awkward/operations/ak_ones_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_pad_none.py` & `awkward-2.1.4/src/awkward/operations/ak_pad_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_parameters.py` & `awkward-2.1.4/src/awkward/operations/ak_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_prod.py` & `awkward-2.1.4/src/awkward/operations/ak_prod.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_ptp.py` & `awkward-2.1.4/src/awkward/operations/ak_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_ravel.py` & `awkward-2.1.4/src/awkward/operations/ak_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_run_lengths.py` & `awkward-2.1.4/src/awkward/operations/ak_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_singletons.py` & `awkward-2.1.4/src/awkward/operations/ak_singletons.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("singletons",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer, regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -76,12 +77,12 @@
                     ak.index.Index64(offsets), layout.project()
                 )
 
             else:
                 return ak.contents.RegularArray(layout, 1).to_ListOffsetArray64(True)
 
         elif layout.is_leaf:
-            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
+            raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
 
     out = ak._do.recursively_apply(layout, action, behavior, numpy_to_regular=True)
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_softmax.py` & `awkward-2.1.4/src/awkward/operations/ak_softmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_sort.py` & `awkward-2.1.4/src/awkward/operations/ak_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_std.py` & `awkward-2.1.4/src/awkward/operations/ak_std.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_strings_astype.py` & `awkward-2.1.4/src/awkward/operations/ak_strings_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_sum.py` & `awkward-2.1.4/src/awkward/operations/ak_sum.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_arrow.py` & `awkward-2.1.4/src/awkward/operations/ak_to_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_arrow_table.py` & `awkward-2.1.4/src/awkward/operations/ak_to_arrow_table.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_backend.py` & `awkward-2.1.4/src/awkward/operations/ak_to_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_buffers.py` & `awkward-2.1.4/src/awkward/operations/ak_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_categorical.py` & `awkward-2.1.4/src/awkward/operations/ak_to_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_cupy.py` & `awkward-2.1.4/src/awkward/operations/ak_to_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_dataframe.py` & `awkward-2.1.4/src/awkward/operations/ak_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_jax.py` & `awkward-2.1.4/src/awkward/operations/ak_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_json.py` & `awkward-2.1.4/src/awkward/operations/ak_to_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_layout.py` & `awkward-2.1.4/src/awkward/operations/ak_to_layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_list.py` & `awkward-2.1.4/src/awkward/operations/ak_to_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_numpy.py` & `awkward-2.1.4/src/awkward/operations/ak_to_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_packed.py` & `awkward-2.1.4/src/awkward/operations/ak_to_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_parquet.py` & `awkward-2.1.4/src/awkward/operations/ak_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_rdataframe.py` & `awkward-2.1.4/src/awkward/operations/ak_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_to_regular.py` & `awkward-2.1.4/src/awkward/operations/ak_to_regular.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_regular",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -77,14 +78,14 @@
 
         def action(layout, depth, **kwargs):
             posaxis = maybe_posaxis(layout, axis, depth)
             if posaxis == depth and layout.is_list:
                 return layout.to_RegularArray()
 
             elif layout.is_leaf:
-                raise np.AxisError(
+                raise AxisError(
                     f"axis={axis} exceeds the depth of this array ({depth})"
                 )
 
         out = ak._do.recursively_apply(layout, action, behavior)
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_transform.py` & `awkward-2.1.4/src/awkward/operations/ak_transform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_type.py` & `awkward-2.1.4/src/awkward/operations/ak_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_unflatten.py` & `awkward-2.1.4/src/awkward/operations/ak_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_unzip.py` & `awkward-2.1.4/src/awkward/operations/ak_unzip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_validity_error.py` & `awkward-2.1.4/src/awkward/operations/ak_validity_error.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_values_astype.py` & `awkward-2.1.4/src/awkward/operations/ak_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_var.py` & `awkward-2.1.4/src/awkward/operations/ak_var.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_where.py` & `awkward-2.1.4/src/awkward/operations/ak_where.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,18 +115,26 @@
             npcondition = backend.index_nplike.asarray(akcondition)
             tags = ak.index.Index8((npcondition == 0).view(np.int8))
             index = ak.index.Index64(
                 backend.index_nplike.arange(tags.length, dtype=np.int64),
                 nplike=backend.index_nplike,
             )
             if not isinstance(left, ak.contents.Content):
-                left = ak.contents.NumpyArray(backend.nplike.repeat(left, tags.length))
+                left = ak.contents.NumpyArray(
+                    backend.nplike.repeat(
+                        backend.nplike.asarray(left),
+                        backend.nplike.shape_item_as_index(tags.length),
+                    )
+                )
             if not isinstance(right, ak.contents.Content):
                 right = ak.contents.NumpyArray(
-                    backend.nplike.repeat(right, tags.length)
+                    backend.nplike.repeat(
+                        backend.nplike.asarray(right),
+                        backend.nplike.shape_item_as_index(tags.length),
+                    )
                 )
             return (
                 ak.contents.UnionArray.simplified(
                     tags,
                     index,
                     [left, right],
                     mergebool=mergebool,
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_with_field.py` & `awkward-2.1.4/src/awkward/operations/ak_with_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,22 +113,25 @@
             base, what = inputs
             backend = base.backend
 
             if isinstance(base, ak.contents.RecordArray):
                 if what is None:
                     what = ak.contents.IndexedOptionArray(
                         ak.index.Index64(
-                            backend.index_nplike.full(len(base), -1, dtype=np.int64),
+                            backend.index_nplike.full(base.length, -1, dtype=np.int64),
                             nplike=backend.index_nplike,
                         ),
                         ak.contents.EmptyArray(),
                     )
                 elif not isinstance(what, ak.contents.Content):
                     what = ak.contents.NumpyArray(
-                        backend.nplike.repeat(what, len(base))
+                        backend.nplike.repeat(
+                            backend.nplike.asarray(what),
+                            backend.nplike.shape_item_as_index(base.length),
+                        )
                     )
                 if base.is_tuple:
                     # Preserve tuple-ness
                     if where is None:
                         fields = None
                     # Otherwise the tuple becomes a record
                     else:
```

### Comparing `awkward-2.1.3/src/awkward/operations/ak_with_name.py` & `awkward-2.1.4/src/awkward/operations/ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_with_parameter.py` & `awkward-2.1.4/src/awkward/operations/ak_with_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_without_field.py` & `awkward-2.1.4/src/awkward/operations/ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_without_parameters.py` & `awkward-2.1.4/src/awkward/operations/ak_without_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_zeros_like.py` & `awkward-2.1.4/src/awkward/operations/ak_zeros_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/operations/ak_zip.py` & `awkward-2.1.4/src/awkward/operations/ak_zip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/types/__init__.py` & `awkward-2.1.4/src/awkward/types/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/types/_awkward_datashape_parser.py` & `awkward-2.1.4/src/awkward/types/_awkward_datashape_parser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/types/arraytype.py` & `awkward-2.1.4/src/awkward/types/arraytype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/types/listtype.py` & `awkward-2.1.4/src/awkward/types/listtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/types/numpytype.py` & `awkward-2.1.4/src/awkward/types/numpytype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/types/optiontype.py` & `awkward-2.1.4/src/awkward/types/optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/types/recordtype.py` & `awkward-2.1.4/src/awkward/types/recordtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/types/regulartype.py` & `awkward-2.1.4/src/awkward/types/regulartype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/types/scalartype.py` & `awkward-2.1.4/src/awkward/types/scalartype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/types/type.py` & `awkward-2.1.4/src/awkward/types/type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/types/uniontype.py` & `awkward-2.1.4/src/awkward/types/uniontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/src/awkward/types/unknowntype.py` & `awkward-2.1.4/src/awkward/types/unknowntype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0002_minimal_listarray.py` & `awkward-2.1.4/tests/test_0002_minimal_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0008_slices_and_getitem.py` & `awkward-2.1.4/tests/test_0008_slices_and_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0011_listarray.py` & `awkward-2.1.4/tests/test_0011_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0013_error_handling_struct.py` & `awkward-2.1.4/tests/test_0013_error_handling_struct.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0014_finish_up_getitem.py` & `awkward-2.1.4/tests/test_0014_finish_up_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0018_fromiter_fillable.py` & `awkward-2.1.4/tests/test_0018_fromiter_fillable.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0019_use_json_library.py` & `awkward-2.1.4/tests/test_0019_use_json_library.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0020_support_unsigned_indexes.py` & `awkward-2.1.4/tests/test_0020_support_unsigned_indexes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0021_emptyarray.py` & `awkward-2.1.4/tests/test_0021_emptyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0023_regular_array.py` & `awkward-2.1.4/tests/test_0023_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0024_use_regular_array.py` & `awkward-2.1.4/tests/test_0024_use_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0025_record_array.py` & `awkward-2.1.4/tests/test_0025_record_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0028_add_dressed_types.py` & `awkward-2.1.4/tests/test_0028_add_dressed_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0032_replace_dressedtype.py` & `awkward-2.1.4/tests/test_0032_replace_dressedtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0046_start_indexedarray.py` & `awkward-2.1.4/tests/test_0046_start_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0049_distinguish_record_and_recordarray_behaviors.py` & `awkward-2.1.4/tests/test_0049_distinguish_record_and_recordarray_behaviors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0057_introducing_forms.py` & `awkward-2.1.4/tests/test_0057_introducing_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0070_argmin_and_argmax.py` & `awkward-2.1.4/tests/test_0070_argmin_and_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0072_fillna_operation.py` & `awkward-2.1.4/tests/test_0072_fillna_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0074_argsort_and_sort.py` & `awkward-2.1.4/tests/test_0074_argsort_and_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0077_zip_operation.py` & `awkward-2.1.4/tests/test_0077_zip_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0078_argcross_and_cross.py` & `awkward-2.1.4/tests/test_0078_argcross_and_cross.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0079_argchoose_and_choose.py` & `awkward-2.1.4/tests/test_0079_argchoose_and_choose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0080_flatpandas_multiindex_rows_and_columns.py` & `awkward-2.1.4/tests/test_0080_flatpandas_multiindex_rows_and_columns.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0084_start_unionarray.py` & `awkward-2.1.4/tests/test_0084_start_unionarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0086_nep13_ufunc.py` & `awkward-2.1.4/tests/test_0086_nep13_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0089_numpy_functions.py` & `awkward-2.1.4/tests/test_0089_numpy_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0093_simplify_uniontypes_and_optiontypes.py` & `awkward-2.1.4/tests/test_0093_simplify_uniontypes_and_optiontypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0107_assign_fields_to_records.py` & `awkward-2.1.4/tests/test_0107_assign_fields_to_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0111_jagged_and_masked_getitem.py` & `awkward-2.1.4/tests/test_0111_jagged_and_masked_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0115_generic_reducer_operation.py` & `awkward-2.1.4/tests/test_0115_generic_reducer_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0118_numba_cpointers.py` & `awkward-2.1.4/tests/test_0118_numba_cpointers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0119_numexpr_and_broadcast_arrays.py` & `awkward-2.1.4/tests/test_0119_numexpr_and_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0124_strings_in_numba.py` & `awkward-2.1.4/tests/test_0124_strings_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0127_tomask_operation.py` & `awkward-2.1.4/tests/test_0127_tomask_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0127b_tomask_operation_numba.py` & `awkward-2.1.4/tests/test_0127b_tomask_operation_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0138_emptyarray_type.py` & `awkward-2.1.4/tests/test_0138_emptyarray_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0150_flatten.py` & `awkward-2.1.4/tests/test_0150_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0163_negative_axis_wrap.py` & `awkward-2.1.4/tests/test_0163_negative_axis_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0166_0167_0170_random_issues.py` & `awkward-2.1.4/tests/test_0166_0167_0170_random_issues.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0173_astype_operation.py` & `awkward-2.1.4/tests/test_0173_astype_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0184_concatenate_operation.py` & `awkward-2.1.4/tests/test_0184_concatenate_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0193_is_none_axis_parameter.py` & `awkward-2.1.4/tests/test_0193_is_none_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0198_tutorial_documentation_1.py` & `awkward-2.1.4/tests/test_0198_tutorial_documentation_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0222_count_with_axis0.py` & `awkward-2.1.4/tests/test_0222_count_with_axis0.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0224_arrow_to_awkward.py` & `awkward-2.1.4/tests/test_0224_arrow_to_awkward.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0264_reduce_last_empty.py` & `awkward-2.1.4/tests/test_0264_reduce_last_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0273_path_for_with_field.py` & `awkward-2.1.4/tests/test_0273_path_for_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0286_broadcast_single_value_with_field.py` & `awkward-2.1.4/tests/test_0286_broadcast_single_value_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0290_bug_fixes_for_hats.py` & `awkward-2.1.4/tests/test_0290_bug_fixes_for_hats.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0315_integerindex.py` & `awkward-2.1.4/tests/test_0315_integerindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0331_pandas_indexedarray.py` & `awkward-2.1.4/tests/test_0331_pandas_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0334_fully_broadcastable_where.py` & `awkward-2.1.4/tests/test_0334_fully_broadcastable_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0339_highlevel_sorting_function.py` & `awkward-2.1.4/tests/test_0339_highlevel_sorting_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0348_form_keys.py` & `awkward-2.1.4/tests/test_0348_form_keys.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0355_mixins.py` & `awkward-2.1.4/tests/test_0355_mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0395_complex_type_arrays.py` & `awkward-2.1.4/tests/test_0395_complex_type_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0395_fix_numba_indexedarray.py` & `awkward-2.1.4/tests/test_0395_fix_numba_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0397_arrays_as_constants_in_numba.py` & `awkward-2.1.4/tests/test_0397_arrays_as_constants_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0401_add_categorical_type_for_arrow_dictionary.py` & `awkward-2.1.4/tests/test_0401_add_categorical_type_for_arrow_dictionary.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0404_array_validity_check.py` & `awkward-2.1.4/tests/test_0404_array_validity_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0410_fix_argminmax_positions_for_missing_values.py` & `awkward-2.1.4/tests/test_0410_fix_argminmax_positions_for_missing_values.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0437_stream_of_many_json_files.py` & `awkward-2.1.4/tests/test_0437_stream_of_many_json_files.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0447_preserve_regularness_in_reduce.py` & `awkward-2.1.4/tests/test_0447_preserve_regularness_in_reduce.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0449_merge_many_arrays_in_one_pass.py` & `awkward-2.1.4/tests/test_0449_merge_many_arrays_in_one_pass.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0493_zeros_ones_full_like.py` & `awkward-2.1.4/tests/test_0493_zeros_ones_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0496_provide_local_index.py` & `awkward-2.1.4/tests/test_0496_provide_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0499_getitem_indexedarray_bug.py` & `awkward-2.1.4/tests/test_0499_getitem_indexedarray_bug.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0504_block_ufuncs_for_strings.py` & `awkward-2.1.4/tests/test_0504_block_ufuncs_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0511_copy_and_deepcopy.py` & `awkward-2.1.4/tests/test_0511_copy_and_deepcopy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py` & `awkward-2.1.4/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0549_numba_array_asarray.py` & `awkward-2.1.4/tests/test_0549_numba_array_asarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0557_min_max_initial_argument.py` & `awkward-2.1.4/tests/test_0557_min_max_initial_argument.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0559_fix_booleans_in_numba.py` & `awkward-2.1.4/tests/test_0559_fix_booleans_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0572_numba_array_ndim.py` & `awkward-2.1.4/tests/test_0572_numba_array_ndim.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0582_propagate_context_in_broadcast_and_apply.py` & `awkward-2.1.4/tests/test_0582_propagate_context_in_broadcast_and_apply.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0583_implement_unflatten_function.py` & `awkward-2.1.4/tests/test_0583_implement_unflatten_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0590_allow_regulararray_size_zero.py` & `awkward-2.1.4/tests/test_0590_allow_regulararray_size_zero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py` & `awkward-2.1.4/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0652_tests_of_complex_numbers.py` & `awkward-2.1.4/tests/test_0652_tests_of_complex_numbers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0674_categorical_validation.py` & `awkward-2.1.4/tests/test_0674_categorical_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0713_getitem_field_should_simplify_optiontype.py` & `awkward-2.1.4/tests/test_0713_getitem_field_should_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py` & `awkward-2.1.4/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0730_unflatten_axis_parameter.py` & `awkward-2.1.4/tests/test_0730_unflatten_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0733_run_lengths.py` & `awkward-2.1.4/tests/test_0733_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0736_implement_argsort_for_strings.py` & `awkward-2.1.4/tests/test_0736_implement_argsort_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0766_prevent_combinations_of_characters.py` & `awkward-2.1.4/tests/test_0766_prevent_combinations_of_characters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0773_typeparser.py` & `awkward-2.1.4/tests/test_0773_typeparser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0788_indexedarray_carrying_recordarray_parameters.py` & `awkward-2.1.4/tests/test_0788_indexedarray_carrying_recordarray_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0794_ak_cartesian_on_empty_array.py` & `awkward-2.1.4/tests/test_0794_ak_cartesian_on_empty_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0803_argsort_fix_type.py` & `awkward-2.1.4/tests/test_0803_argsort_fix_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0806_empty_lists_cartesian_fix.py` & `awkward-2.1.4/tests/test_0806_empty_lists_cartesian_fix.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0813_full_like_dtype_arg.py` & `awkward-2.1.4/tests/test_0813_full_like_dtype_arg.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0815_broadcast_union_types_to_all_possibilities.py` & `awkward-2.1.4/tests/test_0815_broadcast_union_types_to_all_possibilities.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0828_arrow_datatype_null.py` & `awkward-2.1.4/tests/test_0828_arrow_datatype_null.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0835_datetime_type.py` & `awkward-2.1.4/tests/test_0835_datetime_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0835_datetime_type_pandas.py` & `awkward-2.1.4/tests/test_0835_datetime_type_pandas.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0835_datetime_type_pyarrow.py` & `awkward-2.1.4/tests/test_0835_datetime_type_pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0850_argsort_mask_array.py` & `awkward-2.1.4/tests/test_0850_argsort_mask_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0866_getitem_field_and_flatten_unions.py` & `awkward-2.1.4/tests/test_0866_getitem_field_and_flatten_unions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0875_arrow_null_type.py` & `awkward-2.1.4/tests/test_0875_arrow_null_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0879_non_primitive_with_field.py` & `awkward-2.1.4/tests/test_0879_non_primitive_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0884_index_and_identifier_refactoring.py` & `awkward-2.1.4/tests/test_0884_index_and_identifier_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0889_ptp.py` & `awkward-2.1.4/tests/test_0889_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0896_content_classes_refactoring.py` & `awkward-2.1.4/tests/test_0896_content_classes_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0898_unzip_heterogeneous_records.py` & `awkward-2.1.4/tests/test_0898_unzip_heterogeneous_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0905_leading_zeros_in_unflatten.py` & `awkward-2.1.4/tests/test_0905_leading_zeros_in_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0906_arrow_fixed_size_list_type.py` & `awkward-2.1.4/tests/test_0906_arrow_fixed_size_list_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0910_unflatten_counts_relation.py` & `awkward-2.1.4/tests/test_0910_unflatten_counts_relation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0912_packed.py` & `awkward-2.1.4/tests/test_0912_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0914_types_and_forms.py` & `awkward-2.1.4/tests/test_0914_types_and_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0916_datetime_values_astype.py` & `awkward-2.1.4/tests/test_0916_datetime_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0927_numpy_array_nbytes.py` & `awkward-2.1.4/tests/test_0927_numpy_array_nbytes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0930_bug_in_unionarray_purelist_parameter.py` & `awkward-2.1.4/tests/test_0930_bug_in_unionarray_purelist_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0945_argsort_sort_nan_array.py` & `awkward-2.1.4/tests/test_0945_argsort_sort_nan_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0958_new_forms_must_accept_old_form_json.py` & `awkward-2.1.4/tests/test_0958_new_forms_must_accept_old_form_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0959__getitem_array_implementation.py` & `awkward-2.1.4/tests/test_0959__getitem_array_implementation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0975_mask_multidimensional_numpy_array.py` & `awkward-2.1.4/tests/test_0975_mask_multidimensional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0979_where_multidimentional_numpy_array.py` & `awkward-2.1.4/tests/test_0979_where_multidimentional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0982_missing_case_in_nonlocal_reducers.py` & `awkward-2.1.4/tests/test_0982_missing_case_in_nonlocal_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0984_ravel.py` & `awkward-2.1.4/tests/test_0984_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_0992_correct_ptp_unmasking.py` & `awkward-2.1.4/tests/test_0992_correct_ptp_unmasking.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py` & `awkward-2.1.4/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1017_numpyarray_broadcast.py` & `awkward-2.1.4/tests/test_1017_numpyarray_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1030_mixin_class_name.py` & `awkward-2.1.4/tests/test_1030_mixin_class_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1031_start_getitem_next.py` & `awkward-2.1.4/tests/test_1031_start_getitem_next.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1031b_start_getitem_next_specialized.py` & `awkward-2.1.4/tests/test_1031b_start_getitem_next_specialized.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1049_concatenate_single_array.py` & `awkward-2.1.4/tests/test_1049_concatenate_single_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1055_fill_none_numpy_dimension.py` & `awkward-2.1.4/tests/test_1055_fill_none_numpy_dimension.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1059_localindex.py` & `awkward-2.1.4/tests/test_1059_localindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1066_to_numpy_masked_structured_array.py` & `awkward-2.1.4/tests/test_1066_to_numpy_masked_structured_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1071_mask_identity_false_should_not_return_option_type.py` & `awkward-2.1.4/tests/test_1071_mask_identity_false_should_not_return_option_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1072_sort.py` & `awkward-2.1.4/tests/test_1072_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1074_combinations.py` & `awkward-2.1.4/tests/test_1074_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1075_validityerror.py` & `awkward-2.1.4/tests/test_1075_validityerror.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1110_type_tracer_1.py` & `awkward-2.1.4/tests/test_1110_type_tracer_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1116_project_maskedarrays.py` & `awkward-2.1.4/tests/test_1116_project_maskedarrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1125_to_arrow_from_arrow.py` & `awkward-2.1.4/tests/test_1125_to_arrow_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1132_utility_methods_for_highlevel_functions.py` & `awkward-2.1.4/tests/test_1132_utility_methods_for_highlevel_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1134_from_buffers_to_buffers.py` & `awkward-2.1.4/tests/test_1134_from_buffers_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1135_rpad_operation.py` & `awkward-2.1.4/tests/test_1135_rpad_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1136_regulararray_zeros_in_shape.py` & `awkward-2.1.4/tests/test_1136_regulararray_zeros_in_shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1137_num.py` & `awkward-2.1.4/tests/test_1137_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1142_numbers_to_type.py` & `awkward-2.1.4/tests/test_1142_numbers_to_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1149_datetime_sort.py` & `awkward-2.1.4/tests/test_1149_datetime_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1154_arrow_tables_should_preserve_parameters.py` & `awkward-2.1.4/tests/test_1154_arrow_tables_should_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1162_ak_from_json_schema.py` & `awkward-2.1.4/tests/test_1162_ak_from_json_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1183_bugs_found_by_dask_project_2.py` & `awkward-2.1.4/tests/test_1183_bugs_found_by_dask_project_2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1189_fix_singletons_for_non_optional_data.py` & `awkward-2.1.4/tests/test_1189_fix_singletons_for_non_optional_data.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1192_iterables_in___array_function__.py` & `awkward-2.1.4/tests/test_1192_iterables_in___array_function__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1193_is_none_nested_option.py` & `awkward-2.1.4/tests/test_1193_is_none_nested_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1233_ak_with_name.py` & `awkward-2.1.4/tests/test_1233_ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1240_v2_implementation_of_numba_1.py` & `awkward-2.1.4/tests/test_1240_v2_implementation_of_numba_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1259_simplify_optiontype.py` & `awkward-2.1.4/tests/test_1259_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1260_simplify_masked_option_types.py` & `awkward-2.1.4/tests/test_1260_simplify_masked_option_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1271_fix_4D_reducers.py` & `awkward-2.1.4/tests/test_1271_fix_4D_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1294_to_and_from_parquet.py` & `awkward-2.1.4/tests/test_1294_to_and_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py` & `awkward-2.1.4/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1300_awkward_to_cpp_converter_with_cling.py` & `awkward-2.1.4/tests/test_1300_awkward_to_cpp_converter_with_cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1300b_same_for_numba.py` & `awkward-2.1.4/tests/test_1300b_same_for_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1308_zip_after_option.py` & `awkward-2.1.4/tests/test_1308_zip_after_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1318_array_function_types.py` & `awkward-2.1.4/tests/test_1318_array_function_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1320_mask_identity_defaults.py` & `awkward-2.1.4/tests/test_1320_mask_identity_defaults.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1344_broadcast_arrays_depth_limit.py` & `awkward-2.1.4/tests/test_1344_broadcast_arrays_depth_limit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1345_avro_reader.py` & `awkward-2.1.4/tests/test_1345_avro_reader.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1351_is_tuple.py` & `awkward-2.1.4/tests/test_1351_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1374_to_rdataframe.py` & `awkward-2.1.4/tests/test_1374_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1377_ravel_string.py` & `awkward-2.1.4/tests/test_1377_ravel_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1379_reducers_with_axis_None_and_typetracers.py` & `awkward-2.1.4/tests/test_1379_reducers_with_axis_None_and_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1399_from_jax.py` & `awkward-2.1.4/tests/test_1399_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1399_to_jax.py` & `awkward-2.1.4/tests/test_1399_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1405_slicing_untested_cases.py` & `awkward-2.1.4/tests/test_1405_slicing_untested_cases.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1415_behaviour_forwarding.py` & `awkward-2.1.4/tests/test_1415_behaviour_forwarding.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1440_start_v2_to_parquet.py` & `awkward-2.1.4/tests/test_1440_start_v2_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1447_jax_autodiff_slices_ufuncs.py` & `awkward-2.1.4/tests/test_1447_jax_autodiff_slices_ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1449_v2_to_json_from_json_functions.py` & `awkward-2.1.4/tests/test_1449_v2_to_json_from_json_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1453_write_single_records_to_parquet.py` & `awkward-2.1.4/tests/test_1453_write_single_records_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1473_from_rdataframe.py` & `awkward-2.1.4/tests/test_1473_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1477_generator_entry_type_as_rvec.py` & `awkward-2.1.4/tests/test_1477_generator_entry_type_as_rvec.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1490_jax_reducers_combinations.py` & `awkward-2.1.4/tests/test_1490_jax_reducers_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1502_getitem_jagged_issue1406.py` & `awkward-2.1.4/tests/test_1502_getitem_jagged_issue1406.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1504_typetracer_like.py` & `awkward-2.1.4/tests/test_1504_typetracer_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1508_awkward_from_rdataframe.py` & `awkward-2.1.4/tests/test_1508_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1511_set_attribute.py` & `awkward-2.1.4/tests/test_1511_set_attribute.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1539_isnone_axis_check_issue1417.py` & `awkward-2.1.4/tests/test_1539_isnone_axis_check_issue1417.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1559_fix_ufuncs_records_1439.py` & `awkward-2.1.4/tests/test_1559_fix_ufuncs_records_1439.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1565_axis_wrap_if_negative_record.py` & `awkward-2.1.4/tests/test_1565_axis_wrap_if_negative_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1567_fix_longlong_in_Index.py` & `awkward-2.1.4/tests/test_1567_fix_longlong_in_Index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1568_fix_lengths_empty_regular_slices.py` & `awkward-2.1.4/tests/test_1568_fix_lengths_empty_regular_slices.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1586_concatenate_should_preserve_regulararray.py` & `awkward-2.1.4/tests/test_1586_concatenate_should_preserve_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1604_preserve_form_in_concatenate.py` & `awkward-2.1.4/tests/test_1604_preserve_form_in_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1607_no_reducers_on_records.py` & `awkward-2.1.4/tests/test_1607_no_reducers_on_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1613_generator_tolayout_records.py` & `awkward-2.1.4/tests/test_1613_generator_tolayout_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1619_from_parquet_empty_field.py` & `awkward-2.1.4/tests/test_1619_from_parquet_empty_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1620_layout_builders.py` & `awkward-2.1.4/tests/test_1620_layout_builders.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1625_multiple_columns_from_rdataframe.py` & `awkward-2.1.4/tests/test_1625_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1642_from_iter_of_tuples.py` & `awkward-2.1.4/tests/test_1642_from_iter_of_tuples.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1650_Record_to_list_should_listify_itself.py` & `awkward-2.1.4/tests/test_1650_Record_to_list_should_listify_itself.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1671_categorical_type.py` & `awkward-2.1.4/tests/test_1671_categorical_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1672_broadcast_parameters.py` & `awkward-2.1.4/tests/test_1672_broadcast_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1677_array_builder_in_numba.py` & `awkward-2.1.4/tests/test_1677_array_builder_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1685_IndexedArray_project_parameters.py` & `awkward-2.1.4/tests/test_1685_IndexedArray_project_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1686_UnionArray_simplified_preserve_parameters.py` & `awkward-2.1.4/tests/test_1686_UnionArray_simplified_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1688_pack_categorical.py` & `awkward-2.1.4/tests/test_1688_pack_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1703_fill_none_typetracer.py` & `awkward-2.1.4/tests/test_1703_fill_none_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1707_broadcast_parameters_ufunc.py` & `awkward-2.1.4/tests/test_1707_broadcast_parameters_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1709_ak_array_constructor_behavior.py` & `awkward-2.1.4/tests/test_1709_ak_array_constructor_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1747_bytemaskedarray_mergemany.py` & `awkward-2.1.4/tests/test_1747_bytemaskedarray_mergemany.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1753_indexedarray_merge_kernel.py` & `awkward-2.1.4/tests/test_1753_indexedarray_merge_kernel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1762_jax_behavior_support.py` & `awkward-2.1.4/tests/test_1762_jax_behavior_support.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1764_jax_jacobian.py` & `awkward-2.1.4/tests/test_1764_jax_jacobian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1765_add_ioanas_test_of_to_arraylib.py` & `awkward-2.1.4/tests/test_1765_add_ioanas_test_of_to_arraylib.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1766_record_form_fields.py` & `awkward-2.1.4/tests/test_1766_record_form_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1781_rdataframe_snapshot.py` & `awkward-2.1.4/tests/test_1781_rdataframe_snapshot.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1784_reduce_leading_sublist.py` & `awkward-2.1.4/tests/test_1784_reduce_leading_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1790_reduce_regulararray.py` & `awkward-2.1.4/tests/test_1790_reduce_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1791_reduce_trailing_sublist.py` & `awkward-2.1.4/tests/test_1791_reduce_trailing_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1794_run_lengths_empty_sublist.py` & `awkward-2.1.4/tests/test_1794_run_lengths_empty_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1829_to_from_rdataframe_bool.py` & `awkward-2.1.4/tests/test_1829_to_from_rdataframe_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py` & `awkward-2.1.4/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1847_numpy_array_contiguous.py` & `awkward-2.1.4/tests/test_1847_numpy_array_contiguous.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1850_bytemasked_array_to_bytemaskedarray.py` & `awkward-2.1.4/tests/test_1850_bytemasked_array_to_bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1867_pass_behavior_through_combinations.py` & `awkward-2.1.4/tests/test_1867_pass_behavior_through_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1904_drop_none.py` & `awkward-2.1.4/tests/test_1904_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1914_improved_axis_to_posaxis.py` & `awkward-2.1.4/tests/test_1914_improved_axis_to_posaxis.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py` & `awkward-2.1.4/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1930_unflatten_counts_checks.py` & `awkward-2.1.4/tests/test_1930_unflatten_counts_checks.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1936_with_field_broadcasting.py` & `awkward-2.1.4/tests/test_1936_with_field_broadcasting.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1940_ak_backend.py` & `awkward-2.1.4/tests/test_1940_ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1943_regular_indexing.py` & `awkward-2.1.4/tests/test_1943_regular_indexing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1960_awkward_from_rdataframe.py` & `awkward-2.1.4/tests/test_1960_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_1961_ak_without_field.py` & `awkward-2.1.4/tests/test_1961_ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2020_reduce_axis_none.py` & `awkward-2.1.4/tests/test_2020_reduce_axis_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2021_check_TypeTracerArray_in_ak_where.py` & `awkward-2.1.4/tests/test_2021_check_TypeTracerArray_in_ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2023_from_rdataframe.py` & `awkward-2.1.4/tests/test_2023_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py` & `awkward-2.1.4/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2047_ak_transform_regular_to_jagged.py` & `awkward-2.1.4/tests/test_2047_ak_transform_regular_to_jagged.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2055_array_builder_check.py` & `awkward-2.1.4/tests/test_2055_array_builder_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2058_merge_numpy_array.py` & `awkward-2.1.4/tests/test_2058_merge_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2064_fill_none_record.py` & `awkward-2.1.4/tests/test_2064_fill_none_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2067_to_buffers_byteorder.py` & `awkward-2.1.4/tests/test_2067_to_buffers_byteorder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2070_to_layout_string.py` & `awkward-2.1.4/tests/test_2070_to_layout_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2071_unflatten_non_packed_counts.py` & `awkward-2.1.4/tests/test_2071_unflatten_non_packed_counts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2078_array_function_wrap.py` & `awkward-2.1.4/tests/test_2078_array_function_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2082_broadcast_zero_size.py` & `awkward-2.1.4/tests/test_2082_broadcast_zero_size.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2096_ak_scalar_type.py` & `awkward-2.1.4/tests/test_2096_ak_scalar_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2101_pickle_behavior_class.py` & `awkward-2.1.4/tests/test_2101_pickle_behavior_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2104_numpy_merge_option.py` & `awkward-2.1.4/tests/test_2104_numpy_merge_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2106_pickle_class.py` & `awkward-2.1.4/tests/test_2106_pickle_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2108_fill_none_indexed.py` & `awkward-2.1.4/tests/test_2108_fill_none_indexed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2115_fix_up_typetracers.py` & `awkward-2.1.4/tests/test_2115_fix_up_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2125_type_of_scalar.py` & `awkward-2.1.4/tests/test_2125_type_of_scalar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2150_typetracer_high_level_ufunc.py` & `awkward-2.1.4/tests/test_2150_typetracer_high_level_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2179_parameter_merging_rules.py` & `awkward-2.1.4/tests/test_2179_parameter_merging_rules.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2185_merge_union_of_records.py` & `awkward-2.1.4/tests/test_2185_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py` & `awkward-2.1.4/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2198_almost_equal.py` & `awkward-2.1.4/tests/test_2198_almost_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2202_filter_multiple_columns_from_rdataframe.py` & `awkward-2.1.4/tests/test_2202_filter_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2214_offset_bool_index.py` & `awkward-2.1.4/tests/test_2214_offset_bool_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2226_slice_regulararray_typetracer.py` & `awkward-2.1.4/tests/test_2226_slice_regulararray_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2229_getitem_range_slice.py` & `awkward-2.1.4/tests/test_2229_getitem_range_slice.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2234_from_rdataframe_keep_order.py` & `awkward-2.1.4/tests/test_2234_from_rdataframe_keep_order.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2236_merge_union_of_records_option.py` & `awkward-2.1.4/tests/test_2236_merge_union_of_records_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2240_simplify_merge_as_union.py` & `awkward-2.1.4/tests/test_2240_simplify_merge_as_union.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2246_slice_not_packed.py` & `awkward-2.1.4/tests/test_2246_slice_not_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2250_full_like_bool.py` & `awkward-2.1.4/tests/test_2250_full_like_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2258_from_rdataframe_with_arguments.py` & `awkward-2.1.4/tests/test_2258_from_rdataframe_with_arguments.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2263_to_packed_list.py` & `awkward-2.1.4/tests/test_2263_to_packed_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2266_fix_nan_to_num.py` & `awkward-2.1.4/tests/test_2266_fix_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2267_broadcast_fields.py` & `awkward-2.1.4/tests/test_2267_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2293_unflatten_typetracer.py` & `awkward-2.1.4/tests/test_2293_unflatten_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2297_common_backend.py` & `awkward-2.1.4/tests/test_2297_common_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2306_cppyy_git.py` & `awkward-2.1.4/tests/test_2306_cppyy_git.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2319_from_buffers_array.py` & `awkward-2.1.4/tests/test_2319_from_buffers_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2327_array_interface.py` & `awkward-2.1.4/tests/test_2327_array_interface.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2329_cartesian_broadcasting_fixes.py` & `awkward-2.1.4/tests/test_2329_cartesian_broadcasting_fixes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2349_growablebuffer_in_numba.py` & `awkward-2.1.4/tests/test_2349_growablebuffer_in_numba.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,40 +86,40 @@
     growablebuffer.extend(np.array(range(30, 50)))
     assert growablebuffer.snapshot().tolist() == list(range(50))
     assert len(growablebuffer._panels) == 3
 
     # fill more than one panel, starting at a threshold
     growablebuffer.extend(np.array(range(50, 80)))
     assert growablebuffer.snapshot().tolist() == list(range(80))
-    assert len(growablebuffer._panels) == 5
+    assert len(growablebuffer._panels) == 4
 
     # fill more than one panel, not starting at a threshold, but ending on one
     growablebuffer.extend(np.array(range(80, 110)))
     assert growablebuffer.snapshot().tolist() == list(range(110))
-    assert len(growablebuffer._panels) == 6
+    assert len(growablebuffer._panels) == 5
 
     # fill lots of panels, starting at a threshold
     growablebuffer.extend(np.array(range(110, 160)))
     assert growablebuffer.snapshot().tolist() == list(range(160))
-    assert len(growablebuffer._panels) == 9
+    assert len(growablebuffer._panels) == 6
 
     # fill lots of panels, not starting at a threshold or ending on one
     growablebuffer.extend(np.array(range(160, 200)))
     assert growablebuffer.snapshot().tolist() == list(range(200))
-    assert len(growablebuffer._panels) == 11
+    assert len(growablebuffer._panels) == 7
 
     # fill lots of panels, not starting at a threshold, but ending on one
     growablebuffer.extend(np.array(range(200, 250)))
     assert growablebuffer.snapshot().tolist() == list(range(250))
-    assert len(growablebuffer._panels) == 13
+    assert len(growablebuffer._panels) == 8
 
     # fill a whole lot of panels, just for fun
     growablebuffer.extend(np.array(range(250, 1000)))
     assert growablebuffer.snapshot().tolist() == list(range(1000))
-    assert len(growablebuffer._panels) == 51
+    assert len(growablebuffer._panels) == 9
 
 
 def test_unbox():
     @numba.njit
     def f1(x):
         x  # noqa: B018 (we want to test the unboxing)
         return 3.14
@@ -476,33 +476,33 @@
     extend_range(growablebuffer, 30, 50)
     assert snapshot(growablebuffer).tolist() == list(range(50))
     assert len(growablebuffer._panels) == 3
 
     # fill more than one panel, starting at a threshold
     extend_range(growablebuffer, 50, 80)
     assert snapshot(growablebuffer).tolist() == list(range(80))
-    assert len(growablebuffer._panels) == 5
+    assert len(growablebuffer._panels) == 4
 
     # fill more than one panel, not starting at a threshold, but ending on one
     extend_range(growablebuffer, 80, 110)
     assert snapshot(growablebuffer).tolist() == list(range(110))
-    assert len(growablebuffer._panels) == 6
+    assert len(growablebuffer._panels) == 5
 
     # fill lots of panels, starting at a threshold
     extend_range(growablebuffer, 110, 160)
     assert snapshot(growablebuffer).tolist() == list(range(160))
-    assert len(growablebuffer._panels) == 9
+    assert len(growablebuffer._panels) == 6
 
     # fill lots of panels, not starting at a threshold or ending on one
     extend_range(growablebuffer, 160, 200)
     assert snapshot(growablebuffer).tolist() == list(range(200))
-    assert len(growablebuffer._panels) == 11
+    assert len(growablebuffer._panels) == 7
 
     # fill lots of panels, not starting at a threshold, but ending on one
     extend_range(growablebuffer, 200, 250)
     assert snapshot(growablebuffer).tolist() == list(range(250))
-    assert len(growablebuffer._panels) == 13
+    assert len(growablebuffer._panels) == 8
 
     # fill a whole lot of panels, just for fun
     extend_range(growablebuffer, 250, 1000)
     assert snapshot(growablebuffer).tolist() == list(range(1000))
-    assert len(growablebuffer._panels) == 51
+    assert len(growablebuffer._panels) == 9
```

### Comparing `awkward-2.1.3/tests/test_2354_ufunc_same_backend.py` & `awkward-2.1.4/tests/test_2354_ufunc_same_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2355_to_backend_record.py` & `awkward-2.1.4/tests/test_2355_to_backend_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2361_typetracer_asarray_nd.py` & `awkward-2.1.4/tests/test_2361_typetracer_asarray_nd.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2368_type_is_equal.py` & `awkward-2.1.4/tests/test_2368_type_is_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2373_unzip_touching.py` & `awkward-2.1.4/tests/test_2373_unzip_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2374_cartesian_touching.py` & `awkward-2.1.4/tests/test_2374_cartesian_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2385_with_field_empty_record.py` & `awkward-2.1.4/tests/test_2385_with_field_empty_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/test_2395_copy_asarray_touch.py` & `awkward-2.1.4/tests/test_2395_copy_asarray_touch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/list-depths-records-list.parquet` & `awkward-2.1.4/tests/samples/list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/list-depths-records.parquet` & `awkward-2.1.4/tests/samples/list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/list-depths-strings.parquet` & `awkward-2.1.4/tests/samples/list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/list-depths.parquet` & `awkward-2.1.4/tests/samples/list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/nonnullable-depths.parquet` & `awkward-2.1.4/tests/samples/nonnullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/nullable-depths.parquet` & `awkward-2.1.4/tests/samples/nullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/nullable-levels.parquet` & `awkward-2.1.4/tests/samples/nullable-levels.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/nullable-list-depths-records-list.parquet` & `awkward-2.1.4/tests/samples/nullable-list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/nullable-list-depths-records.parquet` & `awkward-2.1.4/tests/samples/nullable-list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/nullable-list-depths-strings.parquet` & `awkward-2.1.4/tests/samples/nullable-list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/nullable-list-depths.parquet` & `awkward-2.1.4/tests/samples/nullable-list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/nullable-record-primitives.parquet` & `awkward-2.1.4/tests/samples/nullable-record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/record-primitives.parquet` & `awkward-2.1.4/tests/samples/record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/test-nan-inf.json` & `awkward-2.1.4/tests/samples/test-nan-inf.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/test-two-arrays.json` & `awkward-2.1.4/tests/samples/test-two-arrays.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests/samples/test.json` & `awkward-2.1.4/tests/samples/test.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests-cuda/test_1276_cuda_num.py` & `awkward-2.1.4/tests-cuda/test_1276_cuda_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests-cuda/test_1276_cuda_transfers.py` & `awkward-2.1.4/tests-cuda/test_1276_cuda_transfers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests-cuda/test_1276_cupy_interop.py` & `awkward-2.1.4/tests-cuda/test_1276_cupy_interop.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests-cuda/test_1276_from_cupy.py` & `awkward-2.1.4/tests-cuda/test_1276_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests-cuda/test_1300_same_for_numba_cuda.py` & `awkward-2.1.4/tests-cuda/test_1300_same_for_numba_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests-cuda/test_1381_check_errors.py` & `awkward-2.1.4/tests-cuda/test_1381_check_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/tests-cuda/test_1809_array_cuda_jit.py` & `awkward-2.1.4/tests-cuda/test_1809_array_cuda_jit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/.gitignore` & `awkward-2.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/LICENSE` & `awkward-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `awkward-2.1.3/pyproject.toml` & `awkward-2.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "hatchling>=1.10.0",
     "hatch-fancy-pypi-readme"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awkward"
-version = "2.1.3"
+version = "2.1.4"
 description = "Manipulate JSON-like data with NumPy-like idioms."
 license = { text = "BSD-3-Clause" }
 requires-python = ">=3.7"
 authors = [
     { name = "Jim Pivarski", email = "pivarski@princeton.edu" },
 ]
 classifiers = [
@@ -36,15 +36,15 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
 dependencies = [
-    "awkward_cpp==14",
+    "awkward_cpp==15",
     "importlib_resources;python_version < \"3.9\"",
     "numpy>=1.17.0",
     "packaging",
     "typing_extensions>=4.1.0; python_version < \"3.11\""
 ]
 dynamic = [
     "readme"
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 [build-system] requires = [ "hatchling>=1.10.0", "hatch-fancy-pypi-readme" ]
-build-backend = "hatchling.build" [project] name = "awkward" version = "2.1.3"
+build-backend = "hatchling.build" [project] name = "awkward" version = "2.1.4"
 description = "Manipulate JSON-like data with NumPy-like idioms." license =
 { text = "BSD-3-Clause" } requires-python = ">=3.7" authors = [ { name = "Jim
 Pivarski", email = "pivarski@princeton.edu" }, ] classifiers = [ "Development
 Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended
 Audience :: Information Technology", "Intended Audience :: Science/Research",
 "License :: OSI Approved :: BSD License", "Operating System :: MacOS :: MacOS
 X", "Operating System :: Microsoft :: Windows", "Operating System :: POSIX ::
@@ -11,15 +11,15 @@
 "Programming Language :: Python :: 3", "Programming Language :: Python :: 3 ::
 Only", "Programming Language :: Python :: 3.7", "Programming Language :: Python
 :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language ::
 Python :: 3.10", "Programming Language :: Python :: 3.11", "Topic ::
 Scientific/Engineering", "Topic :: Scientific/Engineering :: Information
 Analysis", "Topic :: Scientific/Engineering :: Mathematics", "Topic ::
 Scientific/Engineering :: Physics", "Topic :: Software Development", "Topic ::
-Utilities", ] dependencies = [ "awkward_cpp==14",
+Utilities", ] dependencies = [ "awkward_cpp==15",
 "importlib_resources;python_version < \"3.9\"", "numpy>=1.17.0", "packaging",
 "typing_extensions>=4.1.0; python_version < \"3.11\"" ] dynamic = [ "readme" ]
 [project.entry-points.numba_extensions] init = "awkward.numba:_register"
 [project.urls] "Bug Tracker" = "https://github.com/scikit-hep/awkward-1.0/
 issues" "Chat" = "https://gitter.im/Scikit-HEP/awkward-array" "Discussions" =
 "https://github.com/scikit-hep/awkward-1.0/discussions" "Documentation" =
 "https://awkward-array.org" "Homepage" = "https://github.com/scikit-hep/
```

### Comparing `awkward-2.1.3/PKG-INFO` & `awkward-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awkward
-Version: 2.1.3
+Version: 2.1.4
 Summary: Manipulate JSON-like data with NumPy-like idioms.
 Project-URL: Bug Tracker, https://github.com/scikit-hep/awkward-1.0/issues
 Project-URL: Chat, https://gitter.im/Scikit-HEP/awkward-array
 Project-URL: Discussions, https://github.com/scikit-hep/awkward-1.0/discussions
 Project-URL: Documentation, https://awkward-array.org
 Project-URL: Homepage, https://github.com/scikit-hep/awkward-1.0
 Project-URL: Releases, https://github.com/scikit-hep/awkward-1.0/releases
@@ -32,15 +32,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Requires-Dist: awkward-cpp==14
+Requires-Dist: awkward-cpp==15
 Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/scikit-hep/awkward-1.0">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: awkward Version: 2.1.3 Summary: Manipulate JSON-
+Metadata-Version: 2.1 Name: awkward Version: 2.1.4 Summary: Manipulate JSON-
 like data with NumPy-like idioms. Project-URL: Bug Tracker, https://github.com/
 scikit-hep/awkward-1.0/issues Project-URL: Chat, https://gitter.im/Scikit-HEP/
 awkward-array Project-URL: Discussions, https://github.com/scikit-hep/awkward-
 1.0/discussions Project-URL: Documentation, https://awkward-array.org Project-
 URL: Homepage, https://github.com/scikit-hep/awkward-1.0 Project-URL: Releases,
 https://github.com/scikit-hep/awkward-1.0/releases Project-URL: Source Code,
 https://github.com/scikit-hep/awkward-1.0 Author-email: Jim Pivarski
@@ -18,15 +18,15 @@
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
 Software Development Classifier: Topic :: Utilities Requires-Python: >=3.7
-Requires-Dist: awkward-cpp==14 Requires-Dist: importlib-resources;
+Requires-Dist: awkward-cpp==15 Requires-Dist: importlib-resources;
 python_version < '3.9' Requires-Dist: numpy>=1.17.0 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11' Description-
 Content-Type: text/markdown [https://github.com/scikit-hep/awkward-1.0/raw/
 main/docs-img/logo/logo-300px.png] [![PyPI version](https://badge.fury.io/py/
 awkward.svg)](https://pypi.org/project/awkward) [![Conda-Forge](https://
 img.shields.io/conda/vn/conda-forge/awkward)](https://github.com/conda-forge/
 awkward-feedstock) [![Python 3.7â3.11](https://img.shields.io/badge/python-
```

