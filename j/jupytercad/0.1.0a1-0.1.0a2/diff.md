# Comparing `tmp/jupytercad-0.1.0a1.tar.gz` & `tmp/jupytercad-0.1.0a2.tar.gz`

## Comparing `jupytercad-0.1.0a1.tar` & `jupytercad-0.1.0a2.tar`

### file list

```diff
@@ -1,162 +1,174 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/.eslintrc.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/.prettierignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/.prettierrc
--rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/CHANGELOG.md
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/RELEASE.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/extension.webpack.config.js
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/install.json
--rw-r--r--   0        0        0   340807 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad-screenshot.png
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/package.json
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/schema.js
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/setup.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/tsconfig.json
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/tsconfig.worker.json
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/worker.webpack.config.js
--rw-r--r--   0        0        0   311099 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/yarn.lock
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/.github/workflows/binder-on-pr.yml
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/.github/workflows/build.yml
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/.github/workflows/check-release.yml
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/.github/workflows/enforce-labels.yml
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/.github/workflows/update_galata_references.yaml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/binder/environment.yml
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/binder/jupyter_config.json
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/binder/postBuild
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/binder/start
--rw-r--r--   0        0        0   300736 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/examples/ArchDetail.FCStd
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/examples/common.FCStd
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/examples/cut.FCStd
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/examples/example1.FCStd
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/examples/example2.FCStd
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/examples/example3.FCStd
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/examples/example4.FCStd
--rw-r--r--   0        0        0    27100 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/examples/example5.FCStd
--rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/examples/example6.FCStd
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/examples/example_2D.FCStd
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/examples/test.jcad
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/_version.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/fcstd_ydoc.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/jcad_ydoc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/__init__.py
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/loader.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/__init__.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/base_prop.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/property_angle.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/property_bool.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/property_distance.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/property_geometrylist.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/property_length.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/property_link.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/property_link_list.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/property_map.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/property_partshape.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/property_placement.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/geometry/__init__.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/geometry/geom_circle.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad/freecad/props/geometry/geom_linesegment.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad-opencascade/build.yml
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad-opencascade/build_opencascade.js
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad-opencascade/package.json
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/jupytercad-opencascade/yarn.lock
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/scripts/bump-version.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/factory.ts
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/index.ts
--rw-r--r--   0        0        0    35619 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/mainview.tsx
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/model.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/svg.d.ts
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/token.ts
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/tools.ts
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/types.ts
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/widget.tsx
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/annotation/message.tsx
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/annotation/model.ts
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/annotation/view.tsx
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/fcplugin/modelfactory.ts
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/fcplugin/plugins.ts
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/jcadplugin/modelfactory.ts
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/jcadplugin/plugins.ts
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/panelview/annotations.tsx
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/panelview/formbuilder.tsx
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/panelview/header.tsx
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/panelview/leftpanel.tsx
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/panelview/model.ts
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/panelview/objectproperties.tsx
--rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/panelview/objecttree.tsx
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/panelview/rightpanel.tsx
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/box.json
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/cone.json
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/cut.json
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/cylinder.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/extrusion.json
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/fuse.json
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/geomCircle.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/geomLineSegment.json
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/intersection.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/jcad.json
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/placement.json
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/sketch.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/sphere.json
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/schema/torus.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/sketcher/helper.tsx
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/sketcher/panzoom.ts
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/sketcher/sketcherdialog.tsx
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/sketcher/sketchermodel.ts
--rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/sketcher/sketcherwidget.tsx
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/sketcher/types.ts
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/sketcher/elements/circle.ts
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/sketcher/elements/line.ts
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/sketcher/elements/point.ts
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/toolbar/formdialog.tsx
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/toolbar/helpertoolbar.tsx
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/toolbar/model.ts
--rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/toolbar/operatortoolbar.tsx
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/toolbar/parttoolbar.tsx
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/toolbar/sketchertoolbar.tsx
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/toolbar/toolbar.tsx
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/toolbar/usertoolbar.tsx
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/toolbar/widget.tsx
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/worker/actions.ts
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/worker/occapi.ts
--rw-r--r--   0        0        0     8542 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/worker/occparser.ts
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/worker/types.ts
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/worker/utils.ts
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/worker/worker.ts
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/worker/geometry/geomCircle.ts
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/src/worker/geometry/geomLineSegment.ts
--rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/style/index.js
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/style/icon/jvcontrol.svg
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/style/icon/minimize.svg
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/style/icon/visibility.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/style/icon/visibilityOff.svg
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/package.json
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   136932 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/yarn.lock
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/sketcher.spec.ts
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/tree.spec.ts
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts
--rw-r--r--   0        0        0    22422 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/sketcher.spec.ts-snapshots/Sketcher-Circle-example-2D-FCStd-linux.png
--rw-r--r--   0        0        0    14497 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/sketcher.spec.ts-snapshots/Sketcher-Display-example-2D-FCStd-linux.png
--rw-r--r--   0        0        0     8724 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/tree.spec.ts-snapshots/Tree-Display-example1-FCStd-linux.png
--rw-r--r--   0        0        0   430799 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Operator-Add-example2-FCStd-linux.png
--rw-r--r--   0        0        0   432003 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Operator-Edit-example4-FCStd-linux.png
--rw-r--r--   0        0        0   432717 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Operator-Remove-example3-FCStd-linux.png
--rw-r--r--   0        0        0   431717 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-common-FCStd-linux.png
--rw-r--r--   0        0        0   430783 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-cut-FCStd-linux.png
--rw-r--r--   0        0        0   428851 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-example-2D-FCStd-linux.png
--rw-r--r--   0        0        0   435919 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-example1-FCStd-linux.png
--rw-r--r--   0        0        0   429843 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-example2-FCStd-linux.png
--rw-r--r--   0        0        0   432729 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-example3-FCStd-linux.png
--rw-r--r--   0        0        0   431558 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-example4-FCStd-linux.png
--rw-r--r--   0        0        0   433227 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-example5-FCStd-linux.png
--rw-r--r--   0        0        0   439284 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-example6-FCStd-linux.png
--rw-r--r--   0        0        0   433701 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-test-jcad-linux.png
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/README.md
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 jupytercad-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/.eslintrc.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/.prettierrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/.yarnrc.yml
+-rw-r--r--   0        0        0    13503 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/CHANGELOG.md
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/RELEASE.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/extension.webpack.config.js
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/install.json
+-rw-r--r--   0        0        0   340807 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad-screenshot.png
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/package.json
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/schema.js
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/setup.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/tsconfig.json
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/tsconfig.worker.json
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/worker.webpack.config.js
+-rw-r--r--   0        0        0   277215 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/yarn.lock
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/.github/workflows/binder-on-pr.yml
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/.github/workflows/enforce-labels.yml
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/.github/workflows/update_galata_references.yaml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/binder/environment.yml
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/binder/jupyter_config.json
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/binder/postBuild
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/binder/start
+-rw-r--r--   0        0        0   300736 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/examples/ArchDetail.FCStd
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/examples/common.FCStd
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/examples/cut.FCStd
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/examples/example1.FCStd
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/examples/example2.FCStd
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/examples/example3.FCStd
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/examples/example4.FCStd
+-rw-r--r--   0        0        0    27100 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/examples/example5.FCStd
+-rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/examples/example6.FCStd
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/examples/example_2D.FCStd
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/examples/test.jcad
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/_version.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/fcstd_ydoc.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/jcad_ydoc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/__init__.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/loader.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/base_prop.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/property_angle.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/property_bool.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/property_distance.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/property_geometrylist.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/property_length.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/property_link.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/property_link_list.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/property_map.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/property_partshape.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/property_placement.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/geometry/__init__.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/geometry/geom_circle.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/freecad/props/geometry/geom_linesegment.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/notebook/__init__.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/notebook/cad_document.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/notebook/utils.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/notebook/y_connector.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad/notebook/objects/__init__.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad-opencascade/build.yml
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad-opencascade/build_opencascade.js
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad-opencascade/package.json
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/jupytercad-opencascade/yarn.lock
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/scripts/bump-version.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/factory.ts
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/index.ts
+-rw-r--r--   0        0        0    35332 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/mainview.tsx
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/model.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/svg.d.ts
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/token.ts
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/tools.ts
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/types.ts
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/widget.tsx
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/annotation/message.tsx
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/annotation/model.ts
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/annotation/view.tsx
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/fcplugin/modelfactory.ts
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/fcplugin/plugins.ts
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/jcadplugin/modelfactory.ts
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/jcadplugin/plugins.ts
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/notebookrenderer/index.ts
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/notebookrenderer/model.ts
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/notebookrenderer/token.ts
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/notebookrenderer/view.ts
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/notebookrenderer/widgetManager.ts
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/notebookrenderer/yCommProvider.ts
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/panelview/annotations.tsx
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/panelview/formbuilder.tsx
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/panelview/header.tsx
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/panelview/leftpanel.tsx
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/panelview/model.ts
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/panelview/objectproperties.tsx
+-rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/panelview/objecttree.tsx
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/panelview/rightpanel.tsx
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/box.json
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/cone.json
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/cut.json
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/cylinder.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/extrusion.json
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/fuse.json
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/geomCircle.json
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/geomLineSegment.json
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/intersection.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/jcad.json
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/placement.json
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/sketch.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/sphere.json
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/schema/torus.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/sketcher/helper.tsx
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/sketcher/panzoom.ts
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/sketcher/sketcherdialog.tsx
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/sketcher/sketchermodel.ts
+-rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/sketcher/sketcherwidget.tsx
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/sketcher/types.ts
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/sketcher/elements/circle.ts
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/sketcher/elements/line.ts
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/sketcher/elements/point.ts
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/toolbar/formdialog.tsx
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/toolbar/helpertoolbar.tsx
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/toolbar/model.ts
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/toolbar/operatortoolbar.tsx
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/toolbar/parttoolbar.tsx
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/toolbar/sketchertoolbar.tsx
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/toolbar/toolbar.tsx
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/toolbar/usertoolbar.tsx
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/toolbar/widget.tsx
+-rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/worker/actions.ts
+-rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/worker/occapi.ts
+-rw-r--r--   0        0        0     8601 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/worker/occparser.ts
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/worker/types.ts
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/worker/utils.ts
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/worker/worker.ts
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/worker/geometry/geomCircle.ts
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/src/worker/geometry/geomLineSegment.ts
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/style/index.js
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/style/icon/jvcontrol.svg
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/style/icon/minimize.svg
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/style/icon/visibility.svg
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/style/icon/visibilityOff.svg
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/package.json
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   148487 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/sketcher.spec.ts
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/tree.spec.ts
+-rw-r--r--   0        0        0     7377 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts
+-rw-r--r--   0        0        0    26780 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/sketcher.spec.ts-snapshots/Sketcher-Circle-example-2D-FCStd-linux.png
+-rw-r--r--   0        0        0    17554 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/sketcher.spec.ts-snapshots/Sketcher-Display-example-2D-FCStd-linux.png
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/tree.spec.ts-snapshots/Tree-Display-example1-FCStd-linux.png
+-rw-r--r--   0        0        0   430799 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Operator-Add-example2-FCStd-linux.png
+-rw-r--r--   0        0        0   432003 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Operator-Edit-example4-FCStd-linux.png
+-rw-r--r--   0        0        0   428058 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Operator-Remove-example3-FCStd-linux.png
+-rw-r--r--   0        0        0   428143 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-common-FCStd-linux.png
+-rw-r--r--   0        0        0   430142 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-cut-FCStd-linux.png
+-rw-r--r--   0        0        0   428851 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-example-2D-FCStd-linux.png
+-rw-r--r--   0        0        0   430909 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-example1-FCStd-linux.png
+-rw-r--r--   0        0        0   429843 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-example2-FCStd-linux.png
+-rw-r--r--   0        0        0   431473 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-example3-FCStd-linux.png
+-rw-r--r--   0        0        0   431558 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-example4-FCStd-linux.png
+-rw-r--r--   0        0        0   433227 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-example5-FCStd-linux.png
+-rw-r--r--   0        0        0   439284 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-example6-FCStd-linux.png
+-rw-r--r--   0        0        0   433701 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-test-jcad-linux.png
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/README.md
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 jupytercad-0.1.0a2/PKG-INFO
```

### Comparing `jupytercad-0.1.0a1/.eslintrc.js` & `jupytercad-0.1.0a2/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/CHANGELOG.md` & `jupytercad-0.1.0a2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,33 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.1.0a2
+
+([Full Changelog](https://github.com/QuantStack/jupytercad/compare/v0.1.0a1...2f7b81060a1adab614bb6df1284382b0a1a5a546))
+
+### Enhancements made
+
+- Hide source objects after executing operators [#117](https://github.com/QuantStack/jupytercad/pull/117) ([@trungleduc](https://github.com/trungleduc))
+- Expose JupyterCad 3d view and APIs in notebook [#102](https://github.com/QuantStack/jupytercad/pull/102) ([@trungleduc](https://github.com/trungleduc))
+
+### Maintenance and upkeep improvements
+
+- Update to JupyterLab beta 2 [#130](https://github.com/QuantStack/jupytercad/pull/130) ([@trungleduc](https://github.com/trungleduc))
+- Update to JupyterLab beta 0 [#119](https://github.com/QuantStack/jupytercad/pull/119) ([@martinRenou](https://github.com/martinRenou))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/QuantStack/jupytercad/graphs/contributors?from=2023-03-09&to=2023-04-26&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Agithub-actions+updated%3A2023-03-09..2023-04-26&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3AmartinRenou+updated%3A2023-03-09..2023-04-26&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Atrungleduc+updated%3A2023-03-09..2023-04-26&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.1.0a1
 
 ([Full Changelog](https://github.com/QuantStack/jupytercad/compare/c58c7dd5a0ae9bcc010d24db38dbc9a2d68055c8...f7a0f6ba2b00a1661981ccbdda4166be9182d9fc))
 
 ### Enhancements made
 
 - Exploded view [#109](https://github.com/QuantStack/jupytercad/pull/109) ([@martinRenou](https://github.com/martinRenou))
@@ -99,9 +121,7 @@
 - Add dark background and loading animation [#1](https://github.com/QuantStack/jupytercad/pull/1) ([@trungleduc](https://github.com/trungleduc))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/QuantStack/jupytercad/graphs/contributors?from=2021-11-24&to=2023-03-09&type=c))
 
 [@bollwyvl](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Abollwyvl+updated%3A2021-11-24..2023-03-09&type=Issues) | [@davidbrochart](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Adavidbrochart+updated%3A2021-11-24..2023-03-09&type=Issues) | [@github-actions](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Agithub-actions+updated%3A2021-11-24..2023-03-09&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Ahbcarlos+updated%3A2021-11-24..2023-03-09&type=Issues) | [@jtpio](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Ajtpio+updated%3A2021-11-24..2023-03-09&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3AmartinRenou+updated%3A2021-11-24..2023-03-09&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Atrungleduc+updated%3A2021-11-24..2023-03-09&type=Issues)
-
-<!-- <END NEW CHANGELOG ENTRY> -->
```

### Comparing `jupytercad-0.1.0a1/CONTRIBUTING.md` & `jupytercad-0.1.0a2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/RELEASE.md` & `jupytercad-0.1.0a2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/extension.webpack.config.js` & `jupytercad-0.1.0a2/extension.webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/jupytercad-screenshot.png` & `jupytercad-0.1.0a2/jupytercad-screenshot.png`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/package.json` & `jupytercad-0.1.0a2/package.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9349771960066078%*

 * *Differences: {"'dependencies'": "{'@jupyter/ydoc': '^0.3.4 || ^1.0.2', '@jupyterlab/application': "*

 * *                   "'^4.0.0-beta.2', '@jupyterlab/apputils': '^4.0.0-beta.2', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.0-beta.2', '@jupyterlab/docregistry': "*

 * *                   "'^4.0.0-beta.2', '@jupyterlab/filebrowser': '^4.0.0-beta.2', "*

 * *                   "'@jupyterlab/launcher': '^4.0.0-beta.2', '@jupyterlab/mainmenu': "*

 * *                   "'^4.0.0-beta.2', '@jupyterlab/observables': '^5.0.0-beta.2', "*

 * *  […]*

```diff
@@ -4,71 +4,86 @@
         "name": "Trung Le"
     },
     "bugs": {
         "url": "https://github.com/QuantStack/jupytercad/issues"
     },
     "dependencies": {
         "@deathbeds/jupyterlab-rjsf": "^1.1.0",
-        "@jupyter/ydoc": "~0.2.2",
-        "@jupyterlab/application": "~4.0.0-alpha.17",
-        "@jupyterlab/apputils": "~4.0.0-alpha.17",
-        "@jupyterlab/collaboration": "~4.0.0-alpha.17",
-        "@jupyterlab/coreutils": "~6.0.0-alpha.17",
-        "@jupyterlab/docregistry": "~4.0.0-alpha.17",
-        "@jupyterlab/filebrowser": "~4.0.0-alpha.17",
-        "@jupyterlab/launcher": "~4.0.0-alpha.17",
-        "@jupyterlab/mainmenu": "~4.0.0-alpha.17",
-        "@jupyterlab/observables": "~5.0.0-alpha.17",
-        "@jupyterlab/services": "~7.0.0-alpha.17",
-        "@jupyterlab/translation": "~4.0.0-alpha.17",
-        "@jupyterlab/ui-components": "~4.0.0-alpha.32",
-        "@lumino/commands": "~2.0.0-alpha.6",
-        "@lumino/coreutils": "~2.0.0-alpha.6",
-        "@lumino/signaling": "~2.0.0-alpha.6",
-        "@lumino/widgets": "~2.0.0-alpha.6",
+        "@jupyter-widgets/base": "^6.0.2",
+        "@jupyter/collaboration": "^1.0.0-alpha.7",
+        "@jupyter/docprovider": "^1.0.0-alpha.8",
+        "@jupyter/ydoc": "^0.3.4 || ^1.0.2",
+        "@jupyterlab/application": "^4.0.0-beta.2",
+        "@jupyterlab/apputils": "^4.0.0-beta.2",
+        "@jupyterlab/coreutils": "^6.0.0-beta.2",
+        "@jupyterlab/docregistry": "^4.0.0-beta.2",
+        "@jupyterlab/filebrowser": "^4.0.0-beta.2",
+        "@jupyterlab/launcher": "^4.0.0-beta.2",
+        "@jupyterlab/mainmenu": "^4.0.0-beta.2",
+        "@jupyterlab/notebook": "^4.0.0-beta.2",
+        "@jupyterlab/observables": "^5.0.0-beta.2",
+        "@jupyterlab/services": "^7.0.0-beta.2",
+        "@jupyterlab/translation": "^4.0.0-beta.2",
+        "@jupyterlab/ui-components": "^4.0.0-beta.2",
+        "@lumino/commands": "^2.0.0",
+        "@lumino/coreutils": "^2.0.0",
+        "@lumino/signaling": "^2.0.0",
+        "@lumino/widgets": "^2.0.0",
         "@naisutech/react-tree": "^3.0.1",
         "@rjsf/core": "^4.2.0",
         "@types/d3-color": "^3.1.0",
         "@types/three": "^0.134.0",
         "d3-color": "^3.1.0",
         "jupytercad-opencascade": "^0.1.1-alpha.2",
-        "react": "^17.0.1",
+        "lib0": "^0.2.62",
+        "react": "^18.0.1",
         "styled-components": "^5.3.6",
         "three": "^0.135.0",
         "three-mesh-bvh": "^0.5.17",
         "uuid": "^8.3.2"
     },
     "description": "A JupyterLab extension for 3D modelling.",
     "devDependencies": {
         "@apidevtools/json-schema-ref-parser": "^9.0.9",
-        "@jupyterlab/builder": "~4.0.0-alpha.17",
+        "@jupyterlab/builder": "^4.0.0-beta.2",
         "@types/node": "^16.11.10",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "copy-webpack-plugin": "^10.0.0",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "file-loader": "^6.2.0",
         "json-schema-to-typescript": "^10.1.5",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "source-map-loader": "^3.0.0",
         "ts-loader": "^9.2.6",
-        "typescript": "~4.1.3"
+        "typescript": "~4.1.3",
+        "webpack": "^5.76.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/QuantStack/jupytercad",
     "jupyterlab": {
         "extension": true,
         "outputDir": "jupytercad/labextension",
+        "sharedPackages": {
+            "@jupyter-widgets/base": {
+                "bundled": false,
+                "singleton": true
+            },
+            "yjs": {
+                "bundled": false,
+                "singleton": true
+            }
+        },
         "webpackConfig": "./extension.webpack.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
@@ -79,23 +94,28 @@
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/QuantStack/jupytercad.git"
     },
     "resolutions": {
-        "@jupyterlab/apputils": "~4.0.0-alpha.11"
+        "@jupyterlab/apputils": "~4.0.0-beta.2",
+        "@jupyterlab/notebook": "~4.0.0-beta.2",
+        "@jupyterlab/services": " ^7.0.0-beta.2",
+        "@lumino/coreutils": "^2.0.0"
     },
     "scripts": {
         "build": "jlpm build:schema && jlpm run build:lib && jlpm run build:worker && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run clean && jlpm build:schema && jlpm run build:worker:prod && jlpm run build:lib && jlpm run build:labextension",
-        "build:schema": "json2ts -i src/schema -o src/_interface --no-unknownAny --unreachableDefinitions --cwd ./src/schema && cd src/schema && node ../../schema.js",
+        "build:schema": "jlpm build:schema:js && jlpm build:schema:py",
+        "build:schema:js": "json2ts -i src/schema -o src/_interface --no-unknownAny --unreachableDefinitions --cwd ./src/schema && cd src/schema && node ../../schema.js",
+        "build:schema:py": "datamodel-codegen --input src/schema --output jupytercad/notebook/objects/_schema",
         "build:worker": "webpack --config worker.webpack.config.js --mode=development",
         "build:worker:prod": "webpack --config worker.webpack.config.js --mode=production",
         "clean": "jlpm run clean:lib",
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
         "clean:labextension": "rimraf jupytercad/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "eslint": "eslint . --ext .ts,.tsx --fix",
@@ -114,9 +134,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.0-a1"
+    "version": "0.1.0-a2"
 }
```

### Comparing `jupytercad-0.1.0a1/schema.js` & `jupytercad-0.1.0a2/schema.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/tsconfig.json` & `jupytercad-0.1.0a2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/worker.webpack.config.js` & `jupytercad-0.1.0a2/worker.webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/.github/workflows/build.yml` & `jupytercad-0.1.0a2/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,27 @@
     - name: Checkout
       uses: actions/checkout@v3
 
     # Use mamba instead due to freecad
     #- name: Base Setup
     #  uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
     #- name: Install dependencies
-    #  run: python -m pip install -U jupyterlab>=0.4.0a32
+    #  run: python -m pip install -U jupyterlab>=0.4.0b0
 
     - name: Install Conda environment with Micromamba
       uses: mamba-org/provision-with-micromamba@main
       with:
         environment-name: cad
         environment-file: false
-        channels: conda-forge/label/jupyterlab_alpha,conda-forge
+        channels: conda-forge/label/jupyterlab_beta,conda-forge
         extra-specs: |
           python=3.9
-          nodejs=16
+          nodejs=18
           yarn
-          jupyterlab=4.0.0a32
+          "jupyterlab>=4.0.0b0"
           freecad
 
     - name: Lint the extension
       shell: bash -l {0}
       run: |
         set -eux
         jlpm
@@ -87,20 +87,21 @@
         architecture: 'x64'
 
     - uses: actions/download-artifact@v3
       with:
         name: extension-artifacts
 
     - name: Install and Test
+    # TODO Update JupyterLab version
       run: |
         set -eux
         # Remove NodeJS, twice to take care of system and locally installed node versions.
         sudo rm -rf $(which node)
         sudo rm -rf $(which node)
-        pip install "jupyterlab==4.0.0a32" jupytercad*.whl
+        pip install "jupyterlab>=4.0.0b0" jupytercad*.whl
 
         jupyter labextension list
         jupyter labextension list 2>&1 | grep -ie "jupytercad.*OK"
         # jupyterlab.browser_check will fail due to the core extension jupyterlab_pygments.
         # It does not support lab v4.0.0
         #python -m jupyterlab.browser_check --no-chrome-test
 
@@ -116,27 +117,27 @@
     - name: Checkout
       uses: actions/checkout@v3
 
     # Use mamba instead due to freecad
     #- name: Base Setup
     #  uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
     #- name: Install dependencies
-    #  run: python -m pip install -U jupyterlab>=0.4.0a32
+    #  run: python -m pip install -U jupyterlab>=0.4.0b0
 
     - name: Install Conda environment with Micromamba
       uses: mamba-org/provision-with-micromamba@main
       with:
         environment-name: cad
         environment-file: false
-        channels: conda-forge/label/jupyterlab_alpha,conda-forge
+        channels: conda-forge/label/jupyterlab_beta,conda-forge
         extra-specs: |
           python=3.9
-          nodejs=16
+          nodejs=18
           yarn
-          jupyterlab=4.0.0a32
+          "jupyterlab>=4.0.0b0"
           freecad
 
     - name: Download extension package
       uses: actions/download-artifact@v3
       with:
         name: extension-artifacts
 
@@ -158,22 +159,22 @@
       with:
         path: |
           ${{ github.workspace }}/pw-browsers
         key: ${{ runner.os }}-${{ hashFiles('ui-tests/yarn.lock') }}
 
     - name: Install browser
       shell: bash -l {0}
-      run: jlpm playwright install chromium
+      run: npx playwright install chromium
       working-directory: ui-tests
 
     - name: Execute integration tests
       shell: bash -l {0}
       working-directory: ui-tests
       run: |
-        jlpm playwright test
+        npx playwright test
 
     - name: Upload Playwright Test report
       if: always()
       uses: actions/upload-artifact@v3
       with:
         name: jupytercad-playwright-tests
         path: |
@@ -198,20 +199,20 @@
       uses: actions/checkout@v3
 
     - name: Install Conda environment with Micromamba
       uses: mamba-org/provision-with-micromamba@main
       with:
         environment-name: cad
         environment-file: false
-        channels: conda-forge/label/jupyterlab_alpha,conda-forge
+        channels: conda-forge/label/jupyterlab_beta,conda-forge
         extra-specs: |
           python=3.9
-          nodejs=16
+          nodejs=18
           yarn
-          jupyterlab=4.0.0a32
+          "jupyterlab>=4.0.0b0"
           freecad
 
     - name: Setup pip cache
       uses: actions/cache@v2
       with:
         path: ~/.cache/pip
         key: pip-3.9-${{ hashFiles('package.json') }}
@@ -243,15 +244,14 @@
         key: ${{ hashFiles('jupytercad-opencascade/build.yml') }}
 
     - name: Build jupytercad-opencascade
       shell: bash -l {0}
       run: |
         jlpm
         jlpm run build
-        jlpm link
       working-directory: jupytercad-opencascade
 
     - name: Build the extension
       shell: bash -l {0}
       run: |
         jlpm link jupytercad-opencascade
```

### Comparing `jupytercad-0.1.0a1/.github/workflows/check-release.yml` & `jupytercad-0.1.0a2/.github/workflows/check-release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 jobs:
   check_release:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         group: [check_release]
         python-version: ["3.9"]
-        node-version: ["14.x"]
+        node-version: ["18.x"]
 
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
       - name: Base Setup
         uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
```

### Comparing `jupytercad-0.1.0a1/.github/workflows/update_galata_references.yaml` & `jupytercad-0.1.0a2/.github/workflows/update_galata_references.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         run: mamba install -q python=3.9 pip freecad
 
       - name: Install the extension
         shell: bash -l {0}
         run: |
           whereis python
           python -m pip install jupytercad*.whl
-          python -m pip install "jupyterlab>=4.0.0a32"
+          python -m pip install "jupyterlab>=4.0.0b0"
 
       - name: Install dependencies
         shell: bash -l {0}
         working-directory: ui-tests
         env:
           PLAYWRIGHT_SKIP_BROWSER_DOWNLOAD: 1
         run: jlpm install
```

### Comparing `jupytercad-0.1.0a1/binder/postBuild` & `jupytercad-0.1.0a2/binder/postBuild`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/examples/ArchDetail.FCStd` & `jupytercad-0.1.0a2/examples/ArchDetail.FCStd`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/examples/common.FCStd` & `jupytercad-0.1.0a2/examples/common.FCStd`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/examples/cut.FCStd` & `jupytercad-0.1.0a2/examples/cut.FCStd`

 * *Files 22% similar despite different names*

#### zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 4862 bytes, number of entries: 4
--rw-rw-r--  2.0 unx    12133 b- defN 22-Sep-16 17:28 Document.xml
--rw-rw-r--  2.0 unx     8938 b- defN 22-Sep-16 17:28 PartShape.brp
--rw-rw-r--  2.0 unx     4706 b- defN 22-Sep-16 17:28 PartShape1.brp
--rw-rw-r--  2.0 unx    12729 b- defN 22-Sep-16 17:28 PartShape2.brp
-4 files, 38506 bytes uncompressed, 4414 bytes compressed:  88.5%
+Zip file size: 4869 bytes, number of entries: 4
+-rw-rw-r--  2.0 unx    12133 b- defN 23-Jan-17 19:47 Document.xml
+-rw-rw-r--  2.0 unx     8938 b- defN 23-Jan-17 19:47 PartShape.brp
+-rw-rw-r--  2.0 unx     4706 b- defN 23-Jan-17 19:47 PartShape1.brp
+-rw-rw-r--  2.0 unx    12729 b- defN 23-Jan-17 19:47 PartShape2.brp
+4 files, 38506 bytes uncompressed, 4421 bytes compressed:  88.5%
```

#### Document.xml

##### Document.xml

```diff
@@ -19,21 +19,21 @@
     <Property name="CreationDate" type="App::PropertyString" status="16777217">
       <String value="2022-09-16T12:16:29Z"/>
     </Property>
     <Property name="Id" type="App::PropertyString">
       <String value=""/>
     </Property>
     <Property name="Label" type="App::PropertyString" status="1">
-      <String value="tmpsc7tok3n"/>
+      <String value="tmpxcotq79d"/>
     </Property>
     <Property name="LastModifiedBy" type="App::PropertyString">
       <String value=""/>
     </Property>
     <Property name="LastModifiedDate" type="App::PropertyString" status="16777217">
-      <String value="2022-09-16T15:28:55Z"/>
+      <String value="2023-01-17T18:47:40Z"/>
     </Property>
     <Property name="License" type="App::PropertyString" status="1">
       <String value="All rights reserved"/>
     </Property>
     <Property name="LicenseURL" type="App::PropertyString" status="1">
       <String value="http://en.wikipedia.org/wiki/All_rights_reserved"/>
     </Property>
```

### Comparing `jupytercad-0.1.0a1/examples/example1.FCStd` & `jupytercad-0.1.0a2/examples/example1.FCStd`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/examples/example2.FCStd` & `jupytercad-0.1.0a2/examples/example2.FCStd`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/examples/example3.FCStd` & `jupytercad-0.1.0a2/examples/example3.FCStd`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/examples/example4.FCStd` & `jupytercad-0.1.0a2/examples/example4.FCStd`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/examples/example5.FCStd` & `jupytercad-0.1.0a2/examples/example5.FCStd`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/examples/example6.FCStd` & `jupytercad-0.1.0a2/examples/example6.FCStd`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/examples/example_2D.FCStd` & `jupytercad-0.1.0a2/examples/example_2D.FCStd`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/examples/test.jcad` & `jupytercad-0.1.0a2/examples/test.jcad`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/jupytercad/fcstd_ydoc.py` & `jupytercad-0.1.0a2/jupytercad/jcad_ydoc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,61 @@
-from jupyter_ydoc.ydoc import YBaseDoc
-import y_py as Y
+import json
+from typing import Any, Callable
+from functools import partial
 
-from jupytercad.freecad.loader import FCStd
+import y_py as Y
+from jupyter_ydoc.ybasedoc import YBaseDoc
 
 
-class YFCStd(YBaseDoc):
+class YJCad(YBaseDoc):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._ysource = self._ydoc.get_text('source')
         self._yobjects = self._ydoc.get_array('objects')
         self._yoptions = self._ydoc.get_map('options')
         self._ymeta = self._ydoc.get_map('metadata')
-        self._virtual_file = FCStd()
-
-    @property
-    def source(self):
-        fc_objects = self._yobjects.to_json()
-        options = self._yoptions.to_json()
-        meta = self._ymeta.to_json()
-        self._virtual_file.save(fc_objects, options, meta)
-        return self._virtual_file.sources
-
-    @source.setter
-    def source(self, value):
-        virtual_file = self._virtual_file
-        virtual_file.load(value)
-        objects = []
-
-        for obj in virtual_file.objects:
-            objects.append(Y.YMap(obj))
-
+    
+    def version(self) -> str:
+        return '0.1.0'
+    
+    def get(self) -> str:
+        """
+        Returns the content of the document.
+        :return: Document's content.
+        :rtype: Any
+        """
+        objects = json.loads(self._yobjects.to_json()) 
+        options = json.loads(self._yoptions.to_json())
+        meta = json.loads(self._ymeta.to_json())
+        return json.dumps(
+            dict(objects=objects, options=options, metadata=meta), indent=2
+        )
+
+    def set(self, value: str) -> None:
+        """
+        Sets the content of the document.
+        :param value: The content of the document.
+        :type value: Any
+        """
+        valueDict = json.loads(value)
+        newObj = []
+        for obj in valueDict['objects']:
+            newObj.append(Y.YMap(obj))
         with self._ydoc.begin_transaction() as t:
             length = len(self._yobjects)
             self._yobjects.delete_range(t, 0, length)
-            self._yobjects.extend(t, objects)
-
-            self._yoptions.update(t, virtual_file.options.items())
-            self._ymeta.update(t, virtual_file.metadata.items())
+            # workaround for https://github.com/y-crdt/ypy/issues/126:
+            #self._yobjects.extend(t, newObj) 
+            for o in newObj:
+                self._yobjects.append(t, o)
+            self._yoptions.update(t, valueDict['options'].items())
+            self._ymeta.update(t, valueDict['metadata'].items())
 
-    def observe(self, callback):
+    def observe(self, callback: Callable[[str, Any], None]):
         self.unobserve()
-        self._subscriptions[self._ystate] = self._ystate.observe(callback)
-        self._subscriptions[self._ysource] = self._ysource.observe(callback)
-        self._subscriptions[self._yobjects] = self._yobjects.observe_deep(callback)
-        self._subscriptions[self._yoptions] = self._yoptions.observe(callback)
-        self._subscriptions[self._ymeta] = self._ymeta.observe_deep(callback)
+        self._subscriptions[self._ystate] = self._ystate.observe(partial(callback, "state"))
+        self._subscriptions[self._ysource] = self._ysource.observe(partial(callback, "source"))
+        self._subscriptions[self._yobjects] = self._yobjects.observe_deep(
+            partial(callback, "objects")
+        )
+        self._subscriptions[self._yoptions] = self._yoptions.observe(partial(callback, "options"))
+        self._subscriptions[self._ymeta] = self._ymeta.observe(partial(callback, "meta"))
```

### Comparing `jupytercad-0.1.0a1/jupytercad/freecad/loader.py` & `jupytercad-0.1.0a2/jupytercad/freecad/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,47 @@
-import traceback
-from typing import Dict, List, Type
-import tempfile
 import base64
-from pathlib import Path
+import json
+import logging
 import os
-import xml
-import zipfile
+import tempfile
+import traceback
+from typing import Dict, List, Type
 
-from .props.base_prop import BaseProp
 from . import props as Props
-import logging
+from .props.base_prop import BaseProp
 
 logger = logging.getLogger(__file__)
 
 try:
     import freecad as fc
-
     import OfflineRenderingUtils
 
 except ImportError:
-    logger.warn("[JupyterCad] Freecad is not installed!")
+    logger.warn('[JupyterCad] Freecad is not installed!')
     fc = None
 
 
 def _guidata_to_options(guidata):
     """Converts freecad guidata into options that JupyterCad understands"""
     options = {}
 
     for obj_name, data in guidata.items():
         obj_options = {}
 
         # We need to make a special case to "GuiCameraSettings" because freecad's
         # OfflineRenderingUtils mixes the camera settings with 3D objects
-        if obj_name == "GuiCameraSettings":
+        if obj_name == 'GuiCameraSettings':
             options[obj_name] = data
             continue
 
-        if "ShapeColor" in data:
-            obj_options["color"] = list(data["ShapeColor"]["value"])
+        if 'ShapeColor' in data:
+            obj_options['color'] = list(data['ShapeColor']['value'])
 
-        if "Visibility" in data:
-            obj_options["visibility"] = data["Visibility"]["value"]
+        if 'Visibility' in data:
+            obj_options['visibility'] = data['Visibility']['value']
 
         options[obj_name] = obj_options
 
     return options
 
 
 def _options_to_guidata(options):
@@ -52,36 +49,36 @@
     gui_data = {}
 
     for obj_name, data in options.items():
         obj_data = {}
 
         # We need to make a special case to "GuiCameraSettings" because freecad's
         # OfflineRenderingUtils mixes the camera settings with 3D objects
-        if obj_name == "GuiCameraSettings":
+        if obj_name == 'GuiCameraSettings':
             options[obj_name] = data
             continue
 
-        if "color" in data:
-            obj_data["ShapeColor"] = dict(
-                type="App::PropertyColor", value=tuple(data["color"])
+        if 'color' in data:
+            obj_data['ShapeColor'] = dict(
+                type='App::PropertyColor', value=tuple(data['color'])
             )
 
-        if "visibility" in data:
-            obj_data["Visibility"] = dict(
-                type="App::PropertyBool", value=data["visibility"]
+        if 'visibility' in data:
+            obj_data['Visibility'] = dict(
+                type='App::PropertyBool', value=data['visibility']
             )
 
         gui_data[obj_name] = obj_data
 
     return gui_data
 
 
 class FCStd:
     def __init__(self) -> None:
-        self._sources = ""
+        self._sources = ''
         self._objects = []
         self._options = {}
         self._metadata = {}
         self._id = None
         self._visible = True
         self._prop_handlers: Dict[str, Type[BaseProp]] = {}
         for Cls in Props.__dict__.values():
@@ -104,60 +101,64 @@
     def options(self):
         return self._options
 
     def load(self, base64_content: str) -> None:
         if not fc:
             return
         self._sources = base64_content
-        with tempfile.NamedTemporaryFile(delete=False, suffix=".FCStd") as tmp:
+        with tempfile.NamedTemporaryFile(delete=False, suffix='.FCStd') as tmp:
             file_content = base64.b64decode(base64_content)
             tmp.write(file_content)
 
         fc_file = fc.app.openDocument(tmp.name)
 
         # Get metadata
         self._metadata = fc_file.Meta
 
         # Get GuiData (metadata from the GuiDocument.xml file)
-        self._options["guidata"] = _guidata_to_options(
+        self._options['guidata'] = _guidata_to_options(
             OfflineRenderingUtils.getGuiData(tmp.name)
         )
 
         # Get objects
+        self._objects = []
         for obj in fc_file.Objects:
             self._objects.append(self._fc_to_jcad_obj(obj))
 
         os.remove(tmp.name)
 
     def save(self, objects: List, options: Dict, metadata: Dict) -> None:
         try:
             if not fc or len(self._sources) == 0:
                 return
 
-            with tempfile.NamedTemporaryFile(delete=False, suffix=".FCStd") as tmp:
+            with tempfile.NamedTemporaryFile(
+                delete=False, suffix='.FCStd'
+            ) as tmp:
                 file_content = base64.b64decode(self._sources)
                 tmp.write(file_content)
             fc_file = fc.app.openDocument(tmp.name)
             fc_file.Meta = metadata
+            new_objs = dict([(o['name'], o) for o in objects])
 
-            new_objs = dict([(o["name"], o) for o in objects])
             current_objs = dict([(o.Name, o) for o in fc_file.Objects])
+
             to_remove = [x for x in current_objs if x not in new_objs]
             to_add = [x for x in new_objs if x not in current_objs]
             for obj_name in to_remove:
                 fc_file.removeObject(obj_name)
             for obj_name in to_add:
                 py_obj = new_objs[obj_name]
-                fc_file.addObject(py_obj["shape"], py_obj["name"])
+                fc_file.addObject(py_obj['shape'], py_obj['name'])
             to_update = [x for x in new_objs if x in current_objs] + to_add
 
             for obj_name in to_update:
                 py_obj = new_objs[obj_name]
 
-                fc_obj = fc_file.getObject(py_obj["name"])
+                fc_obj = fc_file.getObject(py_obj['name'])
 
                 for prop, jcad_prop_value in py_obj['parameters'].items():
                     prop_type = fc_obj.getTypeIdOfProperty(prop)
                     prop_handler = self._prop_handlers.get(prop_type, None)
                     if prop_handler is not None:
                         fc_value = prop_handler.jcad_to_fc(
                             jcad_prop_value,
@@ -170,19 +171,19 @@
                             try:
                                 setattr(fc_obj, prop, fc_value)
                             except:
                                 pass
 
             OfflineRenderingUtils.save(
                 fc_file,
-                guidata=_options_to_guidata(options.get("guidata", {})),
+                guidata=_options_to_guidata(options.get('guidata', {})),
             )
 
             fc_file.recompute()
-            with open(tmp.name, "rb") as f:
+            with open(tmp.name, 'rb') as f:
                 encoded = base64.b64encode(f.read())
                 self._sources = encoded.decode()
             os.remove(tmp.name)
         except Exception:
             print(traceback.print_exc())
 
     def _fc_to_jcad_obj(self, obj) -> Dict:
@@ -196,9 +197,9 @@
             prop_type = obj.getTypeIdOfProperty(prop)
             prop_value = getattr(obj, prop)
             prop_handler = self._prop_handlers.get(prop_type, None)
             if prop_handler is not None and prop_value is not None:
                 value = prop_handler.fc_to_jcad(prop_value, fc_object=obj)
             else:
                 value = None
-            obj_data["parameters"][prop] = value
+            obj_data['parameters'][prop] = value
         return obj_data
```

### Comparing `jupytercad-0.1.0a1/jupytercad/freecad/props/base_prop.py` & `jupytercad-0.1.0a2/jupytercad/freecad/props/base_prop.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Any, Dict
+from typing import Any
 
 
 class BaseProp(ABC):
     @staticmethod
     @abstractmethod
     def name() -> str:
         pass
```

### Comparing `jupytercad-0.1.0a1/jupytercad/freecad/props/property_geometrylist.py` & `jupytercad-0.1.0a2/jupytercad/freecad/props/property_geometrylist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, List
-from .geometry import geom_handlers
+
 from .base_prop import BaseProp
+from .geometry import geom_handlers
 
 
 class Part_PropertyGeometryList(BaseProp):
     @staticmethod
     def name() -> str:
         return 'Part::PropertyGeometryList'
```

### Comparing `jupytercad-0.1.0a1/jupytercad/freecad/props/property_partshape.py` & `jupytercad-0.1.0a2/jupytercad/freecad/props/property_partshape.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Any
 from io import StringIO
+from typing import Any
+
 from .base_prop import BaseProp
 
 
 class Part_PropertyPartShape(BaseProp):
     @staticmethod
     def name() -> str:
         return 'Part::PropertyPartShape'
```

### Comparing `jupytercad-0.1.0a1/jupytercad/freecad/props/property_placement.py` & `jupytercad-0.1.0a2/jupytercad/freecad/props/property_placement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import math
 from typing import Any
+
 from .base_prop import BaseProp
 
 try:
     import freecad as fc
 except ImportError:
     fc = None
```

### Comparing `jupytercad-0.1.0a1/jupytercad/freecad/props/geometry/geom_circle.py` & `jupytercad-0.1.0a2/jupytercad/freecad/props/geometry/geom_circle.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/jupytercad/freecad/props/geometry/geom_linesegment.py` & `jupytercad-0.1.0a2/jupytercad/freecad/props/geometry/geom_linesegment.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/jupytercad-opencascade/build.yml` & `jupytercad-0.1.0a2/jupytercad-opencascade/build.yml`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/jupytercad-opencascade/build_opencascade.js` & `jupytercad-0.1.0a2/jupytercad-opencascade/build_opencascade.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/jupytercad-opencascade/package.json` & `jupytercad-0.1.0a2/jupytercad-opencascade/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {'delete': "['dependencies']"}*

```diff
@@ -1,13 +1,12 @@
 {
     "author": "QuantStack",
     "bugs": {
         "url": "https://github.com/QuantStack/jupytercad/issues"
     },
-    "dependencies": {},
     "description": "The custom OpenCascade build for JupyterCAD.",
     "devDependencies": {
         "js-yaml": "^4.1.0",
         "rimraf": "^3.0.2"
     },
     "files": [
         "lib/jupytercad.opencascade.js",
```

### Comparing `jupytercad-0.1.0a1/scripts/bump-version.py` & `jupytercad-0.1.0a2/scripts/bump-version.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/factory.ts` & `jupytercad-0.1.0a2/src/factory.ts`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,16 @@
    *
    * @param context Contains the information of the file
    * @returns The widget
    */
   protected createNewWidget(
     context: DocumentRegistry.IContext<JupyterCadModel>
   ): JupyterCadWidget {
-    const content = new JupyterCadPanel(context);
+    const { model } = context;
+    const content = new JupyterCadPanel({ model });
     const toolbarModel = new ToolbarModel({ panel: content, context });
     const toolbar = new ToolbarWidget({
       model: toolbarModel,
       commands: this._commands
     });
     return new JupyterCadWidget({ context, content, toolbar });
   }
```

### Comparing `jupytercad-0.1.0a1/src/index.ts` & `jupytercad-0.1.0a2/src/index.ts`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
   IAnnotation
 } from './token';
 import { jcLightIcon } from './tools';
 import { IAnnotationModel } from './types';
 import { JupyterCadWidget } from './widget';
 import { ToolbarWidget } from './toolbar/widget';
 import { AnnotationModel } from './annotation/model';
+import { notebookRendererPlugin, ypyWidgetManager } from './notebookrenderer';
 
 const NAME_SPACE = 'jupytercad';
 
 const plugin: JupyterFrontEndPlugin<IJupyterCadTracker> = {
   id: 'jupytercad:plugin',
   autoStart: true,
   requires: [IMainMenu, ITranslator],
@@ -71,15 +72,14 @@
     const annotationModel = new AnnotationModel({
       context: tracker.currentWidget?.context
     });
 
     tracker.currentChanged.connect((_, changed) => {
       annotationModel.context = changed?.context || undefined;
     });
-
     return annotationModel;
   }
 };
 
 const controlPanel: JupyterFrontEndPlugin<void> = {
   id: 'jupytercad:controlpanel',
   autoStart: true,
@@ -111,16 +111,14 @@
       restorer.add(rightControlPanel, NAME_SPACE);
     }
     app.shell.add(leftControlPanel, 'left', { rank: 2000 });
     app.shell.add(rightControlPanel, 'right', { rank: 2000 });
   }
 };
 
-export default [plugin, controlPanel, fcplugin, jcadPlugin, annotationPlugin];
-
 /**
  * Add the FreeCAD commands to the application's command registry.
  */
 function addCommands(
   app: JupyterFrontEnd,
   tracker: WidgetTracker<JupyterCadWidget>,
   translator: ITranslator
@@ -161,7 +159,17 @@
     isEnabled
   });
   mainMenu.editMenu.undoers.undo.add({
     id: ToolbarWidget.CommandIDs.undo,
     isEnabled
   });
 }
+
+export default [
+  plugin,
+  controlPanel,
+  fcplugin,
+  jcadPlugin,
+  annotationPlugin,
+  notebookRendererPlugin,
+  ypyWidgetManager
+];
```

### Comparing `jupytercad-0.1.0a1/src/mainview.tsx` & `jupytercad-0.1.0a2/src/mainview.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-import { DocumentRegistry } from '@jupyterlab/docregistry';
+import { MapChange } from '@jupyter/ydoc';
 import { IObservableMap, ObservableMap } from '@jupyterlab/observables';
 import { User } from '@jupyterlab/services';
-
-import { MapChange } from '@jupyter/ydoc';
-
+import { CommandRegistry } from '@lumino/commands';
 import { JSONValue } from '@lumino/coreutils';
 import { ContextMenu } from '@lumino/widgets';
-import { CommandRegistry } from '@lumino/commands';
-
-import * as React from 'react';
 import * as Color from 'd3-color';
+import * as React from 'react';
 import * as THREE from 'three';
-import { OrbitControls } from 'three/examples/jsm/controls/OrbitControls';
-
 import {
+  acceleratedRaycast,
   computeBoundsTree,
-  disposeBoundsTree,
-  acceleratedRaycast
+  disposeBoundsTree
 } from 'three-mesh-bvh';
-
+import { OrbitControls } from 'three/examples/jsm/controls/OrbitControls';
 import { v4 as uuid } from 'uuid';
 
 import {
   AxeHelper,
   ExplodedView,
   IAnnotation,
   IDict,
@@ -54,15 +48,15 @@
 export type BasicMesh = THREE.Mesh<
   THREE.BufferGeometry,
   THREE.MeshBasicMaterial
 >;
 
 interface IProps {
   view: ObservableMap<JSONValue>;
-  context: DocumentRegistry.IContext<IJupyterCadModel>;
+  jcadModel: IJupyterCadModel;
 }
 
 interface IStates {
   id: string; // ID of the component, it is used to identify which component
   //is the source of awareness updates.
   loading: boolean;
   lightTheme: boolean;
@@ -104,48 +98,46 @@
       id: uuid(),
       lightTheme,
       loading: true,
       annotations: {},
       firstLoad: true
     };
 
-    this._pointer = new THREE.Vector2();
+    this._model = this.props.jcadModel;
+    this._worker = this._model.getWorker();
 
-    this._context = props.context;
+    this._pointer = new THREE.Vector2();
     this._collaboratorPointers = {};
-    this._context.ready.then(() => {
-      this._model = this._context.model;
-      this._worker = this._model.getWorker();
-      this._messageChannel = new MessageChannel();
-      this._messageChannel.port1.onmessage = msgEvent => {
-        this.messageHandler(msgEvent.data);
-      };
-      this._postMessage(
-        { action: WorkerAction.REGISTER, payload: { id: this.state.id } },
-        this._messageChannel.port2
-      );
-      this._model.themeChanged.connect(this._handleThemeChange, this);
+    this._messageChannel = new MessageChannel();
+    this._messageChannel.port1.onmessage = msgEvent => {
+      this.messageHandler(msgEvent.data);
+    };
+    this._postMessage(
+      { action: WorkerAction.REGISTER, payload: { id: this.state.id } },
+      this._messageChannel.port2
+    );
+    this._model.themeChanged.connect(this._handleThemeChange, this);
+
+    this._model.sharedObjectsChanged.connect(
+      this._onSharedObjectsChanged,
+      this
+    );
+    this._model.sharedOptionsChanged.connect(
+      this._onSharedOptionsChanged,
+      this
+    );
+    this._model.clientStateChanged.connect(
+      this._onClientSharedStateChanged,
+      this
+    );
+    this._model.sharedMetadataChanged.connect(
+      this._onSharedMetadataChanged,
+      this
+    );
 
-      this._model.sharedObjectsChanged.connect(
-        this._onSharedObjectsChanged,
-        this
-      );
-      this._model.sharedOptionsChanged.connect(
-        this._onSharedOptionsChanged,
-        this
-      );
-      this._model.clientStateChanged.connect(
-        this._onClientSharedStateChanged,
-        this
-      );
-      this._model.sharedMetadataChanged.connect(
-        this._onSharedMetadataChanged,
-        this
-      );
-    });
     if (this._raycaster.params.Line) {
       this._raycaster.params.Line.threshold = 0.1;
     }
   }
 
   componentDidMount(): void {
     window.addEventListener('resize', this._handleWindowResize);
@@ -158,20 +150,15 @@
   }
 
   componentWillUnmount(): void {
     window.cancelAnimationFrame(this._requestID);
     window.removeEventListener('resize', this._handleWindowResize);
     this.props.view.changed.disconnect(this._onViewChanged, this);
     this._controls.dispose();
-    this._postMessage({
-      action: WorkerAction.CLOSE_FILE,
-      payload: {
-        fileName: this._context.path
-      }
-    });
+
     this._model.themeChanged.disconnect(this._handleThemeChange, this);
     this._model.sharedOptionsChanged.disconnect(
       this._onSharedOptionsChanged,
       this
     );
     this._model.sharedObjectsChanged.disconnect(
       this._onSharedObjectsChanged,
@@ -206,15 +193,15 @@
           );
 
           position.add(
             explodedState.vector.multiplyScalar(-explodedState.distance)
           );
         }
 
-        this._model.annotationModel.addAnnotation(uuid(), {
+        this._model.annotationModel?.addAnnotation(uuid(), {
           position: [position.x, position.y, position.z],
           label: 'New annotation',
           contents: [],
           parent: this._pointer3D.parent.name
         });
       },
       label: 'Add annotation',
@@ -397,15 +384,14 @@
       case MainAction.INITIALIZED: {
         if (!this._model) {
           return;
         }
         this._postMessage({
           action: WorkerAction.LOAD_FILE,
           payload: {
-            fileName: this._context.path,
             content: this._model.getContent()
           }
         });
       }
     }
   };
 
@@ -428,15 +414,15 @@
     Object.keys(this.state.annotations).forEach(key => {
       const el = document.getElementById(key);
       if (el) {
         if (
           options.updatePosition &&
           (el.style.opacity !== '0' || options.updateDisplay !== undefined)
         ) {
-          const annotation = this._model.annotationModel.getAnnotation(key);
+          const annotation = this._model.annotationModel?.getAnnotation(key);
           let screenPosition = new THREE.Vector2();
 
           if (annotation) {
             const parent = this._meshGroup?.getObjectByName(
               annotation.parent
             ) as BasicMesh;
             const position = new THREE.Vector3(
@@ -567,15 +553,15 @@
 
     const guidata = this._model.sharedModel.getOption('guidata');
 
     this._boundingGroup = new THREE.Box3();
 
     this._meshGroup = new THREE.Group();
     Object.entries(payload).forEach(([objName, data]) => {
-      const { faceList, edgeList } = data;
+      const { faceList, edgeList, jcObject } = data;
 
       const vertices: Array<any> = [];
       const normals: Array<any> = [];
       const triangles: Array<any> = [];
 
       let vInd = 0;
       if (faceList.length === 0 && edgeList.length === 0) {
@@ -594,26 +580,26 @@
             face.triIndexes[i + 2] + vInd
           );
         }
 
         vInd += face.vertexCoord.length / 3;
       });
 
-      const objdata = guidata ? guidata[objName] : null;
+      const objdata = guidata ? guidata?.[objName] : null;
 
       let color = DEFAULT_MESH_COLOR;
       let visible = true;
       if (objdata) {
         if (Object.prototype.hasOwnProperty.call(objdata, 'color')) {
           const rgba = objdata['color'] as number[];
           color = new THREE.Color(rgba[0], rgba[1], rgba[2]);
         }
-        if (Object.prototype.hasOwnProperty.call(objdata, 'visibility')) {
-          visible = objdata['visibility'];
-        }
+        visible = guidata![objName]['visibility'] = jcObject.visible;
+      } else if (guidata) {
+        guidata[objName] = { visibility: jcObject.visible };
       }
 
       // Compile the connected vertices and faces into a model
       // And add to the scene
       // We need one material per-mesh because we will set the uniform color independently later
       // it's too bad Three.js does not easily allow setting uniforms independently per-mesh
       const material = new THREE.MeshPhongMaterial({
@@ -669,15 +655,17 @@
 
         mesh.add(edgesMesh);
       });
       if (this._meshGroup) {
         this._meshGroup.add(mesh);
       }
     });
-
+    if (guidata) {
+      this._model.sharedModel?.setOption('guidata', guidata);
+    }
     // Update the reflength
     if (this._refLength === null && this._meshGroup.children.length) {
       const boxSizeVec = new THREE.Vector3();
       this._boundingGroup.getSize(boxSizeVec);
 
       this._refLength =
         Math.max(boxSizeVec.x, boxSizeVec.y, boxSizeVec.z) / 5 || 1;
@@ -937,15 +925,14 @@
     _: IJupyterCadDoc,
     change: IJcadObjectDocChange
   ): void {
     if (change.objectChange) {
       this._postMessage({
         action: WorkerAction.LOAD_FILE,
         payload: {
-          fileName: this._context.path,
           content: this._model.getContent()
         }
       });
     }
   }
 
   private _onSharedOptionsChanged(
@@ -1111,14 +1098,17 @@
               background: this.state.remoteUser.color
             }}
           >
             {`Following ${this.state.remoteUser.display_name}`}
           </div>
         ) : null}
         {Object.entries(this.state.annotations).map(([key, annotation]) => {
+          if (!this._model.annotationModel) {
+            return null;
+          }
           const parent = this._meshGroup?.getObjectByName(
             annotation.parent
           ) as BasicMesh;
           const position = new THREE.Vector3(
             annotation.position[0],
             annotation.position[1],
             annotation.position[2]
@@ -1166,15 +1156,14 @@
         />
       </div>
     );
   }
 
   private divRef = React.createRef<HTMLDivElement>(); // Reference of render div
 
-  private _context: DocumentRegistry.IContext<IJupyterCadModel>;
   private _model: IJupyterCadModel;
   private _worker?: Worker = undefined;
   private _messageChannel?: MessageChannel;
 
   private _pointer: THREE.Vector2;
   private _syncPointer: (
     position: THREE.Vector3 | undefined,
```

### Comparing `jupytercad-0.1.0a1/src/model.ts` & `jupytercad-0.1.0a2/src/model.ts`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,34 @@
   IJcadObjectDocChange,
   IJupyterCadClientState,
   IJupyterCadDoc,
   IJupyterCadDocChange,
   IJupyterCadModel,
   Pointer
 } from './types';
+import { DocumentRegistry } from '@jupyterlab/docregistry';
 
 export class JupyterCadModel implements IJupyterCadModel {
-  constructor(annotationModel: IAnnotationModel, languagePreference?: string) {
+  constructor(options: JupyterCadModel.IOptions) {
+    const { annotationModel, sharedModel } = options;
+    if (sharedModel) {
+      this._sharedModel = sharedModel;
+    } else {
+      this._sharedModel = JupyterCadDoc.create();
+    }
     this.sharedModel.awareness.on('change', this._onClientStateChanged);
     this.annotationModel = annotationModel;
   }
 
   readonly collaborative = true;
 
+  get sharedModel(): IJupyterCadDoc {
+    return this._sharedModel;
+  }
+
   get isDisposed(): boolean {
     return this._isDisposed;
   }
 
   get contentChanged(): ISignal<this, void> {
     return this._contentChanged;
   }
@@ -81,19 +92,25 @@
     return this.sharedModel.optionsChanged;
   }
 
   get sharedObjectsChanged(): ISignal<IJupyterCadDoc, IJcadObjectDocChange> {
     return this.sharedModel.objectsChanged;
   }
 
+  get disposed(): ISignal<JupyterCadModel, void> {
+    return this._disposed;
+  }
+
   dispose(): void {
     if (this._isDisposed) {
       return;
     }
     this._isDisposed = true;
+    this._sharedModel.dispose();
+    this._disposed.emit();
     Signal.clearData(this);
   }
 
   toString(): string {
     return JSON.stringify(this.getContent(), null, 2);
   }
 
@@ -193,53 +210,60 @@
     >;
 
     this._clientStateChanged.emit(clients);
   };
 
   readonly defaultKernelName: string = '';
   readonly defaultKernelLanguage: string = '';
-  readonly sharedModel = JupyterCadDoc.create();
-  readonly annotationModel: IAnnotationModel;
+  readonly annotationModel?: IAnnotationModel;
+
+  private _sharedModel: IJupyterCadDoc;
 
   private _dirty = false;
   private _readOnly = false;
   private _isDisposed = false;
 
+  private _disposed = new Signal<this, void>(this);
   private _contentChanged = new Signal<this, void>(this);
   private _stateChanged = new Signal<this, IChangedArgs<any>>(this);
   private _themeChanged = new Signal<this, IChangedArgs<any>>(this);
   private _clientStateChanged = new Signal<
     this,
     Map<number, IJupyterCadClientState>
   >(this);
+
   static worker: Worker;
 }
 
 export class JupyterCadDoc
   extends YDocument<IJupyterCadDocChange>
   implements IJupyterCadDoc
 {
   constructor() {
     super();
 
     this._options = this.ydoc.getMap<Y.Map<any>>('options');
     this._objects = this.ydoc.getArray<Y.Map<any>>('objects');
     this._metadata = this.ydoc.getMap<string>('metadata');
-
     this.undoManager.addToScope(this._objects);
 
     this._objects.observeDeep(this._objectsObserver);
     this._metadata.observe(this._metaObserver);
     this._options.observe(this._optionsObserver);
   }
 
   dispose(): void {
     this._objects.unobserveDeep(this._objectsObserver);
     this._metadata.unobserve(this._metaObserver);
     this._options.unobserve(this._optionsObserver);
+    super.dispose();
+  }
+
+  get version(): string {
+    return '0.1.0';
   }
 
   get objects(): Array<IJCadObject> {
     return this._objects.map(
       obj => JSONExt.deepCopy(obj.toJSON()) as IJCadObject
     );
   }
@@ -309,15 +333,14 @@
   }
 
   updateObjectByName(name: string, key: string, value: any): void {
     const obj = this._getObjectAsYMapByName(name);
     if (!obj) {
       return;
     }
-
     this.transact(() => obj.set(key, value));
   }
 
   getOption(key: keyof IJCadOptions): IDict | undefined {
     const content = this._options.get(key);
     if (!content) {
       return;
@@ -399,7 +422,14 @@
   private _metadata: Y.Map<string>;
   private _metadataChanged = new Signal<IJupyterCadDoc, MapChange>(this);
   private _optionsChanged = new Signal<IJupyterCadDoc, MapChange>(this);
   private _objectsChanged = new Signal<IJupyterCadDoc, IJcadObjectDocChange>(
     this
   );
 }
+
+export namespace JupyterCadModel {
+  export interface IOptions
+    extends DocumentRegistry.IModelOptions<IJupyterCadDoc> {
+    annotationModel?: IAnnotationModel;
+  }
+}
```

### Comparing `jupytercad-0.1.0a1/src/tools.ts` & `jupytercad-0.1.0a2/src/tools.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/types.ts` & `jupytercad-0.1.0a2/src/types.ts`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import { DocumentRegistry, IDocumentWidget } from '@jupyterlab/docregistry';
 import { IChangedArgs } from '@jupyterlab/coreutils';
 import { ReactWidget } from '@jupyterlab/ui-components';
 import { User } from '@jupyterlab/services';
 
-import { MapChange, YDocument, StateChange } from '@jupyter/ydoc';
+import {
+  MapChange,
+  YDocument,
+  StateChange,
+  DocumentChange
+} from '@jupyter/ydoc';
 
 import { ISignal, Signal } from '@lumino/signaling';
 import { JSONObject } from '@lumino/coreutils';
 
 import { IJupyterCadTracker } from './token';
 import {
   IJCadContent,
@@ -24,15 +29,14 @@
 
 /**
  * Action definitions for worker
  */
 export enum WorkerAction {
   LOAD_FILE = 'LOAD_FILE',
   SAVE_FILE = 'SAVE_FILE',
-  CLOSE_FILE = 'CLOSE_FILE',
   REGISTER = 'REGISTER'
 }
 
 interface IMainId {
   id: string;
 }
 
@@ -42,27 +46,19 @@
     id: string;
   };
 }
 
 export interface ILoadFile extends IMainId {
   action: WorkerAction.LOAD_FILE;
   payload: {
-    fileName: string;
     content: IJCadContent;
   };
 }
 
-export interface ICloseFile extends IMainId {
-  action: WorkerAction.CLOSE_FILE;
-  payload: {
-    fileName: string;
-  };
-}
-
-export type IWorkerMessage = ILoadFile | IRegister | ICloseFile;
+export type IWorkerMessage = ILoadFile | IRegister;
 
 /**
  * Action definitions for main thread
  */
 export enum MainAction {
   DISPLAY_SHAPE = 'DISPLAY_SHAPE',
   INITIALIZED = 'INITIALIZED'
@@ -135,15 +131,15 @@
   objectChange?: Array<{
     name: string;
     key: string;
     newValue: IJCadObject | undefined;
   }>;
 }
 
-export interface IJupyterCadDocChange {
+export interface IJupyterCadDocChange extends DocumentChange {
   contextChange?: MapChange;
   contentChange?: MapChange;
   objectChange?: Array<{
     name: string;
     key: string;
     newValue: IJCadObject | undefined;
   }>;
@@ -189,15 +185,15 @@
   remoteUser?: number;
   toolbarForm?: IDict;
 }
 
 export interface IJupyterCadModel extends DocumentRegistry.IModel {
   isDisposed: boolean;
   sharedModel: IJupyterCadDoc;
-  annotationModel: IAnnotationModel;
+  annotationModel?: IAnnotationModel;
   localState: IJupyterCadClientState | null;
 
   themeChanged: Signal<
     IJupyterCadModel,
     IChangedArgs<string, string | null, string>
   >;
   clientStateChanged: ISignal<
@@ -221,14 +217,16 @@
     parentType: 'panel' | 'dialog';
   });
 
   getClientId(): number;
 
   addMetadata(key: string, value: string): void;
   removeMetadata(key: string): void;
+
+  disposed: ISignal<any, void>;
 }
 
 export type IJupyterCadWidget = IDocumentWidget<ReactWidget, IJupyterCadModel>;
 
 export interface IControlPanelModel {
   disconnect(f: any): void;
   documentChanged: ISignal<IJupyterCadTracker, IJupyterCadWidget | null>;
```

### Comparing `jupytercad-0.1.0a1/src/widget.tsx` & `jupytercad-0.1.0a2/src/widget.tsx`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-import * as React from 'react';
-
 import { ReactWidget } from '@jupyterlab/apputils';
-import { ObservableMap, IObservableMap } from '@jupyterlab/observables';
-import { DocumentRegistry, DocumentWidget } from '@jupyterlab/docregistry';
-
+import { DocumentWidget } from '@jupyterlab/docregistry';
+import { IObservableMap, ObservableMap } from '@jupyterlab/observables';
+import { JSONValue } from '@lumino/coreutils';
 import { ISignal, Signal } from '@lumino/signaling';
+import * as React from 'react';
 
 import { MainView } from './mainview';
-import { JupyterCadModel } from './model';
 import {
   AxeHelper,
   ExplodedView,
   IJupyterCadModel,
   IJupyterCadWidget
 } from './types';
-import { JSONValue } from '@lumino/coreutils';
 
 export class JupyterCadWidget
-  extends DocumentWidget<JupyterCadPanel, JupyterCadModel>
+  extends DocumentWidget<JupyterCadPanel, IJupyterCadModel>
   implements IJupyterCadWidget
 {
   constructor(
-    options: DocumentWidget.IOptions<JupyterCadPanel, JupyterCadModel>
+    options: DocumentWidget.IOptions<JupyterCadPanel, IJupyterCadModel>
   ) {
     super(options);
   }
 
   /**
    * Dispose of the resources held by the widget.
    */
@@ -41,18 +38,18 @@
 
 export class JupyterCadPanel extends ReactWidget {
   /**
    * Construct a `ExamplePanel`.
    *
    * @param context - The documents context.
    */
-  constructor(context: DocumentRegistry.IContext<IJupyterCadModel>) {
+  constructor(options: { model: IJupyterCadModel }) {
     super();
     this.addClass('jp-jupytercad-panel');
-    this._context = context;
+    this._jcadModel = options.model;
 
     this._view = new ObservableMap<JSONValue>();
   }
 
   get viewChanged(): ISignal<
     ObservableMap<JSONValue>,
     IObservableMap.IChangedArgs<JSONValue>
@@ -88,13 +85,13 @@
   }
 
   deleteAxes(): void {
     this._view.delete('axes');
   }
 
   render(): JSX.Element {
-    return <MainView view={this._view} context={this._context} />;
+    return <MainView view={this._view} jcadModel={this._jcadModel} />;
   }
 
   private _view: ObservableMap<JSONValue>;
-  private _context: DocumentRegistry.IContext<IJupyterCadModel>;
+  private _jcadModel: IJupyterCadModel;
 }
```

### Comparing `jupytercad-0.1.0a1/src/annotation/message.tsx` & `jupytercad-0.1.0a2/src/annotation/message.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/annotation/model.ts` & `jupytercad-0.1.0a2/src/annotation/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/annotation/view.tsx` & `jupytercad-0.1.0a2/src/annotation/view.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/fcplugin/modelfactory.ts` & `jupytercad-0.1.0a2/src/fcplugin/modelfactory.ts`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import { DocumentRegistry } from '@jupyterlab/docregistry';
 import { Contents } from '@jupyterlab/services';
 
-import { IAnnotationModel } from '../types';
+import { IAnnotationModel, IJupyterCadDoc } from '../types';
 import { JupyterCadModel } from '../model';
 
 /**
  * A Model factory to create new instances of JupyterCadModel.
  */
 export class JupyterCadFCModelFactory
   implements DocumentRegistry.IModelFactory<JupyterCadModel>
 {
   constructor(options: JupyterCadFCModelFactory.IOptions) {
     this._annotationModel = options.annotationModel;
   }
 
   /**
+   * Whether the model is collaborative or not.
+   */
+  readonly collaborative = true;
+
+  /**
    * The name of the model.
    *
    * @returns The name
    */
   get name(): string {
     return 'jupytercad-fcmodel';
   }
@@ -66,26 +71,25 @@
   preferredLanguage(path: string): string {
     return '';
   }
 
   /**
    * Create a new instance of JupyterCadModel.
    *
-   * @param languagePreference Language
-   * @param modelDB Model database
    * @returns The model
    */
   createNew(
-    languagePreference?: string | undefined,
-    collaborationEnabled?: boolean | undefined
+    options: DocumentRegistry.IModelOptions<IJupyterCadDoc>
   ): JupyterCadModel {
-    const model = new JupyterCadModel(
-      this._annotationModel,
-      languagePreference
-    );
+    console.debug('[JupyterCadFCModelFactory.createNew] options:', options);
+    const model = new JupyterCadModel({
+      sharedModel: options.sharedModel,
+      languagePreference: options.languagePreference,
+      annotationModel: this._annotationModel
+    });
     return model;
   }
 
   private _annotationModel: IAnnotationModel;
   private _disposed = false;
 }
```

### Comparing `jupytercad-0.1.0a1/src/fcplugin/plugins.ts` & `jupytercad-0.1.0a2/src/fcplugin/plugins.ts`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,24 @@
 
 import { fileIcon } from '@jupyterlab/ui-components';
 
 import { IFileBrowserFactory } from '@jupyterlab/filebrowser';
 
 import { ILauncher } from '@jupyterlab/launcher';
 
+import {
+  ICollaborativeDrive,
+  SharedDocumentFactory
+} from '@jupyter/docprovider';
+
 import { JupyterCadWidgetFactory } from '../factory';
 import { IAnnotation, IJupyterCadDocTracker } from './../token';
 import { JupyterCadFCModelFactory } from './modelfactory';
 import { IAnnotationModel, IJupyterCadWidget } from '../types';
+import { JupyterCadDoc } from '../model';
 
 const FACTORY = 'Jupytercad Freecad Factory';
 
 // const PALETTE_CATEGORY = 'JupyterCAD';
 
 namespace CommandIDs {
   export const createNew = 'jupytercad:create-new-FCStd-file';
@@ -30,14 +36,15 @@
 
 const activate = (
   app: JupyterFrontEnd,
   tracker: WidgetTracker<IJupyterCadWidget>,
   themeManager: IThemeManager,
   annotationModel: IAnnotationModel,
   browserFactory: IFileBrowserFactory,
+  drive: ICollaborativeDrive,
   launcher: ILauncher | null,
   palette: ICommandPalette | null
 ): void => {
   // Creating the widget factory to register it so the document manager knows about
   // our new DocumentWidget
   const widgetFactory = new JupyterCadWidgetFactory({
     name: FACTORY,
@@ -60,14 +67,22 @@
     displayName: 'FCStd',
     mimeTypes: ['application/octet-stream'],
     extensions: ['.FCStd', 'fcstd'],
     fileFormat: 'base64',
     contentType: 'FCStd'
   });
 
+  const FCStdSharedModelFactory: SharedDocumentFactory = () => {
+    return new JupyterCadDoc();
+  };
+  drive.sharedModelFactory.registerDocumentFactory(
+    'FCStd',
+    FCStdSharedModelFactory
+  );
+
   widgetFactory.widgetCreated.connect((sender, widget) => {
     // Notify the instance tracker if restore data needs to update.
     widget.context.pathChanged.connect(() => {
       tracker.save(widget);
     });
     themeManager.themeChanged.connect((_, changes) =>
       widget.context.model.themeChanged.emit(changes)
@@ -132,15 +147,16 @@
 
 const fcplugin: JupyterFrontEndPlugin<void> = {
   id: 'jupytercad:fcplugin',
   requires: [
     IJupyterCadDocTracker,
     IThemeManager,
     IAnnotation,
-    IFileBrowserFactory
+    IFileBrowserFactory,
+    ICollaborativeDrive
   ],
   optional: [ILauncher, ICommandPalette],
   autoStart: true,
   activate
 };
 
 export default fcplugin;
```

### Comparing `jupytercad-0.1.0a1/src/jcadplugin/modelfactory.ts` & `jupytercad-0.1.0a2/src/jcadplugin/modelfactory.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import { DocumentRegistry } from '@jupyterlab/docregistry';
 import { Contents } from '@jupyterlab/services';
 
-import { IAnnotationModel } from '../types';
+import { IAnnotationModel, IJupyterCadDoc } from '../types';
 import { JupyterCadModel } from '../model';
 
 /**
  * A Model factory to create new instances of JupyterCadModel.
  */
 export class JupyterCadJcadModelFactory
   implements DocumentRegistry.IModelFactory<JupyterCadModel>
 {
   constructor(options: JupyterCadJcadModelFactory.IOptions) {
     this._annotationModel = options.annotationModel;
   }
 
   /**
+   * Whether the model is collaborative or not.
+   */
+  readonly collaborative = true;
+
+  /**
    * The name of the model.
    *
    * @returns The name
    */
   get name(): string {
     return 'jupytercad-jcadmodel';
   }
@@ -66,26 +71,24 @@
   preferredLanguage(path: string): string {
     return '';
   }
 
   /**
    * Create a new instance of JupyterCadModel.
    *
-   * @param languagePreference Language
-   * @param modelDB Model database
    * @returns The model
    */
   createNew(
-    languagePreference?: string | undefined,
-    collaborationEnabled?: boolean | undefined
+    options: DocumentRegistry.IModelOptions<IJupyterCadDoc>
   ): JupyterCadModel {
-    const model = new JupyterCadModel(
-      this._annotationModel,
-      languagePreference
-    );
+    const model = new JupyterCadModel({
+      sharedModel: options.sharedModel,
+      languagePreference: options.languagePreference,
+      annotationModel: this._annotationModel
+    });
     return model;
   }
 
   private _annotationModel: IAnnotationModel;
   private _disposed = false;
 }
```

### Comparing `jupytercad-0.1.0a1/src/jcadplugin/plugins.ts` & `jupytercad-0.1.0a2/src/jcadplugin/plugins.ts`

 * *Files 6% similar despite different names*

```diff
@@ -11,32 +11,39 @@
 
 import { fileIcon } from '@jupyterlab/ui-components';
 
 import { IFileBrowserFactory } from '@jupyterlab/filebrowser';
 
 import { ILauncher } from '@jupyterlab/launcher';
 
+import {
+  ICollaborativeDrive,
+  SharedDocumentFactory
+} from '@jupyter/docprovider';
+
 import { IAnnotationModel, IJupyterCadWidget } from './../types';
 import { IAnnotation, IJupyterCadDocTracker } from './../token';
 import { JupyterCadWidgetFactory } from '../factory';
 import { JupyterCadJcadModelFactory } from './modelfactory';
+import { JupyterCadDoc } from '../model';
 
 const FACTORY = 'Jupytercad Jcad Factory';
 const PALETTE_CATEGORY = 'JupyterCAD';
 
 namespace CommandIDs {
   export const createNew = 'jupytercad:create-new-jcad-file';
 }
 
 const activate = (
   app: JupyterFrontEnd,
   tracker: WidgetTracker<IJupyterCadWidget>,
   themeManager: IThemeManager,
   annotationModel: IAnnotationModel,
   browserFactory: IFileBrowserFactory,
+  drive: ICollaborativeDrive,
   launcher: ILauncher | null,
   palette: ICommandPalette | null
 ): void => {
   const widgetFactory = new JupyterCadWidgetFactory({
     name: FACTORY,
     modelName: 'jupytercad-jcadmodel',
     fileTypes: ['jcad'],
@@ -57,14 +64,22 @@
     displayName: 'JCAD',
     mimeTypes: ['text/json'],
     extensions: ['.jcad', '.JCAD'],
     fileFormat: 'text',
     contentType: 'jcad'
   });
 
+  const jcadSharedModelFactory: SharedDocumentFactory = () => {
+    return new JupyterCadDoc();
+  };
+  drive.sharedModelFactory.registerDocumentFactory(
+    'jcad',
+    jcadSharedModelFactory
+  );
+
   widgetFactory.widgetCreated.connect((sender, widget) => {
     widget.context.pathChanged.connect(() => {
       tracker.save(widget);
     });
     themeManager.themeChanged.connect((_, changes) =>
       widget.context.model.themeChanged.emit(changes)
     );
@@ -127,15 +142,16 @@
 
 const jcadPlugin: JupyterFrontEndPlugin<void> = {
   id: 'jupytercad:jcadplugin',
   requires: [
     IJupyterCadDocTracker,
     IThemeManager,
     IAnnotation,
-    IFileBrowserFactory
+    IFileBrowserFactory,
+    ICollaborativeDrive
   ],
   optional: [ILauncher, ICommandPalette],
   autoStart: true,
   activate
 };
 
 export default jcadPlugin;
```

### Comparing `jupytercad-0.1.0a1/src/panelview/annotations.tsx` & `jupytercad-0.1.0a2/src/panelview/annotations.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/panelview/formbuilder.tsx` & `jupytercad-0.1.0a2/src/panelview/formbuilder.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import * as React from 'react';
-import { ISubmitEvent } from '@rjsf/core';
-import { Widget } from '@lumino/widgets';
 import { SchemaForm } from '@deathbeds/jupyterlab-rjsf';
+import { MessageLoop } from '@lumino/messaging';
+import { Widget } from '@lumino/widgets';
+import { ISubmitEvent } from '@rjsf/core';
+import * as React from 'react';
 
 import { IDict } from '../types';
 
 interface IStates {
   internalData?: IDict;
   schema?: IDict;
 }
@@ -29,15 +30,17 @@
   props: React.PropsWithChildren<any>
 ): JSX.Element => {
   const ref = React.useRef<HTMLDivElement>(null);
   const { children } = props;
   React.useEffect(() => {
     const widget = children as SchemaForm;
     try {
-      Widget.attach(widget, ref.current!);
+      MessageLoop.sendMessage(widget, Widget.Msg.BeforeAttach);
+      ref.current!.insertBefore(widget.node, null);
+      MessageLoop.sendMessage(widget, Widget.Msg.AfterAttach);
     } catch (e) {
       console.warn('Exception while attaching Lumino widget.', e);
     }
     return () => {
       try {
         if (widget.isAttached || widget.node.isConnected) {
           Widget.detach(widget);
```

### Comparing `jupytercad-0.1.0a1/src/panelview/leftpanel.tsx` & `jupytercad-0.1.0a2/src/panelview/leftpanel.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/panelview/model.ts` & `jupytercad-0.1.0a2/src/panelview/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/panelview/objectproperties.tsx` & `jupytercad-0.1.0a2/src/panelview/objectproperties.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/panelview/objecttree.tsx` & `jupytercad-0.1.0a2/src/panelview/objecttree.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/panelview/rightpanel.tsx` & `jupytercad-0.1.0a2/src/panelview/rightpanel.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/box.json` & `jupytercad-0.1.0a2/src/schema/box.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/cone.json` & `jupytercad-0.1.0a2/src/schema/cone.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/cut.json` & `jupytercad-0.1.0a2/src/schema/cut.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/cylinder.json` & `jupytercad-0.1.0a2/src/schema/cylinder.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/extrusion.json` & `jupytercad-0.1.0a2/src/schema/extrusion.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/fuse.json` & `jupytercad-0.1.0a2/src/schema/fuse.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/geomCircle.json` & `jupytercad-0.1.0a2/src/schema/geomCircle.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/geomLineSegment.json` & `jupytercad-0.1.0a2/src/schema/geomLineSegment.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/intersection.json` & `jupytercad-0.1.0a2/src/schema/intersection.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/jcad.json` & `jupytercad-0.1.0a2/src/schema/jcad.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/placement.json` & `jupytercad-0.1.0a2/src/schema/placement.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/sketch.json` & `jupytercad-0.1.0a2/src/schema/sketch.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/sphere.json` & `jupytercad-0.1.0a2/src/schema/sphere.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/schema/torus.json` & `jupytercad-0.1.0a2/src/schema/torus.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/sketcher/helper.tsx` & `jupytercad-0.1.0a2/src/sketcher/helper.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/sketcher/panzoom.ts` & `jupytercad-0.1.0a2/src/sketcher/panzoom.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/sketcher/sketcherdialog.tsx` & `jupytercad-0.1.0a2/src/sketcher/sketcherdialog.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/sketcher/sketchermodel.ts` & `jupytercad-0.1.0a2/src/sketcher/sketchermodel.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/sketcher/sketcherwidget.tsx` & `jupytercad-0.1.0a2/src/sketcher/sketcherwidget.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/sketcher/types.ts` & `jupytercad-0.1.0a2/src/sketcher/types.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/sketcher/elements/line.ts` & `jupytercad-0.1.0a2/src/sketcher/elements/line.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/toolbar/formdialog.tsx` & `jupytercad-0.1.0a2/src/toolbar/formdialog.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/toolbar/helpertoolbar.tsx` & `jupytercad-0.1.0a2/src/toolbar/helpertoolbar.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/toolbar/model.ts` & `jupytercad-0.1.0a2/src/toolbar/model.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import { Signal, ISignal } from '@lumino/signaling';
 import { IJCadModel } from './../_interface/jcad.d';
 import { IDict, IJupyterCadModel } from './../types';
 import { DocumentRegistry } from '@jupyterlab/docregistry';
 import formSchema from '../_interface/forms.json';
 import { IJupyterCadDoc } from '../types';
-import { JupyterCadModel } from './../model';
 import { User } from '@jupyterlab/services';
 import { JupyterCadPanel } from '../widget';
 
 export interface IUserData {
   userId: number;
   userData: User.IIdentity;
 }
@@ -112,21 +111,21 @@
         Name: { type: 'string', description: 'The name of object' },
         ...value['properties']
       };
     });
   }
 
   private _panel: JupyterCadPanel;
-  private _context: DocumentRegistry.IContext<JupyterCadModel>;
+  private _context: DocumentRegistry.IContext<IJupyterCadModel>;
   private _sharedModel?: IJupyterCadDoc;
   private _formSchema = JSON.parse(JSON.stringify(formSchema));
   private _userChanged = new Signal<this, IUserData[]>(this);
   private _usersMap?: Map<number, any>;
   private _filePath?: string;
 }
 
 export namespace ToolbarModel {
   export interface IOptions {
     panel: JupyterCadPanel;
-    context: DocumentRegistry.IContext<JupyterCadModel>;
+    context: DocumentRegistry.IContext<IJupyterCadModel>;
   }
 }
```

### Comparing `jupytercad-0.1.0a1/src/toolbar/operatortoolbar.tsx` & `jupytercad-0.1.0a2/src/toolbar/operatortoolbar.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/toolbar/parttoolbar.tsx` & `jupytercad-0.1.0a2/src/toolbar/parttoolbar.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,17 @@
       }
     },
     CONE: {
       title: 'Cone parameters',
       shape: 'Part::Cone',
       schema: this.props.toolbarModel.formSchema['Part::Cone'],
       default: {
-        Radius1: 5,
-        Radius2: 4,
-        Height: 10,
+        Radius1: 1,
+        Radius2: 0.5,
+        Height: 1,
         Angle: 360,
         Placement: { Position: [0, 0, 0], Axis: [0, 0, 1], Angle: 0 }
       }
     },
     TORUS: {
       title: 'Torus parameters',
       shape: 'Part::Torus',
```

### Comparing `jupytercad-0.1.0a1/src/toolbar/sketchertoolbar.tsx` & `jupytercad-0.1.0a2/src/toolbar/sketchertoolbar.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/toolbar/toolbar.tsx` & `jupytercad-0.1.0a2/src/toolbar/toolbar.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,18 @@
             onChange={e =>
               this.setState(old => ({
                 ...old,
                 selected: e.target.value as any
               }))
             }
           >
-            {this._toolbarOption.map(value => (
-              <option value={value}>{value}</option>
+            {this._toolbarOption.map((value, idx) => (
+              <option key={idx} value={value}>
+                {value}
+              </option>
             ))}
           </select>
           <span>
             <svg
               style={{
                 height: 'auto',
                 position: 'absolute',
@@ -93,15 +95,15 @@
               viewBox="0 0 18 18"
               data-icon="ui-components:caret-down-empty"
             >
               <g
                 xmlns="http://www.w3.org/2000/svg"
                 className="jp-icon3"
                 fill="#616161"
-                shape-rendering="geometricPrecision"
+                shapeRendering="geometricPrecision"
               >
                 <path d="M5.2,5.9L9,9.7l3.8-3.8l1.2,1.2l-4.9,5l-4.9-5L5.2,5.9z"></path>
               </g>
             </svg>
           </span>
         </div>
         {this.state.selected === 'PART' && (
```

### Comparing `jupytercad-0.1.0a1/src/toolbar/usertoolbar.tsx` & `jupytercad-0.1.0a2/src/toolbar/usertoolbar.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/toolbar/widget.tsx` & `jupytercad-0.1.0a2/src/toolbar/widget.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -15,47 +15,48 @@
 
 export class ToolbarWidget extends Toolbar {
   constructor(options: ToolbarWidget.IOptions) {
     const { model, ...rest } = options;
     super(rest);
     this.addClass('jpcad-toolbar-widget');
     this._model = model;
-
-    this.addItem(
-      'undo',
-      new CommandToolbarButton({
-        id: ToolbarWidget.CommandIDs.undo,
-        label: '',
-        icon: undoIcon,
-        commands: options.commands
-      })
-    );
-    this.addItem(
-      'redo',
-      new CommandToolbarButton({
-        id: ToolbarWidget.CommandIDs.redo,
-        label: '',
-        icon: redoIcon,
-        commands: options.commands
-      })
-    );
+    if (options.commands) {
+      this.addItem(
+        'undo',
+        new CommandToolbarButton({
+          id: ToolbarWidget.CommandIDs.undo,
+          label: '',
+          icon: undoIcon,
+          commands: options.commands
+        })
+      );
+      this.addItem(
+        'redo',
+        new CommandToolbarButton({
+          id: ToolbarWidget.CommandIDs.redo,
+          label: '',
+          icon: redoIcon,
+          commands: options.commands
+        })
+      );
+    }
 
     const body = ReactWidget.create(
       <ToolbarReact toolbarModel={this._model} />
     );
     this.addItem('body', body);
   }
 
   private _model: ToolbarModel;
 }
 
 export namespace ToolbarWidget {
   export interface IOptions extends Toolbar.IOptions {
     model: ToolbarModel;
-    commands: CommandRegistry;
+    commands?: CommandRegistry;
   }
 
   /**
    * The command IDs used by the FreeCAD plugin.
    */
   export namespace CommandIDs {
     export const redo = 'jupytercad:redo';
```

### Comparing `jupytercad-0.1.0a1/src/worker/actions.ts` & `jupytercad-0.1.0a2/src/worker/actions.ts`

 * *Files 0% similar despite different names*

```diff
@@ -217,18 +217,15 @@
         occShapes.push({ occShape, jcObject: object });
       }
     }
   });
   return occShapes;
 }
 
-function loadFile(payload: {
-  fileName: string;
-  content: IJCadContent;
-}): IDict | null {
+function loadFile(payload: { content: IJCadContent }): IDict | null {
   const { content } = payload;
   const shapeList = buildModel(content);
   const parser = new OccParser(shapeList);
   const result = parser.execute();
   return result;
 }
```

### Comparing `jupytercad-0.1.0a1/src/worker/occapi.ts` & `jupytercad-0.1.0a2/src/worker/occapi.ts`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,16 @@
       content
     );
     const tool = ShapesFactory[toolShape](
       toolObject[0].parameters as IOperatorArg,
       content
     );
     if (base && tool) {
+      baseObject[0].visible = false;
+      toolObject[0].visible = false;
       const operator = new oc.BRepAlgoAPI_Cut_3(base, tool);
       if (operator.IsDone()) {
         return setShapePlacement(operator.Shape(), Placement);
       }
     }
   }
 }
@@ -170,14 +172,15 @@
     const baseShape = baseObject[0].shape;
     if (baseShape && ShapesFactory[baseShape]) {
       const base = ShapesFactory[baseShape](
         baseObject[0].parameters as IOperatorArg,
         content
       );
       occShapes.push(base);
+      baseObject[0].visible = false;
     }
   });
   const operator = new oc.BRepAlgoAPI_Fuse_3(occShapes[0], occShapes[1]);
   if (operator.IsDone()) {
     return setShapePlacement(operator.Shape(), Placement);
   }
   return;
@@ -198,14 +201,15 @@
     const baseShape = baseObject[0].shape;
     if (baseShape && ShapesFactory[baseShape]) {
       const base = ShapesFactory[baseShape](
         baseObject[0].parameters as IOperatorArg,
         content
       );
       occShapes.push(base);
+      baseObject[0].visible = false;
     }
   });
   const operator = new oc.BRepAlgoAPI_Common_3(occShapes[0], occShapes[1]);
   if (operator.IsDone()) {
     return setShapePlacement(operator.Shape(), Placement);
   }
   return;
```

### Comparing `jupytercad-0.1.0a1/src/worker/occparser.ts` & `jupytercad-0.1.0a2/src/worker/occparser.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import { IDict } from './../types';
 import {
   Handle_Poly_Triangulation,
   OpenCascadeInstance,
   TopoDS_Shape
 } from 'jupytercad-opencascade';
 
 import { IJCadObject } from '../_interface/jcad.d';
@@ -21,14 +22,15 @@
   }
 
   execute(): {
     [key: string]: {
       jcObject: IJCadObject;
       faceList: Array<IFace>;
       edgeList: Array<IEdge>;
+      guiData?: IDict;
     };
   } {
     const maxDeviation = 0.1;
     const theejsData: {
       [key: string]: {
         jcObject: IJCadObject;
         faceList: Array<IFace>;
```

### Comparing `jupytercad-0.1.0a1/src/worker/types.ts` & `jupytercad-0.1.0a2/src/worker/types.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/src/worker/worker.ts` & `jupytercad-0.1.0a2/src/worker/worker.ts`

 * *Files 3% similar despite different names*

```diff
@@ -51,12 +51,9 @@
           action: MainAction.DISPLAY_SHAPE,
           payload: result
         },
         id
       );
       break;
     }
-    case WorkerAction.CLOSE_FILE: {
-      break;
-    }
   }
 };
```

### Comparing `jupytercad-0.1.0a1/src/worker/geometry/geomCircle.ts` & `jupytercad-0.1.0a2/src/worker/geometry/geomCircle.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/style/base.css` & `jupytercad-0.1.0a2/style/base.css`

 * *Files 6% similar despite different names*

```diff
@@ -370,7 +370,15 @@
   right: 5px;
   font-size: var(--jp-ui-font-size0);
 }
 
 .highlight {
   background-color: var(--jp-layout-color2) !important;
 }
+.mimerenderer-jupytercad {
+  height: 600px;
+  width: 100%;
+}
+.mimerenderer-jupytercad > div {
+  height: 100%;
+  width: 100%;
+}
```

### Comparing `jupytercad-0.1.0a1/style/icon/jvcontrol.svg` & `jupytercad-0.1.0a2/style/icon/jvcontrol.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/style/icon/visibility.svg` & `jupytercad-0.1.0a2/style/icon/visibility.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/style/icon/visibilityOff.svg` & `jupytercad-0.1.0a2/style/icon/visibilityOff.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/ui-tests/tests/sketcher.spec.ts` & `jupytercad-0.1.0a2/ui-tests/tests/sketcher.spec.ts`

 * *Files 0% similar despite different names*

```diff
@@ -66,24 +66,24 @@
       .click();
 
     await page.getByRole('combobox').selectOption('SKETCHER');
     await page.getByRole('button', { name: 'NEW' }).click();
     await page.getByRole('button', { name: 'CIRCLE' }).click();
     await page
       .locator('canvas')
-      .nth(3)
+      .nth(1)
       .click({
         position: {
           x: 455,
           y: 209
         }
       });
     await page
       .locator('canvas')
-      .nth(3)
+      .nth(1)
       .click({
         position: {
           x: 455,
           y: 335
         }
       });
     const dialog = await page.$('.lm-Widget.lm-Panel.jp-Dialog-content');
```

### Comparing `jupytercad-0.1.0a1/ui-tests/tests/tree.spec.ts` & `jupytercad-0.1.0a2/ui-tests/tests/tree.spec.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts` & `jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
       const content = galata.newContentsHelper(request);
       await content.deleteDirectory('/examples');
       await content.uploadDirectory(
         path.resolve(__dirname, '../../examples'),
         '/examples'
       );
     });
-
     let errors = 0;
     test.beforeEach(async ({ page }) => {
       page.setViewportSize({ width: 1920, height: 1080 });
       page.on('console', message => {
         if (message.type() === 'error') {
           errors += 1;
         }
```

### Comparing `jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Operator-Add-example2-FCStd-linux.png` & `jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Operator-Add-example2-FCStd-linux.png`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Operator-Edit-example4-FCStd-linux.png` & `jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Operator-Edit-example4-FCStd-linux.png`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-example-2D-FCStd-linux.png` & `jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-example-2D-FCStd-linux.png`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-example2-FCStd-linux.png` & `jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-example2-FCStd-linux.png`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-example4-FCStd-linux.png` & `jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-example4-FCStd-linux.png`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-example5-FCStd-linux.png` & `jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-example5-FCStd-linux.png`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-example6-FCStd-linux.png` & `jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-example6-FCStd-linux.png`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/ui-tests/tests/ui.spec.ts-snapshots/Render-test-jcad-linux.png` & `jupytercad-0.1.0a2/ui-tests/tests/ui.spec.ts-snapshots/Render-test-jcad-linux.png`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/.gitignore` & `jupytercad-0.1.0a2/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -116,8 +116,15 @@
 src/_interface/
 *.db
 
 # Integration tests
 ui-tests/test-results/
 ui-tests/playwright-report/
 
-examples/*.ipynb
+examples/*.ipynb
+# Hatchling
+jupytercad/_version.py
+
+#Schema
+jupytercad/notebook/objects/_schema
+
+.yarn
```

### Comparing `jupytercad-0.1.0a1/LICENSE` & `jupytercad-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0a1/README.md` & `jupytercad-0.1.0a2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 JupyterCAD has support for FreeCAD files, which makes it easy to import and export models from FreeCAD. It also has a range of features for creating and manipulating 3D shapes, including a variety of primitives, transformations, and Boolean operations.
 
 ![jupytercad](./jupytercad-screenshot.png)
 
 ## Requirements
 
-- JupyterLab == 4.0.0a32
+- JupyterLab >= 4.0.0b0
 - freecad (optional)
 
 ## Installation
 
 You can install JupyterCAD using pip:
 
 ```bash
```

### Comparing `jupytercad-0.1.0a1/pyproject.toml` & `jupytercad-0.1.0a2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 [build-system]
 build-backend = "hatchling.build"
-requires = ["hatchling>=1.4.0", "hatch-nodejs-version", "jupyterlab==4.0.0a32"]
+requires = [
+    "hatchling>=1.4.0",
+    "hatch-nodejs-version",
+    "jupyterlab>=4.0.0b0",
+    "datamodel-code-generator",
+]
+
 
 [project]
 name = "jupytercad"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
-    "jupyterlab==4.0.0a32",
+    "jupyterlab>=4.0.0b0",
     "jupyter_server>=2.0.6",
-    "jupyter_ydoc>=0.2.0,<0.3.0"
+    "jupyter_collaboration>=1.0.0a7,<2",
+    "ypywidgets>=0.1.2,<0.2.0",
+    "comm>=0.1.2,<0.2.0"
 ]
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
@@ -48,15 +56,18 @@
 
 [tool.hatch.build.hooks.version]
 path = "jupytercad/_version.py"
 
 [tool.hatch.build.hooks.jupyter-builder]
 dependencies = ["hatch-jupyter-builder>=0.5"]
 build-function = "hatch_jupyter_builder.npm_builder"
-ensured-targets = ["jupytercad/labextension/static/style.js", "jupytercad/labextension/package.json"]
+ensured-targets = [
+    "jupytercad/labextension/static/style.js",
+    "jupytercad/labextension/package.json",
+]
 skip-if-exists = ["jupytercad/labextension/static/style.js"]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 build_cmd = "build:prod"
 npm = ["jlpm"]
 
 [tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
@@ -65,12 +76,16 @@
 source_dir = "src"
 build_dir = "jupytercad/labextension"
 
 [tool.jupyter-releaser.options]
 version-cmd = "python scripts/bump-version.py"
 
 [tool.jupyter-releaser.hooks]
-before-build-npm = ["python -m pip install jupyterlab --pre -U", "jlpm", "jlpm build:prod"]
+before-build-npm = [
+    "python -m pip install datamodel-code-generator jupyterlab --pre -U",
+    "jlpm",
+    "jlpm build:prod",
+]
 before-build-python = ["jlpm clean:all"]
 
 [tool.check-wheel-contents]
 ignore = ["W002"]
```

### Comparing `jupytercad-0.1.0a1/PKG-INFO` & `jupytercad-0.1.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercad
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A JupyterLab extension for 3D modelling.
 Project-URL: Homepage, https://github.com/QuantStack/jupytercad
 Project-URL: Bug Tracker, https://github.com/QuantStack/jupytercad/issues
 Project-URL: Repository, https://github.com/QuantStack/jupytercad.git
 Author-email: Trung Le <leductrungxf@gmail.com>
 License: BSD 3-Clause License
         
@@ -45,32 +45,34 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
+Requires-Dist: comm<0.2.0,>=0.1.2
+Requires-Dist: jupyter-collaboration<2,>=1.0.0a7
 Requires-Dist: jupyter-server>=2.0.6
-Requires-Dist: jupyter-ydoc<0.3.0,>=0.2.0
-Requires-Dist: jupyterlab==4.0.0a32
+Requires-Dist: jupyterlab>=4.0.0b0
+Requires-Dist: ypywidgets<0.2.0,>=0.1.2
 Description-Content-Type: text/markdown
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/QuantStack/jupytercad/main?labpath=lab)
 
 # JupyterCAD - A JupyterLab extension for 3D geometry modeling.
 
 JupyterCAD is a JupyterLab extension for 3D geometry modeling with collaborative editing support. It is designed to allow multiple people to work on the same file at the same time, and to facilitate discussion and collaboration around the 3D shapes being created.
 
 JupyterCAD has support for FreeCAD files, which makes it easy to import and export models from FreeCAD. It also has a range of features for creating and manipulating 3D shapes, including a variety of primitives, transformations, and Boolean operations.
 
 ![jupytercad](./jupytercad-screenshot.png)
 
 ## Requirements
 
-- JupyterLab == 4.0.0a32
+- JupyterLab >= 4.0.0b0
 - freecad (optional)
 
 ## Installation
 
 You can install JupyterCAD using pip:
 
 ```bash
```

